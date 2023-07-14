# Comparing `tmp/oxasl-ve-0.2.1.tar.gz` & `tmp/oxasl-ve-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxasl-ve-0.2.1.tar", last modified: Fri Jul 14 12:21:25 2023, max compression
+gzip compressed data, was "oxasl-ve-0.3.0.tar", last modified: Fri Jul 14 12:19:26 2023, max compression
```

## Comparing `oxasl-ve-0.2.1.tar` & `oxasl-ve-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-14 12:21:25.524985 oxasl-ve-0.2.1/
--rw-r--r--   0 martin    (1000) martin    (1000)    10174 2023-07-13 14:15:11.000000 oxasl-ve-0.2.1/LICENSE
--rw-r--r--   0 martin    (1000) martin    (1000)       33 2023-07-13 14:15:11.000000 oxasl-ve-0.2.1/MANIFEST.in
--rw-r--r--   0 martin    (1000) martin    (1000)      975 2023-07-14 12:21:25.524985 oxasl-ve-0.2.1/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      356 2023-07-13 14:15:11.000000 oxasl-ve-0.2.1/README.md
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-14 12:21:25.524985 oxasl-ve-0.2.1/oxasl_ve/
--rw-r--r--   0 martin    (1000) martin    (1000)      642 2023-07-14 11:19:13.000000 oxasl-ve-0.2.1/oxasl_ve/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)       71 2023-07-14 12:21:25.000000 oxasl-ve-0.2.1/oxasl_ve/_version.py
--rw-r--r--   0 martin    (1000) martin    (1000)    21336 2023-07-14 11:21:08.000000 oxasl-ve-0.2.1/oxasl_ve/api.py
--rwxr-xr-x   0 martin    (1000) martin    (1000)    36072 2023-07-13 14:15:11.000000 oxasl-ve-0.2.1/oxasl_ve/modmat_default.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1304 2023-07-14 11:19:13.000000 oxasl-ve-0.2.1/oxasl_ve/veaslc_cli_wrapper.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-14 12:21:25.524985 oxasl-ve-0.2.1/oxasl_ve/wrappers/
--rw-r--r--   0 martin    (1000) martin    (1000)       49 2023-07-13 14:15:11.000000 oxasl-ve-0.2.1/oxasl_ve/wrappers/__init__.py
--rw-r--r--   0 martin    (1000) martin    (1000)     1006 2023-07-13 14:15:11.000000 oxasl-ve-0.2.1/oxasl_ve/wrappers/veaslc.py
-drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2023-07-14 12:21:25.524985 oxasl-ve-0.2.1/oxasl_ve.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)      975 2023-07-14 12:21:25.000000 oxasl-ve-0.2.1/oxasl_ve.egg-info/PKG-INFO
--rw-r--r--   0 martin    (1000) martin    (1000)      388 2023-07-14 12:21:25.000000 oxasl-ve-0.2.1/oxasl_ve.egg-info/SOURCES.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        1 2023-07-14 12:21:25.000000 oxasl-ve-0.2.1/oxasl_ve.egg-info/dependency_links.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       24 2023-07-14 12:21:25.000000 oxasl-ve-0.2.1/oxasl_ve.egg-info/requires.txt
--rw-r--r--   0 martin    (1000) martin    (1000)        9 2023-07-14 12:21:25.000000 oxasl-ve-0.2.1/oxasl_ve.egg-info/top_level.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       25 2023-07-14 11:14:46.000000 oxasl-ve-0.2.1/requirements.txt
--rw-r--r--   0 martin    (1000) martin    (1000)       38 2023-07-14 12:21:25.524985 oxasl-ve-0.2.1/setup.cfg
--rw-r--r--   0 martin    (1000) martin    (1000)     3768 2023-07-13 14:15:11.000000 oxasl-ve-0.2.1/setup.py
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

### Comparing `oxasl-ve-0.2.1/LICENSE` & `oxasl-ve-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.1/PKG-INFO` & `oxasl-ve-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxasl-ve
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python library for manipulating and modelling ASL data
 Home-page: https://oxasl.readthedocs.io/
 Author: Martin Craig
 Author-email: martin.craig@eng.ox.ac.uk
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `oxasl-ve-0.2.1/oxasl_ve/__init__.py` & `oxasl-ve-0.3.0/oxasl_ve/__init__.py`

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

