# Comparing `tmp/gitlab-ps-utils-0.8.0.tar.gz` & `tmp/gitlab_ps_utils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-ps-utils-0.8.0.tar", max compression
+gzip compressed data, was "gitlab_ps_utils-0.9.0.tar", max compression
```

## Comparing `gitlab-ps-utils-0.8.0.tar` & `gitlab_ps_utils-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1068 2022-04-12 20:40:59.756297 gitlab-ps-utils-0.8.0/LICENSE
--rw-r--r--   0        0        0     1367 2022-04-12 20:40:59.756297 gitlab-ps-utils-0.8.0/README.md
--rw-r--r--   0        0        0        0 2022-04-12 20:40:59.757297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/__init__.py
--rwxr-xr-x   0        0        0    14513 2022-04-12 20:40:59.757297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/api.py
--rw-r--r--   0        0        0      958 2022-04-12 20:40:59.757297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/audit_logger.py
--rw-r--r--   0        0        0     3581 2022-04-12 20:40:59.757297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/base_config.py
--rw-r--r--   0        0        0     2323 2022-04-12 20:40:59.757297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/decorators.py
--rw-r--r--   0        0        0     4912 2022-04-12 20:40:59.757297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/dict_utils.py
--rw-r--r--   0        0        0      195 2022-04-12 20:40:59.757297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/exceptions.py
--rw-r--r--   0        0        0     4860 2022-04-12 20:40:59.757297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/file_utils.py
--rw-r--r--   0        0        0     1386 2022-04-12 20:40:59.757297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/json_utils.py
--rw-r--r--   0        0        0     9988 2022-04-12 20:40:59.757297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/jsondiff.py
--rw-r--r--   0        0        0      673 2022-04-12 20:40:59.757297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/list_utils.py
--rw-r--r--   0        0        0     2095 2022-04-12 20:40:59.757297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/logger.py
--rw-r--r--   0        0        0     4259 2022-04-12 20:40:59.757297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/misc_utils.py
--rw-r--r--   0        0        0      324 2022-04-12 20:40:59.758297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/process.py
--rw-r--r--   0        0        0     8939 2022-04-12 20:40:59.758297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/processes.py
--rw-r--r--   0        0        0     1302 2022-04-12 20:40:59.758297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/string_utils.py
--rw-r--r--   0        0        0      187 2022-04-12 20:40:59.758297 gitlab-ps-utils-0.8.0/gitlab_ps_utils/xml_utils.py
--rw-r--r--   0        0        0      614 2022-04-12 20:40:59.758297 gitlab-ps-utils-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2221 2022-04-12 20:41:13.060111 gitlab-ps-utils-0.8.0/setup.py
--rw-r--r--   0        0        0     2118 2022-04-12 20:41:13.060540 gitlab-ps-utils-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-14 14:44:08.697297 gitlab_ps_utils-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1367 2023-07-14 14:44:08.697297 gitlab_ps_utils-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-14 14:44:08.727297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/__init__.py
+-rwxr-xr-x   0        0        0    14513 2023-07-14 14:44:08.697297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/api.py
+-rw-r--r--   0        0        0      958 2023-07-14 14:44:08.697297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/audit_logger.py
+-rw-r--r--   0        0        0     3581 2023-07-14 14:44:08.697297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/base_config.py
+-rw-r--r--   0        0        0     2323 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/decorators.py
+-rw-r--r--   0        0        0     4912 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/dict_utils.py
+-rw-r--r--   0        0        0      195 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/exceptions.py
+-rw-r--r--   0        0        0     5851 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/file_utils.py
+-rw-r--r--   0        0        0     1386 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/json_utils.py
+-rw-r--r--   0        0        0     9988 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/jsondiff.py
+-rw-r--r--   0        0        0      673 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/list_utils.py
+-rw-r--r--   0        0        0     2095 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/logger.py
+-rw-r--r--   0        0        0     4259 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/misc_utils.py
+-rw-r--r--   0        0        0      324 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/process.py
+-rw-r--r--   0        0        0     8939 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/processes.py
+-rw-r--r--   0        0        0     1302 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/string_utils.py
+-rw-r--r--   0        0        0      187 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/gitlab_ps_utils/xml_utils.py
+-rw-r--r--   0        0        0      614 2023-07-14 14:44:08.698297 gitlab_ps_utils-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2169 1970-01-01 00:00:00.000000 gitlab_ps_utils-0.9.0/PKG-INFO
```

### Comparing `gitlab-ps-utils-0.8.0/LICENSE` & `gitlab_ps_utils-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/README.md` & `gitlab_ps_utils-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/gitlab_ps_utils/api.py` & `gitlab_ps_utils-0.9.0/gitlab_ps_utils/api.py`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/gitlab_ps_utils/audit_logger.py` & `gitlab_ps_utils-0.9.0/gitlab_ps_utils/audit_logger.py`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/gitlab_ps_utils/base_config.py` & `gitlab_ps_utils-0.9.0/gitlab_ps_utils/base_config.py`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/gitlab_ps_utils/decorators.py` & `gitlab_ps_utils-0.9.0/gitlab_ps_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/gitlab_ps_utils/dict_utils.py` & `gitlab_ps_utils-0.9.0/gitlab_ps_utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/gitlab_ps_utils/file_utils.py` & `gitlab_ps_utils-0.9.0/gitlab_ps_utils/file_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,48 +4,65 @@
 import gzip
 import os
 from requests import Session, head, RequestException
 from re import findall
 from time import time
 from traceback import print_exc
 from gitlab_ps_utils.decorators import stable_retry
-
+from tqdm import tqdm
 
 @stable_retry(retries=5, delay=60, backoff=1.2)
 def download_file(url, path, filename=None, headers=None, verify=True):
     '''
     Uses the stable_retry decorator to attempt to stream download a file, typically
     a GitLab .tar.gz file. Any requests status other than 200 will result in
     an error, prompting the stable_retry.
     '''
-    if __is_downloadable(url, verify):
+    is_downloadable, content_type = __is_downloadable(url, verify)
+    if is_downloadable:
         chunk_size = 1024*1024
         session = Session()
         try:
             r = session.get(url, stream=True, headers=headers,
                             allow_redirects=True, verify=verify)
             r.raise_for_status()
             if filename is None:
                 filename = __get_filename_from_cd(
                     r.headers.get('content-disposition'))
+
+            # Get the total file size from the Content-Length header
+            total_size = int(r.headers.get('Content-Length', 0))
+
+            # Create a progress bar using tqdm
+            progress_bar = tqdm(total=total_size, unit='B', unit_scale=True, desc=filename)
+
             file_path = f"{path}/downloads/{filename}"
             create_local_project_export_structure(os.path.dirname(file_path))
             with open(file_path, "wb", chunk_size) as f:
                 for chunk in r.iter_content(chunk_size=chunk_size):
                     if chunk:
                         f.write(chunk)
+                        progress_bar.update(len(chunk))
+
+            progress_bar.close()
+
+            did_fully_download, actual_size = __did_file_fully_download(file_path, total_size)
+            if not did_fully_download:
+                raise OSError(f"File '{filename}' did not fully download.\nActual size: {actual_size}\nExpected size: {total_size}")
+
         except RequestException as re:
             print(
                 f"Download request to {url} failed for {filename} ({path}) due to:\n{re}", file=sys.stderr)
             return None
         except Exception as e:
             print(
                 f"Failed to download {filename} ({path}) from  {url} due to:\n{e}", file=sys.stderr)
             return None
-    return filename
+        return filename
+    raise ValueError(f"Invalid content type [{content_type}] for file [{filename}]")
 
 
 def create_local_project_export_structure(dir_path):
     if not os.path.exists(dir_path):
         try:
             os.makedirs(dir_path)
         except OSError as exc:  # Guard against race condition
@@ -71,31 +88,35 @@
     """
         Does the url contain a downloadable resource
     """
     h = head(url, allow_redirects=True, verify=verify)
     header = h.headers
     content_type = header.get('content-type')
     if 'text' in content_type.lower():
-        return False
+        return False, 'text'
     if 'html' in content_type.lower():
-        return False
-    return True
+        return False, 'html'
+    return True, content_type.lower()
 
 
 def __get_filename_from_cd(cd):
     """
         Get filename from content-disposition
     """
     if not cd:
         return None
     fname = findall('filename=(.+)', cd)
     if len(fname) == 0:
         return None
     return fname[0]
 
+def __did_file_fully_download(file_path, expected_size):
+    actual_size = os.stat(file_path).st_size
+    return actual_size == expected_size, actual_size
+
 
 def is_recent_file(path, age=2592000):
     """
         Check whether a file path exists, is empty and older than 1 month
     """
     try:
         return os.path.exists(path) and os.path.getsize(path) > 0 and (time() - os.path.getmtime(path) < age)
```

