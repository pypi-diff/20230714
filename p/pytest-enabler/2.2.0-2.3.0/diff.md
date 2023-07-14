# Comparing `tmp/pytest-enabler-2.2.0.tar.gz` & `tmp/pytest-enabler-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-enabler-2.2.0.tar", last modified: Mon Jun 26 02:26:47 2023, max compression
+gzip compressed data, was "pytest-enabler-2.3.0.tar", last modified: Fri Jul 14 01:07:17 2023, max compression
```

## Comparing `pytest-enabler-2.2.0.tar` & `pytest-enabler-2.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.850073 pytest-enabler-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.846073 pytest-enabler-2.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.846073 pytest-enabler-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-26 02:26:47.850073 pytest-enabler-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.846073 pytest-enabler-2.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.846073 pytest-enabler-2.2.0/pytest_enabler/
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/pytest_enabler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/pytest_enabler/default.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.850073 pytest-enabler-2.2.0/pytest_enabler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-26 02:26:47.000000 pytest-enabler-2.2.0/pytest_enabler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-26 02:26:47.000000 pytest-enabler-2.2.0/pytest_enabler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 02:26:47.000000 pytest-enabler-2.2.0/pytest_enabler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 02:26:47.000000 pytest-enabler-2.2.0/pytest_enabler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-26 02:26:47.000000 pytest-enabler-2.2.0/pytest_enabler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 02:26:47.000000 pytest-enabler-2.2.0/pytest_enabler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-26 02:26:47.850073 pytest-enabler-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.850073 pytest-enabler-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/tests/test_enabler.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.691273 pytest-enabler-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.683273 pytest-enabler-2.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.683273 pytest-enabler-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-14 01:07:17.691273 pytest-enabler-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.687273 pytest-enabler-2.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.687273 pytest-enabler-2.3.0/pytest_enabler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/pytest_enabler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/pytest_enabler/default.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.687273 pytest-enabler-2.3.0/pytest_enabler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-14 01:07:17.000000 pytest-enabler-2.3.0/pytest_enabler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-14 01:07:17.000000 pytest-enabler-2.3.0/pytest_enabler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:07:17.000000 pytest-enabler-2.3.0/pytest_enabler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 01:07:17.000000 pytest-enabler-2.3.0/pytest_enabler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-14 01:07:17.000000 pytest-enabler-2.3.0/pytest_enabler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 01:07:17.000000 pytest-enabler-2.3.0/pytest_enabler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-14 01:07:17.691273 pytest-enabler-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:07:17.691273 pytest-enabler-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/tests/test_enabler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-14 01:06:54.000000 pytest-enabler-2.3.0/tox.ini
```

### Comparing `pytest-enabler-2.2.0/.github/workflows/main.yml` & `pytest-enabler-2.3.0/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -68,29 +68,29 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Run tests
+      - name: Run
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
@@ -113,16 +113,16 @@
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.11-dev
+          python-version: 3.x
       - name: Install tox
         run: |
           python -m pip install tox
-      - name: Release
+      - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `pytest-enabler-2.2.0/LICENSE` & `pytest-enabler-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.2.0/NEWS.rst` & `pytest-enabler-2.3.0/NEWS.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v2.3.0
+======
+
+Features
+--------
+
+- Added support for pytest-ignore-flaky.
+
+
+Bugfixes
+--------
+
+- If pytest-cov is explicitly enabled, bypass special handling. (#8)
+
+
 v2.2.0
 ======
 
 Features
 --------
 
 - Enabler plugin now includes a default config, enabling the known supported plugins. It's no longer necessary for each project to supply the config to enable plugins.
```

### Comparing `pytest-enabler-2.2.0/PKG-INFO` & `pytest-enabler-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-enabler
-Version: 2.2.0
+Version: 2.3.0
 Summary: Enable installed pytest plugins
 Home-page: https://github.com/jaraco/pytest-enabler
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -54,7 +54,8 @@
 
 - pytest-black
 - pytest-cov
 - pytest-flake8
 - pytest-mypy
 - pytest-ruff
 - pytest-xdist
+- pytest-ignore-flaky
```

### Comparing `pytest-enabler-2.2.0/README.rst` & `pytest-enabler-2.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -36,7 +36,8 @@
 
 - pytest-black
 - pytest-cov
 - pytest-flake8
 - pytest-mypy
 - pytest-ruff
 - pytest-xdist
