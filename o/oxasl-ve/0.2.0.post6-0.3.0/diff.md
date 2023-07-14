# Comparing `tmp/oxasl-ve-0.2.0.post6.tar.gz` & `tmp/oxasl-ve-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxasl-ve-0.2.0.post6.tar", last modified: Wed Jul 12 12:35:27 2023, max compression
+gzip compressed data, was "oxasl-ve-0.3.0.tar", last modified: Fri Jul 14 12:19:26 2023, max compression
```

## Comparing `oxasl-ve-0.2.0.post6.tar` & `oxasl-ve-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-12 12:35:27.758793 oxasl-ve-0.2.0.post6/
--rw-r--r--   0 martin    (1000) martin    (1000)    10174 2022-11-15 15:47:48.000000 oxasl-ve-0.2.0.post6/LICENSE
--rw-r--r--   0 martin    (1000) martin    (1000)       33 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post6/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)      981 2023-07-12 12:35:27.748793 oxasl-ve-0.2.0.post6/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      356 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post6/README.md
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-12 12:35:27.748793 oxasl-ve-0.2.0.post6/oxasl_ve/
--rw-r--r--   0 martin    (1000) martin    (1000)      642 2023-07-12 12:33:06.000000 oxasl-ve-0.2.0.post6/oxasl_ve/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)       77 2023-07-12 12:35:27.000000 oxasl-ve-0.2.0.post6/oxasl_ve/_version.py
--rw-r--r--   0 martin    (1000) martin    (1000)    22544 2023-07-12 12:32:40.000000 oxasl-ve-0.2.0.post6/oxasl_ve/api.py
--rwxr-xr-x   0 martin    (1000) martin    (1000)    36072 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post6/oxasl_ve/modmat_default.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1845 2023-07-11 12:08:12.000000 oxasl-ve-0.2.0.post6/oxasl_ve/veaslc_cli_wrapper.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-12 12:35:27.748793 oxasl-ve-0.2.0.post6/oxasl_ve/wrappers/
--rw-r--r--   0 martin    (1000) martin    (1000)       49 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post6/oxasl_ve/wrappers/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1006 2022-04-05 13:55:39.000000 oxasl-ve-0.2.0.post6/oxasl_ve/wrappers/veaslc.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-12 12:35:27.748793 oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)      981 2023-07-12 12:35:27.000000 oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      388 2023-07-12 12:35:27.000000 oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/SOURCES.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-07-12 12:35:27.000000 oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/dependency_links.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       24 2023-07-12 12:35:27.000000 oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/requires.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        9 2023-07-12 12:35:27.000000 oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/top_level.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       25 2023-07-11 12:03:38.000000 oxasl-ve-0.2.0.post6/requirements.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       38 2023-07-12 12:35:27.758793 oxasl-ve-0.2.0.post6/setup.cfg
--rw-r--r--   0 martin    (1000) martin    (1000)     3768 2022-11-15 15:47:48.000000 oxasl-ve-0.2.0.post6/setup.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-14 12:19:26.634900 oxasl-ve-0.3.0/
+-rw-r--r--   0 martin    (1000) martin    (1000)    10174 2022-11-15 15:47:48.000000 oxasl-ve-0.3.0/LICENSE
+-rw-r--r--   0 martin    (1000) martin    (1000)       33 2022-04-05 13:55:39.000000 oxasl-ve-0.3.0/MANIFEST.in
+-rw-r--r--   0 martin    (1000) martin    (1000)      975 2023-07-14 12:19:26.634900 oxasl-ve-0.3.0/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      356 2022-04-05 13:55:39.000000 oxasl-ve-0.3.0/README.md
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-14 12:19:26.634900 oxasl-ve-0.3.0/oxasl_ve/
+-rw-r--r--   0 martin    (1000) martin    (1000)      622 2023-07-14 09:57:28.000000 oxasl-ve-0.3.0/oxasl_ve/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)       70 2023-07-14 12:19:26.000000 oxasl-ve-0.3.0/oxasl_ve/_version.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    24046 2023-07-14 09:57:28.000000 oxasl-ve-0.3.0/oxasl_ve/api.py
+-rwxr-xr-x   0 martin    (1000) martin    (1000)    36072 2022-04-05 13:55:39.000000 oxasl-ve-0.3.0/oxasl_ve/modmat_default.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1845 2023-07-11 12:08:12.000000 oxasl-ve-0.3.0/oxasl_ve/veaslc_cli_wrapper.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-14 12:19:26.634900 oxasl-ve-0.3.0/oxasl_ve/wrappers/
+-rw-r--r--   0 martin    (1000) martin    (1000)       49 2022-04-05 13:55:39.000000 oxasl-ve-0.3.0/oxasl_ve/wrappers/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     1006 2022-04-05 13:55:39.000000 oxasl-ve-0.3.0/oxasl_ve/wrappers/veaslc.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-14 12:19:26.634900 oxasl-ve-0.3.0/oxasl_ve.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)      975 2023-07-14 12:19:26.000000 oxasl-ve-0.3.0/oxasl_ve.egg-info/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      388 2023-07-14 12:19:26.000000 oxasl-ve-0.3.0/oxasl_ve.egg-info/SOURCES.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-07-14 12:19:26.000000 oxasl-ve-0.3.0/oxasl_ve.egg-info/dependency_links.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       29 2023-07-14 12:19:26.000000 oxasl-ve-0.3.0/oxasl_ve.egg-info/requires.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        9 2023-07-14 12:19:26.000000 oxasl-ve-0.3.0/oxasl_ve.egg-info/top_level.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       30 2023-07-14 09:57:28.000000 oxasl-ve-0.3.0/requirements.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       38 2023-07-14 12:19:26.634900 oxasl-ve-0.3.0/setup.cfg
+-rw-r--r--   0 martin    (1000) martin    (1000)     3768 2022-11-15 15:47:48.000000 oxasl-ve-0.3.0/setup.py
```

### Comparing `oxasl-ve-0.2.0.post6/LICENSE` & `oxasl-ve-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post6/PKG-INFO` & `oxasl-ve-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxasl-ve
-Version: 0.2.0.post6
+Version: 0.3.0
 Summary: Python library for manipulating and modelling ASL data
 Home-page: https://oxasl.readthedocs.io/
 Author: Martin Craig
 Author-email: martin.craig@eng.ox.ac.uk
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `oxasl-ve-0.2.0.post6/oxasl_ve/__init__.py` & `oxasl-ve-0.3.0/oxasl_ve/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 If installed, then it will be called by ``oxasl.oxford_asl.oxasl``
 whenever vessel-encoded data is supplied.
 
 The relevant processing function can also be called independently
 on a ``Workspace`` object, however this will not include the
 standard oxasl preprocessing or registration.
 """
-from .api import model_ve, VeaslOptions, two_to_mac, mac_to_two, veslocs_to_enc, generate_mask
+from .api import run, Options, two_to_mac, mac_to_two, veslocs_to_enc, generate_mask
 from ._version import __version__
 
-__all__ = ["__version__", "model_ve", "VeaslOptions", "two_to_mac", "mac_to_two", "veslocs_to_enc", "generate_mask"]
+__all__ = ["__version__", "run", "Options", "two_to_mac", "mac_to_two", "veslocs_to_enc", "generate_mask"]
```

