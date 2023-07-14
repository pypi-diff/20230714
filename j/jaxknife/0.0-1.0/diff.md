# Comparing `tmp/jaxknife-0.0.tar.gz` & `tmp/jaxknife-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxknife-0.0.tar", last modified: Thu Jul 13 20:15:52 2023, max compression
+gzip compressed data, was "jaxknife-1.0.tar", last modified: Fri Jul 14 13:55:20 2023, max compression
```

## Comparing `jaxknife-0.0.tar` & `jaxknife-1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 katyaleidig   (501) staff       (20)        0 2023-07-13 20:15:52.150270 jaxknife-0.0/
--rw-r--r--   0 katyaleidig   (501) staff       (20)        0 2023-07-12 14:54:14.000000 jaxknife-0.0/LICENSE
--rw-r--r--   0 katyaleidig   (501) staff       (20)       72 2023-07-13 20:15:52.149765 jaxknife-0.0/PKG-INFO
--rw-r--r--   0 katyaleidig   (501) staff       (20)       89 2023-07-10 20:17:56.000000 jaxknife-0.0/README.md
-drwxr-xr-x   0 katyaleidig   (501) staff       (20)        0 2023-07-13 20:15:52.141080 jaxknife-0.0/jaxknife/
--rw-r--r--   0 katyaleidig   (501) staff       (20)       19 2023-07-12 15:00:21.000000 jaxknife-0.0/jaxknife/__init__.py
--rw-r--r--   0 katyaleidig   (501) staff       (20)     1599 2023-07-13 19:59:05.000000 jaxknife-0.0/jaxknife/bootstrap.py
--rw-r--r--   0 katyaleidig   (501) staff       (20)      510 2023-07-12 14:52:11.000000 jaxknife-0.0/jaxknife/stats_funcs.py
-drwxr-xr-x   0 katyaleidig   (501) staff       (20)        0 2023-07-13 20:15:52.147055 jaxknife-0.0/jaxknife.egg-info/
--rw-r--r--   0 katyaleidig   (501) staff       (20)       72 2023-07-13 20:15:51.000000 jaxknife-0.0/jaxknife.egg-info/PKG-INFO
--rw-r--r--   0 katyaleidig   (501) staff       (20)      271 2023-07-13 20:15:51.000000 jaxknife-0.0/jaxknife.egg-info/SOURCES.txt
--rw-r--r--   0 katyaleidig   (501) staff       (20)        1 2023-07-13 20:15:51.000000 jaxknife-0.0/jaxknife.egg-info/dependency_links.txt
--rw-r--r--   0 katyaleidig   (501) staff       (20)       17 2023-07-13 20:15:51.000000 jaxknife-0.0/jaxknife.egg-info/requires.txt
--rw-r--r--   0 katyaleidig   (501) staff       (20)        9 2023-07-13 20:15:51.000000 jaxknife-0.0/jaxknife.egg-info/top_level.txt
--rw-r--r--   0 katyaleidig   (501) staff       (20)       38 2023-07-13 20:15:52.150392 jaxknife-0.0/setup.cfg
--rw-r--r--   0 katyaleidig   (501) staff       (20)      628 2023-07-12 15:16:57.000000 jaxknife-0.0/setup.py
-drwxr-xr-x   0 katyaleidig   (501) staff       (20)        0 2023-07-13 20:15:52.148608 jaxknife-0.0/tests/
--rw-r--r--   0 katyaleidig   (501) staff       (20)      784 2023-07-13 19:59:05.000000 jaxknife-0.0/tests/test_data.py
+drwxr-xr-x   0 katyaleidig   (501) staff       (20)        0 2023-07-14 13:55:20.429775 jaxknife-1.0/
+-rw-r--r--   0 katyaleidig   (501) staff       (20)        0 2023-07-12 14:54:14.000000 jaxknife-1.0/LICENSE
+-rw-r--r--   0 katyaleidig   (501) staff       (20)       72 2023-07-14 13:55:20.428049 jaxknife-1.0/PKG-INFO
+-rw-r--r--   0 katyaleidig   (501) staff       (20)      361 2023-07-14 13:54:32.000000 jaxknife-1.0/README.md
+drwxr-xr-x   0 katyaleidig   (501) staff       (20)        0 2023-07-14 13:55:20.418579 jaxknife-1.0/jaxknife/
+-rw-r--r--   0 katyaleidig   (501) staff       (20)       19 2023-07-14 13:54:32.000000 jaxknife-1.0/jaxknife/__init__.py
+-rw-r--r--   0 katyaleidig   (501) staff       (20)     2849 2023-07-14 13:54:32.000000 jaxknife-1.0/jaxknife/jaxknife.py
+-rw-r--r--   0 katyaleidig   (501) staff       (20)     1309 2023-07-14 13:54:32.000000 jaxknife-1.0/jaxknife/stats_funcs.py
+drwxr-xr-x   0 katyaleidig   (501) staff       (20)        0 2023-07-14 13:55:20.425926 jaxknife-1.0/jaxknife.egg-info/
+-rw-r--r--   0 katyaleidig   (501) staff       (20)       72 2023-07-14 13:55:20.000000 jaxknife-1.0/jaxknife.egg-info/PKG-INFO
+-rw-r--r--   0 katyaleidig   (501) staff       (20)      308 2023-07-14 13:55:20.000000 jaxknife-1.0/jaxknife.egg-info/SOURCES.txt
+-rw-r--r--   0 katyaleidig   (501) staff       (20)        1 2023-07-14 13:55:20.000000 jaxknife-1.0/jaxknife.egg-info/dependency_links.txt
+-rw-r--r--   0 katyaleidig   (501) staff       (20)       17 2023-07-14 13:55:20.000000 jaxknife-1.0/jaxknife.egg-info/requires.txt
+-rw-r--r--   0 katyaleidig   (501) staff       (20)        9 2023-07-14 13:55:20.000000 jaxknife-1.0/jaxknife.egg-info/top_level.txt
+-rw-r--r--   0 katyaleidig   (501) staff       (20)       38 2023-07-14 13:55:20.429995 jaxknife-1.0/setup.cfg
+-rw-r--r--   0 katyaleidig   (501) staff       (20)      628 2023-07-12 15:16:57.000000 jaxknife-1.0/setup.py
+drwxr-xr-x   0 katyaleidig   (501) staff       (20)        0 2023-07-14 13:55:20.427136 jaxknife-1.0/tests/
+-rw-r--r--   0 katyaleidig   (501) staff       (20)      543 2023-07-14 13:54:32.000000 jaxknife-1.0/tests/test_bootstrap_end2end.py
+-rw-r--r--   0 katyaleidig   (501) staff       (20)      907 2023-07-14 13:54:32.000000 jaxknife-1.0/tests/test_resamplers.py
```

### Comparing `jaxknife-0.0/setup.py` & `jaxknife-1.0/setup.py`

 * *Files identical despite different names*

