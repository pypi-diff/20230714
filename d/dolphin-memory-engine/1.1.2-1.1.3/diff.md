# Comparing `tmp/dolphin-memory-engine-1.1.2.tar.gz` & `tmp/dolphin-memory-engine-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolphin-memory-engine-1.1.2.tar", last modified: Wed Sep  7 09:05:30 2022, max compression
+gzip compressed data, was "dolphin-memory-engine-1.1.3.tar", last modified: Fri Jul 14 15:54:33 2023, max compression
```

## Comparing `dolphin-memory-engine-1.1.2.tar` & `dolphin-memory-engine-1.1.3.tar`

### file list

```diff
@@ -1,56 +1,61 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.551880 dolphin-memory-engine-1.1.2/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.499688 dolphin-memory-engine-1.1.2/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.509454 dolphin-memory-engine-1.1.2/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     4560 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/.github/workflows/python.yml
--rw-r--r--   0 runner     (501) staff       (20)      376 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/.gitmodules
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.509858 dolphin-memory-engine-1.1.2/Docs/
--rw-r--r--   0 runner     (501) staff       (20)    24055 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Docs/screenshot.png
--rw-r--r--   0 runner     (501) staff       (20)     1066 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       55 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     2341 2022-09-07 09:05:30.552114 dolphin-memory-engine-1.1.2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1600 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.524011 dolphin-memory-engine-1.1.2/Source/
--rwxr-xr-x   0 runner     (501) staff       (20)      411 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/.clang-format
--rwxr-xr-x   0 runner     (501) staff       (20)      656 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.534551 dolphin-memory-engine-1.1.2/Source/Common/
--rwxr-xr-x   0 runner     (501) staff       (20)      203 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/Common/CommonTypes.h
--rwxr-xr-x   0 runner     (501) staff       (20)     1328 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/Common/CommonUtils.h
--rw-r--r--   0 runner     (501) staff       (20)    12480 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/Common/MemoryCommon.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1379 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/Common/MemoryCommon.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.540607 dolphin-memory-engine-1.1.2/Source/DolphinProcess/
--rw-r--r--   0 runner     (501) staff       (20)     4575 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/DolphinProcess/DolphinAccessor.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1376 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/DolphinProcess/DolphinAccessor.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.541653 dolphin-memory-engine-1.1.2/Source/DolphinProcess/Dummy/
--rw-r--r--   0 runner     (501) staff       (20)      597 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/DolphinProcess/Dummy/DummyDolphinProcess.cpp
--rw-r--r--   0 runner     (501) staff       (20)      486 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/DolphinProcess/Dummy/DummyDolphinProcess.h
--rw-r--r--   0 runner     (501) staff       (20)     1120 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/DolphinProcess/IDolphinProcess.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.542509 dolphin-memory-engine-1.1.2/Source/DolphinProcess/Linux/
--rw-r--r--   0 runner     (501) staff       (20)     5387 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/DolphinProcess/Linux/LinuxDolphinProcess.cpp
--rw-r--r--   0 runner     (501) staff       (20)      568 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/DolphinProcess/Linux/LinuxDolphinProcess.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.543333 dolphin-memory-engine-1.1.2/Source/DolphinProcess/Windows/
--rwxr-xr-x   0 runner     (501) staff       (20)     5742 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/DolphinProcess/Windows/WindowsDolphinProcess.cpp
--rw-r--r--   0 runner     (501) staff       (20)      590 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/DolphinProcess/Windows/WindowsDolphinProcess.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.544227 dolphin-memory-engine-1.1.2/Source/MemoryScanner/
--rw-r--r--   0 runner     (501) staff       (20)    18818 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/MemoryScanner/MemoryScanner.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5118 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/MemoryScanner/MemoryScanner.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.545124 dolphin-memory-engine-1.1.2/Source/MemoryWatch/
--rw-r--r--   0 runner     (501) staff       (20)     9041 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/MemoryWatch/MemWatchEntry.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2202 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Source/MemoryWatch/MemWatchEntry.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.546429 dolphin-memory-engine-1.1.2/Tools/
--rwxr-xr-x   0 runner     (501) staff       (20)       78 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/Tools/format.sh
--rw-r--r--   0 runner     (501) staff       (20)   340887 2022-09-07 09:05:29.000000 dolphin-memory-engine-1.1.2/_dolphin_memory_engine.cpp
--rw-r--r--   0 runner     (501) staff       (20)     6834 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/_dolphin_memory_engine.pyx
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.546857 dolphin-memory-engine-1.1.2/dolphin_memory_engine/
--rw-r--r--   0 runner     (501) staff       (20)       37 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/dolphin_memory_engine/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.550787 dolphin-memory-engine-1.1.2/dolphin_memory_engine.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2341 2022-09-07 09:05:30.000000 dolphin-memory-engine-1.1.2/dolphin_memory_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1226 2022-09-07 09:05:30.000000 dolphin-memory-engine-1.1.2/dolphin_memory_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-09-07 09:05:30.000000 dolphin-memory-engine-1.1.2/dolphin_memory_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-09-07 09:04:58.000000 dolphin-memory-engine-1.1.2/dolphin_memory_engine.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       45 2022-09-07 09:05:30.000000 dolphin-memory-engine-1.1.2/dolphin_memory_engine.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      193 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      837 2022-09-07 09:05:30.553101 dolphin-memory-engine-1.1.2/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     5099 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-09-07 09:05:30.551379 dolphin-memory-engine-1.1.2/test/
--rw-r--r--   0 runner     (501) staff       (20)      254 2022-09-07 09:04:40.000000 dolphin-memory-engine-1.1.2/test/test_native.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.912472 dolphin-memory-engine-1.1.3/
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.365356 dolphin-memory-engine-1.1.3/.github/
+-rw-rw-rw-   0        0        0      730 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/.github/dependabot.yml
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.381073 dolphin-memory-engine-1.1.3/.github/workflows/
+-rw-rw-rw-   0        0        0      618 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/.github/workflows/dependabot.yml
+-rw-rw-rw-   0        0        0     4584 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/.github/workflows/python.yml
+-rw-rw-rw-   0        0        0      772 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/.gitignore
+-rw-rw-rw-   0        0        0        0 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/.gitmodules
+-rw-rw-rw-   0        0        0      432 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/.pre-commit-config.yaml
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.381073 dolphin-memory-engine-1.1.3/Docs/
+-rw-rw-rw-   0        0        0    24055 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Docs/screenshot.png
+-rw-rw-rw-   0        0        0     1087 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2173 2023-07-14 15:54:33.912472 dolphin-memory-engine-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1379 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.381073 dolphin-memory-engine-1.1.3/Source/
+-rw-rw-rw-   0        0        0      428 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/.clang-format
+-rw-rw-rw-   0        0        0      656 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.381073 dolphin-memory-engine-1.1.3/Source/Common/
+-rw-rw-rw-   0        0        0      216 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/Common/CommonTypes.h
+-rw-rw-rw-   0        0        0     2855 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/Common/CommonUtils.h
+-rw-rw-rw-   0        0        0    12988 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/Common/MemoryCommon.cpp
+-rw-rw-rw-   0        0        0     1766 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/Common/MemoryCommon.h
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.381073 dolphin-memory-engine-1.1.3/Source/DolphinProcess/
+-rw-rw-rw-   0        0        0     6014 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/DolphinProcess/DolphinAccessor.cpp
+-rw-rw-rw-   0        0        0     1521 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/DolphinProcess/DolphinAccessor.h
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.381073 dolphin-memory-engine-1.1.3/Source/DolphinProcess/Dummy/
+-rw-rw-rw-   0        0        0      624 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/DolphinProcess/Dummy/DummyDolphinProcess.cpp
+-rw-rw-rw-   0        0        0      505 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/DolphinProcess/Dummy/DummyDolphinProcess.h
+-rw-rw-rw-   0        0        0     1393 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/DolphinProcess/IDolphinProcess.h
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.381073 dolphin-memory-engine-1.1.3/Source/DolphinProcess/Linux/
+-rw-rw-rw-   0        0        0     6809 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/DolphinProcess/Linux/LinuxDolphinProcess.cpp
+-rw-rw-rw-   0        0        0      594 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/DolphinProcess/Linux/LinuxDolphinProcess.h
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.381073 dolphin-memory-engine-1.1.3/Source/DolphinProcess/Windows/
+-rw-rw-rw-   0        0        0     7240 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/DolphinProcess/Windows/WindowsDolphinProcess.cpp
+-rw-rw-rw-   0        0        0      618 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/DolphinProcess/Windows/WindowsDolphinProcess.h
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.381073 dolphin-memory-engine-1.1.3/Source/MemoryScanner/
+-rw-rw-rw-   0        0        0    17628 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/MemoryScanner/MemoryScanner.cpp
+-rw-rw-rw-   0        0        0     5279 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/MemoryScanner/MemoryScanner.h
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.381073 dolphin-memory-engine-1.1.3/Source/MemoryWatch/
+-rw-rw-rw-   0        0        0     9492 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/MemoryWatch/MemWatchEntry.cpp
+-rw-rw-rw-   0        0        0     2270 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Source/MemoryWatch/MemWatchEntry.h
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.381073 dolphin-memory-engine-1.1.3/Tools/
+-rw-rw-rw-   0        0        0       80 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/Tools/format.sh
+-rw-rw-rw-   0        0        0   349159 2023-07-14 15:54:31.000000 dolphin-memory-engine-1.1.3/_dolphin_memory_engine.cpp
+-rw-rw-rw-   0        0        0     7037 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/_dolphin_memory_engine.pyx
+-rw-rw-rw-   0        0        0     1536 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.365356 dolphin-memory-engine-1.1.3/python_src/
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.912472 dolphin-memory-engine-1.1.3/python_src/dolphin_memory_engine/
+-rw-rw-rw-   0        0        0      655 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/python_src/dolphin_memory_engine/__init__.py
+-rw-rw-rw-   0        0        0      164 2023-07-14 15:54:33.000000 dolphin-memory-engine-1.1.3/python_src/dolphin_memory_engine/version.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.912472 dolphin-memory-engine-1.1.3/python_src/dolphin_memory_engine.egg-info/
+-rw-rw-rw-   0        0        0     2173 2023-07-14 15:54:33.000000 dolphin-memory-engine-1.1.3/python_src/dolphin_memory_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1417 2023-07-14 15:54:33.000000 dolphin-memory-engine-1.1.3/python_src/dolphin_memory_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:54:33.000000 dolphin-memory-engine-1.1.3/python_src/dolphin_memory_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-14 15:54:33.000000 dolphin-memory-engine-1.1.3/python_src/dolphin_memory_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-14 15:54:33.000000 dolphin-memory-engine-1.1.3/python_src/dolphin_memory_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      151 2023-07-14 15:54:33.912472 dolphin-memory-engine-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     5223 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:54:33.912472 dolphin-memory-engine-1.1.3/tests/
+-rw-rw-rw-   0        0        0      265 2023-07-14 15:53:30.000000 dolphin-memory-engine-1.1.3/tests/test_native.py
```

### Comparing `dolphin-memory-engine-1.1.2/.github/workflows/python.yml` & `dolphin-memory-engine-1.1.3/.github/workflows/python.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,171 +1,166 @@
-name: Python Package
-
-on:
-  pull_request:
-  push:
-    branches:
-      - '*'
-    tags:
-      - '*'
-
-jobs:
-  build:
-    strategy:
-      fail-fast: false
-      matrix:
-        os:
-          - 'macos-latest'
-          - 'windows-latest'
-        python:
-          - '3.7'
-          - '3.8'
-          - '3.9'
-          - '3.10'
-          - '3.11-dev'
-
-    runs-on: ${{ matrix.os }}
-    name: Wheel for ${{ matrix.os }} (${{ matrix.python }})
-
-    steps:
-      - name: Checkout
-        uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-          submodules: 'recursive'
-
-      - name: Set up Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: "${{ matrix.python }}"
-     
-      - name: Install Python packages
-        run: python -m pip install --upgrade build pip
-
-      - name: build wheel
-        run: python -m build --wheel
-
-      - name: build sdist
-        run: python -m build --sdist
-        if: ${{ matrix.os == 'macos-latest' && matrix.python == '3.10' }}
-      
-      - name: Store the packages
-        uses: actions/upload-artifact@v3
-        with:
-          name: python-package-distributions
-          path: dist
-
-  linux-build:
-    strategy:
-      fail-fast: false
-      matrix:
-        python:
-          - 'cp37-cp37m'
-          - 'cp38-cp38'
-          - 'cp39-cp39'
-          - 'cp310-cp310'
-          - 'cp311-cp311'
-
-    runs-on: ubuntu-latest
-    container: quay.io/pypa/manylinux2014_x86_64
-    name: Wheel for Linux (${{ matrix.python }})
-
-    steps:
-      - name: Checkout
-        uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-          submodules: 'recursive'
-
-      - name: Avoid issues with Git's solution for CVE-2022-24765 breaking setuptools-scm
-        run: git config --global --add safe.directory $(pwd)
-
-      - run: /opt/python/${{ matrix.python }}/bin/python -m venv .venv
-     
-      - name: Install Python packages
-        run: .venv/bin/python -m pip install --upgrade build pip auditwheel
-
-      - name: build wheel
-        run: .venv/bin/python -m build --wheel
-
-      - name: multilinux stuff
-        run: |
-          .venv/bin/python -m auditwheel repair --plat manylinux2014_x86_64 dist/*-linux_x86_64.whl -w dist
-          rm dist/*-linux_x86_64.whl
-      
-      - name: Store the packages
-        uses: actions/upload-artifact@v3
-        with:
-          name: python-package-distributions
-          path: dist
-
-  test:
-    needs:
-      - build
-      - linux-build
-      
-    runs-on: ${{ matrix.os.image }}
-    name: ${{ matrix.os.name }} - Test Python ${{ matrix.python.version }}
-    strategy:
-      fail-fast: false
-      matrix:
-        os:
-          - {name: 'macOS', image: 'macos-latest', wheel: 'macosx_*'}
-          - {name: 'Windows', image: 'windows-latest', wheel: 'win_amd64'}
-          - {name: 'Linux', image: 'ubuntu-latest', wheel: 'manylinux2014_x86_64'}
-        python:
-          - {version: '3.7', wheel: 'cp37-cp37m'}
-          - {version: '3.8', wheel: 'cp38-cp38'}
-          - {version: '3.9', wheel: 'cp39-cp39'}
-          - {version: '3.10', wheel: 'cp310-cp310'}
-          - {version: '3.11-dev', wheel: 'cp311-cp311'}
-
-    steps:
-      - name: Checkout
-        uses: actions/checkout@v3
-
-      - name: Set up Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python.version }}
-
-      - name: Download all the dists
-        uses: actions/download-artifact@v3
-        with:
-          name: python-package-distributions
-          path: dist/
-
-      - name: Install Python packages
-        run: python -m pip install --upgrade pip pytest
-
-      - name: install built wheel
-        run: python -m pip install dist/*-${{ matrix.python.wheel }}-*${{ matrix.os.wheel }}.whl
-        shell: bash
-
-      - name: test
-        run: python -m pytest
-        working-directory: test
-
-  pypi:
-    runs-on: 'ubuntu-latest'
-    needs:
-      - test
-
-    steps:
-      - name: Download all the dists
-        uses: actions/download-artifact@v3
-        with:
-          name: python-package-distributions
-          path: dist/
-
-      - name: Publish 📦 to TestPyPI
-        if: ${{ github.ref == 'refs/heads/main' }}
-        uses: pypa/gh-action-pypi-publish@master
-        with:
-          password: ${{ secrets.testpypi_password }}
-          repository_url: https://test.pypi.org/legacy/
-      
-      - name: Publish 📦 to PyPI
-        if: ${{ startsWith(github.ref, 'refs/tags/') }}
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.pypi_password }}
+name: Python Package
+
+on:
+  pull_request:
+  push:
+    branches:
+      - '*'
+    tags:
+      - '*'
+
+jobs:
+  build:
+    strategy:
+      fail-fast: false
+      matrix:
+        os:
+          - 'macos-latest'
+          - 'windows-latest'
+        python:
+          - '3.8'
+          - '3.9'
+          - '3.10'
+          - '3.11'
+          - '3.12.0-beta - 3.12.0'
+
+    runs-on: ${{ matrix.os }}
+    name: Wheel for ${{ matrix.os }} (${{ matrix.python }})
+
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+          submodules: 'recursive'
+
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: "${{ matrix.python }}"
+     
+      - name: Install Python packages
+        run: python -m pip install --upgrade build pip
+
+      - name: build wheel
+        run: python -m build
+      
+      - name: Store the packages
+        uses: actions/upload-artifact@v3
+        with:
+          name: python-package-distributions
+          path: dist
+
+  linux-build:
+    strategy:
+      fail-fast: false
+      matrix:
+        python:
+          - 'cp38-cp38'
+          - 'cp39-cp39'
+          - 'cp310-cp310'
+          - 'cp311-cp311'
+          - 'cp312-cp312'
+
+    runs-on: ubuntu-latest
+    container: quay.io/pypa/manylinux2014_x86_64
+    name: Wheel for Linux (${{ matrix.python }})
+
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+          submodules: 'recursive'
+
+      - name: Avoid issues with Git's solution for CVE-2022-24765 breaking setuptools-scm
+        run: git config --global --add safe.directory $(pwd)
+
+      - run: /opt/python/${{ matrix.python }}/bin/python -m venv .venv
+     
+      - name: Install Python packages
+        run: .venv/bin/python -m pip install --upgrade build pip auditwheel setuptools
+
+      - name: build
+        run: .venv/bin/python -m build
+
+      - name: multilinux stuff
+        run: |
+          .venv/bin/python -m auditwheel repair --plat manylinux2014_x86_64 dist/*-linux_x86_64.whl -w dist
+          rm dist/*-linux_x86_64.whl
+      
+      - name: Store the packages
+        uses: actions/upload-artifact@v3
+        with:
+          name: python-package-distributions
+          path: dist
+
+  test:
+    needs:
+      - build
+      - linux-build
+      
+    runs-on: ${{ matrix.os.image }}
+    name: ${{ matrix.os.name }} - Test Python ${{ matrix.python.version }}
+    strategy:
+      fail-fast: false
+      matrix:
+        os:
+          - {name: 'macOS', image: 'macos-latest', wheel: 'macosx_*'}
+          - {name: 'Windows', image: 'windows-latest', wheel: 'win_amd64'}
+          - {name: 'Linux', image: 'ubuntu-latest', wheel: 'manylinux2014_x86_64'}
+        python:
+          - {version: '3.8', wheel: 'cp38-cp38'}
+          - {version: '3.9', wheel: 'cp39-cp39'}
+          - {version: '3.10', wheel: 'cp310-cp310'}
+          - {version: '3.11', wheel: 'cp311-cp311'}
+          - {version: '3.12.0-beta - 3.12.0', wheel: 'cp312-cp312'}
+
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v3
+
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python.version }}
+
+      - name: Download all the dists
+        uses: actions/download-artifact@v3
+        with:
+          name: python-package-distributions
+          path: dist/
+
+      - name: Install Python packages
+        run: python -m pip install --upgrade pip
+
+      - name: install built wheel
+        run: python -m pip install "$(ls dist/*-${{ matrix.python.wheel }}-*${{ matrix.os.wheel }}.whl)[test]"
+        shell: bash
+
+      - name: test
+        run: python -m pytest
+
+  pypi:
+    runs-on: 'ubuntu-latest'
+    needs:
+      - test
+
+    steps:
+      - name: Download all the dists
+        uses: actions/download-artifact@v3
+        with:
+          name: python-package-distributions
+          path: dist/
+
+      - name: Publish 📦 to TestPyPI
+        if: ${{ github.ref == 'refs/heads/main' }}
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          password: ${{ secrets.testpypi_password }}
+          repository-url: https://test.pypi.org/legacy/
+      
+      - name: Publish 📦 to PyPI
+        if: ${{ startsWith(github.ref, 'refs/tags/') }}
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          password: ${{ secrets.pypi_password }}
```

### Comparing `dolphin-memory-engine-1.1.2/Docs/screenshot.png` & `dolphin-memory-engine-1.1.3/Docs/screenshot.png`

 * *Files identical despite different names*

### Comparing `dolphin-memory-engine-1.1.2/LICENSE` & `dolphin-memory-engine-1.1.3/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2017 aldelaro5
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2017 aldelaro5
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `dolphin-memory-engine-1.1.2/PKG-INFO` & `dolphin-memory-engine-1.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1
-Name: dolphin-memory-engine
-Version: 1.1.2
-Summary: Hooks into the memory of a running Dolphin processes, allowing access to the game memory.
-Home-page: https://github.com/henriquegemignani/py-dolphin-memory-engine
-Author: Henrique Gemignani
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python Dolphin Memory Engine
-
-[![Travis CI Build Status](https://travis-ci.org/henriquegemignani/py-dolphin-memory-engine.svg?branch=master)](https://travis-ci.org/henriquegemignani/py-dolphin-memory-engine)
-[![AppVeyor CI Build Status](https://ci.appveyor.com/api/projects/status/i5rb9s0w1l4ahbgj?svg=true)](https://ci.appveyor.com/project/henriquegemignani/py-dolphin-memory-engine)
-
-A python library designed to read and write the emulated memory of [the Dolphin emulator](https://github.com/dolphin-emu/dolphin) during runtime. 
-
-Binary wheels are available on pypi for Python 3.6, 3.7 and 3.8. Use `python -m pip install dolphin-memory-engine` with a modern enough version.
-
-
-## System requirements
-Any x86_64 based system should work, however, Mac OS is _not_ supported. Additionally, 32-bit x86 based systems are unsupported since Dolphin dropped their support.
-
-You need to have Dolphin running ***and*** _have the emulation started_ for this program to be useful. As such, the system must meet Dolphin's [system requirements](https://github.com/dolphin-emu/dolphin#system-requirements). Additionally, at least 250 MB of free memory is required.
-
-
-## License
-This program is licensed under the MIT license which grants you the permission to do  anything you wish to with the software, as long as you preserve all copyright notices. (See the file LICENSE for the legal text.)
-
-
-## Development Help
-
-To compile the extension in debug:
-
-$ python3 -m venv venv
-$ source venv/bin/activate
-$ python -m pip install Cython pytest
-$ python setup.py build_ext -g --inplace --force
-$ python -m pytest
+Metadata-Version: 2.1
+Name: dolphin-memory-engine
+Version: 1.1.3
+Summary: Hooks into the memory of a running Dolphin processes, allowing access to the game memory.
+Author: Henrique Gemignani
+Project-URL: Homepage, https://github.com/henriquegemignani/py-dolphin-memory-engine
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+# Python Dolphin Memory Engine
+
+A python library designed to read and write the emulated memory of [the Dolphin emulator](https://github.com/dolphin-emu/dolphin) during runtime. 
+
+Binary wheels are available on pypi for Python 3.8 to 3.12. Use `python -m pip install dolphin-memory-engine`.
+
+
+## System requirements
+Any x86_64 based system should work, however, Mac OS is _not_ supported. Additionally, 32-bit x86 based systems are unsupported since Dolphin dropped their support.
+
+You need to have Dolphin running ***and*** _have the emulation started_ for this program to be useful. As such, the system must meet Dolphin's [system requirements](https://github.com/dolphin-emu/dolphin#system-requirements). Additionally, at least 250 MB of free memory is required.
+
+
+If it doesn't work, verify that you do not have the `nosuid` mount flag on your `/etc/fstab` as it can cause this command to silently fail.
+
+## License
+This program is licensed under the MIT license which grants you the permission to do  anything you wish to with the software, as long as you preserve all copyright notices. (See the file LICENSE for the legal text.)
+
+
+## Development Help
+
+To compile the extension in debug:
+
+$ python3 -m venv venv
+$ source venv/bin/activate
+$ python -m pip install Cython pytest
+$ python setup.py build_ext -g --inplace --force
+$ python -m pytest
```

### Comparing `dolphin-memory-engine-1.1.2/README.md` & `dolphin-memory-engine-1.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# Python Dolphin Memory Engine
-
-[![Travis CI Build Status](https://travis-ci.org/henriquegemignani/py-dolphin-memory-engine.svg?branch=master)](https://travis-ci.org/henriquegemignani/py-dolphin-memory-engine)
-[![AppVeyor CI Build Status](https://ci.appveyor.com/api/projects/status/i5rb9s0w1l4ahbgj?svg=true)](https://ci.appveyor.com/project/henriquegemignani/py-dolphin-memory-engine)
-
-A python library designed to read and write the emulated memory of [the Dolphin emulator](https://github.com/dolphin-emu/dolphin) during runtime. 
-
-Binary wheels are available on pypi for Python 3.6, 3.7 and 3.8. Use `python -m pip install dolphin-memory-engine` with a modern enough version.
-
-
-## System requirements
-Any x86_64 based system should work, however, Mac OS is _not_ supported. Additionally, 32-bit x86 based systems are unsupported since Dolphin dropped their support.
-
-You need to have Dolphin running ***and*** _have the emulation started_ for this program to be useful. As such, the system must meet Dolphin's [system requirements](https://github.com/dolphin-emu/dolphin#system-requirements). Additionally, at least 250 MB of free memory is required.
-
-
-## License
-This program is licensed under the MIT license which grants you the permission to do  anything you wish to with the software, as long as you preserve all copyright notices. (See the file LICENSE for the legal text.)
-
-
-## Development Help
-
-To compile the extension in debug:
-
-$ python3 -m venv venv
-$ source venv/bin/activate
-$ python -m pip install Cython pytest
-$ python setup.py build_ext -g --inplace --force
-$ python -m pytest
+# Python Dolphin Memory Engine
+
+A python library designed to read and write the emulated memory of [the Dolphin emulator](https://github.com/dolphin-emu/dolphin) during runtime. 
+
+Binary wheels are available on pypi for Python 3.8 to 3.12. Use `python -m pip install dolphin-memory-engine`.
+
+
+## System requirements
+Any x86_64 based system should work, however, Mac OS is _not_ supported. Additionally, 32-bit x86 based systems are unsupported since Dolphin dropped their support.
+
+You need to have Dolphin running ***and*** _have the emulation started_ for this program to be useful. As such, the system must meet Dolphin's [system requirements](https://github.com/dolphin-emu/dolphin#system-requirements). Additionally, at least 250 MB of free memory is required.
+
+
+If it doesn't work, verify that you do not have the `nosuid` mount flag on your `/etc/fstab` as it can cause this command to silently fail.
+
+## License
+This program is licensed under the MIT license which grants you the permission to do  anything you wish to with the software, as long as you preserve all copyright notices. (See the file LICENSE for the legal text.)
+
+
+## Development Help
+
+To compile the extension in debug:
+
+$ python3 -m venv venv
+$ source venv/bin/activate
+$ python -m pip install Cython pytest
+$ python setup.py build_ext -g --inplace --force
+$ python -m pytest
```

### Comparing `dolphin-memory-engine-1.1.2/Source/CMakeLists.txt` & `dolphin-memory-engine-1.1.3/Source/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dolphin-memory-engine-1.1.2/Source/Common/MemoryCommon.cpp` & `dolphin-memory-engine-1.1.3/Source/Common/MemoryCommon.cpp`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,508 +1,508 @@
-#include "MemoryCommon.h"
-
-#include <bitset>
-#include <cstring>
-#include <iomanip>
-#include <sstream>
-#include <vector>
-
-#include "../Common/CommonTypes.h"
-#include "../Common/CommonUtils.h"
-
-namespace Common
-{
-size_t getSizeForType(const MemType type, const size_t length)
-{
-  switch (type)
-  {
-  case MemType::type_byte:
-    return sizeof(u8);
-  case MemType::type_halfword:
-    return sizeof(u16);
-  case MemType::type_word:
-    return sizeof(u32);
-  case MemType::type_float:
-    return sizeof(float);
-  case MemType::type_double:
-    return sizeof(double);
-  case MemType::type_string:
-    return length;
-  case MemType::type_byteArray:
-    return length;
-  default:
-    return 0;
-  }
-}
-
-bool shouldBeBSwappedForType(const MemType type)
-{
-  switch (type)
-  {
-  case MemType::type_byte:
-    return false;
-  case MemType::type_halfword:
-    return true;
-  case MemType::type_word:
-    return true;
-  case MemType::type_float:
-    return true;
-  case MemType::type_double:
-    return true;
-  case MemType::type_string:
-    return false;
-  case MemType::type_byteArray:
-    return false;
-  default:
-    return false;
-  }
-}
-
-int getNbrBytesAlignementForType(const MemType type)
-{
-  switch (type)
-  {
-  case MemType::type_byte:
-    return 1;
-  case MemType::type_halfword:
-    return 2;
-  case MemType::type_word:
-    return 4;
-  case MemType::type_float:
-    return 4;
-  case MemType::type_double:
-    return 4;
-  case MemType::type_string:
-    return 1;
-  case MemType::type_byteArray:
-    return 1;
-  default:
-    return 1;
-  }
-}
-
-char* formatStringToMemory(MemOperationReturnCode& returnCode, size_t& actualLength,
-                           const std::string inputString, const MemBase base, const MemType type,
-                           const size_t length)
-{
-  if (inputString.length() == 0)
-  {
-    returnCode = MemOperationReturnCode::invalidInput;
-    return nullptr;
-  }
-
-  std::stringstream ss(inputString);
-  switch (base)
-  {
-  case MemBase::base_octal:
-    ss >> std::oct;
-    break;
-  case MemBase::base_decimal:
-    ss >> std::dec;
-    break;
-  case MemBase::base_hexadecimal:
-    ss >> std::hex;
-    break;
-  }
-
-  size_t size = getSizeForType(type, length);
-  char* buffer = new char[size];
-
-  switch (type)
-  {
-  case MemType::type_byte:
-  {
-    u8 theByte = 0;
-    if (base == MemBase::base_binary)
-    {
-      unsigned long long input = 0;
-      try
-      {
-        input = std::bitset<sizeof(u8) * 8>(inputString).to_ullong();
-      }
-      catch (std::invalid_argument)
-      {
-        delete[] buffer;
-        buffer = nullptr;
-        returnCode = MemOperationReturnCode::invalidInput;
-        return buffer;
-      }
-      theByte = static_cast<u8>(input);
-    }
-    else
-    {
-      int theByteInt = 0;
-      ss >> theByteInt;
-      if (ss.fail())
-      {
-        delete[] buffer;
-        buffer = nullptr;
-        returnCode = MemOperationReturnCode::invalidInput;
-        return buffer;
-      }
-      theByte = static_cast<u8>(theByteInt);
-    }
-
-    std::memcpy(buffer, &theByte, size);
-    actualLength = sizeof(u8);
-    break;
-  }
-
-  case MemType::type_halfword:
-  {
-    u16 theHalfword = 0;
-    if (base == MemBase::base_binary)
-    {
-      unsigned long long input = 0;
-      try
-      {
-        input = std::bitset<sizeof(u16) * 8>(inputString).to_ullong();
-      }
-      catch (std::invalid_argument)
-      {
-        delete[] buffer;
-        buffer = nullptr;
-        returnCode = MemOperationReturnCode::invalidInput;
-        return buffer;
-      }
-      theHalfword = static_cast<u16>(input);
-    }
-    else
-    {
-      ss >> theHalfword;
-      if (ss.fail())
-      {
-        delete[] buffer;
-        buffer = nullptr;
-        returnCode = MemOperationReturnCode::invalidInput;
-        return buffer;
-      }
-    }
-
-    std::memcpy(buffer, &theHalfword, size);
-    actualLength = sizeof(u16);
-    break;
-  }
-
-  case MemType::type_word:
-  {
-    u32 theWord = 0;
-    if (base == MemBase::base_binary)
-    {
-      unsigned long long input = 0;
-      try
-      {
-        input = std::bitset<sizeof(u32) * 8>(inputString).to_ullong();
-      }
-      catch (std::invalid_argument)
-      {
-        delete[] buffer;
-        buffer = nullptr;
-        returnCode = MemOperationReturnCode::invalidInput;
-        return buffer;
-      }
-      theWord = static_cast<u32>(input);
-    }
-    else
-    {
-      ss >> theWord;
-      if (ss.fail())
-      {
-        delete[] buffer;
-        buffer = nullptr;
-        returnCode = MemOperationReturnCode::invalidInput;
-        return buffer;
-      }
-    }
-
-    std::memcpy(buffer, &theWord, size);
-    actualLength = sizeof(u32);
-    break;
-  }
-
-  case MemType::type_float:
-  {
-    float theFloat = 0.0f;
-    // 9 digits is the max number of digits in a flaot that can recover any binary format
-    ss >> std::setprecision(9) >> theFloat;
-    if (ss.fail())
-    {
-      delete[] buffer;
-      buffer = nullptr;
-      returnCode = MemOperationReturnCode::invalidInput;
-      return buffer;
-    }
-    std::memcpy(buffer, &theFloat, size);
-    actualLength = sizeof(float);
-    break;
-  }
-
-  case MemType::type_double:
-  {
-    double theDouble = 0.0;
-    // 17 digits is the max number of digits in a double that can recover any binary format
-    ss >> std::setprecision(17) >> theDouble;
-    if (ss.fail())
-    {
-      delete[] buffer;
-      buffer = nullptr;
-      returnCode = MemOperationReturnCode::invalidInput;
-      return buffer;
-    }
-    std::memcpy(buffer, &theDouble, size);
-    actualLength = sizeof(double);
-    break;
-  }
-
-  case MemType::type_string:
-  {
-    if (inputString.length() > length)
-    {
-      delete[] buffer;
-      buffer = nullptr;
-      returnCode = MemOperationReturnCode::inputTooLong;
-      return buffer;
-    }
-    std::memcpy(buffer, inputString.c_str(), length);
-    actualLength = length;
-    break;
-  }
-
-  case MemType::type_byteArray:
-  {
-    std::vector<std::string> bytes;
-    std::string next;
-    for (auto i : inputString)
-    {
-      if (i == ' ')
-      {
-        if (!next.empty())
-        {
-          bytes.push_back(next);
-          next.clear();
-        }
-      }
-      else
-      {
-        next += i;
-      }
-    }
-    if (!next.empty())
-    {
-      bytes.push_back(next);
-      next.clear();
-    }
-
-    if (bytes.size() > length)
-    {
-      delete[] buffer;
-      buffer = nullptr;
-      returnCode = MemOperationReturnCode::inputTooLong;
-      return buffer;
-    }
-
-    int index = 0;
-    for (const auto& i : bytes)
-    {
-      std::stringstream byteStream(i);
-      ss >> std::hex;
-      u8 theByte = 0;
-      int theByteInt = 0;
-      ss >> theByteInt;
-      if (ss.fail())
-      {
-        delete[] buffer;
-        buffer = nullptr;
-        returnCode = MemOperationReturnCode::invalidInput;
-        return buffer;
-      }
-      theByte = static_cast<u8>(theByteInt);
-      std::memcpy(&(buffer[index]), &theByte, sizeof(u8));
-      index++;
-    }
-    actualLength = bytes.size();
-  }
-  }
-  return buffer;
-}
-
-std::string formatMemoryToString(const char* memory, const MemType type, const size_t length,
-                                 const MemBase base, const bool isUnsigned, const bool withBSwap)
-{
-  std::stringstream ss;
-  switch (base)
-  {
-  case Common::MemBase::base_octal:
-    ss << std::oct;
-    break;
-  case Common::MemBase::base_decimal:
-    ss << std::dec;
-    break;
-  case Common::MemBase::base_hexadecimal:
-    ss << std::hex << std::uppercase;
-    break;
-  }
-
-  switch (type)
-  {
-  case Common::MemType::type_byte:
-  {
-    if (isUnsigned || base == Common::MemBase::base_binary)
-    {
-      u8 unsignedByte = 0;
-      std::memcpy(&unsignedByte, memory, sizeof(u8));
-      if (base == Common::MemBase::base_binary)
-        return std::bitset<sizeof(u8) * 8>(unsignedByte).to_string();
-      // This has to be converted to an integer type because printing a uint8_t would resolve to a
-      // char and print a single character.
-      ss << static_cast<unsigned int>(unsignedByte);
-      return ss.str();
-    }
-    else
-    {
-      s8 aByte = 0;
-      std::memcpy(&aByte, memory, sizeof(s8));
-      // This has to be converted to an integer type because printing a uint8_t would resolve to a
-      // char and print a single character.  Additionaly, casting a signed type to a larger signed
-      // type will extend the sign to match the size of the destination type, this is required for
-      // signed values in decimal, but must be bypassed for other bases, this is solved by first
-      // casting to u8 then to signed int.
-      if (base == Common::MemBase::base_decimal)
-        ss << static_cast<int>(aByte);
-      else
-        ss << static_cast<int>(static_cast<u8>(aByte));
-      return ss.str();
-    }
-  }
-  case Common::MemType::type_halfword:
-  {
-    char* memoryCopy = new char[sizeof(u16)];
-    std::memcpy(memoryCopy, memory, sizeof(u16));
-    if (withBSwap)
-    {
-      u16 halfword = 0;
-      std::memcpy(&halfword, memoryCopy, sizeof(u16));
-      halfword = Common::bSwap16(halfword);
-      std::memcpy(memoryCopy, &halfword, sizeof(u16));
-    }
-
-    if (isUnsigned || base == Common::MemBase::base_binary)
-    {
-      u16 unsignedHalfword = 0;
-      std::memcpy(&unsignedHalfword, memoryCopy, sizeof(u16));
-      if (base == Common::MemBase::base_binary)
-      {
-        delete[] memoryCopy;
-        return std::bitset<sizeof(u16) * 8>(unsignedHalfword).to_string();
-      }
-      ss << unsignedHalfword;
-      delete[] memoryCopy;
-      return ss.str();
-    }
-    s16 aHalfword = 0;
-    std::memcpy(&aHalfword, memoryCopy, sizeof(s16));
-    ss << aHalfword;
-    delete[] memoryCopy;
-    return ss.str();
-  }
-  case Common::MemType::type_word:
-  {
-    char* memoryCopy = new char[sizeof(u32)];
-    std::memcpy(memoryCopy, memory, sizeof(u32));
-    if (withBSwap)
-    {
-      u32 word = 0;
-      std::memcpy(&word, memoryCopy, sizeof(u32));
-      word = Common::bSwap32(word);
-      std::memcpy(memoryCopy, &word, sizeof(u32));
-    }
-
-    if (isUnsigned || base == Common::MemBase::base_binary)
-    {
-      u32 unsignedWord = 0;
-      std::memcpy(&unsignedWord, memoryCopy, sizeof(u32));
-      if (base == Common::MemBase::base_binary)
-      {
-        delete[] memoryCopy;
-        return std::bitset<sizeof(u32) * 8>(unsignedWord).to_string();
-      }
-      ss << unsignedWord;
-      delete[] memoryCopy;
-      return ss.str();
-    }
-    s32 aWord = 0;
-    std::memcpy(&aWord, memoryCopy, sizeof(s32));
-    ss << aWord;
-    delete[] memoryCopy;
-    return ss.str();
-  }
-  case Common::MemType::type_float:
-  {
-    char* memoryCopy = new char[sizeof(u32)];
-    std::memcpy(memoryCopy, memory, sizeof(u32));
-    if (withBSwap)
-    {
-      u32 word = 0;
-      std::memcpy(&word, memoryCopy, sizeof(u32));
-      word = Common::bSwap32(word);
-      std::memcpy(memoryCopy, &word, sizeof(u32));
-    }
-
-    float aFloat = 0.0f;
-    std::memcpy(&aFloat, memoryCopy, sizeof(float));
-    // With 9 digits of precision, it is possible to convert a float back and forth to its binary
-    // representation without any loss
-    ss << std::setprecision(9) << aFloat;
-    delete[] memoryCopy;
-    return ss.str();
-  }
-  case Common::MemType::type_double:
-  {
-    char* memoryCopy = new char[sizeof(u64)];
-    std::memcpy(memoryCopy, memory, sizeof(u64));
-    if (withBSwap)
-    {
-      u64 doubleword = 0;
-      std::memcpy(&doubleword, memoryCopy, sizeof(u64));
-      doubleword = Common::bSwap64(doubleword);
-      std::memcpy(memoryCopy, &doubleword, sizeof(u64));
-    }
-
-    double aDouble = 0.0;
-    std::memcpy(&aDouble, memoryCopy, sizeof(double));
-    // With 17 digits of precision, it is possible to convert a double back and forth to its binary
-    // representation without any loss
-    ss << std::setprecision(17) << aDouble;
-    delete[] memoryCopy;
-    return ss.str();
-  }
-  case Common::MemType::type_string:
-  {
-    int actualLength = 0;
-    for (actualLength; actualLength < length; ++actualLength)
-    {
-      if (*(memory + actualLength) == 0x00)
-        break;
-    }
-    return std::string(memory, actualLength);
-  }
-  case Common::MemType::type_byteArray:
-  {
-    // Force Hexadecimal, no matter the base
-    ss << std::hex << std::uppercase;
-    for (int i = 0; i < length; ++i)
-    {
-      u8 aByte = 0;
-      std::memcpy(&aByte, memory + i, sizeof(u8));
-      ss << std::setfill('0') << std::setw(2) << static_cast<int>(aByte) << " ";
-    }
-    std::string str = ss.str();
-    // Remove the space at the end
-    str.pop_back();
-    return str;
-  }
-  default:
-    return "";
-    break;
-  }
-}
-} // namespace Common
+#include "MemoryCommon.h"
+
+#include <bitset>
+#include <cstring>
+#include <iomanip>
+#include <sstream>
+#include <vector>
+
+#include "../Common/CommonTypes.h"
+#include "../Common/CommonUtils.h"
+
+namespace Common
+{
+size_t getSizeForType(const MemType type, const size_t length)
+{
+  switch (type)
+  {
+  case MemType::type_byte:
+    return sizeof(u8);
+  case MemType::type_halfword:
+    return sizeof(u16);
+  case MemType::type_word:
+    return sizeof(u32);
+  case MemType::type_float:
+    return sizeof(float);
+  case MemType::type_double:
+    return sizeof(double);
+  case MemType::type_string:
+    return length;
+  case MemType::type_byteArray:
+    return length;
+  default:
+    return 0;
+  }
+}
+
+bool shouldBeBSwappedForType(const MemType type)
+{
+  switch (type)
+  {
+  case MemType::type_byte:
+    return false;
+  case MemType::type_halfword:
+    return true;
+  case MemType::type_word:
+    return true;
+  case MemType::type_float:
+    return true;
+  case MemType::type_double:
+    return true;
+  case MemType::type_string:
+    return false;
+  case MemType::type_byteArray:
+    return false;
+  default:
+    return false;
+  }
+}
+
+int getNbrBytesAlignementForType(const MemType type)
+{
+  switch (type)
+  {
+  case MemType::type_byte:
+    return 1;
+  case MemType::type_halfword:
+    return 2;
+  case MemType::type_word:
+    return 4;
+  case MemType::type_float:
+    return 4;
+  case MemType::type_double:
+    return 4;
+  case MemType::type_string:
+    return 1;
+  case MemType::type_byteArray:
+    return 1;
+  default:
+    return 1;
+  }
+}
+
+char* formatStringToMemory(MemOperationReturnCode& returnCode, size_t& actualLength,
+                           const std::string inputString, const MemBase base, const MemType type,
+                           const size_t length)
+{
+  if (inputString.length() == 0)
+  {
+    returnCode = MemOperationReturnCode::invalidInput;
+    return nullptr;
+  }
+
+  std::stringstream ss(inputString);
+  switch (base)
+  {
+  case MemBase::base_octal:
+    ss >> std::oct;
+    break;
+  case MemBase::base_decimal:
+    ss >> std::dec;
+    break;
+  case MemBase::base_hexadecimal:
+    ss >> std::hex;
+    break;
+  }
+
+  size_t size = getSizeForType(type, length);
+  char* buffer = new char[size];
+
+  switch (type)
+  {
+  case MemType::type_byte:
+  {
+    u8 theByte = 0;
+    if (base == MemBase::base_binary)
+    {
+      unsigned long long input = 0;
+      try
+      {
+        input = std::bitset<sizeof(u8) * 8>(inputString).to_ullong();
+      }
+      catch (std::invalid_argument)
+      {
+        delete[] buffer;
+        buffer = nullptr;
+        returnCode = MemOperationReturnCode::invalidInput;
+        return buffer;
+      }
+      theByte = static_cast<u8>(input);
+    }
+    else
+    {
+      int theByteInt = 0;
+      ss >> theByteInt;
+      if (ss.fail())
+      {
+        delete[] buffer;
+        buffer = nullptr;
+        returnCode = MemOperationReturnCode::invalidInput;
+        return buffer;
+      }
+      theByte = static_cast<u8>(theByteInt);
+    }
+
+    std::memcpy(buffer, &theByte, size);
+    actualLength = sizeof(u8);
+    break;
+  }
+
+  case MemType::type_halfword:
+  {
+    u16 theHalfword = 0;
+    if (base == MemBase::base_binary)
+    {
+      unsigned long long input = 0;
+      try
+      {
+        input = std::bitset<sizeof(u16) * 8>(inputString).to_ullong();
+      }
+      catch (std::invalid_argument)
+      {
+        delete[] buffer;
+        buffer = nullptr;
+        returnCode = MemOperationReturnCode::invalidInput;
+        return buffer;
+      }
+      theHalfword = static_cast<u16>(input);
+    }
+    else
+    {
+      ss >> theHalfword;
+      if (ss.fail())
+      {
+        delete[] buffer;
+        buffer = nullptr;
+        returnCode = MemOperationReturnCode::invalidInput;
+        return buffer;
+      }
+    }
+
+    std::memcpy(buffer, &theHalfword, size);
+    actualLength = sizeof(u16);
+    break;
+  }
+
+  case MemType::type_word:
+  {
+    u32 theWord = 0;
+    if (base == MemBase::base_binary)
+    {
+      unsigned long long input = 0;
+      try
+      {
+        input = std::bitset<sizeof(u32) * 8>(inputString).to_ullong();
+      }
+      catch (std::invalid_argument)
+      {
+        delete[] buffer;
+        buffer = nullptr;
+        returnCode = MemOperationReturnCode::invalidInput;
+        return buffer;
+      }
+      theWord = static_cast<u32>(input);
+    }
+    else
+    {
+      ss >> theWord;
+      if (ss.fail())
+      {
+        delete[] buffer;
+        buffer = nullptr;
+        returnCode = MemOperationReturnCode::invalidInput;
+        return buffer;
+      }
+    }
+
+    std::memcpy(buffer, &theWord, size);
+    actualLength = sizeof(u32);
+    break;
+  }
+
+  case MemType::type_float:
+  {
+    float theFloat = 0.0f;
+    // 9 digits is the max number of digits in a flaot that can recover any binary format
+    ss >> std::setprecision(9) >> theFloat;
+    if (ss.fail())
+    {
+      delete[] buffer;
+      buffer = nullptr;
+      returnCode = MemOperationReturnCode::invalidInput;
+      return buffer;
+    }
+    std::memcpy(buffer, &theFloat, size);
+    actualLength = sizeof(float);
+    break;
+  }
+
+  case MemType::type_double:
+  {
+    double theDouble = 0.0;
+    // 17 digits is the max number of digits in a double that can recover any binary format
+    ss >> std::setprecision(17) >> theDouble;
+    if (ss.fail())
+    {
+      delete[] buffer;
+      buffer = nullptr;
+      returnCode = MemOperationReturnCode::invalidInput;
+      return buffer;
+    }
+    std::memcpy(buffer, &theDouble, size);
+    actualLength = sizeof(double);
+    break;
+  }
+
+  case MemType::type_string:
+  {
+    if (inputString.length() > length)
+    {
+      delete[] buffer;
+      buffer = nullptr;
+      returnCode = MemOperationReturnCode::inputTooLong;
+      return buffer;
+    }
+    std::memcpy(buffer, inputString.c_str(), length);
+    actualLength = length;
+    break;
+  }
+
+  case MemType::type_byteArray:
+  {
+    std::vector<std::string> bytes;
+    std::string next;
+    for (auto i : inputString)
+    {
+      if (i == ' ')
+      {
+        if (!next.empty())
+        {
+          bytes.push_back(next);
+          next.clear();
+        }
+      }
+      else
+      {
+        next += i;
+      }
+    }
+    if (!next.empty())
+    {
+      bytes.push_back(next);
+      next.clear();
+    }
+
+    if (bytes.size() > length)
+    {
+      delete[] buffer;
+      buffer = nullptr;
+      returnCode = MemOperationReturnCode::inputTooLong;
+      return buffer;
+    }
+
+    int index = 0;
+    for (const auto& i : bytes)
+    {
+      std::stringstream byteStream(i);
+      ss >> std::hex;
+      u8 theByte = 0;
+      int theByteInt = 0;
+      ss >> theByteInt;
+      if (ss.fail())
+      {
+        delete[] buffer;
+        buffer = nullptr;
+        returnCode = MemOperationReturnCode::invalidInput;
+        return buffer;
+      }
+      theByte = static_cast<u8>(theByteInt);
+      std::memcpy(&(buffer[index]), &theByte, sizeof(u8));
+      index++;
+    }
+    actualLength = bytes.size();
+  }
+  }
+  return buffer;
+}
+
+std::string formatMemoryToString(const char* memory, const MemType type, const size_t length,
+                                 const MemBase base, const bool isUnsigned, const bool withBSwap)
+{
+  std::stringstream ss;
+  switch (base)
+  {
+  case Common::MemBase::base_octal:
+    ss << std::oct;
+    break;
+  case Common::MemBase::base_decimal:
+    ss << std::dec;
+    break;
+  case Common::MemBase::base_hexadecimal:
+    ss << std::hex << std::uppercase;
+    break;
+  }
+
+  switch (type)
+  {
+  case Common::MemType::type_byte:
+  {
+    if (isUnsigned || base == Common::MemBase::base_binary)
+    {
+      u8 unsignedByte = 0;
+      std::memcpy(&unsignedByte, memory, sizeof(u8));
+      if (base == Common::MemBase::base_binary)
+        return std::bitset<sizeof(u8) * 8>(unsignedByte).to_string();
+      // This has to be converted to an integer type because printing a uint8_t would resolve to a
+      // char and print a single character.
+      ss << static_cast<unsigned int>(unsignedByte);
+      return ss.str();
+    }
+    else
+    {
+      s8 aByte = 0;
+      std::memcpy(&aByte, memory, sizeof(s8));
+      // This has to be converted to an integer type because printing a uint8_t would resolve to a
+      // char and print a single character.  Additionaly, casting a signed type to a larger signed
+      // type will extend the sign to match the size of the destination type, this is required for
+      // signed values in decimal, but must be bypassed for other bases, this is solved by first
+      // casting to u8 then to signed int.
+      if (base == Common::MemBase::base_decimal)
+        ss << static_cast<int>(aByte);
+      else
+        ss << static_cast<int>(static_cast<u8>(aByte));
+      return ss.str();
+    }
+  }
+  case Common::MemType::type_halfword:
+  {
+    char* memoryCopy = new char[sizeof(u16)];
+    std::memcpy(memoryCopy, memory, sizeof(u16));
+    if (withBSwap)
+    {
+      u16 halfword = 0;
+      std::memcpy(&halfword, memoryCopy, sizeof(u16));
+      halfword = Common::bSwap16(halfword);
+      std::memcpy(memoryCopy, &halfword, sizeof(u16));
+    }
+
+    if (isUnsigned || base == Common::MemBase::base_binary)
+    {
+      u16 unsignedHalfword = 0;
+      std::memcpy(&unsignedHalfword, memoryCopy, sizeof(u16));
+      if (base == Common::MemBase::base_binary)
+      {
+        delete[] memoryCopy;
+        return std::bitset<sizeof(u16) * 8>(unsignedHalfword).to_string();
+      }
+      ss << unsignedHalfword;
+      delete[] memoryCopy;
+      return ss.str();
+    }
+    s16 aHalfword = 0;
+    std::memcpy(&aHalfword, memoryCopy, sizeof(s16));
+    ss << aHalfword;
+    delete[] memoryCopy;
+    return ss.str();
+  }
+  case Common::MemType::type_word:
+  {
+    char* memoryCopy = new char[sizeof(u32)];
+    std::memcpy(memoryCopy, memory, sizeof(u32));
+    if (withBSwap)
+    {
+      u32 word = 0;
+      std::memcpy(&word, memoryCopy, sizeof(u32));
+      word = Common::bSwap32(word);
+      std::memcpy(memoryCopy, &word, sizeof(u32));
+    }
+
+    if (isUnsigned || base == Common::MemBase::base_binary)
+    {
+      u32 unsignedWord = 0;
+      std::memcpy(&unsignedWord, memoryCopy, sizeof(u32));
+      if (base == Common::MemBase::base_binary)
+      {
+        delete[] memoryCopy;
+        return std::bitset<sizeof(u32) * 8>(unsignedWord).to_string();
+      }
+      ss << unsignedWord;
+      delete[] memoryCopy;
+      return ss.str();
+    }
+    s32 aWord = 0;
+    std::memcpy(&aWord, memoryCopy, sizeof(s32));
+    ss << aWord;
+    delete[] memoryCopy;
+    return ss.str();
+  }
+  case Common::MemType::type_float:
+  {
+    char* memoryCopy = new char[sizeof(u32)];
+    std::memcpy(memoryCopy, memory, sizeof(u32));
+    if (withBSwap)
+    {
+      u32 word = 0;
+      std::memcpy(&word, memoryCopy, sizeof(u32));
+      word = Common::bSwap32(word);
+      std::memcpy(memoryCopy, &word, sizeof(u32));
+    }
+
+    float aFloat = 0.0f;
+    std::memcpy(&aFloat, memoryCopy, sizeof(float));
+    // With 9 digits of precision, it is possible to convert a float back and forth to its binary
+    // representation without any loss
+    ss << std::setprecision(9) << aFloat;
+    delete[] memoryCopy;
+    return ss.str();
+  }
+  case Common::MemType::type_double:
+  {
+    char* memoryCopy = new char[sizeof(u64)];
+    std::memcpy(memoryCopy, memory, sizeof(u64));
+    if (withBSwap)
+    {
+      u64 doubleword = 0;
+      std::memcpy(&doubleword, memoryCopy, sizeof(u64));
+      doubleword = Common::bSwap64(doubleword);
+      std::memcpy(memoryCopy, &doubleword, sizeof(u64));
+    }
+
+    double aDouble = 0.0;
+    std::memcpy(&aDouble, memoryCopy, sizeof(double));
+    // With 17 digits of precision, it is possible to convert a double back and forth to its binary
+    // representation without any loss
+    ss << std::setprecision(17) << aDouble;
+    delete[] memoryCopy;
+    return ss.str();
+  }
+  case Common::MemType::type_string:
+  {
+    int actualLength = 0;
+    for (actualLength; actualLength < length; ++actualLength)
+    {
+      if (*(memory + actualLength) == 0x00)
+        break;
+    }
+    return std::string(memory, actualLength);
+  }
+  case Common::MemType::type_byteArray:
+  {
+    // Force Hexadecimal, no matter the base
+    ss << std::hex << std::uppercase;
+    for (int i = 0; i < length; ++i)
+    {
+      u8 aByte = 0;
+      std::memcpy(&aByte, memory + i, sizeof(u8));
+      ss << std::setfill('0') << std::setw(2) << static_cast<int>(aByte) << " ";
+    }
+    std::string str = ss.str();
+    // Remove the space at the end
+    str.pop_back();
+    return str;
+  }
+  default:
+    return "";
+    break;
+  }
+}
+} // namespace Common
```

### Comparing `dolphin-memory-engine-1.1.2/Source/DolphinProcess/Dummy/DummyDolphinProcess.cpp` & `dolphin-memory-engine-1.1.3/Source/DolphinProcess/Windows/WindowsDolphinProcess.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-#include "DummyDolphinProcess.h"
-#include "../../Common/CommonUtils.h"
-
-namespace DolphinComm
-{
-bool DummyDolphinProcess::obtainEmuRAMInformations()
-{
-  return false;
-}
-
-bool DummyDolphinProcess::findPID()
-{
-  return false;
-}
-
-bool DummyDolphinProcess::readFromRAM(const u32 offset, char* buffer, const size_t size,
-                                      const bool withBSwap)
-{
-  return false;
-}
-
-bool DummyDolphinProcess::writeToRAM(const u32 offset, const char* buffer, const size_t size,
-                                     const bool withBSwap)
-{
-  return false;
-}
-} // namespace DolphinComm
+#ifdef _WIN32
+
+#pragma once
+
+#include <windows.h>
+
+#include "../IDolphinProcess.h"
+
+namespace DolphinComm
+{
+class WindowsDolphinProcess : public IDolphinProcess
+{
+public:
+  WindowsDolphinProcess()
+  {
+  }
+  bool findPID() override;
+  bool obtainEmuRAMInformations() override;
+  bool readFromRAM(const u32 offset, char* buffer, const size_t size,
+                   const bool withBSwap) override;
+  bool writeToRAM(const u32 offset, const char* buffer, const size_t size,
+                  const bool withBSwap) override;
+
+private:
+  HANDLE m_hDolphin;
+};
+} // namespace DolphinComm
+#endif
```

### Comparing `dolphin-memory-engine-1.1.2/Source/DolphinProcess/Linux/LinuxDolphinProcess.h` & `dolphin-memory-engine-1.1.3/Source/DolphinProcess/Linux/LinuxDolphinProcess.h`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-#ifdef __linux__
-
-#pragma once
-
-#include <fstream>
-#include <sstream>
-#include <string>
-
-#include "../IDolphinProcess.h"
-
-namespace DolphinComm
-{
-class LinuxDolphinProcess : public IDolphinProcess
-{
-public:
-  LinuxDolphinProcess()
-  {
-  }
-  bool findPID() override;
-  bool obtainEmuRAMInformations() override;
-  bool readFromRAM(const u32 offset, char* buffer, size_t size, const bool withBSwap) override;
-  bool writeToRAM(const u32 offset, const char* buffer, const size_t size,
-                  const bool withBSwap) override;
-};
-} // namespace DolphinComm
-#endif
+#ifdef __linux__
+
+#pragma once
+
+#include <fstream>
+#include <sstream>
+#include <string>
+
+#include "../IDolphinProcess.h"
+
+namespace DolphinComm
+{
+class LinuxDolphinProcess : public IDolphinProcess
+{
+public:
+  LinuxDolphinProcess()
+  {
+  }
+  bool findPID() override;
+  bool obtainEmuRAMInformations() override;
+  bool readFromRAM(const u32 offset, char* buffer, size_t size, const bool withBSwap) override;
+  bool writeToRAM(const u32 offset, const char* buffer, const size_t size,
+                  const bool withBSwap) override;
+};
+} // namespace DolphinComm
+#endif
```

### Comparing `dolphin-memory-engine-1.1.2/Source/DolphinProcess/Windows/WindowsDolphinProcess.cpp` & `dolphin-memory-engine-1.1.3/Source/DolphinProcess/Windows/WindowsDolphinProcess.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,192 +1,242 @@
-#ifdef _WIN32
-
-#include "WindowsDolphinProcess.h"
-#include "../../Common/CommonUtils.h"
-
-#include <Psapi.h>
-#include <string>
-#include <tlhelp32.h>
-
-namespace DolphinComm
-{
-
-bool WindowsDolphinProcess::findPID()
-{
-  PROCESSENTRY32 entry;
-  entry.dwSize = sizeof(PROCESSENTRY32);
-
-  HANDLE snapshot = CreateToolhelp32Snapshot(TH32CS_SNAPPROCESS, NULL);
-
-  if (Process32First(snapshot, &entry) == TRUE)
-  {
-    do
-    {
-      if (std::string(entry.szExeFile) == "Dolphin.exe" ||
-          std::string(entry.szExeFile) == "DolphinQt2.exe" ||
-          std::string(entry.szExeFile) == "DolphinWx.exe")
-      {
-        m_PID = entry.th32ProcessID;
-        break;
-      }
-    } while (Process32Next(snapshot, &entry) == TRUE);
-  }
-
-  CloseHandle(snapshot);
-  if (m_PID == -1)
-    // Here, Dolphin doesn't appear to be running on the system
-    return false;
-
-  // Get the handle if Dolphin is running since it's required on Windows to read or write into the
-  // RAM of the process and to query the RAM mapping information
-  m_hDolphin = OpenProcess(PROCESS_QUERY_INFORMATION | PROCESS_VM_OPERATION | PROCESS_VM_READ |
-                               PROCESS_VM_WRITE,
-                           FALSE, m_PID);
-  return true;
-}
-
-bool WindowsDolphinProcess::obtainEmuRAMInformations()
-{
-  MEMORY_BASIC_INFORMATION info;
-  bool MEM1Found = false;
-  for (unsigned char* p = nullptr;
-       VirtualQueryEx(m_hDolphin, p, &info, sizeof(info)) == sizeof(info); p += info.RegionSize)
-  {
-    // Check region size so that we know it's MEM2
-    if (info.RegionSize == 0x4000000)
-    {
-      u64 regionBaseAddress = 0;
-      std::memcpy(&regionBaseAddress, &(info.BaseAddress), sizeof(info.BaseAddress));
-      if (MEM1Found && regionBaseAddress > m_emuRAMAddressStart + 0x10000000)
-      {
-        // In some cases MEM2 could actually be before MEM1. Once we find MEM1, ignore regions of
-        // this size that are too far away. There apparently are other non-MEM2 regions of size
-        // 0x4000000.
-        break;
-      }
-      // View the comment for MEM1.
-      PSAPI_WORKING_SET_EX_INFORMATION wsInfo;
-      wsInfo.VirtualAddress = info.BaseAddress;
-      if (QueryWorkingSetEx(m_hDolphin, &wsInfo, sizeof(PSAPI_WORKING_SET_EX_INFORMATION)))
-      {
-        if (wsInfo.VirtualAttributes.Valid)
-        {
-          std::memcpy(&m_MEM2AddressStart, &(regionBaseAddress), sizeof(regionBaseAddress));
-          m_MEM2Present = true;
-        }
-      }
-    }
-    else if (!MEM1Found && info.RegionSize == 0x2000000 && info.Type == MEM_MAPPED)
-    {
-      // Here, it's likely the right page, but it can happen that multiple pages with these criteria
-      // exists and have nothing to do with the emulated memory. Only the right page has valid
-      // working set information so an additional check is required that it is backed by physical
-      // memory.
-      PSAPI_WORKING_SET_EX_INFORMATION wsInfo;
-      wsInfo.VirtualAddress = info.BaseAddress;
-      if (QueryWorkingSetEx(m_hDolphin, &wsInfo, sizeof(PSAPI_WORKING_SET_EX_INFORMATION)))
-      {
-        if (wsInfo.VirtualAttributes.Valid)
-        {
-          std::memcpy(&m_emuRAMAddressStart, &(info.BaseAddress), sizeof(info.BaseAddress));
-          MEM1Found = true;
-        }
-      }
-    }
-    if (MEM1Found && m_MEM2Present)
-      break;
-  }
-  if (m_emuRAMAddressStart == 0)
-  {
-    // Here, Dolphin is running, but the emulation hasn't started
-    return false;
-  }
-  return true;
-}
-
-bool WindowsDolphinProcess::readFromRAM(const u32 offset, char* buffer, const size_t size,
-                                        const bool withBSwap)
-{
-  u64 RAMAddress = m_emuRAMAddressStart + offset;
-  SIZE_T nread = 0;
-  bool bResult = ReadProcessMemory(m_hDolphin, (void*)RAMAddress, buffer, size, &nread);
-  if (bResult && nread == size)
-  {
-    if (withBSwap)
-    {
-      switch (size)
-      {
-      case 2:
-      {
-        u16 halfword = 0;
-        std::memcpy(&halfword, buffer, sizeof(u16));
-        halfword = Common::bSwap16(halfword);
-        std::memcpy(buffer, &halfword, sizeof(u16));
-        break;
-      }
-      case 4:
-      {
-        u32 word = 0;
-        std::memcpy(&word, buffer, sizeof(u32));
-        word = Common::bSwap32(word);
-        std::memcpy(buffer, &word, sizeof(u32));
-        break;
-      }
-      case 8:
-      {
-        u64 doubleword = 0;
-        std::memcpy(&doubleword, buffer, sizeof(u64));
-        doubleword = Common::bSwap64(doubleword);
-        std::memcpy(buffer, &doubleword, sizeof(u64));
-        break;
-      }
-      }
-    }
-    return true;
-  }
-  return false;
-}
-
-bool WindowsDolphinProcess::writeToRAM(const u32 offset, const char* buffer, const size_t size,
-                                       const bool withBSwap)
-{
-  u64 RAMAddress = m_emuRAMAddressStart + offset;
-  SIZE_T nread = 0;
-  char* bufferCopy = new char[size];
-  std::memcpy(bufferCopy, buffer, size);
-  if (withBSwap)
-  {
-    switch (size)
-    {
-    case 2:
-    {
-      u16 halfword = 0;
-      std::memcpy(&halfword, bufferCopy, sizeof(u16));
-      halfword = Common::bSwap16(halfword);
-      std::memcpy(bufferCopy, &halfword, sizeof(u16));
-      break;
-    }
-    case 4:
-    {
-      u32 word = 0;
-      std::memcpy(&word, bufferCopy, sizeof(u32));
-      word = Common::bSwap32(word);
-      std::memcpy(bufferCopy, &word, sizeof(u32));
-      break;
-    }
-    case 8:
-    {
-      u64 doubleword = 0;
-      std::memcpy(&doubleword, bufferCopy, sizeof(u64));
-      doubleword = Common::bSwap64(doubleword);
-      std::memcpy(bufferCopy, &doubleword, sizeof(u64));
-      break;
-    }
-    }
-  }
-
-  bool bResult = WriteProcessMemory(m_hDolphin, (void*)RAMAddress, bufferCopy, size, &nread);
-  delete[] bufferCopy;
-  return (bResult && nread == size);
-}
-} // namespace DolphinComm
-#endif
+#ifdef _WIN32
+
+#include "WindowsDolphinProcess.h"
+#include "../../Common/CommonUtils.h"
+
+#include <Psapi.h>
+#include <string>
+#include <tlhelp32.h>
+
+namespace DolphinComm
+{
+
+bool WindowsDolphinProcess::findPID()
+{
+  PROCESSENTRY32 entry;
+  entry.dwSize = sizeof(PROCESSENTRY32);
+
+  HANDLE snapshot = CreateToolhelp32Snapshot(TH32CS_SNAPPROCESS, NULL);
+
+  if (Process32First(snapshot, &entry) == TRUE)
+  {
+    do
+    {
+      if (std::string(entry.szExeFile) == "Dolphin.exe" ||
+          std::string(entry.szExeFile) == "DolphinQt2.exe" ||
+          std::string(entry.szExeFile) == "DolphinWx.exe")
+      {
+        m_PID = entry.th32ProcessID;
+        break;
+      }
+    } while (Process32Next(snapshot, &entry) == TRUE);
+  }
+
+  CloseHandle(snapshot);
+  if (m_PID == -1)
+    // Here, Dolphin doesn't appear to be running on the system
+    return false;
+
+  // Get the handle if Dolphin is running since it's required on Windows to read or write into the
+  // RAM of the process and to query the RAM mapping information
+  m_hDolphin = OpenProcess(PROCESS_QUERY_INFORMATION | PROCESS_VM_OPERATION | PROCESS_VM_READ |
+                               PROCESS_VM_WRITE,
+                           FALSE, m_PID);
+  return true;
+}
+
+bool WindowsDolphinProcess::obtainEmuRAMInformations()
+{
+  MEMORY_BASIC_INFORMATION info;
+  bool MEM1Found = false;
+  for (unsigned char* p = nullptr;
+       VirtualQueryEx(m_hDolphin, p, &info, sizeof(info)) == sizeof(info); p += info.RegionSize)
+  {
+    // Check region size so that we know it's MEM2
+    if (!m_MEM2Present && info.RegionSize == 0x4000000)
+    {
+      u64 regionBaseAddress = 0;
+      std::memcpy(&regionBaseAddress, &(info.BaseAddress), sizeof(info.BaseAddress));
+      if (MEM1Found && regionBaseAddress > m_emuRAMAddressStart + 0x10000000)
+      {
+        // In some cases MEM2 could actually be before MEM1. Once we find MEM1, ignore regions of
+        // this size that are too far away. There apparently are other non-MEM2 regions of size
+        // 0x4000000.
+        break;
+      }
+      // View the comment for MEM1.
+      PSAPI_WORKING_SET_EX_INFORMATION wsInfo;
+      wsInfo.VirtualAddress = info.BaseAddress;
+      if (QueryWorkingSetEx(m_hDolphin, &wsInfo, sizeof(PSAPI_WORKING_SET_EX_INFORMATION)))
+      {
+        if (wsInfo.VirtualAttributes.Valid)
+        {
+          std::memcpy(&m_MEM2AddressStart, &(regionBaseAddress), sizeof(regionBaseAddress));
+          m_MEM2Present = true;
+        }
+      }
+    }
+    else if (info.RegionSize == 0x2000000 && info.Type == MEM_MAPPED)
+    {
+      // Here, it's likely the right page, but it can happen that multiple pages with these criteria
+      // exists and have nothing to do with the emulated memory. Only the right page has valid
+      // working set information so an additional check is required that it is backed by physical
+      // memory.
+      PSAPI_WORKING_SET_EX_INFORMATION wsInfo;
+      wsInfo.VirtualAddress = info.BaseAddress;
+      if (QueryWorkingSetEx(m_hDolphin, &wsInfo, sizeof(PSAPI_WORKING_SET_EX_INFORMATION)))
+      {
+        if (wsInfo.VirtualAttributes.Valid)
+        {
+          if (!MEM1Found)
+          {
+            std::memcpy(&m_emuRAMAddressStart, &(info.BaseAddress), sizeof(info.BaseAddress));
+            MEM1Found = true;
+          }
+          else
+          {
+            u64 aramCandidate = 0;
+            std::memcpy(&aramCandidate, &(info.BaseAddress), sizeof(info.BaseAddress));
+            if (aramCandidate == m_emuRAMAddressStart + 0x2000000)
+            {
+              m_emuARAMAdressStart = aramCandidate;
+              m_ARAMAccessible = true;
+            }
+          }
+        }
+      }
+    }
+  }
+
+  if (m_MEM2Present)
+  {
+    m_emuARAMAdressStart = 0;
+    m_ARAMAccessible = false;
+  }
+
+  if (m_emuRAMAddressStart == 0)
+  {
+    // Here, Dolphin is running, but the emulation hasn't started
+    return false;
+  }
+  return true;
+}
+
+bool WindowsDolphinProcess::readFromRAM(const u32 offset, char* buffer, const size_t size,
+                                        const bool withBSwap)
+{
+  u64 RAMAddress = 0;
+  if (m_ARAMAccessible)
+  {
+    if (offset >= Common::ARAM_FAKESIZE)
+      RAMAddress = m_emuRAMAddressStart + offset - Common::ARAM_FAKESIZE;
+    else
+      RAMAddress = m_emuARAMAdressStart + offset;
+  }
+  else if (offset >= (Common::MEM2_START - Common::MEM1_START))
+  {
+    RAMAddress = m_MEM2AddressStart + offset - (Common::MEM2_START - Common::MEM1_START);
+  }
+  else
+  {
+    RAMAddress = m_emuRAMAddressStart + offset;
+  }
+
+  SIZE_T nread = 0;
+  bool bResult = ReadProcessMemory(m_hDolphin, (void*)RAMAddress, buffer, size, &nread);
+  if (bResult && nread == size)
+  {
+    if (withBSwap)
+    {
+      switch (size)
+      {
+      case 2:
+      {
+        u16 halfword = 0;
+        std::memcpy(&halfword, buffer, sizeof(u16));
+        halfword = Common::bSwap16(halfword);
+        std::memcpy(buffer, &halfword, sizeof(u16));
+        break;
+      }
+      case 4:
+      {
+        u32 word = 0;
+        std::memcpy(&word, buffer, sizeof(u32));
+        word = Common::bSwap32(word);
+        std::memcpy(buffer, &word, sizeof(u32));
+        break;
+      }
+      case 8:
+      {
+        u64 doubleword = 0;
+        std::memcpy(&doubleword, buffer, sizeof(u64));
+        doubleword = Common::bSwap64(doubleword);
+        std::memcpy(buffer, &doubleword, sizeof(u64));
+        break;
+      }
+      }
+    }
+    return true;
+  }
+  return false;
+}
+
+bool WindowsDolphinProcess::writeToRAM(const u32 offset, const char* buffer, const size_t size,
+                                       const bool withBSwap)
+{
+  u64 RAMAddress = 0;
+  if (m_ARAMAccessible)
+  {
+    if (offset >= Common::ARAM_FAKESIZE)
+      RAMAddress = m_emuRAMAddressStart + offset - Common::ARAM_FAKESIZE;
+    else
+      RAMAddress = m_emuARAMAdressStart + offset;
+  }
+  else if (offset >= (Common::MEM2_START - Common::MEM1_START))
+  {
+    RAMAddress = m_MEM2AddressStart + offset - (Common::MEM2_START - Common::MEM1_START);
+  }
+  else
+  {
+    RAMAddress = m_emuRAMAddressStart + offset;
+  }
+
+  SIZE_T nread = 0;
+  char* bufferCopy = new char[size];
+  std::memcpy(bufferCopy, buffer, size);
+  if (withBSwap)
+  {
+    switch (size)
+    {
+    case 2:
+    {
+      u16 halfword = 0;
+      std::memcpy(&halfword, bufferCopy, sizeof(u16));
+      halfword = Common::bSwap16(halfword);
+      std::memcpy(bufferCopy, &halfword, sizeof(u16));
+      break;
+    }
+    case 4:
+    {
+      u32 word = 0;
+      std::memcpy(&word, bufferCopy, sizeof(u32));
+      word = Common::bSwap32(word);
+      std::memcpy(bufferCopy, &word, sizeof(u32));
+      break;
+    }
+    case 8:
+    {
+      u64 doubleword = 0;
+      std::memcpy(&doubleword, bufferCopy, sizeof(u64));
+      doubleword = Common::bSwap64(doubleword);
+      std::memcpy(bufferCopy, &doubleword, sizeof(u64));
+      break;
+    }
+    }
+  }
+
+  bool bResult = WriteProcessMemory(m_hDolphin, (void*)RAMAddress, bufferCopy, size, &nread);
+  delete[] bufferCopy;
+  return (bResult && nread == size);
+}
+} // namespace DolphinComm
+#endif
```

### Comparing `dolphin-memory-engine-1.1.2/Source/MemoryScanner/MemoryScanner.cpp` & `dolphin-memory-engine-1.1.3/Source/MemoryScanner/MemoryScanner.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,546 +1,483 @@
-#include "MemoryScanner.h"
-
-#include "../Common/CommonUtils.h"
-#include "../DolphinProcess/DolphinAccessor.h"
-
-MemScanner::MemScanner() : m_resultsConsoleAddr(std::vector<u32>())
-{
-}
-
-MemScanner::~MemScanner()
-{
-  delete[] m_scanRAMCache;
-}
-
-Common::MemOperationReturnCode MemScanner::firstScan(const MemScanner::ScanFiter filter,
-                                                     const std::string& searchTerm1,
-                                                     const std::string& searchTerm2)
-{
-  m_scanRAMCache = nullptr;
-  u32 ramSize = 0;
-  u32 MEM2Distance = DolphinComm::DolphinAccessor::getMEM1ToMEM2Distance();
-  if (DolphinComm::DolphinAccessor::isMEM2Present())
-  {
-    ramSize = Common::MEM1_SIZE + Common::MEM2_SIZE;
-    m_scanRAMCache = new char[ramSize];
-    if (!DolphinComm::DolphinAccessor::readFromRAM(
-            Common::dolphinAddrToOffset(Common::MEM2_START, MEM2Distance),
-            m_scanRAMCache + Common::MEM1_SIZE, Common::MEM2_SIZE, false))
-    {
-      delete[] m_scanRAMCache;
-      m_scanRAMCache = nullptr;
-      return Common::MemOperationReturnCode::operationFailed;
-    }
-  }
-  else
-  {
-    ramSize = Common::MEM1_SIZE;
-    m_scanRAMCache = new char[ramSize];
-  }
-
-  if (!DolphinComm::DolphinAccessor::readFromRAM(
-          Common::dolphinAddrToOffset(Common::MEM1_START, MEM2Distance), m_scanRAMCache,
-          Common::MEM1_SIZE, false))
-  {
-    delete[] m_scanRAMCache;
-    m_scanRAMCache = nullptr;
-    return Common::MemOperationReturnCode::operationFailed;
-  }
-
-  if (filter == ScanFiter::unknownInitial)
-  {
-    int alignementDivision =
-        m_enforceMemAlignement ? Common::getNbrBytesAlignementForType(m_memType) : 1;
-    m_resultCount = ((ramSize / alignementDivision) -
-                     Common::getSizeForType(m_memType, static_cast<size_t>(1)));
-    m_wasUnknownInitialValue = true;
-    m_memSize = 1;
-    m_scanStarted = true;
-    return Common::MemOperationReturnCode::OK;
-  }
-
-  bool m_wasUnknownInitialValue = false;
-  Common::MemOperationReturnCode scanReturn = Common::MemOperationReturnCode::OK;
-  size_t termActualLength = 0;
-  size_t termMaxLength = 0;
-  if (m_memType == Common::MemType::type_string)
-    // This is just to have the string formatted with the appropriate length, byte arrays don't need
-    // this because they get copied byte per byte
-    termMaxLength = searchTerm1.length();
-  else
-    // Have no restriction on the length for the rest
-    termMaxLength = ramSize;
-
-  std::string formattedSearchTerm1;
-  if (m_memType == Common::MemType::type_byteArray)
-    formattedSearchTerm1 = addSpacesToBytesArrays(searchTerm1);
-  else
-    formattedSearchTerm1 = searchTerm1;
-
-  char* memoryToCompare1 = Common::formatStringToMemory(
-      scanReturn, termActualLength, formattedSearchTerm1, m_memBase, m_memType, termMaxLength);
-  if (scanReturn != Common::MemOperationReturnCode::OK)
-  {
-    delete[] memoryToCompare1;
-    delete[] m_scanRAMCache;
-    m_scanRAMCache = nullptr;
-    return scanReturn;
-  }
-
-  char* memoryToCompare2 = nullptr;
-  if (filter == ScanFiter::between)
-  {
-    memoryToCompare2 = Common::formatStringToMemory(scanReturn, termActualLength, searchTerm2,
-                                                    m_memBase, m_memType, ramSize);
-    if (scanReturn != Common::MemOperationReturnCode::OK)
-    {
-      delete[] memoryToCompare1;
-      delete[] memoryToCompare2;
-      delete[] m_scanRAMCache;
-      m_scanRAMCache = nullptr;
-      return scanReturn;
-    }
-  }
-
-  bool withBSwap = Common::shouldBeBSwappedForType(m_memType);
-
-  m_memSize = Common::getSizeForType(m_memType, termActualLength);
-
-  char* noOffset = new char[m_memSize];
-  std::memset(noOffset, 0, m_memSize);
-
-  int increment = m_enforceMemAlignement ? Common::getNbrBytesAlignementForType(m_memType) : 1;
-  for (u32 i = 0; i < (ramSize - m_memSize); i += increment)
-  {
-    char* memoryCandidate = &m_scanRAMCache[i];
-    bool isResult = false;
-    switch (filter)
-    {
-    case ScanFiter::exact:
-    {
-      if (m_memType == Common::MemType::type_string || m_memType == Common::MemType::type_byteArray)
-        isResult = (std::memcmp(memoryCandidate, memoryToCompare1, m_memSize) == 0);
-      else
-        isResult = (compareMemoryAsNumbers(memoryCandidate, memoryToCompare1, noOffset, false,
-                                           false, m_memSize) == MemScanner::CompareResult::equal);
-      break;
-    }
-    case ScanFiter::between:
-    {
-      MemScanner::CompareResult result1 = compareMemoryAsNumbers(memoryCandidate, memoryToCompare1,
-                                                                 noOffset, false, false, m_memSize);
-      MemScanner::CompareResult result2 = compareMemoryAsNumbers(memoryCandidate, memoryToCompare2,
-                                                                 noOffset, false, false, m_memSize);
-      isResult = ((result1 == MemScanner::CompareResult::bigger ||
-                   result1 == MemScanner::CompareResult::equal) &&
-                  (result2 == MemScanner::CompareResult::smaller ||
-                   result2 == MemScanner::CompareResult::equal));
-      break;
-    }
-    case ScanFiter::biggerThan:
-    {
-      isResult = (compareMemoryAsNumbers(memoryCandidate, memoryToCompare1, noOffset, false, false,
-                                         m_memSize) == MemScanner::CompareResult::bigger);
-      break;
-    }
-    case ScanFiter::smallerThan:
-    {
-      isResult = (compareMemoryAsNumbers(memoryCandidate, memoryToCompare1, noOffset, false, false,
-                                         m_memSize) == MemScanner::CompareResult::smaller);
-      break;
-    }
-    }
-
-    if (isResult)
-    {
-      u32 consoleOffset = 0;
-      if (i >= Common::MEM1_SIZE)
-        consoleOffset = i + (MEM2Distance - Common::MEM1_SIZE);
-      else
-        consoleOffset = i;
-      m_resultsConsoleAddr.push_back(Common::offsetToDolphinAddr(consoleOffset, MEM2Distance));
-    }
-  }
-  delete[] noOffset;
-  delete[] memoryToCompare1;
-  delete[] memoryToCompare2;
-  m_resultCount = m_resultsConsoleAddr.size();
-  m_scanStarted = true;
-  return Common::MemOperationReturnCode::OK;
-}
-
-Common::MemOperationReturnCode MemScanner::nextScan(const MemScanner::ScanFiter filter,
-                                                    const std::string& searchTerm1,
-                                                    const std::string& searchTerm2)
-{
-  u32 ramSize = 0;
-  u32 MEM2Distance = DolphinComm::DolphinAccessor::getMEM1ToMEM2Distance();
-  char* newerRAMCache = nullptr;
-  if (DolphinComm::DolphinAccessor::isMEM2Present())
-  {
-    ramSize = Common::MEM1_SIZE + Common::MEM2_SIZE;
-    newerRAMCache = new char[ramSize];
-    if (!DolphinComm::DolphinAccessor::readFromRAM(
-            Common::dolphinAddrToOffset(Common::MEM2_START, MEM2Distance),
-            newerRAMCache + Common::MEM1_SIZE, Common::MEM2_SIZE, false))
-    {
-      delete[] m_scanRAMCache;
-      m_scanRAMCache = nullptr;
-      delete[] newerRAMCache;
-      return Common::MemOperationReturnCode::operationFailed;
-    }
-  }
-  else
-  {
-    ramSize = Common::MEM1_SIZE;
-    newerRAMCache = new char[ramSize];
-  }
-
-  u32 offset = Common::dolphinAddrToOffset(Common::MEM1_START, MEM2Distance);
-  if (!DolphinComm::DolphinAccessor::readFromRAM(offset, newerRAMCache, Common::MEM1_SIZE, false))
-  {
-    delete[] m_scanRAMCache;
-    m_scanRAMCache = nullptr;
-    delete[] newerRAMCache;
-    return Common::MemOperationReturnCode::operationFailed;
-  }
-
-  Common::MemOperationReturnCode scanReturn = Common::MemOperationReturnCode::OK;
-  size_t termActualLength = 0;
-  size_t termMaxLength = 0;
-  if (m_memType == Common::MemType::type_string)
-    // This is just to have the string formatted with the appropriate length, byte arrays don't need
-    // this because they get copied byte per byte
-    termMaxLength = searchTerm1.length();
-  else
-    // Have no restriction on the length for the rest
-    termMaxLength = ramSize;
-
-  char* memoryToCompare1 = nullptr;
-  if (filter != ScanFiter::increased && filter != ScanFiter::decreased &&
-      filter != ScanFiter::changed && filter != ScanFiter::unchanged)
-  {
-    std::string formattedSearchTerm1;
-    if (m_memType == Common::MemType::type_byteArray)
-      formattedSearchTerm1 = addSpacesToBytesArrays(searchTerm1);
-    else
-      formattedSearchTerm1 = searchTerm1;
-
-    memoryToCompare1 = Common::formatStringToMemory(
-        scanReturn, termActualLength, formattedSearchTerm1, m_memBase, m_memType, termMaxLength);
-    if (scanReturn != Common::MemOperationReturnCode::OK)
-      return scanReturn;
-  }
-
-  char* memoryToCompare2 = nullptr;
-  if (filter == ScanFiter::between)
-  {
-    memoryToCompare2 = Common::formatStringToMemory(scanReturn, termActualLength, searchTerm2,
-                                                    m_memBase, m_memType, ramSize);
-    if (scanReturn != Common::MemOperationReturnCode::OK)
-      return scanReturn;
-  }
-
-  bool withBSwap = Common::shouldBeBSwappedForType(m_memType);
-
-  m_memSize = Common::getSizeForType(m_memType, termActualLength);
-
-  char* noOffset = new char[m_memSize];
-  std::memset(noOffset, 0, m_memSize);
-
-  std::vector<u32> newerResults = std::vector<u32>();
-
-  if (m_wasUnknownInitialValue)
-  {
-    m_wasUnknownInitialValue = false;
-
-    int increment = m_enforceMemAlignement ? Common::getNbrBytesAlignementForType(m_memType) : 1;
-    for (u32 i = 0; i < (ramSize - m_memSize); i += increment)
-    {
-      u32 consoleOffset = 0;
-      if (i >= Common::MEM1_SIZE)
-        consoleOffset = i + (MEM2Distance - Common::MEM1_SIZE);
-      else
-        consoleOffset = i;
-      if (isHitNextScan(filter, memoryToCompare1, memoryToCompare2, noOffset, newerRAMCache,
-                        m_memSize, i))
-      {
-        newerResults.push_back(Common::offsetToDolphinAddr(consoleOffset, MEM2Distance));
-      }
-    }
-  }
-  else
-  {
-    for (auto i : m_resultsConsoleAddr)
-    {
-      u32 ramIndex = 0;
-      if (Common::dolphinAddrToOffset(i, MEM2Distance) >= Common::MEM1_SIZE)
-        ramIndex =
-            Common::dolphinAddrToOffset(i, MEM2Distance) - (MEM2Distance - Common::MEM1_SIZE);
-      else
-        ramIndex = Common::dolphinAddrToOffset(i, MEM2Distance);
-      if (isHitNextScan(filter, memoryToCompare1, memoryToCompare2, noOffset, newerRAMCache,
-                        m_memSize, ramIndex))
-      {
-        newerResults.push_back(i);
-      }
-    }
-  }
-
-  delete[] noOffset;
-  m_resultsConsoleAddr.clear();
-  std::swap(m_resultsConsoleAddr, newerResults);
-  delete[] m_scanRAMCache;
-  m_scanRAMCache = nullptr;
-  m_scanRAMCache = newerRAMCache;
-  m_resultCount = m_resultsConsoleAddr.size();
-  return Common::MemOperationReturnCode::OK;
-}
-
-void MemScanner::reset()
-{
-  m_resultsConsoleAddr.clear();
-  m_wasUnknownInitialValue = false;
-  delete[] m_scanRAMCache;
-  m_scanRAMCache = nullptr;
-  m_resultCount = 0;
-  m_scanStarted = false;
-}
-
-inline bool MemScanner::isHitNextScan(const MemScanner::ScanFiter filter,
-                                      const char* memoryToCompare1, const char* memoryToCompare2,
-                                      const char* noOffset, const char* newerRAMCache,
-                                      const size_t realSize, const u32 consoleOffset) const
-{
-  char* olderMemory = &m_scanRAMCache[consoleOffset];
-  const char* newerMemory = &newerRAMCache[consoleOffset];
-
-  switch (filter)
-  {
-  case ScanFiter::exact:
-  {
-    if (m_memType == Common::MemType::type_string || m_memType == Common::MemType::type_byteArray)
-      return (std::memcmp(newerMemory, memoryToCompare1, realSize) == 0);
-    else
-      return (compareMemoryAsNumbers(newerMemory, memoryToCompare1, noOffset, false, false,
-                                     realSize) == MemScanner::CompareResult::equal);
-  }
-  case ScanFiter::between:
-  {
-    MemScanner::CompareResult result1 =
-        compareMemoryAsNumbers(newerMemory, memoryToCompare1, noOffset, false, false, realSize);
-    MemScanner::CompareResult result2 =
-        compareMemoryAsNumbers(newerMemory, memoryToCompare2, noOffset, false, false, realSize);
-    return ((result1 == MemScanner::CompareResult::bigger ||
-             result1 == MemScanner::CompareResult::equal) &&
-            (result2 == MemScanner::CompareResult::smaller ||
-             result2 == MemScanner::CompareResult::equal));
-  }
-  case ScanFiter::biggerThan:
-  {
-    return (compareMemoryAsNumbers(newerMemory, memoryToCompare1, noOffset, false, false,
-                                   realSize) == MemScanner::CompareResult::bigger);
-  }
-  case ScanFiter::smallerThan:
-  {
-    return (compareMemoryAsNumbers(newerMemory, memoryToCompare1, noOffset, false, false,
-                                   realSize) == MemScanner::CompareResult::smaller);
-  }
-  case ScanFiter::increasedBy:
-  {
-    return (compareMemoryAsNumbers(newerMemory, olderMemory, memoryToCompare1, false, true,
-                                   realSize) == MemScanner::CompareResult::equal);
-  }
-  case ScanFiter::decreasedBy:
-  {
-    return (compareMemoryAsNumbers(newerMemory, olderMemory, memoryToCompare1, true, true,
-                                   realSize) == MemScanner::CompareResult::equal);
-  }
-  case ScanFiter::increased:
-  {
-    return (compareMemoryAsNumbers(newerMemory, olderMemory, noOffset, false, true, realSize) ==
-            MemScanner::CompareResult::bigger);
-  }
-  case ScanFiter::decreased:
-  {
-    return (compareMemoryAsNumbers(newerMemory, olderMemory, noOffset, false, true, realSize) ==
-            MemScanner::CompareResult::smaller);
-  }
-  case ScanFiter::changed:
-  {
-    MemScanner::CompareResult result =
-        compareMemoryAsNumbers(newerMemory, olderMemory, noOffset, false, true, realSize);
-    return (result == MemScanner::CompareResult::bigger ||
-            result == MemScanner::CompareResult::smaller);
-  }
-  case ScanFiter::unchanged:
-  {
-    return (compareMemoryAsNumbers(newerMemory, olderMemory, noOffset, false, true, realSize) ==
-            MemScanner::CompareResult::equal);
-  }
-  default:
-  {
-    return false;
-  }
-  }
-}
-
-inline MemScanner::CompareResult
-MemScanner::compareMemoryAsNumbers(const char* first, const char* second, const char* offset,
-                                   bool offsetInvert, bool bswapSecond, size_t length) const
-{
-  switch (m_memType)
-  {
-  case Common::MemType::type_byte:
-    if (m_memIsSigned)
-      return compareMemoryAsNumbersWithType<s8>(first, second, offset, offsetInvert, bswapSecond);
-    return compareMemoryAsNumbersWithType<u8>(first, second, offset, offsetInvert, bswapSecond);
-  case Common::MemType::type_halfword:
-    if (m_memIsSigned)
-      return compareMemoryAsNumbersWithType<s16>(first, second, offset, offsetInvert, bswapSecond);
-    return compareMemoryAsNumbersWithType<u16>(first, second, offset, offsetInvert, bswapSecond);
-  case Common::MemType::type_word:
-    if (m_memIsSigned)
-      return compareMemoryAsNumbersWithType<s32>(first, second, offset, offsetInvert, bswapSecond);
-    return compareMemoryAsNumbersWithType<u32>(first, second, offset, offsetInvert, bswapSecond);
-  case Common::MemType::type_float:
-    return compareMemoryAsNumbersWithType<float>(first, second, offset, offsetInvert, bswapSecond);
-  case Common::MemType::type_double:
-    return compareMemoryAsNumbersWithType<double>(first, second, offset, offsetInvert, bswapSecond);
-  default:
-    return MemScanner::CompareResult::nan;
-  }
-}
-
-void MemScanner::setType(const Common::MemType type)
-{
-  m_memType = type;
-}
-
-void MemScanner::setBase(const Common::MemBase base)
-{
-  m_memBase = base;
-}
-
-void MemScanner::setEnforceMemAlignement(const bool enforceAlignement)
-{
-  m_enforceMemAlignement = enforceAlignement;
-}
-
-void MemScanner::setIsSigned(const bool isSigned)
-{
-  m_memIsSigned = isSigned;
-}
-
-int MemScanner::getTermsNumForFilter(const MemScanner::ScanFiter filter) const
-{
-  if (filter == MemScanner::ScanFiter::between)
-    return 2;
-  else if (filter == MemScanner::ScanFiter::exact || filter == MemScanner::ScanFiter::increasedBy ||
-           filter == MemScanner::ScanFiter::decreasedBy ||
-           filter == MemScanner::ScanFiter::biggerThan ||
-           filter == MemScanner::ScanFiter::smallerThan)
-    return 1;
-  return 0;
-}
-
-bool MemScanner::typeSupportsAdditionalOptions(const Common::MemType type) const
-{
-  return (type == Common::MemType::type_byte || type == Common::MemType::type_halfword ||
-          type == Common::MemType::type_word);
-}
-
-std::vector<u32> MemScanner::getResultsConsoleAddr() const
-{
-  return m_resultsConsoleAddr;
-}
-
-std::string MemScanner::getFormattedScannedValueAt(const int index) const
-{
-  u32 MEM2Distance = DolphinComm::DolphinAccessor::getMEM1ToMEM2Distance();
-  u32 offset = Common::dolphinAddrToOffset(m_resultsConsoleAddr.at(index), MEM2Distance);
-  u32 ramIndex = 0;
-  if (offset >= Common::MEM1_SIZE)
-    ramIndex = offset - (MEM2Distance - Common::MEM1_SIZE);
-  else
-    ramIndex = offset;
-  return Common::formatMemoryToString(&m_scanRAMCache[ramIndex], m_memType, m_memSize, m_memBase,
-                                      !m_memIsSigned, Common::shouldBeBSwappedForType(m_memType));
-}
-
-Common::MemOperationReturnCode MemScanner::updateCurrentRAMCache()
-{
-  return DolphinComm::DolphinAccessor::updateRAMCache();
-}
-
-std::string MemScanner::getFormattedCurrentValueAt(const int index) const
-{
-  if (DolphinComm::DolphinAccessor::isValidConsoleAddress(m_resultsConsoleAddr.at(index)))
-  {
-    u32 MEM2Distance = DolphinComm::DolphinAccessor::getMEM1ToMEM2Distance();
-    u32 offset = Common::dolphinAddrToOffset(m_resultsConsoleAddr.at(index), MEM2Distance);
-    u32 ramIndex = 0;
-    if (offset >= Common::MEM1_SIZE)
-      ramIndex = offset - (MEM2Distance - Common::MEM1_SIZE);
-    else
-      ramIndex = offset;
-    return DolphinComm::DolphinAccessor::getFormattedValueFromCache(ramIndex, m_memType, m_memSize,
-                                                                    m_memBase, !m_memIsSigned);
-  }
-  return "";
-}
-
-void MemScanner::removeResultAt(int index)
-{
-  m_resultsConsoleAddr.erase(m_resultsConsoleAddr.begin() + index);
-  m_resultCount--;
-}
-
-std::string MemScanner::addSpacesToBytesArrays(const std::string& bytesArray) const
-{
-  std::string result(bytesArray);
-  int spacesAdded = 0;
-  for (int i = 2; i < bytesArray.length(); i += 2)
-  {
-    if (bytesArray[i] != ' ')
-    {
-      result.insert(i + spacesAdded, 1, ' ');
-      spacesAdded++;
-    }
-    else
-    {
-      i++;
-    }
-  }
-  return result;
-}
-
-size_t MemScanner::getResultCount() const
-{
-  return m_resultCount;
-}
-
-bool MemScanner::hasScanStarted() const
-{
-  return m_scanStarted;
-}
-
-Common::MemType MemScanner::getType() const
-{
-  return m_memType;
-}
-
-Common::MemBase MemScanner::getBase() const
-{
-  return m_memBase;
-}
-
-size_t MemScanner::getLength() const
-{
-  return m_memSize;
-}
-
-bool MemScanner::getIsUnsigned() const
-{
-  return !m_memIsSigned;
-}
+#include "MemoryScanner.h"
+
+#include "../Common/CommonUtils.h"
+#include "../DolphinProcess/DolphinAccessor.h"
+
+MemScanner::MemScanner() : m_resultsConsoleAddr(std::vector<u32>())
+{
+}
+
+MemScanner::~MemScanner()
+{
+  delete[] m_scanRAMCache;
+}
+
+Common::MemOperationReturnCode MemScanner::firstScan(const MemScanner::ScanFiter filter,
+                                                     const std::string& searchTerm1,
+                                                     const std::string& searchTerm2)
+{
+  m_scanRAMCache = nullptr;
+  if (DolphinComm::DolphinAccessor::updateRAMCache() != Common::MemOperationReturnCode::OK)
+  {
+    return Common::MemOperationReturnCode::operationFailed;
+  }
+  u32 ramSize = DolphinComm::DolphinAccessor::getRAMCacheSize();
+  m_scanRAMCache = new char[ramSize];
+  std::memcpy(m_scanRAMCache, DolphinComm::DolphinAccessor::getRAMCache(), ramSize);
+
+  if (filter == ScanFiter::unknownInitial)
+  {
+    int alignementDivision =
+        m_enforceMemAlignement ? Common::getNbrBytesAlignementForType(m_memType) : 1;
+    m_resultCount = ((ramSize / alignementDivision) -
+                     Common::getSizeForType(m_memType, static_cast<size_t>(1)));
+    m_wasUnknownInitialValue = true;
+    m_memSize = 1;
+    m_scanStarted = true;
+    return Common::MemOperationReturnCode::OK;
+  }
+
+  bool m_wasUnknownInitialValue = false;
+  Common::MemOperationReturnCode scanReturn = Common::MemOperationReturnCode::OK;
+  size_t termActualLength = 0;
+  size_t termMaxLength = 0;
+  if (m_memType == Common::MemType::type_string)
+    // This is just to have the string formatted with the appropriate length, byte arrays don't need
+    // this because they get copied byte per byte
+    termMaxLength = searchTerm1.length();
+  else
+    // Have no restriction on the length for the rest
+    termMaxLength = ramSize;
+
+  std::string formattedSearchTerm1;
+  if (m_memType == Common::MemType::type_byteArray)
+    formattedSearchTerm1 = addSpacesToBytesArrays(searchTerm1);
+  else
+    formattedSearchTerm1 = searchTerm1;
+
+  char* memoryToCompare1 = Common::formatStringToMemory(
+      scanReturn, termActualLength, formattedSearchTerm1, m_memBase, m_memType, termMaxLength);
+  if (scanReturn != Common::MemOperationReturnCode::OK)
+  {
+    delete[] memoryToCompare1;
+    delete[] m_scanRAMCache;
+    m_scanRAMCache = nullptr;
+    return scanReturn;
+  }
+
+  char* memoryToCompare2 = nullptr;
+  if (filter == ScanFiter::between)
+  {
+    memoryToCompare2 = Common::formatStringToMemory(scanReturn, termActualLength, searchTerm2,
+                                                    m_memBase, m_memType, ramSize);
+    if (scanReturn != Common::MemOperationReturnCode::OK)
+    {
+      delete[] memoryToCompare1;
+      delete[] memoryToCompare2;
+      delete[] m_scanRAMCache;
+      m_scanRAMCache = nullptr;
+      return scanReturn;
+    }
+  }
+
+  bool withBSwap = Common::shouldBeBSwappedForType(m_memType);
+
+  m_memSize = Common::getSizeForType(m_memType, termActualLength);
+
+  char* noOffset = new char[m_memSize];
+  std::memset(noOffset, 0, m_memSize);
+
+  int increment = m_enforceMemAlignement ? Common::getNbrBytesAlignementForType(m_memType) : 1;
+  for (u32 i = 0; i < (ramSize - m_memSize); i += increment)
+  {
+    char* memoryCandidate = &m_scanRAMCache[i];
+    bool isResult = false;
+    switch (filter)
+    {
+    case ScanFiter::exact:
+    {
+      if (m_memType == Common::MemType::type_string || m_memType == Common::MemType::type_byteArray)
+        isResult = (std::memcmp(memoryCandidate, memoryToCompare1, m_memSize) == 0);
+      else
+        isResult = (compareMemoryAsNumbers(memoryCandidate, memoryToCompare1, noOffset, false,
+                                           false, m_memSize) == MemScanner::CompareResult::equal);
+      break;
+    }
+    case ScanFiter::between:
+    {
+      MemScanner::CompareResult result1 = compareMemoryAsNumbers(memoryCandidate, memoryToCompare1,
+                                                                 noOffset, false, false, m_memSize);
+      MemScanner::CompareResult result2 = compareMemoryAsNumbers(memoryCandidate, memoryToCompare2,
+                                                                 noOffset, false, false, m_memSize);
+      isResult = ((result1 == MemScanner::CompareResult::bigger ||
+                   result1 == MemScanner::CompareResult::equal) &&
+                  (result2 == MemScanner::CompareResult::smaller ||
+                   result2 == MemScanner::CompareResult::equal));
+      break;
+    }
+    case ScanFiter::biggerThan:
+    {
+      isResult = (compareMemoryAsNumbers(memoryCandidate, memoryToCompare1, noOffset, false, false,
+                                         m_memSize) == MemScanner::CompareResult::bigger);
+      break;
+    }
+    case ScanFiter::smallerThan:
+    {
+      isResult = (compareMemoryAsNumbers(memoryCandidate, memoryToCompare1, noOffset, false, false,
+                                         m_memSize) == MemScanner::CompareResult::smaller);
+      break;
+    }
+    }
+
+    if (isResult)
+    {
+      bool aramAccessible = DolphinComm::DolphinAccessor::isARAMAccessible();
+      u32 consoleOffset = Common::cacheIndexToOffset(i, aramAccessible);
+      m_resultsConsoleAddr.push_back(Common::offsetToDolphinAddr(consoleOffset, aramAccessible));
+    }
+  }
+  delete[] noOffset;
+  delete[] memoryToCompare1;
+  delete[] memoryToCompare2;
+  m_resultCount = m_resultsConsoleAddr.size();
+  m_scanStarted = true;
+  return Common::MemOperationReturnCode::OK;
+}
+
+Common::MemOperationReturnCode MemScanner::nextScan(const MemScanner::ScanFiter filter,
+                                                    const std::string& searchTerm1,
+                                                    const std::string& searchTerm2)
+{
+  char* newerRAMCache = nullptr;
+  if (DolphinComm::DolphinAccessor::updateRAMCache() != Common::MemOperationReturnCode::OK)
+  {
+    return Common::MemOperationReturnCode::operationFailed;
+  }
+  u32 ramSize = DolphinComm::DolphinAccessor::getRAMCacheSize();
+  newerRAMCache = new char[ramSize];
+  std::memcpy(newerRAMCache, DolphinComm::DolphinAccessor::getRAMCache(), ramSize);
+
+  Common::MemOperationReturnCode scanReturn = Common::MemOperationReturnCode::OK;
+  size_t termActualLength = 0;
+  size_t termMaxLength = 0;
+  if (m_memType == Common::MemType::type_string)
+    // This is just to have the string formatted with the appropriate length, byte arrays don't need
+    // this because they get copied byte per byte
+    termMaxLength = searchTerm1.length();
+  else
+    // Have no restriction on the length for the rest
+    termMaxLength = ramSize;
+
+  char* memoryToCompare1 = nullptr;
+  if (filter != ScanFiter::increased && filter != ScanFiter::decreased &&
+      filter != ScanFiter::changed && filter != ScanFiter::unchanged)
+  {
+    std::string formattedSearchTerm1;
+    if (m_memType == Common::MemType::type_byteArray)
+      formattedSearchTerm1 = addSpacesToBytesArrays(searchTerm1);
+    else
+      formattedSearchTerm1 = searchTerm1;
+
+    memoryToCompare1 = Common::formatStringToMemory(
+        scanReturn, termActualLength, formattedSearchTerm1, m_memBase, m_memType, termMaxLength);
+    if (scanReturn != Common::MemOperationReturnCode::OK)
+      return scanReturn;
+  }
+
+  char* memoryToCompare2 = nullptr;
+  if (filter == ScanFiter::between)
+  {
+    memoryToCompare2 = Common::formatStringToMemory(scanReturn, termActualLength, searchTerm2,
+                                                    m_memBase, m_memType, ramSize);
+    if (scanReturn != Common::MemOperationReturnCode::OK)
+      return scanReturn;
+  }
+
+  bool withBSwap = Common::shouldBeBSwappedForType(m_memType);
+
+  m_memSize = Common::getSizeForType(m_memType, termActualLength);
+
+  char* noOffset = new char[m_memSize];
+  std::memset(noOffset, 0, m_memSize);
+
+  std::vector<u32> newerResults = std::vector<u32>();
+  bool aramAccessible = DolphinComm::DolphinAccessor::isARAMAccessible();
+
+  if (m_wasUnknownInitialValue)
+  {
+    m_wasUnknownInitialValue = false;
+
+    int increment = m_enforceMemAlignement ? Common::getNbrBytesAlignementForType(m_memType) : 1;
+    for (u32 i = 0; i < (ramSize - m_memSize); i += increment)
+    {
+      if (isHitNextScan(filter, memoryToCompare1, memoryToCompare2, noOffset, newerRAMCache,
+                        m_memSize, i))
+      {
+        u32 offset = Common::cacheIndexToOffset(i, aramAccessible);
+        newerResults.push_back(Common::offsetToDolphinAddr(offset, aramAccessible));
+      }
+    }
+  }
+  else
+  {
+    for (auto i : m_resultsConsoleAddr)
+    {
+      u32 offset = Common::dolphinAddrToOffset(i, aramAccessible);
+      u32 ramIndex = Common::offsetToCacheIndex(offset, aramAccessible);
+      if (isHitNextScan(filter, memoryToCompare1, memoryToCompare2, noOffset, newerRAMCache,
+                        m_memSize, ramIndex))
+      {
+        newerResults.push_back(i);
+      }
+    }
+  }
+
+  delete[] noOffset;
+  m_resultsConsoleAddr.clear();
+  std::swap(m_resultsConsoleAddr, newerResults);
+  delete[] m_scanRAMCache;
+  m_scanRAMCache = nullptr;
+  m_scanRAMCache = newerRAMCache;
+  m_resultCount = m_resultsConsoleAddr.size();
+  return Common::MemOperationReturnCode::OK;
+}
+
+void MemScanner::reset()
+{
+  m_resultsConsoleAddr.clear();
+  m_wasUnknownInitialValue = false;
+  delete[] m_scanRAMCache;
+  m_scanRAMCache = nullptr;
+  m_resultCount = 0;
+  m_scanStarted = false;
+}
+
+inline bool MemScanner::isHitNextScan(const MemScanner::ScanFiter filter,
+                                      const char* memoryToCompare1, const char* memoryToCompare2,
+                                      const char* noOffset, const char* newerRAMCache,
+                                      const size_t realSize, const u32 consoleOffset) const
+{
+  char* olderMemory = &m_scanRAMCache[consoleOffset];
+  const char* newerMemory = &newerRAMCache[consoleOffset];
+
+  switch (filter)
+  {
+  case ScanFiter::exact:
+  {
+    if (m_memType == Common::MemType::type_string || m_memType == Common::MemType::type_byteArray)
+      return (std::memcmp(newerMemory, memoryToCompare1, realSize) == 0);
+    else
+      return (compareMemoryAsNumbers(newerMemory, memoryToCompare1, noOffset, false, false,
+                                     realSize) == MemScanner::CompareResult::equal);
+  }
+  case ScanFiter::between:
+  {
+    MemScanner::CompareResult result1 =
+        compareMemoryAsNumbers(newerMemory, memoryToCompare1, noOffset, false, false, realSize);
+    MemScanner::CompareResult result2 =
+        compareMemoryAsNumbers(newerMemory, memoryToCompare2, noOffset, false, false, realSize);
+    return ((result1 == MemScanner::CompareResult::bigger ||
+             result1 == MemScanner::CompareResult::equal) &&
+            (result2 == MemScanner::CompareResult::smaller ||
+             result2 == MemScanner::CompareResult::equal));
+  }
+  case ScanFiter::biggerThan:
+  {
+    return (compareMemoryAsNumbers(newerMemory, memoryToCompare1, noOffset, false, false,
+                                   realSize) == MemScanner::CompareResult::bigger);
+  }
+  case ScanFiter::smallerThan:
+  {
+    return (compareMemoryAsNumbers(newerMemory, memoryToCompare1, noOffset, false, false,
+                                   realSize) == MemScanner::CompareResult::smaller);
+  }
+  case ScanFiter::increasedBy:
+  {
+    return (compareMemoryAsNumbers(newerMemory, olderMemory, memoryToCompare1, false, true,
+                                   realSize) == MemScanner::CompareResult::equal);
+  }
+  case ScanFiter::decreasedBy:
+  {
+    return (compareMemoryAsNumbers(newerMemory, olderMemory, memoryToCompare1, true, true,
+                                   realSize) == MemScanner::CompareResult::equal);
+  }
+  case ScanFiter::increased:
+  {
+    return (compareMemoryAsNumbers(newerMemory, olderMemory, noOffset, false, true, realSize) ==
+            MemScanner::CompareResult::bigger);
+  }
+  case ScanFiter::decreased:
+  {
+    return (compareMemoryAsNumbers(newerMemory, olderMemory, noOffset, false, true, realSize) ==
+            MemScanner::CompareResult::smaller);
+  }
+  case ScanFiter::changed:
+  {
+    MemScanner::CompareResult result =
+        compareMemoryAsNumbers(newerMemory, olderMemory, noOffset, false, true, realSize);
+    return (result == MemScanner::CompareResult::bigger ||
+            result == MemScanner::CompareResult::smaller);
+  }
+  case ScanFiter::unchanged:
+  {
+    return (compareMemoryAsNumbers(newerMemory, olderMemory, noOffset, false, true, realSize) ==
+            MemScanner::CompareResult::equal);
+  }
+  default:
+  {
+    return false;
+  }
+  }
+}
+
+inline MemScanner::CompareResult
+MemScanner::compareMemoryAsNumbers(const char* first, const char* second, const char* offset,
+                                   bool offsetInvert, bool bswapSecond, size_t length) const
+{
+  switch (m_memType)
+  {
+  case Common::MemType::type_byte:
+    if (m_memIsSigned)
+      return compareMemoryAsNumbersWithType<s8>(first, second, offset, offsetInvert, bswapSecond);
+    return compareMemoryAsNumbersWithType<u8>(first, second, offset, offsetInvert, bswapSecond);
+  case Common::MemType::type_halfword:
+    if (m_memIsSigned)
+      return compareMemoryAsNumbersWithType<s16>(first, second, offset, offsetInvert, bswapSecond);
+    return compareMemoryAsNumbersWithType<u16>(first, second, offset, offsetInvert, bswapSecond);
+  case Common::MemType::type_word:
+    if (m_memIsSigned)
+      return compareMemoryAsNumbersWithType<s32>(first, second, offset, offsetInvert, bswapSecond);
+    return compareMemoryAsNumbersWithType<u32>(first, second, offset, offsetInvert, bswapSecond);
+  case Common::MemType::type_float:
+    return compareMemoryAsNumbersWithType<float>(first, second, offset, offsetInvert, bswapSecond);
+  case Common::MemType::type_double:
+    return compareMemoryAsNumbersWithType<double>(first, second, offset, offsetInvert, bswapSecond);
+  default:
+    return MemScanner::CompareResult::nan;
+  }
+}
+
+void MemScanner::setType(const Common::MemType type)
+{
+  m_memType = type;
+}
+
+void MemScanner::setBase(const Common::MemBase base)
+{
+  m_memBase = base;
+}
+
+void MemScanner::setEnforceMemAlignement(const bool enforceAlignement)
+{
+  m_enforceMemAlignement = enforceAlignement;
+}
+
+void MemScanner::setIsSigned(const bool isSigned)
+{
+  m_memIsSigned = isSigned;
+}
+
+int MemScanner::getTermsNumForFilter(const MemScanner::ScanFiter filter) const
+{
+  if (filter == MemScanner::ScanFiter::between)
+    return 2;
+  else if (filter == MemScanner::ScanFiter::exact || filter == MemScanner::ScanFiter::increasedBy ||
+           filter == MemScanner::ScanFiter::decreasedBy ||
+           filter == MemScanner::ScanFiter::biggerThan ||
+           filter == MemScanner::ScanFiter::smallerThan)
+    return 1;
+  return 0;
+}
+
+bool MemScanner::typeSupportsAdditionalOptions(const Common::MemType type) const
+{
+  return (type == Common::MemType::type_byte || type == Common::MemType::type_halfword ||
+          type == Common::MemType::type_word);
+}
+
+std::vector<u32> MemScanner::getResultsConsoleAddr() const
+{
+  return m_resultsConsoleAddr;
+}
+
+std::string MemScanner::getFormattedScannedValueAt(const int index) const
+{
+  bool aramAccessible = DolphinComm::DolphinAccessor::isARAMAccessible();
+  u32 offset = Common::dolphinAddrToOffset(m_resultsConsoleAddr.at(index), aramAccessible);
+  u32 ramIndex = Common::offsetToCacheIndex(offset, aramAccessible);
+  return Common::formatMemoryToString(&m_scanRAMCache[ramIndex], m_memType, m_memSize, m_memBase,
+                                      !m_memIsSigned, Common::shouldBeBSwappedForType(m_memType));
+}
+
+Common::MemOperationReturnCode MemScanner::updateCurrentRAMCache()
+{
+  return DolphinComm::DolphinAccessor::updateRAMCache();
+}
+
+std::string MemScanner::getFormattedCurrentValueAt(const int index) const
+{
+  if (DolphinComm::DolphinAccessor::isValidConsoleAddress(m_resultsConsoleAddr.at(index)))
+  {
+    bool aramAccessible = DolphinComm::DolphinAccessor::isARAMAccessible();
+    u32 offset = Common::dolphinAddrToOffset(m_resultsConsoleAddr.at(index), aramAccessible);
+    u32 ramIndex = Common::offsetToCacheIndex(offset, aramAccessible);
+    return DolphinComm::DolphinAccessor::getFormattedValueFromCache(ramIndex, m_memType, m_memSize,
+                                                                    m_memBase, !m_memIsSigned);
+  }
+  return "";
+}
+
+void MemScanner::removeResultAt(int index)
+{
+  m_resultsConsoleAddr.erase(m_resultsConsoleAddr.begin() + index);
+  m_resultCount--;
+}
+
+std::string MemScanner::addSpacesToBytesArrays(const std::string& bytesArray) const
+{
+  std::string result(bytesArray);
+  int spacesAdded = 0;
+  for (int i = 2; i < bytesArray.length(); i += 2)
+  {
+    if (bytesArray[i] != ' ')
+    {
+      result.insert(i + spacesAdded, 1, ' ');
+      spacesAdded++;
+    }
+    else
+    {
+      i++;
+    }
+  }
+  return result;
+}
+
+size_t MemScanner::getResultCount() const
+{
+  return m_resultCount;
+}
+
+bool MemScanner::hasScanStarted() const
+{
+  return m_scanStarted;
+}
+
+Common::MemType MemScanner::getType() const
+{
+  return m_memType;
+}
+
+Common::MemBase MemScanner::getBase() const
+{
+  return m_memBase;
+}
+
+size_t MemScanner::getLength() const
+{
+  return m_memSize;
+}
+
+bool MemScanner::getIsUnsigned() const
+{
+  return !m_memIsSigned;
+}
```

### Comparing `dolphin-memory-engine-1.1.2/Source/MemoryScanner/MemoryScanner.h` & `dolphin-memory-engine-1.1.3/Source/MemoryScanner/MemoryScanner.h`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-#pragma once
-
-#include <cstring>
-#include <string>
-#include <vector>
-
-#include "../Common/CommonTypes.h"
-#include "../Common/CommonUtils.h"
-#include "../Common/MemoryCommon.h"
-
-class MemScanner
-{
-public:
-  enum class ScanFiter
-  {
-    exact = 0,
-    increasedBy,
-    decreasedBy,
-    between,
-    biggerThan,
-    smallerThan,
-    increased,
-    decreased,
-    changed,
-    unchanged,
-    unknownInitial
-  };
-
-  enum class CompareResult
-  {
-    bigger,
-    smaller,
-    equal,
-    nan
-  };
-
-  MemScanner();
-  ~MemScanner();
-  Common::MemOperationReturnCode firstScan(const ScanFiter filter, const std::string& searchTerm1,
-                                           const std::string& searchTerm2);
-  Common::MemOperationReturnCode nextScan(const ScanFiter filter, const std::string& searchTerm1,
-                                          const std::string& searchTerm2);
-  void reset();
-  inline CompareResult compareMemoryAsNumbers(const char* first, const char* second,
-                                              const char* offset, bool offsetInvert,
-                                              bool bswapSecond, size_t length) const;
-
-  template <typename T>
-  inline T convertMemoryToType(const char* memory, bool invert) const
-  {
-    T theType;
-    std::memcpy(&theType, memory, sizeof(T));
-    if (invert)
-      theType *= -1;
-    return theType;
-  }
-
-  template <typename T>
-  inline CompareResult compareMemoryAsNumbersWithType(const char* first, const char* second,
-                                                      const char* offset, bool offsetInvert,
-                                                      bool bswapSecond) const
-  {
-    T firstByte;
-    T secondByte;
-    std::memcpy(&firstByte, first, sizeof(T));
-    std::memcpy(&secondByte, second, sizeof(T));
-    size_t size = sizeof(T);
-    switch (size)
-    {
-    case 2:
-    {
-      u16 firstHalfword = 0;
-      std::memcpy(&firstHalfword, &firstByte, sizeof(u16));
-      firstHalfword = Common::bSwap16(firstHalfword);
-      std::memcpy(&firstByte, &firstHalfword, sizeof(u16));
-      if (bswapSecond)
-      {
-        std::memcpy(&firstHalfword, &secondByte, sizeof(u16));
-        firstHalfword = Common::bSwap16(firstHalfword);
-        std::memcpy(&secondByte, &firstHalfword, sizeof(u16));
-      }
-      break;
-    }
-    case 4:
-    {
-      u32 firstWord = 0;
-      std::memcpy(&firstWord, &firstByte, sizeof(u32));
-      firstWord = Common::bSwap32(firstWord);
-      std::memcpy(&firstByte, &firstWord, sizeof(u32));
-      if (bswapSecond)
-      {
-        std::memcpy(&firstWord, &secondByte, sizeof(u32));
-        firstWord = Common::bSwap32(firstWord);
-        std::memcpy(&secondByte, &firstWord, sizeof(u32));
-      }
-      break;
-    }
-    case 8:
-    {
-      u64 firstDoubleword = 0;
-      std::memcpy(&firstDoubleword, &firstByte, sizeof(u64));
-      firstDoubleword = Common::bSwap64(firstDoubleword);
-      std::memcpy(&firstByte, &firstDoubleword, sizeof(u64));
-      if (bswapSecond)
-      {
-        std::memcpy(&firstDoubleword, &secondByte, sizeof(u64));
-        firstDoubleword = Common::bSwap64(firstDoubleword);
-        std::memcpy(&secondByte, &firstDoubleword, sizeof(u64));
-      }
-      break;
-    }
-    }
-
-    if (firstByte != firstByte)
-      return CompareResult::nan;
-
-    if (firstByte < (secondByte + convertMemoryToType<T>(offset, offsetInvert)))
-      return CompareResult::smaller;
-    else if (firstByte > (secondByte + convertMemoryToType<T>(offset, offsetInvert)))
-      return CompareResult::bigger;
-    else
-      return CompareResult::equal;
-  }
-
-  void setType(const Common::MemType type);
-  void setBase(const Common::MemBase base);
-  void setEnforceMemAlignement(const bool enforceAlignement);
-  void setIsSigned(const bool isSigned);
-
-  std::vector<u32> getResultsConsoleAddr() const;
-  size_t getResultCount() const;
-  int getTermsNumForFilter(const ScanFiter filter) const;
-  Common::MemType getType() const;
-  Common::MemBase getBase() const;
-  size_t getLength() const;
-  bool getIsUnsigned() const;
-  std::string getFormattedScannedValueAt(const int index) const;
-  Common::MemOperationReturnCode updateCurrentRAMCache();
-  std::string getFormattedCurrentValueAt(int index) const;
-  void removeResultAt(int index);
-  bool typeSupportsAdditionalOptions(const Common::MemType type) const;
-  bool hasScanStarted() const;
-
-private:
-  inline bool isHitNextScan(const ScanFiter filter, const char* memoryToCompare1,
-                            const char* memoryToCompare2, const char* noOffset,
-                            const char* newerRAMCache, const size_t realSize,
-                            const u32 consoleOffset) const;
-  std::string addSpacesToBytesArrays(const std::string& bytesArray) const;
-
-  Common::MemType m_memType = Common::MemType::type_byte;
-  Common::MemBase m_memBase = Common::MemBase::base_decimal;
-  size_t m_memSize;
-  bool m_enforceMemAlignement = true;
-  bool m_memIsSigned = false;
-  std::vector<u32> m_resultsConsoleAddr;
-  bool m_wasUnknownInitialValue = false;
-  size_t m_resultCount = 0;
-  char* m_scanRAMCache = nullptr;
-  bool m_scanStarted = false;
-};
+#pragma once
+
+#include <cstring>
+#include <string>
+#include <vector>
+
+#include "../Common/CommonTypes.h"
+#include "../Common/CommonUtils.h"
+#include "../Common/MemoryCommon.h"
+
+class MemScanner
+{
+public:
+  enum class ScanFiter
+  {
+    exact = 0,
+    increasedBy,
+    decreasedBy,
+    between,
+    biggerThan,
+    smallerThan,
+    increased,
+    decreased,
+    changed,
+    unchanged,
+    unknownInitial
+  };
+
+  enum class CompareResult
+  {
+    bigger,
+    smaller,
+    equal,
+    nan
+  };
+
+  MemScanner();
+  ~MemScanner();
+  Common::MemOperationReturnCode firstScan(const ScanFiter filter, const std::string& searchTerm1,
+                                           const std::string& searchTerm2);
+  Common::MemOperationReturnCode nextScan(const ScanFiter filter, const std::string& searchTerm1,
+                                          const std::string& searchTerm2);
+  void reset();
+  inline CompareResult compareMemoryAsNumbers(const char* first, const char* second,
+                                              const char* offset, bool offsetInvert,
+                                              bool bswapSecond, size_t length) const;
+
+  template <typename T>
+  inline T convertMemoryToType(const char* memory, bool invert) const
+  {
+    T theType;
+    std::memcpy(&theType, memory, sizeof(T));
+    if (invert)
+      theType *= -1;
+    return theType;
+  }
+
+  template <typename T>
+  inline CompareResult compareMemoryAsNumbersWithType(const char* first, const char* second,
+                                                      const char* offset, bool offsetInvert,
+                                                      bool bswapSecond) const
+  {
+    T firstByte;
+    T secondByte;
+    std::memcpy(&firstByte, first, sizeof(T));
+    std::memcpy(&secondByte, second, sizeof(T));
+    size_t size = sizeof(T);
+    switch (size)
+    {
+    case 2:
+    {
+      u16 firstHalfword = 0;
+      std::memcpy(&firstHalfword, &firstByte, sizeof(u16));
+      firstHalfword = Common::bSwap16(firstHalfword);
+      std::memcpy(&firstByte, &firstHalfword, sizeof(u16));
+      if (bswapSecond)
+      {
+        std::memcpy(&firstHalfword, &secondByte, sizeof(u16));
+        firstHalfword = Common::bSwap16(firstHalfword);
+        std::memcpy(&secondByte, &firstHalfword, sizeof(u16));
+      }
+      break;
+    }
+    case 4:
+    {
+      u32 firstWord = 0;
+      std::memcpy(&firstWord, &firstByte, sizeof(u32));
+      firstWord = Common::bSwap32(firstWord);
+      std::memcpy(&firstByte, &firstWord, sizeof(u32));
+      if (bswapSecond)
+      {
+        std::memcpy(&firstWord, &secondByte, sizeof(u32));
+        firstWord = Common::bSwap32(firstWord);
+        std::memcpy(&secondByte, &firstWord, sizeof(u32));
+      }
+      break;
+    }
+    case 8:
+    {
+      u64 firstDoubleword = 0;
+      std::memcpy(&firstDoubleword, &firstByte, sizeof(u64));
+      firstDoubleword = Common::bSwap64(firstDoubleword);
+      std::memcpy(&firstByte, &firstDoubleword, sizeof(u64));
+      if (bswapSecond)
+      {
+        std::memcpy(&firstDoubleword, &secondByte, sizeof(u64));
+        firstDoubleword = Common::bSwap64(firstDoubleword);
+        std::memcpy(&secondByte, &firstDoubleword, sizeof(u64));
+      }
+      break;
+    }
+    }
+
+    if (firstByte != firstByte)
+      return CompareResult::nan;
+
+    if (firstByte < (secondByte + convertMemoryToType<T>(offset, offsetInvert)))
+      return CompareResult::smaller;
+    else if (firstByte > (secondByte + convertMemoryToType<T>(offset, offsetInvert)))
+      return CompareResult::bigger;
+    else
+      return CompareResult::equal;
+  }
+
+  void setType(const Common::MemType type);
+  void setBase(const Common::MemBase base);
+  void setEnforceMemAlignement(const bool enforceAlignement);
+  void setIsSigned(const bool isSigned);
+
+  std::vector<u32> getResultsConsoleAddr() const;
+  size_t getResultCount() const;
+  int getTermsNumForFilter(const ScanFiter filter) const;
+  Common::MemType getType() const;
+  Common::MemBase getBase() const;
+  size_t getLength() const;
+  bool getIsUnsigned() const;
+  std::string getFormattedScannedValueAt(const int index) const;
+  Common::MemOperationReturnCode updateCurrentRAMCache();
+  std::string getFormattedCurrentValueAt(int index) const;
+  void removeResultAt(int index);
+  bool typeSupportsAdditionalOptions(const Common::MemType type) const;
+  bool hasScanStarted() const;
+
+private:
+  inline bool isHitNextScan(const ScanFiter filter, const char* memoryToCompare1,
+                            const char* memoryToCompare2, const char* noOffset,
+                            const char* newerRAMCache, const size_t realSize,
+                            const u32 consoleOffset) const;
+  std::string addSpacesToBytesArrays(const std::string& bytesArray) const;
+
+  Common::MemType m_memType = Common::MemType::type_byte;
+  Common::MemBase m_memBase = Common::MemBase::base_decimal;
+  size_t m_memSize;
+  bool m_enforceMemAlignement = true;
+  bool m_memIsSigned = false;
+  std::vector<u32> m_resultsConsoleAddr;
+  bool m_wasUnknownInitialValue = false;
+  size_t m_resultCount = 0;
+  char* m_scanRAMCache = nullptr;
+  bool m_scanStarted = false;
+};
```

### Comparing `dolphin-memory-engine-1.1.2/Source/MemoryWatch/MemWatchEntry.cpp` & `dolphin-memory-engine-1.1.3/Source/MemoryWatch/MemWatchEntry.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,341 +1,343 @@
-#include "MemWatchEntry.h"
-
-#include <bitset>
-#include <cstring>
-#include <iomanip>
-#include <ios>
-#include <limits>
-#include <sstream>
-
-#include "../Common/CommonUtils.h"
-#include "../DolphinProcess/DolphinAccessor.h"
-
-MemWatchEntry::MemWatchEntry(const std::string& label, const u32 consoleAddress,
-                             const Common::MemType type, const Common::MemBase base,
-                             const bool isUnsigned, const size_t length,
-                             const bool isBoundToPointer)
-    : m_label(label), m_consoleAddress(consoleAddress), m_type(type), m_isUnsigned(isUnsigned),
-      m_base(base), m_boundToPointer(isBoundToPointer), m_length(length)
-{
-  m_memory = new char[getSizeForType(m_type, m_length)];
-}
-
-MemWatchEntry::MemWatchEntry()
-{
-  m_type = Common::MemType::type_byte;
-  m_base = Common::MemBase::base_decimal;
-  m_memory = new char[sizeof(u8)];
-  *m_memory = 0;
-  m_isUnsigned = false;
-  m_consoleAddress = 0x80000000;
-}
-
-MemWatchEntry::MemWatchEntry(MemWatchEntry* entry)
-    : m_label(entry->m_label), m_consoleAddress(entry->m_consoleAddress), m_type(entry->m_type),
-      m_isUnsigned(entry->m_isUnsigned), m_base(entry->m_base),
-      m_boundToPointer(entry->m_boundToPointer), m_pointerOffsets(entry->m_pointerOffsets),
-      m_length(entry->m_length), m_isValidPointer(entry->m_isValidPointer)
-{
-  m_memory = new char[getSizeForType(entry->getType(), entry->getLength())];
-  std::memcpy(m_memory, entry->getMemory(), getSizeForType(entry->getType(), entry->getLength()));
-}
-
-MemWatchEntry::~MemWatchEntry()
-{
-  delete[] m_memory;
-  delete[] m_freezeMemory;
-}
-
-std::string MemWatchEntry::getLabel() const
-{
-  return m_label;
-}
-
-size_t MemWatchEntry::getLength() const
-{
-  return m_length;
-}
-
-Common::MemType MemWatchEntry::getType() const
-{
-  return m_type;
-}
-
-u32 MemWatchEntry::getConsoleAddress() const
-{
-  return m_consoleAddress;
-}
-
-bool MemWatchEntry::isLocked() const
-{
-  return m_lock;
-}
-
-bool MemWatchEntry::isBoundToPointer() const
-{
-  return m_boundToPointer;
-}
-
-Common::MemBase MemWatchEntry::getBase() const
-{
-  return m_base;
-}
-
-int MemWatchEntry::getPointerOffset(const int index) const
-{
-  return m_pointerOffsets.at(index);
-}
-
-std::vector<int> MemWatchEntry::getPointerOffsets() const
-{
-  return m_pointerOffsets;
-}
-
-size_t MemWatchEntry::getPointerLevel() const
-{
-  return m_pointerOffsets.size();
-}
-
-char* MemWatchEntry::getMemory() const
-{
-  return m_memory;
-}
-
-bool MemWatchEntry::isUnsigned() const
-{
-  return m_isUnsigned;
-}
-
-void MemWatchEntry::setLabel(const std::string& label)
-{
-  m_label = label;
-}
-
-void MemWatchEntry::setConsoleAddress(const u32 address)
-{
-  m_consoleAddress = address;
-}
-
-void MemWatchEntry::setTypeAndLength(const Common::MemType type, const size_t length)
-{
-  size_t oldSize = getSizeForType(m_type, m_length);
-  m_type = type;
-  m_length = length;
-  size_t newSize = getSizeForType(m_type, m_length);
-  if (oldSize != newSize)
-  {
-    delete[] m_memory;
-    m_memory = new char[newSize];
-    std::fill(m_memory, m_memory + newSize, 0);
-  }
-}
-
-void MemWatchEntry::setBase(const Common::MemBase base)
-{
-  m_base = base;
-}
-
-void MemWatchEntry::setLock(const bool doLock)
-{
-  m_lock = doLock;
-  if (m_lock)
-  {
-    if (readMemoryFromRAM() == Common::MemOperationReturnCode::OK)
-    {
-      m_freezeMemSize = getSizeForType(m_type, m_length);
-      m_freezeMemory = new char[m_freezeMemSize];
-      std::memcpy(m_freezeMemory, m_memory, m_freezeMemSize);
-    }
-  }
-  else if (m_freezeMemory != nullptr)
-  {
-    m_freezeMemSize = 0;
-    delete[] m_freezeMemory;
-    m_freezeMemory = nullptr;
-  }
-}
-
-void MemWatchEntry::setSignedUnsigned(const bool isUnsigned)
-{
-  m_isUnsigned = isUnsigned;
-}
-
-void MemWatchEntry::setBoundToPointer(const bool boundToPointer)
-{
-  m_boundToPointer = boundToPointer;
-}
-
-void MemWatchEntry::setPointerOffset(const int pointerOffset, int index)
-{
-  m_pointerOffsets[index] = pointerOffset;
-}
-
-void MemWatchEntry::removeOffset()
-{
-  m_pointerOffsets.pop_back();
-}
-
-void MemWatchEntry::addOffset(const int offset)
-{
-  m_pointerOffsets.push_back(offset);
-}
-
-Common::MemOperationReturnCode MemWatchEntry::freeze()
-{
-  Common::MemOperationReturnCode writeCode = writeMemoryToRAM(m_freezeMemory, m_freezeMemSize);
-  return writeCode;
-}
-
-u32 MemWatchEntry::getAddressForPointerLevel(const int level)
-{
-  if (!m_boundToPointer && level > m_pointerOffsets.size() && level > 0)
-    return 0;
-
-  u32 address = m_consoleAddress;
-  char addressBuffer[sizeof(u32)] = {0};
-  for (int i = 0; i < level; ++i)
-  {
-    if (DolphinComm::DolphinAccessor::readFromRAM(
-            Common::dolphinAddrToOffset(address,
-                                        DolphinComm::DolphinAccessor::getMEM1ToMEM2Distance()),
-            addressBuffer, sizeof(u32), true))
-    {
-      std::memcpy(&address, addressBuffer, sizeof(u32));
-      if (DolphinComm::DolphinAccessor::isValidConsoleAddress(address))
-        address += m_pointerOffsets.at(i);
-      else
-        return 0;
-    }
-    else
-    {
-      return 0;
-    }
-  }
-  return address;
-}
-
-std::string MemWatchEntry::getAddressStringForPointerLevel(const int level)
-{
-  u32 address = getAddressForPointerLevel(level);
-  if (address == 0)
-  {
-    return "???";
-  }
-  else
-  {
-    std::stringstream ss;
-    ss << std::hex << std::uppercase << address;
-    return ss.str();
-  }
-}
-
-Common::MemOperationReturnCode MemWatchEntry::readMemoryFromRAM()
-{
-  u32 realConsoleAddress = m_consoleAddress;
-  u32 MEM2Distance = DolphinComm::DolphinAccessor::getMEM1ToMEM2Distance();
-  if (m_boundToPointer)
-  {
-    char realConsoleAddressBuffer[sizeof(u32)] = {0};
-    for (int offset : m_pointerOffsets)
-    {
-      if (DolphinComm::DolphinAccessor::readFromRAM(
-              Common::dolphinAddrToOffset(realConsoleAddress, MEM2Distance),
-              realConsoleAddressBuffer, sizeof(u32), true))
-      {
-        std::memcpy(&realConsoleAddress, realConsoleAddressBuffer, sizeof(u32));
-        if (DolphinComm::DolphinAccessor::isValidConsoleAddress(realConsoleAddress))
-        {
-          realConsoleAddress += offset;
-        }
-        else
-        {
-          m_isValidPointer = false;
-          return Common::MemOperationReturnCode::invalidPointer;
-        }
-      }
-      else
-      {
-        return Common::MemOperationReturnCode::operationFailed;
-      }
-    }
-    // Resolve sucessful
-    m_isValidPointer = true;
-  }
-  if (DolphinComm::DolphinAccessor::readFromRAM(
-          Common::dolphinAddrToOffset(realConsoleAddress, MEM2Distance), m_memory,
-          getSizeForType(m_type, m_length), shouldBeBSwappedForType(m_type)))
-    return Common::MemOperationReturnCode::OK;
-  return Common::MemOperationReturnCode::operationFailed;
-}
-
-Common::MemOperationReturnCode MemWatchEntry::writeMemoryToRAM(const char* memory,
-                                                               const size_t size)
-{
-  u32 realConsoleAddress = m_consoleAddress;
-  u32 MEM2Distance = DolphinComm::DolphinAccessor::getMEM1ToMEM2Distance();
-  if (m_boundToPointer)
-  {
-    char realConsoleAddressBuffer[sizeof(u32)] = {0};
-    for (int offset : m_pointerOffsets)
-    {
-      if (DolphinComm::DolphinAccessor::readFromRAM(
-              Common::dolphinAddrToOffset(realConsoleAddress, MEM2Distance),
-              realConsoleAddressBuffer, sizeof(u32), true))
-      {
-        std::memcpy(&realConsoleAddress, realConsoleAddressBuffer, sizeof(u32));
-        if (DolphinComm::DolphinAccessor::isValidConsoleAddress(realConsoleAddress))
-        {
-          realConsoleAddress += offset;
-        }
-        else
-        {
-          m_isValidPointer = false;
-          return Common::MemOperationReturnCode::invalidPointer;
-        }
-      }
-      else
-      {
-        return Common::MemOperationReturnCode::operationFailed;
-      }
-    }
-    // Resolve sucessful
-    m_isValidPointer = true;
-  }
-
-  if (DolphinComm::DolphinAccessor::writeToRAM(
-          Common::dolphinAddrToOffset(realConsoleAddress, MEM2Distance), memory, size,
-          shouldBeBSwappedForType(m_type)))
-    return Common::MemOperationReturnCode::OK;
-  return Common::MemOperationReturnCode::operationFailed;
-}
-
-std::string MemWatchEntry::getStringFromMemory() const
-{
-  if (m_boundToPointer && !m_isValidPointer)
-    return "???";
-  return Common::formatMemoryToString(m_memory, m_type, m_length, m_base, m_isUnsigned);
-}
-
-Common::MemOperationReturnCode MemWatchEntry::writeMemoryFromString(const std::string& inputString)
-{
-  Common::MemOperationReturnCode writeReturn = Common::MemOperationReturnCode::OK;
-  size_t sizeToWrite = 0;
-  char* buffer =
-      Common::formatStringToMemory(writeReturn, sizeToWrite, inputString, m_base, m_type, m_length);
-  if (writeReturn != Common::MemOperationReturnCode::OK)
-    return writeReturn;
-
-  writeReturn = writeMemoryToRAM(buffer, sizeToWrite);
-  if (writeReturn == Common::MemOperationReturnCode::OK)
-  {
-    if (m_lock)
-      std::memcpy(m_freezeMemory, buffer, m_freezeMemSize);
-    delete[] buffer;
-    return writeReturn;
-  }
-  else
-  {
-    delete[] buffer;
-    return writeReturn;
-  }
-}
+#include "MemWatchEntry.h"
+
+#include <bitset>
+#include <cstring>
+#include <iomanip>
+#include <ios>
+#include <limits>
+#include <sstream>
+
+#include "../Common/CommonUtils.h"
+#include "../DolphinProcess/DolphinAccessor.h"
+
+MemWatchEntry::MemWatchEntry(const std::string& label, const u32 consoleAddress,
+                             const Common::MemType type, const Common::MemBase base,
+                             const bool isUnsigned, const size_t length,
+                             const bool isBoundToPointer)
+    : m_label(label), m_consoleAddress(consoleAddress), m_type(type), m_isUnsigned(isUnsigned),
+      m_base(base), m_boundToPointer(isBoundToPointer), m_length(length)
+{
+  m_memory = new char[getSizeForType(m_type, m_length)];
+}
+
+MemWatchEntry::MemWatchEntry()
+{
+  m_type = Common::MemType::type_byte;
+  m_base = Common::MemBase::base_decimal;
+  m_memory = new char[sizeof(u8)];
+  *m_memory = 0;
+  m_isUnsigned = false;
+  m_consoleAddress = 0x80000000;
+}
+
+MemWatchEntry::MemWatchEntry(MemWatchEntry* entry)
+    : m_label(entry->m_label), m_consoleAddress(entry->m_consoleAddress), m_type(entry->m_type),
+      m_isUnsigned(entry->m_isUnsigned), m_base(entry->m_base),
+      m_boundToPointer(entry->m_boundToPointer), m_pointerOffsets(entry->m_pointerOffsets),
+      m_length(entry->m_length), m_isValidPointer(entry->m_isValidPointer)
+{
+  m_memory = new char[getSizeForType(entry->getType(), entry->getLength())];
+  std::memcpy(m_memory, entry->getMemory(), getSizeForType(entry->getType(), entry->getLength()));
+}
+
+MemWatchEntry::~MemWatchEntry()
+{
+  delete[] m_memory;
+  delete[] m_freezeMemory;
+}
+
+std::string MemWatchEntry::getLabel() const
+{
+  return m_label;
+}
+
+size_t MemWatchEntry::getLength() const
+{
+  return m_length;
+}
+
+Common::MemType MemWatchEntry::getType() const
+{
+  return m_type;
+}
+
+u32 MemWatchEntry::getConsoleAddress() const
+{
+  return m_consoleAddress;
+}
+
+bool MemWatchEntry::isLocked() const
+{
+  return m_lock;
+}
+
+bool MemWatchEntry::isBoundToPointer() const
+{
+  return m_boundToPointer;
+}
+
+Common::MemBase MemWatchEntry::getBase() const
+{
+  return m_base;
+}
+
+int MemWatchEntry::getPointerOffset(const int index) const
+{
+  return m_pointerOffsets.at(index);
+}
+
+std::vector<int> MemWatchEntry::getPointerOffsets() const
+{
+  return m_pointerOffsets;
+}
+
+size_t MemWatchEntry::getPointerLevel() const
+{
+  return m_pointerOffsets.size();
+}
+
+char* MemWatchEntry::getMemory() const
+{
+  return m_memory;
+}
+
+bool MemWatchEntry::isUnsigned() const
+{
+  return m_isUnsigned;
+}
+
+void MemWatchEntry::setLabel(const std::string& label)
+{
+  m_label = label;
+}
+
+void MemWatchEntry::setConsoleAddress(const u32 address)
+{
+  m_consoleAddress = address;
+}
+
+void MemWatchEntry::setTypeAndLength(const Common::MemType type, const size_t length)
+{
+  size_t oldSize = getSizeForType(m_type, m_length);
+  m_type = type;
+  m_length = length;
+  size_t newSize = getSizeForType(m_type, m_length);
+  if (oldSize != newSize)
+  {
+    delete[] m_memory;
+    m_memory = new char[newSize];
+    std::fill(m_memory, m_memory + newSize, 0);
+  }
+}
+
+void MemWatchEntry::setBase(const Common::MemBase base)
+{
+  m_base = base;
+}
+
+void MemWatchEntry::setLock(const bool doLock)
+{
+  m_lock = doLock;
+  if (m_lock)
+  {
+    if (readMemoryFromRAM() == Common::MemOperationReturnCode::OK)
+    {
+      m_freezeMemSize = getSizeForType(m_type, m_length);
+      m_freezeMemory = new char[m_freezeMemSize];
+      std::memcpy(m_freezeMemory, m_memory, m_freezeMemSize);
+    }
+  }
+  else if (m_freezeMemory != nullptr)
+  {
+    m_freezeMemSize = 0;
+    delete[] m_freezeMemory;
+    m_freezeMemory = nullptr;
+  }
+}
+
+void MemWatchEntry::setSignedUnsigned(const bool isUnsigned)
+{
+  m_isUnsigned = isUnsigned;
+}
+
+void MemWatchEntry::setBoundToPointer(const bool boundToPointer)
+{
+  m_boundToPointer = boundToPointer;
+}
+
+void MemWatchEntry::setPointerOffset(const int pointerOffset, int index)
+{
+  m_pointerOffsets[index] = pointerOffset;
+}
+
+void MemWatchEntry::removeOffset()
+{
+  m_pointerOffsets.pop_back();
+}
+
+void MemWatchEntry::addOffset(const int offset)
+{
+  m_pointerOffsets.push_back(offset);
+}
+
+Common::MemOperationReturnCode MemWatchEntry::freeze()
+{
+  Common::MemOperationReturnCode writeCode = writeMemoryToRAM(m_freezeMemory, m_freezeMemSize);
+  return writeCode;
+}
+
+u32 MemWatchEntry::getAddressForPointerLevel(const int level)
+{
+  if (!m_boundToPointer && level > m_pointerOffsets.size() && level > 0)
+    return 0;
+
+  u32 address = m_consoleAddress;
+  char addressBuffer[sizeof(u32)] = {0};
+  for (int i = 0; i < level; ++i)
+  {
+    if (DolphinComm::DolphinAccessor::readFromRAM(
+            Common::dolphinAddrToOffset(address, DolphinComm::DolphinAccessor::isARAMAccessible()),
+            addressBuffer, sizeof(u32), true))
+    {
+      std::memcpy(&address, addressBuffer, sizeof(u32));
+      if (DolphinComm::DolphinAccessor::isValidConsoleAddress(address))
+        address += m_pointerOffsets.at(i);
+      else
+        return 0;
+    }
+    else
+    {
+      return 0;
+    }
+  }
+  return address;
+}
+
+std::string MemWatchEntry::getAddressStringForPointerLevel(const int level)
+{
+  u32 address = getAddressForPointerLevel(level);
+  if (address == 0)
+  {
+    return "???";
+  }
+  else
+  {
+    std::stringstream ss;
+    ss << std::hex << std::uppercase << address;
+    return ss.str();
+  }
+}
+
+Common::MemOperationReturnCode MemWatchEntry::readMemoryFromRAM()
+{
+  u32 realConsoleAddress = m_consoleAddress;
+  if (m_boundToPointer)
+  {
+    char realConsoleAddressBuffer[sizeof(u32)] = {0};
+    for (int offset : m_pointerOffsets)
+    {
+      if (DolphinComm::DolphinAccessor::readFromRAM(
+              Common::dolphinAddrToOffset(realConsoleAddress,
+                                          DolphinComm::DolphinAccessor::isARAMAccessible()),
+              realConsoleAddressBuffer, sizeof(u32), true))
+      {
+        std::memcpy(&realConsoleAddress, realConsoleAddressBuffer, sizeof(u32));
+        if (DolphinComm::DolphinAccessor::isValidConsoleAddress(realConsoleAddress))
+        {
+          realConsoleAddress += offset;
+        }
+        else
+        {
+          m_isValidPointer = false;
+          return Common::MemOperationReturnCode::invalidPointer;
+        }
+      }
+      else
+      {
+        return Common::MemOperationReturnCode::operationFailed;
+      }
+    }
+    // Resolve sucessful
+    m_isValidPointer = true;
+  }
+
+  if (DolphinComm::DolphinAccessor::readFromRAM(
+          Common::dolphinAddrToOffset(realConsoleAddress,
+                                      DolphinComm::DolphinAccessor::isARAMAccessible()),
+          m_memory, getSizeForType(m_type, m_length), shouldBeBSwappedForType(m_type)))
+    return Common::MemOperationReturnCode::OK;
+  return Common::MemOperationReturnCode::operationFailed;
+}
+
+Common::MemOperationReturnCode MemWatchEntry::writeMemoryToRAM(const char* memory,
+                                                               const size_t size)
+{
+  u32 realConsoleAddress = m_consoleAddress;
+  if (m_boundToPointer)
+  {
+    char realConsoleAddressBuffer[sizeof(u32)] = {0};
+    for (int offset : m_pointerOffsets)
+    {
+      if (DolphinComm::DolphinAccessor::readFromRAM(
+              Common::dolphinAddrToOffset(realConsoleAddress,
+                                          DolphinComm::DolphinAccessor::isARAMAccessible()),
+              realConsoleAddressBuffer, sizeof(u32), true))
+      {
+        std::memcpy(&realConsoleAddress, realConsoleAddressBuffer, sizeof(u32));
+        if (DolphinComm::DolphinAccessor::isValidConsoleAddress(realConsoleAddress))
+        {
+          realConsoleAddress += offset;
+        }
+        else
+        {
+          m_isValidPointer = false;
+          return Common::MemOperationReturnCode::invalidPointer;
+        }
+      }
+      else
+      {
+        return Common::MemOperationReturnCode::operationFailed;
+      }
+    }
+    // Resolve sucessful
+    m_isValidPointer = true;
+  }
+
+  if (DolphinComm::DolphinAccessor::writeToRAM(
+          Common::dolphinAddrToOffset(realConsoleAddress,
+                                      DolphinComm::DolphinAccessor::isARAMAccessible()),
+          memory, size, shouldBeBSwappedForType(m_type)))
+    return Common::MemOperationReturnCode::OK;
+  return Common::MemOperationReturnCode::operationFailed;
+}
+
+std::string MemWatchEntry::getStringFromMemory() const
+{
+  if (m_boundToPointer && !m_isValidPointer)
+    return "???";
+  return Common::formatMemoryToString(m_memory, m_type, m_length, m_base, m_isUnsigned);
+}
+
+Common::MemOperationReturnCode MemWatchEntry::writeMemoryFromString(const std::string& inputString)
+{
+  Common::MemOperationReturnCode writeReturn = Common::MemOperationReturnCode::OK;
+  size_t sizeToWrite = 0;
+  char* buffer =
+      Common::formatStringToMemory(writeReturn, sizeToWrite, inputString, m_base, m_type, m_length);
+  if (writeReturn != Common::MemOperationReturnCode::OK)
+    return writeReturn;
+
+  writeReturn = writeMemoryToRAM(buffer, sizeToWrite);
+  if (writeReturn == Common::MemOperationReturnCode::OK)
+  {
+    if (m_lock)
+      std::memcpy(m_freezeMemory, buffer, m_freezeMemSize);
+    delete[] buffer;
+    return writeReturn;
+  }
+  else
+  {
+    delete[] buffer;
+    return writeReturn;
+  }
+}
```

### Comparing `dolphin-memory-engine-1.1.2/Source/MemoryWatch/MemWatchEntry.h` & `dolphin-memory-engine-1.1.3/Source/MemoryWatch/MemWatchEntry.h`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-#pragma once
-
-#include <string>
-#include <vector>
-
-#include "../Common/CommonTypes.h"
-#include "../Common/MemoryCommon.h"
-
-class MemWatchEntry
-{
-public:
-  MemWatchEntry();
-  MemWatchEntry(const std::string& label, const u32 consoleAddress, const Common::MemType type,
-                const Common::MemBase = Common::MemBase::base_decimal,
-                const bool m_isUnsigned = false, const size_t length = 1,
-                const bool isBoundToPointer = false);
-  MemWatchEntry(MemWatchEntry* entry);
-  ~MemWatchEntry();
-
-  std::string getLabel() const;
-  Common::MemType getType() const;
-  u32 getConsoleAddress() const;
-  bool isLocked() const;
-  bool isBoundToPointer() const;
-  Common::MemBase getBase() const;
-  size_t getLength() const;
-  char* getMemory() const;
-  bool isUnsigned() const;
-  int getPointerOffset(const int index) const;
-  std::vector<int> getPointerOffsets() const;
-  size_t getPointerLevel() const;
-  void setLabel(const std::string& label);
-  void setConsoleAddress(const u32 address);
-  void setTypeAndLength(const Common::MemType type, const size_t length = 1);
-  void setBase(const Common::MemBase base);
-  void setLock(const bool doLock);
-  void setSignedUnsigned(const bool isUnsigned);
-  void setBoundToPointer(const bool boundToPointer);
-  void setPointerOffset(const int pointerOffset, const int index);
-  void addOffset(const int offset);
-  void removeOffset();
-
-  Common::MemOperationReturnCode freeze();
-
-  u32 getAddressForPointerLevel(const int level);
-  std::string getAddressStringForPointerLevel(const int level);
-  Common::MemOperationReturnCode readMemoryFromRAM();
-
-  std::string getStringFromMemory() const;
-  Common::MemOperationReturnCode writeMemoryFromString(const std::string& inputString);
-
-private:
-  Common::MemOperationReturnCode writeMemoryToRAM(const char* memory, const size_t size);
-
-  std::string m_label;
-  u32 m_consoleAddress;
-  bool m_lock = false;
-  Common::MemType m_type;
-  Common::MemBase m_base;
-  bool m_isUnsigned;
-  bool m_boundToPointer = false;
-  std::vector<int> m_pointerOffsets;
-  bool m_isValidPointer = false;
-  char* m_memory;
-  char* m_freezeMemory = nullptr;
-  size_t m_freezeMemSize = 0;
-  size_t m_length = 1;
-};
+#pragma once
+
+#include <string>
+#include <vector>
+
+#include "../Common/CommonTypes.h"
+#include "../Common/MemoryCommon.h"
+
+class MemWatchEntry
+{
+public:
+  MemWatchEntry();
+  MemWatchEntry(const std::string& label, const u32 consoleAddress, const Common::MemType type,
+                const Common::MemBase = Common::MemBase::base_decimal,
+                const bool m_isUnsigned = false, const size_t length = 1,
+                const bool isBoundToPointer = false);
+  MemWatchEntry(MemWatchEntry* entry);
+  ~MemWatchEntry();
+
+  std::string getLabel() const;
+  Common::MemType getType() const;
+  u32 getConsoleAddress() const;
+  bool isLocked() const;
+  bool isBoundToPointer() const;
+  Common::MemBase getBase() const;
+  size_t getLength() const;
+  char* getMemory() const;
+  bool isUnsigned() const;
+  int getPointerOffset(const int index) const;
+  std::vector<int> getPointerOffsets() const;
+  size_t getPointerLevel() const;
+  void setLabel(const std::string& label);
+  void setConsoleAddress(const u32 address);
+  void setTypeAndLength(const Common::MemType type, const size_t length = 1);
+  void setBase(const Common::MemBase base);
+  void setLock(const bool doLock);
+  void setSignedUnsigned(const bool isUnsigned);
+  void setBoundToPointer(const bool boundToPointer);
+  void setPointerOffset(const int pointerOffset, const int index);
+  void addOffset(const int offset);
+  void removeOffset();
+
+  Common::MemOperationReturnCode freeze();
+
+  u32 getAddressForPointerLevel(const int level);
+  std::string getAddressStringForPointerLevel(const int level);
+  Common::MemOperationReturnCode readMemoryFromRAM();
+
+  std::string getStringFromMemory() const;
+  Common::MemOperationReturnCode writeMemoryFromString(const std::string& inputString);
+
+private:
+  Common::MemOperationReturnCode writeMemoryToRAM(const char* memory, const size_t size);
+
+  std::string m_label;
+  u32 m_consoleAddress;
+  bool m_lock = false;
+  Common::MemType m_type;
+  Common::MemBase m_base;
+  bool m_isUnsigned;
+  bool m_boundToPointer = false;
+  std::vector<int> m_pointerOffsets;
+  bool m_isValidPointer = false;
+  char* m_memory;
+  char* m_freezeMemory = nullptr;
+  size_t m_freezeMemSize = 0;
+  size_t m_length = 1;
+};
```

### Comparing `dolphin-memory-engine-1.1.2/_dolphin_memory_engine.cpp` & `dolphin-memory-engine-1.1.3/_dolphin_memory_engine.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "cmake_options": {
-            "dir": "/Users/runner/work/py-dolphin-memory-engine/py-dolphin-memory-engine/Source",
+            "dir": "D:\\a\\py-dolphin-memory-engine\\py-dolphin-memory-engine\\Source",
             "targets": {
                 "dolphin-memory-engine": "lib"
             }
         },
         "depends": [],
         "extra_compile_args": [
-            "-std=c++17"
+            "-DUNICODE",
+            "/std:c++17",
+            "/MD"
         ],
         "language": "c++",
-        "name": "_dolphin_memory_engine",
+        "name": "dolphin_memory_engine._dolphin_memory_engine",
         "sources": [
             "_dolphin_memory_engine.pyx"
         ]
     },
-    "module_name": "_dolphin_memory_engine"
+    "module_name": "dolphin_memory_engine._dolphin_memory_engine"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -97,24 +99,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -222,15 +228,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -261,15 +267,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -398,17 +404,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -478,14 +481,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -585,35 +593,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -771,16 +779,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE___dolphin_memory_engine
-#define __PYX_HAVE_API___dolphin_memory_engine
+#define __PYX_HAVE__dolphin_memory_engine___dolphin_memory_engine
+#define __PYX_HAVE_API__dolphin_memory_engine___dolphin_memory_engine
 /* Early includes */
 #include <stdint.h>
 #include <string.h>
 #include <string>
 #include "ios"
 #include "new"
 #include "stdexcept"
