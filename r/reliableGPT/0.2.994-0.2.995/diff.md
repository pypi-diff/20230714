# Comparing `tmp/reliableGPT-0.2.994.tar.gz` & `tmp/reliableGPT-0.2.995.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.994.tar", last modified: Fri Jul 14 01:20:41 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.995.tar", last modified: Fri Jul 14 01:23:07 2023, max compression
```

## Comparing `reliableGPT-0.2.994.tar` & `reliableGPT-0.2.995.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:20:41.114093 reliableGPT-0.2.994/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.994/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 01:20:41.113919 reliableGPT-0.2.994/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8826 2023-07-14 01:03:18.000000 reliableGPT-0.2.994/README.md
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.994/pyproject.toml
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:20:41.112451 reliableGPT-0.2.994/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 01:20:41.000000 reliableGPT-0.2.994/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      361 2023-07-14 01:20:41.000000 reliableGPT-0.2.994/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-14 01:20:41.000000 reliableGPT-0.2.994/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       63 2023-07-14 01:20:41.000000 reliableGPT-0.2.994/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-14 01:20:41.000000 reliableGPT-0.2.994/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:20:41.113631 reliableGPT-0.2.994/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3148 2023-07-14 01:03:18.000000 reliableGPT-0.2.994/reliablegpt/Alerting.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    22294 2023-07-14 01:13:13.000000 reliableGPT-0.2.994/reliablegpt/IndividualRequest.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.994/reliablegpt/Model.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       58 2023-07-10 15:34:25.000000 reliableGPT-0.2.994/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5281 2023-07-14 01:20:06.000000 reliableGPT-0.2.994/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-14 01:20:41.114134 reliableGPT-0.2.994/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      418 2023-07-14 01:20:16.000000 reliableGPT-0.2.994/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:23:07.610204 reliableGPT-0.2.995/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.995/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 01:23:07.610049 reliableGPT-0.2.995/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8826 2023-07-14 01:03:18.000000 reliableGPT-0.2.995/README.md
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.995/pyproject.toml
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:23:07.608768 reliableGPT-0.2.995/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-14 01:23:07.000000 reliableGPT-0.2.995/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      361 2023-07-14 01:23:07.000000 reliableGPT-0.2.995/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-14 01:23:07.000000 reliableGPT-0.2.995/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       63 2023-07-14 01:23:07.000000 reliableGPT-0.2.995/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-14 01:23:07.000000 reliableGPT-0.2.995/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-14 01:23:07.609769 reliableGPT-0.2.995/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3148 2023-07-14 01:03:18.000000 reliableGPT-0.2.995/reliablegpt/Alerting.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    22309 2023-07-14 01:22:49.000000 reliableGPT-0.2.995/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.995/reliablegpt/Model.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       58 2023-07-10 15:34:25.000000 reliableGPT-0.2.995/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5281 2023-07-14 01:20:06.000000 reliableGPT-0.2.995/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-14 01:23:07.610243 reliableGPT-0.2.995/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      418 2023-07-14 01:22:57.000000 reliableGPT-0.2.995/setup.py
```

### Comparing `reliableGPT-0.2.994/LICENSE` & `reliableGPT-0.2.995/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.994/README.md` & `reliableGPT-0.2.995/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.994/reliablegpt/Alerting.py` & `reliableGPT-0.2.995/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.994/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.995/reliablegpt/IndividualRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
   def handle_unhandled_exception(self, e):
     self.print_verbose(colored("UNHANDLED EXCEPTION OCCURRED", "red"))
     if self.alerting:
       self.alerting.add_error(error_type="Unhandled Exception", error_description=traceback.format_exc())
 
   def print_verbose(self, print_statement):
-    posthog.capture('ishaan_admin@berri.ai', 'print_verbose', str(print_statement)[:2000])
+    posthog.capture('ishaan_admin@berri.ai', 'print_verbose', {'rgpt_data': str(print_statement)[:2000]})
     if self.verbose:
       print(colored("Individual Request: " + str(print_statement), "blue"))
 
   def start_cooldown(self):
     self.set_cooldown = True
     self.cooldown_start_time = time.time()
```

### Comparing `reliableGPT-0.2.994/reliablegpt/Model.py` & `reliableGPT-0.2.995/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.994/reliablegpt/main.py` & `reliableGPT-0.2.995/reliablegpt/main.py`

 * *Files identical despite different names*

