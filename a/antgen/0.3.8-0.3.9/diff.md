# Comparing `tmp/antgen-0.3.8-py3-none-any.whl.zip` & `tmp/antgen-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 42180 bytes, number of entries: 113
+Zip file size: 58696 bytes, number of entries: 115
 -rw-rw-rw-  2.0 fat    18991 b- defN 23-Jul-14 16:58 antgen/ActivityModel.py
 -rw-rw-rw-  2.0 fat     5871 b- defN 23-Jul-14 16:55 antgen/ApplianceModel.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/LICENSE
 -rw-rw-rw-  2.0 fat     7913 b- defN 23-Jul-14 16:55 antgen/LoadModelComponents.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/Tools.py
+-rw-rw-rw-  2.0 fat     5072 b- defN 23-Jul-14 21:11 antgen/Tools.py
 -rw-rw-rw-  2.0 fat     6013 b- defN 23-Jul-14 16:55 antgen/UserModel.py
 -rw-rw-rw-  2.0 fat       76 b- defN 23-Jul-14 16:55 antgen/__init__.py
 -rw-rw-rw-  2.0 fat    19213 b- defN 23-Jul-14 16:55 antgen/antgen.py
 -rw-rw-rw-  2.0 fat      220 b- defN 23-Jul-14 16:55 antgen/default.conf
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/example1.png
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/example2.png
+-rw-rw-rw-  2.0 fat    19813 b- defN 23-Jul-14 17:09 antgen/main.py
 -rw-rw-rw-  2.0 fat     2807 b- defN 23-Jul-14 16:55 antgen/mapping.conf
 -rw-rw-rw-  2.0 fat      104 b- defN 23-Jul-14 16:55 antgen/requirements.txt
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/activities/HOUSEHOLD/dry_clothes.conf
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/activities/HOUSEHOLD/ironing.conf
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/activities/HOUSEHOLD/vacuum.conf
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/activities/HOUSEHOLD/wash_laundry.conf
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/activities/KITCHEN/dishwasher.conf
@@ -104,12 +105,13 @@
 -rw-rw-rw-  2.0 fat     8479 b- defN 23-Jul-14 16:55 antgen/appliances/TV/dev_B80E51/mode0
 -rw-rw-rw-  2.0 fat     8429 b- defN 23-Jul-14 16:55 antgen/appliances/TV/dev_B80E51/mode1
 -rw-rw-rw-  2.0 fat     7571 b- defN 23-Jul-14 16:55 antgen/appliances/TV/dev_B80E51/mode2
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/appliances/VACUUMCLEANER/device_B7E2F8/mode0
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/appliances/WASHINGMACHINE/ECO-H1/mode2
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/appliances/WASHINGMACHINE/ECO-H1/mode3
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 16:55 antgen/appliances/WASHINGMACHINE/_B82E27/mode0
--rw-rw-rw-  2.0 fat      493 b- defN 23-Jul-14 17:06 antgen-0.3.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 17:06 antgen-0.3.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-14 17:06 antgen-0.3.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat    10605 b- defN 23-Jul-14 17:06 antgen-0.3.8.dist-info/RECORD
-113 files, 96884 bytes uncompressed, 24536 bytes compressed:  74.7%
+-rw-rw-rw-  2.0 fat     1131 b- defN 23-Jul-14 21:16 antgen-0.3.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    19191 b- defN 23-Jul-14 21:16 antgen-0.3.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 21:16 antgen-0.3.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-14 21:15 antgen-0.3.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    10769 b- defN 23-Jul-14 21:16 antgen-0.3.9.dist-info/RECORD
+115 files, 141762 bytes uncompressed, 40812 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -27,14 +27,17 @@
 
 Filename: antgen/example1.png
 Comment: 
 
 Filename: antgen/example2.png
 Comment: 
 
+Filename: antgen/main.py
+Comment: 
+
 Filename: antgen/mapping.conf
 Comment: 
 
 Filename: antgen/requirements.txt
 Comment: 
 
 Filename: antgen/activities/HOUSEHOLD/dry_clothes.conf
@@ -321,20 +324,23 @@
 
 Filename: antgen/appliances/WASHINGMACHINE/ECO-H1/mode3
 Comment: 
 
 Filename: antgen/appliances/WASHINGMACHINE/_B82E27/mode0
 Comment: 
 
-Filename: antgen-0.3.8.dist-info/METADATA
+Filename: antgen-0.3.9.dist-info/LICENSE
+Comment: 
+
+Filename: antgen-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: antgen-0.3.8.dist-info/WHEEL
+Filename: antgen-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: antgen-0.3.8.dist-info/top_level.txt
+Filename: antgen-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: antgen-0.3.8.dist-info/RECORD
+Filename: antgen-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## antgen/Tools.py