### Comparing `oxasl-ve-0.2.0.post6/oxasl_ve/api.py` & `oxasl-ve-0.3.0/oxasl_ve/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,54 +20,85 @@
 from ._version import __version__
 from .veaslc_cli_wrapper import veaslc_wrapper
 from .modmat_default import modmat_default
 
 def veslocs_to_enc(veslocs, nvols=8):
     """
     Automatically generate an encoding scheme matrix given initial vessel locations
+
+    :param veslocs: Numpy array of vessel locations each column is vessel and row
+                    1 is X values, row 2 is y values
     """      
-    if nvols not in (6, 8):
-        raise ValueError("Auto-generation of encoding matrix only supported for 6 or 8 encoding cycles")
+    if nvols not in (6, 8, 12):
+        raise ValueError("Auto-generation of encoding matrix only supported for 6, 8 or 12 encoding cycles")
 
     num_vessels = veslocs.shape[-1]
-    if num_vessels != 4:
-        raise ValueError("Auto-generation of encoding matrix only supported with 4 inferred vessels")
+    if nvols in (6, 8) and num_vessels != 4:
+        raise ValueError("6 and 8 cycle encoding requires 4 vessel locations")
+    elif nvols == 12 and num_vessels != 6:
+        raise RuntimeError("12 cycle encoding requires 6 vessel locations")
 
     try:
         lr1, lr2 = veslocs[0, 0], veslocs[0, 1]
         ap1, ap2 = np.mean(veslocs[1, :2]), np.mean(veslocs[1, 2:])
         two = [
             [0, 0, 0, 0],
             [0, 1, 0, 0],
             [90, 2, lr1, lr2],
             [90, 3, lr1, lr2],
             [0, 2, ap1, ap2],
             [0, 3, ap1, ap2],
         ]
-        if nvols == 8:
+        if nvols > 6:
             # Vector from RC to LV
