# Comparing `tmp/appsquared-0.1.1.tar.gz` & `tmp/appsquared-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appsquared-0.1.1.tar", max compression
+gzip compressed data, was "appsquared-1.1.1.tar", max compression
```

## Comparing `appsquared-0.1.1.tar` & `appsquared-1.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1074 2023-05-02 15:57:30.622615 appsquared-0.1.1/LICENSE
--rwxr-xr-x   0        0        0     1082 2023-05-01 19:15:25.904224 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/120loop_check.py
--rwxr-xr-x   0        0        0      987 2023-05-01 19:16:35.781794 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/150loop_check.py
--rwxr-xr-x   0        0        0      971 2023-05-01 19:15:02.928597 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/160loop_check.py
--rwxr-xr-x   0        0        0      983 2023-05-01 19:14:27.655805 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/190loop_check.py
--rw-r--r--   0        0        0      876 2023-05-01 19:10:12.764180 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/Ca_check.py
--rw-r--r--   0        0        0      778 2023-05-01 19:10:22.420578 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/Cb_check.py
--rwxr-xr-x   0        0        0      997 2023-05-01 19:12:16.215665 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/H3_rbs_check.py
--rw-r--r--   0        0        0      788 2023-05-01 19:17:11.244132 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/KM_check.py
--rw-r--r--   0        0        0      812 2023-05-01 19:07:42.142021 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/Sa_check.py
--rw-r--r--   0        0        0      809 2023-05-01 19:07:31.479290 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/Sb_check.py
--rw-r--r--   0        0        0        1 2023-05-02 15:54:18.844626 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/__init__.py
--rw-r--r--   0        0        0      952 2023-05-01 19:22:56.513764 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/contact_diffs.py
--rw-r--r--   0        0        0     5556 2023-05-01 19:12:35.752612 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/glyc.py
--rwxr-xr-x   0        0        0    52846 2023-05-01 19:13:04.444293 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/ligprep_3-sialyl-out.maegz
--rwxr-xr-x   0        0        0    53092 2023-05-01 19:13:20.779405 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/ligprep_6-sialyl-out.maegz
--rw-r--r--   0        0        0  2089310 2023-05-01 19:17:46.083140 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/prep_Darwin_6_2021_trimer.pdb
--rw-r--r--   0        0        0  2706260 2023-05-01 19:17:59.730312 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/prep_Wisconsin_588_trimer.mae
--rw-r--r--   0        0        0  2084309 2023-05-01 19:17:31.294299 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/prep_Wisconsin_588_trimer.pdb
--rw-r--r--   0        0        0      973 2023-05-01 19:10:50.335942 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/rbs_check.py
--rwxr-xr-x   0        0        0     1258 2023-05-01 19:11:19.829156 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/rbs_networked.py
--rwxr-xr-x   0        0        0     7562 2023-05-01 19:20:53.274634 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_Bvic_BCP.sh
--rwxr-xr-x   0        0        0     7291 2023-05-01 19:06:58.945109 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_H1_BCP.sh
--rwxr-xr-x   0        0        0     8260 2023-07-13 21:40:30.722754 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_H3_BCP.sh
--rwxr-xr-x   0        0        0     3107 2023-05-01 19:09:52.292640 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_N2_BCP.sh
--rw-r--r--   0        0        0     2686 2023-05-01 19:21:36.825743 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_contactdiffs.sh
--rwxr-xr-x   0        0        0     1011 2023-05-01 19:21:21.805685 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_contactdiffs_H3.sh
--rw-r--r--   0        0        0      193 2023-05-01 19:31:24.767808 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_glyc.sh
--rw-r--r--   0        0        0      852 2023-05-01 19:09:16.355428 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_rosetta.sh
--rw-r--r--   0        0        0      964 2023-05-01 19:20:30.762454 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_sasa.py
--rw-r--r--   0        0        0      944 2023-05-01 19:06:16.055909 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/sin_check.py
--rw-r--r--   0        0        0      863 2023-05-01 19:08:01.287752 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/siteA_check.py
--rw-r--r--   0        0        0      859 2023-05-01 19:08:11.733634 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/siteB_check.py
--rw-r--r--   0        0        0      856 2023-05-01 19:08:20.790961 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/siteC_check.py
--rw-r--r--   0        0        0      932 2023-05-01 19:08:30.147350 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/siteD_check.py
--rw-r--r--   0        0        0      820 2023-05-01 19:08:45.273748 appsquared-0.1.1/appsquared/src/APPSquared_qxa4/siteE_check.py
--rw-r--r--   0        0        0     1239 2023-07-13 21:50:46.157778 appsquared-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 appsquared-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-02 15:57:30.622615 appsquared-1.1.1/LICENSE
+-rwxr-xr-x   0        0        0     1082 2023-05-01 19:15:25.904224 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/120loop_check.py
+-rwxr-xr-x   0        0        0      987 2023-05-01 19:16:35.781794 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/150loop_check.py
+-rwxr-xr-x   0        0        0      971 2023-05-01 19:15:02.928597 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/160loop_check.py
+-rwxr-xr-x   0        0        0      983 2023-05-01 19:14:27.655805 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/190loop_check.py
+-rw-r--r--   0        0        0      876 2023-05-01 19:10:12.764180 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/Ca_check.py
+-rw-r--r--   0        0        0      778 2023-05-01 19:10:22.420578 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/Cb_check.py
+-rwxr-xr-x   0        0        0      997 2023-05-01 19:12:16.215665 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/H3_rbs_check.py
+-rw-r--r--   0        0        0      788 2023-05-01 19:17:11.244132 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/KM_check.py
+-rw-r--r--   0        0        0      812 2023-05-01 19:07:42.142021 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/Sa_check.py
+-rw-r--r--   0        0        0      809 2023-05-01 19:07:31.479290 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/Sb_check.py
+-rw-r--r--   0        0        0        1 2023-05-02 15:54:18.844626 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/__init__.py
+-rw-r--r--   0        0        0      952 2023-05-01 19:22:56.513764 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/contact_diffs.py
+-rw-r--r--   0        0        0     5587 2023-07-14 18:29:45.849972 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/glyc.py
+-rwxr-xr-x   0        0        0    52846 2023-05-01 19:13:04.444293 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/ligprep_3-sialyl-out.maegz
+-rwxr-xr-x   0        0        0    53092 2023-05-01 19:13:20.779405 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/ligprep_6-sialyl-out.maegz
+-rw-r--r--   0        0        0  2089310 2023-05-01 19:17:46.083140 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/prep_Darwin_6_2021_trimer.pdb
+-rw-r--r--   0        0        0  2706260 2023-05-01 19:17:59.730312 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/prep_Wisconsin_588_trimer.mae
+-rw-r--r--   0        0        0  2084309 2023-05-01 19:17:31.294299 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/prep_Wisconsin_588_trimer.pdb
+-rw-r--r--   0        0        0      973 2023-05-01 19:10:50.335942 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/rbs_check.py
+-rwxr-xr-x   0        0        0     1258 2023-05-01 19:11:19.829156 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/rbs_networked.py
+-rwxr-xr-x   0        0        0     7562 2023-05-01 19:20:53.274634 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_Bvic_BCP.sh
+-rwxr-xr-x   0        0        0     7291 2023-05-01 19:06:58.945109 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_H1_BCP.sh
+-rwxr-xr-x   0        0        0     8260 2023-07-13 21:40:30.722754 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_H3_BCP.sh
+-rwxr-xr-x   0        0        0     3107 2023-05-01 19:09:52.292640 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_N2_BCP.sh
+-rw-r--r--   0        0        0     2686 2023-05-01 19:21:36.825743 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_contactdiffs.sh
+-rwxr-xr-x   0        0        0     1011 2023-05-01 19:21:21.805685 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_contactdiffs_H3.sh
+-rw-r--r--   0        0        0      193 2023-05-01 19:31:24.767808 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_glyc.sh
+-rw-r--r--   0        0        0      852 2023-05-01 19:09:16.355428 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_rosetta.sh
+-rw-r--r--   0        0        0      964 2023-05-01 19:20:30.762454 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_sasa.py
+-rw-r--r--   0        0        0      944 2023-05-01 19:06:16.055909 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/sin_check.py
+-rw-r--r--   0        0        0      863 2023-05-01 19:08:01.287752 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/siteA_check.py
+-rw-r--r--   0        0        0      859 2023-05-01 19:08:11.733634 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/siteB_check.py
+-rw-r--r--   0        0        0      856 2023-05-01 19:08:20.790961 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/siteC_check.py
+-rw-r--r--   0        0        0      932 2023-05-01 19:08:30.147350 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/siteD_check.py
+-rw-r--r--   0        0        0      820 2023-05-01 19:08:45.273748 appsquared-1.1.1/appsquared/src/APPSquared_qxa4/siteE_check.py
+-rw-r--r--   0        0        0     1239 2023-07-14 18:31:02.550498 appsquared-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 appsquared-1.1.1/PKG-INFO
```

### Comparing `appsquared-0.1.1/LICENSE` & `appsquared-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/120loop_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/120loop_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/150loop_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/150loop_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/160loop_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/160loop_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/190loop_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/190loop_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/Ca_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/Ca_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/Cb_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/Cb_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/H3_rbs_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/H3_rbs_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/KM_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/KM_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/Sa_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/Sa_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/Sb_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/Sb_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/contact_diffs.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/contact_diffs.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/glyc.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/glyc.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,8 +103,9 @@
     return structure_df
 ASA = add_dssp_cols(structure,input,gly_dist2)
 output1= pd.DataFrame(ASA)
 #output2= pd.DataFrame(ASA)
 filename1 = input +"gly_ASA_dist.csv"
 #filename2 = input +"ASA_dist.csv"
 output1.to_csv(filename1)
