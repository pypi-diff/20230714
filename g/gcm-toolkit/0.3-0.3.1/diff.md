# Comparing `tmp/gcm_toolkit-0.3.tar.gz` & `tmp/gcm_toolkit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcm_toolkit-0.3.tar", last modified: Tue Feb 28 15:17:54 2023, max compression
+gzip compressed data, was "gcm_toolkit-0.3.1.tar", last modified: Fri Jul 14 06:44:22 2023, max compression
```

## Comparing `gcm_toolkit-0.3.tar` & `gcm_toolkit-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:17:54.912593 gcm_toolkit-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-02-28 15:17:54.912593 gcm_toolkit-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:17:54.908593 gcm_toolkit-0.3/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/bin/convert_to_gcmt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:17:54.908593 gcm_toolkit-0.3/gcm_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:17:54.908593 gcm_toolkit-0.3/gcm_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/core/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/core/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:17:54.912593 gcm_toolkit-0.3/gcm_toolkit/exorad/
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/exorad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/exorad/read_in.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6946 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/exorad/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/gcm_dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    26614 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/gcmtools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:17:54.912593 gcm_toolkit-0.3/gcm_toolkit/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/tests/test_exorad.py
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/tests/test_gcmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/tests/test_gcmtools_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/tests/test_manipulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:17:54.912593 gcm_toolkit-0.3/gcm_toolkit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/utils/gcm_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    58322 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/utils/manipulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/utils/passport.py
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/gcm_toolkit/utils/read_and_write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 15:17:54.908593 gcm_toolkit-0.3/gcm_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-02-28 15:17:54.000000 gcm_toolkit-0.3/gcm_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-02-28 15:17:54.000000 gcm_toolkit-0.3/gcm_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 15:17:54.000000 gcm_toolkit-0.3/gcm_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-28 15:17:54.000000 gcm_toolkit-0.3/gcm_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-28 15:17:54.000000 gcm_toolkit-0.3/gcm_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 15:17:54.912593 gcm_toolkit-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-02-28 15:17:42.000000 gcm_toolkit-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:44:22.253136 gcm_toolkit-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-14 06:44:22.253136 gcm_toolkit-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:44:22.245136 gcm_toolkit-0.3.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/bin/convert_to_gcmt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:44:22.249136 gcm_toolkit-0.3.1/gcm_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:44:22.249136 gcm_toolkit-0.3.1/gcm_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/core/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/core/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:44:22.249136 gcm_toolkit-0.3.1/gcm_toolkit/exorad/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/exorad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/exorad/read_in.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6946 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/exorad/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/gcm_dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26614 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/gcmtools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:44:22.253136 gcm_toolkit-0.3.1/gcm_toolkit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/tests/test_exorad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/tests/test_gcmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/tests/test_gcmtools_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/tests/test_manipulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:44:22.253136 gcm_toolkit-0.3.1/gcm_toolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/utils/clouds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/utils/gcm_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66614 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21186 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/utils/manipulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/utils/passport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/gcm_toolkit/utils/read_and_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 06:44:22.249136 gcm_toolkit-0.3.1/gcm_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-14 06:44:22.000000 gcm_toolkit-0.3.1/gcm_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-14 06:44:22.000000 gcm_toolkit-0.3.1/gcm_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 06:44:22.000000 gcm_toolkit-0.3.1/gcm_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 06:44:22.000000 gcm_toolkit-0.3.1/gcm_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 06:44:22.000000 gcm_toolkit-0.3.1/gcm_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 06:44:22.253136 gcm_toolkit-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-14 06:44:12.000000 gcm_toolkit-0.3.1/setup.py
```

### Comparing `gcm_toolkit-0.3/LICENSE.md` & `gcm_toolkit-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/PKG-INFO` & `gcm_toolkit-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcm_toolkit
-Version: 0.3
+Version: 0.3.1
 Summary: postprocessing stuff
 Home-page: https://github.com/exorad/gcmt
 Author: Aaron David Schneider
 Author-email: aarondavid.schneider@nbi.ku.dk
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `gcm_toolkit-0.3/README.md` & `gcm_toolkit-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/bin/convert_to_gcmt` & `gcm_toolkit-0.3.1/bin/convert_to_gcmt`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/core/const.py` & `gcm_toolkit-0.3.1/gcm_toolkit/core/const.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/core/units.py` & `gcm_toolkit-0.3.1/gcm_toolkit/core/units.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/core/writer.py` & `gcm_toolkit-0.3.1/gcm_toolkit/core/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,27 +124,29 @@
         with open(typ, "w", encoding="utf-8") as fil:
             fil.close()
     else:
         Writer.on = False
         Writer.file_name = None
 
 