@@ -999,24 +1007,24 @@
 
 static const char *__pyx_f[] = {
   "stringsource",
   "_dolphin_memory_engine.pyx",
 };
 
 /*--- Type declarations ---*/
-struct __pyx_obj_22_dolphin_memory_engine_MemWatch;
+struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch;
 
 /* "_dolphin_memory_engine.pyx":99
  * 
  * 
  * cdef class MemWatch:             # <<<<<<<<<<<<<<
  *     cdef MemWatchEntry c_entry
  * 
  */
-struct __pyx_obj_22_dolphin_memory_engine_MemWatch {
+struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch {
   PyObject_HEAD
   MemWatchEntry c_entry;
 };
 
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
@@ -1180,26 +1188,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1401,25 +1409,25 @@
 
 /* Module declarations from 'libcpp' */
 
 /* Module declarations from 'libc.string' */
 
 /* Module declarations from 'libcpp.string' */
 
-/* Module declarations from '_dolphin_memory_engine' */
-static PyTypeObject *__pyx_ptype_22_dolphin_memory_engine_MemWatch = 0;
-static PyObject *__pyx_f_22_dolphin_memory_engine_buffer_to_word(char *); /*proto*/
-static PyObject *__pyx_f_22_dolphin_memory_engine__read_memory(PyObject *, char *, int); /*proto*/
-static PyObject *__pyx_f_22_dolphin_memory_engine__write_memory(PyObject *, char *, int); /*proto*/
+/* Module declarations from 'dolphin_memory_engine._dolphin_memory_engine' */
+static PyTypeObject *__pyx_ptype_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch = 0;
+static PyObject *__pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine_buffer_to_word(char *); /*proto*/
+static PyObject *__pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine__read_memory(PyObject *, char *, int); /*proto*/
+static PyObject *__pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine__write_memory(PyObject *, char *, int); /*proto*/
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
-#define __Pyx_MODULE_NAME "_dolphin_memory_engine"
-extern int __pyx_module_is_main__dolphin_memory_engine;
-int __pyx_module_is_main__dolphin_memory_engine = 0;
+#define __Pyx_MODULE_NAME "dolphin_memory_engine._dolphin_memory_engine"
+extern int __pyx_module_is_main_dolphin_memory_engine___dolphin_memory_engine;
+int __pyx_module_is_main_dolphin_memory_engine___dolphin_memory_engine = 0;
 
-/* Implementation of '_dolphin_memory_engine' */
+/* Implementation of 'dolphin_memory_engine._dolphin_memory_engine' */
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_RuntimeError;
 static const char __pyx_k_List[] = "List";
 static const char __pyx_k_hook[] = "hook";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_size[] = "size";
@@ -1448,52 +1456,52 @@
 static const char __pyx_k_write_byte[] = "write_byte";
 static const char __pyx_k_write_word[] = "write_word";
 static const char __pyx_k_read_double[] = "read_double";
 static const char __pyx_k_write_bytes[] = "write_bytes";
 static const char __pyx_k_write_float[] = "write_float";
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_is_not_valid[] = " is not valid";
-static const char __pyx_k_mem2Distance[] = "mem2Distance";
 static const char __pyx_k_write_double[] = "write_double";
 static const char __pyx_k_assert_hooked[] = "assert_hooked";
 static const char __pyx_k_memory_buffer[] = "memory_buffer";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_console_address[] = "console_address";
 static const char __pyx_k_follow_pointers[] = "follow_pointers";
 static const char __pyx_k_pointer_offsets[] = "pointer_offsets";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_is_aram_accessible[] = "is_aram_accessible";
 static const char __pyx_k_real_console_address[] = "real_console_address";
-static const char __pyx_k_dolphin_memory_engine[] = "_dolphin_memory_engine";
 static const char __pyx_k_Could_not_read_memory_at[] = "Could not read memory at ";
 static const char __pyx_k_Could_not_write_memory_at[] = "Could not write memory at ";
 static const char __pyx_k_dolphin_memory_engine_pyx[] = "_dolphin_memory_engine.pyx";
+static const char __pyx_k_dolphin_memory_engine__dolphin_m[] = "dolphin_memory_engine._dolphin_memory_engine";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static PyObject *__pyx_kp_u_Address;
 static PyObject *__pyx_kp_u_Could_not_read_memory_at;
 static PyObject *__pyx_kp_u_Could_not_write_memory_at;
 static PyObject *__pyx_n_s_List;
 static PyObject *__pyx_n_s_MemWatch;
 static PyObject *__pyx_n_s_RuntimeError;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_assert_hooked;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_console_address;
-static PyObject *__pyx_n_s_dolphin_memory_engine;
+static PyObject *__pyx_n_s_dolphin_memory_engine__dolphin_m;
 static PyObject *__pyx_kp_s_dolphin_memory_engine_pyx;
 static PyObject *__pyx_n_s_follow_pointers;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_hook;
 static PyObject *__pyx_n_s_import;
+static PyObject *__pyx_n_s_is_aram_accessible;
 static PyObject *__pyx_n_s_is_hooked;
 static PyObject *__pyx_kp_u_is_not_valid;
 static PyObject *__pyx_n_s_is_pointer;
 static PyObject *__pyx_n_s_label;
 static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_mem2Distance;
 static PyObject *__pyx_n_s_memory;
 static PyObject *__pyx_n_s_memory_buffer;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_kp_u_not_hooked;
 static PyObject *__pyx_n_s_offset;
 static PyObject *__pyx_n_s_pointer_offsets;
@@ -1514,37 +1522,37 @@
 static PyObject *__pyx_n_s_un_hook;
 static PyObject *__pyx_n_s_value;
 static PyObject *__pyx_n_s_write_byte;
 static PyObject *__pyx_n_s_write_bytes;
 static PyObject *__pyx_n_s_write_double;
 static PyObject *__pyx_n_s_write_float;
 static PyObject *__pyx_n_s_write_word;
-static int __pyx_pf_22_dolphin_memory_engine_8MemWatch___cinit__(struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self, PyObject *__pyx_v_label, PyObject *__pyx_v_console_address, PyObject *__pyx_v_is_pointer); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8MemWatch_2add_offset(struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self, PyObject *__pyx_v_offset); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8MemWatch_4get_value(struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8MemWatch_6read_memory_from_ram(struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8MemWatch_8write_memory_from_string(struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8MemWatch_10__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8MemWatch_12__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_hook(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_2un_hook(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_4is_hooked(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_6assert_hooked(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8follow_pointers(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_pointer_offsets); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_10read_byte(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_12read_word(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_14read_float(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_16read_double(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_18read_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_size); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_20write_byte(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_22write_word(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_24write_float(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, double __pyx_v_value); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_26write_double(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, double __pyx_v_value); /* proto */
-static PyObject *__pyx_pf_22_dolphin_memory_engine_28write_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_memory); /* proto */
-static PyObject *__pyx_tp_new_22_dolphin_memory_engine_MemWatch(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static int __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch___cinit__(struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self, PyObject *__pyx_v_label, PyObject *__pyx_v_console_address, PyObject *__pyx_v_is_pointer); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_2add_offset(struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self, PyObject *__pyx_v_offset); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_4get_value(struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_6read_memory_from_ram(struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_8write_memory_from_string(struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_10__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_12__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_hook(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_2un_hook(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_4is_hooked(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_6assert_hooked(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8follow_pointers(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_pointer_offsets); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_10read_byte(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_12read_word(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_14read_float(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_16read_double(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_18read_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_size); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_20write_byte(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_22write_word(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_24write_float(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, double __pyx_v_value); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_26write_double(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, double __pyx_v_value); /* proto */
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_28write_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_memory); /* proto */
+static PyObject *__pyx_tp_new_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__14;
@@ -1576,15 +1584,15 @@
  * 
  * 
  * cdef buffer_to_word(char* buffer):             # <<<<<<<<<<<<<<
  *     cdef uint32_t* value = <uint32_t*> buffer
  *     return value[0]
  */
 
-static PyObject *__pyx_f_22_dolphin_memory_engine_buffer_to_word(char *__pyx_v_buffer) {
+static PyObject *__pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine_buffer_to_word(char *__pyx_v_buffer) {
   uint32_t *__pyx_v_value;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -1620,15 +1628,15 @@
  *     cdef uint32_t* value = <uint32_t*> buffer
  *     return value[0]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.buffer_to_word", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.buffer_to_word", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -1636,15 +1644,15 @@
  * 
  * 
  * cdef buffer_to_float(char* buffer):             # <<<<<<<<<<<<<<
  *     cdef float* value = <float*> buffer
  *     return value[0]
  */
 
-static PyObject *__pyx_f_22_dolphin_memory_engine_buffer_to_float(char *__pyx_v_buffer) {
+static PyObject *__pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine_buffer_to_float(char *__pyx_v_buffer) {
   float *__pyx_v_value;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -1680,15 +1688,15 @@
  *     cdef float* value = <float*> buffer
  *     return value[0]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.buffer_to_float", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.buffer_to_float", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -1696,15 +1704,15 @@
  * 
  * 
  * cdef buffer_to_double(char* buffer):             # <<<<<<<<<<<<<<
  *     cdef double* value = <double*> buffer
  *     return value[0]
  */
 
-static PyObject *__pyx_f_22_dolphin_memory_engine_buffer_to_double(char *__pyx_v_buffer) {
+static PyObject *__pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine_buffer_to_double(char *__pyx_v_buffer) {
   double *__pyx_v_value;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -1740,15 +1748,15 @@
  *     cdef double* value = <double*> buffer
  *     return value[0]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.buffer_to_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.buffer_to_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -1757,16 +1765,16 @@
  * 
  *     def __cinit__(self, label: str, console_address: int, is_pointer: bool):             # <<<<<<<<<<<<<<
  *         self.c_entry = MemWatchEntry(label.encode("utf-8"), console_address, MemType.type_word, MemBase.base_decimal, False, 1, is_pointer)
  * 
  */
 
 /* Python wrapper */
-static int __pyx_pw_22_dolphin_memory_engine_8MemWatch_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_22_dolphin_memory_engine_8MemWatch_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_label = 0;
   PyObject *__pyx_v_console_address = 0;
   PyObject *__pyx_v_is_pointer = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
@@ -1820,31 +1828,31 @@
     __pyx_v_console_address = values[1];
     __pyx_v_is_pointer = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 102, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("_dolphin_memory_engine.MemWatch.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.MemWatch.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_label), (&PyUnicode_Type), 1, "label", 1))) __PYX_ERR(1, 102, __pyx_L1_error)
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_8MemWatch___cinit__(((struct __pyx_obj_22_dolphin_memory_engine_MemWatch *)__pyx_v_self), __pyx_v_label, __pyx_v_console_address, __pyx_v_is_pointer);
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch___cinit__(((struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *)__pyx_v_self), __pyx_v_label, __pyx_v_console_address, __pyx_v_is_pointer);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_22_dolphin_memory_engine_8MemWatch___cinit__(struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self, PyObject *__pyx_v_label, PyObject *__pyx_v_console_address, PyObject *__pyx_v_is_pointer) {
+static int __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch___cinit__(struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self, PyObject *__pyx_v_label, PyObject *__pyx_v_console_address, PyObject *__pyx_v_is_pointer) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   std::string __pyx_t_2;
   uint32_t __pyx_t_3;
   bool __pyx_t_4;
   int __pyx_lineno = 0;
@@ -1880,15 +1888,15 @@
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.MemWatch.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.MemWatch.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "_dolphin_memory_engine.pyx":105
@@ -1896,28 +1904,28 @@
  * 
  *     def add_offset(self, offset: int):             # <<<<<<<<<<<<<<
  *         self.c_entry.addOffset(offset)
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_8MemWatch_3add_offset(PyObject *__pyx_v_self, PyObject *__pyx_v_offset); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_8MemWatch_2add_offset[] = "MemWatch.add_offset(self, offset: int)";
-static PyObject *__pyx_pw_22_dolphin_memory_engine_8MemWatch_3add_offset(PyObject *__pyx_v_self, PyObject *__pyx_v_offset) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_3add_offset(PyObject *__pyx_v_self, PyObject *__pyx_v_offset); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_2add_offset[] = "MemWatch.add_offset(self, offset: int)";
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_3add_offset(PyObject *__pyx_v_self, PyObject *__pyx_v_offset) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("add_offset (wrapper)", 0);
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_8MemWatch_2add_offset(((struct __pyx_obj_22_dolphin_memory_engine_MemWatch *)__pyx_v_self), ((PyObject *)__pyx_v_offset));
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_2add_offset(((struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *)__pyx_v_self), ((PyObject *)__pyx_v_offset));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8MemWatch_2add_offset(struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self, PyObject *__pyx_v_offset) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_2add_offset(struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self, PyObject *__pyx_v_offset) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_offset", 0);
@@ -1940,15 +1948,15 @@
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("_dolphin_memory_engine.MemWatch.add_offset", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.MemWatch.add_offset", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -1957,28 +1965,28 @@
  * 
  *     def get_value(self):             # <<<<<<<<<<<<<<
  *         return buffer_to_word(self.c_entry.getMemory())
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_8MemWatch_5get_value(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_8MemWatch_4get_value[] = "MemWatch.get_value(self)";
-static PyObject *__pyx_pw_22_dolphin_memory_engine_8MemWatch_5get_value(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_5get_value(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_4get_value[] = "MemWatch.get_value(self)";
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_5get_value(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_value (wrapper)", 0);
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_8MemWatch_4get_value(((struct __pyx_obj_22_dolphin_memory_engine_MemWatch *)__pyx_v_self));
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_4get_value(((struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8MemWatch_4get_value(struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_4get_value(struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_value", 0);
@@ -1987,15 +1995,15 @@
  * 
  *     def get_value(self):
  *         return buffer_to_word(self.c_entry.getMemory())             # <<<<<<<<<<<<<<
  * 
  *     def read_memory_from_ram(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_22_dolphin_memory_engine_buffer_to_word(__pyx_v_self->c_entry.getMemory()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 109, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine_buffer_to_word(__pyx_v_self->c_entry.getMemory()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* "_dolphin_memory_engine.pyx":108
  *         self.c_entry.addOffset(offset)
@@ -2004,15 +2012,15 @@
  *         return buffer_to_word(self.c_entry.getMemory())
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.MemWatch.get_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.MemWatch.get_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -2021,28 +2029,28 @@
  * 
  *     def read_memory_from_ram(self):             # <<<<<<<<<<<<<<
  *         return self.c_entry.readMemoryFromRAM() == MemOperationReturnCode.OK
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_8MemWatch_7read_memory_from_ram(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_8MemWatch_6read_memory_from_ram[] = "MemWatch.read_memory_from_ram(self)";
-static PyObject *__pyx_pw_22_dolphin_memory_engine_8MemWatch_7read_memory_from_ram(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_7read_memory_from_ram(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_6read_memory_from_ram[] = "MemWatch.read_memory_from_ram(self)";
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_7read_memory_from_ram(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_memory_from_ram (wrapper)", 0);
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_8MemWatch_6read_memory_from_ram(((struct __pyx_obj_22_dolphin_memory_engine_MemWatch *)__pyx_v_self));
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_6read_memory_from_ram(((struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8MemWatch_6read_memory_from_ram(struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_6read_memory_from_ram(struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_memory_from_ram", 0);
@@ -2068,15 +2076,15 @@
  *         return self.c_entry.readMemoryFromRAM() == MemOperationReturnCode.OK
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.MemWatch.read_memory_from_ram", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.MemWatch.read_memory_from_ram", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -2085,36 +2093,36 @@
  * 
  *     def write_memory_from_string(self, value: str):             # <<<<<<<<<<<<<<
  *         return self.c_entry.writeMemoryFromString(value.encode("utf-8")) == MemOperationReturnCode.OK
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_8MemWatch_9write_memory_from_string(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_8MemWatch_8write_memory_from_string[] = "MemWatch.write_memory_from_string(self, unicode value: str)";
-static PyObject *__pyx_pw_22_dolphin_memory_engine_8MemWatch_9write_memory_from_string(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_9write_memory_from_string(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_8write_memory_from_string[] = "MemWatch.write_memory_from_string(self, unicode value: str)";
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_9write_memory_from_string(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("write_memory_from_string (wrapper)", 0);
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_value), (&PyUnicode_Type), 1, "value", 1))) __PYX_ERR(1, 114, __pyx_L1_error)
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_8MemWatch_8write_memory_from_string(((struct __pyx_obj_22_dolphin_memory_engine_MemWatch *)__pyx_v_self), ((PyObject*)__pyx_v_value));
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_8write_memory_from_string(((struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *)__pyx_v_self), ((PyObject*)__pyx_v_value));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8MemWatch_8write_memory_from_string(struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_8write_memory_from_string(struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   std::string __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -2149,43 +2157,43 @@
  *         return self.c_entry.writeMemoryFromString(value.encode("utf-8")) == MemOperationReturnCode.OK
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.MemWatch.write_memory_from_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.MemWatch.write_memory_from_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_8MemWatch_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_8MemWatch_10__reduce_cython__[] = "MemWatch.__reduce_cython__(self)";
-static PyObject *__pyx_pw_22_dolphin_memory_engine_8MemWatch_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_10__reduce_cython__[] = "MemWatch.__reduce_cython__(self)";
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_8MemWatch_10__reduce_cython__(((struct __pyx_obj_22_dolphin_memory_engine_MemWatch *)__pyx_v_self));
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_10__reduce_cython__(((struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8MemWatch_10__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_10__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -2207,43 +2215,43 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.MemWatch.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.MemWatch.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_8MemWatch_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_8MemWatch_12__setstate_cython__[] = "MemWatch.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_22_dolphin_memory_engine_8MemWatch_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_12__setstate_cython__[] = "MemWatch.__setstate_cython__(self, __pyx_state)";
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_8MemWatch_12__setstate_cython__(((struct __pyx_obj_22_dolphin_memory_engine_MemWatch *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_12__setstate_cython__(((struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8MemWatch_12__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_22_dolphin_memory_engine_MemWatch *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_12__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -2265,15 +2273,15 @@
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.MemWatch.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.MemWatch.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "_dolphin_memory_engine.pyx":118
@@ -2281,29 +2289,29 @@
  * 
  * def hook():             # <<<<<<<<<<<<<<
  *     return DolphinAccessor.hook()
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_1hook(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_hook[] = "hook()";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_1hook = {"hook", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_1hook, METH_NOARGS, __pyx_doc_22_dolphin_memory_engine_hook};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_1hook(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_1hook(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_hook[] = "hook()";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_1hook = {"hook", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_1hook, METH_NOARGS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_hook};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_1hook(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("hook (wrapper)", 0);
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_hook(__pyx_self);
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_hook(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_hook(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_hook(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("hook", 0);
@@ -2329,15 +2337,15 @@
  *     return DolphinAccessor.hook()
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.hook", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.hook", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -2346,29 +2354,29 @@
  * 
  * def un_hook():             # <<<<<<<<<<<<<<
  *     return DolphinAccessor.unHook()
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_3un_hook(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_2un_hook[] = "un_hook()";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_3un_hook = {"un_hook", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_3un_hook, METH_NOARGS, __pyx_doc_22_dolphin_memory_engine_2un_hook};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_3un_hook(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_3un_hook(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_2un_hook[] = "un_hook()";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_3un_hook = {"un_hook", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_3un_hook, METH_NOARGS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_2un_hook};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_3un_hook(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("un_hook (wrapper)", 0);
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_2un_hook(__pyx_self);
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_2un_hook(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_2un_hook(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_2un_hook(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("un_hook", 0);
@@ -2394,15 +2402,15 @@
  *     return DolphinAccessor.unHook()
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.un_hook", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.un_hook", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -2411,29 +2419,29 @@
  * 
  * def is_hooked() -> bool:             # <<<<<<<<<<<<<<
  *     if DolphinAccessor.getStatus() == DolphinStatus.hooked:
  *         return True
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_5is_hooked(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_4is_hooked[] = "is_hooked() -> bool";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_5is_hooked = {"is_hooked", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_5is_hooked, METH_NOARGS, __pyx_doc_22_dolphin_memory_engine_4is_hooked};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_5is_hooked(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_5is_hooked(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_4is_hooked[] = "is_hooked() -> bool";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_5is_hooked = {"is_hooked", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_5is_hooked, METH_NOARGS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_4is_hooked};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_5is_hooked(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_hooked (wrapper)", 0);
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_4is_hooked(__pyx_self);
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_4is_hooked(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_4is_hooked(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_4is_hooked(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("is_hooked", 0);
 
   /* "_dolphin_memory_engine.pyx":127
  * 
@@ -2500,29 +2508,29 @@
  * 
  * def assert_hooked():             # <<<<<<<<<<<<<<
  *     if not is_hooked():
  *         raise RuntimeError("not hooked")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_7assert_hooked(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_6assert_hooked[] = "assert_hooked()";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_7assert_hooked = {"assert_hooked", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_7assert_hooked, METH_NOARGS, __pyx_doc_22_dolphin_memory_engine_6assert_hooked};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_7assert_hooked(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_7assert_hooked(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_6assert_hooked[] = "assert_hooked()";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_7assert_hooked = {"assert_hooked", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_7assert_hooked, METH_NOARGS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_6assert_hooked};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_7assert_hooked(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("assert_hooked (wrapper)", 0);
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_6assert_hooked(__pyx_self);
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_6assert_hooked(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_6assert_hooked(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_6assert_hooked(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
@@ -2593,15 +2601,15 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("_dolphin_memory_engine.assert_hooked", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.assert_hooked", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -2610,18 +2618,18 @@
  * 
  * def follow_pointers(console_address: int, pointer_offsets: List[int]) -> int:             # <<<<<<<<<<<<<<
  *     assert_hooked()
  *     real_console_address = console_address
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_9follow_pointers(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_8follow_pointers[] = "follow_pointers(console_address: int, pointer_offsets: List[int]) -> int";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_9follow_pointers = {"follow_pointers", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_22_dolphin_memory_engine_9follow_pointers, METH_VARARGS|METH_KEYWORDS, __pyx_doc_22_dolphin_memory_engine_8follow_pointers};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_9follow_pointers(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_9follow_pointers(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8follow_pointers[] = "follow_pointers(console_address: int, pointer_offsets: List[int]) -> int";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_9follow_pointers = {"follow_pointers", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_9follow_pointers, METH_VARARGS|METH_KEYWORDS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8follow_pointers};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_9follow_pointers(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_console_address = 0;
   PyObject *__pyx_v_pointer_offsets = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -2664,28 +2672,28 @@
     __pyx_v_console_address = values[0];
     __pyx_v_pointer_offsets = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("follow_pointers", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 138, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("_dolphin_memory_engine.follow_pointers", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.follow_pointers", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_8follow_pointers(__pyx_self, __pyx_v_console_address, __pyx_v_pointer_offsets);
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8follow_pointers(__pyx_self, __pyx_v_console_address, __pyx_v_pointer_offsets);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_8follow_pointers(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_pointer_offsets) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_8follow_pointers(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_pointer_offsets) {
   PyObject *__pyx_v_real_console_address = NULL;
-  uint32_t __pyx_v_mem2Distance;
+  bool __pyx_v_is_aram_accessible;
   char __pyx_v_memory_buffer[4];
   PyObject *__pyx_v_offset = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -2727,33 +2735,33 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_dolphin_memory_engine.pyx":140
  * def follow_pointers(console_address: int, pointer_offsets: List[int]) -> int:
  *     assert_hooked()
  *     real_console_address = console_address             # <<<<<<<<<<<<<<
  * 
- *     mem2Distance = DolphinAccessor.getMEM1ToMEM2Distance()
+ *     is_aram_accessible = DolphinAccessor.isARAMAccessible()
  */
   __Pyx_INCREF(__pyx_v_console_address);
   __pyx_v_real_console_address = __pyx_v_console_address;
 
   /* "_dolphin_memory_engine.pyx":142
  *     real_console_address = console_address
  * 
- *     mem2Distance = DolphinAccessor.getMEM1ToMEM2Distance()             # <<<<<<<<<<<<<<
+ *     is_aram_accessible = DolphinAccessor.isARAMAccessible()             # <<<<<<<<<<<<<<
  * 
  *     cdef char memory_buffer[4]
  */
-  __pyx_v_mem2Distance = DolphinComm::DolphinAccessor::getMEM1ToMEM2Distance();
+  __pyx_v_is_aram_accessible = DolphinComm::DolphinAccessor::isARAMAccessible();
 
   /* "_dolphin_memory_engine.pyx":145
  * 
  *     cdef char memory_buffer[4]
  *     for offset in pointer_offsets:             # <<<<<<<<<<<<<<
- *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, mem2Distance), memory_buffer, 4, True):
+ *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, is_aram_accessible), memory_buffer, 4, True):
  *             real_console_address = buffer_to_word(memory_buffer)
  */
   if (likely(PyList_CheckExact(__pyx_v_pointer_offsets)) || PyTuple_CheckExact(__pyx_v_pointer_offsets)) {
     __pyx_t_1 = __pyx_v_pointer_offsets; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
     __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_pointer_offsets); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 145, __pyx_L1_error)
@@ -2793,36 +2801,36 @@
     }
     __Pyx_XDECREF_SET(__pyx_v_offset, __pyx_t_2);
     __pyx_t_2 = 0;
 
     /* "_dolphin_memory_engine.pyx":146
  *     cdef char memory_buffer[4]
  *     for offset in pointer_offsets:
- *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, mem2Distance), memory_buffer, 4, True):             # <<<<<<<<<<<<<<
+ *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, is_aram_accessible), memory_buffer, 4, True):             # <<<<<<<<<<<<<<
  *             real_console_address = buffer_to_word(memory_buffer)
  *             if DolphinAccessor.isValidConsoleAddress(real_console_address):
  */
     __pyx_t_6 = __Pyx_PyInt_As_uint32_t(__pyx_v_real_console_address); if (unlikely((__pyx_t_6 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 146, __pyx_L1_error)
-    __pyx_t_7 = (DolphinComm::DolphinAccessor::readFromRAM(Common::dolphinAddrToOffset(__pyx_t_6, __pyx_v_mem2Distance), __pyx_v_memory_buffer, 4, 1) != 0);
+    __pyx_t_7 = (DolphinComm::DolphinAccessor::readFromRAM(Common::dolphinAddrToOffset(__pyx_t_6, __pyx_v_is_aram_accessible), __pyx_v_memory_buffer, 4, 1) != 0);
     if (likely(__pyx_t_7)) {
 
       /* "_dolphin_memory_engine.pyx":147
  *     for offset in pointer_offsets:
- *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, mem2Distance), memory_buffer, 4, True):
+ *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, is_aram_accessible), memory_buffer, 4, True):
  *             real_console_address = buffer_to_word(memory_buffer)             # <<<<<<<<<<<<<<
  *             if DolphinAccessor.isValidConsoleAddress(real_console_address):
  *                 real_console_address += offset
  */
-      __pyx_t_2 = __pyx_f_22_dolphin_memory_engine_buffer_to_word(__pyx_v_memory_buffer); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 147, __pyx_L1_error)
+      __pyx_t_2 = __pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine_buffer_to_word(__pyx_v_memory_buffer); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 147, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF_SET(__pyx_v_real_console_address, __pyx_t_2);
       __pyx_t_2 = 0;
 
       /* "_dolphin_memory_engine.pyx":148
- *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, mem2Distance), memory_buffer, 4, True):
+ *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, is_aram_accessible), memory_buffer, 4, True):
  *             real_console_address = buffer_to_word(memory_buffer)
  *             if DolphinAccessor.isValidConsoleAddress(real_console_address):             # <<<<<<<<<<<<<<
  *                 real_console_address += offset
  *             else:
  */
       __pyx_t_6 = __Pyx_PyInt_As_uint32_t(__pyx_v_real_console_address); if (unlikely((__pyx_t_6 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 148, __pyx_L1_error)
       __pyx_t_7 = (DolphinComm::DolphinAccessor::isValidConsoleAddress(__pyx_t_6) != 0);
@@ -2837,15 +2845,15 @@
  */
         __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_real_console_address, __pyx_v_offset); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 149, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF_SET(__pyx_v_real_console_address, __pyx_t_2);
         __pyx_t_2 = 0;
 
         /* "_dolphin_memory_engine.pyx":148
- *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, mem2Distance), memory_buffer, 4, True):
+ *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, is_aram_accessible), memory_buffer, 4, True):
  *             real_console_address = buffer_to_word(memory_buffer)
  *             if DolphinAccessor.isValidConsoleAddress(real_console_address):             # <<<<<<<<<<<<<<
  *                 real_console_address += offset
  *             else:
  */
         goto __pyx_L6;
       }
@@ -2888,15 +2896,15 @@
         __PYX_ERR(1, 151, __pyx_L1_error)
       }
       __pyx_L6:;
 
       /* "_dolphin_memory_engine.pyx":146
  *     cdef char memory_buffer[4]
  *     for offset in pointer_offsets:
- *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, mem2Distance), memory_buffer, 4, True):             # <<<<<<<<<<<<<<
+ *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, is_aram_accessible), memory_buffer, 4, True):             # <<<<<<<<<<<<<<
  *             real_console_address = buffer_to_word(memory_buffer)
  *             if DolphinAccessor.isValidConsoleAddress(real_console_address):
  */
       goto __pyx_L5;
     }
 
     /* "_dolphin_memory_engine.pyx":153
@@ -2921,15 +2929,15 @@
     }
     __pyx_L5:;
 
     /* "_dolphin_memory_engine.pyx":145
  * 
  *     cdef char memory_buffer[4]
  *     for offset in pointer_offsets:             # <<<<<<<<<<<<<<
- *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, mem2Distance), memory_buffer, 4, True):
+ *         if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, is_aram_accessible), memory_buffer, 4, True):
  *             real_console_address = buffer_to_word(memory_buffer)
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_dolphin_memory_engine.pyx":155
  *             raise RuntimeError(f"Could not read memory at {real_console_address}")
@@ -2952,33 +2960,33 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("_dolphin_memory_engine.follow_pointers", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.follow_pointers", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_real_console_address);
   __Pyx_XDECREF(__pyx_v_offset);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "_dolphin_memory_engine.pyx":158
  * 
  * 
  * cdef _read_memory(console_address, char* memory_buffer, int size):             # <<<<<<<<<<<<<<
  *     assert_hooked()
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):
  */
 
-static PyObject *__pyx_f_22_dolphin_memory_engine__read_memory(PyObject *__pyx_v_console_address, char *__pyx_v_memory_buffer, int __pyx_v_size) {
+static PyObject *__pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine__read_memory(PyObject *__pyx_v_console_address, char *__pyx_v_memory_buffer, int __pyx_v_size) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   uint32_t __pyx_t_4;
   int __pyx_t_5;
@@ -2987,15 +2995,15 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_read_memory", 0);
 
   /* "_dolphin_memory_engine.pyx":159
  * 
  * cdef _read_memory(console_address, char* memory_buffer, int size):
  *     assert_hooked()             # <<<<<<<<<<<<<<
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):
  *         raise RuntimeError(f"Could not read memory at {console_address}")
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_assert_hooked); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -3012,25 +3020,25 @@
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_dolphin_memory_engine.pyx":160
  * cdef _read_memory(console_address, char* memory_buffer, int size):
  *     assert_hooked()
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):             # <<<<<<<<<<<<<<
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):             # <<<<<<<<<<<<<<
  *         raise RuntimeError(f"Could not read memory at {console_address}")
  * 
  */
   __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_console_address); if (unlikely((__pyx_t_4 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 160, __pyx_L1_error)
-  __pyx_t_5 = ((!(DolphinComm::DolphinAccessor::readFromRAM(Common::dolphinAddrToOffset(__pyx_t_4, DolphinComm::DolphinAccessor::getMEM1ToMEM2Distance()), __pyx_v_memory_buffer, __pyx_v_size, 1) != 0)) != 0);
+  __pyx_t_5 = ((!(DolphinComm::DolphinAccessor::readFromRAM(Common::dolphinAddrToOffset(__pyx_t_4, DolphinComm::DolphinAccessor::isARAMAccessible()), __pyx_v_memory_buffer, __pyx_v_size, 1) != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
     /* "_dolphin_memory_engine.pyx":161
  *     assert_hooked()
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):
  *         raise RuntimeError(f"Could not read memory at {console_address}")             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_console_address, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 161, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Could_not_read_memory_at, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 161, __pyx_L1_error)
@@ -3042,36 +3050,36 @@
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(1, 161, __pyx_L1_error)
 
     /* "_dolphin_memory_engine.pyx":160
  * cdef _read_memory(console_address, char* memory_buffer, int size):
  *     assert_hooked()
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):             # <<<<<<<<<<<<<<
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):             # <<<<<<<<<<<<<<
  *         raise RuntimeError(f"Could not read memory at {console_address}")
  * 
  */
   }
 
   /* "_dolphin_memory_engine.pyx":158
  * 
  * 
  * cdef _read_memory(console_address, char* memory_buffer, int size):             # <<<<<<<<<<<<<<
  *     assert_hooked()
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("_dolphin_memory_engine._read_memory", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine._read_memory", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -3080,29 +3088,29 @@
  * 
  * def read_byte(console_address: int) -> int:             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[1]
  *     _read_memory(console_address, memory_buffer, 1)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_11read_byte(PyObject *__pyx_self, PyObject *__pyx_v_console_address); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_10read_byte[] = "read_byte(console_address: int) -> int";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_11read_byte = {"read_byte", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_11read_byte, METH_O, __pyx_doc_22_dolphin_memory_engine_10read_byte};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_11read_byte(PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_11read_byte(PyObject *__pyx_self, PyObject *__pyx_v_console_address); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_10read_byte[] = "read_byte(console_address: int) -> int";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_11read_byte = {"read_byte", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_11read_byte, METH_O, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_10read_byte};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_11read_byte(PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_byte (wrapper)", 0);
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_10read_byte(__pyx_self, ((PyObject *)__pyx_v_console_address));
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_10read_byte(__pyx_self, ((PyObject *)__pyx_v_console_address));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_10read_byte(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_10read_byte(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
   char __pyx_v_memory_buffer[1];
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -3111,15 +3119,15 @@
   /* "_dolphin_memory_engine.pyx":166
  * def read_byte(console_address: int) -> int:
  *     cdef char memory_buffer[1]
  *     _read_memory(console_address, memory_buffer, 1)             # <<<<<<<<<<<<<<
  *     return (<uint8_t*> memory_buffer)[0]
  * 
  */
-  __pyx_t_1 = __pyx_f_22_dolphin_memory_engine__read_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 166, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine__read_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_dolphin_memory_engine.pyx":167
  *     cdef char memory_buffer[1]
  *     _read_memory(console_address, memory_buffer, 1)
  *     return (<uint8_t*> memory_buffer)[0]             # <<<<<<<<<<<<<<
@@ -3140,15 +3148,15 @@
  *     cdef char memory_buffer[1]
  *     _read_memory(console_address, memory_buffer, 1)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.read_byte", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.read_byte", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -3157,29 +3165,29 @@
  * 
  * def read_word(console_address: int) -> int:             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[4]
  *     _read_memory(console_address, memory_buffer, 4)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_13read_word(PyObject *__pyx_self, PyObject *__pyx_v_console_address); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_12read_word[] = "read_word(console_address: int) -> int";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_13read_word = {"read_word", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_13read_word, METH_O, __pyx_doc_22_dolphin_memory_engine_12read_word};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_13read_word(PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_13read_word(PyObject *__pyx_self, PyObject *__pyx_v_console_address); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_12read_word[] = "read_word(console_address: int) -> int";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_13read_word = {"read_word", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_13read_word, METH_O, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_12read_word};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_13read_word(PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_word (wrapper)", 0);
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_12read_word(__pyx_self, ((PyObject *)__pyx_v_console_address));
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_12read_word(__pyx_self, ((PyObject *)__pyx_v_console_address));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_12read_word(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_12read_word(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
   char __pyx_v_memory_buffer[4];
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -3188,15 +3196,15 @@
   /* "_dolphin_memory_engine.pyx":172
  * def read_word(console_address: int) -> int:
  *     cdef char memory_buffer[4]
  *     _read_memory(console_address, memory_buffer, 4)             # <<<<<<<<<<<<<<
  *     return (<uint32_t*> memory_buffer)[0]
  * 
  */
-  __pyx_t_1 = __pyx_f_22_dolphin_memory_engine__read_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 172, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine__read_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_dolphin_memory_engine.pyx":173
  *     cdef char memory_buffer[4]
  *     _read_memory(console_address, memory_buffer, 4)
  *     return (<uint32_t*> memory_buffer)[0]             # <<<<<<<<<<<<<<
@@ -3217,15 +3225,15 @@
  *     cdef char memory_buffer[4]
  *     _read_memory(console_address, memory_buffer, 4)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.read_word", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.read_word", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -3234,29 +3242,29 @@
  * 
  * def read_float(console_address: int) -> float:             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[4]
  *     _read_memory(console_address, memory_buffer, 4)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_15read_float(PyObject *__pyx_self, PyObject *__pyx_v_console_address); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_14read_float[] = "read_float(console_address: int) -> float";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_15read_float = {"read_float", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_15read_float, METH_O, __pyx_doc_22_dolphin_memory_engine_14read_float};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_15read_float(PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_15read_float(PyObject *__pyx_self, PyObject *__pyx_v_console_address); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_14read_float[] = "read_float(console_address: int) -> float";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_15read_float = {"read_float", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_15read_float, METH_O, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_14read_float};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_15read_float(PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_float (wrapper)", 0);
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_14read_float(__pyx_self, ((PyObject *)__pyx_v_console_address));
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_14read_float(__pyx_self, ((PyObject *)__pyx_v_console_address));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_14read_float(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_14read_float(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
   char __pyx_v_memory_buffer[4];
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -3265,15 +3273,15 @@
   /* "_dolphin_memory_engine.pyx":178
  * def read_float(console_address: int) -> float:
  *     cdef char memory_buffer[4]
  *     _read_memory(console_address, memory_buffer, 4)             # <<<<<<<<<<<<<<
  *     return (<float*> memory_buffer)[0]
  * 
  */
-  __pyx_t_1 = __pyx_f_22_dolphin_memory_engine__read_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 178, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine__read_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 178, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_dolphin_memory_engine.pyx":179
  *     cdef char memory_buffer[4]
  *     _read_memory(console_address, memory_buffer, 4)
  *     return (<float*> memory_buffer)[0]             # <<<<<<<<<<<<<<
@@ -3294,15 +3302,15 @@
  *     cdef char memory_buffer[4]
  *     _read_memory(console_address, memory_buffer, 4)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.read_float", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.read_float", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -3311,29 +3319,29 @@
  * 
  * def read_double(console_address: int) -> double:             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[8]
  *     _read_memory(console_address, memory_buffer, 8)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_17read_double(PyObject *__pyx_self, PyObject *__pyx_v_console_address); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_16read_double[] = "read_double(console_address: int) -> double";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_17read_double = {"read_double", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_17read_double, METH_O, __pyx_doc_22_dolphin_memory_engine_16read_double};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_17read_double(PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_17read_double(PyObject *__pyx_self, PyObject *__pyx_v_console_address); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_16read_double[] = "read_double(console_address: int) -> double";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_17read_double = {"read_double", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_17read_double, METH_O, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_16read_double};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_17read_double(PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("read_double (wrapper)", 0);
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_16read_double(__pyx_self, ((PyObject *)__pyx_v_console_address));
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_16read_double(__pyx_self, ((PyObject *)__pyx_v_console_address));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_16read_double(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_16read_double(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address) {
   char __pyx_v_memory_buffer[8];
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -3342,15 +3350,15 @@
   /* "_dolphin_memory_engine.pyx":184
  * def read_double(console_address: int) -> double:
  *     cdef char memory_buffer[8]
  *     _read_memory(console_address, memory_buffer, 8)             # <<<<<<<<<<<<<<
  *     return (<double*> memory_buffer)[0]
  * 
  */
-  __pyx_t_1 = __pyx_f_22_dolphin_memory_engine__read_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 184, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine__read_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_dolphin_memory_engine.pyx":185
  *     cdef char memory_buffer[8]
  *     _read_memory(console_address, memory_buffer, 8)
  *     return (<double*> memory_buffer)[0]             # <<<<<<<<<<<<<<
@@ -3371,35 +3379,35 @@
  *     cdef char memory_buffer[8]
  *     _read_memory(console_address, memory_buffer, 8)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.read_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.read_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "_dolphin_memory_engine.pyx":188
  * 
  * 
  * def read_bytes(console_address: int, size: int) -> bytes:             # <<<<<<<<<<<<<<
  *     memory = bytearray(size)
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, size, False):
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, size, False):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_19read_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_18read_bytes[] = "read_bytes(console_address: int, size: int) -> bytes";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_19read_bytes = {"read_bytes", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_22_dolphin_memory_engine_19read_bytes, METH_VARARGS|METH_KEYWORDS, __pyx_doc_22_dolphin_memory_engine_18read_bytes};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_19read_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_19read_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_18read_bytes[] = "read_bytes(console_address: int, size: int) -> bytes";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_19read_bytes = {"read_bytes", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_19read_bytes, METH_VARARGS|METH_KEYWORDS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_18read_bytes};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_19read_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_console_address = 0;
   PyObject *__pyx_v_size = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -3442,26 +3450,26 @@
     __pyx_v_console_address = values[0];
     __pyx_v_size = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("read_bytes", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 188, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("_dolphin_memory_engine.read_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.read_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_18read_bytes(__pyx_self, __pyx_v_console_address, __pyx_v_size);
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_18read_bytes(__pyx_self, __pyx_v_console_address, __pyx_v_size);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_18read_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_size) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_18read_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_size) {
   PyObject *__pyx_v_memory = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   uint32_t __pyx_t_2;
   char *__pyx_t_3;
   size_t __pyx_t_4;
@@ -3472,38 +3480,38 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_bytes", 0);
 
   /* "_dolphin_memory_engine.pyx":189
  * 
  * def read_bytes(console_address: int, size: int) -> bytes:
  *     memory = bytearray(size)             # <<<<<<<<<<<<<<
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, size, False):
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, size, False):
  *         raise RuntimeError(f"Could not read memory at {console_address}")
  */
   __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyByteArray_Type)), __pyx_v_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_memory = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "_dolphin_memory_engine.pyx":190
  * def read_bytes(console_address: int, size: int) -> bytes:
  *     memory = bytearray(size)
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, size, False):             # <<<<<<<<<<<<<<
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, size, False):             # <<<<<<<<<<<<<<
  *         raise RuntimeError(f"Could not read memory at {console_address}")
  *     return bytes(memory)
  */
   __pyx_t_2 = __Pyx_PyInt_As_uint32_t(__pyx_v_console_address); if (unlikely((__pyx_t_2 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 190, __pyx_L1_error)
   __pyx_t_3 = __Pyx_PyObject_AsWritableString(__pyx_v_memory); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(1, 190, __pyx_L1_error)
   __pyx_t_4 = __Pyx_PyInt_As_size_t(__pyx_v_size); if (unlikely((__pyx_t_4 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 190, __pyx_L1_error)
-  __pyx_t_5 = ((!(DolphinComm::DolphinAccessor::readFromRAM(Common::dolphinAddrToOffset(__pyx_t_2, DolphinComm::DolphinAccessor::getMEM1ToMEM2Distance()), __pyx_t_3, __pyx_t_4, 0) != 0)) != 0);
+  __pyx_t_5 = ((!(DolphinComm::DolphinAccessor::readFromRAM(Common::dolphinAddrToOffset(__pyx_t_2, DolphinComm::DolphinAccessor::isARAMAccessible()), __pyx_t_3, __pyx_t_4, 0) != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
     /* "_dolphin_memory_engine.pyx":191
  *     memory = bytearray(size)
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, size, False):
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, size, False):
  *         raise RuntimeError(f"Could not read memory at {console_address}")             # <<<<<<<<<<<<<<
  *     return bytes(memory)
  * 
  */
     __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_console_address, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 191, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Could_not_read_memory_at, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 191, __pyx_L1_error)
@@ -3515,22 +3523,22 @@
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(1, 191, __pyx_L1_error)
 
     /* "_dolphin_memory_engine.pyx":190
  * def read_bytes(console_address: int, size: int) -> bytes:
  *     memory = bytearray(size)
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, size, False):             # <<<<<<<<<<<<<<
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, size, False):             # <<<<<<<<<<<<<<
  *         raise RuntimeError(f"Could not read memory at {console_address}")
  *     return bytes(memory)
  */
   }
 
   /* "_dolphin_memory_engine.pyx":192
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, size, False):
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, size, False):
  *         raise RuntimeError(f"Could not read memory at {console_address}")
  *     return bytes(memory)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_memory); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 192, __pyx_L1_error)
@@ -3540,39 +3548,39 @@
   goto __pyx_L0;
 
   /* "_dolphin_memory_engine.pyx":188
  * 
  * 
  * def read_bytes(console_address: int, size: int) -> bytes:             # <<<<<<<<<<<<<<
  *     memory = bytearray(size)
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, size, False):
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, size, False):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("_dolphin_memory_engine.read_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.read_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_memory);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "_dolphin_memory_engine.pyx":195
  * 
  * 
  * cdef _write_memory(console_address, char* memory_buffer, int size):             # <<<<<<<<<<<<<<
  *     assert_hooked()
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):
  */
 
-static PyObject *__pyx_f_22_dolphin_memory_engine__write_memory(PyObject *__pyx_v_console_address, char *__pyx_v_memory_buffer, int __pyx_v_size) {
+static PyObject *__pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine__write_memory(PyObject *__pyx_v_console_address, char *__pyx_v_memory_buffer, int __pyx_v_size) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   uint32_t __pyx_t_4;
   int __pyx_t_5;
@@ -3581,15 +3589,15 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_write_memory", 0);
 
   /* "_dolphin_memory_engine.pyx":196
  * 
  * cdef _write_memory(console_address, char* memory_buffer, int size):
  *     assert_hooked()             # <<<<<<<<<<<<<<
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):
  *         raise RuntimeError(f"Could not write memory at {console_address}")
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_assert_hooked); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -3606,25 +3614,25 @@
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_dolphin_memory_engine.pyx":197
  * cdef _write_memory(console_address, char* memory_buffer, int size):
  *     assert_hooked()
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):             # <<<<<<<<<<<<<<
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):             # <<<<<<<<<<<<<<
  *         raise RuntimeError(f"Could not write memory at {console_address}")
  * 
  */
   __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_console_address); if (unlikely((__pyx_t_4 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 197, __pyx_L1_error)
-  __pyx_t_5 = ((!(DolphinComm::DolphinAccessor::writeToRAM(Common::dolphinAddrToOffset(__pyx_t_4, DolphinComm::DolphinAccessor::getMEM1ToMEM2Distance()), __pyx_v_memory_buffer, __pyx_v_size, 1) != 0)) != 0);
+  __pyx_t_5 = ((!(DolphinComm::DolphinAccessor::writeToRAM(Common::dolphinAddrToOffset(__pyx_t_4, DolphinComm::DolphinAccessor::isARAMAccessible()), __pyx_v_memory_buffer, __pyx_v_size, 1) != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
     /* "_dolphin_memory_engine.pyx":198
  *     assert_hooked()
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):
  *         raise RuntimeError(f"Could not write memory at {console_address}")             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_console_address, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 198, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Could_not_write_memory_at, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 198, __pyx_L1_error)
@@ -3636,36 +3644,36 @@
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(1, 198, __pyx_L1_error)
 
     /* "_dolphin_memory_engine.pyx":197
  * cdef _write_memory(console_address, char* memory_buffer, int size):
  *     assert_hooked()
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):             # <<<<<<<<<<<<<<
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):             # <<<<<<<<<<<<<<
  *         raise RuntimeError(f"Could not write memory at {console_address}")
  * 
  */
   }
 
   /* "_dolphin_memory_engine.pyx":195
  * 
  * 
  * cdef _write_memory(console_address, char* memory_buffer, int size):             # <<<<<<<<<<<<<<
  *     assert_hooked()
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("_dolphin_memory_engine._write_memory", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine._write_memory", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -3674,18 +3682,18 @@
  * 
  * def write_byte(console_address: int, value: int):             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[1]
  *     (<uint8_t*> memory_buffer)[0] = value
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_21write_byte(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_20write_byte[] = "write_byte(console_address: int, value: int)";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_21write_byte = {"write_byte", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_22_dolphin_memory_engine_21write_byte, METH_VARARGS|METH_KEYWORDS, __pyx_doc_22_dolphin_memory_engine_20write_byte};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_21write_byte(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_21write_byte(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_20write_byte[] = "write_byte(console_address: int, value: int)";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_21write_byte = {"write_byte", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_21write_byte, METH_VARARGS|METH_KEYWORDS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_20write_byte};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_21write_byte(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_console_address = 0;
   PyObject *__pyx_v_value = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -3728,26 +3736,26 @@
     __pyx_v_console_address = values[0];
     __pyx_v_value = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("write_byte", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 201, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("_dolphin_memory_engine.write_byte", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.write_byte", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_20write_byte(__pyx_self, __pyx_v_console_address, __pyx_v_value);
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_20write_byte(__pyx_self, __pyx_v_console_address, __pyx_v_value);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_20write_byte(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_20write_byte(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_value) {
   char __pyx_v_memory_buffer[1];
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   uint8_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -3767,15 +3775,15 @@
   /* "_dolphin_memory_engine.pyx":204
  *     cdef char memory_buffer[1]
  *     (<uint8_t*> memory_buffer)[0] = value
  *     _write_memory(console_address, memory_buffer, 1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __pyx_f_22_dolphin_memory_engine__write_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 204, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine__write_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":201
  * 
  * 
  * def write_byte(console_address: int, value: int):             # <<<<<<<<<<<<<<
@@ -3784,15 +3792,15 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("_dolphin_memory_engine.write_byte", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.write_byte", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -3801,18 +3809,18 @@
  * 
  * def write_word(console_address: int, value: int):             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[4]
  *     (<uint32_t*> memory_buffer)[0] = value
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_23write_word(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_22write_word[] = "write_word(console_address: int, value: int)";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_23write_word = {"write_word", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_22_dolphin_memory_engine_23write_word, METH_VARARGS|METH_KEYWORDS, __pyx_doc_22_dolphin_memory_engine_22write_word};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_23write_word(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_23write_word(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_22write_word[] = "write_word(console_address: int, value: int)";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_23write_word = {"write_word", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_23write_word, METH_VARARGS|METH_KEYWORDS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_22write_word};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_23write_word(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_console_address = 0;
   PyObject *__pyx_v_value = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -3855,26 +3863,26 @@
     __pyx_v_console_address = values[0];
     __pyx_v_value = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("write_word", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 207, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("_dolphin_memory_engine.write_word", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.write_word", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_22write_word(__pyx_self, __pyx_v_console_address, __pyx_v_value);
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_22write_word(__pyx_self, __pyx_v_console_address, __pyx_v_value);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_22write_word(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_22write_word(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_value) {
   char __pyx_v_memory_buffer[4];
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   uint32_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -3894,15 +3902,15 @@
   /* "_dolphin_memory_engine.pyx":210
  *     cdef char memory_buffer[4]
  *     (<uint32_t*> memory_buffer)[0] = value
  *     _write_memory(console_address, memory_buffer, 4)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __pyx_f_22_dolphin_memory_engine__write_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 4); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 210, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine__write_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 4); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":207
  * 
  * 
  * def write_word(console_address: int, value: int):             # <<<<<<<<<<<<<<
@@ -3911,15 +3919,15 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("_dolphin_memory_engine.write_word", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.write_word", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -3928,18 +3936,18 @@
  * 
  * def write_float(console_address: int, value: float):             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[4]
  *     (<float*> memory_buffer)[0] = value
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_25write_float(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_24write_float[] = "write_float(console_address: int, double value: float)";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_25write_float = {"write_float", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_22_dolphin_memory_engine_25write_float, METH_VARARGS|METH_KEYWORDS, __pyx_doc_22_dolphin_memory_engine_24write_float};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_25write_float(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_25write_float(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_24write_float[] = "write_float(console_address: int, double value: float)";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_25write_float = {"write_float", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_25write_float, METH_VARARGS|METH_KEYWORDS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_24write_float};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_25write_float(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_console_address = 0;
   double __pyx_v_value;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -3982,26 +3990,26 @@
     __pyx_v_console_address = values[0];
     __pyx_v_value = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_value == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 213, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("write_float", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 213, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("_dolphin_memory_engine.write_float", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.write_float", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_24write_float(__pyx_self, __pyx_v_console_address, __pyx_v_value);
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_24write_float(__pyx_self, __pyx_v_console_address, __pyx_v_value);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_24write_float(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, double __pyx_v_value) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_24write_float(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, double __pyx_v_value) {
   char __pyx_v_memory_buffer[4];
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -4019,15 +4027,15 @@
   /* "_dolphin_memory_engine.pyx":216
  *     cdef char memory_buffer[4]
  *     (<float*> memory_buffer)[0] = value
  *     _write_memory(console_address, memory_buffer, 4)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __pyx_f_22_dolphin_memory_engine__write_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 216, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine__write_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_dolphin_memory_engine.pyx":213
  * 
  * 
  * def write_float(console_address: int, value: float):             # <<<<<<<<<<<<<<
@@ -4036,15 +4044,15 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.write_float", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.write_float", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -4053,18 +4061,18 @@
  * 
  * def write_double(console_address: int, value: double):             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[8]
  *     (<double*> memory_buffer)[0] = value
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_27write_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_26write_double[] = "write_double(console_address: int, double value: double)";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_27write_double = {"write_double", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_22_dolphin_memory_engine_27write_double, METH_VARARGS|METH_KEYWORDS, __pyx_doc_22_dolphin_memory_engine_26write_double};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_27write_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_27write_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_26write_double[] = "write_double(console_address: int, double value: double)";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_27write_double = {"write_double", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_27write_double, METH_VARARGS|METH_KEYWORDS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_26write_double};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_27write_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_console_address = 0;
   double __pyx_v_value;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -4107,26 +4115,26 @@
     __pyx_v_console_address = values[0];
     __pyx_v_value = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_value == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 219, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("write_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 219, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("_dolphin_memory_engine.write_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.write_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_26write_double(__pyx_self, __pyx_v_console_address, __pyx_v_value);
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_26write_double(__pyx_self, __pyx_v_console_address, __pyx_v_value);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_26write_double(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, double __pyx_v_value) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_26write_double(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, double __pyx_v_value) {
   char __pyx_v_memory_buffer[8];
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -4144,15 +4152,15 @@
   /* "_dolphin_memory_engine.pyx":222
  *     cdef char memory_buffer[8]
  *     (<double*> memory_buffer)[0] = value
  *     _write_memory(console_address, memory_buffer, 8)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __pyx_f_22_dolphin_memory_engine__write_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_21dolphin_memory_engine_22_dolphin_memory_engine__write_memory(__pyx_v_console_address, __pyx_v_memory_buffer, 8); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_dolphin_memory_engine.pyx":219
  * 
  * 
  * def write_double(console_address: int, value: double):             # <<<<<<<<<<<<<<
@@ -4161,35 +4169,35 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("_dolphin_memory_engine.write_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.write_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "_dolphin_memory_engine.pyx":225
  * 
  * 
  * def write_bytes(console_address: int, memory: bytes):             # <<<<<<<<<<<<<<
  *     assert_hooked()
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, len(memory), False):
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, len(memory), False):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_22_dolphin_memory_engine_29write_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_22_dolphin_memory_engine_28write_bytes[] = "write_bytes(console_address: int, bytes memory: bytes)";
-static PyMethodDef __pyx_mdef_22_dolphin_memory_engine_29write_bytes = {"write_bytes", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_22_dolphin_memory_engine_29write_bytes, METH_VARARGS|METH_KEYWORDS, __pyx_doc_22_dolphin_memory_engine_28write_bytes};
-static PyObject *__pyx_pw_22_dolphin_memory_engine_29write_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_29write_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_28write_bytes[] = "write_bytes(console_address: int, bytes memory: bytes)";
+static PyMethodDef __pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_29write_bytes = {"write_bytes", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_29write_bytes, METH_VARARGS|METH_KEYWORDS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_28write_bytes};
+static PyObject *__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_29write_bytes(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_console_address = 0;
   PyObject *__pyx_v_memory = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -4232,31 +4240,31 @@
     __pyx_v_console_address = values[0];
     __pyx_v_memory = ((PyObject*)values[1]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("write_bytes", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 225, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("_dolphin_memory_engine.write_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.write_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_memory), (&PyBytes_Type), 1, "memory", 1))) __PYX_ERR(1, 225, __pyx_L1_error)
-  __pyx_r = __pyx_pf_22_dolphin_memory_engine_28write_bytes(__pyx_self, __pyx_v_console_address, __pyx_v_memory);
+  __pyx_r = __pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_28write_bytes(__pyx_self, __pyx_v_console_address, __pyx_v_memory);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_22_dolphin_memory_engine_28write_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_memory) {
+static PyObject *__pyx_pf_21dolphin_memory_engine_22_dolphin_memory_engine_28write_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_console_address, PyObject *__pyx_v_memory) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   uint32_t __pyx_t_4;
   char const *__pyx_t_5;
@@ -4267,15 +4275,15 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("write_bytes", 0);
 
   /* "_dolphin_memory_engine.pyx":226
  * 
  * def write_bytes(console_address: int, memory: bytes):
  *     assert_hooked()             # <<<<<<<<<<<<<<
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, len(memory), False):
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, len(memory), False):
  *         raise RuntimeError(f"Could not write memory at {console_address}")
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_assert_hooked); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -4292,34 +4300,34 @@
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "_dolphin_memory_engine.pyx":227
  * def write_bytes(console_address: int, memory: bytes):
  *     assert_hooked()
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, len(memory), False):             # <<<<<<<<<<<<<<
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, len(memory), False):             # <<<<<<<<<<<<<<
  *         raise RuntimeError(f"Could not write memory at {console_address}")
  */
   __pyx_t_4 = __Pyx_PyInt_As_uint32_t(__pyx_v_console_address); if (unlikely((__pyx_t_4 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 227, __pyx_L1_error)
   if (unlikely(__pyx_v_memory == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
     __PYX_ERR(1, 227, __pyx_L1_error)
   }
   __pyx_t_5 = __Pyx_PyBytes_AsString(__pyx_v_memory); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(1, 227, __pyx_L1_error)
   if (unlikely(__pyx_v_memory == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(1, 227, __pyx_L1_error)
   }
   __pyx_t_6 = PyBytes_GET_SIZE(__pyx_v_memory); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(1, 227, __pyx_L1_error)
-  __pyx_t_7 = ((!(DolphinComm::DolphinAccessor::writeToRAM(Common::dolphinAddrToOffset(__pyx_t_4, DolphinComm::DolphinAccessor::getMEM1ToMEM2Distance()), __pyx_t_5, __pyx_t_6, 0) != 0)) != 0);
+  __pyx_t_7 = ((!(DolphinComm::DolphinAccessor::writeToRAM(Common::dolphinAddrToOffset(__pyx_t_4, DolphinComm::DolphinAccessor::isARAMAccessible()), __pyx_t_5, __pyx_t_6, 0) != 0)) != 0);
   if (unlikely(__pyx_t_7)) {
 
     /* "_dolphin_memory_engine.pyx":228
  *     assert_hooked()
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, len(memory), False):
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, len(memory), False):
  *         raise RuntimeError(f"Could not write memory at {console_address}")             # <<<<<<<<<<<<<<
  */
     __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_console_address, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 228, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_Could_not_write_memory_at, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 228, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -4329,35 +4337,35 @@
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(1, 228, __pyx_L1_error)
 
     /* "_dolphin_memory_engine.pyx":227
  * def write_bytes(console_address: int, memory: bytes):
  *     assert_hooked()
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, len(memory), False):             # <<<<<<<<<<<<<<
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, len(memory), False):             # <<<<<<<<<<<<<<
  *         raise RuntimeError(f"Could not write memory at {console_address}")
  */
   }
 
   /* "_dolphin_memory_engine.pyx":225
  * 
  * 
  * def write_bytes(console_address: int, memory: bytes):             # <<<<<<<<<<<<<<
  *     assert_hooked()
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, len(memory), False):
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, len(memory), False):
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("_dolphin_memory_engine.write_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dolphin_memory_engine._dolphin_memory_engine.write_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -4422,59 +4430,59 @@
   __Pyx_AddTraceback("string.from_py.__pyx_convert_string_from_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_tp_new_22_dolphin_memory_engine_MemWatch(PyTypeObject *t, PyObject *a, PyObject *k) {
-  struct __pyx_obj_22_dolphin_memory_engine_MemWatch *p;
+static PyObject *__pyx_tp_new_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch(PyTypeObject *t, PyObject *a, PyObject *k) {
+  struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_22_dolphin_memory_engine_MemWatch *)o);
+  p = ((struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *)o);
   new((void*)&(p->c_entry)) MemWatchEntry();
-  if (unlikely(__pyx_pw_22_dolphin_memory_engine_8MemWatch_1__cinit__(o, a, k) < 0)) goto bad;
+  if (unlikely(__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_1__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
-static void __pyx_tp_dealloc_22_dolphin_memory_engine_MemWatch(PyObject *o) {
-  struct __pyx_obj_22_dolphin_memory_engine_MemWatch *p = (struct __pyx_obj_22_dolphin_memory_engine_MemWatch *)o;
+static void __pyx_tp_dealloc_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch(PyObject *o) {
+  struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *p = (struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   __Pyx_call_destructor(p->c_entry);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static PyMethodDef __pyx_methods_22_dolphin_memory_engine_MemWatch[] = {
-  {"add_offset", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_8MemWatch_3add_offset, METH_O, __pyx_doc_22_dolphin_memory_engine_8MemWatch_2add_offset},
-  {"get_value", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_8MemWatch_5get_value, METH_NOARGS, __pyx_doc_22_dolphin_memory_engine_8MemWatch_4get_value},
-  {"read_memory_from_ram", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_8MemWatch_7read_memory_from_ram, METH_NOARGS, __pyx_doc_22_dolphin_memory_engine_8MemWatch_6read_memory_from_ram},
-  {"write_memory_from_string", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_8MemWatch_9write_memory_from_string, METH_O, __pyx_doc_22_dolphin_memory_engine_8MemWatch_8write_memory_from_string},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_8MemWatch_11__reduce_cython__, METH_NOARGS, __pyx_doc_22_dolphin_memory_engine_8MemWatch_10__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_22_dolphin_memory_engine_8MemWatch_13__setstate_cython__, METH_O, __pyx_doc_22_dolphin_memory_engine_8MemWatch_12__setstate_cython__},
+static PyMethodDef __pyx_methods_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch[] = {
+  {"add_offset", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_3add_offset, METH_O, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_2add_offset},
+  {"get_value", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_5get_value, METH_NOARGS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_4get_value},
+  {"read_memory_from_ram", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_7read_memory_from_ram, METH_NOARGS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_6read_memory_from_ram},
+  {"write_memory_from_string", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_9write_memory_from_string, METH_O, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_8write_memory_from_string},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_11__reduce_cython__, METH_NOARGS, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_10__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_13__setstate_cython__, METH_O, __pyx_doc_21dolphin_memory_engine_22_dolphin_memory_engine_8MemWatch_12__setstate_cython__},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_22_dolphin_memory_engine_MemWatch = {
+static PyTypeObject __pyx_type_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch = {
   PyVarObject_HEAD_INIT(0, 0)
-  "_dolphin_memory_engine.MemWatch", /*tp_name*/
-  sizeof(struct __pyx_obj_22_dolphin_memory_engine_MemWatch), /*tp_basicsize*/
+  "dolphin_memory_engine._dolphin_memory_engine.MemWatch", /*tp_name*/
+  sizeof(struct __pyx_obj_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_22_dolphin_memory_engine_MemWatch, /*tp_dealloc*/
+  __pyx_tp_dealloc_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -4499,25 +4507,25 @@
   0, /*tp_doc*/
   0, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_22_dolphin_memory_engine_MemWatch, /*tp_methods*/
+  __pyx_methods_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_22_dolphin_memory_engine_MemWatch, /*tp_new*/
+  __pyx_tp_new_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
@@ -4528,15 +4536,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -4589,26 +4597,26 @@
   {&__pyx_n_s_List, __pyx_k_List, sizeof(__pyx_k_List), 0, 0, 1, 1},
   {&__pyx_n_s_MemWatch, __pyx_k_MemWatch, sizeof(__pyx_k_MemWatch), 0, 0, 1, 1},
   {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_assert_hooked, __pyx_k_assert_hooked, sizeof(__pyx_k_assert_hooked), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_console_address, __pyx_k_console_address, sizeof(__pyx_k_console_address), 0, 0, 1, 1},
-  {&__pyx_n_s_dolphin_memory_engine, __pyx_k_dolphin_memory_engine, sizeof(__pyx_k_dolphin_memory_engine), 0, 0, 1, 1},
+  {&__pyx_n_s_dolphin_memory_engine__dolphin_m, __pyx_k_dolphin_memory_engine__dolphin_m, sizeof(__pyx_k_dolphin_memory_engine__dolphin_m), 0, 0, 1, 1},
   {&__pyx_kp_s_dolphin_memory_engine_pyx, __pyx_k_dolphin_memory_engine_pyx, sizeof(__pyx_k_dolphin_memory_engine_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_follow_pointers, __pyx_k_follow_pointers, sizeof(__pyx_k_follow_pointers), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_hook, __pyx_k_hook, sizeof(__pyx_k_hook), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+  {&__pyx_n_s_is_aram_accessible, __pyx_k_is_aram_accessible, sizeof(__pyx_k_is_aram_accessible), 0, 0, 1, 1},
   {&__pyx_n_s_is_hooked, __pyx_k_is_hooked, sizeof(__pyx_k_is_hooked), 0, 0, 1, 1},
   {&__pyx_kp_u_is_not_valid, __pyx_k_is_not_valid, sizeof(__pyx_k_is_not_valid), 0, 1, 0, 0},
   {&__pyx_n_s_is_pointer, __pyx_k_is_pointer, sizeof(__pyx_k_is_pointer), 0, 0, 1, 1},
   {&__pyx_n_s_label, __pyx_k_label, sizeof(__pyx_k_label), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_mem2Distance, __pyx_k_mem2Distance, sizeof(__pyx_k_mem2Distance), 0, 0, 1, 1},
   {&__pyx_n_s_memory, __pyx_k_memory, sizeof(__pyx_k_memory), 0, 0, 1, 1},
   {&__pyx_n_s_memory_buffer, __pyx_k_memory_buffer, sizeof(__pyx_k_memory_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_kp_u_not_hooked, __pyx_k_not_hooked, sizeof(__pyx_k_not_hooked), 0, 1, 0, 0},
   {&__pyx_n_s_offset, __pyx_k_offset, sizeof(__pyx_k_offset), 0, 0, 1, 1},
   {&__pyx_n_s_pointer_offsets, __pyx_k_pointer_offsets, sizeof(__pyx_k_pointer_offsets), 0, 0, 1, 1},
@@ -4716,15 +4724,15 @@
   /* "_dolphin_memory_engine.pyx":138
  * 
  * 
  * def follow_pointers(console_address: int, pointer_offsets: List[int]) -> int:             # <<<<<<<<<<<<<<
  *     assert_hooked()
  *     real_console_address = console_address
  */
-  __pyx_tuple__8 = PyTuple_Pack(6, __pyx_n_s_console_address, __pyx_n_s_pointer_offsets, __pyx_n_s_real_console_address, __pyx_n_s_mem2Distance, __pyx_n_s_memory_buffer, __pyx_n_s_offset); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 138, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(6, __pyx_n_s_console_address, __pyx_n_s_pointer_offsets, __pyx_n_s_real_console_address, __pyx_n_s_is_aram_accessible, __pyx_n_s_memory_buffer, __pyx_n_s_offset); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
   __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dolphin_memory_engine_pyx, __pyx_n_s_follow_pointers, 138, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 138, __pyx_L1_error)
 
   /* "_dolphin_memory_engine.pyx":164
  * 
  * 
@@ -4774,15 +4782,15 @@
   __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dolphin_memory_engine_pyx, __pyx_n_s_read_double, 182, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(1, 182, __pyx_L1_error)
 
   /* "_dolphin_memory_engine.pyx":188
  * 
  * 
  * def read_bytes(console_address: int, size: int) -> bytes:             # <<<<<<<<<<<<<<
  *     memory = bytearray(size)
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, size, False):
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, size, False):
  */
   __pyx_tuple__18 = PyTuple_Pack(3, __pyx_n_s_console_address, __pyx_n_s_size, __pyx_n_s_memory); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
   __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dolphin_memory_engine_pyx, __pyx_n_s_read_bytes, 188, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 188, __pyx_L1_error)
 
   /* "_dolphin_memory_engine.pyx":201
@@ -4834,29 +4842,29 @@
   __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dolphin_memory_engine_pyx, __pyx_n_s_write_double, 219, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(1, 219, __pyx_L1_error)
 
   /* "_dolphin_memory_engine.pyx":225
  * 
  * 
  * def write_bytes(console_address: int, memory: bytes):             # <<<<<<<<<<<<<<
  *     assert_hooked()
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, len(memory), False):
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, len(memory), False):
  */
   __pyx_tuple__28 = PyTuple_Pack(2, __pyx_n_s_console_address, __pyx_n_s_memory); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
   __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_dolphin_memory_engine_pyx, __pyx_n_s_write_bytes, 225, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -4893,24 +4901,24 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_22_dolphin_memory_engine_MemWatch) < 0) __PYX_ERR(1, 99, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch) < 0) __PYX_ERR(1, 99, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_22_dolphin_memory_engine_MemWatch.tp_print = 0;
+  __pyx_type_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_22_dolphin_memory_engine_MemWatch.tp_dictoffset && __pyx_type_22_dolphin_memory_engine_MemWatch.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_22_dolphin_memory_engine_MemWatch.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch.tp_dictoffset && __pyx_type_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MemWatch, (PyObject *)&__pyx_type_22_dolphin_memory_engine_MemWatch) < 0) __PYX_ERR(1, 99, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_22_dolphin_memory_engine_MemWatch) < 0) __PYX_ERR(1, 99, __pyx_L1_error)
-  __pyx_ptype_22_dolphin_memory_engine_MemWatch = &__pyx_type_22_dolphin_memory_engine_MemWatch;
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MemWatch, (PyObject *)&__pyx_type_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch) < 0) __PYX_ERR(1, 99, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch) < 0) __PYX_ERR(1, 99, __pyx_L1_error)
+  __pyx_ptype_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch = &__pyx_type_21dolphin_memory_engine_22_dolphin_memory_engine_MemWatch;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -5101,28 +5109,28 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(1, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main__dolphin_memory_engine) {
+  if (__pyx_module_is_main_dolphin_memory_engine___dolphin_memory_engine) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(1, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "_dolphin_memory_engine")) {
-      if (unlikely(PyDict_SetItemString(modules, "_dolphin_memory_engine", __pyx_m) < 0)) __PYX_ERR(1, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "dolphin_memory_engine._dolphin_memory_engine")) {
+      if (unlikely(PyDict_SetItemString(modules, "dolphin_memory_engine._dolphin_memory_engine", __pyx_m) < 0)) __PYX_ERR(1, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -5161,183 +5169,183 @@
   /* "_dolphin_memory_engine.pyx":118
  * 
  * 
  * def hook():             # <<<<<<<<<<<<<<
  *     return DolphinAccessor.hook()
  * 
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_1hook, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 118, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_1hook, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_hook, __pyx_t_2) < 0) __PYX_ERR(1, 118, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":122
  * 
  * 
  * def un_hook():             # <<<<<<<<<<<<<<
  *     return DolphinAccessor.unHook()
  * 
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_3un_hook, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 122, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_3un_hook, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_un_hook, __pyx_t_2) < 0) __PYX_ERR(1, 122, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":126
  * 
  * 
  * def is_hooked() -> bool:             # <<<<<<<<<<<<<<
  *     if DolphinAccessor.getStatus() == DolphinStatus.hooked:
  *         return True
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_5is_hooked, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 126, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_5is_hooked, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_is_hooked, __pyx_t_2) < 0) __PYX_ERR(1, 126, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":133
  * 
  * 
  * def assert_hooked():             # <<<<<<<<<<<<<<
  *     if not is_hooked():
  *         raise RuntimeError("not hooked")
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_7assert_hooked, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 133, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_7assert_hooked, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_assert_hooked, __pyx_t_2) < 0) __PYX_ERR(1, 133, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":138
  * 
  * 
  * def follow_pointers(console_address: int, pointer_offsets: List[int]) -> int:             # <<<<<<<<<<<<<<
  *     assert_hooked()
  *     real_console_address = console_address
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_9follow_pointers, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 138, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_9follow_pointers, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_follow_pointers, __pyx_t_2) < 0) __PYX_ERR(1, 138, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":164
  * 
  * 
  * def read_byte(console_address: int) -> int:             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[1]
  *     _read_memory(console_address, memory_buffer, 1)
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_11read_byte, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 164, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_11read_byte, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_byte, __pyx_t_2) < 0) __PYX_ERR(1, 164, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":170
  * 
  * 
  * def read_word(console_address: int) -> int:             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[4]
  *     _read_memory(console_address, memory_buffer, 4)
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_13read_word, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 170, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_13read_word, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_word, __pyx_t_2) < 0) __PYX_ERR(1, 170, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":176
  * 
  * 
  * def read_float(console_address: int) -> float:             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[4]
  *     _read_memory(console_address, memory_buffer, 4)
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_15read_float, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 176, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_15read_float, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_float, __pyx_t_2) < 0) __PYX_ERR(1, 176, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":182
  * 
  * 
  * def read_double(console_address: int) -> double:             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[8]
  *     _read_memory(console_address, memory_buffer, 8)
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_17read_double, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 182, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_17read_double, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_double, __pyx_t_2) < 0) __PYX_ERR(1, 182, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":188
  * 
  * 
  * def read_bytes(console_address: int, size: int) -> bytes:             # <<<<<<<<<<<<<<
  *     memory = bytearray(size)
- *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, size, False):
+ *     if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, size, False):
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_19read_bytes, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 188, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_19read_bytes, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_bytes, __pyx_t_2) < 0) __PYX_ERR(1, 188, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":201
  * 
  * 
  * def write_byte(console_address: int, value: int):             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[1]
  *     (<uint8_t*> memory_buffer)[0] = value
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_21write_byte, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 201, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_21write_byte, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_write_byte, __pyx_t_2) < 0) __PYX_ERR(1, 201, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":207
  * 
  * 
  * def write_word(console_address: int, value: int):             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[4]
  *     (<uint32_t*> memory_buffer)[0] = value
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_23write_word, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 207, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_23write_word, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 207, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_write_word, __pyx_t_2) < 0) __PYX_ERR(1, 207, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":213
  * 
  * 
  * def write_float(console_address: int, value: float):             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[4]
  *     (<float*> memory_buffer)[0] = value
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_25write_float, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 213, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_25write_float, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 213, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_write_float, __pyx_t_2) < 0) __PYX_ERR(1, 213, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":219
  * 
  * 
  * def write_double(console_address: int, value: double):             # <<<<<<<<<<<<<<
  *     cdef char memory_buffer[8]
  *     (<double*> memory_buffer)[0] = value
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_27write_double, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 219, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_27write_double, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_write_double, __pyx_t_2) < 0) __PYX_ERR(1, 219, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":225
  * 
  * 
  * def write_bytes(console_address: int, memory: bytes):             # <<<<<<<<<<<<<<
  *     assert_hooked()
- *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, len(memory), False):
+ *     if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, len(memory), False):
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_22_dolphin_memory_engine_29write_bytes, NULL, __pyx_n_s_dolphin_memory_engine); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_21dolphin_memory_engine_22_dolphin_memory_engine_29write_bytes, NULL, __pyx_n_s_dolphin_memory_engine__dolphin_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_write_bytes, __pyx_t_2) < 0) __PYX_ERR(1, 225, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "_dolphin_memory_engine.pyx":1
  * from typing import List             # <<<<<<<<<<<<<<
  * 
@@ -5360,19 +5368,19 @@
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init _dolphin_memory_engine", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init dolphin_memory_engine._dolphin_memory_engine", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init _dolphin_memory_engine");
+    PyErr_SetString(PyExc_ImportError, "init dolphin_memory_engine._dolphin_memory_engine");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -5767,28 +5775,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -5997,15 +6005,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -6418,15 +6426,15 @@
         #endif
     }
     return value;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -6765,15 +6773,15 @@
                         } else if (8 * sizeof(uint32_t) >= 4 * PyLong_SHIFT) {
                             return (uint32_t) (((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -6961,15 +6969,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -7195,15 +7203,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -7391,15 +7399,15 @@
                         } else if (8 * sizeof(uint8_t) >= 4 * PyLong_SHIFT) {
                             return (uint8_t) (((((((((uint8_t)digits[3]) << PyLong_SHIFT) | (uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -7625,15 +7633,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `dolphin-memory-engine-1.1.2/_dolphin_memory_engine.pyx` & `dolphin-memory-engine-1.1.3/_dolphin_memory_engine.pyx`

 * *Files 20% similar despite different names*

```diff
@@ -1,228 +1,228 @@
-from typing import List
-
-from libc.stdint cimport uint8_t, uint32_t, uint64_t
-from libcpp cimport bool as c_bool
-from libcpp.string cimport string
-
-
-cdef extern from "Common/MemoryCommon.h" namespace "Common::MemType":
-    cdef enum MemType:
-        type_word
-
-
-cdef extern from "Common/MemoryCommon.h" namespace "Common::MemBase":
-    cdef enum MemBase:
-        base_decimal
-
-
-cdef extern from "Common/MemoryCommon.h" namespace "Common::MemOperationReturnCode":
-    cdef enum MemOperationReturnCode:
-        invalidInput
-        operationFailed
-        inputTooLong
-        invalidPointer
-        OK
-
-cdef extern from "Common/CommonUtils.h" namespace "Common":
-    uint32_t dolphinAddrToOffset(uint32_t, uint32_t)
-    uint32_t offsetToDolphinAddr(uint32_t, uint32_t)
-
-
-cdef extern from "DolphinProcess/DolphinAccessor.h" namespace "DolphinComm::DolphinStatus":
-    cdef enum DolphinStatus:
-        hooked
-        notRunning
-        noEmu
-        unHooked
-
-
-cdef extern from "DolphinProcess/DolphinAccessor.h" namespace "DolphinComm":
-    cdef cppclass DolphinAccessor:
-        @staticmethod
-        void init()
-
-        @staticmethod
-        void free()
-
-        @staticmethod
-        void hook()
-
-        @staticmethod
-        void unHook()
-
-        @staticmethod
-        c_bool readFromRAM(uint32_t, char*, const size_t, c_bool)
-        
-        @staticmethod
-        c_bool writeToRAM(uint32_t, const char*, const size_t, c_bool)
-
-        @staticmethod
-        int getPID()
-        
-        @staticmethod
-        DolphinStatus getStatus()
-
-        @staticmethod
-        c_bool isValidConsoleAddress(uint32_t)
-
-        @staticmethod
-        uint32_t getMEM1ToMEM2Distance()
-
-
-cdef extern from "MemoryWatch/MemWatchEntry.h":
-    cdef cppclass MemWatchEntry:
-        MemWatchEntry()
-        MemWatchEntry(string, uint32_t, MemType, MemBase, c_bool, size_t, c_bool)
-
-        char* getMemory()
-
-        void addOffset(int)
-        MemOperationReturnCode readMemoryFromRAM()
-        MemOperationReturnCode writeMemoryFromString(string)
-
-
-cdef buffer_to_word(char* buffer):
-    cdef uint32_t* value = <uint32_t*> buffer
-    return value[0]
-
-
-cdef buffer_to_float(char* buffer):
-    cdef float* value = <float*> buffer
-    return value[0]
-
-
-cdef buffer_to_double(char* buffer):
-    cdef double* value = <double*> buffer
-    return value[0]
-
-
-cdef class MemWatch:
-    cdef MemWatchEntry c_entry
-
-    def __cinit__(self, label: str, console_address: int, is_pointer: bool):
-        self.c_entry = MemWatchEntry(label.encode("utf-8"), console_address, MemType.type_word, MemBase.base_decimal, False, 1, is_pointer)
-
-    def add_offset(self, offset: int):
-        self.c_entry.addOffset(offset)
-
-    def get_value(self):
-        return buffer_to_word(self.c_entry.getMemory())
-        
-    def read_memory_from_ram(self):
-        return self.c_entry.readMemoryFromRAM() == MemOperationReturnCode.OK
-
-    def write_memory_from_string(self, value: str):
-        return self.c_entry.writeMemoryFromString(value.encode("utf-8")) == MemOperationReturnCode.OK
-
-
-def hook():
-    return DolphinAccessor.hook()
-
-
-def un_hook():
-    return DolphinAccessor.unHook()
-
-
-def is_hooked() -> bool:
-    if DolphinAccessor.getStatus() == DolphinStatus.hooked:
-        return True
-    else:
-        return False
-
-
-def assert_hooked():
-    if not is_hooked():
-        raise RuntimeError("not hooked")
-
-
-def follow_pointers(console_address: int, pointer_offsets: List[int]) -> int:
-    assert_hooked()
-    real_console_address = console_address
-
-    mem2Distance = DolphinAccessor.getMEM1ToMEM2Distance()
-
-    cdef char memory_buffer[4]
-    for offset in pointer_offsets:
-        if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, mem2Distance), memory_buffer, 4, True):
-            real_console_address = buffer_to_word(memory_buffer)
-            if DolphinAccessor.isValidConsoleAddress(real_console_address):
-                real_console_address += offset
-            else:
-                raise RuntimeError(f"Address {real_console_address} is not valid")
-        else:
-            raise RuntimeError(f"Could not read memory at {real_console_address}")
-
-    return real_console_address
-
-
-cdef _read_memory(console_address, char* memory_buffer, int size):
-    assert_hooked()
-    if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):
-        raise RuntimeError(f"Could not read memory at {console_address}")
-
-
-def read_byte(console_address: int) -> int:
-    cdef char memory_buffer[1]
-    _read_memory(console_address, memory_buffer, 1)
-    return (<uint8_t*> memory_buffer)[0]
-
-
-def read_word(console_address: int) -> int:
-    cdef char memory_buffer[4]
-    _read_memory(console_address, memory_buffer, 4)
-    return (<uint32_t*> memory_buffer)[0]
-
-
-def read_float(console_address: int) -> float:
-    cdef char memory_buffer[4]
-    _read_memory(console_address, memory_buffer, 4)
-    return (<float*> memory_buffer)[0]
-
-
-def read_double(console_address: int) -> double:
-    cdef char memory_buffer[8]
-    _read_memory(console_address, memory_buffer, 8)    
-    return (<double*> memory_buffer)[0]
-
-
-def read_bytes(console_address: int, size: int) -> bytes:
-    memory = bytearray(size)
-    if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, size, False):
-        raise RuntimeError(f"Could not read memory at {console_address}")
-    return bytes(memory)
-
-
-cdef _write_memory(console_address, char* memory_buffer, int size):
-    assert_hooked()
-    if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory_buffer, size, True):
-        raise RuntimeError(f"Could not write memory at {console_address}")
-
-
-def write_byte(console_address: int, value: int):
-    cdef char memory_buffer[1]
-    (<uint8_t*> memory_buffer)[0] = value
-    _write_memory(console_address, memory_buffer, 1)
-
-
-def write_word(console_address: int, value: int):
-    cdef char memory_buffer[4]
-    (<uint32_t*> memory_buffer)[0] = value
-    _write_memory(console_address, memory_buffer, 4)
-
-
-def write_float(console_address: int, value: float):
-    cdef char memory_buffer[4]
-    (<float*> memory_buffer)[0] = value
-    _write_memory(console_address, memory_buffer, 4)
-
-
-def write_double(console_address: int, value: double):
-    cdef char memory_buffer[8]
-    (<double*> memory_buffer)[0] = value
-    _write_memory(console_address, memory_buffer, 8)
-
-
-def write_bytes(console_address: int, memory: bytes):
-    assert_hooked()
-    if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.getMEM1ToMEM2Distance()), memory, len(memory), False):
+from typing import List
+
+from libc.stdint cimport uint8_t, uint32_t, uint64_t
+from libcpp cimport bool as c_bool
+from libcpp.string cimport string
+
+
+cdef extern from "Common/MemoryCommon.h" namespace "Common::MemType":
+    cdef enum MemType:
+        type_word
+
+
+cdef extern from "Common/MemoryCommon.h" namespace "Common::MemBase":
+    cdef enum MemBase:
+        base_decimal
+
+
+cdef extern from "Common/MemoryCommon.h" namespace "Common::MemOperationReturnCode":
+    cdef enum MemOperationReturnCode:
+        invalidInput
+        operationFailed
+        inputTooLong
+        invalidPointer
+        OK
+
+cdef extern from "Common/CommonUtils.h" namespace "Common":
+    uint32_t dolphinAddrToOffset(uint32_t, c_bool)
+    uint32_t offsetToDolphinAddr(uint32_t, c_bool)
+
+
+cdef extern from "DolphinProcess/DolphinAccessor.h" namespace "DolphinComm::DolphinStatus":
+    cdef enum DolphinStatus:
+        hooked
+        notRunning
+        noEmu
+        unHooked
+
+
+cdef extern from "DolphinProcess/DolphinAccessor.h" namespace "DolphinComm":
+    cdef cppclass DolphinAccessor:
+        @staticmethod
+        void init()
+
+        @staticmethod
+        void free()
+
+        @staticmethod
+        void hook()
+
+        @staticmethod
+        void unHook()
+
+        @staticmethod
+        c_bool readFromRAM(uint32_t, char*, const size_t, c_bool)
+        
+        @staticmethod
+        c_bool writeToRAM(uint32_t, const char*, const size_t, c_bool)
+
+        @staticmethod
+        int getPID()
+        
+        @staticmethod
+        DolphinStatus getStatus()
+
+        @staticmethod
+        c_bool isValidConsoleAddress(uint32_t)
+
+        @staticmethod
+        c_bool isARAMAccessible()
+
+
+cdef extern from "MemoryWatch/MemWatchEntry.h":
+    cdef cppclass MemWatchEntry:
+        MemWatchEntry()
+        MemWatchEntry(string, uint32_t, MemType, MemBase, c_bool, size_t, c_bool)
+
+        char* getMemory()
+
+        void addOffset(int)
+        MemOperationReturnCode readMemoryFromRAM()
+        MemOperationReturnCode writeMemoryFromString(string)
+
+
+cdef buffer_to_word(char* buffer):
+    cdef uint32_t* value = <uint32_t*> buffer
+    return value[0]
+
+
+cdef buffer_to_float(char* buffer):
+    cdef float* value = <float*> buffer
+    return value[0]
+
+
+cdef buffer_to_double(char* buffer):
+    cdef double* value = <double*> buffer
+    return value[0]
+
+
+cdef class MemWatch:
+    cdef MemWatchEntry c_entry
+
+    def __cinit__(self, label: str, console_address: int, is_pointer: bool):
+        self.c_entry = MemWatchEntry(label.encode("utf-8"), console_address, MemType.type_word, MemBase.base_decimal, False, 1, is_pointer)
+
+    def add_offset(self, offset: int):
+        self.c_entry.addOffset(offset)
+
+    def get_value(self):
+        return buffer_to_word(self.c_entry.getMemory())
+        
+    def read_memory_from_ram(self):
+        return self.c_entry.readMemoryFromRAM() == MemOperationReturnCode.OK
+
+    def write_memory_from_string(self, value: str):
+        return self.c_entry.writeMemoryFromString(value.encode("utf-8")) == MemOperationReturnCode.OK
+
+
+def hook():
+    return DolphinAccessor.hook()
+
+
+def un_hook():
+    return DolphinAccessor.unHook()
+
+
+def is_hooked() -> bool:
+    if DolphinAccessor.getStatus() == DolphinStatus.hooked:
+        return True
+    else:
+        return False
+
+
+def assert_hooked():
+    if not is_hooked():
+        raise RuntimeError("not hooked")
+
+
+def follow_pointers(console_address: int, pointer_offsets: List[int]) -> int:
+    assert_hooked()
+    real_console_address = console_address
+
+    is_aram_accessible = DolphinAccessor.isARAMAccessible()
+
+    cdef char memory_buffer[4]
+    for offset in pointer_offsets:
+        if DolphinAccessor.readFromRAM(dolphinAddrToOffset(real_console_address, is_aram_accessible), memory_buffer, 4, True):
+            real_console_address = buffer_to_word(memory_buffer)
+            if DolphinAccessor.isValidConsoleAddress(real_console_address):
+                real_console_address += offset
+            else:
+                raise RuntimeError(f"Address {real_console_address} is not valid")
+        else:
+            raise RuntimeError(f"Could not read memory at {real_console_address}")
+
+    return real_console_address
+
+
+cdef _read_memory(console_address, char* memory_buffer, int size):
+    assert_hooked()
+    if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):
+        raise RuntimeError(f"Could not read memory at {console_address}")
+
+
+def read_byte(console_address: int) -> int:
+    cdef char memory_buffer[1]
+    _read_memory(console_address, memory_buffer, 1)
+    return (<uint8_t*> memory_buffer)[0]
+
+
+def read_word(console_address: int) -> int:
+    cdef char memory_buffer[4]
+    _read_memory(console_address, memory_buffer, 4)
+    return (<uint32_t*> memory_buffer)[0]
+
+
+def read_float(console_address: int) -> float:
+    cdef char memory_buffer[4]
+    _read_memory(console_address, memory_buffer, 4)
+    return (<float*> memory_buffer)[0]
+
+
+def read_double(console_address: int) -> double:
+    cdef char memory_buffer[8]
+    _read_memory(console_address, memory_buffer, 8)    
+    return (<double*> memory_buffer)[0]
+
+
+def read_bytes(console_address: int, size: int) -> bytes:
+    memory = bytearray(size)
+    if not DolphinAccessor.readFromRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, size, False):
+        raise RuntimeError(f"Could not read memory at {console_address}")
+    return bytes(memory)
+
+
+cdef _write_memory(console_address, char* memory_buffer, int size):
+    assert_hooked()
+    if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory_buffer, size, True):
+        raise RuntimeError(f"Could not write memory at {console_address}")
+
+
+def write_byte(console_address: int, value: int):
+    cdef char memory_buffer[1]
+    (<uint8_t*> memory_buffer)[0] = value
+    _write_memory(console_address, memory_buffer, 1)
+
+
+def write_word(console_address: int, value: int):
+    cdef char memory_buffer[4]
+    (<uint32_t*> memory_buffer)[0] = value
+    _write_memory(console_address, memory_buffer, 4)
+
+
+def write_float(console_address: int, value: float):
+    cdef char memory_buffer[4]
+    (<float*> memory_buffer)[0] = value
+    _write_memory(console_address, memory_buffer, 4)
+
+
+def write_double(console_address: int, value: double):
+    cdef char memory_buffer[8]
+    (<double*> memory_buffer)[0] = value
+    _write_memory(console_address, memory_buffer, 8)
+
+
+def write_bytes(console_address: int, memory: bytes):
+    assert_hooked()
+    if not DolphinAccessor.writeToRAM(dolphinAddrToOffset(console_address, DolphinAccessor.isARAMAccessible()), memory, len(memory), False):
         raise RuntimeError(f"Could not write memory at {console_address}")
```

### Comparing `dolphin-memory-engine-1.1.2/dolphin_memory_engine.egg-info/PKG-INFO` & `dolphin-memory-engine-1.1.3/python_src/dolphin_memory_engine.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1
-Name: dolphin-memory-engine
-Version: 1.1.2
-Summary: Hooks into the memory of a running Dolphin processes, allowing access to the game memory.
-Home-page: https://github.com/henriquegemignani/py-dolphin-memory-engine
-Author: Henrique Gemignani
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python Dolphin Memory Engine
-
-[![Travis CI Build Status](https://travis-ci.org/henriquegemignani/py-dolphin-memory-engine.svg?branch=master)](https://travis-ci.org/henriquegemignani/py-dolphin-memory-engine)
-[![AppVeyor CI Build Status](https://ci.appveyor.com/api/projects/status/i5rb9s0w1l4ahbgj?svg=true)](https://ci.appveyor.com/project/henriquegemignani/py-dolphin-memory-engine)
-
-A python library designed to read and write the emulated memory of [the Dolphin emulator](https://github.com/dolphin-emu/dolphin) during runtime. 
-
-Binary wheels are available on pypi for Python 3.6, 3.7 and 3.8. Use `python -m pip install dolphin-memory-engine` with a modern enough version.
-
-
-## System requirements
-Any x86_64 based system should work, however, Mac OS is _not_ supported. Additionally, 32-bit x86 based systems are unsupported since Dolphin dropped their support.
-
-You need to have Dolphin running ***and*** _have the emulation started_ for this program to be useful. As such, the system must meet Dolphin's [system requirements](https://github.com/dolphin-emu/dolphin#system-requirements). Additionally, at least 250 MB of free memory is required.
-
-
-## License
-This program is licensed under the MIT license which grants you the permission to do  anything you wish to with the software, as long as you preserve all copyright notices. (See the file LICENSE for the legal text.)
-
-
-## Development Help
-
-To compile the extension in debug:
-
-$ python3 -m venv venv
-$ source venv/bin/activate
-$ python -m pip install Cython pytest
-$ python setup.py build_ext -g --inplace --force
-$ python -m pytest
+Metadata-Version: 2.1
+Name: dolphin-memory-engine
+Version: 1.1.3
+Summary: Hooks into the memory of a running Dolphin processes, allowing access to the game memory.
+Author: Henrique Gemignani
+Project-URL: Homepage, https://github.com/henriquegemignani/py-dolphin-memory-engine
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+# Python Dolphin Memory Engine
+
+A python library designed to read and write the emulated memory of [the Dolphin emulator](https://github.com/dolphin-emu/dolphin) during runtime. 
+
+Binary wheels are available on pypi for Python 3.8 to 3.12. Use `python -m pip install dolphin-memory-engine`.
+
+
+## System requirements
+Any x86_64 based system should work, however, Mac OS is _not_ supported. Additionally, 32-bit x86 based systems are unsupported since Dolphin dropped their support.
+
+You need to have Dolphin running ***and*** _have the emulation started_ for this program to be useful. As such, the system must meet Dolphin's [system requirements](https://github.com/dolphin-emu/dolphin#system-requirements). Additionally, at least 250 MB of free memory is required.
+
+
+If it doesn't work, verify that you do not have the `nosuid` mount flag on your `/etc/fstab` as it can cause this command to silently fail.
+
+## License
+This program is licensed under the MIT license which grants you the permission to do  anything you wish to with the software, as long as you preserve all copyright notices. (See the file LICENSE for the legal text.)
+
+
+## Development Help
+
+To compile the extension in debug:
+
+$ python3 -m venv venv
+$ source venv/bin/activate
+$ python -m pip install Cython pytest
+$ python setup.py build_ext -g --inplace --force
+$ python -m pytest
```