-#output2.to_csv(filename2)
+output1.to_parquet(filename1)
+#output2.to_csv(filename2)
```

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/ligprep_3-sialyl-out.maegz` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/ligprep_3-sialyl-out.maegz`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/ligprep_6-sialyl-out.maegz` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/ligprep_6-sialyl-out.maegz`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/prep_Darwin_6_2021_trimer.pdb` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/prep_Darwin_6_2021_trimer.pdb`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/prep_Wisconsin_588_trimer.mae` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/prep_Wisconsin_588_trimer.mae`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/prep_Wisconsin_588_trimer.pdb` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/prep_Wisconsin_588_trimer.pdb`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/rbs_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/rbs_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/rbs_networked.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/rbs_networked.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_Bvic_BCP.sh` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_Bvic_BCP.sh`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_H1_BCP.sh` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_H1_BCP.sh`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_H3_BCP.sh` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_H3_BCP.sh`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_N2_BCP.sh` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_N2_BCP.sh`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_contactdiffs.sh` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_contactdiffs.sh`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_contactdiffs_H3.sh` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_contactdiffs_H3.sh`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_rosetta.sh` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_rosetta.sh`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/run_sasa.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/run_sasa.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/sin_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/sin_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/siteA_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/siteA_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/siteB_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/siteB_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/siteC_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/siteC_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/siteD_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/siteD_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/appsquared/src/APPSquared_qxa4/siteE_check.py` & `appsquared-1.1.1/appsquared/src/APPSquared_qxa4/siteE_check.py`

 * *Files identical despite different names*

### Comparing `appsquared-0.1.1/pyproject.toml` & `appsquared-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "appsquared"
-version = "0.1.1"
+version = "1.1.1"
 description = "Antigenic Prediction for Protein Sequences Pipeline"
 authors = ["nicole.paterson <qxa4@cdc.gov>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.22.4"
```

### Comparing `appsquared-0.1.1/PKG-INFO` & `appsquared-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appsquared
-Version: 0.1.1
+Version: 1.1.1
 Summary: Antigenic Prediction for Protein Sequences Pipeline
 License: MIT
 Author: nicole.paterson
 Author-email: qxa4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

