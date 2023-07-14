# Comparing `tmp/fanfou_sdk-0.0.2.tar.gz` & `tmp/fanfou_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fanfou_sdk-0.0.2.tar", last modified: Mon Dec  9 12:39:09 2019, max compression
+gzip compressed data, was "fanfou_sdk-0.0.3.tar", last modified: Fri Jul 14 16:23:35 2023, max compression
```

## Comparing `fanfou_sdk-0.0.2.tar` & `fanfou_sdk-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 litomore   (501) staff       (20)        0 2019-12-09 12:39:09.000000 fanfou_sdk-0.0.2/
--rw-r--r--   0 litomore   (501) staff       (20)     4322 2019-12-09 12:39:09.000000 fanfou_sdk-0.0.2/PKG-INFO
-drwxr-xr-x   0 litomore   (501) staff       (20)        0 2019-12-09 12:39:09.000000 fanfou_sdk-0.0.2/fanfou_sdk.egg-info/
--rw-r--r--   0 litomore   (501) staff       (20)     4322 2019-12-09 12:39:09.000000 fanfou_sdk-0.0.2/fanfou_sdk.egg-info/PKG-INFO
--rw-r--r--   0 litomore   (501) staff       (20)      269 2019-12-09 12:39:09.000000 fanfou_sdk-0.0.2/fanfou_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 litomore   (501) staff       (20)       13 2019-12-09 12:39:09.000000 fanfou_sdk-0.0.2/fanfou_sdk.egg-info/requires.txt
--rw-r--r--   0 litomore   (501) staff       (20)       11 2019-12-09 12:39:09.000000 fanfou_sdk-0.0.2/fanfou_sdk.egg-info/top_level.txt
--rw-r--r--   0 litomore   (501) staff       (20)        1 2019-12-09 12:39:09.000000 fanfou_sdk-0.0.2/fanfou_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 litomore   (501) staff       (20)     1065 2019-11-30 15:06:24.000000 fanfou_sdk-0.0.2/LICENSE
-drwxr-xr-x   0 litomore   (501) staff       (20)        0 2019-12-09 12:39:09.000000 fanfou_sdk-0.0.2/fanfou_sdk/
--rw-r--r--   0 litomore   (501) staff       (20)       27 2019-12-04 17:48:45.000000 fanfou_sdk-0.0.2/fanfou_sdk/__init__.py
--rw-r--r--   0 litomore   (501) staff       (20)     5490 2019-12-09 12:32:37.000000 fanfou_sdk-0.0.2/fanfou_sdk/fanfou.py
--rw-r--r--   0 litomore   (501) staff       (20)     3795 2019-12-04 18:24:04.000000 fanfou_sdk-0.0.2/fanfou_sdk/oauth.py
--rw-r--r--   0 litomore   (501) staff       (20)     2928 2019-12-09 12:36:29.000000 fanfou_sdk-0.0.2/README.md
--rw-r--r--   0 litomore   (501) staff       (20)      550 2019-12-09 12:38:15.000000 fanfou_sdk-0.0.2/setup.py
--rw-r--r--   0 litomore   (501) staff       (20)      102 2019-12-09 12:39:09.000000 fanfou_sdk-0.0.2/setup.cfg
+drwxr-xr-x   0 litomore   (501) staff       (20)        0 2023-07-14 16:23:35.176400 fanfou_sdk-0.0.3/
+-rw-r--r--   0 litomore   (501) staff       (20)     1065 2023-07-09 08:38:56.000000 fanfou_sdk-0.0.3/LICENSE
+-rw-r--r--   0 litomore   (501) staff       (20)     3165 2023-07-14 16:23:35.176455 fanfou_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 litomore   (501) staff       (20)     2866 2023-07-09 08:38:56.000000 fanfou_sdk-0.0.3/README.md
+drwxr-xr-x   0 litomore   (501) staff       (20)        0 2023-07-14 16:23:35.175619 fanfou_sdk-0.0.3/fanfou_sdk/
+-rw-r--r--   0 litomore   (501) staff       (20)       27 2023-07-09 08:38:56.000000 fanfou_sdk-0.0.3/fanfou_sdk/__init__.py
+-rw-r--r--   0 litomore   (501) staff       (20)     5490 2023-07-09 08:38:56.000000 fanfou_sdk-0.0.3/fanfou_sdk/fanfou.py
+-rw-r--r--   0 litomore   (501) staff       (20)     3795 2023-07-09 08:38:56.000000 fanfou_sdk-0.0.3/fanfou_sdk/oauth.py
+drwxr-xr-x   0 litomore   (501) staff       (20)        0 2023-07-14 16:23:35.176241 fanfou_sdk-0.0.3/fanfou_sdk.egg-info/
+-rw-r--r--   0 litomore   (501) staff       (20)     3165 2023-07-14 16:23:35.000000 fanfou_sdk-0.0.3/fanfou_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 litomore   (501) staff       (20)      269 2023-07-14 16:23:35.000000 fanfou_sdk-0.0.3/fanfou_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 litomore   (501) staff       (20)        1 2023-07-14 16:23:35.000000 fanfou_sdk-0.0.3/fanfou_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 litomore   (501) staff       (20)       13 2023-07-14 16:23:35.000000 fanfou_sdk-0.0.3/fanfou_sdk.egg-info/requires.txt
+-rw-r--r--   0 litomore   (501) staff       (20)       11 2023-07-14 16:23:35.000000 fanfou_sdk-0.0.3/fanfou_sdk.egg-info/top_level.txt
+-rw-r--r--   0 litomore   (501) staff       (20)      102 2023-07-14 16:23:35.176656 fanfou_sdk-0.0.3/setup.cfg
+-rw-r--r--   0 litomore   (501) staff       (20)      532 2023-07-14 16:13:59.000000 fanfou_sdk-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fanfou_sdk-0.0.2/LICENSE` & `fanfou_sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fanfou_sdk-0.0.2/fanfou_sdk/fanfou.py` & `fanfou_sdk-0.0.3/fanfou_sdk/fanfou.py`

 * *Files identical despite different names*

### Comparing `fanfou_sdk-0.0.2/fanfou_sdk/oauth.py` & `fanfou_sdk-0.0.3/fanfou_sdk/oauth.py`

 * *Files identical despite different names*

### Comparing `fanfou_sdk-0.0.2/README.md` & `fanfou_sdk-0.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,166 +18,163 @@
 00000110: 6661 6e66 6f75 2d73 646b 295d 2868 7474  fanfou-sdk)](htt
 00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00000130: 4c69 746f 4d6f 7265 2f66 616e 666f 752d  LitoMore/fanfou-
 00000140: 7364 6b2d 7079 7468 6f6e 2f62 6c6f 622f  sdk-python/blob/
 00000150: 6d61 7374 6572 2f4c 4943 454e 5345 290a  master/LICENSE).
 00000160: 0a46 616e 666f 7520 5344 4b20 666f 7220  .Fanfou SDK for 
 00000170: 5079 7468 6f6e 0a0a 2323 2049 6e73 7461  Python..## Insta