-            LV_minus_RC = veslocs[:2, 3] - veslocs[:2, 0]
+            LV_minus_RC = veslocs[:, 3] - veslocs[:, 0]
 
             # Want to tag RC and LV simultaneously - gradient angle required
             # is acos[normalised(LV - RC).x]
             tag_rad = math.acos(LV_minus_RC[0] / np.linalg.norm(LV_minus_RC))
             tag_deg = math.degrees(tag_rad)
 
             # Unit vector in gradient direction
             G = [math.sin(tag_rad), math.cos(tag_rad)]
 
             # Calculate distance from isocentre to each vessel
             # Dot product of location with gradient unit vector
-            isodist = [sum(veslocs[:2, v] * G) for v in range(num_vessels)]
+            isodist = [np.dot(veslocs[:, v], G) for v in range(num_vessels)]
             vA = (isodist[0] + isodist[3])/2
             vB = vA + (abs(vA -isodist[1]) + abs(vA - isodist[2]))/2
             two += [
                 [tag_deg, 2, vA, vB],
                 [tag_deg, 3, vA, vB],
             ]
+        if nvols == 12:
+            # 9 and 10: RICA vs RECA
+            RC_minus_REC = veslocs[:, 0] - veslocs[:, 4]
+            tag_rad = math.acos(RC_minus_REC[0] / np.linalg.norm(RC_minus_REC))
+            tag_deg = math.degrees(tag_rad)
+           
+            # Calculate distances from isocentre in this direction
+            # Note that isodist has already been defined above
+            vA9and10 = isodist[4] # RECA
+            vB9and10 = isodist[0] # RICA
+            two += [
+                [tag_deg, 2, vA9and10, vB9and10],
+                [tag_deg, 3, vA9and10, vB9and10],
+            ]
+
+            # 11 and 12: LICA vs LECA as above
+            LEC_minus_LC = veslocs[:, 5] - veslocs[:, 1]
+            tag_rad = math.acos(LEC_minus_LC[0] / np.linalg.norm(LEC_minus_LC))
+            tag_deg = math.degrees(tag_rad)
+            
+            vA11and12 = isodist[1] # LICA
+            vB11and12 = isodist[5] # LECA
+            two += [
+                [tag_deg, 2, vA11and12, vB11and12],
+                [tag_deg, 3, vA11and12, vB11and12],
+            ]
 
         return np.array(two, dtype=np.float32)
     except: 
         traceback.print_exc()
         raise RuntimeError("Error generating encoding matrix from vessel locations. Check your vessel locations file.")
 
 def two_to_mac(two):
@@ -302,30 +333,30 @@
     # "for a standard ASL sequence, in the label condition we measure S - B (where S is 
     #  static tissue and B is blood signal) and in the control condition we measure S + B, 
     #  so control - label gives us 2B, which is what is normally passed into oxford_asl. 
     #  However, when we explicitly define the encoding matrix and do the decoding, we are 
     #  directly estimating B, rather than 2B, so the output of the decoding is half what 
     #  you would expect from a conventional control - label subtraction."
     #    - Thomas Okell
-    basildirs = []
+    quantify_wsps = []
     for vessel in range(num_vessels):
         wsp.log.write("\n - Processing vessel %i\n" % (vessel+1))
         subname = "basil_vessel%i" % (vessel+1)
-        basildirs.append("vessel%i" % (vessel+1))
+        quantify_wsps.append(subname)
         wsp_ves = wsp.sub(subname)
         vessel_data = np.zeros(list(wsp.asldata.shape[:3]) + [wsp.asldata.ntis,], dtype=np.float32)
         for ti_idx in range(wsp.asldata.ntis):
             flow = getattr(wsp.veasl, "pld%i" % (ti_idx+1)).flow
             vessel_data[..., ti_idx] = flow.data[..., vessel] * 2
         wsp_ves.asldata = wsp.veasl.asldata_mar.derived(vessel_data, iaf="diff", order="rt")
         wsp_ves.iaf = wsp_ves.asldata.iaf
-        basil.basil(wsp_ves)
+        basil.fit.run(wsp_ves)
         report = Report("Output for vessel %i" % (vessel+1))
         wsp.report.add(subname, report)