-def write_status(tag, message):
+def write_status(tag, message, end='\n'):
     """
     Write a status output that is auto layouted according to
     _writer set up. Careful: an ERROR status will call a
     ValueError.
 
     Parameters
     ----------
     tag : str
         tag of the status. Some have pre-defined meaning:
         'STAT', 'INFO', 'E-INFO', 'WARN', 'ERROR'
     message : str
         The message to be printed.
+    end : str, optional
+        end of string, default='\n'
     """
     writer = Writer()
     # define colors and layout according to tags
     color = writer.get_color(tag=tag)
     space = writer.get_spacer(tag=tag)
 
     # add line breaks after _writer.line_length characters
@@ -162,15 +164,15 @@
             line = tag_length + line[Writer.line_length + 1 :]
     liner += line
 
     # check if verbosity is whished
     if Writer.on:
         # write message to terminal
         if Writer.file_name is None:
-            print(color + liner + Writer.ENDC)
+            print(color + liner + Writer.ENDC, end=end)
 
         # write message to file
         else:
             with open(Writer.file_name, "a", encoding="utf-8") as fil:
                 fil.write(liner + "\n")
 
     if tag == "ERROR":
```

### Comparing `gcm_toolkit-0.3/gcm_toolkit/exorad/utils.py` & `gcm_toolkit-0.3.1/gcm_toolkit/exorad/utils.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/gcm_dataset_collection.py` & `gcm_toolkit-0.3.1/gcm_toolkit/gcm_dataset_collection.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/gcmtools.py` & `gcm_toolkit-0.3.1/gcm_toolkit/gcmtools.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/tests/test_exorad.py` & `gcm_toolkit-0.3.1/gcm_toolkit/tests/test_exorad.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/tests/test_gcmt.py` & `gcm_toolkit-0.3.1/gcm_toolkit/tests/test_gcmt.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/tests/test_gcmtools_common.py` & `gcm_toolkit-0.3.1/gcm_toolkit/tests/test_gcmtools_common.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/tests/test_interface.py` & `gcm_toolkit-0.3.1/gcm_toolkit/tests/test_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,14 +38,25 @@
     # Note: the pRT.setup_opa_structure is done by tools internally
 
     tools = GCMT(p_unit="bar", time_unit="day")  # create a GCMT object
     tools.read_raw(
         gcm=expected["gcm"], data_path=data_path, d_lat=15, d_lon=15
     )
 
+    # add cloud properties
+    dsi_clouds = tools.get_models('0')
+    tmp = np.ones((len(dsi_clouds['time']), len(dsi_clouds['lat']),
+                   len(dsi_clouds['lon']), len(dsi_clouds['Z_l'])))
+    dsi_clouds['ClAb'] = (('time', 'lat', 'lon', 'Z_l'), tmp*1e-5)
+    dsi_clouds['ClDs'] = (('time', 'lat', 'lon', 'Z_l'), tmp*1e2)
+    dsi_clouds['ClDr'] = (('time', 'lat', 'lon', 'Z_l'), tmp*1e3)
+    dsi_clouds['ClVf_Test1[s]'] = (('time', 'lat', 'lon', 'Z_l'), tmp*0.5)
+    dsi_clouds['ClVf_Test2[s]'] = (('time', 'lat', 'lon', 'Z_l'), tmp*0.5)
+    tools._replace_model('0', dsi_clouds)
+
     phases = np.linspace(0, 1, 50)
     interface = tools.get_prt_interface(pRT)
 
     interface.set_data(time=expected["times"][-1])
     interface.chem_from_poorman("T", co_ratio=0.55, feh_ratio=0.0)
 
     spectra = interface.calc_phase_spectrum(
@@ -98,22 +109,32 @@
             Rstar=expected["Rstar"],
             Tstar=None,
             semimajoraxis=expected["semimajoraxis"],
             normalize=True,
         )
 
     # test transit calculation set up
-    interface.set_data(time=expected["times"][-1], terminator_avg=True)
+    interface.set_data(time=expected["times"][-1], terminator_avg=True, lon_resolution=60)
     assert (interface.dsi['lon'].values == [-90, 90]).all()
     assert interface.dsi['lat'].values == [0]
 
     # test transit calculation
     interface.chem_from_poorman("T", co_ratio=0.55, feh_ratio=0.0)
     wave, spectra = interface.calc_transit_spectrum(mmw=2.33)
