# Comparing `tmp/hydrusvideodeduplicator-0.2.3.tar.gz` & `tmp/hydrusvideodeduplicator-0.2.4.tar.gz`

## Comparing `hydrusvideodeduplicator-0.2.3.tar` & `hydrusvideodeduplicator-0.2.4.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/Dockerfile
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/docker-compose.yml
--rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/docker-entrypoint.sh
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/__init__.py
--rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/__main__.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/config.py
--rw-r--r--   0        0        0    17840 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/dedup.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/dedup_util.py
--rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/LICENSE
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/README.md
--rw-r--r--   0        0        0    36873 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/__init__.py
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/utils.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/__init__.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/hasher/__init__.py
--rw-r--r--   0        0        0    23841 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tests/__init__.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tests/matrix_test.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tools/__init__.py
--rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/types/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/types/containers.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/types/exceptions.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/utils/__init__.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/vpdqpy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/vpdqpy/__main__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/vpdqpy/typing_utils.py
--rw-r--r--   0        0        0     7086 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/LICENSE
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/README.md
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/Dockerfile
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/docker-compose.yml
+-rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/docker-entrypoint.sh
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/.vscode/settings.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/__init__.py
+-rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/__main__.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/config.py
+-rw-r--r--   0        0        0    20971 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/dedup.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/dedup_util.py
+-rw-r--r--   0        0        0    34519 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/hydrus_api/LICENSE
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/hydrus_api/README.md
+-rw-r--r--   0        0        0    36865 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/hydrus_api/__init__.py
+-rw-r--r--   0        0        0     5290 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/hydrus_api/utils.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/__init__.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/hasher/__init__.py
+-rw-r--r--   0        0        0    23627 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/tests/__init__.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/tests/matrix_test.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/tools/__init__.py
+-rw-r--r--   0        0        0    10912 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/types/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/types/containers.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/types/exceptions.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/utils/__init__.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/vpdqpy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/vpdqpy/__main__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/vpdqpy/typing_utils.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/README.md
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 hydrusvideodeduplicator-0.2.4/PKG-INFO
```

### Comparing `hydrusvideodeduplicator-0.2.3/docker-compose.yml` & `hydrusvideodeduplicator-0.2.4/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.3/docker-entrypoint.sh` & `hydrusvideodeduplicator-0.2.4/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/__main__.py` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import typer
 from rich import print as rprint
 
 import hydrusvideodeduplicator.hydrus_api as hydrus_api
 
 from .__about__ import __version__
-from .config import HYDRUS_API_KEY, HYDRUS_API_URL, REQUESTS_CA_BUNDLE, HYDRUS_QUERY, HYDRUS_LOCAL_FILE_SERVICE_KEYS
+from .config import HYDRUS_API_KEY, HYDRUS_API_URL, HYDRUS_LOCAL_FILE_SERVICE_KEYS, HYDRUS_QUERY, REQUESTS_CA_BUNDLE
 from .dedup import HydrusVideoDeduplicator
 
 """
 Parameters:
 - api_key will be read from env var $HYDRUS_API_KEY or .env file
 - api_url will be read from env var $HYDRUS_API_URL or .env file
 - to add custom queries, do
@@ -30,15 +30,17 @@
     query: Annotated[Optional[List[str]], typer.Option(help="Custom Hydrus tag query")] = HYDRUS_QUERY,
     threshold: Annotated[
         Optional[float], typer.Option(help="Similarity threshold for a pair of videos where 100 is identical")
     ] = 75.0,
     skip_hashing: Annotated[
         Optional[bool], typer.Option(help="Skip perceptual hashing and just search for duplicates")
     ] = False,
-    file_service_key: Annotated[Optional[List[str]], typer.Option(help="Local file service key")] = HYDRUS_LOCAL_FILE_SERVICE_KEYS,
+    file_service_key: Annotated[
+        Optional[List[str]], typer.Option(help="Local file service key")
+    ] = HYDRUS_LOCAL_FILE_SERVICE_KEYS,
     verify_cert: Annotated[
         Optional[str], typer.Option(help="Path to TLS cert. This forces verification.")
     ] = REQUESTS_CA_BUNDLE,
     clear_search_cache: Annotated[
         Optional[bool], typer.Option(help="Clear the cache that tracks what files have already been compared")
     ] = False,
     verbose: Annotated[Optional[bool], typer.Option(help="Verbose logging")] = False,
@@ -57,15 +59,14 @@
     # Logs are separate from printing in this program.
     if not verbose:
         logging.disable()
 
     # Clear cache
     if clear_search_cache:
         HydrusVideoDeduplicator.clear_search_cache()
-        rprint("[green] Cleared search cache.")
 
     # CLI overwrites env vars with no default value
     if not api_key:
         api_key = HYDRUS_API_KEY
 
     # Check for necessary variables
     if not api_key:
@@ -133,16 +134,17 @@
         rprint("[red] ERROR: Invalid similarity threshold. Must be between 0 and 100.")
         raise typer.Exit(code=1)
     superdeduper.threshold = threshold
 
     superdeduper.clear_trashed_files_from_db()
 
     # Run all deduplicate functionality
-    superdeduper.deduplicate(overwrite=overwrite, custom_query=query, skip_hashing=skip_hashing,
-                             file_service_keys=file_service_key)
+    superdeduper.deduplicate(
+        overwrite=overwrite, custom_query=query, skip_hashing=skip_hashing, file_service_keys=file_service_key
+    )
 
     raise typer.Exit()
 
 
 try:
     typer.run(main)
 except KeyboardInterrupt as exc:
```

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/config.py` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import json
 import os
 from pathlib import Path
 from platform import uname
-import json
 
 from dotenv import load_dotenv
-from appdirs import AppDirs
+from platformdirs import PlatformDirs
 
 
 class InvalidEnvironmentVariable(Exception):
     """Raise for when environment variables are invalid."""
 
     def __init__(self, msg):
         super().__init__(msg)
@@ -47,15 +47,15 @@
     from socket import gethostname
 
     _DEFAULT_IP = f"{gethostname()}.local"
 
 HYDRUS_API_URL = os.getenv("HYDRUS_API_URL", f"https://{_DEFAULT_IP}:{_DEFAULT_PORT}")
 
 # ~/.local/share/hydrusvideodeduplicator/ on Linux
-_DEDUP_DATABASE_DIR_ENV = AppDirs("hydrusvideodeduplicator").user_data_dir
+_DEDUP_DATABASE_DIR_ENV = PlatformDirs("hydrusvideodeduplicator").user_data_dir
 _DEDUP_DATABASE_DIR_ENV = os.getenv("DEDUP_DATABASE_DIR", _DEDUP_DATABASE_DIR_ENV)
 DEDUP_DATABASE_DIR = Path(_DEDUP_DATABASE_DIR_ENV)
 
 _DEDUP_DATABASE_NAME_ENV = os.getenv("DEDUP_DATABASE_NAME", "videohashes")
 DEDUP_DATABASE_FILE = Path(DEDUP_DATABASE_DIR, f"{_DEDUP_DATABASE_NAME_ENV}.sqlite")
 
 REQUESTS_CA_BUNDLE = os.getenv("REQUESTS_CA_BUNDLE")
```

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/dedup.py` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/dedup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from joblib import Parallel, delayed
 from rich import print as rprint
 from sqlitedict import SqliteDict
 from tqdm import tqdm
 
 if TYPE_CHECKING:
+    from collections.abc import Generator, Iterable, Sequence
     from typing import Any
-    from collections.abc import Iterable, Sequence, Generator
 
 import hydrusvideodeduplicator.hydrus_api as hydrus_api
-import hydrusvideodeduplicator.hydrus_api.utils
+import hydrusvideodeduplicator.hydrus_api.utils as hydrus_api_utils
 
 from .config import DEDUP_DATABASE_DIR, DEDUP_DATABASE_FILE
 from .dedup_util import database_accessible
 from .vpdqpy.vpdqpy import Vpdq
 
 
 class HydrusVideoDeduplicator:
@@ -38,17 +38,20 @@
         # If any of these are large they should probably be lazily loaded
         self.all_services = self.client.get_services()
 
     # Verify client connection and permissions
     # Will throw a hydrus_api.APIError if something is wrong
     def verify_api_connection(self) -> None:
         self.hydlog.info(
-            f"Client API version: v{self.client.VERSION} | Endpoint API version: v{self.client.get_api_version()['version']}"
+            (
+                f"Client API version: v{self.client.VERSION}"
+                "| Endpoint API version: v{self.client.get_api_version()['version']}"
+            )
         )
-        hydrus_api.utils.verify_permissions(self.client, hydrus_api.utils.Permission)
+        hydrus_api_utils.verify_permissions(self.client, hydrus_api.utils.Permission)
 
     # Verify that the supplied file_service_key is a valid key for a local file service
     def verify_file_service_keys(self, file_service_keys: Iterable[str]) -> None:
         VALID_SERVICE_TYPES = [hydrus_api.ServiceType.ALL_LOCAL_FILES, hydrus_api.ServiceType.FILE_DOMAIN]
 
         for file_service_key in file_service_keys:
             file_service = self.all_services['services'].get(file_service_key)
@@ -65,15 +68,19 @@
         overwrite: bool = False,
         custom_query: Sequence[str] | None = None,
         skip_hashing: bool = False,
         file_service_keys: Sequence[str] | None = None,
     ) -> None:
         # Add perceptual hashes to video files
         # system:filetype tags are really inconsistent
-        search_tags = ['system:filetype=video, gif, apng', 'system:has duration']
+        search_tags = [
+            'system:filetype=video, gif, apng',
+            'system:has duration',
+            'system:file service is not currently in trash',
+        ]
 
         query = False
         if custom_query is not None:
             # Remove whitespace and empty strings
             custom_query = [x for x in custom_query if x.strip()]
             if len(custom_query) > 0:
                 search_tags.extend(custom_query)
@@ -136,15 +143,14 @@
             pass
 
         with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
             dblen = len(hashdb)
             dbsize = os.path.getsize(DEDUP_DATABASE_FILE)
 
             if dblen > 0:
-                rprint(f"[blue] Database found with {dblen} videos already hashed.")
                 self.hydlog.info(f"Database found of length {dblen}, size {dbsize} bytes")
             else:
                 self.hydlog.info(f"Database not found. Creating one at {DEDUP_DATABASE_FILE}")
 
             try:
                 with tqdm(total=len(video_hashes), dynamic_ncols=True, unit="video", colour="BLUE") as pbar:
                     count_since_last_commit = 0
@@ -155,16 +161,14 @@
                         # Only calculate new hash if it's missing or if overwrite is true
                         if not overwrite and video_hash in hashdb and "perceptual_hash" in hashdb[video_hash]:
                             continue
 
                         # Get video file from Hydrus
                         try:
                             video_response = self.client.get_file(hash_=video_hash)
-                            # video_metadata = self.client.get_file_metadata(hashes=[video_hash], only_return_basic_information=False)
-                            # print(video_metadata)
                         except hydrus_api.HydrusAPIException:
                             rprint("[red] Failed to get video from Hydrus.")
                             self.hydlog.error("Error getting video from Hydrus.")
                             continue
 
                         # Calculate perceptual_hash
                         try:
@@ -194,14 +198,15 @@
                 self.hydlog.error(interrupt_msg)
 
             else:
                 rprint("[green] Finished perceptual hash processing.")
 
             finally:
                 hashdb.commit()
+                rprint(f"[green] Added {len(hashdb) - dblen} new videos to database.")
                 self.hydlog.info("Finished perceptual hash processing.")
 
     def get_potential_duplicate_count_hydrus(self, file_service_keys: Iterable[str]) -> int:
         return self.client.get_potentials_count(file_service_keys=file_service_keys)["potential_duplicates_count"]
 
     def compare_videos(self, video1_hash: str, video2_hash: str, video1_phash: str, video2_phash: str) -> None:
         vpdq_hash1 = Vpdq.json_to_vpdq(video1_phash)
@@ -220,35 +225,33 @@
                 "hash_b": str(video2_hash),
                 "relationship": int(hydrus_api.DuplicateStatus.POTENTIAL_DUPLICATES),
                 "do_default_content_merge": True,
             }
 
             self.client.set_file_relationships([new_relationship])
 
-    # Delete cache row in database
+    # Delete cache search index value for each video in database
     @staticmethod
     def clear_search_cache() -> None:
-        try:
-            with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
-                for key in hashdb:
-                    row = hashdb[key]
-                    if "farthest_search_index" in row:
-                        del row["farthest_search_index"]
-                    hashdb[key] = row
-                hashdb.commit()
-        except OSError:
-            rprint(f"[red] Database does not exist. Cannot clear search cache.")
+        if not database_accessible(DEDUP_DATABASE_FILE, tablename="videos"):
+            return
+        with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
+            for key in hashdb:
+                row = hashdb[key]
+                if "farthest_search_index" in row:
+                    del row["farthest_search_index"]
+                hashdb[key] = row
+            hashdb.commit()
+        rprint("[green] Cleared search cache.")
 
-    # Sliding window duplicate comparisons
-    # Alternatively, I could scan duplicates when added and never do it again which would be one of the best ways without a VP tree
     def _find_potential_duplicates(
         self, limited_video_hashes: Sequence[str] | None = None, file_service_keys: Iterable[str] | None = None
     ) -> None:
         if not database_accessible(DEDUP_DATABASE_FILE, tablename="videos", verbose=True):
-            rprint(f"[red] Could not search for duplicates.")
+            rprint("[red] Could not search for duplicates.")
             return
 
         # Number of potential duplicates before adding more. Just for user info.
         pre_dedupe_count = self.get_potential_duplicate_count_hydrus(file_service_keys)
 
         # BUG: If this process is interrupted, the farthest_search_index will not save for ANY entries.
         #      I think it might be because every entry in the column needs an entry for SQlite but I'm not sure.
@@ -292,93 +295,169 @@
                                 video_counter += 1
                                 pbar.update(1)
 
                                 row = hashdb[video1_hash]
 
                                 # Store last furthest searched position in the database for each element
                                 # This way you only have to start searching at that place instead of at i+1 if it exists
-                                row.setdefault("farthest_search_index", i + 1)
+                                farthest_search_index = row.setdefault("farthest_search_index", i + 1)
 
-                                # This is not necessary but may increase speed by avoiding any of the code below
-                                if row["farthest_search_index"] >= len(hashdb) - 1:
+                                assert farthest_search_index <= total
+                                if farthest_search_index == total:
+                                    # This file has already been searched for dupes against all other videos in the DB
                                     continue
 
                                 parallel(
                                     delayed(self.compare_videos)(
                                         video1_hash,
                                         video2_hash,
                                         hashdb[video1_hash]["perceptual_hash"],
                                         hashdb[video2_hash]["perceptual_hash"],
                                     )
                                     for video2_hash in islice(hashdb, row["farthest_search_index"], None)
                                 )
 
-                                # Update furthest search position to the current length of the table
-                                row["farthest_search_index"] = len(hashdb) - 1
+                                # Video has now been compared against all other videos for dupes,
+                                # so update farthest_search_index to the current length of the table
+                                row["farthest_search_index"] = total
                                 hashdb[video1_hash] = row
                                 count_since_last_commit += 1
 
                                 if count_since_last_commit >= commit_interval:
                                     hashdb.commit()
                                     count_since_last_commit = 0
 
             except KeyboardInterrupt:
-                pass
+                rprint("[yellow] Duplicate search was interrupted!")
             finally:
                 hashdb.commit()
 
         # Statistics for user
         post_dedupe_count = self.get_potential_duplicate_count_hydrus(file_service_keys)
         new_dedupes_count = post_dedupe_count - pre_dedupe_count
         if new_dedupes_count > 0:
             rprint(f"[green] {new_dedupes_count} new potential duplicates marked for processing!")
         else:
             rprint("[green] No new potential duplicates found.")
 
     @staticmethod
-    def batched(iterable, n) -> Generator[tuple, Any, None]:
-        "Batch data into tuples of length n. The last batch may be shorter."
-        # batched('ABCDEFG', 3) --> ABC DEF G
-        if n < 1:
-            raise ValueError('n must be at least one')
+    def batched(iterable: Iterable, n: int) -> Generator[tuple, Any, None]:
+        """
+        Batch data into tuples of length n. The last batch may be shorter."
+        batched('ABCDEFG', 3) --> ABC DEF G
+        DO NOT use this for iterating over the database. Use batched_and_save_db instead.
+        """
+        assert n >= 1
         it = iter(iterable)
         while batch := tuple(islice(it, n)):
             yield batch
 
-    # Check if files are trashed
-    # Returns a dictionary of hash : trashed_or_not
-    def is_files_trashed_hydrus(self, file_hashes: Iterable[str]) -> dict:
+    @staticmethod
+    def batched_and_save_db(
+        db: SqliteDict,
+        n: int,
+        chunk_size: int | None = None,
+    ) -> Generator[dict[str, dict[str, Any]], Any, None]:
+        """
+        Batch rows of into rows of length n and save changes after each batch or after chunk_size batches.
+        """
+        assert n >= 1
+        assert chunk_size is None or chunk_size >= 1
+        if chunk_size is None:
+            chunk_size = n
+        it = iter(db.items())
+        while batch_items := dict(islice(it, n)):
+            batch_dict = {
+                key: {col: val for col, val in row.items() if col != 'key'} for key, row in batch_items.items()
+            }
+
+            yield batch_dict
+
+            # Save changes after each batch
+            db.commit()
+
+    def is_files_deleted_hydrus(self, file_hashes: Iterable[str]) -> dict[str, bool]:
+        """
+        Check if files are trashed or deleted in Hydrus
+        Returns a dictionary of hash : trashed_or_not
+        """
         videos_metadata = self.client.get_file_metadata(hashes=file_hashes, only_return_basic_information=False)[
             "metadata"
         ]
 
         result = {}
         for video_metadata in videos_metadata:
-            # This should never happen
+            # This should never happen, but it shouldn't break the program if it does
             if "hash" not in video_metadata:
                 logging.error("Hash not found for potentially trashed file.")
                 continue
-            video_hash = video_metadata['hash']
-            is_trashed: bool = video_metadata.get('is_trashed', False)
-            is_deleted: bool = video_metadata.get('is_deleted', False)
-            result[video_hash] = is_trashed or is_deleted
+            video_hash = video_metadata["hash"]
+            is_deleted: bool = video_metadata.get("is_deleted", False)
+            result[video_hash] = is_deleted
         return result
 
-    # Delete trashed and deleted files from Hydrus from the database
+    @staticmethod
+    def update_search_cache(new_total: int | None = None) -> None:
+        """
+        Update the search cache to clamp the farthest_search_index to the current length of the database
+        """
+        assert new_total is None or new_total >= 0
+
+        if not database_accessible(DEDUP_DATABASE_FILE, tablename="videos"):
+            return
+
+        CHUNK_SIZE = 256
+        with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c", outer_stack=False) as hashdb:
+            if new_total is None:
+                new_total = len(hashdb)
+            for batched_items in HydrusVideoDeduplicator.batched_and_save_db(hashdb, CHUNK_SIZE):
+                for item in batched_items.items():
+                    row = hashdb[item[0]]
+                    if 'farthest_search_index' in row and row['farthest_search_index'] > new_total:
+                        row['farthest_search_index'] = new_total
+                        hashdb[item[0]] = row
+
     def clear_trashed_files_from_db(self) -> None:
+        """
+        Delete trashed and deleted files from Hydrus from the database
+        TODO: This doesn't have to run everytime. Run it every couple startups or something.
+        """
         if not database_accessible(DEDUP_DATABASE_FILE, tablename="videos"):
             return
 
         try:
-            CHUNK_SIZE = 32
-            delete_count = 0
-            with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c") as hashdb:
-                for batched_keys in self.batched(hashdb, CHUNK_SIZE):
-                    is_trashed_result = self.is_files_trashed_hydrus(batched_keys)
-                    for result in is_trashed_result.items():
-                        if result[1] is True:
-                            del hashdb[result[0]]
-                            delete_count += 1
-                    hashdb.commit()
-            self.hydlog.info(f"Cleared {delete_count} trashed files from the database.")
-        except OSError:
-            rprint("[red] Error while clearing trashed files cache.")
+            with SqliteDict(str(DEDUP_DATABASE_FILE), tablename="videos", flag="c", outer_stack=False) as hashdb:
+                # This is EXPENSIVE. sqlitedict gets len by iterating over the entire database!
+                if (total := len(hashdb)) < 1:
+                    return
+
+                delete_count = 0
+                rprint(f"[blue] Database found with {total} videos already hashed.")
+                try:
+                    with tqdm(
+                        dynamic_ncols=True,
+                        total=total,
+                        desc="Clearing trashed videos",
+                        unit="video",
+                        colour="BLUE",
+                    ) as pbar:
+                        CHUNK_SIZE = 32
+                        for batched_items in self.batched_and_save_db(hashdb, CHUNK_SIZE):
+                            is_trashed_result = self.is_files_deleted_hydrus(batched_items.keys())
+                            for result in is_trashed_result.items():
+                                video_hash = result[0]
+                                is_trashed = result[1]
+                                if is_trashed is True:
+                                    del hashdb[video_hash]
+                                    delete_count += 1
+                            pbar.update(min(CHUNK_SIZE, total - pbar.n))
+                except Exception as exc:
+                    rprint("[red] Error while clearing trashed videos cache.")
+                    print(exc)
+                    self.hydlog.error(exc)
+                finally:
+                    if delete_count > 0:
+                        print(f"Cleared {delete_count} trashed videos from the database.")
+                    self.update_search_cache(total - delete_count)
+
+        except OSError as exc:
+            self.hydlog.info(exc)
```

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/LICENSE` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/hydrus_api/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/__init__.py` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/hydrus_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+import collections.abc as abc
 import enum
 import json
 import os
 import typing as T