### Comparing `gitlab-ps-utils-0.8.0/gitlab_ps_utils/json_utils.py` & `gitlab_ps_utils-0.9.0/gitlab_ps_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/gitlab_ps_utils/jsondiff.py` & `gitlab_ps_utils-0.9.0/gitlab_ps_utils/jsondiff.py`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/gitlab_ps_utils/list_utils.py` & `gitlab_ps_utils-0.9.0/gitlab_ps_utils/list_utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/gitlab_ps_utils/logger.py` & `gitlab_ps_utils-0.9.0/gitlab_ps_utils/logger.py`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/gitlab_ps_utils/misc_utils.py` & `gitlab_ps_utils-0.9.0/gitlab_ps_utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/gitlab_ps_utils/processes.py` & `gitlab_ps_utils-0.9.0/gitlab_ps_utils/processes.py`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/gitlab_ps_utils/string_utils.py` & `gitlab_ps_utils-0.9.0/gitlab_ps_utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-ps-utils-0.8.0/pyproject.toml` & `gitlab_ps_utils-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitlab-ps-utils"
-version = "0.8.0"
+version = "0.9.0"
 description = "Shared python utilities used by GitLab Professional Services tooling"
 authors = ["GitLab Professional Services <proserv@gitlab.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/gitlab-org/professional-services-automation/gitlab-ps-utils"
 
 [tool.poetry.dependencies]
```

### Comparing `gitlab-ps-utils-0.8.0/PKG-INFO` & `gitlab_ps_utils-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: gitlab-ps-utils
-Version: 0.8.0
+Version: 0.9.0
 Summary: Shared python utilities used by GitLab Professional Services tooling
 Home-page: https://gitlab.com/gitlab-org/professional-services-automation/gitlab-ps-utils
 License: MIT
 Author: GitLab Professional Services
 Author-email: proserv@gitlab.com
 Requires-Python: >=3.8.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: tqdm (>=4.61.0,<5.0.0)
 Requires-Dist: xmltodict (>=0.12.0,<0.13.0)
 Description-Content-Type: text/markdown
 
 # GitLab PS Utils
```