### Comparing `oxasl-ve-0.2.1/oxasl_ve/api.py` & `oxasl-ve-0.3.0/oxasl_ve/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,70 +3,102 @@
 
 Library for processing vessel-encoded ASL data
 
 Copyright (c) 2008-2013 Univerisity of Oxford
 """
 import math
 import traceback
+from optparse import OptionGroup
 
 import numpy as np
 
 from fsl.data.image import Image
 
 from oxasl import basil
-from oxasl.options import OptionCategory, IgnorableOptionGroup
+from oxasl.options import OptionCategory
 from oxasl.reporting import Report
 
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
@@ -215,199 +247,234 @@
     if wsp.infer_loc == "rigid":
         tx, ty, rot = tuple(extras["trans"])
         wsp.log.write("     Translation: %.3g, %.3g  Rotation: %.3g (degrees)\n" % (tx, ty, rot * 180 / math.pi))
     wsp.log.write("   - Class proportions:\n")
     wsp.log.write("     %s\n" % wsp.pis)
 
 def _decode(wsp):
-    if wsp.veasl is None:
-        wsp.sub("veasl")
-
     if wsp.veslocs.ndim != 2 or wsp.veslocs.shape[0] != 2:
         raise ValueError("Vessel locations should have two rows (XY co-ordinates) and one column per vessel")
     
     wsp.log.write("\nPerforming vessel decoding\n")
     wsp.log.write(" - Initial vessel locations:\n")
     wsp.log.write("   X: %s\n" % wsp.veslocs[0, :])
     wsp.log.write("   Y: %s\n" % wsp.veslocs[1, :])
     num_vessels = wsp.veslocs.shape[1]
 
     if wsp.encdef is not None:
-        # Encoding definition supplied by user - assumed to be in MAC format. 
-        wsp.veasl.enc_mac = wsp.encdef
-        wsp.veasl.enc_two, imlist = mac_to_two(wsp.veasl.enc_mac)
+        # Encoding definition supplied by user
+        wsp.log.write("\n - Encoding definition supplied by user in '%s' format\n" % wsp.encdef_format)
+        if wsp.encdef_format == "mac":
+            wsp.enc_mac = wsp.encdef
+            wsp.enc_two, imlist = mac_to_two(wsp.enc_mac)
+        elif wsp.encdef_format == "two":
+            wsp.enc_two = wsp.encdef
+            wsp.enc_mac, imlist = two_to_mac(wsp.enc_two)
+        else:
+            raise ValueError("Unknown encoding definition format: %s" % wsp.encdef_format)
 
         # imlist describes the series of encoded volumes - normally the default is fine
         if wsp.imlist is None:
-            wsp.veasl.imlist = imlist
+            wsp.imlist = imlist
     else:
-        # Auto-generate encoding definition from the initial vessel locations
-        wsp.veasl.enc_two = veslocs_to_enc(wsp.veslocs, wsp.asldata.nenc)
-        wsp.veasl.enc_mac, wsp.veasl.imlist = two_to_mac(wsp.veasl.enc_two)
-    
+        wsp.log.write("\n - Encoding definition will be automatically generated from vessel locations")
+        wsp.enc_two = veslocs_to_enc(wsp.veslocs, wsp.asldata.nenc)
+        wsp.enc_mac, wsp.imlist = two_to_mac(wsp.enc_two)
+
     wsp.log.write("\n - Encoding matrix:\nTWO\n")
-    for row in wsp.veasl.enc_two:
+    for row in wsp.enc_two:
         wsp.log.write("   %s\n" % ", ".join([str(v) for v in row]))
     wsp.log.write("MAC:\n")
-    for row in wsp.veasl.enc_mac:
+    for row in wsp.enc_mac:
         wsp.log.write("   %s\n" % ", ".join([str(v) for v in row]))
 
     # Modulation matrix
     if wsp.modmat is None:
-        wsp.veasl.modmat = modmat_default
-
-    # Set iaf on the workspace so it is always possible to detect when we are using
-    # pairwise subtracted data
-    wsp.veasl.iaf = wsp.asldata.iaf
+        wsp.modmat = modmat_default
 
     # Make sure encoding cycles are together in the data and 
     # average over repeats if required FIXME is this wise/required?
-    wsp.veasl.asldata_mar = wsp.asldata.mean_across_repeats(diff=False).reorder(out_order="lrt")
+    wsp.asldata_mar = wsp.asldata.mean_across_repeats(diff=False).reorder(out_order="lrt")
    
-    wsp.veasl.infer_loc = wsp.ifnone("infer_loc", "rigid")
+    wsp.infer_loc = wsp.ifnone("infer_loc", "rigid")
     if wsp.init_loc and wsp.asldata.ntis > 1:
         wsp.log.write("\n - Doing initial fit for vessel locations using mean data\n")
-        asldata_mean = np.zeros(list(wsp.veasl.asldata_mar.data.shape[:3]) + [wsp.asldata.ntc], dtype=np.float32)
+        asldata_mean = np.zeros(list(wsp.asldata_mar.data.shape[:3]) + [wsp.asldata.ntc], dtype=np.float32)
         for idx in range(wsp.asldata.ntis):
-            asldata_mean += wsp.veasl.asldata_mar[..., idx*wsp.asldata.ntc:(idx+1)*wsp.asldata.ntc]
+            asldata_mean += wsp.asldata_mar[..., idx*wsp.asldata.ntc:(idx+1)*wsp.asldata.ntc]
         asldata_mean /= wsp.asldata.ntis
         asldata_mean = Image(asldata_mean, header=wsp.asldata.header)
 
-        wsp_init = wsp.veasl.sub("init")
+        wsp_init = wsp.sub("init")
         wsp_init.asldata = asldata_mean
 
         _decode_infer(wsp_init)
-        wsp.veasl.veslocs_orig = wsp.veasl.veslocs
-        wsp.veasl.veslocs = wsp_init.veslocs
-        wsp.veasl.infer_loc = wsp.ifnone("infer_loc_pld", "none")
+        wsp.veslocs_orig = wsp.veslocs
+        wsp.veslocs = wsp_init.veslocs
+        wsp.infer_loc = wsp.ifnone("infer_loc_pld", "none")
 
     # Do vessel decoding on each TI/PLD with fixed vessel locations
     for idx in range(wsp.asldata.ntis):
         wsp.log.write("\n - Fitting PLD %i\n" % (idx+1))
-        wsp_ti = wsp.veasl.sub("pld%i" % (idx+1))
-        wsp_ti.asldata = wsp.veasl.asldata_mar.single_ti(idx)
+        wsp_ti = wsp.sub("pld%i" % (idx+1))
+        wsp_ti.asldata = wsp.asldata_mar.single_ti(idx)
         _decode_infer(wsp_ti)
         if wsp.asldata.ntis == 1:
-            wsp.veasl.veslocs_orig = wsp.veasl.veslocs
-            wsp.veasl.veslocs = wsp_ti.veslocs
+            wsp.veslocs_orig = wsp.veslocs
+            wsp.veslocs = wsp_ti.veslocs
 
     wsp.log.write("\nDONE vessel decoding\n")
     return num_vessels
 
 def _model_vessels(wsp, num_vessels):
-    from oxasl import oxford_asl
     wsp.log.write("\nProcessing per-vessel decoded images\n\n")
-    wsp.sub("output")
-
+    
     # Generate per-vessel subtracted images. Note that we multiply the flow by 2. Why?
     #
     # "for a standard ASL sequence, in the label condition we measure S - B (where S is 
     #  static tissue and B is blood signal) and in the control condition we measure S + B, 
     #  so control - label gives us 2B, which is what is normally passed into oxford_asl. 
     #  However, when we explicitly define the encoding matrix and do the decoding, we are 
     #  directly estimating B, rather than 2B, so the output of the decoding is half what 
     #  you would expect from a conventional control - label subtraction."
     #    - Thomas Okell
+    quantify_wsps = []
     for vessel in range(num_vessels):
         wsp.log.write("\n - Processing vessel %i\n" % (vessel+1))
-        wsp_ves = wsp.veasl.sub("vessel%i" % (vessel+1))
+        subname = "basil_vessel%i" % (vessel+1)
+        quantify_wsps.append(subname)
+        wsp_ves = wsp.sub(subname)
         vessel_data = np.zeros(list(wsp.asldata.shape[:3]) + [wsp.asldata.ntis,], dtype=np.float32)
         for ti_idx in range(wsp.asldata.ntis):
             flow = getattr(wsp.veasl, "pld%i" % (ti_idx+1)).flow
             vessel_data[..., ti_idx] = flow.data[..., vessel] * 2
-        vessel_img = wsp.veasl.asldata_mar.derived(vessel_data, iaf="diff", order="rt")
-        wsp_ves.asldata = vessel_img
-        basil.basil(wsp_ves, wsp_ves)
-        subname = "vessel%i" % (vessel+1)
+        wsp_ves.asldata = wsp.veasl.asldata_mar.derived(vessel_data, iaf="diff", order="rt")
+        wsp_ves.iaf = wsp_ves.asldata.iaf
+        basil.fit.run(wsp_ves)
         report = Report("Output for vessel %i" % (vessel+1))
-        oxford_asl.output_native(wsp.output.sub(subname), wsp_ves, report=report)
         wsp.report.add(subname, report)
+    wsp.quantify_wsps = quantify_wsps
 
-def _combine_vessels_sum(wsp, num_vessels, output):
+def _combine_vessels_sum(wsp, num_vessels, basil_output):
     """
     Generate combined vessel output by summing the contributions
     from individual vessels
     
     Used for perfusion data
     """
-    have_output = False
-    all_vessel_img = None
-    for vessel in range(num_vessels):
-        vessel_wsp = getattr(wsp.output, "vessel%i" % (vessel+1))
-        vessel_img = getattr(vessel_wsp.native, output, None)
-        if vessel_img is not None:
-            if all_vessel_img is None:
-                all_vessel_img = np.zeros(vessel_img.shape, dtype=np.float32)
-            all_vessel_img += vessel_img.data
-            have_output = True
-    if have_output:
-        setattr(wsp.output.all_vessels.native, output, Image(all_vessel_img, header=wsp.asldata.header))
+    step = 1
+    all_vessel_step_wsp = None
+    while 1:
+        step_name = "step%i" % step
+        all_vessel_img = None
+        for vessel in range(num_vessels):
+            vessel_wsp = getattr(wsp, "basil_vessel%i" % (vessel+1))
+            step_wsp = getattr(vessel_wsp, step_name, None)
+            if step_wsp is None:
+                break
+            vessel_img = getattr(step_wsp, basil_output, None)
+            if vessel_img is not None:
+                if all_vessel_img is None:
+                    all_vessel_img = np.zeros(vessel_img.shape, dtype=np.float32)
+                all_vessel_img += vessel_img.data
+        if all_vessel_img is not None:
+            all_vessel_step_wsp = getattr(wsp.basil, step_name, None)
+            if all_vessel_step_wsp is None:
+                wsp.basil.sub(step_name)
+                all_vessel_step_wsp = getattr(wsp.basil, step_name)
+            setattr(all_vessel_step_wsp, basil_output, Image(all_vessel_img, header=wsp.asldata.header))
+        if step_wsp is None:
+            break
+        step += 1
+    if wsp.basil.finalstep is None:
+        wsp.basil.finalstep = all_vessel_step_wsp
 
-def _combine_vessels_weighted(wsp, num_vessels, output, method="weightedperf"):
+def _combine_vessels_weighted(wsp, num_vessels, basil_output, method="weightedperf"):
     """
     Generate combined vessel output by summing the contributions
     from individual vessels weighted by voxelwise perfusion
     
     Used for arrival time and variance/std dev
     """
-    vessel_perf = np.zeros(list(wsp.asldata.shape[:3]) + [num_vessels,], dtype=np.float32)
-    vessel_output = np.zeros(list(wsp.asldata.shape[:3]) + [num_vessels,], dtype=np.float32)
-    have_output = False
-    for vessel in range(num_vessels):
-        vessel_wsp = getattr(wsp.output, "vessel%i" % (vessel+1))
-        vessel_img = getattr(vessel_wsp.native, output, None)
-        if vessel_img is not None:
-            vessel_perf[..., vessel] = vessel_wsp.native.perfusion.data
-            vessel_output[..., vessel] = vessel_img.data
-            have_output = True
-
-    if have_output:
-        if method == "singleperf":
-            # This selects the arrival time from a single vessel with highest perfusion
-            best_vessel = np.argmax(vessel_perf, -1)
-            shape3d, t = vessel_output.shape[:-1], vessel_output.shape[-1]
-            flat = vessel_output.reshape(-1, t)[np.arange(np.prod(shape3d)), best_vessel.ravel()]
-            all_vessel_output = flat.reshape(shape3d)
-            wsp.output.all_vessels.native.best_vessel = Image(best_vessel+1, header=wsp.asldata.header)
-        elif method == "weightedperf":
-            # Tests the arrival time from a weighted average of vessels weighted by perfusion. Note that
-            # we need to protect against divide by zero
-            total_perf = wsp.output.all_vessels.native.perfusion.data
-            total_perf[total_perf == 0] = 1
-            all_vessel_output = np.nan_to_num(np.sum(vessel_perf * vessel_output, axis=-1) / total_perf)
-        #elif combine_method == "weightedprob":
-        #    # Sets the arrival time as a weighted average by vessel probability FIXME not working right now
-        #    all_vessel_output = np.sum(prob * vessel_arrival, axis=-1)
-        else:
-            raise ValueError("Unrecognized combination method for weighted combination: %s" % method)
-        setattr(wsp.output.all_vessels.native, output, Image(all_vessel_output, header=wsp.asldata.header))
+    step = 1
+    all_vessel_step_wsp = None
+    while 1:
+        step_name = "step%i" % step
+        all_vessel_img = None
+
+        vessel_perf = np.zeros(list(wsp.asldata.shape[:3]) + [num_vessels,], dtype=np.float32)
+        vessel_output = np.zeros(list(wsp.asldata.shape[:3]) + [num_vessels,], dtype=np.float32)
+        have_output = False
+        for vessel in range(num_vessels):
+            vessel_wsp = getattr(wsp, "basil_vessel%i" % (vessel+1))
+            step_wsp = getattr(vessel_wsp, step_name, None)
+            if step_wsp is None:
+                break
+            vessel_img = getattr(step_wsp, basil_output, None)
+            if vessel_img is not None:
+                vessel_perf[..., vessel] = vessel_wsp.finalstep.mean_ftiss.data
+                vessel_output[..., vessel] = vessel_img.data
+                have_output = True
+
+        if have_output:
+            all_vessel_step_wsp = getattr(wsp.basil, step_name, None)
+            if all_vessel_step_wsp is None:
+                wsp.basil.sub(step_name)
+                all_vessel_step_wsp = getattr(wsp.basil, step_name)
+
+            if method == "singleperf":
+                # This selects the arrival time from a single vessel with highest perfusion
+                best_vessel = np.argmax(vessel_perf, -1)
+                shape3d, t = vessel_output.shape[:-1], vessel_output.shape[-1]
+                flat = vessel_output.reshape(-1, t)[np.arange(np.prod(shape3d)), best_vessel.ravel()]
+                all_vessel_img = flat.reshape(shape3d)
+                all_vessel_step_wsp.best_vessel = Image(best_vessel+1, header=wsp.asldata.header)
+            elif method == "weightedperf":
+                # Tests the arrival time from a weighted average of vessels weighted by perfusion. Note that
+                # we need to protect against divide by zero
+                total_perf = wsp.basil.finalstep.mean_ftiss.data
+                total_perf[total_perf <= 0] = 1
+                all_vessel_img = np.nan_to_num(np.sum(vessel_perf * vessel_output, axis=-1) / total_perf)
+            #elif combine_method == "weightedprob":
+            #    # Sets the arrival time as a weighted average by vessel probability FIXME not working right now
+            #    all_vessel_output = np.sum(prob * vessel_arrival, axis=-1)
+            else:
+                raise ValueError("Unrecognized combination method for weighted combination: %s" % method)
+            setattr(all_vessel_step_wsp, basil_output, Image(all_vessel_img, header=wsp.asldata.header))
+        if step_wsp is None:
+            break
+        step += 1
+    if wsp.basil.finalstep is None:
+        wsp.basil.finalstep = all_vessel_step_wsp
 
 def _combine_vessels(wsp, num_vessels):
     """
     Generate combined output for all vessels
     """
-    from oxasl import oxford_asl
     wsp.log.write("\nGenerating combined images for all vessels\n\n")
+    wsp.sub("basil")
 
     # Generate combined perfusion and aCBV maps over all vessels
-    wsp.output.sub("all_vessels")
-    wsp.output.all_vessels.sub("native")
-    for otype in ("", "_calib", "_std", "_var", "_std_calib", "_var_calib"):
-        for oname in ("perfusion", "aCBV", "modelfit", "arrival"):
-            output = "%s%s" % (oname, otype)
-            if oname != "arrival" and otype  in ("", "_calib"):
-                _combine_vessels_sum(wsp, num_vessels, output)                
+    for otype in ("", "mean_", "std_"):
+        for oname in ("ftiss", "fblood", "modelfit", "delttiss", "deltblood"):
+            basil_output = "%s%s" % (otype, oname)
+            if not oname.startswith("delt") and otype  in ("", "mean_"):
+                _combine_vessels_sum(wsp, num_vessels, basil_output)                
             else:
-                _combine_vessels_weighted(wsp, num_vessels, output, method=wsp.ifnone("arrival_combine", "weightedperf"))
+                _combine_vessels_weighted(wsp, num_vessels, basil_output, method=wsp.ifnone("arrival_combine", "weightedperf"))
+
+    # All Basil-type directories must save the analysis mask
+    wsp.basil.analysis_mask = wsp.basil_vessel1.analysis_mask
 
-    report = Report("Combined output for all vessels")
-    oxford_asl.output_report(wsp.output.all_vessels.native, report=report)
-    wsp.report.add("all_vessels", report)
+    #report = Report("Combined output for all vessels")
+    #oxford_asl.output_report(wsp.output.all_vessels.native, report=report)
+    #wsp.report.add("all_vessels", report)
+    wsp.quantify_wsps.append("basil")
 
-def model_ve(wsp):
+def run(wsp):
     """
     Do vessel decoding and modelling on vessel-encoded ASL data
 
     :param wsp: Workspace object
 
     Required workspace attributes
     -----------------------------