-    assert sum(wave) == 28.373223101833855
+    assert sum(spectra) == 45237213620.18512
+
+    # test transit calculation
+    interface.chem_from_poorman("T", co_ratio=0.55, feh_ratio=0.0)
+    wave, spectra = interface.calc_transit_spectrum(mmw=2.33, clouds=True)
+    assert sum(spectra) == 45331292591.13728
+
+    # test transit calculation
+    interface.chem_from_poorman("T", co_ratio=0.55, feh_ratio=0.0)
+    wave, spectra = interface.calc_transit_spectrum(mmw=2.33, clouds=True, use_bruggemann=True)
+    assert sum(spectra) == 45237213620.53514
 
     # Test if Pa works
     interface.dsi.attrs["p_unit"] = "Pa"
     interface.set_data(time=expected["times"][-1])
 
     # Test if something weird works
     interface.dsi.attrs["p_unit"] = "wrong"
```

### Comparing `gcm_toolkit-0.3/gcm_toolkit/tests/test_manipulations.py` & `gcm_toolkit-0.3.1/gcm_toolkit/tests/test_manipulations.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/tests/test_plots.py` & `gcm_toolkit-0.3.1/gcm_toolkit/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/tests/test_utils.py` & `gcm_toolkit-0.3.1/gcm_toolkit/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/tests/test_writer.py` & `gcm_toolkit-0.3.1/gcm_toolkit/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/utils/gcm_plotting.py` & `gcm_toolkit-0.3.1/gcm_toolkit/utils/gcm_plotting.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/utils/interface.py` & `gcm_toolkit-0.3.1/gcm_toolkit/utils/interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,23 @@
  e.g.: - petitRADTRANS            (Molliere+2019)
        - gCMCRT                   (Lee+2022)
        - 1D and pseudo-2D PAC     (Agundez+2014)
        - ...
 ==============================================================
 """
 import math
+import types
 import numpy as np
 import xarray as xr
 
 from ..core import writer as wrt
 from ..core.const import VARNAMES as c
+from ..utils.passport import is_the_data_cloudy
+from ..utils.clouds import cloud_opacities, patch_cloud_mix_opa, patch_calc_transm, \
+                           patch_delete_clouds
 
 
 class _Chemistry:
     """
     Chemistry class used to deal with different kinds of chemical models.
     """
 
@@ -232,50 +236,50 @@
                              'were selected, but only one can be given.')
 
         dsi = self.tools.get_one_model(tag).sel(time=time)
 
         if terminator_avg:
             # avarage over longitudinal opening angle. Note, this step also corrects
             # for smaller areas at polar regions
-            ds_morning = dsi.where((dsi[c['lon']] > -90 - lon_resolution/2) *
-                                   (dsi[c['lon']] < -90 + lon_resolution/2)).mean(c['lon'])
-            ds_evening = dsi.where((dsi[c['lon']] > 90 - lon_resolution/2) *
-                                   (dsi[c['lon']] < 90 + lon_resolution/2)).mean(c['lon'])
+            ds_m = dsi.where((dsi[c['lon']] > -90 - lon_resolution/2) *
+                             (dsi[c['lon']] < -90 + lon_resolution/2)).mean(c['lon'])
+            ds_e = dsi.where((dsi[c['lon']] > 90 - lon_resolution/2) *
+                             (dsi[c['lon']] < 90 + lon_resolution/2)).mean(c['lon'])
 
             # set latitude step size
             lat_step = 180 / lat_points
             lat_x = np.linspace(-90+lat_step/2, 90-lat_step/2, lat_points)
 
             # generate new dataset
             ds_transit = xr.Dataset(
-                data_vars=dict(
-                ),
-                coords=dict(
-                    lat=([c["lat"]], lat_x),
-                    lon=([c["lon"]], [-90, 90]),
-                    Z_l=([c["Z_l"]], dsi[c['Z_l']].values),
-                    Z=([c["Z"]], dsi[c['Z']].values)
-                ),
+                data_vars={},
+                coords={
+                    'lat': ([c["lat"]], lat_x),
+                    'lon': ([c["lon"]], [-90, 90]),
+                    'Z_l': ([c["Z_l"]], dsi[c['Z_l']].values),
+                    'Z': ([c["Z"]], dsi[c['Z']].values)
+                },
                 attrs=dsi.attrs
             )
 
-            # empty array to fill with temperature data
-            tmp = np.zeros((lat_points, 2, len(dsi[c["Z"]].values)))
-
             # avarage in latitude space
-            for lat in range(lat_points):
-                tmp[lat, 0, :] = ds_morning.where((ds_morning[c['lat']] > lat*lat_step - 90) *
-                                                  (ds_morning[c['lat']] < (lat+1)*lat_step - 90)
-                                                  ).mean(c['lat'])['T'].values
-                tmp[lat, 1, :] = ds_evening.where((ds_evening[c['lat']] > lat*lat_step - 90) *
-                                                  (ds_evening[c['lat']] < (lat+1)*lat_step - 90)
-                                                  ).mean(c['lat'])['T'].values
+            for key in ds_e.keys():
+                if key in ['T', 'ClAb', 'ClDs', 'ClDr'] or 'ClVf' in key:
+                    # empty array to fill with data
+                    tmp = np.zeros((lat_points, 2, len(dsi[c["Z"]].values)))
+                    for lat in range(lat_points):
+                        tmp[lat, 0, :] = ds_m.where((ds_m[c['lat']] > lat*lat_step - 90) *
+                                                    (ds_m[c['lat']] < (lat+1) * lat_step - 90)
+                                                    ).mean(c['lat'])[key].values
+                        tmp[lat, 1, :] = ds_e.where((ds_e[c['lat']] > lat*lat_step - 90) *
+                                                    (ds_e[c['lat']] < (lat+1)*lat_step - 90)
+                                                    ).mean(c['lat'])[key].values
 
-            # saving results
-            ds_transit[c['T']] = ((c['lat'], c['lon'], c['Z_l']), tmp)
+                    # saving results
+                    ds_transit[key] = ((c['lat'], c['lon'], c['Z_l']), tmp)
 
             # add mark that data is ready for tranist callcuations
             ds_transit.attrs['transit'] = True
 
             # return prepared dataset
             dsi = ds_transit
 
@@ -336,14 +340,16 @@
             A GCMTools object that is linked to the interface
         pRT: petitRADTRANS.Radtrans
             A pRT Radtrans object
         """
         super().__init__(tools)
         self.prt = prt
 