-import collections.abc as abc
 
 import requests
 
 __version__ = "5.0.0"
 
 DEFAULT_API_URL = "http://127.0.0.1:45869/"
 HYDRUS_METADATA_ENCODING = "utf-8"
@@ -278,15 +278,15 @@
     _SET_KINGS_PATH = "/manage_file_relationships/set_kings"
 
     def __init__(
         self,
         access_key: T.Optional[str] = None,
         api_url: str = DEFAULT_API_URL,
         session: T.Optional[requests.Session] = None,
-        verify_cert: T.Optional[str] = None, # Path to cert
+        verify_cert: T.Optional[str] = None,  # Path to cert
     ) -> None:
         """
         See https://hydrusnetwork.github.io/hydrus/client_api.html for documentation.
         """
 
         self.access_key = access_key
         self.api_url = api_url.rstrip("/")
@@ -301,20 +301,20 @@
         # protocol
         json_data = kwargs.pop("json", None)
         if json_data is not None:
             kwargs["data"] = json.dumps(json_data, cls=_ABCJSONEncoder)
             # Since we aren't using the json keyword-argument, we have to set the Content-Type manually
             kwargs["headers"]["Content-Type"] = "application/json"
 
-        if self._verify_cert == None:
+        if self._verify_cert is None:
             kwargs["verify"] = False
