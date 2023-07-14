# Comparing `tmp/PyVCG-1.0.0.tar.gz` & `tmp/PyVCG-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyVCG-1.0.0.tar", last modified: Tue Jul 11 11:10:24 2023, max compression
+gzip compressed data, was "PyVCG-1.0.1.tar", last modified: Fri Jul 14 07:41:35 2023, max compression
```

## Comparing `PyVCG-1.0.0.tar` & `PyVCG-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-11 11:10:24.279796 PyVCG-1.0.0/
--rw-r--r--   0 florian   (1000) florian   (1000)    35149 2023-06-30 05:59:33.000000 PyVCG-1.0.0/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     3295 2023-07-11 11:10:24.279796 PyVCG-1.0.0/PKG-INFO
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-11 11:10:24.279796 PyVCG-1.0.0/PyVCG.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     3295 2023-07-11 11:10:24.000000 PyVCG-1.0.0/PyVCG.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      399 2023-07-11 11:10:24.000000 PyVCG-1.0.0/PyVCG.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-07-11 11:10:24.000000 PyVCG-1.0.0/PyVCG.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       12 2023-07-11 11:10:24.000000 PyVCG-1.0.0/PyVCG.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        6 2023-07-11 11:10:24.000000 PyVCG-1.0.0/PyVCG.egg-info/top_level.txt
--rw-r--r--   0 florian   (1000) florian   (1000)     2301 2023-07-11 11:06:20.000000 PyVCG-1.0.0/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-11 11:10:24.279796 PyVCG-1.0.0/pyvcg/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-30 18:37:56.000000 PyVCG-1.0.0/pyvcg/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-11 11:10:24.279796 PyVCG-1.0.0/pyvcg/driver/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-09 17:34:46.000000 PyVCG-1.0.0/pyvcg/driver/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    20285 2023-07-11 11:06:20.000000 PyVCG-1.0.0/pyvcg/driver/cvc5_api.py
--rw-r--r--   0 florian   (1000) florian   (1000)    13462 2023-07-11 11:06:20.000000 PyVCG-1.0.0/pyvcg/driver/file_smtlib.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6402 2023-07-09 17:38:38.000000 PyVCG-1.0.0/pyvcg/graph.py
--rw-r--r--   0 florian   (1000) florian   (1000)    41486 2023-07-11 11:06:20.000000 PyVCG-1.0.0/pyvcg/smt.py
--rw-r--r--   0 florian   (1000) florian   (1000)     3160 2023-07-04 10:59:04.000000 PyVCG-1.0.0/pyvcg/vcg.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1953 2023-07-11 11:07:56.000000 PyVCG-1.0.0/pyvcg/version.py
--rw-r--r--   0 florian   (1000) florian   (1000)       91 2023-07-11 11:10:24.279796 PyVCG-1.0.0/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2088 2023-07-09 18:13:59.000000 PyVCG-1.0.0/setup.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-11 11:10:24.279796 PyVCG-1.0.0/tests/
--rw-r--r--   0 florian   (1000) florian   (1000)     1851 2023-06-30 09:23:58.000000 PyVCG-1.0.0/tests/testGraphSimple.py
--rw-r--r--   0 florian   (1000) florian   (1000)     3603 2023-07-09 17:37:20.000000 PyVCG-1.0.0/tests/testSimpleVCG.py
--rw-r--r--   0 florian   (1000) florian   (1000)    35917 2023-07-11 11:06:20.000000 PyVCG-1.0.0/tests/testSmt.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-14 07:41:35.467819 PyVCG-1.0.1/
+-rw-r--r--   0 florian   (1000) florian   (1000)    35149 2023-06-30 05:59:33.000000 PyVCG-1.0.1/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     3299 2023-07-14 07:41:35.467819 PyVCG-1.0.1/PKG-INFO
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-14 07:41:35.467819 PyVCG-1.0.1/PyVCG.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     3299 2023-07-14 07:41:35.000000 PyVCG-1.0.1/PyVCG.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      399 2023-07-14 07:41:35.000000 PyVCG-1.0.1/PyVCG.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-07-14 07:41:35.000000 PyVCG-1.0.1/PyVCG.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       12 2023-07-14 07:41:35.000000 PyVCG-1.0.1/PyVCG.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        6 2023-07-14 07:41:35.000000 PyVCG-1.0.1/PyVCG.egg-info/top_level.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)     2301 2023-07-11 11:06:20.000000 PyVCG-1.0.1/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-14 07:41:35.467819 PyVCG-1.0.1/pyvcg/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-30 18:37:56.000000 PyVCG-1.0.1/pyvcg/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-14 07:41:35.467819 PyVCG-1.0.1/pyvcg/driver/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-07-09 17:34:46.000000 PyVCG-1.0.1/pyvcg/driver/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    20285 2023-07-11 11:06:20.000000 PyVCG-1.0.1/pyvcg/driver/cvc5_api.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    13462 2023-07-11 11:06:20.000000 PyVCG-1.0.1/pyvcg/driver/file_smtlib.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6402 2023-07-09 17:38:38.000000 PyVCG-1.0.1/pyvcg/graph.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    41586 2023-07-14 07:41:10.000000 PyVCG-1.0.1/pyvcg/smt.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3160 2023-07-04 10:59:04.000000 PyVCG-1.0.1/pyvcg/vcg.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1953 2023-07-14 07:41:32.000000 PyVCG-1.0.1/pyvcg/version.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       91 2023-07-14 07:41:35.467819 PyVCG-1.0.1/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2092 2023-07-14 07:41:10.000000 PyVCG-1.0.1/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-07-14 07:41:35.467819 PyVCG-1.0.1/tests/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1851 2023-06-30 09:23:58.000000 PyVCG-1.0.1/tests/testGraphSimple.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3603 2023-07-09 17:37:20.000000 PyVCG-1.0.1/tests/testSimpleVCG.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    36399 2023-07-14 07:41:10.000000 PyVCG-1.0.1/tests/testSmt.py
```

### Comparing `PyVCG-1.0.0/LICENSE` & `PyVCG-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.0/PKG-INFO` & `PyVCG-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVCG
-Version: 1.0.0
+Version: 1.0.1
 Summary: Verification Condition Generator
 Home-page: https://github.com/florianschanda/PyVCG
 Author: Florian Schanda
 Author-email: florian@schanda.org.uk
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/florianschanda/PyVCG/issues
 Project-URL: Documentation, https://github.com/pages/florianschanda/PyVCG/
