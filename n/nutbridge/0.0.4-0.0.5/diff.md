# Comparing `tmp/nutbridge-0.0.4.tar.gz` & `tmp/nutbridge-0.0.5.tar.gz`

## Comparing `nutbridge-0.0.4.tar` & `nutbridge-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 nutbridge-0.0.4/.env
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 nutbridge-0.0.4/requirements.txt
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nutbridge-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0   258935 2020-02-02 00:00:00.000000 nutbridge-0.0.4/example/test.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nutbridge-0.0.4/nutbridge/__init__.py
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 nutbridge-0.0.4/nutbridge/nutbridge.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 nutbridge-0.0.4/.gitignore
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nutbridge-0.0.4/README.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nutbridge-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 nutbridge-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 nutbridge-0.0.5/.env
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 nutbridge-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nutbridge-0.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0   258935 2020-02-02 00:00:00.000000 nutbridge-0.0.5/example/test.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nutbridge-0.0.5/nutbridge/__init__.py
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 nutbridge-0.0.5/nutbridge/nutbridge.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 nutbridge-0.0.5/.gitignore
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nutbridge-0.0.5/README.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nutbridge-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 nutbridge-0.0.5/PKG-INFO
```

### Comparing `nutbridge-0.0.4/requirements.txt` & `nutbridge-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `nutbridge-0.0.4/example/test.png` & `nutbridge-0.0.5/example/test.png`

 * *Files identical despite different names*

### Comparing `nutbridge-0.0.4/nutbridge/nutbridge.py` & `nutbridge-0.0.5/nutbridge/nutbridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,20 +171,23 @@
     response = client.list_objects_v2(
         Bucket=bucket,
         Prefix=remote_folder_path,
     )
 
     for obj in response["Contents"]:
         relative_path = obj["Key"].replace(remote_folder_path, "")
-        local_path = os.path.join(local_folder_path, relative_path.lstrip("/"))
+        local_path = os.path.join(local_folder_path, relative_path[1:])
         os.makedirs(os.path.dirname(local_path), exist_ok=True)
 
+        if relative_path[-1] == "/":
+            continue
+
         with tqdm(
             total=round(obj["Size"] / 1024 / 1024, 2),
-            desc=f"Downloading object to {local_path}",
+            desc=f"Downloading object from {obj['Key']} to {local_path}",
             unit="MB",
             colour="cyan",
             bar_format="{l_bar}{bar:10}| {n_fmt}/{total_fmt} [{elapsed}<{remaining}, {rate_fmt}{postfix}]",
         ) as pbar:
             client.download_file(
                 bucket,
                 obj["Key"],
```

### Comparing `nutbridge-0.0.4/pyproject.toml` & `nutbridge-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "nutbridge"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Charis Giaralis", email="charis.giaralis@squaredev.io" },
 ]
 description = "A small wrapper on top of boto3 to make it easier to work with AWS S3"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `nutbridge-0.0.4/PKG-INFO` & `nutbridge-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutbridge
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small wrapper on top of boto3 to make it easier to work with AWS S3
 Project-URL: Homepage, https://github.com/squaredev-io/nutbridge
 Project-URL: Bug Tracker, https://github.com/squaredev-io/nutbridge/issues
 Author-email: Charis Giaralis <charis.giaralis@squaredev.io>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