+        wrt.write_status("STAT", "Created Interface class for gcm_toolkit and petitRADTRANS")
+
     def set_data(self, time, tag=None, regrid_lowres=False,
                  terminator_avg=False, lat_points=1, lon_resolution=10):
         """
         Set the data to be used for the interface
 
         Parameters
         ----------
@@ -357,14 +363,25 @@
             terminator avaraging. This requires lat_points and lon_resolution.
         lat_points: int, optional
             number of equally spaced latitude grid points for each terminator (morning and evening)
         lon_resolution: float, optional
             longitudinal opening angle for terminator avareging
         """
 
+        wrt.write_status("STAT", "Selected data set for petitRADTRANS interface")
+        wrt.write_status("INFO", "time: " + str(time))
+        if tag is not None:
+            wrt.write_status("INFO", "tag: " + tag)
+        else:
+            wrt.write_status("INFO", "No tag given")
+
+        if terminator_avg:
+            wrt.write_status("INFO", "Data set ready for transmission spectrum calculation")
+
+
         self._set_data_common(time, tag=tag, regrid_lowres=regrid_lowres,
                               terminator_avg=terminator_avg, lat_points=lat_points,
                               lon_resolution=lon_resolution)
 
         if self.dsi.p_unit == "bar":
             press = self.dsi.Z.values
         elif self.dsi.p_unit == "Pa":
