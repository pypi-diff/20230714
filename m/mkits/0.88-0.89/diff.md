# Comparing `tmp/mkits-0.88-py3-none-any.whl.zip` & `tmp/mkits-0.89-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -3,21 +3,21 @@
 -rw-rw-r--  2.0 unx     5820 b- defN 23-Jun-12 08:42 mkits/boltz.py
 -rw-rw-r--  2.0 unx    55870 b- defN 23-Jun-22 08:16 mkits/builder.py
 -rw-rw-r--  2.0 unx     5669 b- defN 23-Jun-12 08:42 mkits/critic2.py
 -rw-rw-r--  2.0 unx    21610 b- defN 23-Jul-13 18:54 mkits/database.py
 -rw-rw-r--  2.0 unx     2750 b- defN 23-Jun-12 08:42 mkits/fdmnes.py
 -rw-rw-r--  2.0 unx    46998 b- defN 23-Jul-14 19:04 mkits/globle.py
 -rw-rw-r--  2.0 unx      603 b- defN 23-Jun-12 08:42 mkits/gui.py
--rw-rw-r--  2.0 unx    20366 b- defN 23-Jul-14 19:07 mkits/main.py
+-rw-rw-r--  2.0 unx    20366 b- defN 23-Jul-14 19:14 mkits/main.py
 -rw-rw-r--  2.0 unx    28640 b- defN 23-Jun-12 08:42 mkits/qe.py
 -rw-rw-r--  2.0 unx    11851 b- defN 23-Jun-12 08:42 mkits/structgen.py
 -rw-rw-r--  2.0 unx      586 b- defN 23-Jun-12 08:42 mkits/sysfc.py
 -rw-rw-r--  2.0 unx       70 b- defN 23-Jun-12 08:42 mkits/test.py
 -rw-rw-r--  2.0 unx    86844 b- defN 23-Jul-13 19:00 mkits/vasp.py
 -rw-rw-r--  2.0 unx     6046 b- defN 23-Jun-12 08:42 mkits/wien.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Jul-14 19:07 mkits-0.88.dist-info/LICENSE
--rw-rw-r--  2.0 unx      746 b- defN 23-Jul-14 19:07 mkits-0.88.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-14 19:07 mkits-0.88.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Jul-14 19:07 mkits-0.88.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-14 19:07 mkits-0.88.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1534 b- defN 23-Jul-14 19:07 mkits-0.88.dist-info/RECORD
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jul-14 19:14 mkits-0.89.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      746 b- defN 23-Jul-14 19:14 mkits-0.89.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-14 19:14 mkits-0.89.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Jul-14 19:14 mkits-0.89.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-14 19:14 mkits-0.89.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1534 b- defN 23-Jul-14 19:14 mkits-0.89.dist-info/RECORD
 21 files, 297268 bytes uncompressed, 65983 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -39,26 +39,26 @@
 
 Filename: mkits/vasp.py
 Comment: 
 
 Filename: mkits/wien.py
 Comment: 
 
-Filename: mkits-0.88.dist-info/LICENSE
+Filename: mkits-0.89.dist-info/LICENSE
 Comment: 
 
-Filename: mkits-0.88.dist-info/METADATA
+Filename: mkits-0.89.dist-info/METADATA
 Comment: 
 
-Filename: mkits-0.88.dist-info/WHEEL
+Filename: mkits-0.89.dist-info/WHEEL
 Comment: 
 
-Filename: mkits-0.88.dist-info/entry_points.txt
+Filename: mkits-0.89.dist-info/entry_points.txt
 Comment: 
 
-Filename: mkits-0.88.dist-info/top_level.txt
+Filename: mkits-0.89.dist-info/top_level.txt
 Comment: 
 
-Filename: mkits-0.88.dist-info/RECORD
+Filename: mkits-0.89.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mkits/main.py

```diff
@@ -136,15 +136,15 @@
 def parse_arguments():
     parser = argparse.ArgumentParser(
         description="DFT helper"
     )
     parser.add_argument(
         "--version",
         action="version",
-        version="0.88",
+        version="0.89",
         help="print version information"
     )
     subparser = parser.add_subparsers(
         help="sub command:"
     )
     # ==========================================================================
     # subparser
```

