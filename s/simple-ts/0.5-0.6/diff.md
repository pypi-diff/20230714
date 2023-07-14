# Comparing `tmp/simple_ts-0.5.tar.gz` & `tmp/simple_ts-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_ts-0.5.tar", last modified: Fri Jul 14 04:05:06 2023, max compression
+gzip compressed data, was "simple_ts-0.6.tar", last modified: Fri Jul 14 04:08:42 2023, max compression
```

## Comparing `simple_ts-0.5.tar` & `simple_ts-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 04:05:06.769194 simple_ts-0.5/
--rw-rw-rw-   0        0        0      125 2023-07-14 04:05:06.769194 simple_ts-0.5/PKG-INFO
--rw-rw-rw-   0        0        0      655 2023-07-14 03:15:08.000000 simple_ts-0.5/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 04:05:06.769194 simple_ts-0.5/setup.cfg
--rw-rw-rw-   0        0        0      262 2023-07-14 04:04:56.000000 simple_ts-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 04:05:06.753557 simple_ts-0.5/simple_ts.egg-info/
--rw-rw-rw-   0        0        0      125 2023-07-14 04:05:06.000000 simple_ts-0.5/simple_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-14 04:05:06.000000 simple_ts-0.5/simple_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 04:05:06.000000 simple_ts-0.5/simple_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-14 04:05:06.000000 simple_ts-0.5/simple_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 04:05:06.000000 simple_ts-0.5/simple_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 04:05:06.769194 simple_ts-0.5/simplets/
--rw-rw-rw-   0        0        0       35 2023-07-14 04:04:35.000000 simple_ts-0.5/simplets/__init__.py
--rw-rw-rw-   0        0        0     2860 2023-07-14 03:42:27.000000 simple_ts-0.5/simplets/simplets.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:08:42.894399 simple_ts-0.6/
+-rw-rw-rw-   0        0        0      125 2023-07-14 04:08:42.894399 simple_ts-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2023-07-14 03:15:08.000000 simple_ts-0.6/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 04:08:42.894399 simple_ts-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      262 2023-07-14 04:08:34.000000 simple_ts-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:08:42.886914 simple_ts-0.6/simple_ts.egg-info/
+-rw-rw-rw-   0        0        0      125 2023-07-14 04:08:42.000000 simple_ts-0.6/simple_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-14 04:08:42.000000 simple_ts-0.6/simple_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 04:08:42.000000 simple_ts-0.6/simple_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-14 04:08:42.000000 simple_ts-0.6/simple_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 04:08:42.000000 simple_ts-0.6/simple_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 04:08:42.894399 simple_ts-0.6/simplets/
+-rw-rw-rw-   0        0        0       35 2023-07-14 04:04:35.000000 simple_ts-0.6/simplets/__init__.py
+-rw-rw-rw-   0        0        0     2854 2023-07-14 04:08:24.000000 simple_ts-0.6/simplets/simplets.py
```

### Comparing `simple_ts-0.5/README.txt` & `simple_ts-0.6/README.txt`

 * *Files identical despite different names*

### Comparing `simple_ts-0.5/simplets/simplets.py` & `simple_ts-0.6/simplets/simplets.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         trend = result.trend
         seasonal = result.seasonal
         residuals = result.resid
 
 # Plotar as componentes da decomposição
         plt.figure(figsize=(10, 8))
         plt.subplot(411)
-        plt.plot(serie_ar, label='Original')
+        plt.plot(ts, label='Original')
         plt.legend(loc='upper left')
 
         plt.subplot(412)
         plt.plot(trend, label='Tendência')
         plt.legend(loc='upper left')
 
         plt.subplot(413)
```

