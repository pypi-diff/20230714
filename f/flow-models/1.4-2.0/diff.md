# Comparing `tmp/flow_models-1.4.tar.gz` & `tmp/flow_models-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow_models-1.4.tar", last modified: Sat Jul  8 21:36:00 2023, max compression
+gzip compressed data, was "flow_models-2.0.tar", last modified: Fri Jul 14 13:39:49 2023, max compression
```

## Comparing `flow_models-1.4.tar` & `flow_models-2.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:36:00.638553 flow_models-1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 21:35:51.000000 flow_models-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-08 21:36:00.638553 flow_models-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-08 21:35:51.000000 flow_models-1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:36:00.634554 flow_models-1.4/flow_models/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/anonymize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/cut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:36:00.638553 flow_models-1.4/flow_models/elephants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/elephants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/elephants/calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/elephants/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/elephants/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/elephants/sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:36:00.638553 flow_models-1.4/flow_models/first_mirror/
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/first_mirror/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)    15093 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/hist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/hist_np.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:36:00.638553 flow_models-1.4/flow_models/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/cryptopan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23462 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/kde.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/mix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/lib/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/series_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-08 21:35:51.000000 flow_models-1.4/flow_models/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:36:00.638553 flow_models-1.4/flow_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-08 21:36:00.000000 flow_models-1.4/flow_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-08 21:36:00.000000 flow_models-1.4/flow_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:36:00.000000 flow_models-1.4/flow_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-08 21:36:00.000000 flow_models-1.4/flow_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:36:00.638553 flow_models-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-08 21:35:51.000000 flow_models-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:39:49.629207 flow_models-2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-14 13:39:39.000000 flow_models-2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-14 13:39:49.629207 flow_models-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-14 13:39:39.000000 flow_models-2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:39:49.629207 flow_models-2.0/flow_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/cut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:39:49.629207 flow_models-2.0/flow_models/elephants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/elephants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/elephants/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/elephants/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/elephants/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/elephants/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:39:49.629207 flow_models-2.0/flow_models/first_mirror/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/first_mirror/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/first_mirror/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15093 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/hist_np.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:39:49.629207 flow_models-2.0/flow_models/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/lib/cryptopan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/lib/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24724 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/lib/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/lib/kde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/lib/mix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/lib/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/lib/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/series_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-14 13:39:39.000000 flow_models-2.0/flow_models/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:39:49.629207 flow_models-2.0/flow_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-14 13:39:49.000000 flow_models-2.0/flow_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-14 13:39:49.000000 flow_models-2.0/flow_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:39:49.000000 flow_models-2.0/flow_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 13:39:49.000000 flow_models-2.0/flow_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 13:39:49.629207 flow_models-2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-14 13:39:39.000000 flow_models-2.0/setup.py
```

### Comparing `flow_models-1.4/LICENSE` & `flow_models-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/PKG-INFO` & `flow_models-2.0/flow_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flow_models
-Version: 1.4
+Name: flow-models
+Version: 2.0
 Summary: A framework for analysis and modeling of IP network flows
 Home-page: https://github.com/piotrjurkiewicz/flow-models
 Author: Piotr Jurkiewicz
 Author-email: piotr.jerzy.jurkiewicz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `flow_models-1.4/README.md` & `flow_models-2.0/README.md`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models/anonymize.py` & `flow_models-2.0/flow_models/anonymize.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from input and to be skipped (skip_out) and written (count_out) after filtering.
 
 Example: (encrypts flow records in binary format and outputs as csv lines to standard output)
 
     flow_models.anonymize -i binary -O - --count-in 1000 --key boojahyoo3vaeToong0Eijee7Ahz3yee sorted
 """
 
-def anonymize(in_files, output, in_format='nfcapd', out_format='csv_flow', skip_in=0, count_in=None, skip_out=0, count_out=None, filter_expr=None, key=None):
+def anonymize(in_files, output, in_format='nfcapd', out_format='csv_flow', skip_in=0, count_in=None, skip_out=0, count_out=None, filter_expr=None, key=''):
     """
     Anonymizes IP addresses in IPv4 flows using Crypto-PAn algorithm.
 
     Parameters
     ----------
     in_files : list[pathlib.Path]
         input files paths
@@ -46,18 +46,19 @@
         number of flows to read from input
     skip_out : int, default 0
         number of flows to skip after filtering
     count_out : int, default None, meaning all flows
         number of flows to output after filtering
     filter_expr : CodeType, optional
         filter expression
