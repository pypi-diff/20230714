# Comparing `tmp/pbs_installer-2023.7.13.post0.tar.gz` & `tmp/pbs_installer-2023.7.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbs_installer-2023.7.13.post0.tar", last modified: Thu Jul 13 13:04:04 2023, max compression
+gzip compressed data, was "pbs_installer-2023.7.14.tar", last modified: Fri Jul 14 01:40:23 2023, max compression
```

## Comparing `pbs_installer-2023.7.13.post0.tar` & `pbs_installer-2023.7.14.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1059 2023-07-13 13:03:50.299560 pbs_installer-2023.7.13.post0/LICENSE
--rw-r--r--   0        0        0      331 2023-07-13 13:03:50.299560 pbs_installer-2023.7.13.post0/README.md
--rw-r--r--   0        0        0      889 2023-07-13 13:04:04.543616 pbs_installer-2023.7.13.post0/pyproject.toml
--rw-r--r--   0        0        0      196 2023-07-13 13:03:50.299560 pbs_installer-2023.7.13.post0/src/pbs_installer/__init__.py
--rw-r--r--   0        0        0      450 2023-07-13 13:03:50.299560 pbs_installer-2023.7.13.post0/src/pbs_installer/__main__.py
--rw-r--r--   0        0        0     3762 2023-07-13 13:03:50.299560 pbs_installer-2023.7.13.post0/src/pbs_installer/_install.py
--rw-r--r--   0        0        0     1613 2023-07-13 13:03:50.299560 pbs_installer-2023.7.13.post0/src/pbs_installer/_utils.py
--rw-r--r--   0        0        0    65314 2023-07-13 13:03:50.303558 pbs_installer-2023.7.13.post0/src/pbs_installer/_versions.py
--rw-r--r--   0        0        0        0 2023-07-13 13:03:50.303558 pbs_installer-2023.7.13.post0/tests/__init__.py
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 pbs_installer-2023.7.13.post0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-14 01:39:52.588540 pbs_installer-2023.7.14/LICENSE
+-rw-r--r--   0        0        0      331 2023-07-14 01:39:52.588540 pbs_installer-2023.7.14/README.md
+-rw-r--r--   0        0        0     1034 2023-07-14 01:40:23.280692 pbs_installer-2023.7.14/pyproject.toml
+-rw-r--r--   0        0        0      275 2023-07-14 01:39:52.588540 pbs_installer-2023.7.14/src/pbs_installer/__init__.py
+-rw-r--r--   0        0        0     1100 2023-07-14 01:39:52.588540 pbs_installer-2023.7.14/src/pbs_installer/__main__.py
+-rw-r--r--   0        0        0     4930 2023-07-14 01:39:52.592540 pbs_installer-2023.7.14/src/pbs_installer/_install.py
+-rw-r--r--   0        0        0     1613 2023-07-14 01:39:52.592540 pbs_installer-2023.7.14/src/pbs_installer/_utils.py
+-rw-r--r--   0        0        0    65314 2023-07-14 01:39:52.592540 pbs_installer-2023.7.14/src/pbs_installer/_versions.py
+-rw-r--r--   0        0        0        0 2023-07-14 01:39:52.592540 pbs_installer-2023.7.14/tests/__init__.py
+-rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 pbs_installer-2023.7.14/PKG-INFO
```

### Comparing `pbs_installer-2023.7.13.post0/LICENSE` & `pbs_installer-2023.7.14/LICENSE`

 * *Files identical despite different names*

### Comparing `pbs_installer-2023.7.13.post0/pyproject.toml` & `pbs_installer-2023.7.14/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 [project]
 name = "pbs-installer"
 description = "Installer for Python Build Standalone"
 authors = [
     { name = "Frost Ming", email = "me@frostming.com" },
 ]
-dependencies = [
-    "zstandard>=0.21.0",
-]
+dependencies = []
 requires-python = ">=3.7"
 readme = "README.md"
 dynamic = []