```diff
@@ -0,0 +1,317 @@
+00000000: 2320 2020 414e 5467 656e 202d 2d20 7468  #   ANTgen -- th
+00000010: 6520 414d 4241 4c2d 6261 7365 6420 4e49  e AMBAL-based NI
+00000020: 4c4d 2054 7261 6365 2067 656e 6572 6174  LM Trace generat
+00000030: 6f72 0d0a 230d 0a23 2020 2043 6f70 7972  or..#..#   Copyr
+00000040: 6967 6874 2028 4329 2032 3031 3920 2041  ight (C) 2019  A
+00000050: 6e64 7265 6173 2052 6569 6e68 6172 6474  ndreas Reinhardt
+00000060: 203c 7265 696e 6861 7264 7440 6965 6565   <reinhardt@ieee
+00000070: 2e6f 7267 3e2c 2054 5520 436c 6175 7374  .org>, TU Claust
+00000080: 6861 6c0d 0a23 0d0a 2320 2020 5065 726d  hal..#..#   Perm
+00000090: 6973 7369 6f6e 2069 7320 6865 7265 6279  ission is hereby
+000000a0: 2067 7261 6e74 6564 2c20 6672 6565 206f   granted, free o
+000000b0: 6620 6368 6172 6765 2c20 746f 2061 6e79  f charge, to any
+000000c0: 2070 6572 736f 6e20 6f62 7461 696e 696e   person obtainin
+000000d0: 6720 6120 636f 7079 0d0a 2320 2020 6f66  g a copy..#   of
+000000e0: 2074 6869 7320 736f 6674 7761 7265 2061   this software a
+000000f0: 6e64 2061 7373 6f63 6961 7465 6420 646f  nd associated do
+00000100: 6375 6d65 6e74 6174 696f 6e20 6669 6c65  cumentation file
+00000110: 7320 2874 6865 2022 536f 6674 7761 7265  s (the "Software
+00000120: 2229 2c20 746f 2064 6561 6c0d 0a23 2020  "), to deal..#  
+00000130: 2069 6e20 7468 6520 536f 6674 7761 7265   in the Software
+00000140: 2077 6974 686f 7574 2072 6573 7472 6963   without restric
+00000150: 7469 6f6e 2c20 696e 636c 7564 696e 6720  tion, including 
+00000160: 7769 7468 6f75 7420 6c69 6d69 7461 7469  without limitati
+00000170: 6f6e 2074 6865 2072 6967 6874 730d 0a23  on the rights..#
+00000180: 2020 2074 6f20 7573 652c 2063 6f70 792c     to use, copy,
+00000190: 206d 6f64 6966 792c 206d 6572 6765 2c20   modify, merge, 
+000001a0: 7075 626c 6973 682c 2064 6973 7472 6962  publish, distrib
+000001b0: 7574 652c 2073 7562 6c69 6365 6e73 652c  ute, sublicense,
+000001c0: 2061 6e64 2f6f 7220 7365 6c6c 0d0a 2320   and/or sell..# 
+000001d0: 2020 636f 7069 6573 206f 6620 7468 6520    copies of the 
+000001e0: 536f 6674 7761 7265 2c20 616e 6420 746f  Software, and to
+000001f0: 2070 6572 6d69 7420 7065 7273 6f6e 7320   permit persons 
+00000200: 746f 2077 686f 6d20 7468 6520 536f 6674  to whom the Soft
+00000210: 7761 7265 2069 730d 0a23 2020 2066 7572  ware is..#   fur
+00000220: 6e69 7368 6564 2074 6f20 646f 2073 6f2c  nished to do so,
+00000230: 2073 7562 6a65 6374 2074 6f20 7468 6520   subject to the 
+00000240: 666f 6c6c 6f77 696e 6720 636f 6e64 6974  following condit
+00000250: 696f 6e73 3a0d 0a23 0d0a 2320 2020 5468  ions:..#..#   Th
+00000260: 6520 6162 6f76 6520 636f 7079 7269 6768  e above copyrigh
+00000270: 7420 6e6f 7469 6365 2061 6e64 2074 6869  t notice and thi
+00000280: 7320 7065 726d 6973 7369 6f6e 206e 6f74  s permission not
+00000290: 6963 6520 7368 616c 6c20 6265 2069 6e63  ice shall be inc
+000002a0: 6c75 6465 6420 696e 2061 6c6c 0d0a 2320  luded in all..# 
+000002b0: 2020 636f 7069 6573 206f 7220 7375 6273    copies or subs
+000002c0: 7461 6e74 6961 6c20 706f 7274 696f 6e73  tantial portions
+000002d0: 206f 6620 7468 6520 536f 6674 7761 7265   of the Software
+000002e0: 2e0d 0a23 0d0a 2320 2020 5448 4520 534f  ...#..#   THE SO
+000002f0: 4654 5741 5245 2049 5320 5052 4f56 4944  FTWARE IS PROVID
+00000300: 4544 2022 4153 2049 5322 2c20 5749 5448  ED "AS IS", WITH
+00000310: 4f55 5420 5741 5252 414e 5459 204f 4620  OUT WARRANTY OF 
+00000320: 414e 5920 4b49 4e44 2c20 4558 5052 4553  ANY KIND, EXPRES
+00000330: 5320 4f52 0d0a 2320 2020 494d 504c 4945  S OR..#   IMPLIE
+00000340: 442c 2049 4e43 4c55 4449 4e47 2042 5554  D, INCLUDING BUT
+00000350: 204e 4f54 204c 494d 4954 4544 2054 4f20   NOT LIMITED TO 
+00000360: 5448 4520 5741 5252 414e 5449 4553 204f  THE WARRANTIES O
+00000370: 4620 4d45 5243 4841 4e54 4142 494c 4954  F MERCHANTABILIT
+00000380: 592c 0d0a 2320 2020 4649 544e 4553 5320  Y,..#   FITNESS 
+00000390: 464f 5220 4120 5041 5254 4943 554c 4152  FOR A PARTICULAR
+000003a0: 2050 5552 504f 5345 2041 4e44 204e 4f4e   PURPOSE AND NON
+000003b0: 494e 4652 494e 4745 4d45 4e54 2e20 494e  INFRINGEMENT. IN
+000003c0: 204e 4f20 4556 454e 5420 5348 414c 4c20   NO EVENT SHALL 
+000003d0: 5448 450d 0a23 2020 2041 5554 484f 5253  THE..#   AUTHORS
+000003e0: 204f 5220 434f 5059 5249 4748 5420 484f   OR COPYRIGHT HO
+000003f0: 4c44 4552 5320 4245 204c 4941 424c 4520  LDERS BE LIABLE 
+00000400: 464f 5220 414e 5920 434c 4149 4d2c 2044  FOR ANY CLAIM, D
+00000410: 414d 4147 4553 204f 5220 4f54 4845 520d  AMAGES OR OTHER.
+00000420: 0a23 2020 204c 4941 4249 4c49 5459 2c20  .#   LIABILITY, 
+00000430: 5748 4554 4845 5220 494e 2041 4e20 4143  WHETHER IN AN AC
+00000440: 5449 4f4e 204f 4620 434f 4e54 5241 4354  TION OF CONTRACT
+00000450: 2c20 544f 5254 204f 5220 4f54 4845 5257  , TORT OR OTHERW
+00000460: 4953 452c 2041 5249 5349 4e47 2046 524f  ISE, ARISING FRO
+00000470: 4d2c 0d0a 2320 2020 4f55 5420 4f46 204f  M,..#   OUT OF O
+00000480: 5220 494e 2043 4f4e 4e45 4354 494f 4e20  R IN CONNECTION 
+00000490: 5749 5448 2054 4845 2053 4f46 5457 4152  WITH THE SOFTWAR
+000004a0: 4520 4f52 2054 4845 2055 5345 204f 5220  E OR THE USE OR 
+000004b0: 4f54 4845 5220 4445 414c 494e 4753 2049  OTHER DEALINGS I
+000004c0: 4e20 5448 450d 0a23 2020 2053 4f46 5457  N THE..#   SOFTW
+000004d0: 4152 452e 0d0a 696d 706f 7274 206e 756d  ARE...import num
+000004e0: 7079 2061 7320 6e70 0d0a 6672 6f6d 2062  py as np..from b
+000004f0: 6974 6172 7261 7920 696d 706f 7274 2062  itarray import b
+00000500: 6974 6172 7261 790d 0a0d 0a23 206c 6574  itarray....# let
+00000510: 2773 2064 6566 696e 6520 736f 6d65 2063  's define some c
+00000520: 6f6e 7374 616e 7473 0d0a 7365 6373 5f70  onstants..secs_p
+00000530: 6572 5f62 6c6f 636b 203d 2039 3030 2020  er_block = 900  
+00000540: 2320 3630 303d 3130 6d69 6e2c 2039 3030  # 600=10min, 900
+00000550: 3d31 356d 696e 2c20 3132 3030 3d32 306d  =15min, 1200=20m
+00000560: 696e 2c20 3138 3030 3d33 306d 696e 2c20  in, 1800=30min, 
+00000570: 3336 3030 3d36 306d 696e 0d0a 626c 6f63  3600=60min..bloc
+00000580: 6b5f 7365 7061 7261 746f 7220 3d20 3620  k_separator = 6 
+00000590: 2023 2073 7061 6365 2062 6c6f 636b 7320   # space blocks 
+000005a0: 6170 6172 7420 6576 6572 7920 6e20 686f  apart every n ho
+000005b0: 7572 730d 0a0d 0a23 2069 6e74 6572 6e61  urs....# interna
+000005c0: 6c20 7661 7269 6162 6c65 730d 0a77 6565  l variables..wee
+000005d0: 6b64 6179 7320 3d20 7b30 3a20 276d 6f6e  kdays = {0: 'mon
+000005e0: 6461 7927 2c20 313a 2027 7475 6573 6461  day', 1: 'tuesda
+000005f0: 7927 2c20 323a 2027 7765 646e 6573 6461  y', 2: 'wednesda
+00000600: 7927 2c20 333a 2027 7468 7572 7364 6179  y', 3: 'thursday
+00000610: 272c 2034 3a20 2766 7269 6461 7927 2c20  ', 4: 'friday', 
+00000620: 353a 2027 7361 7475 7264 6179 272c 2036  5: 'saturday', 6
+00000630: 3a20 2773 756e 6461 7927 7d0d 0a73 6563  : 'sunday'}..sec
+00000640: 735f 7065 725f 6461 7920 3d20 3836 3430  s_per_day = 8640
+00000650: 300d 0a62 6c6f 636b 735f 7065 725f 6461  0..blocks_per_da
+00000660: 7920 3d20 696e 7428 7365 6373 5f70 6572  y = int(secs_per
+00000670: 5f64 6179 202f 2073 6563 735f 7065 725f  _day / secs_per_
+00000680: 626c 6f63 6b29 0d0a 626c 6f63 6b73 5f70  block)..blocks_p
+00000690: 6572 5f68 6f75 7220 3d20 696e 7428 626c  er_hour = int(bl
+000006a0: 6f63 6b73 5f70 6572 5f64 6179 202f 2032  ocks_per_day / 2
+000006b0: 3429 0d0a 0d0a 2320 4865 6c70 6572 2074  4)....# Helper t
+000006c0: 6f20 6765 7420 6120 6269 746d 6170 206f  o get a bitmap o
+000006d0: 6620 7573 6572 2070 7265 7365 6e63 6520  f user presence 
+000006e0: 6174 2068 6f6d 650d 0a64 6566 2067 6574  at home..def get
+000006f0: 5f62 6974 6d61 705f 6672 6f6d 5f74 696d  _bitmap_from_tim
+00000700: 6572 616e 6765 2863 6f6d 6d61 5f73 6570  erange(comma_sep
+00000710: 6172 6174 6564 5f74 696d 6572 616e 6765  arated_timerange
+00000720: 293a 0d0a 2020 2020 626d 7020 3d20 6269  ):..    bmp = bi
+00000730: 7461 7272 6179 2873 6563 735f 7065 725f  tarray(secs_per_
+00000740: 6461 7929 2020 2320 616c 7761 7973 2072  day)  # always r
+00000750: 6574 7572 6e20 2a6f 6e65 2a20 6461 7920  eturn *one* day 
+00000760: 6f66 2062 6974 730d 0a20 2020 2062 6d70  of bits..    bmp
+00000770: 2e73 6574 616c 6c28 4661 6c73 6529 0d0a  .setall(False)..
+00000780: 0d0a 2020 2020 666f 7220 7469 6d65 5f72  ..    for time_r
+00000790: 616e 6765 2069 6e20 636f 6d6d 615f 7365  ange in comma_se
+000007a0: 7061 7261 7465 645f 7469 6d65 7261 6e67  parated_timerang
+000007b0: 652e 7370 6c69 7428 272c 2729 3a0d 0a20  e.split(','):.. 
+000007c0: 2020 2020 2020 2069 6620 272d 2720 6e6f         if '-' no
+000007d0: 7420 696e 2074 696d 655f 7261 6e67 653a  t in time_range:
+000007e0: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
+000007f0: 2020 2028 6672 2c20 746f 2920 3d20 7469     (fr, to) = ti
+00000800: 6d65 5f72 616e 6765 2e73 706c 6974 2827  me_range.split('
+00000810: 2d27 290d 0a20 2020 2020 2020 2069 6620  -')..        if 
+00000820: 273a 2720 6e6f 7420 696e 2066 7220 6f72  ':' not in fr or
+00000830: 2027 3a27 206e 6f74 2069 6e20 746f 3a20   ':' not in to: 
+00000840: 636f 6e74 696e 7565 0d0a 0d0a 2020 2020  continue....    
+00000850: 2020 2020 2320 7061 7273 6520 2766 726f      # parse 'fro
+00000860: 6d27 2074 696d 650d 0a20 2020 2020 2020  m' time..       
+00000870: 2028 6872 2c20 6d6e 2920 3d20 6672 2e73   (hr, mn) = fr.s
+00000880: 706c 6974 2827 3a27 290d 0a20 2020 2020  plit(':')..     
+00000890: 2020 2069 6620 696e 7428 6872 2920 3e3d     if int(hr) >=
+000008a0: 2032 343a 2068 7220 3d20 3234 3b20 6d6e   24: hr = 24; mn
+000008b0: 203d 2030 0d0a 2020 2020 2020 2020 6672   = 0..        fr
+000008c0: 6f6d 5f6f 6666 7365 7420 3d20 3630 202a  om_offset = 60 *
+000008d0: 2028 696e 7428 6872 2920 2a20 3630 202b   (int(hr) * 60 +
+000008e0: 2069 6e74 286d 6e29 290d 0a0d 0a20 2020   int(mn))....   
+000008f0: 2020 2020 2023 2070 6172 7365 2027 746f       # parse 'to
+00000900: 2720 7469 6d65 0d0a 2020 2020 2020 2020  ' time..        
+00000910: 2868 722c 206d 6e29 203d 2074 6f2e 7370  (hr, mn) = to.sp
+00000920: 6c69 7428 273a 2729 0d0a 2020 2020 2020  lit(':')..      
+00000930: 2020 6966 2069 6e74 2868 7229 203e 3d20    if int(hr) >= 
+00000940: 3234 3a20 6872 203d 2032 343b 206d 6e20  24: hr = 24; mn 
+00000950: 3d20 300d 0a20 2020 2020 2020 2074 6f5f  = 0..        to_
+00000960: 6f66 6673 6574 203d 2036 3020 2a20 2869  offset = 60 * (i
+00000970: 6e74 2868 7229 202a 2036 3020 2b20 696e  nt(hr) * 60 + in
+00000980: 7428 6d6e 2929 0d0a 0d0a 2020 2020 2020  t(mn))....      
+00000990: 2020 626d 705b 6672 6f6d 5f6f 6666 7365    bmp[from_offse
+000009a0: 743a 746f 5f6f 6666 7365 745d 203d 2054  t:to_offset] = T
+000009b0: 7275 650d 0a20 2020 2023 2069 7465 7261  rue..    # itera
+000009c0: 7469 6e67 206f 7665 7220 616c 6c20 7469  ting over all ti
+000009d0: 6d65 2072 616e 6765 7320 636f 6d70 6c65  me ranges comple
+000009e0: 7465 640d 0a0d 0a20 2020 2072 6574 7572  ted....    retur
+000009f0: 6e20 626d 700d 0a0d 0a0d 0a64 6566 2067  n bmp......def g
+00000a00: 6574 5f62 6974 6d61 705f 6672 6f6d 5f77  et_bitmap_from_w
+00000a10: 6565 6b64 6179 5f6c 6973 7428 7765 656b  eekday_list(week
+00000a20: 6461 795f 6c69 7374 2c20 6e75 6d5f 6461  day_list, num_da
+00000a30: 7973 2c20 7374 6172 745f 6461 793d 3029  ys, start_day=0)
+00000a40: 3a0d 0a20 2020 2062 6d70 203d 2062 6974  :..    bmp = bit
+00000a50: 6172 7261 7928 7365 6373 5f70 6572 5f64  array(secs_per_d
+00000a60: 6179 202a 206e 756d 5f64 6179 7329 0d0a  ay * num_days)..
+00000a70: 2020 2020 626d 702e 7365 7461 6c6c 2854      bmp.setall(T
+00000a80: 7275 6529 0d0a 0d0a 2020 2020 2320 7265  rue)....    # re
+00000a90: 6164 2064 6169 6c79 2072 616e 6765 7320  ad daily ranges 
+00000aa0: 2877 656c 6c2c 2061 7420 6c65 6173 7420  (well, at least 
+00000ab0: 666f 7220 7468 6520 6461 7973 2064 6566  for the days def
+00000ac0: 696e 6564 290d 0a20 2020 2074 696d 6573  ined)..    times
+00000ad0: 7061 6e73 203d 207b 7d0d 0a20 2020 2066  pans = {}..    f
+00000ae0: 6f72 2064 6179 2069 6e20 7765 656b 6461  or day in weekda
+00000af0: 7973 2e76 616c 7565 7328 293a 0d0a 2020  ys.values():..  
+00000b00: 2020 2020 2020 6966 2064 6179 2069 6e20        if day in 
+00000b10: 7765 656b 6461 795f 6c69 7374 3a0d 0a20  weekday_list:.. 
+00000b20: 2020 2020 2020 2020 2020 2074 696d 6573             times
+00000b30: 7061 6e73 5b64 6179 5d20 3d20 6765 745f  pans[day] = get_
+00000b40: 6269 746d 6170 5f66 726f 6d5f 7469 6d65  bitmap_from_time
+00000b50: 7261 6e67 6528 7765 656b 6461 795f 6c69  range(weekday_li
+00000b60: 7374 2e67 6574 2864 6179 2929 0d0a 0d0a  st.get(day))....
+00000b70: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00000b80: 6765 286e 756d 5f64 6179 7329 3a0d 0a20  ge(num_days):.. 
+00000b90: 2020 2020 2020 2064 6179 203d 2077 6565         day = wee
+00000ba0: 6b64 6179 732e 6765 7428 696e 7428 2873  kdays.get(int((s
+00000bb0: 7461 7274 5f64 6179 202b 2069 2920 2520  tart_day + i) % 
+00000bc0: 3729 290d 0a20 2020 2020 2020 2069 6620  7))..        if 
+00000bd0: 6461 7920 696e 2074 696d 6573 7061 6e73  day in timespans
+00000be0: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
+00000bf0: 2020 2020 2020 626d 705b 6920 2a20 7365        bmp[i * se
+00000c00: 6373 5f70 6572 5f64 6179 3a28 6920 2b20  cs_per_day:(i + 
+00000c10: 3129 202a 2073 6563 735f 7065 725f 6461  1) * secs_per_da
+00000c20: 795d 2026 3d20 7469 6d65 7370 616e 735b  y] &= timespans[
+00000c30: 6461 795d 0d0a 2020 2020 2020 2020 656c  day]..        el
+00000c40: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00000c50: 2062 6d70 5b69 202a 2073 6563 735f 7065   bmp[i * secs_pe
+00000c60: 725f 6461 793a 2869 202b 2031 2920 2a20  r_day:(i + 1) * 
+00000c70: 7365 6373 5f70 6572 5f64 6179 5d20 3d20  secs_per_day] = 
+00000c80: 4661 6c73 650d 0a20 2020 2023 2041 6c6c  False..    # All
+00000c90: 2061 7661 696c 6162 696c 6974 7920 6c65   availability le
+00000ca0: 7665 6c73 2073 686f 756c 6420 6265 2069  vels should be i
+00000cb0: 6e69 7469 616c 697a 6564 2062 7920 6e6f  nitialized by no
+00000cc0: 770d 0a0d 0a20 2020 2072 6574 7572 6e20  w....    return 
+00000cd0: 626d 700d 0a0d 0a0d 0a64 6566 2063 6f75  bmp......def cou
+00000ce0: 6e74 2862 6974 6d61 702c 2076 616c 7565  nt(bitmap, value
+00000cf0: 3d54 7275 6529 3a0d 0a20 2020 2072 6574  =True):..    ret
+00000d00: 7572 6e20 6269 746d 6170 2e63 6f75 6e74  urn bitmap.count
+00000d10: 2876 616c 7565 290d 0a0d 0a0d 0a64 6566  (value)......def
+00000d20: 2076 6973 7561 6c69 7a65 5f68 6561 6465   visualize_heade
+00000d30: 7228 7374 6172 745f 6461 7920 3d20 3029  r(start_day = 0)
+00000d40: 3a0d 0a20 2020 206f 7574 203d 2027 2027  :..    out = ' '
+00000d50: 202a 2036 0d0a 2020 2020 6966 2062 6c6f   * 6..    if blo
+00000d60: 636b 735f 7065 725f 686f 7572 203d 3d20  cks_per_hour == 
+00000d70: 313a 0d0a 2020 2020 2020 2020 666f 7220  1:..        for 
+00000d80: 6920 696e 2072 616e 6765 2830 2c20 3234  i in range(0, 24
+00000d90: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00000da0: 6f75 7420 2b3d 2027 7b3a 3178 7d20 272e  out += '{:1x} '.
+00000db0: 666f 726d 6174 2869 2531 3229 0d0a 2020  format(i%12)..  
+00000dc0: 2020 2020 2020 2020 2020 6966 2069 2021            if i !
+00000dd0: 3d20 3020 616e 6420 2831 202b 2069 2920  = 0 and (1 + i) 
+00000de0: 2520 626c 6f63 6b5f 7365 7061 7261 746f  % block_separato
+00000df0: 7220 3d3d 2030 3a0d 0a20 2020 2020 2020  r == 0:..       
+00000e00: 2020 2020 2020 2020 206f 7574 202b 3d20           out += 
+00000e10: 2720 2027 0d0a 2020 2020 656c 7365 3a0d  '  '..    else:.
+00000e20: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+00000e30: 6e20 7261 6e67 6528 302c 2032 3429 3a0d  n range(0, 24):.
+00000e40: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00000e50: 7274 5f74 696d 6520 3d20 7374 7228 6929  rt_time = str(i)
+00000e60: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00000e70: 6172 745f 7469 6d65 202b 3d20 2768 2720  art_time += 'h' 
+00000e80: 6966 2062 6c6f 636b 735f 7065 725f 686f  if blocks_per_ho
+00000e90: 7572 203e 2032 2065 6c73 6520 2727 0d0a  ur > 2 else ''..
+00000ea0: 2020 2020 2020 2020 2020 2020 6f75 7420              out 
+00000eb0: 2b3d 2027 7b3a 3c73 7d7b 7d20 272e 666f  += '{:<s}{} '.fo
+00000ec0: 726d 6174 2873 7461 7274 5f74 696d 652c  rmat(start_time,
+00000ed0: 2027 2027 202a 2028 626c 6f63 6b73 5f70   ' ' * (blocks_p
+00000ee0: 6572 5f68 6f75 722d 6c65 6e28 7374 6172  er_hour-len(star
+00000ef0: 745f 7469 6d65 2929 290d 0a20 2020 2020  t_time)))..     
+00000f00: 2020 2020 2020 2069 6620 6920 213d 2030         if i != 0
+00000f10: 2061 6e64 2028 312b 6929 2025 2062 6c6f   and (1+i) % blo
+00000f20: 636b 5f73 6570 6172 6174 6f72 203d 3d20  ck_separator == 
+00000f30: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+00000f40: 2020 2020 6f75 7420 2b3d 2027 2020 270d      out += '  '.
+00000f50: 0a20 2020 2072 6574 7572 6e20 6f75 740d  .    return out.
+00000f60: 0a0d 0a64 6566 2076 6973 7561 6c69 7a65  ...def visualize
+00000f70: 5f6d 6170 2862 6974 6d61 702c 2073 7461  _map(bitmap, sta
+00000f80: 7274 5f64 6179 3d30 293a 0d0a 2020 2020  rt_day=0):..    
+00000f90: 6f75 7420 3d20 5b5d 0d0a 0d0a 2020 2020  out = []....    
+00000fa0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00000fb0: 6528 6269 746d 6170 2c20 6269 7461 7272  e(bitmap, bitarr
+00000fc0: 6179 293a 0d0a 2020 2020 2020 2020 6f75  ay):..        ou
+00000fd0: 742e 6170 7065 6e64 2822 5b4e 6f20 6269  t.append("[No bi
+00000fe0: 7420 6d61 7020 746f 2064 6973 706c 6179  t map to display
+00000ff0: 5d22 290d 0a20 2020 2020 2020 2072 6574  ]")..        ret
+00001000: 7572 6e20 6f75 740d 0a0d 0a20 2020 2066  urn out....    f
+00001010: 6f72 2069 2069 6e20 7261 6e67 6528 696e  or i in range(in
+00001020: 7428 6c65 6e28 6269 746d 6170 2920 2f20  t(len(bitmap) / 
+00001030: 7365 6373 5f70 6572 5f64 6179 2929 3a0d  secs_per_day)):.
+00001040: 0a20 2020 2020 2020 2062 7566 203d 2027  .        buf = '
+00001050: 5b7b 3a33 2e33 7d5d 2027 2e66 6f72 6d61  [{:3.3}] '.forma
+00001060: 7428 7765 656b 6461 7973 5b28 2873 7461  t(weekdays[((sta
+00001070: 7274 5f64 6179 202b 2069 2920 2520 3729  rt_day + i) % 7)
+00001080: 5d29 0d0a 2020 2020 2020 2020 666f 7220  ])..        for 
+00001090: 6a20 696e 2072 616e 6765 2862 6c6f 636b  j in range(block
+000010a0: 735f 7065 725f 6461 7929 3a0d 0a20 2020  s_per_day):..   
+000010b0: 2020 2020 2020 2020 2069 6620 6a20 2520           if j % 
+000010c0: 626c 6f63 6b73 5f70 6572 5f68 6f75 7220  blocks_per_hour 
+000010d0: 3d3d 2030 2061 6e64 206a 2021 3d20 303a  == 0 and j != 0:
+000010e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000010f0: 2020 6275 6620 2b3d 2027 2027 0d0a 2020    buf += ' '..  
+00001100: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00001110: 2069 6e74 286a 2f62 6c6f 636b 735f 7065   int(j/blocks_pe
+00001120: 725f 686f 7572 2920 2520 626c 6f63 6b5f  r_hour) % block_
+00001130: 7365 7061 7261 746f 7220 3d3d 2030 3a0d  separator == 0:.
+00001140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001150: 2020 2020 2062 7566 202b 3d20 277c 2027       buf += '| '
+00001160: 0d0a 2020 2020 2020 2020 2020 2020 6f6e  ..            on
+00001170: 6573 203d 2063 6f75 6e74 2862 6974 6d61  es = count(bitma
+00001180: 705b 6920 2a20 7365 6373 5f70 6572 5f64  p[i * secs_per_d
+00001190: 6179 202b 206a 202a 2073 6563 735f 7065  ay + j * secs_pe
+000011a0: 725f 626c 6f63 6b3a 2069 202a 2073 6563  r_block: i * sec
+000011b0: 735f 7065 725f 6461 7920 2b20 286a 2b31  s_per_day + (j+1
+000011c0: 2920 2a20 7365 6373 5f70 6572 5f62 6c6f  ) * secs_per_blo
+000011d0: 636b 5d2c 2054 7275 6529 0d0a 2020 2020  ck], True)..    
+000011e0: 2020 2020 2020 2020 2320 7669 7375 616c          # visual
+000011f0: 697a 6520 6672 6163 7469 6f6e 2061 7661  ize fraction ava
+00001200: 696c 6162 696c 6974 7920 7573 696e 6720  ilability using 
+00001210: 2762 6f78 7927 2075 6e69 636f 6465 2063  'boxy' unicode c
+00001220: 6861 7273 0d0a 2020 2020 2020 2020 2020  hars..          
+00001230: 2020 6275 6620 2b3d 2063 6872 2839 3630    buf += chr(960
+00001240: 3120 2b20 696e 7428 6e70 2e66 6c6f 6f72  1 + int(np.floor
+00001250: 2837 202a 206f 6e65 732f 7365 6373 5f70  (7 * ones/secs_p
+00001260: 6572 5f62 6c6f 636b 2929 290d 0a20 2020  er_block)))..   
+00001270: 2020 2020 206f 7574 2e61 7070 656e 6428       out.append(
+00001280: 6275 6629 0d0a 0d0a 2020 2020 7265 7475  buf)....    retu
+00001290: 726e 206f 7574 0d0a 0d0a 0d0a 6465 6620  rn out......def 
+000012a0: 6765 745f 6561 726c 6965 7374 2862 6974  get_earliest(bit
+000012b0: 6d61 7029 3a0d 0a20 2020 2074 7279 3a0d  map):..    try:.
+000012c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000012d0: 6269 746d 6170 2e69 6e64 6578 2854 7275  bitmap.index(Tru
+000012e0: 6529 0d0a 2020 2020 6578 6365 7074 2056  e)..    except V
+000012f0: 616c 7565 4572 726f 723a 0d0a 2020 2020  alueError:..    
+00001300: 2020 2020 7265 7475 726e 204e 6f6e 650d      return None.
+00001310: 0a0d 0a0d 0a64 6566 2067 6574 5f6c 6174  .....def get_lat
+00001320: 6573 7428 6269 746d 6170 293a 0d0a 2020  est(bitmap):..  
+00001330: 2020 626d 7020 3d20 6269 746d 6170 2e63    bmp = bitmap.c
+00001340: 6f70 7928 290d 0a20 2020 2062 6d70 2e72  opy()..    bmp.r
+00001350: 6576 6572 7365 2829 0d0a 2020 2020 6f66  everse()..    of
+00001360: 6620 3d20 6765 745f 6561 726c 6965 7374  f = get_earliest
+00001370: 2862 6d70 290d 0a20 2020 2069 6620 6f66  (bmp)..    if of
+00001380: 6620 6973 206e 6f74 204e 6f6e 6520 616e  f is not None an
+00001390: 6420 6f66 6620 3e3d 2030 3a0d 0a20 2020  d off >= 0:..   
+000013a0: 2020 2020 2072 6574 7572 6e20 6c65 6e28       return len(
+000013b0: 6269 746d 6170 2920 2d20 6f66 660d 0a20  bitmap) - off.. 
+000013c0: 2020 2072 6574 7572 6e20 4e6f 6e65 0d0a     return None..
```