-    key : bytes
+    key : str
         encryption key (32 bytes)
     """
 
+    key = key.encode()
     if not key or len(key) != 32:
         ValueError("Please specify 32 bytes long encryption key")
 
     cp = CryptoPan(key)
     ip_cache = {}
 
     reader, writer = IN_FORMATS[in_format], OUT_FORMATS[out_format]
@@ -66,15 +67,15 @@
     next(writer)
 
     counters = {'skip_in': skip_in, 'count_in': count_in, 'skip_out': skip_out, 'count_out': count_out}
     written = 0
 
     for file in in_files:
         for af, prot, inif, outif, sa0, sa1, sa2, sa3, da0, da1, da2, da3, sp, dp, first, first_ms, last, last_ms, packets, octets, aggs in reader(file, counters=counters, filter_expr=filter_expr):
-            if af == 2:
+            if not af or af == 2:
                 try:
                     sa3 = ip_cache[sa3]
                 except KeyError:
                     ip_cache[sa3] = cp.anonymize(sa3)
                     sa3 = ip_cache[sa3]
                 try:
                     da3 = ip_cache[da3]
@@ -87,15 +88,15 @@
 
     writer.close()
 
     logmsg(f'Finished all files. Written: {written}')
 
 def parser():
     p = IOArgumentParser(description=__doc__, epilog=EPILOG)
-    p.add_argument('--key', type=bytes, default=None, help='32 bytes long encryption key')
+    p.add_argument('--key', type=str, default='', help='32 bytes long encryption key')
     return p
 
 def main():
     app_args = parser().parse_args()
     anonymize(**vars(app_args))
```

### Comparing `flow_models-1.4/flow_models/convert.py` & `flow_models-2.0/flow_models/convert.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models/cut.py` & `flow_models-2.0/flow_models/cut.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,37 +68,51 @@
     """
 
     if in_format != 'binary' or out_format != 'binary':
         raise ValueError("Both input and output formats must be binary")
     if filter_expr is not None:
         raise NotImplementedError("Filter expressions are not supported")
 
+    in_files = prepare_file_list(in_files)
+
     if output != sys.stdout:
         output = pathlib.Path(output)
         if output.is_dir() or len(in_files) > 1:
             output.mkdir(parents=True, exist_ok=True)
         else:
             output.parent.mkdir(parents=True, exist_ok=True)
 
-    for in_file in prepare_file_list(in_files):
+    for in_file in in_files:
         try:
             size = array.array(in_file.suffix[1:]).itemsize
-            skip_in = skip_in * size
+            if skip_in > 0:
+                skip = skip_in * size
+            else:
+                skip = 0
             if count_in is not None:
-                count_in = count_in * size
+                if count_in > 0:
+                    count = count_in * size
+                else:
+                    count = 0
             else:
-                count_in = in_file.stat().st_size - skip_in
-            count_in = count_in - skip_out * size
-            count_in = min(count_in, count_out * size)
+                count = in_file.stat().st_size - skip
+            if skip_out > 0:
+                count = count - skip_out * size
+                skip += skip_out * size
+            if count_out is not None:
+                if count_out > 0:
+                    count = min(count, count_out * size)
+                else:
+                    count = 0
         except TypeError:
             logmsg('Cut array:', in_file, 'Wrong type')
             return
 
         logmsg('Cut array:', in_file, size)
-        subprocess.run(['dd', f'if={in_file}', f'of={output}' if output != sys.stdout else 'status=none', f'count={count_in}', f'skip={skip_in}', 'iflag=count_bytes,skip_bytes'])
+        subprocess.run(['dd', f'if={in_file}', f'of={output / in_file.name}' if output != sys.stdout else 'status=none', f'count={count}', f'skip={skip}', 'iflag=count_bytes,skip_bytes'])
 
 
 def parser():
     p = IOArgumentParser(description=__doc__, epilog=EPILOG)
     p._option_string_actions['-i'].choices = ['binary']
     p._option_string_actions['-i'].default = 'binary'
     p._option_string_actions['-o'].choices = ['binary']
```

### Comparing `flow_models-1.4/flow_models/elephants/calculate.py` & `flow_models-2.0/flow_models/elephants/calculate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/python3
+"""
+Calculates flow reduction curves from mixture or histogram data for first, threshold and sampling methods.
+"""
+
 import argparse
 
 import numpy as np
 import pandas as pd
 import scipy.interpolate
 import scipy.stats
 
@@ -138,15 +142,35 @@
     ad['occupancy_mean'] = 1 / ad['fraction_mean']
     for what in ['flows', 'packets', 'fraction', 'octets']:
         ad[what + '_mean'] *= 100
 
     return pd.DataFrame(ad, x_probs if method == 'sampling' else x)
 
 def calculate(obj, index=None, x_val='length', methods=tuple(METHODS)):
-    data = load_data(obj)
+    """
+    Calculate flow table occupancy reduction curve for given traffic coverages.
+
+    Parameters
+    ----------
+    obj : os.PathLike
+        csv_hist histogram file or mixture directory
+    index : int | numpy.array, optional
+        flow size thresholds to calculate upon or their number, default [2..2^24]
+    x_val : str, default 'length'
+        x axis value
+    methods : list, ['first', 'threshold', 'sampling']
+        methods to calculate
+
+    Returns
+    -------
+    dict[str, pd.DataFrame]
+        calculated DataFrame for each method
+    """
+
+    data = list(load_data([obj]).values())[0]
 
     if index is None:
         index = 1 / np.power(2, range(25))
     elif isinstance(index, int):
         index = 1 / np.logspace(0, 32, index, base=2)
     else:
         index = index
