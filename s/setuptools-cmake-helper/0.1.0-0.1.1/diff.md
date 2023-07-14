# Comparing `tmp/setuptools-cmake-helper-0.1.0.tar.gz` & `tmp/setuptools-cmake-helper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-cmake-helper-0.1.0.tar", last modified: Fri Jul 14 20:06:28 2023, max compression
+gzip compressed data, was "setuptools-cmake-helper-0.1.1.tar", last modified: Fri Jul 14 20:53:06 2023, max compression
```

## Comparing `setuptools-cmake-helper-0.1.0.tar` & `setuptools-cmake-helper-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:06:28.085203 setuptools-cmake-helper-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:06:28.081203 setuptools-cmake-helper-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:06:28.081203 setuptools-cmake-helper-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 20:06:28.085203 setuptools-cmake-helper-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 20:06:28.085203 setuptools-cmake-helper-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:06:28.081203 setuptools-cmake-helper-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:06:28.081203 setuptools-cmake-helper-0.1.0/src/setuptools_cmake_helper/
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/src/setuptools_cmake_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 20:06:27.000000 setuptools-cmake-helper-0.1.0/src/setuptools_cmake_helper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:06:28.081203 setuptools-cmake-helper-0.1.0/src/setuptools_cmake_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 20:06:28.000000 setuptools-cmake-helper-0.1.0/src/setuptools_cmake_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-14 20:06:28.000000 setuptools-cmake-helper-0.1.0/src/setuptools_cmake_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 20:06:28.000000 setuptools-cmake-helper-0.1.0/src/setuptools_cmake_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 20:06:28.000000 setuptools-cmake-helper-0.1.0/src/setuptools_cmake_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 20:06:28.000000 setuptools-cmake-helper-0.1.0/src/setuptools_cmake_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:06:28.081203 setuptools-cmake-helper-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/tests/test_build_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:06:28.081203 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:06:28.081203 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/cmake_src/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/cmake_src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/cmake_src/cmake_lib.c
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/cmake_src/cmake_lib.h
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:06:28.081203 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/python_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:06:28.081203 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/python_src/test_package/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/python_src/test_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:06:28.085203 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/wrap_src/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-14 20:06:18.000000 setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/wrap_src/wrap.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.120028 setuptools-cmake-helper-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.116028 setuptools-cmake-helper-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.116028 setuptools-cmake-helper-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 20:53:06.120028 setuptools-cmake-helper-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 20:53:06.120028 setuptools-cmake-helper-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.116028 setuptools-cmake-helper-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.116028 setuptools-cmake-helper-0.1.1/src/setuptools_cmake_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/src/setuptools_cmake_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 20:53:06.000000 setuptools-cmake-helper-0.1.1/src/setuptools_cmake_helper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.120028 setuptools-cmake-helper-0.1.1/src/setuptools_cmake_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 20:53:06.000000 setuptools-cmake-helper-0.1.1/src/setuptools_cmake_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-14 20:53:06.000000 setuptools-cmake-helper-0.1.1/src/setuptools_cmake_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 20:53:06.000000 setuptools-cmake-helper-0.1.1/src/setuptools_cmake_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 20:53:06.000000 setuptools-cmake-helper-0.1.1/src/setuptools_cmake_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 20:53:06.000000 setuptools-cmake-helper-0.1.1/src/setuptools_cmake_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.120028 setuptools-cmake-helper-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_build_projects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.120028 setuptools-cmake-helper-0.1.1/tests/test_package_cython/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_cython/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.120028 setuptools-cmake-helper-0.1.1/tests/test_package_cython/cmake_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_cython/cmake_src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_cython/cmake_src/cmake_lib.c
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_cython/cmake_src/cmake_lib.h
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_cython/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.116028 setuptools-cmake-helper-0.1.1/tests/test_package_cython/python_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.120028 setuptools-cmake-helper-0.1.1/tests/test_package_cython/python_src/test_package/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_cython/python_src/test_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_cython/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_cython/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.120028 setuptools-cmake-helper-0.1.1/tests/test_package_cython/wrap_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_cython/wrap_src/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_cython/wrap_src/_native.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.120028 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.120028 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/cmake_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/cmake_src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/cmake_src/cmake_lib.c
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/cmake_src/cmake_lib.h
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.116028 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/python_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.120028 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/python_src/test_package/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/python_src/test_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:53:06.120028 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/wrap_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-14 20:52:54.000000 setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/wrap_src/wrap.c
```

### Comparing `setuptools-cmake-helper-0.1.0/.github/dependabot.yml` & `setuptools-cmake-helper-0.1.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `setuptools-cmake-helper-0.1.0/.github/workflows/ci.yml` & `setuptools-cmake-helper-0.1.1/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
       - name: Download all the dists
         uses: actions/download-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
 
       - name: Install built wheel
-        run: python -m pip install "$(ls dist/*.whl)[test]"
+        run: python -m pip install "$(ls dist/*.whl)[cython,test]"
 
       - name: run pytest
         run: python -m pytest --cov
 
       - name: codecov
         uses: codecov/codecov-action@v3
```