@@ -569,14 +586,17 @@
     def calc_transit_spectrum(
             self,
             mmw,
             gravity=None,
             rplanet=None,
             pressure_0=None,
             mass_frac=None,
+            clouds=None,
+            use_bruggemann=False,
+            asymmetric=False,
     ):
         """
         Calculate the transit spectrum. This function avarages T-p profiles in
         the terminator region and uses poorman equilbriums chemistry.
 
         Parameters
         ----------
@@ -591,15 +611,30 @@
             pressure level of the gravity and radius. Will default to the value provided by GCMT.
         mass_frac: List[List[Dict]], optional
             The mass fractions for each t_p point. Structure is as follows: mass_frac[i][j]['key']
             - i: [2 elements] 0 for morning terminator, 1 for evening terminator
             - j: [lat_points elements] latitude point starting from lowest
                  (closeset to lat = -90) to highest (closest to lat = 90)
             - dict must contain all mass fractions  elements given as opacity species to prt
-
+        clouds: Union[np.ndarray[i, j, h, w, k], bool], optional
+            The cloud opacities for each t_p point. Structure is as follows:
+            mass_frac[i][j][w][h][k]
+            - i: [2 elements] 0 for morning terminator, 1 for evening terminator
+            - j: [lat_points elements] latitude point starting from lowest
+                 (closeset to lat = -90) to highest (closest to lat = 90)
+            - w: [number of wavelength bins] this has to be equivalent to the wavelength
+                 structure of prt.
+            - h: [number of pressure points] this needs to be equivalent to the pressure
+                structure of the gcm.
+            - k: 0 for kappa_absorption and 1 for kappa_scatering
+        use_bruggemann: bool, optional
+            If this flag is set to true, bruggemann mixing is used. This is
+            more accurate but takes much longer to calculate.
+        asymmetric : bool, optional
+            If true, the spectra will be calculated for the morning and evening limb speratly.
 
         Returns
         -------
         wavelengths: xr.DataArray
             Wavelengths of the output spectra in micron
         spectra: xr.DataArray
             transit radius in cm
@@ -620,74 +655,210 @@
         if rplanet is None:
             rplanet = self.dsi.attrs.get(c["R_p"]) * 100
 
         # check if pressure is given, if not use gcm value
         if pressure_0 is None:
             pressure_0 = np.max(self.prt.press)*1e-6
 
+        # output
+        wrt.write_status("STAT", "Calculate transmission spectra")
+        wrt.write_status("INFO", "gravity: " + str(gravity))
+        wrt.write_status("INFO", "rplanet: " + str(rplanet))
+        if clouds is not None:
+            if isinstance(clouds, bool):
+                wrt.write_status("INFO", "Using GCM cloud structure")
+            else:
+                wrt.write_status("INFO", "Using given cloud structure")
+            if use_bruggemann:
+                wrt.write_status("INFO", "Bruggemann mixing used")
+            else:
+                wrt.write_status("INFO", "LLL mixing used")
+
+
+
+        # check if clouds are wished
+        do_clouds = False
+        if clouds is not None:
+            if isinstance(clouds, bool):
+                # set cloud flag to input
+                do_clouds = clouds
+            else:
+                do_clouds = True
+
+            # check if clouds are possible
+            if do_clouds and not is_the_data_cloudy(self.dsi, clouds_only=True):
+                raise ValueError('Not all required data to consider clouds within '
+                                 'petitRADTRANS are available within the GCM given.')
+            # sort out if input was bool or list
+
         # get profile for each latitude and each terminator
         spectra_list = []
+        output_list = []
+        del_lat = 180/len(self.dsi[c['lat']].values)
         for i, lat in enumerate(self.dsi[c['lat']].values):
             # add morning terminator spectra
-            spectra_list.append(self._get_1_transit_spectra([i, lat], -90, mass_frac, gravity,
-                                                            mmw, rplanet, pressure_0))
+            spectra_list.append(self._get_1_transit_spectra([i, lat], [0, -90], mass_frac, gravity,
+                                                            mmw, rplanet, pressure_0,
+                                                            do_clouds, clouds, use_bruggemann))
+            output_list.append([(-90, (i+0.5)*del_lat - 90), spectra_list[-1]])
 
             # add evening terminator spectra
-            spectra_list.append(self._get_1_transit_spectra([i, lat], 90, mass_frac, gravity,
-                                                            mmw, rplanet, pressure_0))
-
-        # avarage over all profiles (area avaraged)
-        spectra = (np.asarray(spectra_list))**2/len(np.asarray(spectra_list))
-        spectra = np.sqrt(np.sum(spectra, axis=0))
+            spectra_list.append(self._get_1_transit_spectra([i, lat], [1, 90], mass_frac, gravity,
+                                                            mmw, rplanet, pressure_0,
+                                                            do_clouds, clouds, use_bruggemann))
+            output_list.append([(90, (i+0.5)*del_lat - 90), spectra_list[-1]])
 
         # calcualte wavelengths in micron
         wavelengths = 29979245800.0/self.prt.freq/1e-4
+        
+        # calcualte spectra either for each limb seperatly or together
+        if not asymmetric:
+            spectra = (np.asarray(spectra_list))**2/len(np.asarray(spectra_list))
+            spectra = np.sqrt(np.sum(spectra, axis=0))
+        else:
+            spectra = np.zeros((2, len(wavelengths)))
+            for pos, spec in output_list:
+                if pos[0] == -90:
+                    spectra[0, :] += (np.asarray(spec))**2/len(np.asarray(spectra_list))*2
+                else:
+                    spectra[1, :] += (np.asarray(spec))**2/len(np.asarray(spectra_list))*2
+                    
+            spectra = np.sqrt(spectra)
+
 
         # return the final spectra
         return wavelengths, spectra
 
-    def _get_1_transit_spectra(self, lat, lon, mass_frac, gravity, mmw, rplanet, pressure_0):
+    def _get_1_transit_spectra(self, lat, lon, mass_frac, gravity, mmw, rplanet,
+                               pressure_0, do_clouds, clouds, use_bruggemann):
+        """
+        Calculate the transit spectrum. This function avarages T-p profiles in
+        the terminator region and uses poorman equilbriums chemistry.
+
+        Parameters
+        ----------
+        lat: Tuple
+            Tuple containing latitude index and latitude angle.
+        lon: Tuple
+            Tuple containing longitude index and latitude angle.
+        mass_frac: Union[None, List[List[Dict]]]
+            The mass fractions for each t_p point. Structure is as follows: mass_frac[i][j]['key']
+            - i: [2 elements] 0 for morning terminator, 1 for evening terminator
+            - j: [lat_points elements] latitude point starting from lowest
+                 (closeset to lat = -90) to highest (closest to lat = 90)
+            - dict must contain all mass fractions  elements given as opacity species to prt
+        gravity: float
+            surface gravity in !cgs!.
+        mmw: float or 1D-array
+            Mean molecular weight (in atomic units). Will be globally uniform if
+            float or horizonatally uniform if 1D.
+        rplanet: float
+            planet radius in !cm!.
+        pressure_0: float
+            pressure level of the gravity and radius.
+        do_clouds: bool
+            Flag if clouds should be included or not
+        clouds: Union[np.ndarray[i, j, h, w, k], bool]
+            The cloud opacities for each t_p point. Structure is as follows:
+            mass_frac[i][j][w][h][k]
+            - i: [2 elements] 0 for morning terminator, 1 for evening terminator
+            - j: [lat_points elements] latitude point starting from lowest
+                 (closeset to lat = -90) to highest (closest to lat = 90)
+            - w: [number of wavelength bins] this has to be equivalent to the wavelength
+                 structure of prt.
+            - h: [number of pressure points] this needs to be equivalent to the pressure
+                structure of the gcm.
+            - k: 0 for kappa_absorption and 1 for kappa_scatering
+        use_bruggemann: bool
+            If this flag is set to true, bruggemann mixing is used. This is
+            more accurate but takes much longer to calculate.
+
+        Returns
+        -------
+        prt.transmision object
+            petitRADTRAN transmission object
+
+        """
         # get temperature profile
-        temp = self.dsi.sel(lat=lat[1], lon=lon)[c['T']].values
+        temp = self.dsi.sel(lat=lat[1], lon=lon[1])[c['T']].values
 
         # calculate chemistry in mass fractions
         if mass_frac is None:
-            chem = self.chemistry.abunds.sel(lat=lat[1], lon=lon)
+            chem = self.chemistry.abunds.sel(lat=lat[1], lon=lon[1])
             abus = {}
 
             # from xarray to dict
             for key in chem.data_vars:
                 abus[key] = chem[key].values
             del abus['T']
 
             # flip the script
             for key in abus:
                 abus[key] = abus[key][::-1]
         else:
             abus = mass_frac[0][lat[0]]
 
+        # prepare array for cloud data
+        cloud_data = np.zeros((2, len(self.prt.freq), len(self.prt.press)))
+
+        # check if clouds are wished
+        if do_clouds:
+            # adjust prt for clouds
+            self.prt.clouds_mix_opa = types.MethodType(patch_cloud_mix_opa, self.prt)
+            self.prt.calc_transm = types.MethodType(patch_calc_transm, self.prt)
+            self.prt.delete_clouds = types.MethodType(patch_delete_clouds, self.prt)
+
+            # load or calculate cloud opacities
+            if isinstance(clouds, bool):
+                # find all volume fractions
+                vol_fracs = {}
+                for key in self.dsi.keys():
+                    if 'ClVf' in key:
+                        vol_fracs[key[5:]] = self.dsi.sel(lat=lat[1], lon=lon[1])[key].values[::-1]
+
+                # calculate cloud opacities
+                # qabs is the absorption efficiency, qsca the scattering efficiency
+                # and csec the cross-section
+                qabs, qsca, csec = cloud_opacities(
+                    299792458 / self.prt.freq,
+                    self.dsi.sel(lat=lat[1], lon=lon[1])['ClDs'].values[::-1]*1e-6,
+                    self.dsi.sel(lat=lat[1], lon=lon[1])['ClAb'].values[::-1],
+                    self.dsi.sel(lat=lat[1], lon=lon[1])['ClDr'].values[::-1],
+                    vol_fracs,
+                    use_bruggemann
+                    )
+
+                # save opacity kappas
+                for k, _ in enumerate(csec):
+                    cloud_data[0, :, k] = qabs[k] * csec[k]
+                    cloud_data[1, :, k] = qsca[k] * csec[k]
+            else:
+                # load data from input if given
+                cloud_data[0, :, :] = clouds[lon[0], lat[0], :, :, 0]
+                cloud_data[1, :, :] = clouds[lon[0], lat[0], :, :, 1]
+
         # check if all opacity species are in mass fractions
         for key in self.prt.line_species:
             if key not in abus:
                 # if a species is missing, check for partial matches
                 for k_abus in abus:
-                    if k_abus in key:
+                    if k_abus+'_' in key:
                         abus[key] = abus[k_abus]
                         break
                 else:
                     # if a species can not be found fully or partally, give error
                     raise ValueError('Opacity species ' + key + ' missing in mass fraction input')
 
-        # calcualte transmision spectra for the morning terminator of current lat point
-        self.prt.calc_transm(temp[::-1],
-                             abus,
-                             gravity,
-                             mmw*np.ones_like(temp),
-                             R_pl=rplanet,
-                             P0_bar=pressure_0)
+        # calculate transmission spectra for the morning terminator of current lat point
+        if do_clouds:
+            self.prt.calc_transm(temp[::-1], abus, gravity, mmw*np.ones_like(temp),
+                                 R_pl=rplanet, P0_bar=pressure_0, clouds=cloud_data)
+        else:
+            self.prt.calc_transm(temp[::-1], abus, gravity, mmw*np.ones_like(temp),
+                                R_pl=rplanet, P0_bar=pressure_0)
 
         # add the spectra to the list
         return self.prt.transm_rad
 
     def _get_stellar_spec(self, wlen, t_star):
         """
         Helperfunction from petitRADTRANS that calculates the stellar spectrum