@@ -157,22 +181,25 @@
             df = calculate_data(data, np.array(index), x_val, method)
         else:
             df = calculate_mix(data, np.array(index), x_val, method)
         dataframes[method] = df
 
     return dataframes
 
+def parser():
+    p = argparse.ArgumentParser(description=__doc__)
+    p.add_argument('-n', type=int, default=None, help='number of index points')
+    p.add_argument('-x', default='length', choices=X_VALUES, help='x axis value')
+    p.add_argument('-m', default='all', choices=METHODS, help='method')
+    p.add_argument('--save', action='store_true', help='save to files')
+    p.add_argument('file', help='csv_hist file or mixture directory')
+    return p
+
 def main():
-    parser = argparse.ArgumentParser(description=__doc__)
-    parser.add_argument('-n', type=int, default=None, help='number of index points')
-    parser.add_argument('-x', default='length', choices=X_VALUES, help='x axis value')
-    parser.add_argument('-m', default='all', choices=METHODS, help='method')
-    parser.add_argument('--save', action='store_true', help='save to files')
-    parser.add_argument('file', help='csv_hist file or mixture directory')
-    app_args = parser.parse_args()
+    app_args = parser().parse_args()
 
     if app_args.m == 'all':
         methods = METHODS
     else:
         methods = [app_args.m]
 
     resdic = calculate(app_args.file, app_args.n, app_args.x, methods)
```

### Comparing `flow_models-1.4/flow_models/elephants/plot.py` & `flow_models-2.0/flow_models/elephants/plot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/python3
+"""
+Plots flow reduction curves from mixture or histogram data for first, threshold and sampling methods.
+"""
+
 import argparse
 import collections
 import pathlib
 
 import matplotlib.pyplot as plt
 import matplotlib.ticker
 import numpy as np
@@ -174,14 +178,35 @@
                 plt.close(fig)
 
         if one:
             out = f'results_{method}'
             save_figure(fig, out)
             plt.close(fig)
 
+def print_tables(simulated):
+    for x_val in X_VALUES:
+        dd = pd.concat({'first': simulated['first'][x_val], 'threshold': simulated['threshold'][x_val],
+                        'sampling': simulated['sampling'][x_val]})
+        df = dd.loc[['first', 'threshold']].unstack(0)
+        if x_val == 'length':
+            df = df.iloc[:22]
+        df = df[['octets_mean', 'operations_mean', 'occupancy_mean']]
+        df = df.swaplevel(axis=1).sort_index(axis=1).reindex(['octets_mean', 'operations_mean', 'occupancy_mean'],
+                                                             axis=1, level=1)
+        df.index = df.index.astype(np.int64)
+        print(df.to_latex(float_format='%.2f'))
+
+        df = dd.loc[['sampling']].unstack(0)
+        if x_val == 'length':
+            df = df.iloc[:22]
+        df = df[['octets_mean', 'operations_mean', 'occupancy_mean']]
+        df = df.swaplevel(axis=1).sort_index(axis=1).reindex(['octets_mean', 'operations_mean', 'occupancy_mean'],
+                                                             axis=1, level=1)
+        print(df.to_latex(float_format='%.2f'))
+
 def plot_probability():
     fig, ax = plt.subplots(1, 1, figsize=FIGSIZE)
     idx = np.geomspace(1, 1000, 512)
     ax.plot(idx, 1 - (1 - 0.1) ** idx, 'k-', lw=2,
             label='p  0.1$')
     ax.plot(idx, 1 - (1 - 0.01) ** idx, 'k-', lw=2,
             label='p = 0.1$')
@@ -209,20 +234,24 @@
         for method, df in calculate('../mixtures/all/' + x_val, 1024, x_val=x_val, methods=methods).items():
             calculated[method][x_val] = df.dropna()
 
     plot_all(calculated, simulated, one)
     plot_usage(calculated, 'occupancy')
     plot_usage(calculated, 'operations')
     plot_traffic(calculated)
+    print_tables(simulated)
+
+def parser():
+    p = argparse.ArgumentParser(description=__doc__)
+    p.add_argument('--one', action='store_true', help='plot in one file')
+    p.add_argument('files', nargs='+', help='csv_hist files to plot')
+    return p
 
 def main():
-    parser = argparse.ArgumentParser(description=__doc__)
-    parser.add_argument('--one', action='store_true', help='plot in one file')
-    parser.add_argument('files', nargs='+', help='csv_hist files to plot')
-    app_args = parser.parse_args()
+    app_args = parser().parse_args()
 
     with matplotlib_config(latex=False):
         plot_probability()
         plot(app_args.files, app_args.one)
 
 
 if __name__ == '__main__':
