# Comparing `tmp/tabela-sac-1.0.0.tar.gz` & `tmp/tabela-sac-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabela-sac-1.0.0.tar", last modified: Thu Mar  9 15:03:48 2023, max compression
+gzip compressed data, was "tabela-sac-2.0.0.tar", last modified: Fri Jul 14 19:14:12 2023, max compression
```

## Comparing `tabela-sac-1.0.0.tar` & `tabela-sac-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-03-09 15:03:48.468846 tabela-sac-1.0.0/
--rw-r--r--   0 joaonogueira   (501) staff       (20)    11337 2022-12-24 20:24:01.000000 tabela-sac-1.0.0/LICENSE
--rw-r--r--   0 joaonogueira   (501) staff       (20)      111 2022-12-24 20:24:01.000000 tabela-sac-1.0.0/MANIFEST.in
--rw-r--r--   0 joaonogueira   (501) staff       (20)     4056 2023-03-09 15:03:48.468679 tabela-sac-1.0.0/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)     3237 2023-03-08 18:04:51.000000 tabela-sac-1.0.0/README.md
--rw-r--r--   0 joaonogueira   (501) staff       (20)      969 2023-03-09 15:00:12.000000 tabela-sac-1.0.0/settings.ini
--rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-03-09 15:03:48.468903 tabela-sac-1.0.0/setup.cfg
--rw-r--r--   0 joaonogueira   (501) staff       (20)     2541 2022-12-24 20:24:01.000000 tabela-sac-1.0.0/setup.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-03-09 15:03:48.466872 tabela-sac-1.0.0/tabela_sac/
--rw-r--r--   0 joaonogueira   (501) staff       (20)       22 2023-03-09 15:00:12.000000 tabela-sac-1.0.0/tabela_sac/__init__.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)      914 2023-03-09 15:00:12.000000 tabela-sac-1.0.0/tabela_sac/_modidx.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)     1114 2023-03-09 15:00:12.000000 tabela-sac-1.0.0/tabela_sac/cli.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)     1450 2023-03-09 15:00:12.000000 tabela-sac-1.0.0/tabela_sac/core.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-03-09 15:03:48.468347 tabela-sac-1.0.0/tabela_sac.egg-info/
--rw-r--r--   0 joaonogueira   (501) staff       (20)     4056 2023-03-09 15:03:48.000000 tabela-sac-1.0.0/tabela_sac.egg-info/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      372 2023-03-09 15:03:48.000000 tabela-sac-1.0.0/tabela_sac.egg-info/SOURCES.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-03-09 15:03:48.000000 tabela-sac-1.0.0/tabela_sac.egg-info/dependency_links.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)      113 2023-03-09 15:03:48.000000 tabela-sac-1.0.0/tabela_sac.egg-info/entry_points.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2022-12-24 20:39:29.000000 tabela-sac-1.0.0/tabela_sac.egg-info/not-zip-safe
--rw-r--r--   0 joaonogueira   (501) staff       (20)       31 2023-03-09 15:03:48.000000 tabela-sac-1.0.0/tabela_sac.egg-info/requires.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)       11 2023-03-09 15:03:48.000000 tabela-sac-1.0.0/tabela_sac.egg-info/top_level.txt
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-14 19:14:12.981102 tabela-sac-2.0.0/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)    11337 2023-07-14 16:26:43.000000 tabela-sac-2.0.0/LICENSE
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      111 2023-07-14 16:26:43.000000 tabela-sac-2.0.0/MANIFEST.in
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     9605 2023-07-14 19:14:12.980738 tabela-sac-2.0.0/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     8806 2023-07-14 19:05:54.000000 tabela-sac-2.0.0/README.md
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      969 2023-07-14 19:06:22.000000 tabela-sac-2.0.0/settings.ini
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-07-14 19:14:12.981215 tabela-sac-2.0.0/setup.cfg
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     2541 2023-07-14 16:26:43.000000 tabela-sac-2.0.0/setup.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-14 19:14:12.979039 tabela-sac-2.0.0/tabela_sac/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       22 2023-07-14 19:06:28.000000 tabela-sac-2.0.0/tabela_sac/__init__.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     1175 2023-07-14 19:06:28.000000 tabela-sac-2.0.0/tabela_sac/_modidx.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     1114 2023-07-14 19:06:28.000000 tabela-sac-2.0.0/tabela_sac/cli.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     3355 2023-07-14 19:06:28.000000 tabela-sac-2.0.0/tabela_sac/core.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-14 19:14:12.980516 tabela-sac-2.0.0/tabela_sac.egg-info/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     9605 2023-07-14 19:14:12.000000 tabela-sac-2.0.0/tabela_sac.egg-info/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      372 2023-07-14 19:14:12.000000 tabela-sac-2.0.0/tabela_sac.egg-info/SOURCES.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-07-14 19:14:12.000000 tabela-sac-2.0.0/tabela_sac.egg-info/dependency_links.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      112 2023-07-14 19:14:12.000000 tabela-sac-2.0.0/tabela_sac.egg-info/entry_points.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-07-14 17:00:43.000000 tabela-sac-2.0.0/tabela_sac.egg-info/not-zip-safe
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       31 2023-07-14 19:14:12.000000 tabela-sac-2.0.0/tabela_sac.egg-info/requires.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       11 2023-07-14 19:14:12.000000 tabela-sac-2.0.0/tabela_sac.egg-info/top_level.txt
```

### Comparing `tabela-sac-1.0.0/LICENSE` & `tabela-sac-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tabela-sac-1.0.0/settings.ini` & `tabela-sac-2.0.0/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = tabela-sac
 lib_name = tabela-sac
-version = 1.0.0
+version = 2.0.0
 min_python = 3.7
 license = apache2
 doc_path = _docs
 lib_path = tabela_sac
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `tabela-sac-1.0.0/setup.py` & `tabela-sac-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `tabela-sac-1.0.0/tabela_sac/_modidx.py` & `tabela-sac-2.0.0/tabela_sac/_modidx.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,8 +5,10 @@
                 'doc_host': 'https://joaopcnogueira.github.io',
                 'git_url': 'https://github.com/joaopcnogueira/tabela-sac',
                 'lib_path': 'tabela_sac'},
   'syms': { 'tabela_sac.cli': { 'tabela_sac.cli.gerar_tabela_sac': ('cli.html#gerar_tabela_sac', 'tabela_sac/cli.py'),
                                 'tabela_sac.cli.install_package': ('cli.html#install_package', 'tabela_sac/cli.py')},
             'tabela_sac.core': { 'tabela_sac.core.SACCalculator': ('core.html#saccalculator', 'tabela_sac/core.py'),
                                  'tabela_sac.core.SACCalculator.__init__': ('core.html#saccalculator.__init__', 'tabela_sac/core.py'),
+                                 'tabela_sac.core.SACCalculator.amortizacao_extra_mensal': ( 'core.html#saccalculator.amortizacao_extra_mensal',
+                                                                                             'tabela_sac/core.py'),
                                  'tabela_sac.core.SACCalculator.tabela': ('core.html#saccalculator.tabela', 'tabela_sac/core.py')}}}
```

### Comparing `tabela-sac-1.0.0/tabela_sac/cli.py` & `tabela-sac-2.0.0/tabela_sac/cli.py`

 * *Files identical despite different names*