@@ -1300,20 +1471,20 @@
             # Write the file:
             # should be written in order of decreasing pressures:
             if p[1] < p[0]:
                 index_order = range(0, len(p))             # write in same order
             elif p[1] > p[0]:
                 index_order = range(len(p)-1, -1, -1)   # write in reverse order
             with open(full_path, 'w') as f:
-                    f.write('! altitude[km]   pressure[bar]   temperature[K]\n')
-                    for k in index_order:
-                        line = '  ' + '{:4.4f}'.format(alt[k]/1000) + '   ' + \
-                                '  ' + '{:1.4E}'.format(p[k]) + '  ' + \
-                                '  ' + '{:4.2f}'.format(T.values[k]) + '\n'
-                        f.write(line)
+                f.write('! altitude[km]   pressure[bar]   temperature[K]\n')
+                for k in index_order:
+                    line = '  ' + '{:4.4f}'.format(alt[k]/1000) + '   ' + \
+                            '  ' + '{:1.4E}'.format(p[k]) + '  ' + \
+                            '  ' + '{:4.2f}'.format(T.values[k]) + '\n'
+                    f.write(line)
             wrt.write_status('INFO', 'File written: ' + full_path)
 
             # Remember the apt-file in a list for easy submission
             with open(destination+'apt_list.txt', 'a') as listfile:
                 listfile.write(model_name + f'_{int(lon)}\n')
 
             # If required, a control plot is saved to show the input data