-            requests.packages.urllib3.disable_warnings() 
+            requests.packages.urllib3.disable_warnings()
         else:
             kwargs["verify"] = self._verify_cert
-        
+
         try:
             response = self.session.request(method, self.api_url + path, **kwargs)
         except requests.RequestException as error:
             # Re-raise connection and timeout errors as hydrus.ConnectionErrors so these are more easy to handle for
             # client applications
             raise ConnectionError(*error.args)
```

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/hydrus_api/utils.py` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/hydrus_api/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,22 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import collections
 import os
 import typing as T
 import collections.abc as abc
 
-from hydrusvideodeduplicator.hydrus_api import DEFAULT_API_URL, HYDRUS_METADATA_ENCODING, BinaryFileLike, Client, ImportStatus, Permission
+from hydrusvideodeduplicator.hydrus_api import (
+    DEFAULT_API_URL,
+    HYDRUS_METADATA_ENCODING,
+    BinaryFileLike,
+    Client,
+    ImportStatus,
+    Permission,
+)
 
 _X = T.TypeVar("_X")
 
 
 # This is public so other code can import it to annotate their own types
 class TextFileLike(T.Protocol):
     def read(self) -> str:
```

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/hasher/pdq_hasher.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     PDQ_DO_DIH_FLIP_PLUS1 = 0x40
     PDQ_DO_DIH_FLIP_MINUS1 = 0x80
     PDQ_DO_DIH_ALL = 0xFF
 
     DCT_matrix: List[List[float]] = []
 
     def compute_dct_matrix(self):
-        matrix_scale_factor = math.sqrt(2.0 / 64.0)
+        # matrix_scale_factor = math.sqrt(2.0 / 64.0)
         d = [0] * 16
         for i in range(0, 16):
             di = [0] * 64
             for j in range(0, 64):
                 di[j] = math.cos((math.pi / 2 / 64.0) * (i + 1) * (2 * j + 1))
             d[i] = di
         return d
@@ -89,65 +89,55 @@
         numCols, numRows = img.size
         buffer1 = MatrixUtil.allocateMatrixAsRowMajorArray(numRows, numCols)
         buffer2 = MatrixUtil.allocateMatrixAsRowMajorArray(numRows, numCols)
         buffer64x64 = MatrixUtil.allocateMatrix(64, 64)
         buffer16x64 = MatrixUtil.allocateMatrix(16, 64)
         buffer16x16 = MatrixUtil.allocateMatrix(16, 16)
         t1 = time.time()
-        rv = self.fromImage(
-            img, buffer1, buffer2, buffer64x64, buffer16x64, buffer16x16
-        )
+        rv = self.fromImage(img, buffer1, buffer2, buffer64x64, buffer16x64, buffer16x16)
         t2 = time.time()
 
         if hashingMetadata is not None:
             hashingMetadata.imageHeightTimesWidth = numRows * numCols
             hashingMetadata.readSeconds = readSeconds
             hashingMetadata.hashSeconds = t2 - t1
         return rv
 
     def fromBufferedImage(self, img):
         try:
-            #img = Image.open(img_bytes)
+            # img = Image.open(img_bytes)
             # resizing the image proportionally to max 512px width and max 512px height
             img.thumbnail((512, 512))
         except IOError as e:
             raise e
         numCols, numRows = img.size
         buffer1 = MatrixUtil.allocateMatrixAsRowMajorArray(numRows, numCols)
         buffer2 = MatrixUtil.allocateMatrixAsRowMajorArray(numRows, numCols)
         buffer64x64 = MatrixUtil.allocateMatrix(64, 64)
         buffer16x64 = MatrixUtil.allocateMatrix(16, 64)
         buffer16x16 = MatrixUtil.allocateMatrix(16, 16)
-        return self.fromImage(
-            img, buffer1, buffer2, buffer64x64, buffer16x64, buffer16x16
-        )
+        return self.fromImage(img, buffer1, buffer2, buffer64x64, buffer16x64, buffer16x16)
 
     def fromImage(self, img, buffer1, buffer2, buffer64x64, buffer16x64, buffer16x16):
         numCols, numRows = img.size
         self.fillFloatLumaFromBufferImage(img, buffer1)
-        return self.pdqHash256FromFloatLuma(
-            buffer1, buffer2, numRows, numCols, buffer64x64, buffer16x64, buffer16x16
-        )
+        return self.pdqHash256FromFloatLuma(buffer1, buffer2, numRows, numCols, buffer64x64, buffer16x64, buffer16x16)
 
     def fillFloatLumaFromBufferImage(self, img, luma):
         numCols, numRows = img.size
         rgb_image = img.convert("RGB")
         pixels = rgb_image.load()
 
         for i in range(numRows):
             for j in range(numCols):
                 r, g, b = pixels[j, i]
                 luma[i * numCols + j] = (
-                    self.LUMA_FROM_R_COEFF * r
-                    + self.LUMA_FROM_G_COEFF * g
-                    + self.LUMA_FROM_B_COEFF * b
+                    self.LUMA_FROM_R_COEFF * r + self.LUMA_FROM_G_COEFF * g + self.LUMA_FROM_B_COEFF * b
                 )
 
-
-
     def pdqHash256FromFloatLuma(
         self,
         fullBuffer1,
         fullBuffer2,
         numRows,
         numCols,
         buffer64x64,
@@ -294,17 +284,15 @@
             hashFlipY,
             hashFlipPlus1,
             hashFlipMinus1,
             quality,
         )
 
     @classmethod
-    def decimateFloat(
-        cls, in_, inNumRows, inNumCols, out  # numRows x numCols in row-major order
-    ):
+    def decimateFloat(cls, in_, inNumRows, inNumCols, out):  # numRows x numCols in row-major order
         for i in range(64):
             ini = int(((i + 0.5) * inNumRows) / 64)
             for j in range(64):
                 inj = int(((j + 0.5) * inNumCols) / 64)
                 out[i][j] = in_[ini * inNumCols + inj]
 
     @classmethod
@@ -452,37 +440,30 @@
                 if dctOutput16x16[i][j] > dctMedian:
                     _hash.setBit(i * 16 + j)
         return _hash
 
     @classmethod
     def computeJaroszFilterWindowSize(cls, dimension):
         """Round up. See comments at top of file for details."""
-        return int(
-            (dimension + cls.PDQ_JAROSZ_WINDOW_SIZE_DIVISOR - 1)
-            / cls.PDQ_JAROSZ_WINDOW_SIZE_DIVISOR
-        )
+        return int((dimension + cls.PDQ_JAROSZ_WINDOW_SIZE_DIVISOR - 1) / cls.PDQ_JAROSZ_WINDOW_SIZE_DIVISOR)
 
     @classmethod
     def jaroszFilterFloat(
         cls,
         buffer1,
         buffer2,
         numRows,
         numCols,
         windowSizeAlongRows,
         windowSizeAlongCols,
         nreps,
     ):
         for _i in range(nreps):
-            cls.boxAlongRowsFloat(
-                buffer1, buffer2, numRows, numCols, windowSizeAlongRows
-            )
-            cls.boxAlongColsFloat(
-                buffer2, buffer1, numRows, numCols, windowSizeAlongCols
-            )
+            cls.boxAlongRowsFloat(buffer1, buffer2, numRows, numCols, windowSizeAlongRows)
+            cls.boxAlongColsFloat(buffer2, buffer1, numRows, numCols, windowSizeAlongCols)
 
     """
     ----------------------------------------------------------------
     # 7 and 4
     #
     #    0 0 0 0 0 0 0 0 0 0 1 1 1 1 1 1
     #    0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5
@@ -628,15 +609,14 @@
 
         # PHASE 4: FINAL WRITES WITH SMALL WINDOW
         for i in range(phase_4_nreps):
             _sum -= invec[inStartOffset + (i + phase_3_nreps + phase_2_nreps) * stride]
             currentWindowSize -= 1
             outvec[outStartOffset + (i + phase_3_nreps + phase_2_nreps) * stride] = _sum / currentWindowSize
 
-
     @classmethod
     def boxAlongRowsFloat(cls, _input, output, numRows, numCols, windowSize):
         """
         input - matrix as numRows x numCols in row-major order
         output - matrix as numRows x numCols in row-major order
         """
         for i in range(numRows):
```

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/tests/hash256_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 
     def test_incorrect_hex_length(self) -> None:
         with self.assertRaises(PDQHashFormatException):
             Hash256.fromHexString("AAA")
 
     def test_incorrect_hex_format(self) -> None:
         with self.assertRaises(PDQHashFormatException):
