# Comparing `tmp/mobicontrol-1.1.0.tar.gz` & `tmp/mobicontrol-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobicontrol-1.1.0.tar", last modified: Fri Jul 14 11:41:03 2023, max compression
+gzip compressed data, was "mobicontrol-1.2.0.tar", last modified: Fri Jul 14 12:16:29 2023, max compression
```

## Comparing `mobicontrol-1.1.0.tar` & `mobicontrol-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/mobicontrol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/mobicontrol/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/cli/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/cli/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/mobicontrol/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/client/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/client/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/client/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/mobicontrol/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/mobicontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 11:41:03.000000 mobicontrol-1.1.0/mobicontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 11:41:03.000000 mobicontrol-1.1.0/mobicontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:41:03.000000 mobicontrol-1.1.0/mobicontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 11:41:03.000000 mobicontrol-1.1.0/mobicontrol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 11:41:03.000000 mobicontrol-1.1.0/mobicontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 11:41:03.000000 mobicontrol-1.1.0/mobicontrol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:41:03.455071 mobicontrol-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 11:40:39.000000 mobicontrol-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:16:29.222600 mobicontrol-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 12:16:29.222600 mobicontrol-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:16:29.218599 mobicontrol-1.2.0/mobicontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:16:01.000000 mobicontrol-1.2.0/mobicontrol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:16:29.218599 mobicontrol-1.2.0/mobicontrol/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-14 12:16:01.000000 mobicontrol-1.2.0/mobicontrol/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-14 12:16:01.000000 mobicontrol-1.2.0/mobicontrol/cli/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-14 12:16:01.000000 mobicontrol-1.2.0/mobicontrol/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-14 12:16:01.000000 mobicontrol-1.2.0/mobicontrol/cli/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:16:29.222600 mobicontrol-1.2.0/mobicontrol/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-14 12:16:01.000000 mobicontrol-1.2.0/mobicontrol/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-14 12:16:01.000000 mobicontrol-1.2.0/mobicontrol/client/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-14 12:16:01.000000 mobicontrol-1.2.0/mobicontrol/client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-14 12:16:01.000000 mobicontrol-1.2.0/mobicontrol/client/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 12:16:01.000000 mobicontrol-1.2.0/mobicontrol/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:16:29.218599 mobicontrol-1.2.0/mobicontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 12:16:29.000000 mobicontrol-1.2.0/mobicontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 12:16:29.000000 mobicontrol-1.2.0/mobicontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:16:29.000000 mobicontrol-1.2.0/mobicontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 12:16:29.000000 mobicontrol-1.2.0/mobicontrol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 12:16:29.000000 mobicontrol-1.2.0/mobicontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 12:16:29.000000 mobicontrol-1.2.0/mobicontrol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:16:29.222600 mobicontrol-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 12:16:01.000000 mobicontrol-1.2.0/setup.py
```

### Comparing `mobicontrol-1.1.0/mobicontrol/cli/__init__.py` & `mobicontrol-1.2.0/mobicontrol/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.1.0/mobicontrol/cli/apply.py` & `mobicontrol-1.2.0/mobicontrol/cli/apply.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             "Authorization": f"Bearer {github_token}",
         },
     )
 
     data = assets.json()
 
     for asset in data:
-        if filename in asset["url"]:
+        if filename in asset["name"]:
             asset = asset
             break
     else:
         raise click.ClickException(f"Could not find asset matching '{filename}'.")
 
     file = requests.get(
         asset["url"],
@@ -144,19 +144,32 @@
         raise click.ClickException(str(e))
 
 
 @mobicontrol.command()
 @click.option("--file", type=click.Path(exists=True), required=True)
 @click.pass_context
 def apply(ctx, file: str):
-    with open(file) as f:
-        data = yaml.safe_load(f)
+    apply_paths = []
+    if os.path.isdir(file):
+        for root, dirs, files in os.walk(file):
+            for file in files:
+                apply_paths.append(os.path.join(root, file))
+    else:
+        files = [file]
+
+    click.echo(f"Found {len(apply_paths)} files to apply.")
+    for file in apply_paths:
+        click.echo(f"Applying {file}.")
+        with open(file) as f:
+            data = yaml.safe_load(f)
+
+        if data["resourceType"] == "policy":
+            apply_policy(ctx, data)
 
-    if data["resourceType"] == "policy":
-        apply_policy(ctx, data)
+        click.echo(f"{file} applied.")
 
 
 @mobicontrol.command()
 @click.option("--file", type=click.Path(exists=True), required=True)
 @click.pass_context
 def delete(ctx, file: str):
     with open(file) as f:
```

### Comparing `mobicontrol-1.1.0/mobicontrol/cli/apps.py` & `mobicontrol-1.2.0/mobicontrol/cli/apps.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.1.0/mobicontrol/cli/policies.py` & `mobicontrol-1.2.0/mobicontrol/cli/policies.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.1.0/mobicontrol/client/__init__.py` & `mobicontrol-1.2.0/mobicontrol/client/__init__.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.1.0/mobicontrol/client/apps.py` & `mobicontrol-1.2.0/mobicontrol/client/apps.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.1.0/mobicontrol/client/auth.py` & `mobicontrol-1.2.0/mobicontrol/client/auth.py`

 * *Files identical despite different names*

### Comparing `mobicontrol-1.1.0/mobicontrol/client/policies.py` & `mobicontrol-1.2.0/mobicontrol/client/policies.py`

 * *Files identical despite different names*