```

### Comparing `flow_models-1.4/flow_models/elephants/simulate.py` & `flow_models-2.0/flow_models/elephants/simulate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/python3
+"""
+Simulates first, threshold and sampling elephant detection methods on packet-level from mixture or histogram data.
+"""
+
 import argparse
 import collections
 import concurrent.futures
 import json
 import os
 import pathlib
 import pickle
@@ -95,15 +99,41 @@
             fraction_covered += fraction_of_flow_covered
             octets_covered += octets * fraction_of_flow_covered
     result_u = np.array([flows_all, packets_all, octets_all, flows_added, packets_covered], dtype='u8')
     result_f = np.array([fraction_covered, octets_covered], dtype='f8')
     return method, p, r, result_u, result_f
 
 def simulate(obj, size=1, x_val='length', seed=None, methods=tuple(METHODS), rounds=5, affinity=False):
-    data = load_data(obj)
+    """
+    Simulate flow table occupancy reduction curve for given traffic coverages.
+
+    Parameters
+    ----------
+    obj : os.PathLike
+        csv_hist histogram file or mixture directory
+    size : int, default 1
+        number of flows to generate
+    x_val : str, default 'length'
+        x axis value
+    seed : int, optional
+        seed for the random generator
+    methods : list, ['first', 'threshold', 'sampling']
+        methods to calculate
+    rounds : int, default 5
+        number of repetitions of simulation on generated flows
+    affinity: bool, default False
+        set per-cpu affinity for all processes
+
+    Returns
+    -------
+    dict[str, pd.DataFrame]
+        calculated DataFrame for each method
+    """
+
+    data = list(load_data([obj]).values())[0]
 
     x = 1 / np.power(2, range(25))
 
     running = [0]
     done = collections.defaultdict(int)
     results = {}
     lock = threading.Lock()
@@ -175,25 +205,28 @@
             df.sort_index(ascending=False, inplace=True)
         else:
             df.index = df.index.astype('uint64')
         dd[k] = df
 
     return dd
 
+def parser():
+    p = argparse.ArgumentParser(description=__doc__)
+    p.add_argument('-n', type=int, default=1000000, help='number of generated flows')
+    p.add_argument('-r', type=int, default=10, help='rounds')
+    p.add_argument('--seed', type=int, default=None, help='seed')
+    p.add_argument('-x', default='length', choices=X_VALUES, help='x axis value')
+    p.add_argument('-m', default='all', choices=METHODS, help='method')
+    p.add_argument('--save', action='store_true', help='save to files')
+    p.add_argument('--affinity', action='store_true', help='set affinity')
+    p.add_argument('file', help='csv_hist file or mixture directory')
+    return p
+
 def main():
-    parser = argparse.ArgumentParser(description=__doc__)
-    parser.add_argument('-n', type=int, default=1000000, help='number of generated flows')
-    parser.add_argument('-r', type=int, default=10, help='rounds')
-    parser.add_argument('--seed', type=int, default=None, help='seed')
-    parser.add_argument('-x', default='length', choices=X_VALUES, help='x axis value')
-    parser.add_argument('-m', default='all', choices=METHODS, help='method')
-    parser.add_argument('--save', action='store_true', help='save to files')
-    parser.add_argument('--affinity', action='store_true', help='set affinity')
-    parser.add_argument('file', help='csv_hist file or mixture directory')
-    app_args = parser.parse_args()
+    app_args = parser().parse_args()
 
     if app_args.m == 'all':
         methods = METHODS
     else:
         methods = [app_args.m]
 
     if app_args.save:
```

### Comparing `flow_models-1.4/flow_models/first_mirror/simulate.py` & `flow_models-2.0/flow_models/first_mirror/simulate.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 from input and to be skipped (skip_out) and written (count_out) after filtering.
 
 Example: (simulates mirroring of first 3 packets of a flow to control plane)
 
     flow_models.first_mirror.simulate -i binary -O mirror_3 --mirror 3 sorted
 """
 
-def series(in_files, output, in_format='nfcapd', out_format='csv_series', skip_in=0, count_in=None, skip_out=0, count_out=None, filter_expr=None, mirror=0):
+def first_mirror(in_files, output, in_format='nfcapd', out_format='csv_series', skip_in=0, count_in=None, skip_out=0, count_out=None, filter_expr=None, mirror=0):
     """
-    Generate packets and octets time series from flow records.
+    Generate mirrored packets and octets time series from flow records.
 
     Parameters
     ----------
     in_files : list[pathlib.Path]
         input files paths
     output : os.PathLike
         directory path
@@ -55,76 +55,65 @@
     assert out_format == 'csv_series'
 
     fields = ['first', 'first_ms', 'last', 'last_ms', 'packets', 'octets']
 
     counters = {'skip_in': skip_in, 'count_in': count_in, 'skip_out': skip_out, 'count_out': count_out}
     written = 0
 