-00000180: 6c6c 0a0a 6060 6062 6173 680a 2420 7069  ll..```bash.$ pi
-00000190: 7020 696e 7374 616c 6c20 6661 6e66 6f75  p install fanfou
-000001a0: 5f73 646b 0a60 6060 0a0a 2d2d 2d0a 0a3c  _sdk.```..---..<
-000001b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000001c0: 7777 772e 7061 7472 656f 6e2e 636f 6d2f  www.patreon.com/
-000001d0: 4c69 746f 4d6f 7265 223e 0a20 203c 696d  LitoMore">.  <im
-000001e0: 6720 7372 633d 2268 7474 7073 3a2f 2f63  g src="https://c
-000001f0: 352e 7061 7472 656f 6e2e 636f 6d2f 6578  5.patreon.com/ex
-00000200: 7465 726e 616c 2f6c 6f67 6f2f 6265 636f  ternal/logo/beco
-00000210: 6d65 5f61 5f70 6174 726f 6e5f 6275 7474  me_a_patron_butt
-00000220: 6f6e 4032 782e 706e 6722 2077 6964 7468  on@2x.png" width
-00000230: 3d22 3136 3022 3e0a 3c2f 613e 0a0a 2323  ="160">.</a>..##
-00000240: 2055 7361 6765 0a0a 2323 2320 4f41 7574   Usage..### OAut
-00000250: 680a 0a60 6060 7079 7468 6f6e 0a66 726f  h..```python.fro
-00000260: 6d20 6661 6e66 6f75 5f73 646b 2069 6d70  m fanfou_sdk imp
-00000270: 6f72 7420 4661 6e66 6f75 0a0a 6666 203d  ort Fanfou..ff =
-00000280: 2046 616e 666f 7528 0a20 2020 2063 6f6e   Fanfou(.    con
-00000290: 7375 6d65 725f 6b65 793d 2727 2c0a 2020  sumer_key='',.  
-000002a0: 2020 636f 6e73 756d 6572 5f73 6563 7265    consumer_secre
-000002b0: 743d 2727 2c0a 2020 2020 6f61 7574 685f  t='',.    oauth_
-000002c0: 746f 6b65 6e3d 2727 2c0a 2020 2020 6f61  token='',.    oa
-000002d0: 7574 685f 746f 6b65 6e5f 7365 6372 6574  uth_token_secret
-000002e0: 3d27 270a 290a 0a72 6573 756c 742c 2072  =''.)..result, r
-000002f0: 6573 706f 6e73 6520 3d20 6666 2e67 6574  esponse = ff.get
-00000300: 2827 2f73 7461 7475 7365 732f 686f 6d65  ('/statuses/home
-00000310: 5f74 696d 656c 696e 6527 2c20 7b27 666f  _timeline', {'fo
-00000320: 726d 6174 273a 2027 6874 6d6c 277d 290a  rmat': 'html'}).
-00000330: 7072 696e 7428 7265 7375 6c74 2c20 7265  print(result, re
-00000340: 7370 6f6e 7365 290a 6060 600a 0a23 2323  sponse).```..###
-00000350: 2058 4175 7468 0a0a 6060 6070 7974 686f   XAuth..```pytho
-00000360: 6e0a 6666 203d 2046 616e 666f 7528 0a20  n.ff = Fanfou(. 
-00000370: 2063 6f6e 7375 6d65 725f 6b65 793d 2727   consumer_key=''
-00000380: 2c0a 2020 636f 6e73 756d 6572 5f73 6563  ,.  consumer_sec
-00000390: 7265 743d 2727 2c0a 2020 7573 6572 6e61  ret='',.  userna
-000003a0: 6d65 3d27 272c 0a20 2070 6173 7377 6f72  me='',.  passwor
-000003b0: 643d 2727 0a29 0a0a 746f 6b65 6e2c 2072  d=''.)..token, r
-000003c0: 6573 706f 6e73 6520 3d20 6666 2e78 6175  esponse = ff.xau
-000003d0: 7468 2829 0a70 7269 6e74 2874 6f6b 656e  th().print(token
-000003e0: 2c20 7265 7370 6f6e 7365 290a 0a74 696d  , response)..tim
-000003f0: 656c 696e 652c 205f 203d 2066 662e 6765  eline, _ = ff.ge
-00000400: 7428 272f 7374 6174 7573 6573 2f70 7562  t('/statuses/pub
-00000410: 6c69 635f 7469 6d65 6c69 6e65 272c 207b  lic_timeline', {
-00000420: 2763 6f75 6e74 273a 2031 307d 290a 7072  'count': 10}).pr
-00000430: 696e 7428 7469 6d65 6c69 6e65 290a 0a73  int(timeline)..s
-00000440: 7461 7475 732c 205f 203d 2066 662e 706f  tatus, _ = ff.po
-00000450: 7374 2827 2f73 7461 7475 7365 732f 7570  st('/statuses/up
-00000460: 6461 7465 272c 207b 2773 7461 7475 7327  date', {'status'
-00000470: 3a20 2748 6920 4661 6e66 6f75 277d 290a  : 'Hi Fanfou'}).
-00000480: 7072 696e 7428 7374 6174 7573 290a 6060  print(status).``
-00000490: 600a 0a23 2323 204f 7074 696f 6e73 0a0a  `..### Options..
-000004a0: 2d20 6063 6f6e 7375 6d65 725f 6b65 7960  - `consumer_key`
-000004b0: 3a20 5468 6520 636f 6e73 756d 6572 206b  : The consumer k
-000004c0: 6579 0a2d 2060 636f 6e73 756d 6572 5f73  ey.- `consumer_s
-000004d0: 6563 7265 7460 3a20 5468 6520 636f 6e73  ecret`: The cons
-000004e0: 756d 6572 2073 6563 7265 740a 2d20 606f  umer secret.- `o
-000004f0: 6175 7468 5f74 6f6b 656e 603a 2054 6865  auth_token`: The
-00000500: 204f 4175 7468 2074 6f6b 656e 0a2d 2060   OAuth token.- `
-00000510: 6f61 7574 685f 746f 6b65 6e5f 7365 6372  oauth_token_secr
-00000520: 6574 603a 2054 6865 204f 4175 7468 2074  et`: The OAuth t
-00000530: 6f6b 656e 2073 6563 7265 740a 2d20 6075  oken secret.- `u
-00000540: 7365 726e 616d 6560 3a20 5468 6520 4661  sername`: The Fa
-00000550: 6e66 6f75 2075 7365 726e 616d 650a 2d20  nfou username.- 
-00000560: 6070 6173 7377 6f72 6460 3a20 5468 6520  `password`: The 
-00000570: 4661 6e66 6f75 2070 6173 7377 6f72 640a  Fanfou password.
-00000580: 2d20 6070 726f 746f 636f 6c60 3a20 5365  - `protocol`: Se
-00000590: 7420 7468 6520 7072 6f74 6f74 6f6c 2c20  t the prototol, 
-000005a0: 6465 6661 756c 7420 6973 2060 6874 7470  default is `http
-000005b0: 3a60 0a2d 2060 6170 695f 646f 6d61 696e  :`.- `api_domain
-000005c0: 603a 2053 6574 2074 6865 2041 5049 2064  `: Set the API d
-000005d0: 6f6d 6169 6e2c 2064 6566 6175 6c74 2069  omain, default i
-000005e0: 7320 6061 7069 2e66 616e 666f 752e 636f  s `api.fanfou.co
-000005f0: 6d60 0a2d 2060 6f61 7574 685f 6f6d 6169  m`.- `oauth_omai
-00000600: 6e60 3a20 5365 7420 7468 6520 4f41 7574  n`: Set the OAut
-00000610: 6820 646f 6d61 696e 2c20 6465 6661 756c  h domain, defaul
-00000620: 7420 6973 2060 6661 6e66 6f75 2e63 6f6d  t is `fanfou.com
-00000630: 600a 2d20 6068 6f6f 6b73 603a 2048 6f6f  `.- `hooks`: Hoo
-00000640: 6b73 2061 6c6c 6f77 206d 6f64 6966 6963  ks allow modific
-00000650: 6174 696f 6e73 2077 6974 6820 4f41 7574  ations with OAut
-00000660: 680a 0a3e 2046 6f72 206d 6f72 6520 4661  h..> For more Fa
-00000670: 6e66 6f75 2041 5049 2064 6f63 732c 2073  nfou API docs, s
-00000680: 6565 2074 6865 205b 4661 6e66 6f75 2041  ee the [Fanfou A
-00000690: 5049 2064 6f63 5d28 6874 7470 733a 2f2f  PI doc](https://
-000006a0: 6769 7468 7562 2e63 6f6d 2f46 616e 666f  github.com/Fanfo
-000006b0: 7541 5049 2f46 616e 466f 7541 5049 446f  uAPI/FanFouAPIDo
-000006c0: 632f 7769 6b69 292e 0a0a 2323 2041 5049  c/wiki)...## API
-000006d0: 0a0a 6060 600a 6666 2e72 6571 7565 7374  ..```.ff.request
-000006e0: 5f74 6f6b 656e 2829 0a66 662e 6163 6365  _token().ff.acce
-000006f0: 7373 5f74 6f6b 656e 2874 6f6b 656e 290a  ss_token(token).
-00000700: 6666 2e78 6175 7468 2829 0a66 662e 6765  ff.xauth().ff.ge
-00000710: 7428 7572 692c 2070 6172 616d 733d 7b7d  t(uri, params={}
-00000720: 290a 6666 2e70 6f73 7428 7572 692c 2070  ).ff.post(uri, p
-00000730: 6172 616d 733d 7b7d 2c20 6669 6c65 733d  arams={}, files=
-00000740: 4e6f 6e65 290a 6060 600a 0a23 2323 2045  None).```..### E
-00000750: 7861 6d70 6c65 730a 0a60 6060 7079 7468  xamples..```pyth
-00000760: 6f6e 0a23 2047 6574 2072 6571 7565 7374  on.# Get request
-00000770: 2074 6f6b 656e 0a74 6f6b 656e 2c20 5f20   token.token, _ 
-00000780: 3d20 6666 2e72 6571 7565 7374 5f74 6f6b  = ff.request_tok
-00000790: 656e 2829 0a70 7269 6e74 2874 6f6b 656e  en().print(token
-000007a0: 290a 0a23 2047 6574 2061 6363 6573 7320  )..# Get access 
-000007b0: 746f 6b65 6e0a 746f 6b65 6e2c 205f 203d  token.token, _ =
-000007c0: 2066 662e 6163 6365 7373 5f74 6f6b 656e   ff.access_token
-000007d0: 2829 0a70 7269 6e74 2874 6f6b 656e 290a  ().print(token).
-000007e0: 0a23 2047 6574 2074 696d 656c 696e 650a  .# Get timeline.
-000007f0: 746c 2c20 5f20 3d20 6666 2e67 6574 2827  tl, _ = ff.get('
-00000800: 2f73 7461 7475 7365 732f 686f 6d65 5f74  /statuses/home_t
-00000810: 696d 656c 696e 6527 290a 7072 696e 7428  imeline').print(
-00000820: 746c 290a 0a23 2050 6f73 7420 7374 6174  tl)..# Post stat
-00000830: 7573 0a73 742c 205f 203d 2066 662e 706f  us.st, _ = ff.po
-00000840: 7374 2827 2f73 7461 7475 7365 732f 7570  st('/statuses/up
-00000850: 6461 7465 272c 207b 7374 6174 7573 3a20  date', {status: 
-00000860: 2768 6920 666c 6f72 6127 7d29 0a70 7269  'hi flora'}).pri
-00000870: 6e74 2873 7429 0a0a 2320 5570 6c6f 6164  nt(st)..# Upload
-00000880: 2070 686f 746f 0a73 742c 205f 203d 2066   photo.st, _ = f
-00000890: 662e 706f 7374 280a 2020 272f 7068 6f74  f.post(.  '/phot
-000008a0: 6f73 2f75 706c 6f61 6427 2c0a 2020 7061  os/upload',.  pa
-000008b0: 7261 6d73 3d7b 2773 7461 7475 7327 3a20  rams={'status': 
-000008c0: 2775 6e69 636f 726e 277d 2c0a 2020 6669  'unicorn'},.  fi
-000008d0: 6c65 733d 7b27 7068 6f74 6f27 3a20 6f70  les={'photo': op
-000008e0: 656e 2827 6669 6c65 5f70 6174 6827 2c20  en('file_path', 
-000008f0: 2772 6227 297d 0a29 0a70 7269 6e74 2873  'rb')}.).print(s
-00000900: 7429 0a60 6060 0a0a 2323 2320 5469 7073  t).```..### Tips
-00000910: 0a0a 5573 6520 6068 6f6f 6b73 6020 666f  ..Use `hooks` fo
-00000920: 7220 796f 7572 2072 6576 6572 7365 2d70  r your reverse-p
-00000930: 726f 7879 2073 6572 7665 720a 0a60 6060  roxy server..```
-00000940: 7079 7468 6f6e 0a66 6620 3d20 4661 6e66  python.ff = Fanf
-00000950: 6f75 280a 2020 636f 6e73 756d 6572 5f6b  ou(.  consumer_k
-00000960: 6579 3d27 272c 0a20 2063 6f6e 7375 6d65  ey='',.  consume
-00000970: 725f 7365 6372 6574 3d27 272c 0a20 206f  r_secret='',.  o
-00000980: 6175 7468 5f74 6f6b 656e 3d27 272c 0a20  auth_token='',. 
-00000990: 206f 6175 7468 5f74 6f6b 656e 5f73 6563   oauth_token_sec
-000009a0: 7265 743d 2727 2c0a 2020 6170 695f 646f  ret='',.  api_do
-000009b0: 6d61 696e 3d27 6170 692e 6578 616d 706c  main='api.exampl
-000009c0: 652e 636f 6d27 2c0a 2020 6f61 7574 685f  e.com',.  oauth_
-000009d0: 646f 6d61 696e 3d27 6578 616d 706c 652e  domain='example.
-000009e0: 636f 6d27 2c0a 2020 686f 6f6b 733d 7b0a  com',.  hooks={.
-000009f0: 2020 2020 2762 6173 655f 7374 7269 6e67      'base_string
-00000a00: 273a 206c 616d 6264 6120 733a 2073 2e72  ': lambda s: s.r
-00000a10: 6570 6c61 6365 2827 6578 616d 706c 652e  eplace('example.
-00000a20: 636f 6d27 2c20 2766 616e 666f 752e 636f  com', 'fanfou.co
-00000a30: 6d27 290a 2020 7d0a 290a 6060 600a 0a23  m').  }.).```..#
-00000a40: 2320 5265 6c61 7465 640a 0a2d 205b 6661  # Related..- [fa
-00000a50: 6e66 6f75 2d73 646b 2d6e 6f64 655d 2868  nfou-sdk-node](h
-00000a60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000a70: 6d2f 6661 6e66 6f75 6a73 2f66 616e 666f  m/fanfoujs/fanfo
-00000a80: 752d 7364 6b2d 6e6f 6465 2920 2d20 4661  u-sdk-node) - Fa
-00000a90: 6e66 6f75 2053 444b 2066 6f72 204e 6f64  nfou SDK for Nod
-00000aa0: 652e 6a73 0a2d 205b 6661 6e66 6f75 2d73  e.js.- [fanfou-s
-00000ab0: 646b 2d62 726f 7773 6572 5d28 6874 7470  dk-browser](http
-00000ac0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
-00000ad0: 616e 666f 756a 732f 6661 6e66 6f75 2d73  anfoujs/fanfou-s
-00000ae0: 646b 2d62 726f 7773 6572 2920 2d20 4661  dk-browser) - Fa
-00000af0: 6e66 6f75 2053 444b 2066 6f72 2062 726f  nfou SDK for bro
-00000b00: 7773 6572 0a2d 205b 6661 6e66 6f75 2d73  wser.- [fanfou-s
-00000b10: 646b 2d77 6561 7070 5d28 6874 7470 733a  dk-weapp](https:
-00000b20: 2f2f 6769 7468 7562 2e63 6f6d 2f66 616e  //github.com/fan
-00000b30: 666f 756a 732f 6661 6e66 6f75 2d73 646b  foujs/fanfou-sdk
-00000b40: 2d77 6561 7070 2920 2d20 4661 6e66 6f75  -weapp) - Fanfou
-00000b50: 2053 444b 2066 6f72 2057 6541 7070 0a0a   SDK for WeApp..
-00000b60: 2323 204c 6963 656e 7365 0a0a 4d49 540a  ## License..MIT.
+00000180: 6c6c 0a0a 6060 6073 6865 6c6c 0a70 6970  ll..```shell.pip
+00000190: 2069 6e73 7461 6c6c 2066 616e 666f 755f   install fanfou_
+000001a0: 7364 6b0a 6060 600a 0a23 2320 5573 6167  sdk.```..## Usag
+000001b0: 650a 0a23 2323 204f 4175 7468 0a0a 6060  e..### OAuth..``
+000001c0: 6070 7974 686f 6e0a 6672 6f6d 2066 616e  `python.from fan
+000001d0: 666f 755f 7364 6b20 696d 706f 7274 2046  fou_sdk import F
+000001e0: 616e 666f 750a 0a66 6620 3d20 4661 6e66  anfou..ff = Fanf
+000001f0: 6f75 280a 2020 2020 636f 6e73 756d 6572  ou(.    consumer
+00000200: 5f6b 6579 3d27 272c 0a20 2020 2063 6f6e  _key='',.    con
+00000210: 7375 6d65 725f 7365 6372 6574 3d27 272c  sumer_secret='',
+00000220: 0a20 2020 206f 6175 7468 5f74 6f6b 656e  .    oauth_token
+00000230: 3d27 272c 0a20 2020 206f 6175 7468 5f74  ='',.    oauth_t
+00000240: 6f6b 656e 5f73 6563 7265 743d 2727 0a29  oken_secret=''.)
+00000250: 0a0a 7265 7375 6c74 2c20 7265 7370 6f6e  ..result, respon
+00000260: 7365 203d 2066 662e 6765 7428 272f 7374  se = ff.get('/st
+00000270: 6174 7573 6573 2f68 6f6d 655f 7469 6d65  atuses/home_time
+00000280: 6c69 6e65 272c 207b 2766 6f72 6d61 7427  line', {'format'
+00000290: 3a20 2768 746d 6c27 7d29 0a70 7269 6e74  : 'html'}).print
+000002a0: 2872 6573 756c 742c 2072 6573 706f 6e73  (result, respons
+000002b0: 6529 0a60 6060 0a0a 2323 2320 5841 7574  e).```..### XAut
+000002c0: 680a 0a60 6060 7079 7468 6f6e 0a66 6620  h..```python.ff 
+000002d0: 3d20 4661 6e66 6f75 280a 2020 636f 6e73  = Fanfou(.  cons
+000002e0: 756d 6572 5f6b 6579 3d27 272c 0a20 2063  umer_key='',.  c
+000002f0: 6f6e 7375 6d65 725f 7365 6372 6574 3d27  onsumer_secret='
+00000300: 272c 0a20 2075 7365 726e 616d 653d 2727  ',.  username=''
+00000310: 2c0a 2020 7061 7373 776f 7264 3d27 270a  ,.  password=''.
+00000320: 290a 0a74 6f6b 656e 2c20 7265 7370 6f6e  )..token, respon
+00000330: 7365 203d 2066 662e 7861 7574 6828 290a  se = ff.xauth().
+00000340: 7072 696e 7428 746f 6b65 6e2c 2072 6573  print(token, res
+00000350: 706f 6e73 6529 0a0a 7469 6d65 6c69 6e65  ponse)..timeline
+00000360: 2c20 5f20 3d20 6666 2e67 6574 2827 2f73  , _ = ff.get('/s
+00000370: 7461 7475 7365 732f 7075 626c 6963 5f74  tatuses/public_t
+00000380: 696d 656c 696e 6527 2c20 7b27 636f 756e  imeline', {'coun
+00000390: 7427 3a20 3130 7d29 0a70 7269 6e74 2874  t': 10}).print(t
+000003a0: 696d 656c 696e 6529 0a0a 7374 6174 7573  imeline)..status
+000003b0: 2c20 5f20 3d20 6666 2e70 6f73 7428 272f  , _ = ff.post('/
+000003c0: 7374 6174 7573 6573 2f75 7064 6174 6527  statuses/update'
+000003d0: 2c20 7b27 7374 6174 7573 273a 2027 4869  , {'status': 'Hi
+000003e0: 2046 616e 666f 7527 7d29 0a70 7269 6e74   Fanfou'}).print
+000003f0: 2873 7461 7475 7329 0a60 6060 0a0a 2323  (status).```..##
+00000400: 2320 4f70 7469 6f6e 730a 0a2d 2060 636f  # Options..- `co
+00000410: 6e73 756d 6572 5f6b 6579 603a 2054 6865  nsumer_key`: The
+00000420: 2063 6f6e 7375 6d65 7220 6b65 790a 2d20   consumer key.- 
+00000430: 6063 6f6e 7375 6d65 725f 7365 6372 6574  `consumer_secret
+00000440: 603a 2054 6865 2063 6f6e 7375 6d65 7220  `: The consumer 
+00000450: 7365 6372 6574 0a2d 2060 6f61 7574 685f  secret.- `oauth_
+00000460: 746f 6b65 6e60 3a20 5468 6520 4f41 7574  token`: The OAut
+00000470: 6820 746f 6b65 6e0a 2d20 606f 6175 7468  h token.- `oauth
+00000480: 5f74 6f6b 656e 5f73 6563 7265 7460 3a20  _token_secret`: 
+00000490: 5468 6520 4f41 7574 6820 746f 6b65 6e20  The OAuth token 
+000004a0: 7365 6372 6574 0a2d 2060 7573 6572 6e61  secret.- `userna
+000004b0: 6d65 603a 2054 6865 2046 616e 666f 7520  me`: The Fanfou 
+000004c0: 7573 6572 6e61 6d65 0a2d 2060 7061 7373  username.- `pass
+000004d0: 776f 7264 603a 2054 6865 2046 616e 666f  word`: The Fanfo
+000004e0: 7520 7061 7373 776f 7264 0a2d 2060 7072  u password.- `pr
+000004f0: 6f74 6f63 6f6c 603a 2053 6574 2074 6865  otocol`: Set the
+00000500: 2070 726f 746f 746f 6c2c 2064 6566 6175   prototol, defau
+00000510: 6c74 2069 7320 6068 7474 703a 600a 2d20  lt is `http:`.- 
+00000520: 6061 7069 5f64 6f6d 6169 6e60 3a20 5365  `api_domain`: Se
+00000530: 7420 7468 6520 4150 4920 646f 6d61 696e  t the API domain
+00000540: 2c20 6465 6661 756c 7420 6973 2060 6170  , default is `ap
+00000550: 692e 6661 6e66 6f75 2e63 6f6d 600a 2d20  i.fanfou.com`.- 
+00000560: 606f 6175 7468 5f6f 6d61 696e 603a 2053  `oauth_omain`: S
+00000570: 6574 2074 6865 204f 4175 7468 2064 6f6d  et the OAuth dom
+00000580: 6169 6e2c 2064 6566 6175 6c74 2069 7320  ain, default is 
+00000590: 6066 616e 666f 752e 636f 6d60 0a2d 2060  `fanfou.com`.- `
+000005a0: 686f 6f6b 7360 3a20 486f 6f6b 7320 616c  hooks`: Hooks al
+000005b0: 6c6f 7720 6d6f 6469 6669 6361 7469 6f6e  low modification
+000005c0: 7320 7769 7468 204f 4175 7468 0a0a 3e20  s with OAuth..> 
+000005d0: 466f 7220 6d6f 7265 2046 616e 666f 7520  For more Fanfou 
+000005e0: 4150 4920 646f 6373 2c20 7365 6520 7468  API docs, see th
+000005f0: 6520 5b46 616e 666f 7520 4150 4920 646f  e [Fanfou API do
+00000600: 635d 2868 7474 7073 3a2f 2f67 6974 6875  c](https://githu
+00000610: 622e 636f 6d2f 4661 6e66 6f75 4150 492f  b.com/FanfouAPI/
+00000620: 4661 6e46 6f75 4150 4944 6f63 2f77 696b  FanFouAPIDoc/wik
+00000630: 6929 2e0a 0a23 2320 4150 490a 0a60 6060  i)...## API..```
+00000640: 0a66 662e 7265 7175 6573 745f 746f 6b65  .ff.request_toke
+00000650: 6e28 290a 6666 2e61 6363 6573 735f 746f  n().ff.access_to
+00000660: 6b65 6e28 746f 6b65 6e29 0a66 662e 7861  ken(token).ff.xa
+00000670: 7574 6828 290a 6666 2e67 6574 2875 7269  uth().ff.get(uri
+00000680: 2c20 7061 7261 6d73 3d7b 7d29 0a66 662e  , params={}).ff.
+00000690: 706f 7374 2875 7269 2c20 7061 7261 6d73  post(uri, params
+000006a0: 3d7b 7d2c 2066 696c 6573 3d4e 6f6e 6529  ={}, files=None)
+000006b0: 0a60 6060 0a0a 2323 2320 4578 616d 706c  .```..### Exampl
+000006c0: 6573 0a0a 6060 6070 7974 686f 6e0a 2320  es..```python.# 
+000006d0: 4765 7420 7265 7175 6573 7420 746f 6b65  Get request toke
+000006e0: 6e0a 746f 6b65 6e2c 205f 203d 2066 662e  n.token, _ = ff.
+000006f0: 7265 7175 6573 745f 746f 6b65 6e28 290a  request_token().
+00000700: 7072 696e 7428 746f 6b65 6e29 0a0a 2320  print(token)..# 
+00000710: 4765 7420 6163 6365 7373 2074 6f6b 656e  Get access token
+00000720: 0a74 6f6b 656e 2c20 5f20 3d20 6666 2e61  .token, _ = ff.a
+00000730: 6363 6573 735f 746f 6b65 6e28 290a 7072  ccess_token().pr
+00000740: 696e 7428 746f 6b65 6e29 0a0a 2320 4765  int(token)..# Ge
+00000750: 7420 7469 6d65 6c69 6e65 0a74 6c2c 205f  t timeline.tl, _
+00000760: 203d 2066 662e 6765 7428 272f 7374 6174   = ff.get('/stat
+00000770: 7573 6573 2f68 6f6d 655f 7469 6d65 6c69  uses/home_timeli
+00000780: 6e65 2729 0a70 7269 6e74 2874 6c29 0a0a  ne').print(tl)..
+00000790: 2320 506f 7374 2073 7461 7475 730a 7374  # Post status.st
+000007a0: 2c20 5f20 3d20 6666 2e70 6f73 7428 272f  , _ = ff.post('/
+000007b0: 7374 6174 7573 6573 2f75 7064 6174 6527  statuses/update'
+000007c0: 2c20 7b73 7461 7475 733a 2027 6869 2066  , {status: 'hi f
+000007d0: 6c6f 7261 277d 290a 7072 696e 7428 7374  lora'}).print(st
+000007e0: 290a 0a23 2055 706c 6f61 6420 7068 6f74  )..# Upload phot
+000007f0: 6f0a 7374 2c20 5f20 3d20 6666 2e70 6f73  o.st, _ = ff.pos
+00000800: 7428 0a20 2027 2f70 686f 746f 732f 7570  t(.  '/photos/up
+00000810: 6c6f 6164 272c 0a20 2070 6172 616d 733d  load',.  params=
+00000820: 7b27 7374 6174 7573 273a 2027 756e 6963  {'status': 'unic
+00000830: 6f72 6e27 7d2c 0a20 2066 696c 6573 3d7b  orn'},.  files={
+00000840: 2770 686f 746f 273a 206f 7065 6e28 2766  'photo': open('f
+00000850: 696c 655f 7061 7468 272c 2027 7262 2729  ile_path', 'rb')
+00000860: 7d0a 290a 7072 696e 7428 7374 290a 6060  }.).print(st).``
+00000870: 600a 0a23 2323 2054 6970 730a 0a55 7365  `..### Tips..Use
+00000880: 2060 686f 6f6b 7360 2066 6f72 2079 6f75   `hooks` for you
+00000890: 7220 7265 7665 7273 652d 7072 6f78 7920  r reverse-proxy 
+000008a0: 7365 7276 6572 0a0a 6060 6070 7974 686f  server..```pytho
+000008b0: 6e0a 6666 203d 2046 616e 666f 7528 0a20  n.ff = Fanfou(. 
+000008c0: 2063 6f6e 7375 6d65 725f 6b65 793d 2727   consumer_key=''
+000008d0: 2c0a 2020 636f 6e73 756d 6572 5f73 6563  ,.  consumer_sec
+000008e0: 7265 743d 2727 2c0a 2020 6f61 7574 685f  ret='',.  oauth_
+000008f0: 746f 6b65 6e3d 2727 2c0a 2020 6f61 7574  token='',.  oaut
+00000900: 685f 746f 6b65 6e5f 7365 6372 6574 3d27  h_token_secret='
+00000910: 272c 0a20 2061 7069 5f64 6f6d 6169 6e3d  ',.  api_domain=
+00000920: 2761 7069 2e65 7861 6d70 6c65 2e63 6f6d  'api.example.com
+00000930: 272c 0a20 206f 6175 7468 5f64 6f6d 6169  ',.  oauth_domai
+00000940: 6e3d 2765 7861 6d70 6c65 2e63 6f6d 272c  n='example.com',
+00000950: 0a20 2068 6f6f 6b73 3d7b 0a20 2020 2027  .  hooks={.    '
+00000960: 6261 7365 5f73 7472 696e 6727 3a20 6c61  base_string': la
+00000970: 6d62 6461 2073 3a20 732e 7265 706c 6163  mbda s: s.replac
+00000980: 6528 2765 7861 6d70 6c65 2e63 6f6d 272c  e('example.com',
+00000990: 2027 6661 6e66 6f75 2e63 6f6d 2729 0a20   'fanfou.com'). 
+000009a0: 207d 0a29 0a60 6060 0a0a 2323 2052 656c   }.).```..## Rel
+000009b0: 6174 6564 0a0a 2d20 5b66 616e 666f 752d  ated..- [fanfou-
+000009c0: 7364 6b2d 6e6f 6465 5d28 6874 7470 733a  sdk-node](https:
+000009d0: 2f2f 6769 7468 7562 2e63 6f6d 2f66 616e  //github.com/fan
+000009e0: 666f 756a 732f 6661 6e66 6f75 2d73 646b  foujs/fanfou-sdk
+000009f0: 2d6e 6f64 6529 202d 2046 616e 666f 7520  -node) - Fanfou 
+00000a00: 5344 4b20 666f 7220 4e6f 6465 2e6a 730a  SDK for Node.js.
+00000a10: 2d20 5b66 616e 666f 752d 7364 6b2d 6465  - [fanfou-sdk-de
+00000a20: 6e6f 5d28 6874 7470 733a 2f2f 6769 7468  no](https://gith
+00000a30: 7562 2e63 6f6d 2f4c 6974 6f4d 6f72 652f  ub.com/LitoMore/
+00000a40: 6661 6e66 6f75 2d73 646b 2d64 656e 6f29  fanfou-sdk-deno)
+00000a50: 202d 2046 616e 666f 7520 5344 4b20 666f   - Fanfou SDK fo
+00000a60: 7220 4465 6e6f 0a2d 205b 6661 6e66 6f75  r Deno.- [fanfou
+00000a70: 2d73 646b 2d62 726f 7773 6572 5d28 6874  -sdk-browser](ht
+00000a80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000a90: 2f66 616e 666f 756a 732f 6661 6e66 6f75  /fanfoujs/fanfou
+00000aa0: 2d73 646b 2d62 726f 7773 6572 2920 2d20  -sdk-browser) - 
+00000ab0: 4661 6e66 6f75 2053 444b 2066 6f72 2062  Fanfou SDK for b
+00000ac0: 726f 7773 6572 0a2d 205b 6661 6e66 6f75  rowser.- [fanfou
+00000ad0: 2d73 646b 2d77 6561 7070 5d28 6874 7470  -sdk-weapp](http
+00000ae0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f66  s://github.com/f
+00000af0: 616e 666f 756a 732f 6661 6e66 6f75 2d73  anfoujs/fanfou-s
+00000b00: 646b 2d77 6561 7070 2920 2d20 4661 6e66  dk-weapp) - Fanf
+00000b10: 6f75 2053 444b 2066 6f72 2057 6541 7070  ou SDK for WeApp
+00000b20: 0a0a 2323 204c 6963 656e 7365 0a0a 4d49  ..## License..MI
+00000b30: 540a                                     T.
```

### Comparing `fanfou_sdk-0.0.2/setup.py` & `fanfou_sdk-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
-import fanfou_sdk
 
 DESC = open('README.md').read()
 
 setup(name='fanfou_sdk',
-      version='0.0.2',
+      version='0.0.3',
       description='Fanfou SDK for Python',
       author='LitoMore',
       author_email='litomore@gmail.com',
       url='https://github.com/LitoMore/fanfou-sdk-python',
       packages=['fanfou_sdk'],
       install_requires=['six', 'requests'],
       long_description=DESC,
```