+- pytest-ignore-flaky
```

### Comparing `pytest-enabler-2.2.0/docs/conf.py` & `pytest-enabler-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.2.0/pytest.ini` & `pytest-enabler-2.3.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.2.0/pytest_enabler/__init__.py` & `pytest-enabler-2.3.0/pytest_enabler/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,15 +70,21 @@
     pytest_cov runs its command-line checks so early that no hooks
     can intervene. By now, the hook that installs the plugin has
     already run and failed to enable the plugin. So, parse the config
     specially and re-run the hook.
     """
     if 'cov' not in plugins:
         return
+
+    if early_config.pluginmanager.getplugin('_cov'):
+        # cov was explicitly configured (#8)
+        return
+
     _remove_deps()
     # important: parse all known args to ensure pytest-cov can configure
     # itself based on other plugins like pytest-xdist (see #1).
     parser.parse_known_and_unknown_args(args, early_config.known_args_namespace)
+
     with contextlib.suppress(ImportError):
         import pytest_cov.plugin
 
-        pytest_cov.plugin.pytest_load_initial_conftests(early_config, parser, args)
+    pytest_cov.plugin.pytest_load_initial_conftests(early_config, parser, args)
```

### Comparing `pytest-enabler-2.2.0/pytest_enabler.egg-info/PKG-INFO` & `pytest-enabler-2.3.0/pytest_enabler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-enabler
-Version: 2.2.0
+Version: 2.3.0
 Summary: Enable installed pytest plugins
 Home-page: https://github.com/jaraco/pytest-enabler
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -54,7 +54,8 @@
 
 - pytest-black
 - pytest-cov
 - pytest-flake8
 - pytest-mypy
 - pytest-ruff
 - pytest-xdist
+- pytest-ignore-flaky
```

### Comparing `pytest-enabler-2.2.0/pytest_enabler.egg-info/SOURCES.txt` & `pytest-enabler-2.3.0/pytest_enabler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.2.0/setup.cfg` & `pytest-enabler-2.3.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -35,21 +35,21 @@
 	pytest >= 6
 	pytest-checkdocs >= 2.4
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
-	pytest-enabler >= 1.3
+	pytest-enabler >= 2.2
 	pytest-ruff
 	
 	types-toml
 docs = 
 	sphinx >= 3.5
-	jaraco.packaging >= 9
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
 
 [options.entry_points]
 pytest11 = 
 	plugin-enabled options = pytest_enabler
```

### Comparing `pytest-enabler-2.2.0/tests/test_enabler.py` & `pytest-enabler-2.3.0/tests/test_enabler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import subprocess
 import sys
 from unittest import mock
 
 import pytest
 
 import pytest_enabler as enabler
 
@@ -17,30 +18,43 @@
     config.pluginmanager.has_plugin = lambda name: name == 'black'
     args = []
     enabler.pytest_load_initial_conftests(config, None, args)
     assert args == ['--black']
 
 
 def test_pytest_addoption_override(pyproject):
-    pyproject.write_text('[tool.pytest-enabler.black]\naddopts="--black2"\n')
+    pyproject.write_text(
+        '[tool.pytest-enabler.black]\naddopts="--black2"\n',
+        encoding='utf-8',
+    )
     config = mock.MagicMock()
     config.pluginmanager.has_plugin = lambda name: name == 'black'
     args = []
     enabler.pytest_load_initial_conftests(config, None, args)
     assert args == ['--black2']
 
 
 def test_pytest_addoption_disable(pyproject):
-    pyproject.write_text('[tool.pytest-enabler.black]\n#addopts="--black"\n')
+    pyproject.write_text(
+        '[tool.pytest-enabler.black]\n#addopts="--black"\n',
+        encoding='utf-8',
+    )
     config = mock.MagicMock()
     config.pluginmanager.has_plugin = lambda name: name == 'black'
     args = []
     enabler.pytest_load_initial_conftests(config, None, args)
     assert args == []
 
 
 def test_remove_deps(monkeypatch):
     """
     Invoke _remove_deps to push coverage.
     """
     monkeypatch.setattr(sys, 'modules', dict(sys.modules))
     enabler._remove_deps()
+
+
+def test_coverage_explicit(tmp_path, monkeypatch):
+    monkeypatch.chdir(tmp_path)
+    test = tmp_path.joinpath('test_x.py')
+    test.write_text('def test_x():\n    pass\n', encoding='utf-8')
+    subprocess.check_call([sys.executable, '-m', 'pytest', '--cov'])
```

### Comparing `pytest-enabler-2.2.0/tox.ini` & `pytest-enabler-2.3.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-[tox]
-toxworkdir={env:TOX_WORK_DIR:.tox}
-
-
 [testenv]
 deps =
 setenv =
 	PYTHONWARNDEFAULTENCODING = 1
 commands =
 	pytest {posargs}
 usedevelop = True
```