-    # [flows, packets, octets, packets_mirrored, octets_mirrored]
-    dd = collections.defaultdict(lambda: [[0, 0, 0, 0, 0] for _ in range(86400)])
+    # [packets_mirrored, octets_mirrored]
+    dd = collections.defaultdict(lambda: [[0, 0] for _ in range(86400)])
 
     for file in in_files:
         for af, prot, inif, outif, sa0, sa1, sa2, sa3, da0, da1, da2, da3, sp, dp, first, first_ms, last, last_ms, packets, octets, aggs in reader(file, counters=counters, filter_expr=filter_expr, fields=fields):
             day = first // 86400
             second_in_day = first % 86400
             d = dd[day]
-            d[second_in_day][0] += 1
             if packets == 1:
-                d[second_in_day][1] += 1
-                d[second_in_day][2] += octets
                 if mirror > 0:
-                    d[second_in_day][3] += 1
-                    d[second_in_day][4] += octets
+                    d[second_in_day][0] += 1
+                    d[second_in_day][1] += octets
             else:
                 float_second_in_day = second_in_day + first_ms / 1000
                 duration = last - first + (last_ms - first_ms) / 1000
                 piat = duration / packets
                 avg_packet_size = octets / packets
                 int_packet_size = avg_packet_size.__trunc__()
-                for n in range(packets):
+                for n in range(min(packets, mirror)):
                     packet_size = int_packet_size + (octets - int_packet_size - avg_packet_size * (packets - 1 - n)).__trunc__()
                     ds = d[float_second_in_day.__trunc__()]
-                    ds[1] += 1
-                    ds[2] += packet_size
-                    if n < mirror:
-                        ds[3] += 1
-                        ds[4] += packet_size
+                    ds[0] += 1
+                    ds[1] += packet_size
                     octets -= packet_size
                     float_second_in_day += piat
                     while float_second_in_day >= 86400.0:
                         day += 1
                         float_second_in_day -= 86400.0
                         d = dd[day]
-                assert octets == 0
             written += 1
         logmsg(f'Finished: {file}. Written: {written}')
 
     output = pathlib.Path(output)
     output.mkdir(parents=True, exist_ok=True)
     for day in dd:
-        with open(output / f"{day}.flows", 'w') as f, open(output / f"{day}.packets", 'w') as p, open(output / f"{day}.octets", 'w') as o, \
-             open(output / f"{day}.packets_mirrored", 'w') as pm, open(output / f"{day}.octets_mirrored", 'w') as om:
+        with open(output / f"{day}.packets_mirrored", 'w') as pm, open(output / f"{day}.octets_mirrored", 'w') as om:
             for second_in_day in range(86400):
-                f.write("%d\n" % dd[day][second_in_day][0])
-                p.write("%d\n" % dd[day][second_in_day][1])
-                o.write("%d\n" % dd[day][second_in_day][2])
-                pm.write("%d\n" % dd[day][second_in_day][3])
-                om.write("%d\n" % dd[day][second_in_day][4])
+                pm.write("%d\n" % dd[day][second_in_day][0])
+                om.write("%d\n" % dd[day][second_in_day][1])
 
     logmsg(f'Finished all files. Written: {written}')
 
 def parser():
     p = IOArgumentParser(description=__doc__, epilog=EPILOG)
     p._option_string_actions['-o'].choices = ['csv_series']
     p._option_string_actions['-o'].default = 'csv_series'
     p._option_string_actions['-O'].help = 'directory for output'
     p._option_string_actions['-O'].default = '.'
     p.add_argument('--mirror', default=0, type=int, help='mirror first N packets')
     return p
 
 def main():
     app_args = parser().parse_args()
-    series(**vars(app_args))
+    first_mirror(**vars(app_args))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `flow_models-1.4/flow_models/fit.py` & `flow_models-2.0/flow_models/fit.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models/generate.py` & `flow_models-2.0/flow_models/generate.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models/hist.py` & `flow_models-2.0/flow_models/hist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 """
 Calculates histograms of flows length, size, duration or rate.
 """
 
-from .lib.io import IOArgumentParser, IN_FORMATS, write_none, write_line, FILTER_HELP
+from .lib.io import IOArgumentParser, IN_FORMATS, write_none, write_line, FILTER_HELP, write_append
 from .lib.util import logmsg, bin_calc_one, bin_calc_log
 
 EPILOG = \
 f"""
 Use this tool to calculate histogram of flow features.
 
 The output is a histogram of a selected feature in csv_hist format.
@@ -23,15 +23,15 @@
 
 Example: (calculates logarithmically binned histogram of flow length from the sorted directory)
 
     flow_models.hist -i binary -x length -b 12 sorted
 """
 
 X_VALUES = ['length', 'size', 'duration', 'rate']
-OUT_FORMATS = {'csv_hist': write_line, 'none': write_none}
+OUT_FORMATS = {'csv_hist': write_line, 'append': write_append, 'none': write_none}
 
 class FlowBin:
 
     __slots__ = 'bin_lo', 'bin_hi', 'flows_sum', 'packets_sum', 'octets_sum', 'duration_sum', 'rate_sum', 'aggs_sum'
 
     def __init__(self, bin_lo, bin_hi):
         self.bin_lo = bin_lo
@@ -42,15 +42,15 @@
         self.duration_sum = 0
         self.rate_sum = 0
         self.aggs_sum = 0
 
     def to_line(self, fields):
         return ','.join(str(int(getattr(self, c))) for c in fields)
 
-def hist(in_files, output, in_format='nfcapd', out_format='csv_hist', skip_in=0, count_in=None, skip_out=0, count_out=None, filter_expr=None, bin_exp=0, x_value='length', additional_columns=()):
+def hist(in_files, output, in_format='nfcapd', out_format='csv_hist', skip_in=0, count_in=None, skip_out=0, count_out=None, filter_expr=None, bin_exp=0, x_value='length', additional_columns=[]):
     """
     Calculates histograms of flows length, size, duration or rate.
 
     Parameters
     ----------
     in_files : list[os.PathLike]
         input files paths
```