## Comparing `mkits-0.88.dist-info/LICENSE` & `mkits-0.89.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mkits-0.88.dist-info/METADATA` & `mkits-0.89.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkits
-Version: 0.88
+Version: 0.89
 Summary: multi-DFT codes assistant program.
 Home-page: https://github.com/leon-venir/mkits
 Download-URL: https://github.com/leon-venir/mkits
 Author: Leon Ma
 Author-email: blustery.med@hotmail.com
 License: GPLv3+
 Keywords: DFT code assistant
```

## Comparing `mkits-0.88.dist-info/RECORD` & `mkits-0.89.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 mkits/boltz.py,sha256=5AOim-BK3FttzNm2kOMl_wyYv60HW3mvIzFs_yRdUG8,5820
 mkits/builder.py,sha256=DPJFfsyQHSyo_XAcqkdfYvrXJGRPd3t4gq01tbQ0Xho,55870
 mkits/critic2.py,sha256=oKdw9-kuJ_w3Pr_-3HjVFEJpIzXZ4y2u9p-Cgd6EhZM,5669
 mkits/database.py,sha256=BAABeSpglqhsHFQ3SbtFoHoEvMM2WI8xoPwJzMnahxI,21610
 mkits/fdmnes.py,sha256=fT5Smhjc9nbnxa-0UmiQtAgqmtStPCsGeHZB2ha_KMo,2750
 mkits/globle.py,sha256=tYFD7Zyyq2-0bBjCPNRKjXY7VMkJXdJBcATCPutqghM,46998
 mkits/gui.py,sha256=Hm80AqQ5Xo5YOFiL9Dw_YbqB0SH1T7cnz_1hEZ5LJR8,603
-mkits/main.py,sha256=7WP_aPOycPRHRuPc-vau-ZelvMclz1LW-8ryaGM9_VE,20366
+mkits/main.py,sha256=9IBV2r1Ir8NVl-iHPWv33yTsFIduFOR17rh1Si9hIoE,20366
 mkits/qe.py,sha256=wQGhhpYaN8sF1Mv6FnRYAHa7iVgv_REWkvmbmGVGyxM,28640
 mkits/structgen.py,sha256=KU7YEJyVul54e_hz7x5koe4Y9OvnAEJk-wmroSeu9GM,11851
 mkits/sysfc.py,sha256=3n-LRQvhn20sKm6MetdDIr5TDSW9Bwm-rn_EUtRytH4,586
 mkits/test.py,sha256=r0q-U05Ea5btuX387Bf9xq1_UcqQ3lsYSA0G1CHMN8o,70
 mkits/vasp.py,sha256=ajbPhvk1lQB_Hn-YNodTqhB9ts7jbTp0k5oIQfWAgag,86844
 mkits/wien.py,sha256=mAUse-LRuNfsGtuaWy_scLiuVjPSTyQQr1WoJnLDuaU,6046
-mkits-0.88.dist-info/LICENSE,sha256=K-70wSDhtej9fT8-2bgPAhF-HWnGJFcVJih6oW_VB40,1065
-mkits-0.88.dist-info/METADATA,sha256=bUBqPlwlnJe50Kq0pYPCJkLvGlkB0lt3O8xlct3dahk,746
-mkits-0.88.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mkits-0.88.dist-info/entry_points.txt,sha256=eASBlPfzZhYGByBpPrgqW6sql7PxU6FmyVELsmJyFU8,48
-mkits-0.88.dist-info/top_level.txt,sha256=mwi1qPFoGPi5qCr_1rVYYvxdjjukwIaUfF_n2itDwh8,6
-mkits-0.88.dist-info/RECORD,,
+mkits-0.89.dist-info/LICENSE,sha256=K-70wSDhtej9fT8-2bgPAhF-HWnGJFcVJih6oW_VB40,1065
+mkits-0.89.dist-info/METADATA,sha256=QHAuqig3PKOf7ZF5M4keLyad7rIEn_fMzlpMhGM9nlA,746
+mkits-0.89.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mkits-0.89.dist-info/entry_points.txt,sha256=eASBlPfzZhYGByBpPrgqW6sql7PxU6FmyVELsmJyFU8,48
+mkits-0.89.dist-info/top_level.txt,sha256=mwi1qPFoGPi5qCr_1rVYYvxdjjukwIaUfF_n2itDwh8,6
+mkits-0.89.dist-info/RECORD,,
```

