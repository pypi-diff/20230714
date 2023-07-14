# Comparing `tmp/pyalslib-1.1.3.tar.gz` & `tmp/pyalslib-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalslib-1.1.3.tar", last modified: Wed Jun 14 05:39:20 2023, max compression
+gzip compressed data, was "pyalslib-1.1.4.tar", last modified: Fri Jul 14 21:47:23 2023, max compression
```

## Comparing `pyalslib-1.1.3.tar` & `pyalslib-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-14 05:39:20.688910 pyalslib-1.1.3/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    35149 2023-06-13 17:51:00.000000 pyalslib-1.1.3/LICENSE
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-06-14 05:39:20.687910 pyalslib-1.1.3/PKG-INFO
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1186 2023-06-13 17:51:00.000000 pyalslib-1.1.3/README.md
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-14 05:39:20.686910 pyalslib-1.1.3/pyalslib/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     5995 2023-06-13 17:51:00.000000 pyalslib-1.1.3/pyalslib/ALSCatalog.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     7265 2023-06-13 17:51:00.000000 pyalslib-1.1.3/pyalslib/ALSCatalogCache.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    17129 2023-06-14 05:38:51.000000 pyalslib-1.1.3/pyalslib/ALSGraph.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1859 2023-06-13 17:51:00.000000 pyalslib-1.1.3/pyalslib/ALSRewriter.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    17375 2023-06-13 17:51:00.000000 pyalslib-1.1.3/pyalslib/ALSSMT.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2117 2023-06-13 17:51:00.000000 pyalslib-1.1.3/pyalslib/Utility.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    11381 2023-06-13 18:06:04.000000 pyalslib-1.1.3/pyalslib/YosysHelper.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      405 2023-06-14 05:39:07.000000 pyalslib-1.1.3/pyalslib/__init__.py
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-14 05:39:20.687910 pyalslib-1.1.3/pyalslib.egg-info/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-06-14 05:39:20.000000 pyalslib-1.1.3/pyalslib.egg-info/PKG-INFO
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      365 2023-06-14 05:39:20.000000 pyalslib-1.1.3/pyalslib.egg-info/SOURCES.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)        1 2023-06-14 05:39:20.000000 pyalslib-1.1.3/pyalslib.egg-info/dependency_links.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)       49 2023-06-14 05:39:20.000000 pyalslib-1.1.3/pyalslib.egg-info/requires.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)        9 2023-06-14 05:39:20.000000 pyalslib-1.1.3/pyalslib.egg-info/top_level.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)       38 2023-06-14 05:39:20.688910 pyalslib-1.1.3/setup.cfg
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1735 2023-06-14 05:39:03.000000 pyalslib-1.1.3/setup.py
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-07-14 21:47:23.955770 pyalslib-1.1.4/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    35149 2023-06-22 16:36:50.000000 pyalslib-1.1.4/LICENSE
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-07-14 21:47:23.955770 pyalslib-1.1.4/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1186 2023-06-22 16:36:50.000000 pyalslib-1.1.4/README.md
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-07-14 21:47:23.955770 pyalslib-1.1.4/pyalslib/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     5995 2023-06-22 16:36:50.000000 pyalslib-1.1.4/pyalslib/ALSCatalog.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     7265 2023-06-22 16:36:50.000000 pyalslib-1.1.4/pyalslib/ALSCatalogCache.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    17129 2023-06-22 16:36:50.000000 pyalslib-1.1.4/pyalslib/ALSGraph.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1723 2023-07-14 13:18:33.000000 pyalslib-1.1.4/pyalslib/ALSRewriter.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    17375 2023-06-22 16:36:50.000000 pyalslib-1.1.4/pyalslib/ALSSMT.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2117 2023-06-22 16:36:50.000000 pyalslib-1.1.4/pyalslib/Utility.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    11381 2023-07-14 13:18:53.000000 pyalslib-1.1.4/pyalslib/YosysHelper.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      405 2023-07-14 13:07:47.000000 pyalslib-1.1.4/pyalslib/__init__.py
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-07-14 21:47:23.955770 pyalslib-1.1.4/pyalslib.egg-info/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-07-14 21:47:23.000000 pyalslib-1.1.4/pyalslib.egg-info/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      365 2023-07-14 21:47:23.000000 pyalslib-1.1.4/pyalslib.egg-info/SOURCES.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)        1 2023-07-14 21:47:23.000000 pyalslib-1.1.4/pyalslib.egg-info/dependency_links.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)       49 2023-07-14 21:47:23.000000 pyalslib-1.1.4/pyalslib.egg-info/requires.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)        9 2023-07-14 21:47:23.000000 pyalslib-1.1.4/pyalslib.egg-info/top_level.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)       38 2023-07-14 21:47:23.955770 pyalslib-1.1.4/setup.cfg
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1735 2023-07-14 13:07:43.000000 pyalslib-1.1.4/setup.py
```

### Comparing `pyalslib-1.1.3/LICENSE` & `pyalslib-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.3/PKG-INFO` & `pyalslib-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalslib
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
 Home-page: https://github.com/SalvatoreBarone/pyALSlib
 Author: Salvatore Barone
 Author-email: salvatore.barone@unina.it
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/pyALSlib/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/pyALSlib
 Keywords: Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