### Comparing `flow_models-1.4/flow_models/hist_np.py` & `flow_models-2.0/flow_models/hist_np.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import concurrent.futures
 import functools
 import os
 import pathlib
 
 import numpy as np
 
-from .lib.io import write_line, write_none, IOArgumentParser, load_arrays, FILTER_HELP
+from .lib.io import write_line, write_none, IOArgumentParser, load_arrays, FILTER_HELP, write_append
 from .lib.util import logmsg, bin_calc_log, measure_memory
 
 EPILOG = \
 f"""
 Use this tool to calculate histogram of flow features.
 
 The output is a histogram of a selected feature in csv_hist format.
@@ -34,15 +34,15 @@
 """
 
 # MAX_MEM = 64 * (1024 ** 3)
 MAX_MEM = os.sysconf('SC_PAGE_SIZE') * os.sysconf('SC_PHYS_PAGES') // 4
 N_JOBS = 4
 
 X_VALUES = ['length', 'size']
-OUT_FORMATS = {'csv_hist': write_line, 'none': write_none}
+OUT_FORMATS = {'csv_hist': write_line, 'append': write_append, 'none': write_none}
 
 def get_column_array(mm, column, start, stop):
     if column in mm:
         return mm[column][start:stop]
     elif column in ['duration', 'rate']:
         if 'duration' in mm:
             dur = mm['duration'][start:stop]
@@ -148,15 +148,15 @@
             else:
                 logmsg(f'Done directory: {path} chunk: [{start}:{stop}]')
 
     logmsg(f'Done directory: {path} chunk: all')
 
     return results
 
-def hist(in_files, output, in_format='binary', out_format='csv_hist', skip_in=0, count_in=None, skip_out=0, count_out=None, filter_expr=None, bin_exp=0, x_value='length', additional_columns=()):
+def hist(in_files, output, in_format='binary', out_format='csv_hist', skip_in=0, count_in=None, skip_out=0, count_out=None, filter_expr=None, bin_exp=0, x_value='length', additional_columns=[]):
     """
     Calculates histograms of flows length, size, duration or rate.
 
     Parameters
     ----------
     in_files : list[os.PathLike]
         input files paths
```

### Comparing `flow_models-1.4/flow_models/lib/cryptopan.py` & `flow_models-2.0/flow_models/lib/cryptopan.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models/lib/data.py` & `flow_models-2.0/flow_models/lib/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 
 def load_data(objects):
     """
     Loads mixtures or histograms into a structured dictionary.
 
     Parameters
     ----------
-    objects : list[pathlib.Path]
+    objects : list[os.PathLike]
         list of paths to load
 
     Returns
     -------
     dict
         container with loaded data
     """
```

### Comparing `flow_models-1.4/flow_models/lib/io.py` & `flow_models-2.0/flow_models/lib/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import array
 import io
 import mmap
+import os
 import pathlib
 import subprocess
 import sys
 import warnings
 
 from flow_models.lib.util import logmsg
 
@@ -75,14 +76,21 @@
     fields.first_ms.append(flow[15])
     fields.last.append(flow[16])
     fields.last_ms.append(flow[17])
     fields.packets.append(flow[18])
     fields.octets.append(flow[19])
     fields.aggs.append(flow[20])
 
+def flow_to_int(flow):
+    return int(flow[0]), int(flow[1]), int(flow[2]), int(flow[3]), \
+           int(flow[4]), int(flow[5]), int(flow[6]), int(flow[7]), \
+           int(flow[8]), int(flow[9]), int(flow[10]), int(flow[11]), \
+           int(flow[12]), int(flow[13]), int(flow[14]), int(flow[15]), int(flow[16]), int(flow[17]), \
+           int(flow[18]), int(flow[19]), int(flow[20])
+
 def read_flow_csv(in_file, counters=None, filter_expr=None, fields=None):
     """
     Read and yield all flows in a csv_flow file/stream.
 
     Parameters
     ----------
     in_file : os.PathLike | io.TextIOWrapper
