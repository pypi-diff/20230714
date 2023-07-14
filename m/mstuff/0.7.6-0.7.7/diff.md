# Comparing `tmp/mstuff-0.7.6.tar.gz` & `tmp/mstuff-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mstuff-0.7.6.tar", last modified: Wed Apr 12 04:05:57 2023, max compression
+gzip compressed data, was "mstuff-0.7.7.tar", last modified: Fri Jul 14 02:42:06 2023, max compression
```

## Comparing `mstuff-0.7.6.tar` & `mstuff-0.7.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 04:05:57.496019 mstuff-0.7.6/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      120 2023-04-12 04:05:57.495856 mstuff-0.7.6/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:02.000000 mstuff-0.7.6/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 04:05:57.495020 mstuff-0.7.6/mstuff/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      163 2023-03-08 18:10:18.000000 mstuff-0.7.6/mstuff/__init__.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     3837 2023-03-18 01:39:41.000000 mstuff-0.7.6/mstuff/http.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     3615 2023-03-15 21:27:41.000000 mstuff-0.7.6/mstuff/mstuff.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-04-12 04:05:57.495694 mstuff-0.7.6/mstuff.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      120 2023-04-12 04:05:57.000000 mstuff-0.7.6/mstuff.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      225 2023-04-12 04:05:57.000000 mstuff-0.7.6/mstuff.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-04-12 04:05:57.000000 mstuff-0.7.6/mstuff.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       17 2023-04-12 04:05:57.000000 mstuff-0.7.6/mstuff.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        7 2023-04-12 04:05:57.000000 mstuff-0.7.6/mstuff.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      186 2023-04-12 04:05:53.000000 mstuff-0.7.6/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-04-12 04:05:57.496063 mstuff-0.7.6/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-07-14 02:42:06.865858 mstuff-0.7.7/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      120 2023-07-14 02:42:06.865581 mstuff-0.7.7/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:02.000000 mstuff-0.7.7/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-07-14 02:42:06.864521 mstuff-0.7.7/mstuff/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      163 2023-03-08 18:10:18.000000 mstuff-0.7.7/mstuff/__init__.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     3836 2023-07-03 15:22:37.000000 mstuff-0.7.7/mstuff/http.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     3716 2023-07-03 15:22:50.000000 mstuff-0.7.7/mstuff/mstuff.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-07-14 02:42:06.865322 mstuff-0.7.7/mstuff.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      120 2023-07-14 02:42:06.000000 mstuff-0.7.7/mstuff.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      225 2023-07-14 02:42:06.000000 mstuff-0.7.7/mstuff.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-07-14 02:42:06.000000 mstuff-0.7.7/mstuff.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       17 2023-07-14 02:42:06.000000 mstuff-0.7.7/mstuff.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        7 2023-07-14 02:42:06.000000 mstuff-0.7.7/mstuff.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      186 2023-07-14 02:41:59.000000 mstuff-0.7.7/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-07-14 02:42:06.865954 mstuff-0.7.7/setup.cfg
```

### Comparing `mstuff-0.7.6/mstuff/http.py` & `mstuff-0.7.7/mstuff/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,11 +137,10 @@
         data=None,
         params=None,
         headers=None,
         status_checker=_default_resp_checker,
         **kwargs
 ):
     resp = requests.request(method, path, json=json, data=data, params=params, headers=headers, **kwargs)
-
     if status_checker is not None:
         status_checker(resp)
     return resp
```

### Comparing `mstuff-0.7.6/mstuff/mstuff.py` & `mstuff-0.7.7/mstuff/mstuff.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,34 +12,32 @@
 
 from mstuff.http import http_get
 
 _suppress_version_warning = False
 
 
 def warn_if_old(mod_name):
-    resp = http_get(f"https://pypi.org/project/{mod_name}", status_checker=None)
+    # need trailing slash in url below. It should be an automatic redirect, but I was having issues...
+    resp = http_get(f"https://pypi.org/project/{mod_name}/", status_checker=None)
     if resp.status_code == 404:
         print(f"package {mod_name} does not yet exist?")
         return
-
     try:
         this_version = pkg_resources.get_distribution(mod_name).version
     except pkg_resources.DistributionNotFound:
         this_version = None
 
-
     # https://stackoverflow.com/a/27239645/6596010
     def versions(package_name):
         url = "https://pypi.org/pypi/%s/json" % (package_name,)
         data = json.loads(requests.get(url).text)
         versions = list(data["releases"].keys())
         versions.sort(key=StrictVersion)
         return versions
 
-
     online_versions = versions(mod_name)
     latest_version = online_versions[len(online_versions) - 1]
     if this_version != latest_version:
         if not _suppress_version_warning:
             print(
                 f"WARNING: You are using {mod_name} {this_version} but the latest version is {latest_version}. In the terminal use `python -m pip install {mod_name} --upgrade` to update."
             )
```