```

### Comparing `pyalslib-1.1.3/README.md` & `pyalslib-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.3/pyalslib/ALSCatalog.py` & `pyalslib-1.1.4/pyalslib/ALSCatalog.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.3/pyalslib/ALSCatalogCache.py` & `pyalslib-1.1.4/pyalslib/ALSCatalogCache.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.3/pyalslib/ALSGraph.py` & `pyalslib-1.1.4/pyalslib/ALSGraph.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.3/pyalslib/ALSRewriter.py` & `pyalslib-1.1.4/pyalslib/ALSRewriter.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,26 +24,23 @@
 
     def generate_hdl(self, pareto_set, out_dir):
         for n, c in enumerate(pareto_set):
             self.rewrite_and_save("original", c, f"{out_dir}/variant_{n:05d}")
 
     def rewrite_and_save(self, design_name, solution, destination):
         configuration = self.problem.matter_configuration(solution)
-        self.helper.load_design(design_name)
-        self.helper.to_aig(configuration)
-        self.helper.reverse_splitnets()
-        self.helper.clean()
-        self.helper.opt()
-        self.helper.write_verilog(destination)
-        self.helper.reset()
-        self.helper.delete()
+        self.rewrite_and_save_configured(design_name, configuration, destination)
 
     def rewrite_and_save_configured(self, design_name, configuration, destination):
+        self.helper.reset()
+        self.helper.delete()
         self.helper.load_design(design_name)
         self.helper.to_aig(configuration)
         self.helper.reverse_splitnets()
         self.helper.clean()
         self.helper.opt()
         self.helper.write_verilog(destination)
         self.helper.reset()
         self.helper.delete()
+
+
```

### Comparing `pyalslib-1.1.3/pyalslib/ALSSMT.py` & `pyalslib-1.1.4/pyalslib/ALSSMT.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.3/pyalslib/Utility.py` & `pyalslib-1.1.4/pyalslib/Utility.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.3/pyalslib/YosysHelper.py` & `pyalslib-1.1.4/pyalslib/YosysHelper.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.3/pyalslib.egg-info/PKG-INFO` & `pyalslib-1.1.4/pyalslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalslib
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
 Home-page: https://github.com/SalvatoreBarone/pyALSlib
 Author: Salvatore Barone
 Author-email: salvatore.barone@unina.it
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/pyALSlib/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/pyALSlib
 Keywords: Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
```

### Comparing `pyalslib-1.1.3/setup.py` & `pyalslib-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pyalslib",
-    version="1.1.3",
+    version="1.1.4",
     description="Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique",
     long_description="Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique. Please visit https://github.com/SalvatoreBarone/pyALSlib",
     url="https://github.com/SalvatoreBarone/pyALSlib",
     author="Salvatore Barone",
     author_email="salvatore.barone@unina.it",
     classifiers=[
         "Intended Audience :: Information Technology",
```