@@ -12,15 +12,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Compilers
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.8, <=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Verification Condition Generator
 
 PyVCG is a utility library to generate VCs directly for
 [CVC5](https://cvc5.github.io) or standard-compliant
```

### Comparing `PyVCG-1.0.0/PyVCG.egg-info/PKG-INFO` & `PyVCG-1.0.1/PyVCG.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyVCG
-Version: 1.0.0
+Version: 1.0.1
 Summary: Verification Condition Generator
 Home-page: https://github.com/florianschanda/PyVCG
 Author: Florian Schanda
 Author-email: florian@schanda.org.uk
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/florianschanda/PyVCG/issues
 Project-URL: Documentation, https://github.com/pages/florianschanda/PyVCG/
@@ -12,15 +12,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Compilers
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.8, <=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Verification Condition Generator
 
 PyVCG is a utility library to generate VCs directly for
 [CVC5](https://cvc5.github.io) or standard-compliant
```

### Comparing `PyVCG-1.0.0/README.md` & `PyVCG-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.0/pyvcg/driver/cvc5_api.py` & `PyVCG-1.0.1/pyvcg/driver/cvc5_api.py`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.0/pyvcg/driver/file_smtlib.py` & `PyVCG-1.0.1/pyvcg/driver/file_smtlib.py`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.0/pyvcg/graph.py` & `PyVCG-1.0.1/pyvcg/graph.py`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.0/pyvcg/smt.py` & `PyVCG-1.0.1/pyvcg/smt.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,14 +283,15 @@
         assert False
 
     def visit_constant_declaration(self, node, tr_symbol, tr_value):
         assert isinstance(node, Constant_Declaration)
 
     def visit_function_declaration(self, node, tr_sort, tr_body):
         assert isinstance(node, Function_Declaration)
+        node.function.walk(self)
         self.logics.add("functions")
 
     def visit_assertion(self, node, tr_expression):
         assert isinstance(node, Assertion)
 
     def visit_enumeration_declaration(self, node):
         assert isinstance(node, Enumeration_Declaration)
@@ -321,14 +322,16 @@
         if node.name == "Seq":
             self.logics.add("sequences")
         else:
             assert False, "unexpected base sort %s" % node.name
 
     def visit_function(self, node):
         assert isinstance(node, Function)
+        for param in node.parameters:
+            param.walk(self)
         self.logics.add("functions")
 
     def visit_enumeration(self, node):
         assert isinstance(node, Enumeration)
         self.logics.add("datatypes")
 
     def visit_record(self, node):
```

### Comparing `PyVCG-1.0.0/pyvcg/vcg.py` & `PyVCG-1.0.1/pyvcg/vcg.py`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.0/pyvcg/version.py` & `PyVCG-1.0.1/pyvcg/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 ##  General Public License for more details.                                ##
 ##                                                                          ##
 ##  You should have received a copy of the GNU General Public License       ##
 ##  along with PyVCG. If not, see <http://www.gnu.org/licenses/>.           ##
 ##                                                                          ##
 ##############################################################################
 
-VERSION_TUPLE = (1, 0, 0)
+VERSION_TUPLE = (1, 0, 1)
 VERSION_SUFFIX = ""
 
 PYVCG_VERSION = ("%u.%u.%u" % VERSION_TUPLE) + \
     ("-%s" % VERSION_SUFFIX if VERSION_SUFFIX else "")
 
 FULL_NAME = "PyVCG %s" % PYVCG_VERSION
```

### Comparing `PyVCG-1.0.0/setup.py` & `PyVCG-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=project_urls["Source Code"],
     project_urls=project_urls,
     license="GNU General Public License v3",
     packages=["pyvcg", "pyvcg.driver"],
     install_requires=["cvc5>=1.0.5"],
-    python_requires=">=3.9, <4",
+    python_requires=">=3.8, <=3.10",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: POSIX :: Linux",
         "Topic :: Scientific/Engineering :: Mathematics",
```

### Comparing `PyVCG-1.0.0/tests/testGraphSimple.py` & `PyVCG-1.0.1/tests/testGraphSimple.py`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.0/tests/testSimpleVCG.py` & `PyVCG-1.0.1/tests/testSimpleVCG.py`

 * *Files identical despite different names*

### Comparing `PyVCG-1.0.0/tests/testSmt.py` & `PyVCG-1.0.1/tests/testSmt.py`

 * *Files 0% similar despite different names*

```diff
@@ -980,14 +980,31 @@
             (get-value (a))
             (get-value (b))
             (exit)
             """
         )
         self.assertValue("b", self.values["a"] * 2)
 
+    def test_UF_Unused(self):
+        s_par = smt.Bound_Variable(smt.BUILTIN_STRING, "x")
+        s_fun = smt.Function("potato", smt.BUILTIN_BOOLEAN, s_par)
+        self.script.add_statement(smt.Function_Declaration(s_fun))
+
+        self.assertResult(
+            "sat",
+            """
+            (set-logic QF_UFS)
+            (set-option :produce-models true)
+
+            (declare-fun potato (String) Bool)
+            (check-sat)
+            (exit)
+            """
+        )
+
     def test_ITE(self):
         sym_a = smt.Constant(smt.BUILTIN_INTEGER, "a")
         self.script.add_statement(
             smt.Constant_Declaration(sym_a,
                                      relevant=True))
         sym_b = smt.Constant(smt.BUILTIN_STRING, "b")
         self.script.add_statement(
```

