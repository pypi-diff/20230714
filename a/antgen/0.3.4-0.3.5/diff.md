# Comparing `tmp/antgen-0.3.4.tar.gz` & `tmp/antgen-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\antgen-0.3.4.tar", last modified: Fri Jul 14 16:45:53 2023, max compression
+gzip compressed data, was "dist\antgen-0.3.5.tar", last modified: Fri Jul 14 16:50:05 2023, max compression
```

## Comparing `antgen-0.3.4.tar` & `antgen-0.3.5.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/
--rw-rw-rw-   0        0        0      500 2023-07-14 16:45:53.000000 antgen-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    18211 2023-07-14 13:41:32.000000 antgen-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/
--rw-rw-rw-   0        0        0    18871 2023-07-14 13:41:32.000000 antgen-0.3.4/antgen/ActivityModel.py
--rw-rw-rw-   0        0        0     5871 2023-07-14 13:41:32.000000 antgen-0.3.4/antgen/ApplianceModel.py
--rw-rw-rw-   0        0        0     1091 2022-10-04 15:48:11.000000 antgen-0.3.4/antgen/LICENSE
--rw-rw-rw-   0        0        0     7913 2023-07-14 13:41:32.000000 antgen-0.3.4/antgen/LoadModelComponents.py
--rw-rw-rw-   0        0        0     4936 2023-07-14 13:41:32.000000 antgen-0.3.4/antgen/Tools.py
--rw-rw-rw-   0        0        0     6013 2023-07-14 13:41:32.000000 antgen-0.3.4/antgen/UserModel.py
--rw-rw-rw-   0        0        0       76 2022-10-05 22:20:56.000000 antgen-0.3.4/antgen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/activities/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/activities/HOUSEHOLD/
--rw-rw-rw-   0        0        0     3401 2023-07-14 13:41:34.000000 antgen-0.3.4/antgen/activities/HOUSEHOLD/dry_clothes.conf
--rw-rw-rw-   0        0        0      313 2023-07-14 13:41:34.000000 antgen-0.3.4/antgen/activities/HOUSEHOLD/ironing.conf
--rw-rw-rw-   0        0        0      316 2023-07-14 13:41:34.000000 antgen-0.3.4/antgen/activities/HOUSEHOLD/vacuum.conf
--rw-rw-rw-   0        0        0     3410 2023-07-14 13:41:34.000000 antgen-0.3.4/antgen/activities/HOUSEHOLD/wash_laundry.conf
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/activities/KITCHEN/
--rw-rw-rw-   0        0        0      449 2023-07-14 13:41:34.000000 antgen-0.3.4/antgen/activities/KITCHEN/dishwasher.conf
--rw-rw-rw-   0        0        0      456 2023-07-14 13:41:34.000000 antgen-0.3.4/antgen/activities/KITCHEN/fried_egg.conf
--rw-rw-rw-   0        0        0      322 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/activities/KITCHEN/heating_lunch.conf
--rw-rw-rw-   0        0        0     1294 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/activities/KITCHEN/preparing_breakfast.conf
--rw-rw-rw-   0        0        0      601 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/activities/KITCHEN/preparing_dinner.conf
--rw-rw-rw-   0        0        0      449 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/activities/KITCHEN/refrigerator.conf
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/activities/LEISURE/
--rw-rw-rw-   0        0        0      473 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/activities/LEISURE/listen_music.conf
--rw-rw-rw-   0        0        0      321 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/activities/LEISURE/use_pc.conf
--rw-rw-rw-   0        0        0      434 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/activities/LEISURE/watch_tv.conf
--rw-rw-rw-   0        0        0    19213 2023-07-14 13:41:32.000000 antgen-0.3.4/antgen/antgen.py
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/AMPLIFIER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/AMPLIFIER/dev_AF6490/
--rw-rw-rw-   0        0        0      586 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/appliances/AMPLIFIER/dev_AF6490/mode0
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/BREADCUTTER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/BREADCUTTER/dev_B7DF9D/
--rw-rw-rw-   0        0        0      182 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/appliances/BREADCUTTER/dev_B7DF9D/mode0
--rw-rw-rw-   0        0        0      182 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/appliances/BREADCUTTER/dev_B7DF9D/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/CDPLAYER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/CDPLAYER/dev_C3E6D1/
--rw-rw-rw-   0        0        0      523 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/appliances/CDPLAYER/dev_C3E6D1/mode0
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/COFFEEMAKER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/COFFEEMAKER/ECO-H1/
--rw-rw-rw-   0        0        0     3087 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/appliances/COFFEEMAKER/ECO-H1/mode0
--rw-rw-rw-   0        0        0     3319 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/appliances/COFFEEMAKER/ECO-H1/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/COFFEEMAKER/dev_735E9D/
--rw-rw-rw-   0        0        0     3208 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/appliances/COFFEEMAKER/dev_735E9D/mode0
--rw-rw-rw-   0        0        0     3101 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/appliances/COFFEEMAKER/dev_735E9D/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/COOKINGSTOVE/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/COOKINGSTOVE/dev_D33097/
--rw-rw-rw-   0        0        0      591 2023-07-14 13:41:35.000000 antgen-0.3.4/antgen/appliances/COOKINGSTOVE/dev_D33097/mode0
--rw-rw-rw-   0        0        0      379 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/COOKINGSTOVE/dev_D33097/mode1
--rw-rw-rw-   0        0        0      511 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/COOKINGSTOVE/dev_D33097/mode2
--rw-rw-rw-   0        0        0      381 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/COOKINGSTOVE/dev_D33097/mode3
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/DISHWASHER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/DISHWASHER/dev_995BAC/
--rw-rw-rw-   0        0        0      788 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/DISHWASHER/dev_995BAC/mode0
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/DRYER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/DRYER/ECO-H1/
--rw-rw-rw-   0        0        0     1185 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/DRYER/ECO-H1/mode0
--rw-rw-rw-   0        0        0     1564 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/DRYER/ECO-H1/mode1
--rw-rw-rw-   0        0        0     1452 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/DRYER/ECO-H1/mode2
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/FREEZER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/
--rw-rw-rw-   0        0        0      981 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode0
--rw-rw-rw-   0        0        0      914 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode1
--rw-rw-rw-   0        0        0      753 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode2
--rw-rw-rw-   0        0        0     1197 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode3
--rw-rw-rw-   0        0        0      804 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode4
--rw-rw-rw-   0        0        0      693 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode5
--rw-rw-rw-   0        0        0      693 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode6
--rw-rw-rw-   0        0        0      651 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode7
--rw-rw-rw-   0        0        0      957 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode8
--rw-rw-rw-   0        0        0      738 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode9
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/IRON/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/IRON/dev_D337C2/
--rw-rw-rw-   0        0        0     5229 2023-07-14 13:41:36.000000 antgen-0.3.4/antgen/appliances/IRON/dev_D337C2/mode0
--rw-rw-rw-   0        0        0     5897 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/IRON/dev_D337C2/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/KETTLE/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/KETTLE/ECO-H1/
--rw-rw-rw-   0        0        0      417 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/KETTLE/ECO-H1/mode0
--rw-rw-rw-   0        0        0     1079 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/KETTLE/ECO-H1/mode1
--rw-rw-rw-   0        0        0     1050 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/KETTLE/ECO-H1/mode2
--rw-rw-rw-   0        0        0      676 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/KETTLE/ECO-H1/mode3
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/KETTLE/dev_5AE2CA/
--rw-rw-rw-   0        0        0      376 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/KETTLE/dev_5AE2CA/mode0
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/MICROWAVE/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/MICROWAVE/dev_98A0D3/
--rw-rw-rw-   0        0        0      483 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/MICROWAVE/dev_98A0D3/mode0
--rw-rw-rw-   0        0        0     1146 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/MICROWAVE/dev_98A0D3/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/PC/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/PC/Desktop_Denis/
--rw-rw-rw-   0        0        0     1644 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/PC/Desktop_Denis/mode0
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/PC/ECO-H1/
--rw-rw-rw-   0        0        0     1072 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/PC/ECO-H1/mode0
--rw-rw-rw-   0        0        0     2503 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/PC/ECO-H1/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/PRINTER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/PRINTER/dev_11F01E/
--rw-rw-rw-   0        0        0     1592 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/PRINTER/dev_11F01E/mode0
--rw-rw-rw-   0        0        0     2638 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/PRINTER/dev_11F01E/mode1
--rw-rw-rw-   0        0        0      846 2023-07-14 13:41:37.000000 antgen-0.3.4/antgen/appliances/PRINTER/dev_11F01E/mode2
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/
--rw-rw-rw-   0        0        0     1032 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode0
--rw-rw-rw-   0        0        0     1466 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode1
--rw-rw-rw-   0        0        0     1081 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode4
--rw-rw-rw-   0        0        0      961 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode5
--rw-rw-rw-   0        0        0      978 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode6
--rw-rw-rw-   0        0        0     1018 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode7
--rw-rw-rw-   0        0        0      690 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode8
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev20111228/
--rw-rw-rw-   0        0        0     1357 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev20111228/mode0
--rw-rw-rw-   0        0        0     2812 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev20111228/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/
--rw-rw-rw-   0        0        0      393 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode0
--rw-rw-rw-   0        0        0      498 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode1
--rw-rw-rw-   0        0        0      498 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode10
--rw-rw-rw-   0        0        0      497 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode11
--rw-rw-rw-   0        0        0      603 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode12
--rw-rw-rw-   0        0        0      497 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode13
--rw-rw-rw-   0        0        0      498 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode14
--rw-rw-rw-   0        0        0      498 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode15
--rw-rw-rw-   0        0        0     1673 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode16
--rw-rw-rw-   0        0        0      749 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode17
--rw-rw-rw-   0        0        0      602 2023-07-14 13:41:38.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode18
--rw-rw-rw-   0        0        0      498 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode19
--rw-rw-rw-   0        0        0      603 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode2
--rw-rw-rw-   0        0        0      498 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode20
--rw-rw-rw-   0        0        0      603 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode21
--rw-rw-rw-   0        0        0      498 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode22
--rw-rw-rw-   0        0        0      228 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode23
--rw-rw-rw-   0        0        0      497 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode3
--rw-rw-rw-   0        0        0      497 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode4
--rw-rw-rw-   0        0        0      497 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode5
--rw-rw-rw-   0        0        0      498 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode6
--rw-rw-rw-   0        0        0      499 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode7
--rw-rw-rw-   0        0        0      498 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode8
--rw-rw-rw-   0        0        0      499 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode9
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/TOASTER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/TOASTER/dev_98ABD2/
--rw-rw-rw-   0        0        0     2214 2023-07-14 13:41:39.000000 antgen-0.3.4/antgen/appliances/TOASTER/dev_98ABD2/mode0
--rw-rw-rw-   0        0        0      481 2023-07-14 13:41:40.000000 antgen-0.3.4/antgen/appliances/TOASTER/dev_98ABD2/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/TV/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/TV/dev_B80E51/
--rw-rw-rw-   0        0        0     8479 2023-07-14 13:41:40.000000 antgen-0.3.4/antgen/appliances/TV/dev_B80E51/mode0
--rw-rw-rw-   0        0        0     8429 2023-07-14 13:41:40.000000 antgen-0.3.4/antgen/appliances/TV/dev_B80E51/mode1
--rw-rw-rw-   0        0        0     7571 2023-07-14 13:41:40.000000 antgen-0.3.4/antgen/appliances/TV/dev_B80E51/mode2
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/VACUUMCLEANER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/VACUUMCLEANER/device_B7E2F8/
--rw-rw-rw-   0        0        0      448 2023-07-14 13:41:40.000000 antgen-0.3.4/antgen/appliances/VACUUMCLEANER/device_B7E2F8/mode0
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/WASHINGMACHINE/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/WASHINGMACHINE/ECO-H1/
--rw-rw-rw-   0        0        0     4205 2023-07-14 13:41:40.000000 antgen-0.3.4/antgen/appliances/WASHINGMACHINE/ECO-H1/mode2
--rw-rw-rw-   0        0        0     4050 2023-07-14 13:41:40.000000 antgen-0.3.4/antgen/appliances/WASHINGMACHINE/ECO-H1/mode3
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen/appliances/WASHINGMACHINE/_B82E27/
--rw-rw-rw-   0        0        0     9448 2023-07-14 13:41:40.000000 antgen-0.3.4/antgen/appliances/WASHINGMACHINE/_B82E27/mode0
--rw-rw-rw-   0        0        0      220 2023-07-14 13:41:32.000000 antgen-0.3.4/antgen/default.conf
--rw-rw-rw-   0        0        0   144322 2023-07-14 13:41:32.000000 antgen-0.3.4/antgen/example1.png
--rw-rw-rw-   0        0        0   122664 2023-07-14 13:41:32.000000 antgen-0.3.4/antgen/example2.png
--rw-rw-rw-   0        0        0     2807 2023-07-14 13:41:33.000000 antgen-0.3.4/antgen/mapping.conf
--rw-rw-rw-   0        0        0      104 2023-07-14 13:41:33.000000 antgen-0.3.4/antgen/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen.egg-info/
--rw-rw-rw-   0        0        0      500 2023-07-14 16:45:52.000000 antgen-0.3.4/antgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4655 2023-07-14 16:45:53.000000 antgen-0.3.4/antgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 16:45:52.000000 antgen-0.3.4/antgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-14 16:45:52.000000 antgen-0.3.4/antgen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      679 2023-07-14 16:29:12.000000 antgen-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 16:45:53.000000 antgen-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      678 2023-07-14 16:45:35.000000 antgen-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/
+-rw-rw-rw-   0        0        0      500 2023-07-14 16:50:05.000000 antgen-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    18211 2023-07-14 13:41:32.000000 antgen-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/
+-rw-rw-rw-   0        0        0    18871 2023-07-14 13:41:32.000000 antgen-0.3.5/antgen/ActivityModel.py
+-rw-rw-rw-   0        0        0     5871 2023-07-14 13:41:32.000000 antgen-0.3.5/antgen/ApplianceModel.py
+-rw-rw-rw-   0        0        0     1091 2022-10-04 15:48:11.000000 antgen-0.3.5/antgen/LICENSE
+-rw-rw-rw-   0        0        0     7913 2023-07-14 13:41:32.000000 antgen-0.3.5/antgen/LoadModelComponents.py
+-rw-rw-rw-   0        0        0     4936 2023-07-14 13:41:32.000000 antgen-0.3.5/antgen/Tools.py
+-rw-rw-rw-   0        0        0     6013 2023-07-14 13:41:32.000000 antgen-0.3.5/antgen/UserModel.py
+-rw-rw-rw-   0        0        0       76 2022-10-05 22:20:56.000000 antgen-0.3.5/antgen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/activities/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/activities/HOUSEHOLD/
+-rw-rw-rw-   0        0        0     3401 2023-07-14 13:41:34.000000 antgen-0.3.5/antgen/activities/HOUSEHOLD/dry_clothes.conf
+-rw-rw-rw-   0        0        0      313 2023-07-14 13:41:34.000000 antgen-0.3.5/antgen/activities/HOUSEHOLD/ironing.conf
+-rw-rw-rw-   0        0        0      316 2023-07-14 13:41:34.000000 antgen-0.3.5/antgen/activities/HOUSEHOLD/vacuum.conf
+-rw-rw-rw-   0        0        0     3410 2023-07-14 13:41:34.000000 antgen-0.3.5/antgen/activities/HOUSEHOLD/wash_laundry.conf
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/activities/KITCHEN/
+-rw-rw-rw-   0        0        0      449 2023-07-14 13:41:34.000000 antgen-0.3.5/antgen/activities/KITCHEN/dishwasher.conf
+-rw-rw-rw-   0        0        0      456 2023-07-14 13:41:34.000000 antgen-0.3.5/antgen/activities/KITCHEN/fried_egg.conf
+-rw-rw-rw-   0        0        0      322 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/activities/KITCHEN/heating_lunch.conf
+-rw-rw-rw-   0        0        0     1294 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/activities/KITCHEN/preparing_breakfast.conf
+-rw-rw-rw-   0        0        0      601 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/activities/KITCHEN/preparing_dinner.conf
+-rw-rw-rw-   0        0        0      449 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/activities/KITCHEN/refrigerator.conf
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/activities/LEISURE/
+-rw-rw-rw-   0        0        0      473 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/activities/LEISURE/listen_music.conf
+-rw-rw-rw-   0        0        0      321 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/activities/LEISURE/use_pc.conf
+-rw-rw-rw-   0        0        0      434 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/activities/LEISURE/watch_tv.conf
+-rw-rw-rw-   0        0        0    19213 2023-07-14 13:41:32.000000 antgen-0.3.5/antgen/antgen.py
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/AMPLIFIER/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/AMPLIFIER/dev_AF6490/
+-rw-rw-rw-   0        0        0      586 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/appliances/AMPLIFIER/dev_AF6490/mode0
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/BREADCUTTER/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/BREADCUTTER/dev_B7DF9D/
+-rw-rw-rw-   0        0        0      182 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/appliances/BREADCUTTER/dev_B7DF9D/mode0
+-rw-rw-rw-   0        0        0      182 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/appliances/BREADCUTTER/dev_B7DF9D/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/CDPLAYER/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/CDPLAYER/dev_C3E6D1/
+-rw-rw-rw-   0        0        0      523 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/appliances/CDPLAYER/dev_C3E6D1/mode0
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/COFFEEMAKER/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/COFFEEMAKER/ECO-H1/
+-rw-rw-rw-   0        0        0     3087 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/appliances/COFFEEMAKER/ECO-H1/mode0
+-rw-rw-rw-   0        0        0     3319 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/appliances/COFFEEMAKER/ECO-H1/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/COFFEEMAKER/dev_735E9D/
+-rw-rw-rw-   0        0        0     3208 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/appliances/COFFEEMAKER/dev_735E9D/mode0
+-rw-rw-rw-   0        0        0     3101 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/appliances/COFFEEMAKER/dev_735E9D/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/COOKINGSTOVE/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/COOKINGSTOVE/dev_D33097/
+-rw-rw-rw-   0        0        0      591 2023-07-14 13:41:35.000000 antgen-0.3.5/antgen/appliances/COOKINGSTOVE/dev_D33097/mode0
+-rw-rw-rw-   0        0        0      379 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/COOKINGSTOVE/dev_D33097/mode1
+-rw-rw-rw-   0        0        0      511 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/COOKINGSTOVE/dev_D33097/mode2
+-rw-rw-rw-   0        0        0      381 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/COOKINGSTOVE/dev_D33097/mode3
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/DISHWASHER/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/DISHWASHER/dev_995BAC/
+-rw-rw-rw-   0        0        0      788 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/DISHWASHER/dev_995BAC/mode0
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/DRYER/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/DRYER/ECO-H1/
+-rw-rw-rw-   0        0        0     1185 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/DRYER/ECO-H1/mode0
+-rw-rw-rw-   0        0        0     1564 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/DRYER/ECO-H1/mode1
+-rw-rw-rw-   0        0        0     1452 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/DRYER/ECO-H1/mode2
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/FREEZER/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/
+-rw-rw-rw-   0        0        0      981 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode0
+-rw-rw-rw-   0        0        0      914 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode1
+-rw-rw-rw-   0        0        0      753 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode2
+-rw-rw-rw-   0        0        0     1197 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode3
+-rw-rw-rw-   0        0        0      804 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode4
+-rw-rw-rw-   0        0        0      693 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode5
+-rw-rw-rw-   0        0        0      693 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode6
+-rw-rw-rw-   0        0        0      651 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode7
+-rw-rw-rw-   0        0        0      957 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode8
+-rw-rw-rw-   0        0        0      738 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode9
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/IRON/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/IRON/dev_D337C2/
+-rw-rw-rw-   0        0        0     5229 2023-07-14 13:41:36.000000 antgen-0.3.5/antgen/appliances/IRON/dev_D337C2/mode0
+-rw-rw-rw-   0        0        0     5897 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/IRON/dev_D337C2/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/KETTLE/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/KETTLE/ECO-H1/
+-rw-rw-rw-   0        0        0      417 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/KETTLE/ECO-H1/mode0
+-rw-rw-rw-   0        0        0     1079 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/KETTLE/ECO-H1/mode1
+-rw-rw-rw-   0        0        0     1050 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/KETTLE/ECO-H1/mode2
+-rw-rw-rw-   0        0        0      676 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/KETTLE/ECO-H1/mode3
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/KETTLE/dev_5AE2CA/
+-rw-rw-rw-   0        0        0      376 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/KETTLE/dev_5AE2CA/mode0
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/MICROWAVE/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/MICROWAVE/dev_98A0D3/
+-rw-rw-rw-   0        0        0      483 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/MICROWAVE/dev_98A0D3/mode0
+-rw-rw-rw-   0        0        0     1146 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/MICROWAVE/dev_98A0D3/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/PC/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/PC/Desktop_Denis/
+-rw-rw-rw-   0        0        0     1644 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/PC/Desktop_Denis/mode0
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/PC/ECO-H1/
+-rw-rw-rw-   0        0        0     1072 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/PC/ECO-H1/mode0
+-rw-rw-rw-   0        0        0     2503 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/PC/ECO-H1/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/PRINTER/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/PRINTER/dev_11F01E/
+-rw-rw-rw-   0        0        0     1592 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/PRINTER/dev_11F01E/mode0
+-rw-rw-rw-   0        0        0     2638 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/PRINTER/dev_11F01E/mode1
+-rw-rw-rw-   0        0        0      846 2023-07-14 13:41:37.000000 antgen-0.3.5/antgen/appliances/PRINTER/dev_11F01E/mode2
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/
+-rw-rw-rw-   0        0        0     1032 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode0
+-rw-rw-rw-   0        0        0     1466 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode1
+-rw-rw-rw-   0        0        0     1081 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode4
+-rw-rw-rw-   0        0        0      961 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode5
+-rw-rw-rw-   0        0        0      978 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode6
+-rw-rw-rw-   0        0        0     1018 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode7
+-rw-rw-rw-   0        0        0      690 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode8
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev20111228/
+-rw-rw-rw-   0        0        0     1357 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev20111228/mode0
+-rw-rw-rw-   0        0        0     2812 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev20111228/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/
+-rw-rw-rw-   0        0        0      393 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode0
+-rw-rw-rw-   0        0        0      498 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode1
+-rw-rw-rw-   0        0        0      498 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode10
+-rw-rw-rw-   0        0        0      497 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode11
+-rw-rw-rw-   0        0        0      603 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode12
+-rw-rw-rw-   0        0        0      497 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode13
+-rw-rw-rw-   0        0        0      498 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode14
+-rw-rw-rw-   0        0        0      498 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode15
+-rw-rw-rw-   0        0        0     1673 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode16
+-rw-rw-rw-   0        0        0      749 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode17
+-rw-rw-rw-   0        0        0      602 2023-07-14 13:41:38.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode18
+-rw-rw-rw-   0        0        0      498 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode19
+-rw-rw-rw-   0        0        0      603 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode2
+-rw-rw-rw-   0        0        0      498 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode20
+-rw-rw-rw-   0        0        0      603 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode21
+-rw-rw-rw-   0        0        0      498 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode22
+-rw-rw-rw-   0        0        0      228 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode23
+-rw-rw-rw-   0        0        0      497 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode3
+-rw-rw-rw-   0        0        0      497 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode4
+-rw-rw-rw-   0        0        0      497 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode5
+-rw-rw-rw-   0        0        0      498 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode6
+-rw-rw-rw-   0        0        0      499 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode7
+-rw-rw-rw-   0        0        0      498 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode8
+-rw-rw-rw-   0        0        0      499 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode9
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/TOASTER/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/TOASTER/dev_98ABD2/
+-rw-rw-rw-   0        0        0     2214 2023-07-14 13:41:39.000000 antgen-0.3.5/antgen/appliances/TOASTER/dev_98ABD2/mode0
+-rw-rw-rw-   0        0        0      481 2023-07-14 13:41:40.000000 antgen-0.3.5/antgen/appliances/TOASTER/dev_98ABD2/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/TV/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/TV/dev_B80E51/
+-rw-rw-rw-   0        0        0     8479 2023-07-14 13:41:40.000000 antgen-0.3.5/antgen/appliances/TV/dev_B80E51/mode0
+-rw-rw-rw-   0        0        0     8429 2023-07-14 13:41:40.000000 antgen-0.3.5/antgen/appliances/TV/dev_B80E51/mode1
+-rw-rw-rw-   0        0        0     7571 2023-07-14 13:41:40.000000 antgen-0.3.5/antgen/appliances/TV/dev_B80E51/mode2
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/VACUUMCLEANER/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/VACUUMCLEANER/device_B7E2F8/
+-rw-rw-rw-   0        0        0      448 2023-07-14 13:41:40.000000 antgen-0.3.5/antgen/appliances/VACUUMCLEANER/device_B7E2F8/mode0
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/WASHINGMACHINE/
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/WASHINGMACHINE/ECO-H1/
+-rw-rw-rw-   0        0        0     4205 2023-07-14 13:41:40.000000 antgen-0.3.5/antgen/appliances/WASHINGMACHINE/ECO-H1/mode2
+-rw-rw-rw-   0        0        0     4050 2023-07-14 13:41:40.000000 antgen-0.3.5/antgen/appliances/WASHINGMACHINE/ECO-H1/mode3
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen/appliances/WASHINGMACHINE/_B82E27/
+-rw-rw-rw-   0        0        0     9448 2023-07-14 13:41:40.000000 antgen-0.3.5/antgen/appliances/WASHINGMACHINE/_B82E27/mode0
+-rw-rw-rw-   0        0        0      220 2023-07-14 13:41:32.000000 antgen-0.3.5/antgen/default.conf
+-rw-rw-rw-   0        0        0   144322 2023-07-14 13:41:32.000000 antgen-0.3.5/antgen/example1.png
+-rw-rw-rw-   0        0        0   122664 2023-07-14 13:41:32.000000 antgen-0.3.5/antgen/example2.png
+-rw-rw-rw-   0        0        0     2807 2023-07-14 13:41:33.000000 antgen-0.3.5/antgen/mapping.conf
+-rw-rw-rw-   0        0        0      104 2023-07-14 13:41:33.000000 antgen-0.3.5/antgen/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen.egg-info/
+-rw-rw-rw-   0        0        0      500 2023-07-14 16:50:04.000000 antgen-0.3.5/antgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4655 2023-07-14 16:50:05.000000 antgen-0.3.5/antgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 16:50:04.000000 antgen-0.3.5/antgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-14 16:50:04.000000 antgen-0.3.5/antgen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      679 2023-07-14 16:29:12.000000 antgen-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 16:50:05.000000 antgen-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      678 2023-07-14 16:48:14.000000 antgen-0.3.5/setup.py
```

### Comparing `antgen-0.3.4/README.md` & `antgen-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/ActivityModel.py` & `antgen-0.3.5/antgen/ActivityModel.py`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/ApplianceModel.py` & `antgen-0.3.5/antgen/ApplianceModel.py`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/LICENSE` & `antgen-0.3.5/antgen/LICENSE`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/LoadModelComponents.py` & `antgen-0.3.5/antgen/LoadModelComponents.py`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/Tools.py` & `antgen-0.3.5/antgen/Tools.py`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/UserModel.py` & `antgen-0.3.5/antgen/UserModel.py`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/activities/HOUSEHOLD/dry_clothes.conf` & `antgen-0.3.5/antgen/activities/HOUSEHOLD/dry_clothes.conf`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/activities/HOUSEHOLD/wash_laundry.conf` & `antgen-0.3.5/antgen/activities/HOUSEHOLD/wash_laundry.conf`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/activities/KITCHEN/preparing_breakfast.conf` & `antgen-0.3.5/antgen/activities/KITCHEN/preparing_breakfast.conf`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/activities/KITCHEN/preparing_dinner.conf` & `antgen-0.3.5/antgen/activities/KITCHEN/preparing_dinner.conf`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/antgen.py` & `antgen-0.3.5/antgen/antgen.py`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/AMPLIFIER/dev_AF6490/mode0` & `antgen-0.3.5/antgen/appliances/AMPLIFIER/dev_AF6490/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/CDPLAYER/dev_C3E6D1/mode0` & `antgen-0.3.5/antgen/appliances/CDPLAYER/dev_C3E6D1/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/COFFEEMAKER/ECO-H1/mode0` & `antgen-0.3.5/antgen/appliances/COFFEEMAKER/ECO-H1/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/COFFEEMAKER/ECO-H1/mode1` & `antgen-0.3.5/antgen/appliances/COFFEEMAKER/ECO-H1/mode1`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/COFFEEMAKER/dev_735E9D/mode0` & `antgen-0.3.5/antgen/appliances/COFFEEMAKER/dev_735E9D/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/COFFEEMAKER/dev_735E9D/mode1` & `antgen-0.3.5/antgen/appliances/COFFEEMAKER/dev_735E9D/mode1`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/COOKINGSTOVE/dev_D33097/mode0` & `antgen-0.3.5/antgen/appliances/COOKINGSTOVE/dev_D33097/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/DISHWASHER/dev_995BAC/mode0` & `antgen-0.3.5/antgen/appliances/DISHWASHER/dev_995BAC/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/DRYER/ECO-H1/mode0` & `antgen-0.3.5/antgen/appliances/DRYER/ECO-H1/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/DRYER/ECO-H1/mode1` & `antgen-0.3.5/antgen/appliances/DRYER/ECO-H1/mode1`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/DRYER/ECO-H1/mode2` & `antgen-0.3.5/antgen/appliances/DRYER/ECO-H1/mode2`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode0` & `antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode1` & `antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode1`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode2` & `antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode2`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode3` & `antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode3`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode4` & `antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode4`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode5` & `antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode5`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode6` & `antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode6`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode7` & `antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode7`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode8` & `antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode8`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/FREEZER/ECO-H1/mode9` & `antgen-0.3.5/antgen/appliances/FREEZER/ECO-H1/mode9`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/IRON/dev_D337C2/mode0` & `antgen-0.3.5/antgen/appliances/IRON/dev_D337C2/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/IRON/dev_D337C2/mode1` & `antgen-0.3.5/antgen/appliances/IRON/dev_D337C2/mode1`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/KETTLE/ECO-H1/mode1` & `antgen-0.3.5/antgen/appliances/KETTLE/ECO-H1/mode1`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/KETTLE/ECO-H1/mode2` & `antgen-0.3.5/antgen/appliances/KETTLE/ECO-H1/mode2`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/KETTLE/ECO-H1/mode3` & `antgen-0.3.5/antgen/appliances/KETTLE/ECO-H1/mode3`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/MICROWAVE/dev_98A0D3/mode1` & `antgen-0.3.5/antgen/appliances/MICROWAVE/dev_98A0D3/mode1`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/PC/Desktop_Denis/mode0` & `antgen-0.3.5/antgen/appliances/PC/Desktop_Denis/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/PC/ECO-H1/mode0` & `antgen-0.3.5/antgen/appliances/PC/ECO-H1/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/PC/ECO-H1/mode1` & `antgen-0.3.5/antgen/appliances/PC/ECO-H1/mode1`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/PRINTER/dev_11F01E/mode0` & `antgen-0.3.5/antgen/appliances/PRINTER/dev_11F01E/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/PRINTER/dev_11F01E/mode1` & `antgen-0.3.5/antgen/appliances/PRINTER/dev_11F01E/mode1`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/PRINTER/dev_11F01E/mode2` & `antgen-0.3.5/antgen/appliances/PRINTER/dev_11F01E/mode2`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode0` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode1` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode1`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode4` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode4`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode5` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode5`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode6` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode6`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode7` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode7`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/ECO-H1/mode8` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/ECO-H1/mode8`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev20111228/mode0` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev20111228/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev20111228/mode1` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev20111228/mode1`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode12` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode12`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode16` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode16`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode17` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode17`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode18` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode18`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode2` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode2`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/REFRIGERATOR/dev_76C07F/mode21` & `antgen-0.3.5/antgen/appliances/REFRIGERATOR/dev_76C07F/mode21`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/TOASTER/dev_98ABD2/mode0` & `antgen-0.3.5/antgen/appliances/TOASTER/dev_98ABD2/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/TV/dev_B80E51/mode0` & `antgen-0.3.5/antgen/appliances/TV/dev_B80E51/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/TV/dev_B80E51/mode1` & `antgen-0.3.5/antgen/appliances/TV/dev_B80E51/mode1`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/TV/dev_B80E51/mode2` & `antgen-0.3.5/antgen/appliances/TV/dev_B80E51/mode2`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/WASHINGMACHINE/ECO-H1/mode2` & `antgen-0.3.5/antgen/appliances/WASHINGMACHINE/ECO-H1/mode2`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/WASHINGMACHINE/ECO-H1/mode3` & `antgen-0.3.5/antgen/appliances/WASHINGMACHINE/ECO-H1/mode3`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/appliances/WASHINGMACHINE/_B82E27/mode0` & `antgen-0.3.5/antgen/appliances/WASHINGMACHINE/_B82E27/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/example1.png` & `antgen-0.3.5/antgen/example1.png`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/example2.png` & `antgen-0.3.5/antgen/example2.png`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen/mapping.conf` & `antgen-0.3.5/antgen/mapping.conf`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/antgen.egg-info/SOURCES.txt` & `antgen-0.3.5/antgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/pyproject.toml` & `antgen-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `antgen-0.3.4/setup.py` & `antgen-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='antgen',
-    version='0.3.4',
+    version='0.3.5',
     author='Nuno Velosa',
     author_email='nunovelosa@hotmail.com',
     description='This tool generates synthetic macroscopic load signatures for their use in conjunction with NILM (load disaggregation) tools.',
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