## Comparing `antgen-0.3.8.dist-info/RECORD` & `antgen-0.3.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 antgen/ActivityModel.py,sha256=Z13C5Bt3PamPCccy98SexYwUjLyoi9Dl3ZUI4oKwh8g,18991
 antgen/ApplianceModel.py,sha256=3oNBr3Z6WQyk_qDSHY8Bxk8AzHsYVcbjquwxeHfb0OY,5871
 antgen/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antgen/LoadModelComponents.py,sha256=Jkc_y5BQlBVtO6gARPP3GlPAVXOZYl0bJPiKDlqAAQc,7913
-antgen/Tools.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+antgen/Tools.py,sha256=yWpF_aDymNyZZLA67TRveYXyw65UqF8q2JAr3x6CSrw,5072
 antgen/UserModel.py,sha256=zJY7DdHGMFhPKIF6f8GFcNYkMo3R21j0fCYA_ZC06Kw,6013
 antgen/__init__.py,sha256=Lh7NOd9-n-o-7iRw3-RIoQCF_F57zhZQktJjCkSYOgA,76
 antgen/antgen.py,sha256=w3M4uuhk2XGjZVME2qdzLuLFxrAzQf_JmagamVrSXyw,19213
 antgen/default.conf,sha256=NYFOp_xShbio69zA08WiGfJ6yCfVCd9I23vuvixiwrM,220
 antgen/example1.png,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antgen/example2.png,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+antgen/main.py,sha256=os4x-q6ptnzlR0z0KhewSPPwYFDM-bbYMqvy7J9jZOk,19813
 antgen/mapping.conf,sha256=0zYaZfNFH_45jDz7Y-3xrS_m2qR4RTsVB9Mn9gE_bfc,2807
 antgen/requirements.txt,sha256=clHsyYiSPVNavXzmRO0lSa466ngl4x0gPFLtSLxFrRk,104
 antgen/activities/HOUSEHOLD/dry_clothes.conf,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antgen/activities/HOUSEHOLD/ironing.conf,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antgen/activities/HOUSEHOLD/vacuum.conf,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antgen/activities/HOUSEHOLD/wash_laundry.conf,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antgen/activities/KITCHEN/dishwasher.conf,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -103,11 +104,12 @@
 antgen/appliances/TV/dev_B80E51/mode0,sha256=a3JQ0p4UmAeziqu76TUIE0NEgwarF8s9-V79z_WbXHg,8479
 antgen/appliances/TV/dev_B80E51/mode1,sha256=WO8fJkigYVDKJnPUHwpaDN70phKT5E4HnGPSBlBZ4T4,8429
 antgen/appliances/TV/dev_B80E51/mode2,sha256=alEsZDlZNMIV-nknaLlvugV8qdZXcZQlXNndekICV4g,7571
 antgen/appliances/VACUUMCLEANER/device_B7E2F8/mode0,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antgen/appliances/WASHINGMACHINE/ECO-H1/mode2,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antgen/appliances/WASHINGMACHINE/ECO-H1/mode3,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antgen/appliances/WASHINGMACHINE/_B82E27/mode0,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-antgen-0.3.8.dist-info/METADATA,sha256=nCCKI6NUmc6ToKo0deKiRZ3aWqJLH2VjTxCH8IN6EH0,493
-antgen-0.3.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-antgen-0.3.8.dist-info/top_level.txt,sha256=lVuIG72qQlyQ93EJRsuVyiYiguJXsWRIEmfRIskw8dQ,7
-antgen-0.3.8.dist-info/RECORD,,
+antgen-0.3.9.dist-info/LICENSE,sha256=V3ZQ1IsxFIISGJvPm_i0oYdUGgjyadaICziDVtKoULk,1131
+antgen-0.3.9.dist-info/METADATA,sha256=LPhG_32XnG3_59yE68uMl5S8Nhlqn1zlhGoxZOtyjIU,19191
+antgen-0.3.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+antgen-0.3.9.dist-info/top_level.txt,sha256=lVuIG72qQlyQ93EJRsuVyiYiguJXsWRIEmfRIskw8dQ,7
+antgen-0.3.9.dist-info/RECORD,,
```