-version = "2023.7.13.post0"
+version = "2023.7.14"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
-full = [
+download = [
     "requests>=2.24.0",
 ]
+install = [
+    "zstandard>=0.21.0",
+]
+all = [
+    "pbs-installer[download,install]",
+]
 
 [project.scripts]
 pbs-install = "pbs_installer.__main__:main"
 
 [build-system]
 requires = [
     "pdm-backend",
@@ -40,7 +44,14 @@
 [tool.pdm.scripts.update]
 shell = "./scripts/update.sh"
 
 [tool.black]
 line-length = 100
 include = "\\.pyi?$"
 exclude = "/(\n    \\.eggs\n  | \\.git\n  | \\.hg\n  | \\.mypy_cache\n  | \\.tox\n  | \\.venv\n  | build\n  | dist\n  | src/pythonfinder/_vendor\n)\n"
+
+[tool.ruff]
+line-length = 100
+extend-select = [
+    "I",
+]
+target-version = "py310"
```

### Comparing `pbs_installer-2023.7.13.post0/src/pbs_installer/_install.py` & `pbs_installer-2023.7.14/src/pbs_installer/_install.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,14 +25,19 @@
     return {
         "X-GitHub-Api-Version": "2022-11-28",
         "Authorization": f"Bearer {TOKEN}",
     }
 
 
 def get_download_link(request: str) -> tuple[PythonVersion, str]:
+    """Get the download URL matching the given requested version.
+
+    :param request: The version of Python to install, e.g. 3.8,3.10.4
+    :return: A tuple of the PythonVersion and the download URL
+    """
     from ._versions import PYTHON_VERSIONS
 
     for py_ver, urls in PYTHON_VERSIONS.items():
         if not py_ver.matches(request):
             continue
 
         for arch, platform, url in urls:
@@ -50,14 +55,21 @@
     if not resp.ok:
         logger.warning("No checksum found for %s, this would be insecure", url)
         return None
     return resp.text.strip()
 
 
 def download(url: str, destination: StrPath, session: requests.Session | None = None) -> str:
+    """Download the given url to the destination.
+
+    :param url: The url to download
+    :param destination: The file path to download to
+    :param session: A requests session to use for downloading, or None to create a new one
+    :return: The original filename of the downloaded file
+    """
     logger.debug("Downloading url %s to %s", url, destination)
     filename = unquote(url.rsplit("/")[-1])
     try:
         import requests
     except ModuleNotFoundError:
         raise RuntimeError("You must install requests to use this function") from None
 
@@ -79,14 +91,21 @@
         raise RuntimeError(f"Checksum mismatch. Expected {checksum}, got {hasher.hexdigest()}")
     return filename
 
 
 def install_file(
     filename: StrPath, destination: StrPath, original_filename: str | None = None
 ) -> None:
+    """Unpack the downloaded file to the destination.
+
+    :param filename: The file to unpack
+    :param destination: The directory to unpack to
+    :param original_filename: The original filename of the file, if it was renamed
+    """
+
     import tarfile
 
     import zstandard as zstd
 
     if original_filename is None:
         original_filename = str(filename)
     logger.debug(
@@ -105,16 +124,29 @@
                 unpack_tar(z, destination, 1)
 
     else:
         with tarfile.open(filename) as z:
             unpack_tar(z, destination, 1)
 
 
-def install(request: str, destination: StrPath, session: requests.Session | None = None) -> None:
-    """Download and install the requested python version"""
+def install(
+    request: str,
+    destination: StrPath,
+    version_dir: bool = False,
+    session: requests.Session | None = None,
+) -> None:
+    """Download and install the requested python version.
+
+    :param request: The version of Python to install, e.g. 3.8,3.10.4
+    :param destination: The directory to install to
+    :param version_dir: Whether to install to a subdirectory named with the python version
+    :param session: A requests session to use for downloading
+    """
     ver, url = get_download_link(request)
-    logger.debug("Installing %s", ver)
+    if version_dir:
+        destination = os.path.join(destination, str(ver))
+    logger.debug("Installing %s to %s", ver, destination)
     os.makedirs(destination, exist_ok=True)
     with tempfile.NamedTemporaryFile() as tf:
         tf.close()
         original_filename = download(url, tf.name, session)
         install_file(tf.name, destination, original_filename)
```

### Comparing `pbs_installer-2023.7.13.post0/src/pbs_installer/_utils.py` & `pbs_installer-2023.7.14/src/pbs_installer/_utils.py`

 * *Files identical despite different names*

### Comparing `pbs_installer-2023.7.13.post0/src/pbs_installer/_versions.py` & `pbs_installer-2023.7.14/src/pbs_installer/_versions.py`

 * *Files identical despite different names*

### Comparing `pbs_installer-2023.7.13.post0/PKG-INFO` & `pbs_installer-2023.7.14/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: pbs-installer
-Version: 2023.7.13.post0
+Version: 2023.7.14
 Summary: Installer for Python Build Standalone
 Author-Email: Frost Ming <me@frostming.com>
 License: MIT
 Requires-Python: >=3.7
-Requires-Dist: zstandard>=0.21.0
-Requires-Dist: requests>=2.24.0; extra == "full"
-Provides-Extra: full
+Provides-Extra: download
+Provides-Extra: install
+Provides-Extra: all
+Requires-Dist: requests>=2.24.0; extra == "download"
+Requires-Dist: zstandard>=0.21.0; extra == "install"
+Requires-Dist: pbs-installer[download,install]; extra == "all"
 Description-Content-Type: text/markdown
 
 # pbs-installer
 
 [![PyPI](https://img.shields.io/pypi/v/pbs-installer)](https://pypi.org/project/pbs-installer)
 
 An installer for @indygreg's [python-build-standalone](https://github.com/indygreg/python-build-standalone)
```