-            Hash256.fromHexString(
-                "9c151c3af838278e3ef57c180c7d031c07aefd12f2ccc1e18f2a1e1c7d0ff16!"
-            )
+            Hash256.fromHexString("9c151c3af838278e3ef57c180c7d031c07aefd12f2ccc1e18f2a1e1c7d0ff16!")
 
     def test_correct_hex_format(self) -> None:
         hash = Hash256.fromHexString(self.SAMPLE_HASH)
         self.assertNotEquals(hash, None)
 
     def test_clone(self) -> None:
         hash = Hash256.fromHexString(self.SAMPLE_HASH)
```

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/tests/pdq_test.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/tools/pdq_photo_hasher_tool.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/env python
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # isort:skip_file
+from ..hasher.pdq_hasher import PDQHasher
+from ..types.hash256 import Hash256
 
 import argparse
 import os
 import sys
 
 sys.path.append(os.path.join(os.path.dirname(__file__), "../.."))
 
-from ..hasher.pdq_hasher import PDQHasher
-from ..types.hash256 import Hash256
-
 
 class PDQPhotoHasherTool:
     """Tool for computing PDQ hashes of image files (JPEG, PNG, etc.).
     Example use from within pdqhashing directory in Instagram Container:
     python tools/pdq_photo_hasher_tool.py ../media/sample_data/pdq/misc-images/b.jpg --pdq"""
 
     PROGNAME = "PDQPhotoHasherTool"
@@ -31,51 +30,43 @@
             self.pdqHashPrev = _pdqHashPrev
             self.hadError = _hadError
 
     @classmethod
     def main(cls, args):
         parser = argparse.ArgumentParser(
             prog=cls.PROGNAME,
-            description="Create PDQ Photo hashes for provided files. "
-            + "Supported filetypes are: JPEG and PNG.",
+            description="Create PDQ Photo hashes for provided files. " + "Supported filetypes are: JPEG and PNG.",
         )
 
         parser.add_argument(
             "filenames",
             nargs="*",
             type=str,
             help="Filenames/paths of the files to be processed.",
         )
 
         parser.add_argument(
             "-i",
             "--filesOnStdin",
             action="store_true",
-            help=(
-                "Take filenames from stdin, in which case there must be "
-                + "no filenames on the command line."
-            ),
+            help=("Take filenames from stdin, in which case there must be " + "no filenames on the command line."),
         )
 
         parser.add_argument(
             "-d",
             "--doDetailedOutput",
             action="store_true",
-            help="Print norm, delta, etc; Otherwise, print just hash, "
-            + "quality and filename.",
+            help="Print norm, delta, etc; Otherwise, print just hash, " + "quality and filename.",
         )
 
         parser.add_argument(
             "--pdq",
             dest="doPDQ",
             action="store_true",
-            help=(
-                "Take filenames from stdin, in which case there must be "
-                + "no filenames on the command line."
-            ),
+            help=("Take filenames from stdin, in which case there must be " + "no filenames on the command line."),
         )
 
         parser.add_argument(
             "--pdqdih",
             dest="doPDQDih",
             action="store_true",
             help="Print all 8 dihedral-transform hashes.",
@@ -127,17 +118,15 @@
                         args.doTimings,
                         args.keepGoingAfterErrors,
                         context,
                     )
                     sys.stdout.flush()
                 exit(0)
             except IOError:
-                sys.stderr.write(
-                    "{}: couldn't read line {} \n".format(cls.PROGNAME, lno)
-                )
+                sys.stderr.write("{}: couldn't read line {} \n".format(cls.PROGNAME, lno))
                 exit(1)
 
         for filename in args.filenames:
             context.numPDQHash += 1
             cls.processFile(
                 pdqHasher,
                 filename,
@@ -174,19 +163,15 @@
         delta = int()
         hashingMetadata = PDQHasher.HashingMetadata()
         if doPDQHash:
             try:
                 hashAndQuality = pdqHasher.fromFile(filename, hashingMetadata)
             except IOError as e:
                 context.hadError = True
-                sys.stderr.write(
-                    "{}: could not read image file {}, Error {}\n".format(
-                        cls.PROGNAME, filename, e
-                    )
-                )
+                sys.stderr.write("{}: could not read image file {}, Error {}\n".format(cls.PROGNAME, filename, e))
                 if keepGoingAfterErrors:
                     return
                 else:
                     exit(1)
             hash = hashAndQuality.getHash()
             quality = hashAndQuality.getQuality()
             norm = hash.hammingNorm()
@@ -195,36 +180,30 @@
                 delta = 0
             else:
                 delta = hash.hammingDistance(context.pdqHashPrev)
 
             if not doDetailedOutput:
                 print("{},{},{}".format(hash, quality, filename))
             else:
-                output = "hash={},norm={},delta={},quality={}".format(
-                    hash, norm, delta, quality
-                )
+                output = "hash={},norm={},delta={},quality={}".format(hash, norm, delta, quality)
                 if doTimings:
                     output += ",dims={},readSeconds={:.6f},hashSeconds={:.6f}".format(
                         hashingMetadata.imageHeightTimesWidth,
                         hashingMetadata.readSeconds,
                         hashingMetadata.hashSeconds,
                     )
                 output += ",filename={}".format(filename)
                 print(output)
             context.pdqHashPrev = hash
         if doPDQDih:
             try:
-                dihedralBag = pdqHasher.dihedralFromFile(
-                    filename, hashingMetadata, PDQHasher.PDQ_DO_DIH_ALL
-                )
-            except IOError as e:
+                dihedralBag = pdqHasher.dihedralFromFile(filename, hashingMetadata, PDQHasher.PDQ_DO_DIH_ALL)
+            except IOError:
                 context.hadError = True
-                sys.stderr.write(
-                    "%s: could not read image file %s.\n".format(cls.PROGNAME, filename)
-                )
+                sys.stderr.write(f"{cls.PROGNAME}: could not read image file {filename}.\n")
                 if keepGoingAfterErrors:
                     return
                 else:
                     exit(1)
             if not doDetailedOutput:
                 if doPDQDihAcross:
                     print(
@@ -240,110 +219,60 @@
                             dihedralBag.quality,
                             filename,
                         )
                     )
                 else:
                     bquality = dihedralBag.quality
                     print("{},{},{}".format(dihedralBag.hash, bquality, filename))
-                    print(
-                        "{},{},{}".format(dihedralBag.hashRotate90, bquality, filename)
-                    )
-                    print(
-                        "{},{},{}".format(dihedralBag.hashRotate180, bquality, filename)
-                    )
-                    print(
-                        "{},{},{}".format(dihedralBag.hashRotate270, bquality, filename)
-                    )
+                    print("{},{},{}".format(dihedralBag.hashRotate90, bquality, filename))
+                    print("{},{},{}".format(dihedralBag.hashRotate180, bquality, filename))
+                    print("{},{},{}".format(dihedralBag.hashRotate270, bquality, filename))
                     print("{},{},{}".format(dihedralBag.hashFlipX, bquality, filename))
                     print("{},{},{}".format(dihedralBag.hashFlipY, bquality, filename))
-                    print(
-                        "{},{},{}".format(dihedralBag.hashFlipPlus1, bquality, filename)
-                    )
-                    print(
-                        "{},{},{}".format(
-                            dihedralBag.hashFlipMinus1, bquality, filename
-                        )
-                    )
+                    print("{},{},{}".format(dihedralBag.hashFlipPlus1, bquality, filename))
+                    print("{},{},{}".format(dihedralBag.hashFlipMinus1, bquality, filename))
             else:
                 if doPDQDihAcross:
-                    output = "hash={},quality={}".format(
-                        dihedralBag.hash, dihedralBag.quality
-                    )
+                    output = "hash={},quality={}".format(dihedralBag.hash, dihedralBag.quality)
                     if doTimings:
-                        output += (
-                            ",dims={},readSeconds={:.6f},hashSeconds={:.6f}".format(
-                                hashingMetadata.imageHeightTimesWidth,
-                                hashingMetadata.readSeconds,
-                                hashingMetadata.hashSeconds,
-                            )
+                        output += ",dims={},readSeconds={:.6f},hashSeconds={:.6f}".format(
+                            hashingMetadata.imageHeightTimesWidth,
+                            hashingMetadata.readSeconds,
+                            hashingMetadata.hashSeconds,
+                        )
+                    output += (
+                        ",orig={},rot90={},rot180={},,rot270={},flipx={},flipy={},flipp={},flipm={},filename={}".format(
+                            dihedralBag.hash,
+                            dihedralBag.hashRotate90,
+                            dihedralBag.hashRotate180,
+                            dihedralBag.hashRotate270,
+                            dihedralBag.hashFlipX,
+                            dihedralBag.hashFlipY,
+                            dihedralBag.hashFlipPlus1,
+                            dihedralBag.hashFlipMinus1,
+                            filename,
                         )
-                    output += ",orig={},rot90={},rot180={},,rot270={},flipx={},flipy={},flipp={},flipm={},filename={}".format(
-                        dihedralBag.hash,
-                        dihedralBag.hashRotate90,
-                        dihedralBag.hashRotate180,
-                        dihedralBag.hashRotate270,
-                        dihedralBag.hashFlipX,
-                        dihedralBag.hashFlipY,
-                        dihedralBag.hashFlipPlus1,
-                        dihedralBag.hashFlipMinus1,
-                        filename,
                     )
                     print(output)
                 else:
-                    output = "hash={},quality={}".format(
-                        dihedralBag.hash, dihedralBag.quality
-                    )
+                    output = "hash={},quality={}".format(dihedralBag.hash, dihedralBag.quality)
                     if doTimings:
-                        output += (
-                            ",dims={},readSeconds={:.6f},hashSeconds={:.6f}".format(
-                                hashingMetadata.imageHeightTimesWidth,
-                                hashingMetadata.readSeconds,
-                                hashingMetadata.hashSeconds,
-                            )
+                        output += ",dims={},readSeconds={:.6f},hashSeconds={:.6f}".format(
+                            hashingMetadata.imageHeightTimesWidth,
+                            hashingMetadata.readSeconds,
+                            hashingMetadata.hashSeconds,
                         )
                     output += ",filename={}".format(filename)
                     print(output)
-                    print(
-                        "hash={},xform=orig,filename={}".format(
-                            dihedralBag.hash, filename
-                        )
-                    )
-                    print(
-                        "hash={},xform=rot90,filename={}".format(
-                            dihedralBag.hashRotate90, filename
-                        )
-                    )
-                    print(
-                        "hash={},xform=rot180,filename={}".format(
-                            dihedralBag.hashRotate180, filename
-                        )
-                    )
-                    print(
-                        "hash={},xform=rot270,filename={}".format(
-                            dihedralBag.hashRotate270, filename
-                        )
-                    )
-                    print(
-                        "hash={},xform=flipx,filename={}".format(
-                            dihedralBag.hashFlipX, filename
-                        )
-                    )
-                    print(
-                        "hash={},xform=flipy,filename={}".format(
-                            dihedralBag.hashFlipY, filename
-                        )
-                    )
-                    print(
-                        "hash={},xform=flipp,filename={}".format(
-                            dihedralBag.hashFlipPlus1, filename
-                        )
-                    )
-                    print(
-                        "hash={},xform=flipm,filename={}".format(
-                            dihedralBag.hashFlipMinus1, filename
-                        )
-                    )
+                    print("hash={},xform=orig,filename={}".format(dihedralBag.hash, filename))
+                    print("hash={},xform=rot90,filename={}".format(dihedralBag.hashRotate90, filename))
+                    print("hash={},xform=rot180,filename={}".format(dihedralBag.hashRotate180, filename))
+                    print("hash={},xform=rot270,filename={}".format(dihedralBag.hashRotate270, filename))
+                    print("hash={},xform=flipx,filename={}".format(dihedralBag.hashFlipX, filename))
+                    print("hash={},xform=flipy,filename={}".format(dihedralBag.hashFlipY, filename))
+                    print("hash={},xform=flipp,filename={}".format(dihedralBag.hashFlipPlus1, filename))
+                    print("hash={},xform=flipm,filename={}".format(dihedralBag.hashFlipMinus1, filename))
             context.pdqHashPrev = dihedralBag.hash.clone()
 
 
 if __name__ == "__main__":
     PDQPhotoHasherTool.main(sys.argv)
```

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/types/containers.py` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/types/containers.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/types/hash256.py`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/pdqhashing/utils/matrix.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,8 @@
                 min_val = mingtguess
 
         if less >= midn:
             return maxltguess
         elif less + equal >= midn:
             return guess
         else:
-            return mingtguess
+            return mingtguess
```

### Comparing `hydrusvideodeduplicator-0.2.3/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py` & `hydrusvideodeduplicator-0.2.4/src/hydrusvideodeduplicator/vpdqpy/vpdqpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from __future__ import annotations
 
 import io
 import json
+import logging
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING
-import logging
 
 import av
 from PIL import Image
 
 from ..pdqhashing.hasher.pdq_hasher import PDQHasher
+from ..pdqhashing.types.hash256 import Hash256
 
 if TYPE_CHECKING:
     from typing import Annotated, Generator
 
     from .typing_utils import ValueRange
 
-    from ..pdqhashing.types.containers import HashAndQuality
-
-from ..pdqhashing.types.hash256 import Hash256
-
 
 @dataclass(slots=True)
 class VpdqFeature:
     pdq_hash: Hash256  # 64 char hex string
     quality: float  # 0 to 100
     frame_number: int
```

### Comparing `hydrusvideodeduplicator-0.2.3/.gitignore` & `hydrusvideodeduplicator-0.2.4/.gitignore`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# Perceptual Hash Database
-thedb
-
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
@@ -159,8 +156,32 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # Pickle
-*.pkl
+*.pkl
+
+# Created by https://www.toptal.com/developers/gitignore/api/visualstudiocode
+# Edit at https://www.toptal.com/developers/gitignore?templates=visualstudiocode
+
+### VisualStudioCode ###
+.vscode/*
+!.vscode/settings.json
+!.vscode/tasks.json
+!.vscode/launch.json
+!.vscode/extensions.json
+!.vscode/*.code-snippets
+
+# Local History for Visual Studio Code
+.history/
+
+# Built Visual Studio Code Extensions
+*.vsix
+
+### VisualStudioCode Patch ###
+# Ignore all local history of files
+.history
+.ionide
+
+# End of https://www.toptal.com/developers/gitignore/api/visualstudiocode
```

