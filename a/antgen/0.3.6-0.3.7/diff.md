# Comparing `tmp/antgen-0.3.6.tar.gz` & `tmp/antgen-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\antgen-0.3.6.tar", last modified: Fri Jul 14 16:55:54 2023, max compression
+gzip compressed data, was "dist\antgen-0.3.7.tar", last modified: Fri Jul 14 17:00:59 2023, max compression
```

## Comparing `antgen-0.3.6.tar` & `antgen-0.3.7.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/
--rw-rw-rw-   0        0        0      500 2023-07-14 16:55:54.000000 antgen-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0    18211 2023-07-14 13:41:32.000000 antgen-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/
--rw-rw-rw-   0        0        0    18871 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/ActivityModel.py
--rw-rw-rw-   0        0        0     5871 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/ApplianceModel.py
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/LICENSE
--rw-rw-rw-   0        0        0     7913 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/LoadModelComponents.py
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/Tools.py
--rw-rw-rw-   0        0        0     6013 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/UserModel.py
--rw-rw-rw-   0        0        0       76 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/activities/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/activities/HOUSEHOLD/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/activities/HOUSEHOLD/dry_clothes.conf
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/activities/HOUSEHOLD/ironing.conf
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/activities/HOUSEHOLD/vacuum.conf
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/activities/HOUSEHOLD/wash_laundry.conf
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/activities/KITCHEN/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/activities/KITCHEN/dishwasher.conf
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/activities/KITCHEN/fried_egg.conf
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/activities/KITCHEN/heating_lunch.conf
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/activities/KITCHEN/preparing_breakfast.conf
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/activities/KITCHEN/preparing_dinner.conf
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/activities/KITCHEN/refrigerator.conf
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/activities/LEISURE/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/activities/LEISURE/listen_music.conf
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/activities/LEISURE/use_pc.conf
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/activities/LEISURE/watch_tv.conf
--rw-rw-rw-   0        0        0    19213 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/antgen.py
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/AMPLIFIER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/AMPLIFIER/dev_AF6490/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/AMPLIFIER/dev_AF6490/mode0
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/BREADCUTTER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/BREADCUTTER/dev_B7DF9D/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/BREADCUTTER/dev_B7DF9D/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/BREADCUTTER/dev_B7DF9D/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/CDPLAYER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/CDPLAYER/dev_C3E6D1/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/CDPLAYER/dev_C3E6D1/mode0
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/COFFEEMAKER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/COFFEEMAKER/ECO-H1/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/COFFEEMAKER/ECO-H1/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/COFFEEMAKER/ECO-H1/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/COFFEEMAKER/dev_735E9D/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/COFFEEMAKER/dev_735E9D/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/COFFEEMAKER/dev_735E9D/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/COOKINGSTOVE/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/COOKINGSTOVE/dev_D33097/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/COOKINGSTOVE/dev_D33097/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/COOKINGSTOVE/dev_D33097/mode1
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/COOKINGSTOVE/dev_D33097/mode2
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/COOKINGSTOVE/dev_D33097/mode3
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/DISHWASHER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/DISHWASHER/dev_995BAC/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/DISHWASHER/dev_995BAC/mode0
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/DRYER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/DRYER/ECO-H1/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/DRYER/ECO-H1/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/DRYER/ECO-H1/mode1
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/DRYER/ECO-H1/mode2
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/FREEZER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/FREEZER/ECO-H1/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/FREEZER/ECO-H1/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/FREEZER/ECO-H1/mode1
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/FREEZER/ECO-H1/mode2
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/FREEZER/ECO-H1/mode3
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/FREEZER/ECO-H1/mode4
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/FREEZER/ECO-H1/mode5
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/FREEZER/ECO-H1/mode6
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/FREEZER/ECO-H1/mode7
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/FREEZER/ECO-H1/mode8
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/FREEZER/ECO-H1/mode9
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/IRON/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/IRON/dev_D337C2/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/IRON/dev_D337C2/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/IRON/dev_D337C2/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/KETTLE/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/KETTLE/ECO-H1/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/KETTLE/ECO-H1/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/KETTLE/ECO-H1/mode1
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/KETTLE/ECO-H1/mode2
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/KETTLE/ECO-H1/mode3
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/KETTLE/dev_5AE2CA/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/KETTLE/dev_5AE2CA/mode0
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/MICROWAVE/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/MICROWAVE/dev_98A0D3/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/MICROWAVE/dev_98A0D3/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/MICROWAVE/dev_98A0D3/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/PC/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/PC/Desktop_Denis/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/PC/Desktop_Denis/mode0
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/PC/ECO-H1/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/PC/ECO-H1/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/PC/ECO-H1/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/PRINTER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/PRINTER/dev_11F01E/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/PRINTER/dev_11F01E/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/PRINTER/dev_11F01E/mode1
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/PRINTER/dev_11F01E/mode2
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/ECO-H1/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/ECO-H1/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/ECO-H1/mode1
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/ECO-H1/mode4
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/ECO-H1/mode5
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/ECO-H1/mode6
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/ECO-H1/mode7
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/ECO-H1/mode8
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev20111228/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev20111228/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev20111228/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode1
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode10
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode11
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode12
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode13
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode14
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode15
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode16
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode17
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode18
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode19
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode2
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode20
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode21
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode22
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode23
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode3
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode4
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode5
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode6
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode7
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode8
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/REFRIGERATOR/dev_76C07F/mode9
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/TOASTER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/TOASTER/dev_98ABD2/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/TOASTER/dev_98ABD2/mode0
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/TOASTER/dev_98ABD2/mode1
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/TV/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/TV/dev_B80E51/
--rw-rw-rw-   0        0        0     8479 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/TV/dev_B80E51/mode0
--rw-rw-rw-   0        0        0     8429 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/TV/dev_B80E51/mode1
--rw-rw-rw-   0        0        0     7571 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/TV/dev_B80E51/mode2
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/VACUUMCLEANER/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/VACUUMCLEANER/device_B7E2F8/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/VACUUMCLEANER/device_B7E2F8/mode0
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/WASHINGMACHINE/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/WASHINGMACHINE/ECO-H1/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/WASHINGMACHINE/ECO-H1/mode2
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/appliances/WASHINGMACHINE/ECO-H1/mode3
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen/appliances/WASHINGMACHINE/_B82E27/
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/appliances/WASHINGMACHINE/_B82E27/mode0
--rw-rw-rw-   0        0        0      220 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/default.conf
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/example1.png
--rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/example2.png
--rw-rw-rw-   0        0        0     2807 2023-07-14 16:55:27.000000 antgen-0.3.6/antgen/mapping.conf
--rw-rw-rw-   0        0        0      104 2023-07-14 16:55:26.000000 antgen-0.3.6/antgen/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen.egg-info/
--rw-rw-rw-   0        0        0      500 2023-07-14 16:55:53.000000 antgen-0.3.6/antgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4655 2023-07-14 16:55:54.000000 antgen-0.3.6/antgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 16:55:53.000000 antgen-0.3.6/antgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-14 16:55:53.000000 antgen-0.3.6/antgen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      679 2023-07-14 16:53:24.000000 antgen-0.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 16:55:54.000000 antgen-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      678 2023-07-14 16:53:20.000000 antgen-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/
+-rw-rw-rw-   0        0        0      500 2023-07-14 17:00:59.000000 antgen-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0    18211 2023-07-14 13:41:32.000000 antgen-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/
+-rw-rw-rw-   0        0        0    18991 2023-07-14 16:58:18.000000 antgen-0.3.7/antgen/ActivityModel.py
+-rw-rw-rw-   0        0        0     5871 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/ApplianceModel.py
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/LICENSE
+-rw-rw-rw-   0        0        0     7913 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/LoadModelComponents.py
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/Tools.py
+-rw-rw-rw-   0        0        0     6013 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/UserModel.py
+-rw-rw-rw-   0        0        0       76 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/activities/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/activities/HOUSEHOLD/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/activities/HOUSEHOLD/dry_clothes.conf
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/activities/HOUSEHOLD/ironing.conf
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/activities/HOUSEHOLD/vacuum.conf
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/activities/HOUSEHOLD/wash_laundry.conf
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/activities/KITCHEN/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/activities/KITCHEN/dishwasher.conf
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/activities/KITCHEN/fried_egg.conf
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/activities/KITCHEN/heating_lunch.conf
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/activities/KITCHEN/preparing_breakfast.conf
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/activities/KITCHEN/preparing_dinner.conf
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/activities/KITCHEN/refrigerator.conf
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/activities/LEISURE/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/activities/LEISURE/listen_music.conf
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/activities/LEISURE/use_pc.conf
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/activities/LEISURE/watch_tv.conf
+-rw-rw-rw-   0        0        0    19213 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/antgen.py
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/AMPLIFIER/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/AMPLIFIER/dev_AF6490/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/AMPLIFIER/dev_AF6490/mode0
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/BREADCUTTER/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/BREADCUTTER/dev_B7DF9D/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/BREADCUTTER/dev_B7DF9D/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/BREADCUTTER/dev_B7DF9D/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/CDPLAYER/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/CDPLAYER/dev_C3E6D1/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/CDPLAYER/dev_C3E6D1/mode0
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/COFFEEMAKER/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/COFFEEMAKER/ECO-H1/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/COFFEEMAKER/ECO-H1/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/COFFEEMAKER/ECO-H1/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/COFFEEMAKER/dev_735E9D/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/COFFEEMAKER/dev_735E9D/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/COFFEEMAKER/dev_735E9D/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/COOKINGSTOVE/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/COOKINGSTOVE/dev_D33097/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/COOKINGSTOVE/dev_D33097/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/COOKINGSTOVE/dev_D33097/mode1
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/COOKINGSTOVE/dev_D33097/mode2
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/COOKINGSTOVE/dev_D33097/mode3
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/DISHWASHER/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/DISHWASHER/dev_995BAC/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/DISHWASHER/dev_995BAC/mode0
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/DRYER/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/DRYER/ECO-H1/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/DRYER/ECO-H1/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/DRYER/ECO-H1/mode1
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/DRYER/ECO-H1/mode2
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/FREEZER/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/FREEZER/ECO-H1/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/FREEZER/ECO-H1/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/FREEZER/ECO-H1/mode1
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/FREEZER/ECO-H1/mode2
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/FREEZER/ECO-H1/mode3
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/FREEZER/ECO-H1/mode4
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/FREEZER/ECO-H1/mode5
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/FREEZER/ECO-H1/mode6
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/FREEZER/ECO-H1/mode7
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/FREEZER/ECO-H1/mode8
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/FREEZER/ECO-H1/mode9
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/IRON/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/IRON/dev_D337C2/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/IRON/dev_D337C2/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/IRON/dev_D337C2/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/KETTLE/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/KETTLE/ECO-H1/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/KETTLE/ECO-H1/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/KETTLE/ECO-H1/mode1
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/KETTLE/ECO-H1/mode2
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/KETTLE/ECO-H1/mode3
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/KETTLE/dev_5AE2CA/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/KETTLE/dev_5AE2CA/mode0
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/MICROWAVE/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/MICROWAVE/dev_98A0D3/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/MICROWAVE/dev_98A0D3/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/MICROWAVE/dev_98A0D3/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/PC/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/PC/Desktop_Denis/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/PC/Desktop_Denis/mode0
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/PC/ECO-H1/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/PC/ECO-H1/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/PC/ECO-H1/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/PRINTER/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/PRINTER/dev_11F01E/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/PRINTER/dev_11F01E/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/PRINTER/dev_11F01E/mode1
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/PRINTER/dev_11F01E/mode2
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/ECO-H1/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/ECO-H1/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/ECO-H1/mode1
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/ECO-H1/mode4
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/ECO-H1/mode5
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/ECO-H1/mode6
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/ECO-H1/mode7
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/ECO-H1/mode8
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev20111228/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev20111228/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev20111228/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode1
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode10
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode11
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode12
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode13
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode14
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode15
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode16
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode17
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode18
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode19
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode2
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode20
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode21
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode22
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode23
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode3
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode4
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode5
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode6
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode7
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode8
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/REFRIGERATOR/dev_76C07F/mode9
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/TOASTER/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/TOASTER/dev_98ABD2/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/TOASTER/dev_98ABD2/mode0
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/TOASTER/dev_98ABD2/mode1
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/TV/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/TV/dev_B80E51/
+-rw-rw-rw-   0        0        0     8479 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/TV/dev_B80E51/mode0
+-rw-rw-rw-   0        0        0     8429 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/TV/dev_B80E51/mode1
+-rw-rw-rw-   0        0        0     7571 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/TV/dev_B80E51/mode2
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/VACUUMCLEANER/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/VACUUMCLEANER/device_B7E2F8/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/VACUUMCLEANER/device_B7E2F8/mode0
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen/appliances/WASHINGMACHINE/
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/WASHINGMACHINE/ECO-H1/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/WASHINGMACHINE/ECO-H1/mode2
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/appliances/WASHINGMACHINE/ECO-H1/mode3
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:59.000000 antgen-0.3.7/antgen/appliances/WASHINGMACHINE/_B82E27/
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/appliances/WASHINGMACHINE/_B82E27/mode0
+-rw-rw-rw-   0        0        0      220 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/default.conf
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/example1.png
+-rw-rw-rw-   0        0        0        0 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/example2.png
+-rw-rw-rw-   0        0        0     2807 2023-07-14 16:55:27.000000 antgen-0.3.7/antgen/mapping.conf
+-rw-rw-rw-   0        0        0      104 2023-07-14 16:55:26.000000 antgen-0.3.7/antgen/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen.egg-info/
+-rw-rw-rw-   0        0        0      500 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4655 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-14 17:00:58.000000 antgen-0.3.7/antgen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      679 2023-07-14 17:00:10.000000 antgen-0.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 17:00:59.000000 antgen-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      678 2023-07-14 16:59:54.000000 antgen-0.3.7/setup.py
```

### Comparing `antgen-0.3.6/README.md` & `antgen-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `antgen-0.3.6/antgen/ActivityModel.py` & `antgen-0.3.7/antgen/ActivityModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,17 @@
        figured out by calling *unique_appliances()* need a binding to an ApplianceModel to be synthesized."""
 
     def __init__(self, model_file):
         self.logger = logging.getLogger(__name__)
 
         # IMPORTANT
         #model_file = "/Users/nunovelosa/Desktop/antgen/" + model_file
-        model_file = "C:/Users/Nuno.Velosa/Desktop/antgen/" + model_file
+        #model_file = "C:/Users/Nuno.Velosa/Desktop/antgen/" + model_file
+        current_path = os.path.dirname(os.path.abspath(__file__))
+        model_file = current_path + "/" + model_file
         # IMPORTANT
 
         # Check if file actually exists
         if not os.path.isfile(model_file):
             raise ValueError("Configuration file {} not found. Terminating...".format(model_file))
 
         # Parse the file
```