-    wsp.basildirs = basildirs
+    wsp.quantify_wsps = quantify_wsps
 
 def _combine_vessels_sum(wsp, num_vessels, basil_output):
     """
     Generate combined vessel output by summing the contributions
     from individual vessels
     
     Used for perfusion data
@@ -419,29 +450,31 @@
     """
     Generate combined output for all vessels
     """
     wsp.log.write("\nGenerating combined images for all vessels\n\n")
     wsp.sub("basil")
 
     # Generate combined perfusion and aCBV maps over all vessels
-    wsp.sub("basil")
     for otype in ("", "mean_", "std_"):
         for oname in ("ftiss", "fblood", "modelfit", "delttiss", "deltblood"):
             basil_output = "%s%s" % (otype, oname)
             if not oname.startswith("delt") and otype  in ("", "mean_"):
                 _combine_vessels_sum(wsp, num_vessels, basil_output)                
             else:
                 _combine_vessels_weighted(wsp, num_vessels, basil_output, method=wsp.ifnone("arrival_combine", "weightedperf"))
 
+    # All Basil-type directories must save the analysis mask
+    wsp.basil.analysis_mask = wsp.basil_vessel1.analysis_mask
+
     #report = Report("Combined output for all vessels")
     #oxford_asl.output_report(wsp.output.all_vessels.native, report=report)
     #wsp.report.add("all_vessels", report)
-    wsp.basildirs.append("")
+    wsp.quantify_wsps.append("basil")
 
-def model_ve(wsp):
+def run(wsp):
     """
     Do vessel decoding and modelling on vessel-encoded ASL data
 
     :param wsp: Workspace object
 
     Required workspace attributes
     -----------------------------
@@ -481,15 +514,15 @@
     """
     num_vessels = _decode(wsp.sub("veasl"))
     _model_vessels(wsp, num_vessels)
     _combine_vessels(wsp, num_vessels)
 
     wsp.log.write("\nDONE processing\n")
 
-class VeaslOptions(OptionCategory):
+class Options(OptionCategory):
     """
     OptionCategory which contains options for preprocessing ASL data
     """
 
     def __init__(self, **kwargs):
         OptionCategory.__init__(self, "oxasl_ve", **kwargs)
 
@@ -503,14 +536,15 @@
         g.add_option("--infer-loc", help="Vessel location inference method to use. For multi-pld data can also infer vessel locations individually using --infer-loc-pld", choices=["none", "xy", "rigid", "affine"], default="rigid")
         g.add_option("--init-loc", help="For multi-PLD data, initialise vessel locations by fitting with mean data", action="store_true", default=False)
         g.add_option("--infer-loc-pld", help="For multi-PLD data when --init-loc is specified, this specifies an optional additional vessel location inference method during individual PLD fitting.", choices=["none", "xy", "rigid", "affine"], default="none")
         g.add_option("--xy-std", help="Prior standard deviation for vessel positions", type="float", default=1.0)
         g.add_option("--rot-std", help="Prior standard deviation for rotation angle (degrees) if using rigid body inference", type="float", default=1.2)
         g.add_option("--v-mean", help="Prior mean flow velocity if using --infer-v", type="float", default=0.3)
         g.add_option("--v-std", help="Prior standard deviation for flow velocity if using --infer-v", type="float", default=0.01)
+        g.add_option("--infer-mask", help="Inference mask", type="image")
         g.add_option("--infer-mask-frac", help="Fraction of 99th percentile to use when generating inference mask", type="float", default=0.5)
         g.add_option("--modmat", help="Modulation matrix file")
         g.add_option("--encdef", help="Encoding definition file", type="matrix")
         g.add_option("--encdef-format", help="Encoding definition file format", default="mac")
         g.add_option("--arrival-combine", help="Method for combining arrival time maps", choices=["weightedperf", "singleperf"], default="weightedperf")
         ret.append(g)
         g = OptionGroup(parser, "VEASL options for --method=mcmc")
```

### Comparing `oxasl-ve-0.2.0.post6/oxasl_ve/modmat_default.py` & `oxasl-ve-0.3.0/oxasl_ve/modmat_default.py`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post6/oxasl_ve/veaslc_cli_wrapper.py` & `oxasl-ve-0.3.0/oxasl_ve/veaslc_cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post6/oxasl_ve/wrappers/veaslc.py` & `oxasl-ve-0.3.0/oxasl_ve/wrappers/veaslc.py`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.0.post6/oxasl_ve.egg-info/PKG-INFO` & `oxasl-ve-0.3.0/oxasl_ve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxasl-ve
-Version: 0.2.0.post6
+Version: 0.3.0
 Summary: Python library for manipulating and modelling ASL data
 Home-page: https://oxasl.readthedocs.io/
 Author: Martin Craig
 Author-email: martin.craig@eng.ox.ac.uk
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `oxasl-ve-0.2.0.post6/setup.py` & `oxasl-ve-0.3.0/setup.py`

 * *Files identical despite different names*