### Comparing `setuptools-cmake-helper-0.1.0/.gitignore` & `setuptools-cmake-helper-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `setuptools-cmake-helper-0.1.0/LICENSE` & `setuptools-cmake-helper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-cmake-helper-0.1.0/PKG-INFO` & `setuptools-cmake-helper-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-cmake-helper
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simpler helper to build a Python C/C++ Extension using CMake
 Author: Henrique Gemignani Passos Lima
 Project-URL: Homepage, https://github.com/henriquegemignani/setuptools-cmake-helper
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `setuptools-cmake-helper-0.1.0/pyproject.toml` & `setuptools-cmake-helper-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `setuptools-cmake-helper-0.1.0/src/setuptools_cmake_helper/__init__.py` & `setuptools-cmake-helper-0.1.1/src/setuptools_cmake_helper/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         cmake_project: os.PathLike,
         cmake_targets: list[str],
         *args,
         **kw,
     ):
         super().__init__(name, sources, *args, **kw)
         self.cmake_options = {
-            "dir": os.fspath(cmake_project.resolve()),
+            "dir": os.fspath(Path(cmake_project).resolve()),
             "targets": cmake_targets,
         }
 
 
 class CMakeBuild(build_ext):
     def run(self):
         try:
@@ -126,15 +126,16 @@
     from Cython.Build.Dependencies import default_create_extension
 
     def cythonize_extensions(
         ext_modules: list[CMakeExtension], include_paths: list[str], language_level: str
     ):
         def create_extension(template, kwds):
             """"""
-            kwds["cmake_options"] = template.cmake_options
+            kwds["cmake_project"] = template.cmake_options["dir"]
+            kwds["cmake_targets"] = template.cmake_options["targets"]
             return default_create_extension(template, kwds)
 
         cythonized_ext_modules = cythonize(
             ext_modules,
             include_path=include_paths,
             compiler_directives={
                 "embedsignature": True,
```

### Comparing `setuptools-cmake-helper-0.1.0/src/setuptools_cmake_helper.egg-info/PKG-INFO` & `setuptools-cmake-helper-0.1.1/src/setuptools_cmake_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-cmake-helper
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simpler helper to build a Python C/C++ Extension using CMake
 Author: Henrique Gemignani Passos Lima
 Project-URL: Homepage, https://github.com/henriquegemignani/setuptools-cmake-helper
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/cmake_src/CMakeLists.txt` & `setuptools-cmake-helper-0.1.1/tests/test_package_cython/cmake_src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/setup.py` & `setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-cmake-helper-0.1.0/tests/test_package_simple_cpp/wrap_src/wrap.c` & `setuptools-cmake-helper-0.1.1/tests/test_package_simple_cpp/wrap_src/wrap.c`

 * *Files identical despite different names*