@@ -124,29 +132,29 @@
                     counters['count_in'] -= 1
                 else:
                     break
             af, prot, inif, outif, \
             sa0, sa1, sa2, sa3, \
             da0, da1, da2, da3, \
             sp, dp, first, first_ms, last, last_ms, \
-            packets, octets, aggs = line.split(',')
+            packets, octets, aggs = flow_to_int(line.split(','))
             if filter_expr is None or eval(filter_expr):
                 if counters['skip_out'] > 0:
                     counters['skip_out'] -= 1
                 else:
                     if counters['count_out'] is not None:
                         if counters['count_out'] > 0:
                             counters['count_out'] -= 1
                         else:
                             break
-                    yield int(af), int(prot), int(inif), int(outif), \
-                          int(sa0), int(sa1), int(sa2), int(sa3), \
-                          int(da0), int(da1), int(da2), int(da3), \
-                          int(sp), int(dp), \
-                          int(first), int(first_ms), int(last), int(last_ms), int(packets), int(octets), int(aggs)
+                    yield af, prot, inif, outif, \
+                          sa0, sa1, sa2, sa3, \
+                          da0, da1, da2, da3, \
+                          sp, dp, first, first_ms, last, last_ms, \
+                          packets, octets, aggs
 
     if not isinstance(in_file, io.IOBase):
         stream.close()
 
 def read_pipe(in_file, counters=None, filter_expr=None, fields=None):
     """
     Read and yield all flows in a nfdump pipe file/stream.
@@ -194,30 +202,38 @@
                     counters['count_in'] -= 1
                 else:
                     break
             af, first, last, prot, \
             sa0, sa1, sa2, sa3, sp, da0, da1, da2, da3, dp, \
             srcas, dstas, inif, outif, \
             tcp_flags, tos, packets, octets = line.split(b'|')
-            first, first_ms = first[:-3], first[-3:]
-            last, last_ms = last[:-3], last[-3:]
+            first, first_ms = int(first[:-3]), int(first[-3:])
+            last, last_ms = int(last[:-3]), int(last[-3:])
+            af, prot, inif, outif, \
+            sa0, sa1, sa2, sa3, \
+            da0, da1, da2, da3, \
+            sp, dp, packets, octets, aggs = int(af), int(prot), int(inif), int(outif), \
+                                            int(sa0), int(sa1), int(sa2), int(sa3), \
+                                            int(da0), int(da1), int(da2), int(da3), \
+                                            int(sp), int(dp), \
+                                            int(packets), int(octets), 0
             if filter_expr is None or eval(filter_expr):
                 if counters['skip_out'] > 0:
                     counters['skip_out'] -= 1
                 else:
                     if counters['count_out'] is not None:
                         if counters['count_out'] > 0:
                             counters['count_out'] -= 1
                         else:
                             break
-                    yield int(af), int(prot), int(inif), int(outif), \
-                          int(sa0), int(sa1), int(sa2), int(sa3), \
-                          int(da0), int(da1), int(da2), int(da3), \
-                          int(sp), int(dp), \
-                          int(first), int(first_ms), int(last), int(last_ms), int(packets), int(octets), 0
+                    yield af, prot, inif, outif, \
+                          sa0, sa1, sa2, sa3, \
+                          da0, da1, da2, da3, \
+                          sp, dp, first, first_ms, last, last_ms, \
+                          packets, octets, aggs
 
     if not isinstance(in_file, io.IOBase):
         stream.close()
 
 def read_nfcapd(in_file, counters=None, filter_expr=None, fields=None):
     """
     Read and yield all flows in a nfdump nfpcapd file.
@@ -292,14 +308,16 @@
     path = pathlib.Path(in_dir)
     assert path.exists() and path.is_dir()
     flows = Flows()
     fields_to_load = [name for name in flows.fields if fields is None or name in fields]
     use_numpy = True
 
     arrays, filtered, size = load_arrays(path, fields_to_load, counters, filter_expr)
+    if not size:
+        return
     for name in flows.fields:
         if name in arrays:
             setattr(flows, name, arrays[name])
             if isinstance(arrays[name], memoryview):
                 use_numpy = False
         else:
             setattr(flows, name, ZeroArray())
@@ -358,14 +376,24 @@
                           da0, da1, da2, da3, \
                           sp, dp, \
                           first, first_ms, last, last_ms, packets, octets, aggs
 def write_none(_):
     while True:
         _ = yield
 
+def write_append(output, *_):
+    while True:
+        flow = yield
+        output.append(flow)
+
+def write_extend(output, *_):
+    while True:
+        flow = yield
+        output.extend(flow)
+
 def write_line(output, header_line=None):
     """
     Write lines to the output.
 
     Parameters
     ----------
     output : os.PathLike | io.TextIOWrapper
@@ -491,17 +519,20 @@
     """
 
     name, dtype, path = find_array_path(path)
     flags = mmap.MAP_SHARED if mode == 'c' else mmap.MAP_SHARED
     prot = mmap.PROT_READ
     if mode != 'r':
         prot |= mmap.PROT_WRITE