### Comparing `antgen-0.3.6/antgen/ApplianceModel.py` & `antgen-0.3.7/antgen/ApplianceModel.py`

 * *Files identical despite different names*

### Comparing `antgen-0.3.6/antgen/LoadModelComponents.py` & `antgen-0.3.7/antgen/LoadModelComponents.py`

 * *Files identical despite different names*

### Comparing `antgen-0.3.6/antgen/UserModel.py` & `antgen-0.3.7/antgen/UserModel.py`

 * *Files identical despite different names*

### Comparing `antgen-0.3.6/antgen/antgen.py` & `antgen-0.3.7/antgen/antgen.py`

 * *Files identical despite different names*

### Comparing `antgen-0.3.6/antgen/appliances/TV/dev_B80E51/mode0` & `antgen-0.3.7/antgen/appliances/TV/dev_B80E51/mode0`

 * *Files identical despite different names*

### Comparing `antgen-0.3.6/antgen/appliances/TV/dev_B80E51/mode1` & `antgen-0.3.7/antgen/appliances/TV/dev_B80E51/mode1`

 * *Files identical despite different names*

### Comparing `antgen-0.3.6/antgen/appliances/TV/dev_B80E51/mode2` & `antgen-0.3.7/antgen/appliances/TV/dev_B80E51/mode2`

 * *Files identical despite different names*

### Comparing `antgen-0.3.6/antgen/mapping.conf` & `antgen-0.3.7/antgen/mapping.conf`

 * *Files identical despite different names*

### Comparing `antgen-0.3.6/antgen.egg-info/SOURCES.txt` & `antgen-0.3.7/antgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antgen-0.3.6/pyproject.toml` & `antgen-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "antgen"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
   { name="Nuno Velosa", email="nunovelosa@hotmail.com" },
 ]
 description = "This tool generates synthetic macroscopic load signatures for their use in conjunction with NILM (load disaggregation) tools."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `antgen-0.3.6/setup.py` & `antgen-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='antgen',
-    version='0.3.6',
+    version='0.3.7',
     author='Nuno Velosa',
     author_email='nunovelosa@hotmail.com',
     description='This tool generates synthetic macroscopic load signatures for their use in conjunction with NILM (load disaggregation) tools.',
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