```

### Comparing `gcm_toolkit-0.3/gcm_toolkit/utils/manipulations.py` & `gcm_toolkit-0.3.1/gcm_toolkit/utils/manipulations.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit/utils/passport.py` & `gcm_toolkit-0.3.1/gcm_toolkit/utils/passport.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
  This file is used to classify input data. All functionalities
  here return a boolean which states True if the given input
  dataset fulfills all the classification requirements of the
  given function. The check for a basic function will raise a
  value error if the conditions are not fulfilled.
 ==============================================================
 """
+import numpy as np
 from ..core import writer as wrt
 from ..core.const import VARNAMES as c
-import numpy as np
 
 
 def is_the_data_basic(dataset):
     """
     Check if the dataset fulfills the minimal requirements for
     a dataset to be used with gcm_toolkit. If not, this function
     raises a Value error.
@@ -166,15 +166,15 @@
             + "not correctly sorted from bottom to top"
             + "therefore does not qualify as a basic GCM dataset.",
         )
 
     return is_the_data_ok
 
 
-def is_the_data_cloudy(dataset):
+def is_the_data_cloudy(dataset, clouds_only=False):
     """
     Check if the dataset fulfills the minimal requirements for
     a dataset to be used with gcm_toolkit.
 
     Parameters
     ----------
     dataset : xarray.Dataset
@@ -183,50 +183,43 @@
     Returns
     -------
     bool
         Returns true if the dataset fulfills the basic
         requirements or False if not.
     """
 