-    with open(str(path)) as f:
-        mm = mmap.mmap(f.fileno(), 0, flags=flags, prot=prot)
-    mv = memoryview(mm).cast(dtype)
+    if os.path.getsize(str(path)) > 0:
+        with open(str(path)) as f:
+            mm = mmap.mmap(f.fileno(), 0, flags=flags, prot=prot)
+        mv = memoryview(mm).cast(dtype)
+    else:
+        mv = memoryview(b'').cast(dtype)
     return name, dtype, mv
 
 def load_array_np(path, mode='r'):
     """
     Load a numpy array as numpy.memmap.
 
     Parameters
@@ -567,43 +598,49 @@
                 name, dtype, ar = load_array_mv(path / name, 'r')
             if size is None:
                 size = len(ar)
             else:
                 assert len(ar) == size
             if counters['skip_in'] > 0:
                 ar = ar[counters['skip_in']:]
-            if counters['count_in'] is not None and counters['count_in'] > 0:
-                ar = ar[:counters['count_in']]
+            if counters['count_in'] is not None:
+                if counters['count_in'] > 0:
+                    ar = ar[:counters['count_in']]
+                else:
+                    ar = ar[0:0]
             ars[name] = ar
         except FileNotFoundError:
             warnings.warn(f"Array file for flow field '{name}' not found in directory {path}."
                           " Assuming zero as value of this field")
             ars[name] = ZeroArray()
 
     if size is not None:
         if counters['skip_in'] > 0:
             size = max(size - counters['skip_in'], 0)
             counters['skip_in'] -= min(counters['skip_in'], size)
-        if counters['count_in'] is not None and counters['count_in'] > 0:
-            size = min(size, counters['count_in'])
-            counters['count_in'] -= min(counters['count_in'], size)
+        if counters['count_in'] is not None:
+            if counters['count_in'] > 0:
+                size = min(size, counters['count_in'])
+                counters['count_in'] -= min(counters['count_in'], size)
+            else:
+                size = 0
 
     for ar in ars.values():
         if not isinstance(ar, ZeroArray):
             assert len(ar) == size
 
     filtered = ...
     if use_numpy and filter_expr is not None:
         for name in filter_expr.co_names:
             if isinstance(ars[name], ZeroArray):
                 raise ValueError(f"Filter is using flow field '{name}' which is not present in input files")
         logmsg(f"Starting filtering: {filter_expr.co_filename}")
         filtered = eval(filter_expr, ars)
         filtered_count = np.count_nonzero(filtered)
-        logmsg(f"Finished filtering: {filtered_count}/{size} ({100 * filtered_count/size} %)")
+        logmsg(f"Finished filtering: {filtered_count}/{size} ({100 * filtered_count/size if size else 0} %)")
 
     arrays = {}
     for name in (fields if use_numpy else fields_to_load):
         arrays[name] = ars[name]
 
     return arrays, filtered, size
 
@@ -669,8 +706,8 @@
             else:
                 namespace.output = pathlib.Path(namespace.output)
         if 'filter_expr' in namespace and namespace.filter_expr:
             namespace.filter_expr = compile(namespace.filter_expr, f'FILTER: {namespace.filter_expr}', 'eval')
         return namespace
 
 IN_FORMATS = {'csv_flow': read_flow_csv, 'pipe': read_pipe, 'nfcapd': read_nfcapd, 'binary': read_flow_binary}
-OUT_FORMATS = {'csv_flow': write_flow_csv, 'binary': write_flow_binary, 'none': write_none}
+OUT_FORMATS = {'csv_flow': write_flow_csv, 'binary': write_flow_binary, 'append': write_append, 'extend': write_extend, 'none': write_none}
```

### Comparing `flow_models-1.4/flow_models/lib/kde.py` & `flow_models-2.0/flow_models/lib/kde.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models/lib/mix.py` & `flow_models-2.0/flow_models/lib/mix.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models/lib/plot.py` & `flow_models-2.0/flow_models/lib/plot.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models/lib/util.py` & `flow_models-2.0/flow_models/lib/util.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models/merge.py` & `flow_models-2.0/flow_models/merge.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models/plot.py` & `flow_models-2.0/flow_models/plot.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models/series.py` & `flow_models-2.0/flow_models/series.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models/sort.py` & `flow_models-2.0/flow_models/sort.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models/summary.py` & `flow_models-2.0/flow_models/summary.py`

 * *Files identical despite different names*

### Comparing `flow_models-1.4/flow_models.egg-info/PKG-INFO` & `flow_models-2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flow-models
-Version: 1.4
+Name: flow_models
+Version: 2.0
 Summary: A framework for analysis and modeling of IP network flows
 Home-page: https://github.com/piotrjurkiewicz/flow-models
 Author: Piotr Jurkiewicz
 Author-email: piotr.jerzy.jurkiewicz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `flow_models-1.4/setup.py` & `flow_models-2.0/setup.py`

 * *Files identical despite different names*