@@ -441,52 +508,48 @@
       - ``veasl.vessel<n>``    - Sub workspace containing model fitting output for vessel 
                                  <n> at all PLDs
       - ``output.vessel<n>``   - Sub workspace containing native/structural/standard space 
                                  parameter maps for vessel <n>
       - ``output.all_vessels`` - Sub workspace containing native/structural/standard space 
                                  parameter maps for all vessels combined
     """
-    from oxasl import oxford_asl
-
-    num_vessels = _decode(wsp)
+    num_vessels = _decode(wsp.sub("veasl"))
     _model_vessels(wsp, num_vessels)
     _combine_vessels(wsp, num_vessels)
 
-    # Re-do registration using all-vessel PWI map.
-    oxford_asl.redo_reg(wsp, wsp.output.all_vessels.native.perfusion)
-
-    oxford_asl.output_trans(wsp.output.all_vessels)
-
     wsp.log.write("\nDONE processing\n")
 
-class VeaslOptions(OptionCategory):
+class Options(OptionCategory):
     """
     OptionCategory which contains options for preprocessing ASL data
     """
 
     def __init__(self, **kwargs):
         OptionCategory.__init__(self, "oxasl_ve", **kwargs)
 
     def groups(self, parser):
         ret = []
-        g = IgnorableOptionGroup(parser, "VEASL Options")
+        g = OptionGroup(parser, "VEASL Options")
         g.add_option("--veslocs", help="Vessel locations file", type="matrix")
         g.add_option("--nfpc", help="Number of flows per class", type="int", default=2)
         g.add_option("--veasl-method", help="VEASL inference method", choices=["map", "mcmc"], default="map")
         g.add_option("--infer-v", help="Infer flow velocity", action="store_true", default=False)
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
+        g.add_option("--encdef", help="Encoding definition file", type="matrix")
+        g.add_option("--encdef-format", help="Encoding definition file format", default="mac")
         g.add_option("--arrival-combine", help="Method for combining arrival time maps", choices=["weightedperf", "singleperf"], default="weightedperf")
         ret.append(g)
-        g = IgnorableOptionGroup(parser, "VEASL options for --method=mcmc")
+        g = OptionGroup(parser, "VEASL options for --method=mcmc")
         g.add_option("--njumps", help="Number of parameter jumps", type="int", default=500)
         g.add_option("--burnin", help="Number of jumps before sampling begins", type="int", default=10)
         g.add_option("--sample-every", help="Sampling frequency in jumps", type="int", default=1)
         ret.append(g)
         return ret
```

### Comparing `oxasl-ve-0.2.1/oxasl_ve/modmat_default.py` & `oxasl-ve-0.3.0/oxasl_ve/modmat_default.py`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.1/oxasl_ve/wrappers/veaslc.py` & `oxasl-ve-0.3.0/oxasl_ve/wrappers/veaslc.py`

 * *Files identical despite different names*

### Comparing `oxasl-ve-0.2.1/oxasl_ve.egg-info/PKG-INFO` & `oxasl-ve-0.3.0/oxasl_ve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxasl-ve
-Version: 0.2.1
+Version: 0.3.0
 Summary: Python library for manipulating and modelling ASL data
 Home-page: https://oxasl.readthedocs.io/
 Author: Martin Craig
 Author-email: martin.craig@eng.ox.ac.uk
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `oxasl-ve-0.2.1/setup.py` & `oxasl-ve-0.3.0/setup.py`

 * *Files identical despite different names*

