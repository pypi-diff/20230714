# Comparing `tmp/abin_sim-1.1.3.tar.gz` & `tmp/abin_sim-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abin_sim-1.1.3.tar", max compression
+gzip compressed data, was "abin_sim-1.1.4.tar", max compression
```

## Comparing `abin_sim-1.1.3.tar` & `abin_sim-1.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      260 2023-07-06 11:46:40.980893 abin_sim-1.1.3/LICENSE
--rw-r--r--   0        0        0     8594 2023-07-06 11:46:40.980893 abin_sim-1.1.3/README.md
--rw-r--r--   0        0        0       21 2023-07-06 11:46:40.980893 abin_sim-1.1.3/abin_sim/__init__.py
--rw-r--r--   0        0        0     8435 2023-07-06 11:46:40.980893 abin_sim-1.1.3/abin_sim/cli.py
--rw-r--r--   0        0        0      194 2023-07-06 11:46:40.980893 abin_sim-1.1.3/abin_sim/config.py
--rw-r--r--   0        0        0     1174 2023-07-06 11:46:40.980893 abin_sim-1.1.3/abin_sim/core/file_manager.py
--rw-r--r--   0        0        0     5830 2023-07-06 11:46:40.980893 abin_sim-1.1.3/abin_sim/core/functions.py
--rw-r--r--   0        0        0     1190 2023-07-06 11:46:40.980893 abin_sim-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     9483 1970-01-01 00:00:00.000000 abin_sim-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-07-14 14:26:11.781594 abin_sim-1.1.4/LICENSE
+-rw-r--r--   0        0        0     8594 2023-07-14 14:26:11.781594 abin_sim-1.1.4/README.md
+-rw-r--r--   0        0        0       21 2023-07-14 14:26:11.781594 abin_sim-1.1.4/abin_sim/__init__.py
+-rw-r--r--   0        0        0     8435 2023-07-14 14:26:11.781594 abin_sim-1.1.4/abin_sim/cli.py
+-rw-r--r--   0        0        0      194 2023-07-14 14:26:11.781594 abin_sim-1.1.4/abin_sim/config.py
+-rw-r--r--   0        0        0     1174 2023-07-14 14:26:11.781594 abin_sim-1.1.4/abin_sim/core/file_manager.py
+-rw-r--r--   0        0        0     5836 2023-07-14 14:26:11.781594 abin_sim-1.1.4/abin_sim/core/functions.py
+-rw-r--r--   0        0        0     1190 2023-07-14 14:26:11.781594 abin_sim-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     9483 1970-01-01 00:00:00.000000 abin_sim-1.1.4/PKG-INFO
```

### Comparing `abin_sim-1.1.3/README.md` & `abin_sim-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `abin_sim-1.1.3/abin_sim/cli.py` & `abin_sim-1.1.4/abin_sim/cli.py`

 * *Files identical despite different names*

### Comparing `abin_sim-1.1.3/abin_sim/core/file_manager.py` & `abin_sim-1.1.4/abin_sim/core/file_manager.py`

 * *Files identical despite different names*

### Comparing `abin_sim-1.1.3/abin_sim/core/functions.py` & `abin_sim-1.1.4/abin_sim/core/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,17 @@
 ) -> dict:
     with open(file, 'r') as f:
         content = f.readlines()
 
     contentList = [x.strip().split('^#')[0].split('=', 1) for x in content if '=' in x.split('^#')[0]]
     contentDict = dict(contentList)
     for k, v in contentList:
-        for i, x in enumerate(v.split('$')[1:]):
-            key = re.findall(r'\w+', x)[0]
-            v = v.replace('$' + key, contentDict[key])
+        # for i, x in enumerate(v.split('$')[1:]):
+        #     key = re.findall(r'\w+', x)[0]
+        #     v = v.replace('$' + key, contentDict[key])
         if '=' in v:
             contentDict[k] = f"'{v.strip()}'"
         else:
             contentDict[k] = v.strip()
 
     return json.dumps(contentDict)
```

### Comparing `abin_sim-1.1.3/pyproject.toml` & `abin_sim-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abin-sim"
-version = "1.1.3"
+version = "1.1.4"
 description = "ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech"
 license = "BeerWare"
 authors = ["Bonatto <andrebonatto@gmail.com>"]
 readme = "README.md"
 packages = [{include = "abin_sim"}]
 classifiers = [
     "Topic :: Utilities",
```

### Comparing `abin_sim-1.1.3/PKG-INFO` & `abin_sim-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abin-sim
-Version: 1.1.3
+Version: 1.1.4
 Summary: ABIN é um CLI para interagir com a API do Vault e auxiliar os Desenvolvedores nos projetos da SIMTech
 License: Beerware
 Author: Bonatto
 Author-email: andrebonatto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