### Comparing `hydrusvideodeduplicator-0.2.3/LICENSE` & `hydrusvideodeduplicator-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrusvideodeduplicator-0.2.3/README.md` & `hydrusvideodeduplicator-0.2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
   <img src="https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/assets/104981058/e65383e8-1978-46aa-88b6-6fdda9767367">
   
 Hydrus Video Deduplicator finds potential duplicate videos through the Hydrus API
 
 
 [![PyPI - Version](https://img.shields.io/pypi/v/hydrusvideodeduplicator.svg)](https://pypi.org/project/hydrusvideodeduplicator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hydrusvideodeduplicator.svg)](https://pypi.org/project/hydrusvideodeduplicator)
+[![PyPI downloads](https://img.shields.io/pypi/dm/hydrusvideodeduplicator.svg)](https://pypistats.org/packages/hydrusvideodeduplicator)
 [![GitHub Repo stars](https://img.shields.io/github/stars/hydrusvideodeduplicator/hydrus-video-deduplicator)](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/stargazers)
 
 </div>
 
 ---
 
 ## How It Works:
@@ -21,15 +22,15 @@
 
 You can choose to process only a subset of videos with `--query` using Hydrus tags, e.g. `--query="character:edward"` will only process videos with the tag `character:edward`.
 
 For more information check out the [wiki](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki) and the [FAQ](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki/faq)
 
 ---
 
-## Installation:
+## [Installation:](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki/Installation)
 #### Dependencies:
 - Python >=3.10
 - FFmpeg
 
 ```sh
 python3 -m pip install hydrusvideodeduplicator
 ```
@@ -71,8 +72,8 @@
 
 [Hydrus API Library](https://gitlab.com/cryzed/hydrus-api) (GNU AGPLv3) by cryzed
 
 [pdq](https://github.com/facebook/ThreatExchange/tree/main/pdq) (BSD) by Meta
 
 [vpdq](https://github.com/facebook/ThreatExchange/tree/main/vpdq) (BSD) by Meta
 
-[Big Buck Bunny](https://peach.blender.org/about)  (CC BY 3.0) clips by Blender Foundation
+[Big Buck Bunny](https://peach.blender.org/about), [Sintel](https://durian.blender.org/about/)  (CC BY 3.0) clips by Blender Foundation
```

### Comparing `hydrusvideodeduplicator-0.2.3/PKG-INFO` & `hydrusvideodeduplicator-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: hydrusvideodeduplicator
-Version: 0.2.3
+Version: 0.2.4
 Summary: Video deduplicator utility for Hydrus Network
 Project-URL: Documentation, https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator#readme
 Project-URL: Issues, https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/issues
 Project-URL: Source, https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator
 Author-email: hydrusvideodeduplicator <applenannerapple@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
-Requires-Dist: appdirs
 Requires-Dist: av
 Requires-Dist: joblib
 Requires-Dist: numpy
 Requires-Dist: pillow
+Requires-Dist: platformdirs
 Requires-Dist: psutil
 Requires-Dist: python-dotenv
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: sqlitedict
 Requires-Dist: tqdm
 Requires-Dist: typer
@@ -33,14 +33,15 @@
   <img src="https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/assets/104981058/e65383e8-1978-46aa-88b6-6fdda9767367">
   
 Hydrus Video Deduplicator finds potential duplicate videos through the Hydrus API
 
 
 [![PyPI - Version](https://img.shields.io/pypi/v/hydrusvideodeduplicator.svg)](https://pypi.org/project/hydrusvideodeduplicator)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hydrusvideodeduplicator.svg)](https://pypi.org/project/hydrusvideodeduplicator)
+[![PyPI downloads](https://img.shields.io/pypi/dm/hydrusvideodeduplicator.svg)](https://pypistats.org/packages/hydrusvideodeduplicator)
 [![GitHub Repo stars](https://img.shields.io/github/stars/hydrusvideodeduplicator/hydrus-video-deduplicator)](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/stargazers)
 
 </div>
 
 ---
 
 ## How It Works:
@@ -50,15 +51,15 @@
 
 You can choose to process only a subset of videos with `--query` using Hydrus tags, e.g. `--query="character:edward"` will only process videos with the tag `character:edward`.
 
 For more information check out the [wiki](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki) and the [FAQ](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki/faq)
 
 ---
 
-## Installation:
+## [Installation:](https://github.com/hydrusvideodeduplicator/hydrus-video-deduplicator/wiki/Installation)
 #### Dependencies:
 - Python >=3.10
 - FFmpeg
 
 ```sh
 python3 -m pip install hydrusvideodeduplicator
 ```
@@ -100,8 +101,8 @@
 
 [Hydrus API Library](https://gitlab.com/cryzed/hydrus-api) (GNU AGPLv3) by cryzed
 
 [pdq](https://github.com/facebook/ThreatExchange/tree/main/pdq) (BSD) by Meta
 
 [vpdq](https://github.com/facebook/ThreatExchange/tree/main/vpdq) (BSD) by Meta
 
-[Big Buck Bunny](https://peach.blender.org/about)  (CC BY 3.0) clips by Blender Foundation
+[Big Buck Bunny](https://peach.blender.org/about), [Sintel](https://durian.blender.org/about/)  (CC BY 3.0) clips by Blender Foundation
```