-    # check first if the dataset fulfills the basic requirements
     is_the_data_ok = True
-    if not is_the_data_basic(dataset):
+
+    # check first if the dataset fulfills the basic requirements
+    if not clouds_only and not is_the_data_basic(dataset):
         # variable to check if everything is OK
         is_the_data_ok = False
 
     # get names of all data variables and attributes
     data_variables = list(dataset.keys())
 
     if "ClAb" not in data_variables:
         wrt.write_status(
             "WARN",
             "ClAb (cloud abundance) is missing from the dataset "
             + str(dataset.attrs["tag"]),
         )
         is_the_data_ok = False
 
-    if "ClDr" not in data_variables:
+    if "ClDs" not in data_variables:
         wrt.write_status(
             "WARN",
-            "ClDr (cloud particle radius) is missing from the dataset "
+            "ClDs (cloud particle radius) is missing from the dataset "
             + str(dataset.attrs["tag"]),
         )
         is_the_data_ok = False
 
-    if "ClKs" not in data_variables:
-        wrt.write_status(
-            "WARN",
-            "ClKs (cloud scattering opacity) is missing from the dataset "
-            + str(dataset.attrs["tag"]),
-        )
-        is_the_data_ok = False
-
-    if "ClKa" not in data_variables:
+    if "ClDr" not in data_variables:
         wrt.write_status(
             "WARN",
-            "ClKa (cloud absorption opacity) is missing from the dataset "
+            "ClDr (cloud particle density) is missing from the dataset "
             + str(dataset.attrs["tag"]),
-        )
+            )
         is_the_data_ok = False
 
     # return status of the check
     return is_the_data_ok
```

### Comparing `gcm_toolkit-0.3/gcm_toolkit/utils/read_and_write.py` & `gcm_toolkit-0.3.1/gcm_toolkit/utils/read_and_write.py`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/gcm_toolkit.egg-info/PKG-INFO` & `gcm_toolkit-0.3.1/gcm_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcm-toolkit
-Version: 0.3
+Version: 0.3.1
 Summary: postprocessing stuff
 Home-page: https://github.com/exorad/gcmt
 Author: Aaron David Schneider
 Author-email: aarondavid.schneider@nbi.ku.dk
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `gcm_toolkit-0.3/gcm_toolkit.egg-info/SOURCES.txt` & `gcm_toolkit-0.3.1/gcm_toolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,12 +24,13 @@
 gcm_toolkit/tests/test_gcmtools_common.py
 gcm_toolkit/tests/test_interface.py
 gcm_toolkit/tests/test_manipulations.py
 gcm_toolkit/tests/test_plots.py
 gcm_toolkit/tests/test_utils.py
 gcm_toolkit/tests/test_writer.py
 gcm_toolkit/utils/__init__.py
+gcm_toolkit/utils/clouds.py
 gcm_toolkit/utils/gcm_plotting.py
 gcm_toolkit/utils/interface.py
 gcm_toolkit/utils/manipulations.py
 gcm_toolkit/utils/passport.py
 gcm_toolkit/utils/read_and_write.py
```

### Comparing `gcm_toolkit-0.3/pyproject.toml` & `gcm_toolkit-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gcm_toolkit-0.3/setup.py` & `gcm_toolkit-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "xarray",
     "pyyaml",
     "pre-commit",
 ]
 
 setup(
     name="gcm_toolkit",
-    version="v0.3",
+    version="v0.3.1",
     packages=find_packages(),
     include_package_data=True,
     scripts=["bin/convert_to_gcmt"],
     url="https://github.com/exorad/gcmt",
     license="MIT",
     author="Aaron David Schneider",
     author_email="aarondavid.schneider@nbi.ku.dk",
```

