# Comparing `tmp/evennia-2.0.1.tar.gz` & `tmp/evennia-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evennia-2.0.1.tar", last modified: Sat Jun 17 07:20:24 2023, max compression
+gzip compressed data, was "evennia-2.1.0.tar", last modified: Fri Jul 14 13:16:43 2023, max compression
```

## Comparing `evennia-2.0.1.tar` & `evennia-2.1.0.tar`

### file list

```diff
@@ -1,966 +1,966 @@
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.694343 evennia-2.0.1/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1531 2023-06-10 17:39:32.000000 evennia-2.0.1/LICENSE.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5239 2023-06-17 07:20:24.694343 evennia-2.0.1/PKG-INFO
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3027 2023-06-10 17:39:32.000000 evennia-2.0.1/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.610344 evennia-2.0.1/bin/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/bin/unix/
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)      210 2023-06-10 17:39:32.000000 evennia-2.0.1/bin/unix/evennia
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        6 2023-06-17 07:13:51.000000 evennia-2.0.1/evennia/VERSION.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      438 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/VERSION_REQS.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13414 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1839 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/__main__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.618344 evennia-2.0.1/evennia/accounts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      214 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    67542 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26018 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/bots.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9574 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.618344 evennia-2.0.1/evennia/accounts/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7211 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/migrations/0002_move_defaults.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/migrations/0003_auto_20150209_2234.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2158 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/migrations/0004_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1010 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/migrations/0005_auto_20160905_0902.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1488 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/migrations/0006_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1927 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/migrations/0007_copy_player_to_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3944 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/migrations/0008_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      867 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/migrations/0009_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/migrations/0010_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4017 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      490 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/migrations/0012_defaultaccount_alter_accountdb_id_account_bot_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5740 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16280 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/accounts/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.618344 evennia-2.0.1/evennia/commands/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      304 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.618344 evennia-2.0.1/evennia/commands/_trial_temp/
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/_trial_temp/_trial_marker
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    31705 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/cmdhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8287 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/cmdparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27219 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/cmdset.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26150 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/cmdsethandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29198 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/command.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.618344 evennia-2.0.1/evennia/commands/default/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37414 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    19605 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/admin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    23003 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/batchprocess.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   167198 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/building.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2358 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/cmdset_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3032 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/cmdset_character.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      371 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/cmdset_session.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      872 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/cmdset_unloggedin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    76302 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22494 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/general.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    39551 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12788 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/muxcommand.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3152 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/syscommands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42195 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/system.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    81792 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17419 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/default/unloggedin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    46641 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/commands/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.622344 evennia-2.0.1/evennia/comms/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      207 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32556 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16863 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/managers.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.622344 evennia-2.0.1/evennia/comms/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3523 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      500 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0002_msg_db_hide_from_objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3784 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0003_auto_20140917_0756.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0004_auto_20150118_1631.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      641 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0005_auto_20150223_1517.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      615 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0007_msg_db_tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0008_auto_20160905_0902.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3872 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0009_auto_20160921_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0010_auto_20161206_1912.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1029 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0011_auto_20170217_2039.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4563 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0011_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      267 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0012_merge_20170617_2017.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4778 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0013_auto_20170705_1726.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0014_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      943 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0015_auto_20170706_2041.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      462 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0016_auto_20180925_1735.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7069 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0017_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      665 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0018_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1713 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0019_auto_20210514_2032.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      916 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0020_auto_20210514_2210.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3635 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0021_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22638 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3166 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/comms/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.622344 evennia-2.0.1/evennia/contrib/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      198 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.622344 evennia-2.0.1/evennia/contrib/base_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.622344 evennia-2.0.1/evennia/contrib/base_systems/awsstorage/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7695 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/awsstorage/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/awsstorage/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32480 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22503 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/awsstorage/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.622344 evennia-2.0.1/evennia/contrib/base_systems/building_menu/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    46012 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/building_menu/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      148 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/building_menu/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42659 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/building_menu/building_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6878 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/building_menu/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.622344 evennia-2.0.1/evennia/contrib/base_systems/color_markups/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2641 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/color_markups/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/color_markups/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8605 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/color_markups/color_markups.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/color_markups/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.622344 evennia-2.0.1/evennia/contrib/base_systems/components/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6397 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/components/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      952 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/components/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3915 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/components/component.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3762 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/components/dbfield.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11201 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/components/holder.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7237 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/components/signals.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14575 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/components/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.622344 evennia-2.0.1/evennia/contrib/base_systems/custom_gametime/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1549 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/custom_gametime/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      439 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/custom_gametime/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10390 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/custom_gametime/custom_gametime.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2017 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/custom_gametime/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.626344 evennia-2.0.1/evennia/contrib/base_systems/email_login/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1022 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/email_login/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      136 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/email_login/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1445 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/email_login/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10264 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/email_login/email_login.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1200 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/email_login/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.626344 evennia-2.0.1/evennia/contrib/base_systems/godotwebsocket/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8938 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/godotwebsocket/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      703 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/godotwebsocket/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3074 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27602 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2690 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/godotwebsocket/webclient.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.626344 evennia-2.0.1/evennia/contrib/base_systems/ingame_python/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    40300 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/ingame_python/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      128 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/ingame_python/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6777 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/ingame_python/callbackhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21872 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/ingame_python/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3048 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/ingame_python/eventfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    23990 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/ingame_python/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21618 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/ingame_python/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34963 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/ingame_python/typeclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8151 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/ingame_python/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.626344 evennia-2.0.1/evennia/contrib/base_systems/menu_login/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      787 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/menu_login/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/menu_login/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1206 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/menu_login/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8781 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/menu_login/menu_login.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      265 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/menu_login/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.626344 evennia-2.0.1/evennia/contrib/base_systems/mux_comms_cmds/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/mux_comms_cmds/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/mux_comms_cmds/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16012 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2298 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/mux_comms_cmds/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.626344 evennia-2.0.1/evennia/contrib/base_systems/unixcommand/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2241 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/unixcommand/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/unixcommand/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1654 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/unixcommand/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9989 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/base_systems/unixcommand/unixcommand.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.626344 evennia-2.0.1/evennia/contrib/full_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       75 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.626344 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5210 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22699 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10565 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34348 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7942 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/room.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      753 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9582 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/state.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.626344 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/states/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/states/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4168 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10461 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6112 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.626344 evennia-2.0.1/evennia/contrib/game_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      269 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.630344 evennia-2.0.1/evennia/contrib/game_systems/barter/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4322 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/barter/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/barter/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29726 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/barter/barter.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5976 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/barter/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.630344 evennia-2.0.1/evennia/contrib/game_systems/clothing/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4249 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/clothing/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      199 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/clothing/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24574 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/clothing/clothing.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4816 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/clothing/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.630344 evennia-2.0.1/evennia/contrib/game_systems/containers/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2508 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/containers/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       66 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/containers/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10015 2023-06-17 07:04:02.000000 evennia-2.0.1/evennia/contrib/game_systems/containers/containers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2734 2023-06-17 07:04:02.000000 evennia-2.0.1/evennia/contrib/game_systems/containers/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.630344 evennia-2.0.1/evennia/contrib/game_systems/cooldowns/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2084 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/cooldowns/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       88 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/cooldowns/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7580 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/cooldowns/cooldowns.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6135 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/cooldowns/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.630344 evennia-2.0.1/evennia/contrib/game_systems/crafting/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11186 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/crafting/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      233 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/crafting/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41597 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/crafting/crafting.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17892 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/crafting/example_recipes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24911 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/crafting/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.630344 evennia-2.0.1/evennia/contrib/game_systems/gendersub/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1986 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/gendersub/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      123 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/gendersub/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5096 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/gendersub/gendersub.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1091 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/gendersub/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.630344 evennia-2.0.1/evennia/contrib/game_systems/mail/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/mail/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      115 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/mail/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14841 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/mail/mail.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1852 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/mail/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.630344 evennia-2.0.1/evennia/contrib/game_systems/multidescer/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      932 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/multidescer/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/multidescer/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9951 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/multidescer/multidescer.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/multidescer/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.630344 evennia-2.0.1/evennia/contrib/game_systems/puzzles/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2181 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/puzzles/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/puzzles/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27837 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/puzzles/puzzles.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41328 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/puzzles/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.630344 evennia-2.0.1/evennia/contrib/game_systems/turnbattle/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2940 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/turnbattle/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/turnbattle/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28762 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/turnbattle/tb_basic.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    23139 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/turnbattle/tb_equip.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37446 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/turnbattle/tb_items.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30705 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/turnbattle/tb_magic.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    38339 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/turnbattle/tb_range.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29682 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/game_systems/turnbattle/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.630344 evennia-2.0.1/evennia/contrib/grid/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.630344 evennia-2.0.1/evennia/contrib/grid/extended_room/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6348 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/extended_room/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      454 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/extended_room/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34157 2023-06-17 07:04:02.000000 evennia-2.0.1/evennia/contrib/grid/extended_room/extended_room.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12997 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/extended_room/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.634343 evennia-2.0.1/evennia/contrib/grid/ingame_map_display/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1358 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/ingame_map_display/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       92 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/ingame_map_display/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10572 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/ingame_map_display/ingame_map_display.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/ingame_map_display/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.634343 evennia-2.0.1/evennia/contrib/grid/mapbuilder/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9672 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/mapbuilder/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/mapbuilder/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17398 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/mapbuilder/mapbuilder.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6435 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/mapbuilder/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.634343 evennia-2.0.1/evennia/contrib/grid/simpledoor/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1356 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/simpledoor/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/simpledoor/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5838 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/simpledoor/simpledoor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/simpledoor/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.634343 evennia-2.0.1/evennia/contrib/grid/slow_exit/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1730 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/slow_exit/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      203 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/slow_exit/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5046 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/slow_exit/slow_exit.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      824 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/slow_exit/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.634343 evennia-2.0.1/evennia/contrib/grid/wilderness/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4932 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/wilderness/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      394 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/wilderness/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6026 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/wilderness/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28916 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/wilderness/wilderness.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.634343 evennia-2.0.1/evennia/contrib/grid/xyzgrid/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    54690 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/xyzgrid/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      202 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/xyzgrid/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20837 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/xyzgrid/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7822 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/xyzgrid/example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13723 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/xyzgrid/launchcmd.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1145 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/xyzgrid/prototypes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42072 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/xyzgrid/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1043 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/xyzgrid/utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    40413 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/xyzgrid/xymap.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    52070 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/xyzgrid/xymap_legend.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10484 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/xyzgrid/xyzgrid.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24616 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/grid/xyzgrid/xyzroom.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.634343 evennia-2.0.1/evennia/contrib/rpg/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      406 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.634343 evennia-2.0.1/evennia/contrib/rpg/buffs/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22364 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/buffs/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/buffs/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    45607 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/buffs/buff.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3893 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/buffs/samplebuffs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16470 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/buffs/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.634343 evennia-2.0.1/evennia/contrib/rpg/character_creator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3924 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/character_creator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      176 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/character_creator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8148 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/character_creator/character_creator.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21006 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/character_creator/example_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1552 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/character_creator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.634343 evennia-2.0.1/evennia/contrib/rpg/dice/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/dice/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      177 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/dice/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10272 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/dice/dice.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      901 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/dice/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.638343 evennia-2.0.1/evennia/contrib/rpg/health_bar/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1264 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/health_bar/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/health_bar/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4913 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/health_bar/health_bar.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1634 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/health_bar/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.638343 evennia-2.0.1/evennia/contrib/rpg/rpsystem/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9938 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/rpsystem/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      793 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/rpsystem/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24722 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/rpsystem/rplanguage.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    65825 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/rpsystem/rpsystem.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14981 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/rpsystem/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.638343 evennia-2.0.1/evennia/contrib/rpg/traits/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14246 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/traits/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      294 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/traits/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37184 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/traits/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    54252 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/rpg/traits/traits.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.638343 evennia-2.0.1/evennia/contrib/tutorials/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      151 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.638343 evennia-2.0.1/evennia/contrib/tutorials/batchprocessor/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1623 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/batchprocessor/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       50 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/batchprocessor/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3618 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/batchprocessor/example_batch_code.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.638343 evennia-2.0.1/evennia/contrib/tutorials/bodyfunctions/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      471 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/bodyfunctions/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/bodyfunctions/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2311 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3324 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/bodyfunctions/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.638343 evennia-2.0.1/evennia/contrib/tutorials/evadventure/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1180 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      164 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.638343 evennia-2.0.1/evennia/contrib/tutorials/evadventure/batchscripts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       73 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/batchscripts/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1820 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1436 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3996 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/build_techdemo.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/build_world.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12610 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11199 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/chargen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17122 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/combat_base.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28417 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/combat_turnbased.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18301 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/combat_twitch.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12500 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17918 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/dungeon.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1742 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/enums.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14608 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/equipment.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12264 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/npcs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11174 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8743 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/quests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11708 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/random_tables.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3154 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12169 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/rules.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17153 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/shops.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.642343 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1389 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/mixins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1266 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2151 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_chargen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28061 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_combat.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3741 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7811 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_equipment.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      542 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_npcs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4629 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_quests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2237 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8083 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_rules.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      712 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1485 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/evadventure/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.642343 evennia-2.0.1/evennia/contrib/tutorials/mirror/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      429 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/mirror/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/mirror/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2235 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/mirror/mirror.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.642343 evennia-2.0.1/evennia/contrib/tutorials/red_button/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1344 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/red_button/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/red_button/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18609 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/red_button/red_button.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.642343 evennia-2.0.1/evennia/contrib/tutorials/talking_npc/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/talking_npc/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/talking_npc/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3697 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/talking_npc/talking_npc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      449 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/talking_npc/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.642343 evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4302 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      125 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    50297 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/build.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25293 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/intro_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16130 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/mob.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42155 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42922 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7342 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.642343 evennia-2.0.1/evennia/contrib/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       67 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.642343 evennia-2.0.1/evennia/contrib/utils/auditing/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3303 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/auditing/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/auditing/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2065 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/auditing/outputs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8515 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/auditing/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6047 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/auditing/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.642343 evennia-2.0.1/evennia/contrib/utils/fieldfill/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5816 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/fieldfill/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      288 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/fieldfill/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26382 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/fieldfill/fieldfill.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.642343 evennia-2.0.1/evennia/contrib/utils/git_integration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3139 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/git_integration/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       86 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/git_integration/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7737 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/git_integration/git_integration.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2828 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/git_integration/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.646343 evennia-2.0.1/evennia/contrib/utils/name_generator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9815 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/name_generator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/name_generator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   232619 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/name_generator/btn_givennames.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    56503 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/name_generator/btn_surnames.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14447 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/name_generator/namegen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4914 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/name_generator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.646343 evennia-2.0.1/evennia/contrib/utils/random_string_generator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2165 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/random_string_generator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      268 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/random_string_generator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12595 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/random_string_generator/random_string_generator.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      737 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/random_string_generator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.646343 evennia-2.0.1/evennia/contrib/utils/tree_select/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5935 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/tree_select/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      109 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/tree_select/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2199 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/tree_select/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20930 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/contrib/utils/tree_select/tree_select.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.646343 evennia-2.0.1/evennia/game_template/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1521 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.646343 evennia-2.0.1/evennia/game_template/commands/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      676 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/commands/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/commands/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7738 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/commands/command.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2636 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/commands/default_cmdsets.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      551 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/gitignore
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.646343 evennia-2.0.1/evennia/game_template/server/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1718 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/server/conf/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      629 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/at_initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2154 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/at_search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/at_server_startstop.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2174 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/cmdparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1159 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/inlinefuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1419 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/inputfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1065 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/lockfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4009 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/mssp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      709 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/portal_services_plugins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      714 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/secret_settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      705 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/server_services_plugins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1347 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/serversession.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/conf/web_plugins.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/server/logs/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      839 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/server/logs/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/typeclasses/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      733 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/typeclasses/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/typeclasses/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3774 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/typeclasses/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2920 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/typeclasses/channels.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1525 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/typeclasses/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2044 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/typeclasses/exits.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8847 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/typeclasses/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      551 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/typeclasses/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4394 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/typeclasses/scripts.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/web/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2939 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/web/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      296 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/admin/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/admin/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      520 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/admin/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/web/api/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/api/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/web/static/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      849 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/static/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.610344 evennia-2.0.1/evennia/game_template/web/static/rest_framework/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/web/static/rest_framework/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       53 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/static/rest_framework/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/web/static/rest_framework/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       47 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/static/rest_framework/images/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.610344 evennia-2.0.1/evennia/game_template/web/static/webclient/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/web/static/webclient/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      132 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/static/webclient/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/web/static/webclient/js/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/static/webclient/js/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.610344 evennia-2.0.1/evennia/game_template/web/static/website/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/web/static/website/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/static/website/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/web/static/website/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      135 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/static/website/images/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.650343 evennia-2.0.1/evennia/game_template/web/templates/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      760 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/templates/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.654343 evennia-2.0.1/evennia/game_template/web/templates/rest_framework/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       58 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/templates/rest_framework/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.654343 evennia-2.0.1/evennia/game_template/web/templates/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      223 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/templates/webclient/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.654343 evennia-2.0.1/evennia/game_template/web/templates/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/templates/website/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.654343 evennia-2.0.1/evennia/game_template/web/templates/website/flatpages/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/templates/website/flatpages/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.654343 evennia-2.0.1/evennia/game_template/web/templates/website/registration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      152 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/templates/website/registration/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1099 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.654343 evennia-2.0.1/evennia/game_template/web/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1102 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/webclient/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/webclient/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      539 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/webclient/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.654343 evennia-2.0.1/evennia/game_template/web/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1262 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/website/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/website/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      509 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/website/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.654343 evennia-2.0.1/evennia/game_template/web/website/views/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/web/website/views/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.654343 evennia-2.0.1/evennia/game_template/world/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/world/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/world/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      999 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/world/batch_cmds.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2186 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/world/help_entries.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3646 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/game_template/world/prototypes.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.654343 evennia-2.0.1/evennia/help/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/help/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8013 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/help/filehelp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6229 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/help/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.658343 evennia-2.0.1/evennia/help/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2222 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/help/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      577 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/help/migrations/0002_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1688 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/help/migrations/0003_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/help/migrations/0004_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1166 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/help/migrations/0005_auto_20210530_1818.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      473 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/help/migrations/0006_alter_helpentry_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/help/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9729 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/help/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3736 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/help/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7673 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/help/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.658343 evennia-2.0.1/evennia/locale/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2686 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/README
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/locale/de/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.658343 evennia-2.0.1/evennia/locale/de/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10764 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14475 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/locale/es/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.658343 evennia-2.0.1/evennia/locale/es/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3821 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30981 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/locale/fr/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.658343 evennia-2.0.1/evennia/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26255 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    38581 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/locale/it/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.658343 evennia-2.0.1/evennia/locale/it/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6944 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    35844 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/locale/ko/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.658343 evennia-2.0.1/evennia/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3569 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/ko/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30924 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/ko/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/locale/la/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.662343 evennia-2.0.1/evennia/locale/la/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6537 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/la/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32786 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/la/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/locale/pl/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.662343 evennia-2.0.1/evennia/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28236 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/locale/pt/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.662343 evennia-2.0.1/evennia/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25584 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42122 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/locale/ru/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.662343 evennia-2.0.1/evennia/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2281 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29419 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/locale/sv/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.662343 evennia-2.0.1/evennia/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29036 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    43353 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/locale/zh/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.662343 evennia-2.0.1/evennia/locale/zh/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3300 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/zh/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30540 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locale/zh/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.666343 evennia-2.0.1/evennia/locks/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      240 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locks/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22093 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locks/lockfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26966 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locks/lockhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13732 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/locks/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.666343 evennia-2.0.1/evennia/objects/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      120 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29704 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.670343 evennia-2.0.1/evennia/objects/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4315 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1193 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/0002_auto_20140917_0756.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      810 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      530 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/0004_auto_20150118_1622.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      410 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/0005_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1599 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/0006_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/0007_objectdb_db_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/0008_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/0009_remove_objectdb_db_player.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5028 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/0010_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1351 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/0011_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4011 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      488 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/0013_defaultobject_alter_objectdb_id_defaultcharacter_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13399 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   118892 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17072 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/objects/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.670343 evennia-2.0.1/evennia/prototypes/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6567 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/prototypes/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/prototypes/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    92110 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/prototypes/menus.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2912 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/prototypes/protfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    46537 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/prototypes/prototypes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42860 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/prototypes/spawner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    39636 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/prototypes/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.670343 evennia-2.0.1/evennia/scripts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      229 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11275 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.670343 evennia-2.0.1/evennia/scripts/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4762 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      675 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0002_auto_20150118_1625.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1507 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      861 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0004_auto_20150306_1354.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      430 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0005_auto_20150306_1441.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      710 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0006_auto_20150310_2249.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      396 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0007_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      913 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0008_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1271 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0009_scriptdb_db_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0010_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4655 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0012_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      666 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0013_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      752 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0014_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3329 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0015_convert_contrib_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/0016_scriptbase_alter_scriptdb_id_defaultscript_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6311 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8746 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/monitorhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5326 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/scripthandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27441 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20801 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/taskhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10678 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24661 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/scripts/tickerhandler.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.674343 evennia-2.0.1/evennia/server/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      234 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8697 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/amp_client.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16629 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/connection_wizard.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7955 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/deprecations.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    79833 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/evennia_launcher.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.674343 evennia-2.0.1/evennia/server/game_index_client/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4321 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/game_index_client/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       45 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/game_index_client/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6256 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/game_index_client/client.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1990 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/game_index_client/service.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7622 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    19709 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/inputfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1708 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.674343 evennia-2.0.1/evennia/server/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      812 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1363 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/migrations/0002_auto_20190128_2311.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/migrations/0003_alter_serverconfig_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3818 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/models.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.674343 evennia-2.0.1/evennia/server/portal/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17922 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/amp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17520 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/amp_server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18478 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/discord.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11345 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/grapevine.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14242 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/irc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2571 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/mccp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3882 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/mssp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2341 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/mxp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2359 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/naws.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16018 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/portal.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17163 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/portalsessionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4450 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/rss.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15920 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/ssh.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3319 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/ssl.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1785 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/suppress_ga.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17379 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/telnet.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15609 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/telnet_oob.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4861 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/telnet_ssl.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14725 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7073 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/ttype.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11403 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/webclient.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15897 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/portal/webclient_ajax.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.678343 evennia-2.0.1/evennia/server/profiling/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      212 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/profiling/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/profiling/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20881 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/profiling/dummyrunner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9427 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/profiling/dummyrunner_settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3924 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/profiling/memplot.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1375 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/profiling/settings_mixin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1095 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/profiling/test_queries.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5371 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/profiling/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1345 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/profiling/timetrace.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28633 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14599 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/serversession.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5616 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/session.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30009 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/sessionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4935 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/signals.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.678343 evennia-2.0.1/evennia/server/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/tests/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4721 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/tests/test_amp_connection.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      521 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/tests/test_initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7305 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/tests/test_launcher.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4444 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/tests/test_misc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9256 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/tests/test_server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/tests/testrunner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7101 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/throttle.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2763 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/validators.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8653 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/server/webserver.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    60833 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/settings_default.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.678343 evennia-2.0.1/evennia/typeclasses/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    64398 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    31304 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/managers.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.678343 evennia-2.0.1/evennia/typeclasses/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6101 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      768 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0002_auto_20150109_0913.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2266 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      833 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0004_auto_20151101_1759.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      922 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0005_auto_20160625_1812.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1444 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3899 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1699 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4230 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1993 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0010_delete_old_player_tables.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5265 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0011_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      821 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0013_auto_20191015_1922.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0014_alter_tag_db_category.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      362 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0015_alter_attribute_options.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37156 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30224 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17813 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/typeclasses/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.682343 evennia-2.0.1/evennia/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      320 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    51381 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/ansi.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15392 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/batchprocessors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8077 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/containers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10242 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/create.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32812 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/dbserialize.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41419 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/eveditor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2734 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/evennia-mode.el
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21081 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/evform.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    78957 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/evmenu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18330 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/evmore.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    65173 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/evtable.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    53272 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/funcparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8754 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/gametime.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.682343 evennia-2.0.1/evennia/utils/idmapper/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1309 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/idmapper/LICENSE.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1097 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/idmapper/README_evennia.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1992 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/idmapper/README_orig.rst
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       64 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/idmapper/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1181 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/idmapper/manager.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24820 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/idmapper/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2876 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/idmapper/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18789 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/logger.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10265 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/optionclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6455 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/optionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11093 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/picklefield.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14179 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25088 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/test_resources.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.682343 evennia-2.0.1/evennia/utils/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.682343 evennia-2.0.1/evennia/utils/tests/data/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/data/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      274 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/data/broken_script.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1125 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/data/evform_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6245 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/data/evmenu_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      382 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/data/prototypes_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1608 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_ansi.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7052 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_batchprocessors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3463 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_containers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7032 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_create_functions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7888 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_dbserialize.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11752 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_eveditor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12172 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_evform.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11763 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_evmenu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12101 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_evtable.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30844 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_funcparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3942 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_gametime.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4460 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13564 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_tagparsing.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5509 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_text2html.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29937 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6371 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/tests/test_validatorfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12235 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/text2html.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    97272 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9489 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/validatorfuncs.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.682343 evennia-2.0.1/evennia/utils/verb_conjugation/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18011 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/verb_conjugation/LICENSE.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/verb_conjugation/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9885 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/verb_conjugation/conjugate.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11298 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/verb_conjugation/pronouns.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10493 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/verb_conjugation/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   554408 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/utils/verb_conjugation/verbs.txt
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.686343 evennia-2.0.1/evennia/web/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1150 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      127 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.686343 evennia-2.0.1/evennia/web/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      428 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/admin/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14125 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/admin/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8627 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/admin/attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8508 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/admin/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/admin/frontpage.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1889 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/admin/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11915 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/admin/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4499 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/admin/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      508 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/admin/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8955 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/admin/tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      878 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/admin/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2884 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/admin/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.686343 evennia-2.0.1/evennia/web/api/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7674 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/api/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/api/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4268 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/api/filters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3949 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/api/permissions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      277 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/api/root.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9905 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/api/serializers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8148 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/api/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2293 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/api/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5828 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/api/views.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/web/static/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/web/static/rest_framework/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.686343 evennia-2.0.1/evennia/web/static/rest_framework/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      298 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/rest_framework/css/api.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.686343 evennia-2.0.1/evennia/web/static/rest_framework/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/rest_framework/images/favicon.ico
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/web/static/webclient/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.686343 evennia-2.0.1/evennia/web/static/webclient/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2104 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/css/goldenlayout.css
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27268 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/css/webclient.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.686343 evennia-2.0.1/evennia/web/static/webclient/fonts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22208 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/fonts/DejaVuSansMono.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.686343 evennia-2.0.1/evennia/web/static/webclient/js/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18546 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/evennia.js
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.690343 evennia-2.0.1/evennia/web/static/webclient/js/plugins/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      563 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/clienthelp.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3914 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/default_in.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1958 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/default_out.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      345 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/default_unload.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3785 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/font.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29030 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/goldenlayout.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2114 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2981 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/history.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5031 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/hotbuttons.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1969 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/html.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1912 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/iframe.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4666 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/message_routing.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/multimedia.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2842 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/notifications.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      909 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/oob.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6262 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/options2.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2790 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/popups.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10949 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/plugins/text2html.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9705 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/js/webclient_gui.js
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.690343 evennia-2.0.1/evennia/web/static/webclient/media/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3624 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/webclient/media/notification.wav
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/web/static/website/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.690343 evennia-2.0.1/evennia/web/static/website/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/website/css/custom.css
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2013 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/website/css/website.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.690343 evennia-2.0.1/evennia/web/static/website/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/website/images/LICENCE
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)    17938 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/website/images/evennia_logo.png
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21167 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/website/images/evennia_logo_festive.png
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/static/website/images/favicon.ico
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.614344 evennia-2.0.1/evennia/web/templates/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.690343 evennia-2.0.1/evennia/web/templates/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1621 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/admin/app_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6462 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/admin/frontpage.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.690343 evennia-2.0.1/evennia/web/templates/rest_framework/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      903 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/rest_framework/api.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      417 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/rest_framework/redoc.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.690343 evennia-2.0.1/evennia/web/templates/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7691 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/webclient/base.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1058 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/webclient/webclient.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.690343 evennia-2.0.1/evennia/web/templates/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      510 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/404.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      614 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/500.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4078 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/_menu.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3132 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/base.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2858 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/channel_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2667 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/channel_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1402 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/character_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/character_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1139 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/character_manage_list.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.690343 evennia-2.0.1/evennia/web/templates/website/flatpages/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      341 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/flatpages/default.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1501 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/generic_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2715 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/help_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5052 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/help_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5367 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/index.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      180 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/messages.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      900 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/object_confirm_delete.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1034 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/object_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/object_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1484 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/pagination.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.694343 evennia-2.0.1/evennia/web/templates/website/registration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/registration/logged_out.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1957 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/registration/login.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/registration/password_change_done.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1422 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/registration/password_change_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      813 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/registration/password_reset_complete.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1747 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/registration/password_reset_confirm.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/registration/password_reset_done.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      566 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/registration/password_reset_email.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1577 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/registration/password_reset_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/registration/register.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      671 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templates/website/tbi.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.694343 evennia-2.0.1/evennia/web/templatetags/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      287 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templatetags/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templatetags/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/templatetags/addclass.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.694343 evennia-2.0.1/evennia/web/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/utils/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1256 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/utils/adminsite.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/utils/apache_wsgi.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1815 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/utils/backends.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2035 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/utils/evennia_modpy_apache.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/utils/evennia_wsgi_apache.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4137 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/utils/general_context.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2712 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/utils/middleware.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2443 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/utils/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.694343 evennia-2.0.1/evennia/web/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/webclient/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/webclient/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      795 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/webclient/views.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.694343 evennia-2.0.1/evennia/web/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       31 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/website/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5736 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/website/forms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12503 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/website/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2575 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/website/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.694343 evennia-2.0.1/evennia/web/website/views/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/website/views/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2120 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/website/views/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5329 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/website/views/channels.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8330 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/website/views/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      311 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/website/views/errors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11796 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/website/views/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/website/views/index.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2353 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/website/views/mixins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9037 2023-06-10 17:39:32.000000 evennia-2.0.1/evennia/web/website/views/objects.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-17 07:20:24.618344 evennia-2.0.1/evennia.egg-info/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5239 2023-06-17 07:20:23.000000 evennia-2.0.1/evennia.egg-info/PKG-INFO
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34996 2023-06-17 07:20:24.000000 evennia-2.0.1/evennia.egg-info/SOURCES.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        1 2023-06-17 07:20:23.000000 evennia-2.0.1/evennia.egg-info/dependency_links.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2023-06-17 07:20:23.000000 evennia-2.0.1/evennia.egg-info/requires.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        8 2023-06-17 07:20:23.000000 evennia-2.0.1/evennia.egg-info/top_level.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3961 2023-06-17 07:13:42.000000 evennia-2.0.1/pyproject.toml
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       38 2023-06-17 07:20:24.694343 evennia-2.0.1/setup.cfg
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1388 2023-06-10 17:39:32.000000 evennia-2.0.1/setup.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.413076 evennia-2.1.0/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1531 2023-06-10 17:39:32.000000 evennia-2.1.0/LICENSE.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5239 2023-07-14 13:16:43.413076 evennia-2.1.0/PKG-INFO
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3027 2023-06-10 17:39:32.000000 evennia-2.1.0/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.377077 evennia-2.1.0/bin/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/bin/unix/
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)      210 2023-06-10 17:39:32.000000 evennia-2.1.0/bin/unix/evennia
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        6 2023-07-14 13:12:33.000000 evennia-2.1.0/evennia/VERSION.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      438 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/VERSION_REQS.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13414 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1839 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/__main__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/accounts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      214 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    67542 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26018 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/bots.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9574 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/accounts/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7211 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/migrations/0002_move_defaults.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/migrations/0003_auto_20150209_2234.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2158 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/migrations/0004_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1010 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/migrations/0005_auto_20160905_0902.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1488 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/migrations/0006_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1927 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/migrations/0007_copy_player_to_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3944 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/migrations/0008_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      867 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/migrations/0009_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/migrations/0010_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4017 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      490 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/migrations/0012_defaultaccount_alter_accountdb_id_account_bot_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5740 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16280 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/accounts/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/commands/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      304 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/commands/_trial_temp/
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/_trial_temp/_trial_marker
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    31705 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/cmdhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8287 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/cmdparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27219 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/cmdset.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26150 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/cmdsethandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29198 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/command.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.385077 evennia-2.1.0/evennia/commands/default/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37414 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    19605 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/admin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    23003 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/batchprocess.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   167198 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/building.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2358 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/cmdset_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3032 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/cmdset_character.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      371 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/cmdset_session.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      872 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/cmdset_unloggedin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    76302 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22494 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/general.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    39551 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12788 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/muxcommand.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3152 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/syscommands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42195 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/system.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    81792 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17419 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/default/unloggedin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    46641 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/commands/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.385077 evennia-2.1.0/evennia/comms/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      207 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32556 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16863 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/managers.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.385077 evennia-2.1.0/evennia/comms/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3523 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      500 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0002_msg_db_hide_from_objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3784 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0003_auto_20140917_0756.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0004_auto_20150118_1631.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      641 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0005_auto_20150223_1517.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      615 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0007_msg_db_tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0008_auto_20160905_0902.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3872 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0009_auto_20160921_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0010_auto_20161206_1912.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1029 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0011_auto_20170217_2039.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4563 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0011_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      267 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0012_merge_20170617_2017.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4778 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0013_auto_20170705_1726.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0014_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      943 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0015_auto_20170706_2041.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      462 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0016_auto_20180925_1735.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7069 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0017_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      665 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0018_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1713 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0019_auto_20210514_2032.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      916 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0020_auto_20210514_2210.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3635 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0021_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22638 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3166 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/comms/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.385077 evennia-2.1.0/evennia/contrib/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      198 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.385077 evennia-2.1.0/evennia/contrib/base_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.385077 evennia-2.1.0/evennia/contrib/base_systems/awsstorage/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7695 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/awsstorage/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/awsstorage/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32480 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22503 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/awsstorage/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.385077 evennia-2.1.0/evennia/contrib/base_systems/building_menu/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    46012 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/building_menu/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      148 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/building_menu/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42659 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/building_menu/building_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6878 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/building_menu/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.385077 evennia-2.1.0/evennia/contrib/base_systems/color_markups/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2641 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/color_markups/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/color_markups/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8605 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/color_markups/color_markups.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/color_markups/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.385077 evennia-2.1.0/evennia/contrib/base_systems/components/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6397 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/components/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      952 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/components/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3915 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/components/component.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3762 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/components/dbfield.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11201 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/components/holder.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7237 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/components/signals.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14575 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/components/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.385077 evennia-2.1.0/evennia/contrib/base_systems/custom_gametime/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1549 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/custom_gametime/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      439 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/custom_gametime/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10390 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2017 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/custom_gametime/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.385077 evennia-2.1.0/evennia/contrib/base_systems/email_login/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1022 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/email_login/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      136 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/email_login/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1445 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/email_login/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10264 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/email_login/email_login.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1200 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/email_login/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.385077 evennia-2.1.0/evennia/contrib/base_systems/godotwebsocket/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8938 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/godotwebsocket/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      703 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/godotwebsocket/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3074 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27602 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2690 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/godotwebsocket/webclient.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.385077 evennia-2.1.0/evennia/contrib/base_systems/ingame_python/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    40300 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/ingame_python/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      128 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/ingame_python/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6777 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21872 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/ingame_python/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3048 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    23990 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/ingame_python/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21618 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/ingame_python/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34963 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/ingame_python/typeclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8151 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/ingame_python/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/base_systems/menu_login/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      787 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/menu_login/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/menu_login/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1206 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/menu_login/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8781 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/menu_login/menu_login.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      265 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/menu_login/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/base_systems/mux_comms_cmds/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/mux_comms_cmds/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/mux_comms_cmds/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16012 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2298 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/base_systems/unixcommand/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2241 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/unixcommand/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/unixcommand/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1654 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/unixcommand/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9989 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/base_systems/unixcommand/unixcommand.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/full_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       75 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5210 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22699 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10565 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34348 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7942 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/room.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      753 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9582 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/state.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/states/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/states/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4168 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10461 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6112 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/game_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      269 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/game_systems/barter/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4322 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/barter/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/barter/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29726 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/barter/barter.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5976 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/barter/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/game_systems/clothing/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4256 2023-06-26 18:18:53.000000 evennia-2.1.0/evennia/contrib/game_systems/clothing/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      199 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/clothing/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24575 2023-06-26 18:18:53.000000 evennia-2.1.0/evennia/contrib/game_systems/clothing/clothing.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4816 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/clothing/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/game_systems/containers/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2508 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/containers/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       66 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/containers/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10015 2023-06-17 07:04:02.000000 evennia-2.1.0/evennia/contrib/game_systems/containers/containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2734 2023-06-17 07:04:02.000000 evennia-2.1.0/evennia/contrib/game_systems/containers/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/game_systems/cooldowns/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2084 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/cooldowns/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       88 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/cooldowns/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7580 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/cooldowns/cooldowns.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6135 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/cooldowns/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/game_systems/crafting/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11186 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/crafting/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      233 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/crafting/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41597 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/crafting/crafting.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17892 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/crafting/example_recipes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24911 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/crafting/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/game_systems/gendersub/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1986 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/gendersub/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      123 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/gendersub/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5096 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/gendersub/gendersub.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1091 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/gendersub/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/game_systems/mail/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/mail/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      115 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/mail/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14841 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/mail/mail.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1852 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/mail/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/game_systems/multidescer/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      932 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/multidescer/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/multidescer/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9951 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/multidescer/multidescer.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/multidescer/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/game_systems/puzzles/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2181 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/puzzles/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/puzzles/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27837 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/puzzles/puzzles.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41328 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/puzzles/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/game_systems/turnbattle/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2940 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/turnbattle/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/turnbattle/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28762 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/turnbattle/tb_basic.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    23139 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/turnbattle/tb_equip.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37446 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/turnbattle/tb_items.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30705 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/turnbattle/tb_magic.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    38339 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/turnbattle/tb_range.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29682 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/game_systems/turnbattle/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/grid/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/grid/extended_room/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6348 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/extended_room/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      454 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/extended_room/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34300 2023-07-14 12:56:38.000000 evennia-2.1.0/evennia/contrib/grid/extended_room/extended_room.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12997 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/extended_room/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/grid/ingame_map_display/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1358 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/ingame_map_display/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       92 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/ingame_map_display/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10572 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/ingame_map_display/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/grid/mapbuilder/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9672 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/mapbuilder/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/mapbuilder/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17398 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/mapbuilder/mapbuilder.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6435 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/mapbuilder/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/grid/simpledoor/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1356 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/simpledoor/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/simpledoor/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5838 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/simpledoor/simpledoor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/simpledoor/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/grid/slow_exit/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1730 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/slow_exit/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      203 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/slow_exit/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5046 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/slow_exit/slow_exit.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      824 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/slow_exit/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.389077 evennia-2.1.0/evennia/contrib/grid/wilderness/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4932 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/wilderness/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      394 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/wilderness/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6026 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/wilderness/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28916 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/wilderness/wilderness.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/grid/xyzgrid/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    54690 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/xyzgrid/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      202 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/xyzgrid/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20846 2023-07-14 10:46:28.000000 evennia-2.1.0/evennia/contrib/grid/xyzgrid/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7822 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/xyzgrid/example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13723 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/xyzgrid/launchcmd.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1145 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/xyzgrid/prototypes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42072 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/xyzgrid/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1043 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/xyzgrid/utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    40413 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/xyzgrid/xymap.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    52070 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/xyzgrid/xymap_legend.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10484 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/xyzgrid/xyzgrid.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24616 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/grid/xyzgrid/xyzroom.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/rpg/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      406 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/rpg/buffs/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22364 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/buffs/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/buffs/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    45607 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/buffs/buff.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3893 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/buffs/samplebuffs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16470 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/buffs/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/rpg/character_creator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3924 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/character_creator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      176 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/character_creator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8148 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/character_creator/character_creator.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21006 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/character_creator/example_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1552 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/character_creator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/rpg/dice/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2999 2023-07-14 12:31:31.000000 evennia-2.1.0/evennia/contrib/rpg/dice/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      177 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/dice/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12745 2023-07-14 12:26:05.000000 evennia-2.1.0/evennia/contrib/rpg/dice/dice.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1441 2023-06-17 16:27:00.000000 evennia-2.1.0/evennia/contrib/rpg/dice/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/rpg/health_bar/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1264 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/health_bar/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/health_bar/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4913 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/health_bar/health_bar.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1634 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/health_bar/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/rpg/rpsystem/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9938 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/rpsystem/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      793 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/rpsystem/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24722 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/rpsystem/rplanguage.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    65825 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/rpsystem/rpsystem.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14981 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/rpsystem/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/rpg/traits/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14246 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/traits/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      294 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/traits/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37184 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/traits/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    54252 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/rpg/traits/traits.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/tutorials/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      151 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/tutorials/batchprocessor/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1623 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/batchprocessor/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       50 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/batchprocessor/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3618 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/tutorials/bodyfunctions/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      471 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/bodyfunctions/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/bodyfunctions/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2311 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3324 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/bodyfunctions/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/tutorials/evadventure/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1180 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      164 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/tutorials/evadventure/batchscripts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       73 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/batchscripts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1820 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1436 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3996 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/build_techdemo.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/build_world.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12610 2023-07-14 11:02:18.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11199 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/chargen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16990 2023-07-14 11:21:22.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/combat_base.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27710 2023-07-14 11:29:21.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/combat_turnbased.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18189 2023-07-14 11:22:47.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/combat_twitch.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12500 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17918 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/dungeon.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1742 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/enums.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14537 2023-07-14 11:29:25.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/equipment.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12264 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/npcs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11174 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8743 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/quests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11708 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/random_tables.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3154 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12169 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/rules.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17153 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/shops.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1389 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/mixins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1266 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2151 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28143 2023-07-14 11:37:24.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_combat.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3741 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7811 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      542 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_npcs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4629 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2237 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8083 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      712 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1485 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/evadventure/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/tutorials/mirror/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      429 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/mirror/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/mirror/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2235 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/mirror/mirror.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/tutorials/red_button/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1344 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/red_button/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/red_button/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18609 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/red_button/red_button.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.393077 evennia-2.1.0/evennia/contrib/tutorials/talking_npc/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/talking_npc/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/talking_npc/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3697 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/talking_npc/talking_npc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      449 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/talking_npc/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4302 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      125 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    50297 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/build.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25293 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16130 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/mob.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42155 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42922 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7342 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/contrib/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       67 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/contrib/utils/auditing/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3303 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/auditing/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/auditing/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2065 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/auditing/outputs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8515 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/auditing/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6047 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/auditing/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/contrib/utils/fieldfill/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5816 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/fieldfill/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      288 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/fieldfill/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26382 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/fieldfill/fieldfill.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/contrib/utils/git_integration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3139 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/git_integration/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       86 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/git_integration/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7737 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/git_integration/git_integration.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2828 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/git_integration/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/contrib/utils/name_generator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9815 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/name_generator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/name_generator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   232619 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/name_generator/btn_givennames.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    56503 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/name_generator/btn_surnames.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14447 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/name_generator/namegen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4914 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/name_generator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/contrib/utils/random_string_generator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2165 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/random_string_generator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      268 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/random_string_generator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12595 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/random_string_generator/random_string_generator.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      737 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/random_string_generator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/contrib/utils/tree_select/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5935 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/tree_select/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      109 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/tree_select/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2199 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/tree_select/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20930 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/contrib/utils/tree_select/tree_select.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1521 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/commands/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      676 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/commands/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/commands/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7738 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/commands/command.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2636 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/commands/default_cmdsets.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      551 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/gitignore
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/server/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1718 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/server/conf/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      629 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/at_initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2154 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/at_search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/at_server_startstop.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2174 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/cmdparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1159 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/inlinefuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1419 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/inputfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1065 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/lockfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4009 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/mssp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      709 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/portal_services_plugins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      714 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/secret_settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      705 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/server_services_plugins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1347 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/serversession.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/conf/web_plugins.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/server/logs/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      839 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/server/logs/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/typeclasses/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      733 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/typeclasses/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/typeclasses/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3774 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/typeclasses/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2920 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/typeclasses/channels.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1525 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/typeclasses/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2044 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/typeclasses/exits.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8847 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/typeclasses/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      551 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/typeclasses/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4394 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/typeclasses/scripts.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2939 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      296 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/admin/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/admin/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      520 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/admin/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/api/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/api/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/static/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      849 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/static/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/game_template/web/static/rest_framework/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/static/rest_framework/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       53 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/static/rest_framework/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/static/rest_framework/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       47 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/static/rest_framework/images/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/game_template/web/static/webclient/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/static/webclient/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      132 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/static/webclient/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/static/webclient/js/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/static/webclient/js/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/game_template/web/static/website/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/static/website/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/static/website/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/static/website/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      135 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/static/website/images/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/templates/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      760 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/templates/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/templates/rest_framework/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       58 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/templates/rest_framework/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/templates/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      223 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/templates/webclient/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/templates/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/templates/website/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/templates/website/flatpages/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/templates/website/flatpages/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/templates/website/registration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      152 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/templates/website/registration/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1099 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1102 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/webclient/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/webclient/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      539 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/webclient/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1262 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/website/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/website/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      509 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/website/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/web/website/views/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/web/website/views/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/game_template/world/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/world/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/world/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      999 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/world/batch_cmds.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2186 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/world/help_entries.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3646 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/game_template/world/prototypes.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/help/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/help/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8013 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/help/filehelp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6229 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/help/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.397077 evennia-2.1.0/evennia/help/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2222 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/help/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      577 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/help/migrations/0002_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1688 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/help/migrations/0003_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/help/migrations/0004_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1166 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/help/migrations/0005_auto_20210530_1818.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      473 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/help/migrations/0006_alter_helpentry_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/help/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9729 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/help/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3736 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/help/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7673 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/help/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/locale/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2686 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/README
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/locale/de/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10764 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14475 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/locale/es/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3821 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30981 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/locale/fr/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26255 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    38581 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/locale/it/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6944 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    35844 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/locale/ko/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3569 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30924 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/locale/la/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/locale/la/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6537 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/la/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32786 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/la/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/locale/pl/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28236 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/locale/pt/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25584 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42122 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/locale/ru/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2281 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29419 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/locale/sv/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29036 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    43353 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/locale/zh/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/locale/zh/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3300 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/zh/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30540 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locale/zh/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/locks/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      240 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locks/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22093 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locks/lockfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26966 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locks/lockhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13732 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/locks/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/objects/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      120 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29704 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/objects/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4315 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1193 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/0002_auto_20140917_0756.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      810 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      530 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/0004_auto_20150118_1622.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      410 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/0005_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1599 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/0006_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/0007_objectdb_db_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/0008_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5028 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/0010_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1351 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/0011_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4011 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      488 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/0013_defaultobject_alter_objectdb_id_defaultcharacter_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13399 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   118892 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17072 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/objects/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/prototypes/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6567 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/prototypes/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/prototypes/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    92110 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/prototypes/menus.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2912 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/prototypes/protfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    46537 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/prototypes/prototypes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42860 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/prototypes/spawner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    39636 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/prototypes/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/scripts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      229 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11275 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/scripts/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4762 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      675 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0002_auto_20150118_1625.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1507 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      861 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0004_auto_20150306_1354.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      430 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0005_auto_20150306_1441.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      710 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0006_auto_20150310_2249.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      396 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0007_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      913 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0008_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1271 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0009_scriptdb_db_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0010_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4655 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0012_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      666 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0013_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      752 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0014_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3329 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0015_convert_contrib_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/0016_scriptbase_alter_scriptdb_id_defaultscript_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6311 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8746 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/monitorhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5326 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/scripthandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27441 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20801 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/taskhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10678 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24661 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/scripts/tickerhandler.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.401077 evennia-2.1.0/evennia/server/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      234 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8697 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/amp_client.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16629 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/connection_wizard.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7955 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/deprecations.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    79833 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/evennia_launcher.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.405077 evennia-2.1.0/evennia/server/game_index_client/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4321 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/game_index_client/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       45 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/game_index_client/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6256 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/game_index_client/client.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1990 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/game_index_client/service.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7622 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    19709 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/inputfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1708 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.405077 evennia-2.1.0/evennia/server/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      812 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1363 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/migrations/0002_auto_20190128_2311.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/migrations/0003_alter_serverconfig_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3818 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/models.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.405077 evennia-2.1.0/evennia/server/portal/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17922 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/amp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17520 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/amp_server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18478 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/discord.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11345 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/grapevine.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14242 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/irc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2571 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/mccp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3882 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/mssp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2341 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/mxp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2359 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/naws.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16018 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/portal.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17163 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/portalsessionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4450 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/rss.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15920 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/ssh.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3319 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/ssl.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1785 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/suppress_ga.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17379 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/telnet.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15609 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/telnet_oob.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4751 2023-07-14 11:12:11.000000 evennia-2.1.0/evennia/server/portal/telnet_ssl.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14725 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7073 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/ttype.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11403 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/webclient.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15897 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/portal/webclient_ajax.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.405077 evennia-2.1.0/evennia/server/profiling/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      212 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/profiling/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/profiling/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20881 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/profiling/dummyrunner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9427 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/profiling/dummyrunner_settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3924 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/profiling/memplot.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1375 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/profiling/settings_mixin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1095 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/profiling/test_queries.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5371 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/profiling/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1345 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/profiling/timetrace.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28633 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14599 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/serversession.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5616 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/session.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30009 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/sessionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4935 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/signals.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.405077 evennia-2.1.0/evennia/server/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/tests/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4721 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/tests/test_amp_connection.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      521 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/tests/test_initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7305 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/tests/test_launcher.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4444 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/tests/test_misc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9256 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/tests/test_server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/tests/testrunner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7101 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/throttle.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2763 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/validators.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8653 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/server/webserver.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    61131 2023-07-14 11:12:02.000000 evennia-2.1.0/evennia/settings_default.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.405077 evennia-2.1.0/evennia/typeclasses/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    64398 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    31304 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/managers.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.405077 evennia-2.1.0/evennia/typeclasses/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6101 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      768 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2266 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      833 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      922 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1444 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3899 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1699 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4230 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1993 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5265 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      821 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      362 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0015_alter_attribute_options.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37156 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30224 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17813 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/typeclasses/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.405077 evennia-2.1.0/evennia/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      320 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    51381 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/ansi.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15392 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/batchprocessors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8077 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10242 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/create.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32812 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/dbserialize.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41419 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/eveditor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2734 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/evennia-mode.el
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21081 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/evform.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    78957 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/evmenu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18330 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/evmore.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    65173 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/evtable.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    53272 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/funcparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8754 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/gametime.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/utils/idmapper/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1309 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/idmapper/LICENSE.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1097 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/idmapper/README_evennia.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1992 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/idmapper/README_orig.rst
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       64 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/idmapper/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1181 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/idmapper/manager.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24820 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/idmapper/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2876 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/idmapper/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18789 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/logger.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10265 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/optionclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6455 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/optionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11093 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/picklefield.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14179 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25088 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/test_resources.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/utils/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/utils/tests/data/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/data/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      274 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/data/broken_script.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1125 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/data/evform_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6245 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/data/evmenu_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      382 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/data/prototypes_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1608 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_ansi.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7052 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_batchprocessors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3463 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7032 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_create_functions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7888 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_dbserialize.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11752 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_eveditor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12172 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_evform.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11763 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_evmenu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12101 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_evtable.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30844 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_funcparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3942 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_gametime.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4460 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13564 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_tagparsing.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5509 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_text2html.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29937 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6371 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/tests/test_validatorfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12235 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/text2html.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    97272 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9489 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/validatorfuncs.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/utils/verb_conjugation/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18011 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/verb_conjugation/LICENSE.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/verb_conjugation/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9885 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/verb_conjugation/conjugate.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11298 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/verb_conjugation/pronouns.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10493 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/verb_conjugation/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   554408 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/utils/verb_conjugation/verbs.txt
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/web/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1150 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      127 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/web/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      428 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/admin/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14125 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/admin/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8627 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/admin/attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8508 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/admin/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/admin/frontpage.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1889 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/admin/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11915 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/admin/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4499 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/admin/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      508 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/admin/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8955 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/admin/tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      878 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/admin/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2884 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/admin/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/web/api/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7674 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/api/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/api/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4268 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/api/filters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3949 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/api/permissions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      277 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/api/root.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9905 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/api/serializers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8148 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/api/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2293 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/api/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5828 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/api/views.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/web/static/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/web/static/rest_framework/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/web/static/rest_framework/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      298 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/rest_framework/css/api.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/web/static/rest_framework/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/rest_framework/images/favicon.ico
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/web/static/webclient/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/web/static/webclient/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2104 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/css/goldenlayout.css
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27268 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/css/webclient.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/web/static/webclient/fonts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22208 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/fonts/DejaVuSansMono.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/web/static/webclient/js/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18546 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/evennia.js
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/web/static/webclient/js/plugins/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      563 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/clienthelp.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3914 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/default_in.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1958 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/default_out.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      345 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/default_unload.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3785 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/font.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29030 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/goldenlayout.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2114 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2981 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/history.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5031 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/hotbuttons.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1969 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/html.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1912 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/iframe.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4666 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/message_routing.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/multimedia.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2842 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/notifications.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      909 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/oob.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6262 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/options2.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2790 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/popups.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10949 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/plugins/text2html.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9705 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/js/webclient_gui.js
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/web/static/webclient/media/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3624 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/webclient/media/notification.wav
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/web/static/website/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.409077 evennia-2.1.0/evennia/web/static/website/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/website/css/custom.css
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2013 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/website/css/website.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.413076 evennia-2.1.0/evennia/web/static/website/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/website/images/LICENCE
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)    17938 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/website/images/evennia_logo.png
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21167 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/website/images/evennia_logo_festive.png
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/static/website/images/favicon.ico
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia/web/templates/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.413076 evennia-2.1.0/evennia/web/templates/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1621 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/admin/app_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6462 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/admin/frontpage.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.413076 evennia-2.1.0/evennia/web/templates/rest_framework/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      903 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/rest_framework/api.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      417 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/rest_framework/redoc.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.413076 evennia-2.1.0/evennia/web/templates/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7691 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/webclient/base.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1058 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/webclient/webclient.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.413076 evennia-2.1.0/evennia/web/templates/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      510 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/404.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      614 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/500.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4078 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/_menu.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3132 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/base.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2858 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/channel_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2667 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/channel_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1402 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/character_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/character_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1139 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/character_manage_list.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.413076 evennia-2.1.0/evennia/web/templates/website/flatpages/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      341 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/flatpages/default.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1501 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/generic_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2715 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/help_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5052 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/help_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5367 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/index.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      180 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/messages.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      900 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/object_confirm_delete.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1034 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/object_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/object_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1484 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/pagination.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.413076 evennia-2.1.0/evennia/web/templates/website/registration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/registration/logged_out.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1957 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/registration/login.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/registration/password_change_done.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1422 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/registration/password_change_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      813 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/registration/password_reset_complete.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1747 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/registration/password_reset_confirm.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/registration/password_reset_done.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      566 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/registration/password_reset_email.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1577 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/registration/password_reset_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/registration/register.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      671 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templates/website/tbi.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.413076 evennia-2.1.0/evennia/web/templatetags/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      287 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templatetags/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templatetags/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/templatetags/addclass.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.413076 evennia-2.1.0/evennia/web/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/utils/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1256 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/utils/adminsite.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/utils/apache_wsgi.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1815 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/utils/backends.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2035 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/utils/evennia_modpy_apache.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/utils/evennia_wsgi_apache.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4137 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/utils/general_context.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2712 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/utils/middleware.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2443 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/utils/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.413076 evennia-2.1.0/evennia/web/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/webclient/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/webclient/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      795 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/webclient/views.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.413076 evennia-2.1.0/evennia/web/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       31 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/website/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5736 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/website/forms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12503 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/website/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2575 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/website/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.413076 evennia-2.1.0/evennia/web/website/views/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/website/views/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2120 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/website/views/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5329 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/website/views/channels.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8330 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/website/views/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      311 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/website/views/errors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11796 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/website/views/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/website/views/index.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2353 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/website/views/mixins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9037 2023-06-10 17:39:32.000000 evennia-2.1.0/evennia/web/website/views/objects.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-07-14 13:16:43.381077 evennia-2.1.0/evennia.egg-info/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5239 2023-07-14 13:16:43.000000 evennia-2.1.0/evennia.egg-info/PKG-INFO
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34996 2023-07-14 13:16:43.000000 evennia-2.1.0/evennia.egg-info/SOURCES.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        1 2023-07-14 13:16:43.000000 evennia-2.1.0/evennia.egg-info/dependency_links.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2023-07-14 13:16:43.000000 evennia-2.1.0/evennia.egg-info/requires.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        8 2023-07-14 13:16:43.000000 evennia-2.1.0/evennia.egg-info/top_level.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3961 2023-07-14 13:12:56.000000 evennia-2.1.0/pyproject.toml
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       38 2023-07-14 13:16:43.413076 evennia-2.1.0/setup.cfg
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1388 2023-06-10 17:39:32.000000 evennia-2.1.0/setup.py
```

### Comparing `evennia-2.0.1/LICENSE.txt` & `evennia-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/PKG-INFO` & `evennia-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evennia
-Version: 2.0.1
+Version: 2.1.0
 Summary: A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc).
 Maintainer-email: Griatch <griatch@gmail.com>
 License: BSD
 Project-URL: Homepage, https://www.evennia.com
 Project-URL: Github, https://github.com/evennia/evennia
 Project-URL: Documentation, https://www.evennia.com/docs/latest/index.html
 Project-URL: Live Demo, https://demo.evennia.com/
```

### Comparing `evennia-2.0.1/README.md` & `evennia-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/__init__.py` & `evennia-2.1.0/evennia/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/__main__.py` & `evennia-2.1.0/evennia/__main__.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/accounts.py` & `evennia-2.1.0/evennia/accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/bots.py` & `evennia-2.1.0/evennia/accounts/bots.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/manager.py` & `evennia-2.1.0/evennia/accounts/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/migrations/0001_initial.py` & `evennia-2.1.0/evennia/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/migrations/0003_auto_20150209_2234.py` & `evennia-2.1.0/evennia/accounts/migrations/0003_auto_20150209_2234.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/migrations/0004_auto_20150403_2339.py` & `evennia-2.1.0/evennia/accounts/migrations/0004_auto_20150403_2339.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/migrations/0005_auto_20160905_0902.py` & `evennia-2.1.0/evennia/accounts/migrations/0005_auto_20160905_0902.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/migrations/0006_auto_20170606_1731.py` & `evennia-2.1.0/evennia/accounts/migrations/0006_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/migrations/0007_copy_player_to_account.py` & `evennia-2.1.0/evennia/accounts/migrations/0007_copy_player_to_account.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/migrations/0008_auto_20190128_1820.py` & `evennia-2.1.0/evennia/accounts/migrations/0008_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/migrations/0009_auto_20191025_0831.py` & `evennia-2.1.0/evennia/accounts/migrations/0009_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py` & `evennia-2.1.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/models.py` & `evennia-2.1.0/evennia/accounts/models.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/accounts/tests.py` & `evennia-2.1.0/evennia/accounts/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/cmdhandler.py` & `evennia-2.1.0/evennia/commands/cmdhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/cmdparser.py` & `evennia-2.1.0/evennia/commands/cmdparser.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/cmdset.py` & `evennia-2.1.0/evennia/commands/cmdset.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/cmdsethandler.py` & `evennia-2.1.0/evennia/commands/cmdsethandler.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/command.py` & `evennia-2.1.0/evennia/commands/command.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/account.py` & `evennia-2.1.0/evennia/commands/default/account.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/admin.py` & `evennia-2.1.0/evennia/commands/default/admin.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/batchprocess.py` & `evennia-2.1.0/evennia/commands/default/batchprocess.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/building.py` & `evennia-2.1.0/evennia/commands/default/building.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/cmdset_account.py` & `evennia-2.1.0/evennia/commands/default/cmdset_account.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/cmdset_character.py` & `evennia-2.1.0/evennia/commands/default/cmdset_character.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/cmdset_unloggedin.py` & `evennia-2.1.0/evennia/commands/default/cmdset_unloggedin.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/comms.py` & `evennia-2.1.0/evennia/commands/default/comms.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/general.py` & `evennia-2.1.0/evennia/commands/default/general.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/help.py` & `evennia-2.1.0/evennia/commands/default/help.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/muxcommand.py` & `evennia-2.1.0/evennia/commands/default/muxcommand.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/syscommands.py` & `evennia-2.1.0/evennia/commands/default/syscommands.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/system.py` & `evennia-2.1.0/evennia/commands/default/system.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/tests.py` & `evennia-2.1.0/evennia/commands/default/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/default/unloggedin.py` & `evennia-2.1.0/evennia/commands/default/unloggedin.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/commands/tests.py` & `evennia-2.1.0/evennia/commands/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/comms.py` & `evennia-2.1.0/evennia/comms/comms.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/managers.py` & `evennia-2.1.0/evennia/comms/managers.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0001_initial.py` & `evennia-2.1.0/evennia/comms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0003_auto_20140917_0756.py` & `evennia-2.1.0/evennia/comms/migrations/0003_auto_20140917_0756.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0005_auto_20150223_1517.py` & `evennia-2.1.0/evennia/comms/migrations/0005_auto_20150223_1517.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py` & `evennia-2.1.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0007_msg_db_tags.py` & `evennia-2.1.0/evennia/comms/migrations/0007_msg_db_tags.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0009_auto_20160921_1731.py` & `evennia-2.1.0/evennia/comms/migrations/0009_auto_20160921_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0010_auto_20161206_1912.py` & `evennia-2.1.0/evennia/comms/migrations/0010_auto_20161206_1912.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0011_auto_20170217_2039.py` & `evennia-2.1.0/evennia/comms/migrations/0011_auto_20170217_2039.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0011_auto_20170606_1731.py` & `evennia-2.1.0/evennia/comms/migrations/0011_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0013_auto_20170705_1726.py` & `evennia-2.1.0/evennia/comms/migrations/0013_auto_20170705_1726.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0014_auto_20170705_1736.py` & `evennia-2.1.0/evennia/comms/migrations/0014_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0015_auto_20170706_2041.py` & `evennia-2.1.0/evennia/comms/migrations/0015_auto_20170706_2041.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0017_auto_20190128_1820.py` & `evennia-2.1.0/evennia/comms/migrations/0017_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0018_auto_20191025_0831.py` & `evennia-2.1.0/evennia/comms/migrations/0018_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0019_auto_20210514_2032.py` & `evennia-2.1.0/evennia/comms/migrations/0019_auto_20210514_2032.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0020_auto_20210514_2210.py` & `evennia-2.1.0/evennia/comms/migrations/0020_auto_20210514_2210.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0021_auto_20210520_2137.py` & `evennia-2.1.0/evennia/comms/migrations/0021_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py` & `evennia-2.1.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/models.py` & `evennia-2.1.0/evennia/comms/models.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/comms/tests.py` & `evennia-2.1.0/evennia/comms/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/README.md` & `evennia-2.1.0/evennia/contrib/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/awsstorage/README.md` & `evennia-2.1.0/evennia/contrib/base_systems/awsstorage/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py` & `evennia-2.1.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/awsstorage/tests.py` & `evennia-2.1.0/evennia/contrib/base_systems/awsstorage/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/building_menu/README.md` & `evennia-2.1.0/evennia/contrib/base_systems/building_menu/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/building_menu/building_menu.py` & `evennia-2.1.0/evennia/contrib/base_systems/building_menu/building_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/building_menu/tests.py` & `evennia-2.1.0/evennia/contrib/base_systems/building_menu/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/color_markups/README.md` & `evennia-2.1.0/evennia/contrib/base_systems/color_markups/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/color_markups/color_markups.py` & `evennia-2.1.0/evennia/contrib/base_systems/color_markups/color_markups.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/color_markups/tests.py` & `evennia-2.1.0/evennia/contrib/base_systems/color_markups/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/components/README.md` & `evennia-2.1.0/evennia/contrib/base_systems/components/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/components/__init__.py` & `evennia-2.1.0/evennia/contrib/base_systems/components/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/components/component.py` & `evennia-2.1.0/evennia/contrib/base_systems/components/component.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/components/dbfield.py` & `evennia-2.1.0/evennia/contrib/base_systems/components/dbfield.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/components/holder.py` & `evennia-2.1.0/evennia/contrib/base_systems/components/holder.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/components/signals.py` & `evennia-2.1.0/evennia/contrib/base_systems/components/signals.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/components/tests.py` & `evennia-2.1.0/evennia/contrib/base_systems/components/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/custom_gametime/README.md` & `evennia-2.1.0/evennia/contrib/base_systems/custom_gametime/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/custom_gametime/custom_gametime.py` & `evennia-2.1.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/custom_gametime/tests.py` & `evennia-2.1.0/evennia/contrib/base_systems/custom_gametime/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/email_login/README.md` & `evennia-2.1.0/evennia/contrib/base_systems/email_login/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/email_login/connection_screens.py` & `evennia-2.1.0/evennia/contrib/base_systems/email_login/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/email_login/email_login.py` & `evennia-2.1.0/evennia/contrib/base_systems/email_login/email_login.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/email_login/tests.py` & `evennia-2.1.0/evennia/contrib/base_systems/email_login/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/godotwebsocket/README.md` & `evennia-2.1.0/evennia/contrib/base_systems/godotwebsocket/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/godotwebsocket/__init__.py` & `evennia-2.1.0/evennia/contrib/base_systems/godotwebsocket/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py` & `evennia-2.1.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py` & `evennia-2.1.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/godotwebsocket/webclient.py` & `evennia-2.1.0/evennia/contrib/base_systems/godotwebsocket/webclient.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/ingame_python/README.md` & `evennia-2.1.0/evennia/contrib/base_systems/ingame_python/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/ingame_python/callbackhandler.py` & `evennia-2.1.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/ingame_python/commands.py` & `evennia-2.1.0/evennia/contrib/base_systems/ingame_python/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/ingame_python/eventfuncs.py` & `evennia-2.1.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/ingame_python/scripts.py` & `evennia-2.1.0/evennia/contrib/base_systems/ingame_python/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/ingame_python/tests.py` & `evennia-2.1.0/evennia/contrib/base_systems/ingame_python/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/ingame_python/typeclasses.py` & `evennia-2.1.0/evennia/contrib/base_systems/ingame_python/typeclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/ingame_python/utils.py` & `evennia-2.1.0/evennia/contrib/base_systems/ingame_python/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/menu_login/README.md` & `evennia-2.1.0/evennia/contrib/base_systems/menu_login/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/menu_login/connection_screens.py` & `evennia-2.1.0/evennia/contrib/base_systems/menu_login/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/menu_login/menu_login.py` & `evennia-2.1.0/evennia/contrib/base_systems/menu_login/menu_login.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/mux_comms_cmds/README.md` & `evennia-2.1.0/evennia/contrib/base_systems/mux_comms_cmds/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py` & `evennia-2.1.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/mux_comms_cmds/tests.py` & `evennia-2.1.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/unixcommand/README.md` & `evennia-2.1.0/evennia/contrib/base_systems/unixcommand/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/unixcommand/tests.py` & `evennia-2.1.0/evennia/contrib/base_systems/unixcommand/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/base_systems/unixcommand/unixcommand.py` & `evennia-2.1.0/evennia/contrib/base_systems/unixcommand/unixcommand.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/README.md` & `evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/commands.py` & `evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/menu.py` & `evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/menu.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/objects.py` & `evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/room.py` & `evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/room.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/scripts.py` & `evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/state.py` & `evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/state.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/states/README.md` & `evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/states/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py` & `evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/tests.py` & `evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/full_systems/evscaperoom/utils.py` & `evennia-2.1.0/evennia/contrib/full_systems/evscaperoom/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/barter/README.md` & `evennia-2.1.0/evennia/contrib/game_systems/barter/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/barter/barter.py` & `evennia-2.1.0/evennia/contrib/game_systems/barter/barter.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/barter/tests.py` & `evennia-2.1.0/evennia/contrib/game_systems/barter/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/clothing/README.md` & `evennia-2.1.0/evennia/contrib/game_systems/clothing/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ```
 
 ## Usage
 
 Once installed, you can use the default builder commands to create clothes
 with which to test the system:
 
-    create a pretty shirt : evennia.contrib.game_systems.clothing.Clothing
+    create a pretty shirt : evennia.contrib.game_systems.clothing.ContribClothing
     set shirt/clothing_type = 'top'
     wear shirt
 
 A character's description may look like this:
 
     Superuser(#1)
     This is User #1.
```

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/clothing/clothing.py` & `evennia-2.1.0/evennia/contrib/game_systems/clothing/clothing.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,15 +556,15 @@
             return
         if to_cover == cover_with:
             self.caller.msg("You can't cover an item with itself!")
             return
 
         if not inherits_from(cover_with, ContribClothing):
             self.caller.msg(f"{cover_with.name} isn't something you can wear.")
-            rturn
+            return
 
         if cover_with.db.clothing_type in CLOTHING_TYPE_CANT_COVER_WITH:
             self.caller.msg(f"You can't cover anything with {cover_with.name}.")
             return
 
         if covered_by := cover_with.db.covered_by:
             self.caller.msg(f"{cover_with.name} is already covered by {covered_by.name}.")
```

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/clothing/tests.py` & `evennia-2.1.0/evennia/contrib/game_systems/clothing/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/containers/README.md` & `evennia-2.1.0/evennia/contrib/game_systems/containers/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/containers/containers.py` & `evennia-2.1.0/evennia/contrib/game_systems/containers/containers.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/containers/tests.py` & `evennia-2.1.0/evennia/contrib/game_systems/containers/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/cooldowns/README.md` & `evennia-2.1.0/evennia/contrib/game_systems/cooldowns/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/cooldowns/cooldowns.py` & `evennia-2.1.0/evennia/contrib/game_systems/cooldowns/cooldowns.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/cooldowns/tests.py` & `evennia-2.1.0/evennia/contrib/game_systems/cooldowns/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/crafting/README.md` & `evennia-2.1.0/evennia/contrib/game_systems/crafting/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/crafting/crafting.py` & `evennia-2.1.0/evennia/contrib/game_systems/crafting/crafting.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/crafting/example_recipes.py` & `evennia-2.1.0/evennia/contrib/game_systems/crafting/example_recipes.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/crafting/tests.py` & `evennia-2.1.0/evennia/contrib/game_systems/crafting/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/gendersub/README.md` & `evennia-2.1.0/evennia/contrib/game_systems/gendersub/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/gendersub/gendersub.py` & `evennia-2.1.0/evennia/contrib/game_systems/gendersub/gendersub.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/gendersub/tests.py` & `evennia-2.1.0/evennia/contrib/game_systems/gendersub/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/mail/README.md` & `evennia-2.1.0/evennia/contrib/game_systems/mail/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/mail/mail.py` & `evennia-2.1.0/evennia/contrib/game_systems/mail/mail.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/mail/tests.py` & `evennia-2.1.0/evennia/contrib/game_systems/mail/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/multidescer/README.md` & `evennia-2.1.0/evennia/contrib/game_systems/multidescer/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/multidescer/multidescer.py` & `evennia-2.1.0/evennia/contrib/game_systems/multidescer/multidescer.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/multidescer/tests.py` & `evennia-2.1.0/evennia/contrib/game_systems/multidescer/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/puzzles/README.md` & `evennia-2.1.0/evennia/contrib/game_systems/puzzles/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/puzzles/puzzles.py` & `evennia-2.1.0/evennia/contrib/game_systems/puzzles/puzzles.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/puzzles/tests.py` & `evennia-2.1.0/evennia/contrib/game_systems/puzzles/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/turnbattle/README.md` & `evennia-2.1.0/evennia/contrib/game_systems/turnbattle/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/turnbattle/tb_basic.py` & `evennia-2.1.0/evennia/contrib/game_systems/turnbattle/tb_basic.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/turnbattle/tb_equip.py` & `evennia-2.1.0/evennia/contrib/game_systems/turnbattle/tb_equip.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/turnbattle/tb_items.py` & `evennia-2.1.0/evennia/contrib/game_systems/turnbattle/tb_items.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/turnbattle/tb_magic.py` & `evennia-2.1.0/evennia/contrib/game_systems/turnbattle/tb_magic.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/turnbattle/tb_range.py` & `evennia-2.1.0/evennia/contrib/game_systems/turnbattle/tb_range.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/game_systems/turnbattle/tests.py` & `evennia-2.1.0/evennia/contrib/game_systems/turnbattle/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/extended_room/README.md` & `evennia-2.1.0/evennia/contrib/grid/extended_room/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/extended_room/extended_room.py` & `evennia-2.1.0/evennia/contrib/grid/extended_room/extended_room.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,16 @@
       to add an actual database object for it. The `detail` command is used to add/remove details.
 
     Room messages
     - Set `room_message_rate > 0` and add a list of `room_messages`. These will be randomly
       echoed to the room at the given rate.
 
     """
+    # fallback description if nothing else is set
+    fallback_desc = "You see nothing special."
 
     # tag room_state category
     room_state_tag_category = "room_state"
 
     # time setup
     months_per_year = 12
     hours_per_day = 24
@@ -406,15 +408,15 @@
 
         # no matching room_states, use time-based seasons. Also support legacy *_desc form
         season = self.get_season()
         if desc := descriptions.get(f"desc_{season}") or descriptions.get(f"{season}_desc"):
             return desc
 
         # fallback to normal desc Attribute
-        return self.attributes.get("desc")
+        return self.attributes.get("desc", self.fallback_desc)
 
     def replace_legacy_time_of_day_markup(self, desc):
         """
         Filter description by legacy markup like `<morning>...</morning>`. Filter
         out all such markings that does not match the current time. Supports
         'morning', 'afternoon', 'evening' and 'night'.
 
@@ -424,14 +426,15 @@
         Returns:
             str: A possibly modified description.
 
         Notes:
             This is legacy. Use the $state markup for new rooms instead.
 
         """
+        desc = desc or ""
         time_of_day = self.get_time_of_day()
 
         # regexes for in-desc replacements (gets cached)
         if not hasattr(self, "legacy_timeofday_regex_map"):
             timeslots = deque()
             for time_of_day in self.times_of_day:
                 timeslots.append(
```

### Comparing `evennia-2.0.1/evennia/contrib/grid/extended_room/tests.py` & `evennia-2.1.0/evennia/contrib/grid/extended_room/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/ingame_map_display/README.md` & `evennia-2.1.0/evennia/contrib/grid/ingame_map_display/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/ingame_map_display/ingame_map_display.py` & `evennia-2.1.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/ingame_map_display/tests.py` & `evennia-2.1.0/evennia/contrib/grid/ingame_map_display/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/mapbuilder/README.md` & `evennia-2.1.0/evennia/contrib/grid/mapbuilder/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/mapbuilder/mapbuilder.py` & `evennia-2.1.0/evennia/contrib/grid/mapbuilder/mapbuilder.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/mapbuilder/tests.py` & `evennia-2.1.0/evennia/contrib/grid/mapbuilder/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/simpledoor/README.md` & `evennia-2.1.0/evennia/contrib/grid/simpledoor/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/simpledoor/simpledoor.py` & `evennia-2.1.0/evennia/contrib/grid/simpledoor/simpledoor.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/simpledoor/tests.py` & `evennia-2.1.0/evennia/contrib/grid/simpledoor/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/slow_exit/README.md` & `evennia-2.1.0/evennia/contrib/grid/slow_exit/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/slow_exit/slow_exit.py` & `evennia-2.1.0/evennia/contrib/grid/slow_exit/slow_exit.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/slow_exit/tests.py` & `evennia-2.1.0/evennia/contrib/grid/slow_exit/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/wilderness/README.md` & `evennia-2.1.0/evennia/contrib/grid/wilderness/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/wilderness/tests.py` & `evennia-2.1.0/evennia/contrib/grid/wilderness/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/wilderness/wilderness.py` & `evennia-2.1.0/evennia/contrib/grid/wilderness/wilderness.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/xyzgrid/README.md` & `evennia-2.1.0/evennia/contrib/grid/xyzgrid/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/xyzgrid/commands.py` & `evennia-2.1.0/evennia/contrib/grid/xyzgrid/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         X, Y, *Z = inp.split(",", 2)
         if Z:
             # Z was specified
             Z = Z[0]
         else:
             # use current location's Z, if it exists
             try:
-                xyz = self.caller.xyz
+                xyz = self.caller.location.xyz
             except AttributeError:
                 self.caller.msg(
                     "Z-coordinate is also required since you are not currently "
                     "in a room with a Z coordinate of its own."
                 )
                 raise InterruptCommand
             else:
```

### Comparing `evennia-2.0.1/evennia/contrib/grid/xyzgrid/example.py` & `evennia-2.1.0/evennia/contrib/grid/xyzgrid/example.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/xyzgrid/launchcmd.py` & `evennia-2.1.0/evennia/contrib/grid/xyzgrid/launchcmd.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/xyzgrid/prototypes.py` & `evennia-2.1.0/evennia/contrib/grid/xyzgrid/prototypes.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/xyzgrid/tests.py` & `evennia-2.1.0/evennia/contrib/grid/xyzgrid/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/xyzgrid/utils.py` & `evennia-2.1.0/evennia/contrib/grid/xyzgrid/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/xyzgrid/xymap.py` & `evennia-2.1.0/evennia/contrib/grid/xyzgrid/xymap.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/xyzgrid/xymap_legend.py` & `evennia-2.1.0/evennia/contrib/grid/xyzgrid/xymap_legend.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/xyzgrid/xyzgrid.py` & `evennia-2.1.0/evennia/contrib/grid/xyzgrid/xyzgrid.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/grid/xyzgrid/xyzroom.py` & `evennia-2.1.0/evennia/contrib/grid/xyzgrid/xyzroom.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/buffs/README.md` & `evennia-2.1.0/evennia/contrib/rpg/buffs/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/buffs/buff.py` & `evennia-2.1.0/evennia/contrib/rpg/buffs/buff.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/buffs/samplebuffs.py` & `evennia-2.1.0/evennia/contrib/rpg/buffs/samplebuffs.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/buffs/tests.py` & `evennia-2.1.0/evennia/contrib/rpg/buffs/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/character_creator/README.md` & `evennia-2.1.0/evennia/contrib/rpg/character_creator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/character_creator/character_creator.py` & `evennia-2.1.0/evennia/contrib/rpg/character_creator/character_creator.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/character_creator/example_menu.py` & `evennia-2.1.0/evennia/contrib/rpg/character_creator/example_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/character_creator/tests.py` & `evennia-2.1.0/evennia/contrib/rpg/character_creator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/dice/dice.py` & `evennia-2.1.0/evennia/contrib/rpg/dice/dice.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,121 +29,188 @@
 # in mygame/commands/default_cmdsets.py
 
 # ...
 from evennia.contrib.rpg import dice  <---
 
 class CharacterCmdSet(default_cmds.CharacterCmdSet):
     # ...
-    def at_object_creation(self):
+    def at_cmdset_creation(self):
         # ...
         self.add(dice.CmdDice())  # <---
 
 ```
 
 # Usage:
 
     roll 1d100 + 10
 
 To roll dice in code, use the `roll` function from this module:
 
-```python
+    from evennia.contrib.rpg import dice
 
-from evennia.contrib.rpg import dice
-dice.roll_dice(3, 10, ("+", 2))  # 3d10 + 2
+    dice.roll("3d10 + 2")
+
+
+If your system generates the dice dynamically you can also enter each part
+of the roll separately:
+
+    dice.roll(3, 10, ("+", 2))  # 3d10 + 2
 
-```
 
 """
 import re
+from ast import literal_eval
 from random import randint
 
 from evennia import CmdSet, default_cmds
+from evennia.utils.utils import simple_eval
 
 
-def roll(dicenum, dicetype, modifier=None, conditional=None, return_tuple=False):
+def roll(
+    dice,
+    dicetype=6,
+    modifier=None,
+    conditional=None,
+    return_tuple=False,
+    max_dicenum=10,
+    max_dicetype=1000,
+):
     """
     This is a standard dice roller.
 
     Args:
-     dicenum (int): Number of dice to roll (the result to be added).
-     dicetype (int): Number of sides of the dice to be rolled.
-     modifier (tuple): A tuple `(operator, value)`, where operator is
+     dice (int or str): If an `int`, this is the number of dice to roll, and `dicetype` is used
+        to determine the type. If a `str`, it should be on the form `NdM` where `N` is the number
+        of dice and `M` is the number of sides on each die. Also
+        `NdM [modifier] [number] [conditional]` is understood, e.g. `1d6 + 3`
+        or `2d10 / 2 > 10`.
+     dicetype (int, optional): Number of sides of the dice to be rolled. Ignored if
+        `dice` is a string.
+     modifier (tuple, optional): A tuple `(operator, value)`, where operator is
         one of `"+"`, `"-"`, `"/"` or `"*"`. The result of the dice
-        roll(s) will be modified by this value.
-     conditional (tuple): A tuple `(conditional, value)`, where
+        roll(s) will be modified by this value. Ignored if `dice` is a string.
+     conditional (tuple, optional): A tuple `(conditional, value)`, where
         conditional is one of `"=="`,`"<"`,`">"`,`">="`,`"<=`" or "`!=`".
-        This allows the roller to directly return a result depending
-        on if the conditional was passed or not.
+        Ignored if `dice` is a string.
      return_tuple (bool): Return a tuple with all individual roll
         results or not.
+     max_dicenum (int): The max number of dice to allow to be rolled.
+     max_dicetype (int): The max number of sides on the dice to roll.
 
     Returns:
-        roll_result (int): The result of the roll + modifiers. This is the
-             default return.
-        condition_result (bool): A True/False value returned if `conditional`
-            is set but not `return_tuple`. This effectively hides the result
-            of the roll.
-        full_result (tuple): If, return_tuple` is `True`, instead
-            return a tuple `(result, outcome, diff, rolls)`. Here,
-            `result` is the normal result of the roll + modifiers.
-            `outcome` and `diff` are the boolean result of the roll and
-            absolute difference to the `conditional` input; they will
-            be will be `None` if `conditional` is not set. `rolls` is
-            itself a tuple holding all the individual rolls in the case of
-            multiple die-rolls.
+        int, bool or tuple : By default, this is the result of the roll + modifiers.  If
+        `conditional` is given, or `dice` is a string defining a conditional, then a True/False
+        value is returned. Finally, if `return_tuple` is set, this is a tuple
+        `(result, outcome, diff, rolls)`, where, `result` is the the normal result of the
+        roll + modifiers,  `outcome` and `diff` are the boolean absolute difference between the roll
+        and the `conditional` input; both will be will be `None` if `conditional` is not set.
+        The `rolls` a tuple holding all the individual rolls (one or more depending on how many
+        dice were rolled).
 
     Raises:
         TypeError if non-supported modifiers or conditionals are given.
 
     Notes:
         All input numbers are converted to integers.
 
     Examples:
-        print roll_dice(2, 6) # 2d6
-        <<< 7
-        print roll_dice(1, 100, ('+', 5) # 1d100 + 5
-        <<< 34
-        print roll_dice(1, 20, conditional=('<', 10) # let'say we roll 3
-        <<< True
-        print roll_dice(3, 10, return_tuple=True)
-        <<< (11, None, None, (2, 5, 4))
-        print roll_dice(2, 20, ('-', 2), conditional=('>=', 10), return_tuple=True)
-        <<< (8, False, 2, (4, 6)) # roll was 4 + 6 - 2 = 8
+        ::
+            # string form
+            print roll("3d6 + 2")
+            10
+            print roll("2d10 + 2 > 10")
+            True
+            print roll("2d20 - 2 >= 10")
+            (8, False, 2, (4, 6)) # roll was 4 + 6 - 2 = 8
+
+            # explicit arguments
+            print roll(2, 6) # 2d6
+            7
+            print roll(1, 100, ('+', 5) # 1d100 + 5
+            4
+            print roll(1, 20, conditional=('<', 10) # let'say we roll 3
+            True
+            print roll(3, 10, return_tuple=True)
+            (11, None, None, (2, 5, 4))
+            print roll(2, 20, ('-', 2), conditional=('>=', 10), return_tuple=True)
+            (8, False, 2, (4, 6)) # roll was 4 + 6 - 2 = 8
 
     """
-    dicenum = int(dicenum)
-    dicetype = int(dicetype)
+
+    modifier_string = ""
+    conditional_string = ""
+    conditional_value = None
+    if isinstance(dice, str) and "d" in dice.lower():
+        # A string is given, parse it as NdM dice notation
+        roll_string = dice.lower()
+
+        # split to get the NdM syntax
+        dicenum, rest = roll_string.split("d", 1)
+
+        # parse packwards right-to-left
+        if any(True for cond in ("==", "<", ">", "!=", "<=", ">=") if cond in rest):
+            # split out any conditionals, like '< 12'
+            rest, *conditionals = re.split(r"(==|<=|>=|<|>|!=)", rest, maxsplit=1)
+            try:
+                conditional_value = int(conditionals[1])
+            except ValueError:
+                raise TypeError(
+                    f"Conditional '{conditionals[-1]}' was not recognized. Must be a number."
+                )
+            conditional_string = "".join(conditionals)
+
+        if any(True for op in ("+", "-", "*", "/") if op in rest):
+            # split out any modifiers, like '+ 2'
+            rest, *modifiers = re.split(r"(\+|-|/|\*)", rest, maxsplit=1)
+            modifier_string = "".join(modifiers)
+
+        # whatever is left is the dice type
+        dicetype = rest
+
+    else:
+        # an integer is given - explicit modifiers and conditionals as part of kwargs
+        dicenum = int(dice)
+        dicetype = int(dicetype)
+        if modifier:
+            modifier_string = "".join(str(part) for part in modifier)
+        if conditional:
+            conditional_value = int(conditional[1])
+            conditional_string = "".join(str(part) for part in conditional)
+
+    try:
+        dicenum = int(dicenum)
+        dicetype = int(dicetype)
+    except Exception:
+        raise TypeError(
+            f"The number of dice and dice-size must both be numerical. Got '{dicenum}' "
+            f"and '{dicetype}'."
+        )
+    if 0 < dicenum > max_dicenum:
+        raise TypeError(f"Invalid number of dice rolled (must be between 1 and {max_dicenum}).")
+    if 0 < dicetype > max_dicetype:
+        raise TypeError(f"Invalid die-size used (must be between 1 and {max_dicetype} sides).")
 
     # roll all dice, remembering each roll
-    rolls = tuple([randint(1, dicetype) for roll in range(dicenum)])
+    rolls = tuple([randint(1, dicetype) for _ in range(dicenum)])
     result = sum(rolls)
 
-    if modifier:
-        # make sure to check types well before eval
-        mod, modvalue = modifier
-        if mod not in ("+", "-", "*", "/"):
-            raise TypeError("Non-supported dice modifier: %s" % mod)
-        modvalue = int(modvalue)  # for safety
-        result = eval("%s %s %s" % (result, mod, modvalue))
+    if modifier_string:
+        result = simple_eval(f"{result} {modifier_string}")
+
     outcome, diff = None, None
-    if conditional:
-        # make sure to check types well before eval
-        cond, condvalue = conditional
-        if cond not in (">", "<", ">=", "<=", "!=", "=="):
-            raise TypeError("Non-supported dice result conditional: %s" % conditional)
-        condvalue = int(condvalue)  # for safety
-        outcome = eval("%s %s %s" % (result, cond, condvalue))  # True/False
-        diff = abs(result - condvalue)
+    if conditional_string and conditional_value:
+        outcome = simple_eval(f"{result} {conditional_string}")
+        diff = abs(result - conditional_value)
+
     if return_tuple:
         return result, outcome, diff, rolls
+    elif conditional or (conditional_string and conditional_value):
+        return outcome  # True|False
     else:
-        if conditional:
-            return outcome
-        else:
-            return result
+        return result  # integer
 
 
 # legacy alias
 roll_dice = roll
 
 
 RE_PARTS = re.compile(r"(d|\+|-|/|\*|<|>|<=|>=|!=|==)")
@@ -231,15 +298,16 @@
         try:
             result, outcome, diff, rolls = roll_dice(
                 ndice, nsides, modifier=modifier, conditional=conditional, return_tuple=True
             )
         except ValueError:
             self.caller.msg(
                 "You need to enter valid integer numbers, modifiers and operators."
-                " |w%s|n was not understood." % self.args
+                " |w%s|n was not understood."
+                % self.args
             )
             return
         # format output
         if len(rolls) > 1:
             rolls = ", ".join(str(roll) for roll in rolls[:-1]) + " and " + str(rolls[-1])
         else:
             rolls = rolls[0]
```

### Comparing `evennia-2.0.1/evennia/contrib/rpg/dice/tests.py` & `evennia-2.1.0/evennia/contrib/rpg/dice/tests.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 """
 Testing of TestDice.
 
 """
 
-from mock import patch
-
 from evennia.commands.default.tests import BaseEvenniaCommandTest
+from mock import patch
 
 from . import dice
 
 
 @patch("evennia.contrib.rpg.dice.dice.randint", return_value=5)
 class TestDice(BaseEvenniaCommandTest):
     def test_roll_dice(self, mocked_randint):
-        self.assertEqual(dice.roll_dice(6, 6, modifier=("+", 4)), mocked_randint() * 6 + 4)
-        self.assertEqual(dice.roll_dice(6, 6, conditional=("<", 35)), True)
-        self.assertEqual(dice.roll_dice(6, 6, conditional=(">", 33)), False)
+        self.assertEqual(dice.roll(6, 6, modifier=("+", 4)), mocked_randint() * 6 + 4)
+        self.assertEqual(dice.roll(6, 6, conditional=("<", 35)), True)
+        self.assertEqual(dice.roll(6, 6, conditional=(">", 33)), False)
 
     def test_cmddice(self, mocked_randint):
         self.call(
             dice.CmdDice(), "3d6 + 4", "You roll 3d6 + 4.| Roll(s): 5, 5 and 5. Total result is 19."
         )
         self.call(dice.CmdDice(), "100000d1000", "The maximum roll allowed is 10000d10000.")
         self.call(dice.CmdDice(), "/secret 3d6 + 4", "You roll 3d6 + 4 (secret, not echoed).")
+
+    def test_string_form(self, mocked_randint):
+        self.assertEqual(dice.roll("6d6 + 4"), mocked_randint() * 6 + 4)
+        self.assertEqual(dice.roll("6d6 < 35"), True)
+        self.assertEqual(dice.roll("6d6 > 35"), False)
+        self.assertEqual(dice.roll("2d10 + 5 >= 14"), True)
+
+    def test_maxvals(self, mocked_randint):
+        with self.assertRaises(TypeError):
+            dice.roll(11, 1001, max_dicenum=10, max_dicetype=1000)
+        with self.assertRaises(TypeError):
+            dice.roll(10, 1001, max_dicenum=10, max_dicetype=1000)
```

### Comparing `evennia-2.0.1/evennia/contrib/rpg/health_bar/README.md` & `evennia-2.1.0/evennia/contrib/rpg/health_bar/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/health_bar/health_bar.py` & `evennia-2.1.0/evennia/contrib/rpg/health_bar/health_bar.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/health_bar/tests.py` & `evennia-2.1.0/evennia/contrib/rpg/health_bar/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/rpsystem/README.md` & `evennia-2.1.0/evennia/contrib/rpg/rpsystem/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/rpsystem/__init__.py` & `evennia-2.1.0/evennia/contrib/rpg/rpsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/rpsystem/rplanguage.py` & `evennia-2.1.0/evennia/contrib/rpg/rpsystem/rplanguage.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/rpsystem/rpsystem.py` & `evennia-2.1.0/evennia/contrib/rpg/rpsystem/rpsystem.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/rpsystem/tests.py` & `evennia-2.1.0/evennia/contrib/rpg/rpsystem/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/traits/README.md` & `evennia-2.1.0/evennia/contrib/rpg/traits/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/traits/tests.py` & `evennia-2.1.0/evennia/contrib/rpg/traits/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/rpg/traits/traits.py` & `evennia-2.1.0/evennia/contrib/rpg/traits/traits.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/batchprocessor/README.md` & `evennia-2.1.0/evennia/contrib/tutorials/batchprocessor/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev` & `evennia-2.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/batchprocessor/example_batch_code.py` & `evennia-2.1.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py` & `evennia-2.1.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/bodyfunctions/tests.py` & `evennia-2.1.0/evennia/contrib/tutorials/bodyfunctions/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/README.md` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/batchscripts/turnbased_combat_demo.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/batchscripts/twitch_combat_demo.ev`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/build_techdemo.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/build_techdemo.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/characters.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/characters.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/chargen.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/chargen.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/combat_base.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/combat_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,16 +352,14 @@
         Gregor (Hurt)                   Goblin brawler(Hurt)
         Bob (Perfect)         vs        Goblin grunt 1 (Hurt)
                                         Goblin grunt 2 (Perfect)
                                         Goblin grunt 3 (Wounded)
 
         """
         allies, enemies = self.get_sides(combatant)
-        # we must include outselves at the top of the list (we are not returned from get_sides)
-        allies.insert(0, combatant)
         nallies, nenemies = len(allies), len(enemies)
 
         # prepare colors and hurt-levels
         allies = [f"{ally} ({ally.hurt_level})" for ally in allies]
         enemies = [f"{enemy} ({enemy.hurt_level})" for enemy in enemies]
 
         # the center column with the 'vs'
```

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/combat_turnbased.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/combat_turnbased.py`

 * *Files 3% similar despite different names*

```diff
@@ -246,19 +246,19 @@
             enemies = [comb for comb in self.combatants if comb != combatant]
         else:
             # otherwise, enemies/allies depend on who combatant is
             pcs = [comb for comb in self.combatants if inherits_from(comb, EvAdventureCharacter)]
             npcs = [comb for comb in self.combatants if comb not in pcs]
             if combatant in pcs:
                 # combatant is a PC, so NPCs are all enemies
-                allies = [comb for comb in pcs if comb != combatant]
+                allies = pcs
                 enemies = npcs
             else:
                 # combatant is an NPC, so PCs are all enemies
-                allies = [comb for comb in npcs if comb != combatant]
+                allies = npcs
                 enemies = pcs
         return allies, enemies
 
     def queue_action(self, combatant, action_dict):
         """
         Queue an action by adding the new actiondict.
 
@@ -341,15 +341,15 @@
 
         # check if one side won the battle
         if not self.combatants:
             # noone left in combat - maybe they killed each other or all fled
             surviving_combatant = None
             allies, enemies = (), ()
         else:
-            # grab a random survivor and check of they have any living enemies.
+            # grab a random survivor and check if they have any living enemies.
             surviving_combatant = random.choice(list(self.combatants.keys()))
             allies, enemies = self.get_sides(surviving_combatant)
 
         if not enemies:
             # if one way or another, there are no more enemies to fight
             still_standing = list_to_string(f"$You({comb.key})" for comb in allies)
             knocked_out = list_to_string(comb for comb in self.defeated_combatants if comb.hp > 0)
@@ -533,27 +533,14 @@
     """
     text = "Choose an ally to target."
     action_dict = kwargs["action_dict"]
 
     combathandler = _get_combathandler(caller)
     allies, _ = combathandler.get_sides(caller)
 
-    # can choose yourself
-    options = [
-        {
-            "desc": "Yourself",
-            "goto": (
-                _step_wizard,
-                {
-                    **kwargs,
-                    **{"action_dict": {**action_dict, **{"target": caller}}},
-                },
-            ),
-        }
-    ]
     options.extend(
         [
             {
                 "desc": target.get_display_name(caller),
                 "goto": (
                     _step_wizard,
                     {
@@ -575,27 +562,14 @@
     """
     text = "Choose an ally as a recipient."
     action_dict = kwargs["action_dict"]
 
     combathandler = _get_combathandler(caller)
     allies, _ = combathandler.get_sides(caller)
 
-    # can choose yourself
-    options = [
-        {
-            "desc": "Yourself",
-            "goto": (
-                _step_wizard,
-                {
-                    **kwargs,
-                    **{"action_dict": {**action_dict, **{"recipient": caller}}},
-                },
-            ),
-        }
-    ]
     options.extend(
         [
             {
                 "desc": target.get_display_name(caller),
                 "goto": (
                     _step_wizard,
                     {
```

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/combat_twitch.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/combat_twitch.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,19 +102,19 @@
             enemies = [comb for comb in combatants if comb != combatant]
         else:
             # otherwise, enemies/allies depend on who combatant is
             pcs = [comb for comb in combatants if inherits_from(comb, EvAdventureCharacter)]
             npcs = [comb for comb in combatants if comb not in pcs]
             if combatant in pcs:
                 # combatant is a PC, so NPCs are all enemies
-                allies = [comb for comb in pcs if comb != combatant]
+                allies = pcs
                 enemies = npcs
             else:
                 # combatant is an NPC, so PCs are all enemies
-                allies = [comb for comb in npcs if comb != combatant]
+                allies = npcs
                 enemies = pcs
         return allies, enemies
 
     def give_advantage(self, recipient, target):
         """
         Let a benefiter gain advantage against the target.
 
@@ -212,15 +212,14 @@
 
     def check_stop_combat(self):
         """
         Check if the combat is over.
         """
 
         allies, enemies = self.get_sides(self.obj)
-        allies.append(self.obj)
 
         location = self.obj.location
 
         # only keep combatants that are alive and still in the same room
         allies = [comb for comb in allies if comb.hp > 0 and comb.location == location]
         enemies = [comb for comb in enemies if comb.hp > 0 and comb.location == location]
```

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/commands.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/dungeon.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/dungeon.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/enums.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/enums.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/equipment.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/equipment.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,24 +89,22 @@
     def validate_slot_usage(self, obj):
         """
         Check if obj can fit in equipment, based on its size.
 
         Args:
             obj (EvAdventureObject): The object to add.
 
-        Raise:
-            EquipmentError: If there's not enough room.
-
         """
         if not inherits_from(obj, EvAdventureObject):
             raise EquipmentError(f"{obj.key} is not something that can be equipped.")
 
         size = obj.size
         max_slots = self.max_slots
         current_slot_usage = self.count_slots()
+
         if current_slot_usage + size > max_slots:
             slots_left = max_slots - current_slot_usage
             raise EquipmentError(
                 f"Equipment full ($int2str({slots_left}) slots "
                 f"remaining, {obj.key} needs $int2str({size}) "
                 f"$pluralize(slot, {size}))."
             )
```

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/npcs.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/npcs.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/objects.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/quests.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/quests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/random_tables.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/random_tables.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/rooms.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/rules.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/rules.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/shops.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/shops.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/mixins.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_characters.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_characters.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_chargen.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_combat.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_combat.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,26 +77,26 @@
             from_obj=None,
             mapping={"testchar": self.combatant, "testmonster": self.target},
         )
 
     def test_get_combat_summary(self):
         """Test combat summary"""
 
-        self.combathandler.get_sides = Mock(return_value=([], [self.target]))
+        self.combathandler.get_sides = Mock(return_value=([self.combatant], [self.target]))
 
         # as seen from one side
         result = str(self.combathandler.get_combat_summary(self.combatant))
 
         self.assertEqual(
             strip_ansi(result),
             " testchar (Perfect)  vs  testmonster (Perfect) ",
         )
 
         # as seen from other side
-        self.combathandler.get_sides = Mock(return_value=([], [self.combatant]))
+        self.combathandler.get_sides = Mock(return_value=([self.target], [self.combatant]))
         result = str(self.combathandler.get_combat_summary(self.target))
 
         self.assertEqual(
             strip_ansi(result),
             " testmonster (Perfect)  vs  testchar (Perfect) ",
         )
 
@@ -379,19 +379,19 @@
             attributes=(("is_idle", True),),
         )
         self.combathandler.add_combatant(combatant2)
         self.combathandler.add_combatant(target2)
 
         # allies to combatant
         allies, enemies = self.combathandler.get_sides(self.combatant)
-        self.assertEqual((allies, enemies), ([combatant2], [self.target, target2]))
+        self.assertEqual((allies, enemies), ([self.combatant, combatant2], [self.target, target2]))
 
         # allies to monster
         allies, enemies = self.combathandler.get_sides(self.target)
-        self.assertEqual((allies, enemies), ([target2], [self.combatant, combatant2]))
+        self.assertEqual((allies, enemies), ([self.target, target2], [self.combatant, combatant2]))
 
     def test_queue_and_execute_action(self):
         """Queue actions and execute"""
 
         hold = {"key": "hold"}
 
         self.combathandler.queue_action(self.combatant, hold)
@@ -547,15 +547,15 @@
             combat_twitch.EvAdventureCombatTwitchHandler.get_or_create_combathandler(
                 self.target, key="combathandler"
             )
         )
 
     def test_get_sides(self):
         sides = self.combatant_combathandler.get_sides(self.combatant)
-        self.assertEqual(sides, ([], [self.target]))
+        self.assertEqual(sides, ([self.combatant], [self.target]))
 
     def test_give_advantage(self):
         self.combatant_combathandler.give_advantage(self.combatant, self.target)
         self.assertTrue(self.combatant_combathandler.advantage_against[self.target])
 
     def test_give_disadvantage(self):
         self.combatant_combathandler.give_disadvantage(self.combatant, self.target)
@@ -608,15 +608,15 @@
             text=("Noone stands after the dust settles.", {}), from_obj=self.combatant
         )
         self.combatant_combathandler.stop_combat.assert_called()
 
         # only one side wiped out
         self.combatant.hp = 10
         self.target.hp = -1
-        self.combatant_combathandler.get_sides = Mock(return_value=([], []))
+        self.combatant_combathandler.get_sides = Mock(return_value=([self.combatant], []))
         self.combatant_combathandler.check_stop_combat()
         self.combatant.msg.assert_called_with(
             text=("The combat is over.", {}), from_obj=self.combatant
         )
 
     @patch("evennia.contrib.tutorials.evadventure.combat_twitch.unrepeat", new=Mock())
     @patch("evennia.contrib.tutorials.evadventure.combat_twitch.repeat", new=Mock())
```

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_commands.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_equipment.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_npcs.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_npcs.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_quests.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_rooms.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_rules.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/tests/test_utils.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/evadventure/utils.py` & `evennia-2.1.0/evennia/contrib/tutorials/evadventure/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/mirror/mirror.py` & `evennia-2.1.0/evennia/contrib/tutorials/mirror/mirror.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/red_button/README.md` & `evennia-2.1.0/evennia/contrib/tutorials/red_button/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/red_button/red_button.py` & `evennia-2.1.0/evennia/contrib/tutorials/red_button/red_button.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/talking_npc/README.md` & `evennia-2.1.0/evennia/contrib/tutorials/talking_npc/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/talking_npc/talking_npc.py` & `evennia-2.1.0/evennia/contrib/tutorials/talking_npc/talking_npc.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/README.md` & `evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/build.ev` & `evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/build.ev`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/intro_menu.py` & `evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/mob.py` & `evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/mob.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/objects.py` & `evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/rooms.py` & `evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/tutorials/tutorial_world/tests.py` & `evennia-2.1.0/evennia/contrib/tutorials/tutorial_world/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/auditing/README.md` & `evennia-2.1.0/evennia/contrib/utils/auditing/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/auditing/outputs.py` & `evennia-2.1.0/evennia/contrib/utils/auditing/outputs.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/auditing/server.py` & `evennia-2.1.0/evennia/contrib/utils/auditing/server.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/auditing/tests.py` & `evennia-2.1.0/evennia/contrib/utils/auditing/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/fieldfill/README.md` & `evennia-2.1.0/evennia/contrib/utils/fieldfill/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/fieldfill/fieldfill.py` & `evennia-2.1.0/evennia/contrib/utils/fieldfill/fieldfill.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/git_integration/README.md` & `evennia-2.1.0/evennia/contrib/utils/git_integration/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/git_integration/git_integration.py` & `evennia-2.1.0/evennia/contrib/utils/git_integration/git_integration.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/git_integration/tests.py` & `evennia-2.1.0/evennia/contrib/utils/git_integration/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/name_generator/README.md` & `evennia-2.1.0/evennia/contrib/utils/name_generator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/name_generator/btn_givennames.txt` & `evennia-2.1.0/evennia/contrib/utils/name_generator/btn_givennames.txt`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/name_generator/btn_surnames.txt` & `evennia-2.1.0/evennia/contrib/utils/name_generator/btn_surnames.txt`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/name_generator/namegen.py` & `evennia-2.1.0/evennia/contrib/utils/name_generator/namegen.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/name_generator/tests.py` & `evennia-2.1.0/evennia/contrib/utils/name_generator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/random_string_generator/README.md` & `evennia-2.1.0/evennia/contrib/utils/random_string_generator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/random_string_generator/random_string_generator.py` & `evennia-2.1.0/evennia/contrib/utils/random_string_generator/random_string_generator.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/random_string_generator/tests.py` & `evennia-2.1.0/evennia/contrib/utils/random_string_generator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/tree_select/README.md` & `evennia-2.1.0/evennia/contrib/utils/tree_select/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/tree_select/tests.py` & `evennia-2.1.0/evennia/contrib/utils/tree_select/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/contrib/utils/tree_select/tree_select.py` & `evennia-2.1.0/evennia/contrib/utils/tree_select/tree_select.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/README.md` & `evennia-2.1.0/evennia/game_template/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/commands/README.md` & `evennia-2.1.0/evennia/game_template/commands/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/commands/command.py` & `evennia-2.1.0/evennia/game_template/commands/command.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/commands/default_cmdsets.py` & `evennia-2.1.0/evennia/game_template/commands/default_cmdsets.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/gitignore` & `evennia-2.1.0/evennia/game_template/gitignore`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/README.md` & `evennia-2.1.0/evennia/game_template/server/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/at_initial_setup.py` & `evennia-2.1.0/evennia/game_template/server/conf/at_initial_setup.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/at_search.py` & `evennia-2.1.0/evennia/game_template/server/conf/at_search.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/at_server_startstop.py` & `evennia-2.1.0/evennia/game_template/server/conf/at_server_startstop.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/cmdparser.py` & `evennia-2.1.0/evennia/game_template/server/conf/cmdparser.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/connection_screens.py` & `evennia-2.1.0/evennia/game_template/server/conf/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/inlinefuncs.py` & `evennia-2.1.0/evennia/game_template/server/conf/inlinefuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/inputfuncs.py` & `evennia-2.1.0/evennia/game_template/server/conf/inputfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/lockfuncs.py` & `evennia-2.1.0/evennia/game_template/server/conf/lockfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/mssp.py` & `evennia-2.1.0/evennia/game_template/server/conf/mssp.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/portal_services_plugins.py` & `evennia-2.1.0/evennia/game_template/server/conf/portal_services_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/secret_settings.py` & `evennia-2.1.0/evennia/game_template/server/conf/secret_settings.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/server_services_plugins.py` & `evennia-2.1.0/evennia/game_template/server/conf/server_services_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/serversession.py` & `evennia-2.1.0/evennia/game_template/server/conf/serversession.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/settings.py` & `evennia-2.1.0/evennia/game_template/server/conf/settings.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/conf/web_plugins.py` & `evennia-2.1.0/evennia/game_template/server/conf/web_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/server/logs/README.md` & `evennia-2.1.0/evennia/game_template/server/logs/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/typeclasses/README.md` & `evennia-2.1.0/evennia/game_template/typeclasses/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/typeclasses/accounts.py` & `evennia-2.1.0/evennia/game_template/typeclasses/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/typeclasses/channels.py` & `evennia-2.1.0/evennia/game_template/typeclasses/channels.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/typeclasses/characters.py` & `evennia-2.1.0/evennia/game_template/typeclasses/characters.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/typeclasses/exits.py` & `evennia-2.1.0/evennia/game_template/typeclasses/exits.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/typeclasses/objects.py` & `evennia-2.1.0/evennia/game_template/typeclasses/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/typeclasses/rooms.py` & `evennia-2.1.0/evennia/game_template/typeclasses/rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/typeclasses/scripts.py` & `evennia-2.1.0/evennia/game_template/typeclasses/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/web/README.md` & `evennia-2.1.0/evennia/game_template/web/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/web/admin/urls.py` & `evennia-2.1.0/evennia/game_template/web/admin/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/web/static/README.md` & `evennia-2.1.0/evennia/game_template/web/static/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/web/templates/README.md` & `evennia-2.1.0/evennia/game_template/web/templates/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/web/urls.py` & `evennia-2.1.0/evennia/game_template/web/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/web/webclient/README.md` & `evennia-2.1.0/evennia/game_template/web/webclient/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/web/webclient/urls.py` & `evennia-2.1.0/evennia/game_template/web/webclient/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/web/website/README.md` & `evennia-2.1.0/evennia/game_template/web/website/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/world/batch_cmds.ev` & `evennia-2.1.0/evennia/game_template/world/batch_cmds.ev`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/world/help_entries.py` & `evennia-2.1.0/evennia/game_template/world/help_entries.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/game_template/world/prototypes.py` & `evennia-2.1.0/evennia/game_template/world/prototypes.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/help/filehelp.py` & `evennia-2.1.0/evennia/help/filehelp.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/help/manager.py` & `evennia-2.1.0/evennia/help/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/help/migrations/0001_initial.py` & `evennia-2.1.0/evennia/help/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/help/migrations/0002_auto_20170606_1731.py` & `evennia-2.1.0/evennia/help/migrations/0002_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/help/migrations/0003_auto_20190128_1820.py` & `evennia-2.1.0/evennia/help/migrations/0003_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/help/migrations/0004_auto_20210520_2137.py` & `evennia-2.1.0/evennia/help/migrations/0004_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/help/migrations/0005_auto_20210530_1818.py` & `evennia-2.1.0/evennia/help/migrations/0005_auto_20210530_1818.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/help/models.py` & `evennia-2.1.0/evennia/help/models.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/help/tests.py` & `evennia-2.1.0/evennia/help/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/help/utils.py` & `evennia-2.1.0/evennia/help/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/README` & `evennia-2.1.0/evennia/locale/README`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/de/LC_MESSAGES/django.mo` & `evennia-2.1.0/evennia/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/de/LC_MESSAGES/django.po` & `evennia-2.1.0/evennia/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/es/LC_MESSAGES/django.mo` & `evennia-2.1.0/evennia/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/es/LC_MESSAGES/django.po` & `evennia-2.1.0/evennia/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/fr/LC_MESSAGES/django.mo` & `evennia-2.1.0/evennia/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/fr/LC_MESSAGES/django.po` & `evennia-2.1.0/evennia/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/it/LC_MESSAGES/django.mo` & `evennia-2.1.0/evennia/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/it/LC_MESSAGES/django.po` & `evennia-2.1.0/evennia/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/ko/LC_MESSAGES/django.mo` & `evennia-2.1.0/evennia/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/ko/LC_MESSAGES/django.po` & `evennia-2.1.0/evennia/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/la/LC_MESSAGES/django.mo` & `evennia-2.1.0/evennia/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/la/LC_MESSAGES/django.po` & `evennia-2.1.0/evennia/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/pl/LC_MESSAGES/django.mo` & `evennia-2.1.0/evennia/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/pl/LC_MESSAGES/django.po` & `evennia-2.1.0/evennia/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/pt/LC_MESSAGES/django.mo` & `evennia-2.1.0/evennia/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/pt/LC_MESSAGES/django.po` & `evennia-2.1.0/evennia/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/ru/LC_MESSAGES/django.mo` & `evennia-2.1.0/evennia/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/ru/LC_MESSAGES/django.po` & `evennia-2.1.0/evennia/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/sv/LC_MESSAGES/django.mo` & `evennia-2.1.0/evennia/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/sv/LC_MESSAGES/django.po` & `evennia-2.1.0/evennia/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/zh/LC_MESSAGES/django.mo` & `evennia-2.1.0/evennia/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locale/zh/LC_MESSAGES/django.po` & `evennia-2.1.0/evennia/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locks/lockfuncs.py` & `evennia-2.1.0/evennia/locks/lockfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locks/lockhandler.py` & `evennia-2.1.0/evennia/locks/lockhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/locks/tests.py` & `evennia-2.1.0/evennia/locks/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/manager.py` & `evennia-2.1.0/evennia/objects/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/migrations/0001_initial.py` & `evennia-2.1.0/evennia/objects/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/migrations/0002_auto_20140917_0756.py` & `evennia-2.1.0/evennia/objects/migrations/0002_auto_20140917_0756.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py` & `evennia-2.1.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/migrations/0004_auto_20150118_1622.py` & `evennia-2.1.0/evennia/objects/migrations/0004_auto_20150118_1622.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/migrations/0006_auto_20170606_1731.py` & `evennia-2.1.0/evennia/objects/migrations/0006_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/migrations/0007_objectdb_db_account.py` & `evennia-2.1.0/evennia/objects/migrations/0007_objectdb_db_account.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/migrations/0008_auto_20170705_1736.py` & `evennia-2.1.0/evennia/objects/migrations/0008_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/migrations/0009_remove_objectdb_db_player.py` & `evennia-2.1.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/migrations/0010_auto_20190128_1820.py` & `evennia-2.1.0/evennia/objects/migrations/0010_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/migrations/0011_auto_20191025_0831.py` & `evennia-2.1.0/evennia/objects/migrations/0011_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py` & `evennia-2.1.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/models.py` & `evennia-2.1.0/evennia/objects/models.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/objects.py` & `evennia-2.1.0/evennia/objects/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/objects/tests.py` & `evennia-2.1.0/evennia/objects/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/prototypes/README.md` & `evennia-2.1.0/evennia/prototypes/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/prototypes/menus.py` & `evennia-2.1.0/evennia/prototypes/menus.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/prototypes/protfuncs.py` & `evennia-2.1.0/evennia/prototypes/protfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/prototypes/prototypes.py` & `evennia-2.1.0/evennia/prototypes/prototypes.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/prototypes/spawner.py` & `evennia-2.1.0/evennia/prototypes/spawner.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/prototypes/tests.py` & `evennia-2.1.0/evennia/prototypes/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/manager.py` & `evennia-2.1.0/evennia/scripts/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/migrations/0001_initial.py` & `evennia-2.1.0/evennia/scripts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/migrations/0002_auto_20150118_1625.py` & `evennia-2.1.0/evennia/scripts/migrations/0002_auto_20150118_1625.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py` & `evennia-2.1.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/migrations/0004_auto_20150306_1354.py` & `evennia-2.1.0/evennia/scripts/migrations/0004_auto_20150306_1354.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/migrations/0006_auto_20150310_2249.py` & `evennia-2.1.0/evennia/scripts/migrations/0006_auto_20150310_2249.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/migrations/0008_auto_20170606_1731.py` & `evennia-2.1.0/evennia/scripts/migrations/0008_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/migrations/0009_scriptdb_db_account.py` & `evennia-2.1.0/evennia/scripts/migrations/0009_scriptdb_db_account.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/migrations/0010_auto_20170705_1736.py` & `evennia-2.1.0/evennia/scripts/migrations/0010_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py` & `evennia-2.1.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/migrations/0012_auto_20190128_1820.py` & `evennia-2.1.0/evennia/scripts/migrations/0012_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/migrations/0013_auto_20191025_0831.py` & `evennia-2.1.0/evennia/scripts/migrations/0013_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/migrations/0014_auto_20210520_2137.py` & `evennia-2.1.0/evennia/scripts/migrations/0014_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/migrations/0015_convert_contrib_paths.py` & `evennia-2.1.0/evennia/scripts/migrations/0015_convert_contrib_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/models.py` & `evennia-2.1.0/evennia/scripts/models.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/monitorhandler.py` & `evennia-2.1.0/evennia/scripts/monitorhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/scripthandler.py` & `evennia-2.1.0/evennia/scripts/scripthandler.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/scripts.py` & `evennia-2.1.0/evennia/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/taskhandler.py` & `evennia-2.1.0/evennia/scripts/taskhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/tests.py` & `evennia-2.1.0/evennia/scripts/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/scripts/tickerhandler.py` & `evennia-2.1.0/evennia/scripts/tickerhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/amp_client.py` & `evennia-2.1.0/evennia/server/amp_client.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/connection_wizard.py` & `evennia-2.1.0/evennia/server/connection_wizard.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/deprecations.py` & `evennia-2.1.0/evennia/server/deprecations.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/evennia_launcher.py` & `evennia-2.1.0/evennia/server/evennia_launcher.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/game_index_client/README.md` & `evennia-2.1.0/evennia/server/game_index_client/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/game_index_client/client.py` & `evennia-2.1.0/evennia/server/game_index_client/client.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/game_index_client/service.py` & `evennia-2.1.0/evennia/server/game_index_client/service.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/initial_setup.py` & `evennia-2.1.0/evennia/server/initial_setup.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/inputfuncs.py` & `evennia-2.1.0/evennia/server/inputfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/manager.py` & `evennia-2.1.0/evennia/server/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/migrations/0001_initial.py` & `evennia-2.1.0/evennia/server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/migrations/0002_auto_20190128_2311.py` & `evennia-2.1.0/evennia/server/migrations/0002_auto_20190128_2311.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/models.py` & `evennia-2.1.0/evennia/server/models.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/amp.py` & `evennia-2.1.0/evennia/server/portal/amp.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/amp_server.py` & `evennia-2.1.0/evennia/server/portal/amp_server.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/discord.py` & `evennia-2.1.0/evennia/server/portal/discord.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/grapevine.py` & `evennia-2.1.0/evennia/server/portal/grapevine.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/irc.py` & `evennia-2.1.0/evennia/server/portal/irc.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/mccp.py` & `evennia-2.1.0/evennia/server/portal/mccp.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/mssp.py` & `evennia-2.1.0/evennia/server/portal/mssp.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/mxp.py` & `evennia-2.1.0/evennia/server/portal/mxp.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/naws.py` & `evennia-2.1.0/evennia/server/portal/naws.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/portal.py` & `evennia-2.1.0/evennia/server/portal/portal.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/portalsessionhandler.py` & `evennia-2.1.0/evennia/server/portal/portalsessionhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/rss.py` & `evennia-2.1.0/evennia/server/portal/rss.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/ssh.py` & `evennia-2.1.0/evennia/server/portal/ssh.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/ssl.py` & `evennia-2.1.0/evennia/server/portal/ssl.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/suppress_ga.py` & `evennia-2.1.0/evennia/server/portal/suppress_ga.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/telnet.py` & `evennia-2.1.0/evennia/server/portal/telnet.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/telnet_oob.py` & `evennia-2.1.0/evennia/server/portal/telnet_oob.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/telnet_ssl.py` & `evennia-2.1.0/evennia/server/portal/telnet_ssl.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,22 +32,15 @@
 _GAME_DIR = settings.GAME_DIR
 
 _PRIVATE_KEY_LENGTH = 2048
 _PRIVATE_KEY_FILE = os.path.join(_GAME_DIR, "server", "ssl.key")
 _PUBLIC_KEY_FILE = os.path.join(_GAME_DIR, "server", "ssl-public.key")
 _CERTIFICATE_FILE = os.path.join(_GAME_DIR, "server", "ssl.cert")
 _CERTIFICATE_EXPIRE = 365 * 24 * 60 * 60 * 20  # 20 years
-_CERTIFICATE_ISSUER = {
-    "C": "EV",
-    "ST": "Evennia",
-    "L": "Evennia",
-    "O": "Evennia Security",
-    "OU": "Evennia Department",
-    "CN": "evennia",
-}
+_CERTIFICATE_ISSUER = settings.SSL_CERTIFICATE_ISSUER
 
 # messages
 
 NO_AUTOGEN = f"""
 Evennia could not auto-generate the SSL private- and public keys ({{err}}).
 If this error persists, create them manually (using the tools for your OS). The files
 should be placed and named like this:
```

### Comparing `evennia-2.0.1/evennia/server/portal/tests.py` & `evennia-2.1.0/evennia/server/portal/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/ttype.py` & `evennia-2.1.0/evennia/server/portal/ttype.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/webclient.py` & `evennia-2.1.0/evennia/server/portal/webclient.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/portal/webclient_ajax.py` & `evennia-2.1.0/evennia/server/portal/webclient_ajax.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/profiling/dummyrunner.py` & `evennia-2.1.0/evennia/server/profiling/dummyrunner.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/profiling/dummyrunner_settings.py` & `evennia-2.1.0/evennia/server/profiling/dummyrunner_settings.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/profiling/memplot.py` & `evennia-2.1.0/evennia/server/profiling/memplot.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/profiling/settings_mixin.py` & `evennia-2.1.0/evennia/server/profiling/settings_mixin.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/profiling/test_queries.py` & `evennia-2.1.0/evennia/server/profiling/test_queries.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/profiling/tests.py` & `evennia-2.1.0/evennia/server/profiling/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/profiling/timetrace.py` & `evennia-2.1.0/evennia/server/profiling/timetrace.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/server.py` & `evennia-2.1.0/evennia/server/server.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/serversession.py` & `evennia-2.1.0/evennia/server/serversession.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/session.py` & `evennia-2.1.0/evennia/server/session.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/sessionhandler.py` & `evennia-2.1.0/evennia/server/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/signals.py` & `evennia-2.1.0/evennia/server/signals.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/tests/test_amp_connection.py` & `evennia-2.1.0/evennia/server/tests/test_amp_connection.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/tests/test_initial_setup.py` & `evennia-2.1.0/evennia/server/tests/test_initial_setup.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/tests/test_launcher.py` & `evennia-2.1.0/evennia/server/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/tests/test_misc.py` & `evennia-2.1.0/evennia/server/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/tests/test_server.py` & `evennia-2.1.0/evennia/server/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/tests/testrunner.py` & `evennia-2.1.0/evennia/server/tests/testrunner.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/throttle.py` & `evennia-2.1.0/evennia/server/throttle.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/validators.py` & `evennia-2.1.0/evennia/server/validators.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/server/webserver.py` & `evennia-2.1.0/evennia/server/webserver.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/settings_default.py` & `evennia-2.1.0/evennia/settings_default.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,24 @@
 TELNET_INTERFACES = ["0.0.0.0"]
 # Activate Telnet+SSL protocol (SecureSocketLibrary) for supporting clients
 SSL_ENABLED = False
 # Ports to use for Telnet+SSL
 SSL_PORTS = [4003]
 # Telnet+SSL Interface addresses to listen to. If 0.0.0.0, listen to all. Use :: for IPv6.
 SSL_INTERFACES = ["0.0.0.0"]
+# Telnet+SSL certificate issuers. Don't change unless you have issues, e.g. CN may need to be
+# changed to your server's hostname.
+SSL_CERTIFICATE_ISSUER = {
+    "C": "EV",
+    "ST": "Evennia",
+    "L": "Evennia",
+    "O": "Evennia Security",
+    "OU": "Evennia Department",
+    "CN": "evennia",
+}
 # OOB (out-of-band) telnet communication allows Evennia to communicate
 # special commands and data with enabled Telnet clients. This is used
 # to create custom client interfaces over a telnet connection. To make
 # full use of OOB, you need to prepare functions to handle the data
 # server-side (see INPUT_FUNC_MODULES). TELNET_ENABLED is required for this
 # to work.
 TELNET_OOB_ENABLED = False
```

### Comparing `evennia-2.0.1/evennia/typeclasses/attributes.py` & `evennia-2.1.0/evennia/typeclasses/attributes.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/managers.py` & `evennia-2.1.0/evennia/typeclasses/managers.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0001_initial.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0002_auto_20150109_0913.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0004_auto_20151101_1759.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0005_auto_20160625_1812.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0010_delete_old_player_tables.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0011_auto_20190128_1820.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0013_auto_20191015_1922.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0014_alter_tag_db_category.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py` & `evennia-2.1.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/models.py` & `evennia-2.1.0/evennia/typeclasses/models.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/tags.py` & `evennia-2.1.0/evennia/typeclasses/tags.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/typeclasses/tests.py` & `evennia-2.1.0/evennia/typeclasses/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/ansi.py` & `evennia-2.1.0/evennia/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/batchprocessors.py` & `evennia-2.1.0/evennia/utils/batchprocessors.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/containers.py` & `evennia-2.1.0/evennia/utils/containers.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/create.py` & `evennia-2.1.0/evennia/utils/create.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/dbserialize.py` & `evennia-2.1.0/evennia/utils/dbserialize.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/eveditor.py` & `evennia-2.1.0/evennia/utils/eveditor.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/evennia-mode.el` & `evennia-2.1.0/evennia/utils/evennia-mode.el`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/evform.py` & `evennia-2.1.0/evennia/utils/evform.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/evmenu.py` & `evennia-2.1.0/evennia/utils/evmenu.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/evmore.py` & `evennia-2.1.0/evennia/utils/evmore.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/evtable.py` & `evennia-2.1.0/evennia/utils/evtable.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/funcparser.py` & `evennia-2.1.0/evennia/utils/funcparser.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/gametime.py` & `evennia-2.1.0/evennia/utils/gametime.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/idmapper/LICENSE.md` & `evennia-2.1.0/evennia/utils/idmapper/LICENSE.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/idmapper/README_evennia.md` & `evennia-2.1.0/evennia/utils/idmapper/README_evennia.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/idmapper/README_orig.rst` & `evennia-2.1.0/evennia/utils/idmapper/README_orig.rst`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/idmapper/manager.py` & `evennia-2.1.0/evennia/utils/idmapper/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/idmapper/models.py` & `evennia-2.1.0/evennia/utils/idmapper/models.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/idmapper/tests.py` & `evennia-2.1.0/evennia/utils/idmapper/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/logger.py` & `evennia-2.1.0/evennia/utils/logger.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/optionclasses.py` & `evennia-2.1.0/evennia/utils/optionclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/optionhandler.py` & `evennia-2.1.0/evennia/utils/optionhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/picklefield.py` & `evennia-2.1.0/evennia/utils/picklefield.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/search.py` & `evennia-2.1.0/evennia/utils/search.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/test_resources.py` & `evennia-2.1.0/evennia/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/data/evform_example.py` & `evennia-2.1.0/evennia/utils/tests/data/evform_example.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/data/evmenu_example.py` & `evennia-2.1.0/evennia/utils/tests/data/evmenu_example.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_ansi.py` & `evennia-2.1.0/evennia/utils/tests/test_ansi.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_batchprocessors.py` & `evennia-2.1.0/evennia/utils/tests/test_batchprocessors.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_containers.py` & `evennia-2.1.0/evennia/utils/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_create_functions.py` & `evennia-2.1.0/evennia/utils/tests/test_create_functions.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_dbserialize.py` & `evennia-2.1.0/evennia/utils/tests/test_dbserialize.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_eveditor.py` & `evennia-2.1.0/evennia/utils/tests/test_eveditor.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_evform.py` & `evennia-2.1.0/evennia/utils/tests/test_evform.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_evmenu.py` & `evennia-2.1.0/evennia/utils/tests/test_evmenu.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_evtable.py` & `evennia-2.1.0/evennia/utils/tests/test_evtable.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_funcparser.py` & `evennia-2.1.0/evennia/utils/tests/test_funcparser.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_gametime.py` & `evennia-2.1.0/evennia/utils/tests/test_gametime.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_search.py` & `evennia-2.1.0/evennia/utils/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_tagparsing.py` & `evennia-2.1.0/evennia/utils/tests/test_tagparsing.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_text2html.py` & `evennia-2.1.0/evennia/utils/tests/test_text2html.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_utils.py` & `evennia-2.1.0/evennia/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/tests/test_validatorfuncs.py` & `evennia-2.1.0/evennia/utils/tests/test_validatorfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/text2html.py` & `evennia-2.1.0/evennia/utils/text2html.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/utils.py` & `evennia-2.1.0/evennia/utils/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/validatorfuncs.py` & `evennia-2.1.0/evennia/utils/validatorfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/verb_conjugation/LICENSE.txt` & `evennia-2.1.0/evennia/utils/verb_conjugation/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/verb_conjugation/conjugate.py` & `evennia-2.1.0/evennia/utils/verb_conjugation/conjugate.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/verb_conjugation/pronouns.py` & `evennia-2.1.0/evennia/utils/verb_conjugation/pronouns.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/verb_conjugation/tests.py` & `evennia-2.1.0/evennia/utils/verb_conjugation/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/utils/verb_conjugation/verbs.txt` & `evennia-2.1.0/evennia/utils/verb_conjugation/verbs.txt`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/README.md` & `evennia-2.1.0/evennia/web/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/admin/accounts.py` & `evennia-2.1.0/evennia/web/admin/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/admin/attributes.py` & `evennia-2.1.0/evennia/web/admin/attributes.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/admin/comms.py` & `evennia-2.1.0/evennia/web/admin/comms.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/admin/frontpage.py` & `evennia-2.1.0/evennia/web/admin/frontpage.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/admin/help.py` & `evennia-2.1.0/evennia/web/admin/help.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/admin/objects.py` & `evennia-2.1.0/evennia/web/admin/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/admin/scripts.py` & `evennia-2.1.0/evennia/web/admin/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/admin/tags.py` & `evennia-2.1.0/evennia/web/admin/tags.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/admin/urls.py` & `evennia-2.1.0/evennia/web/admin/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/admin/utils.py` & `evennia-2.1.0/evennia/web/admin/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/api/README.md` & `evennia-2.1.0/evennia/web/api/README.md`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/api/filters.py` & `evennia-2.1.0/evennia/web/api/filters.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/api/permissions.py` & `evennia-2.1.0/evennia/web/api/permissions.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/api/serializers.py` & `evennia-2.1.0/evennia/web/api/serializers.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/api/tests.py` & `evennia-2.1.0/evennia/web/api/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/api/urls.py` & `evennia-2.1.0/evennia/web/api/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/api/views.py` & `evennia-2.1.0/evennia/web/api/views.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/rest_framework/images/favicon.ico` & `evennia-2.1.0/evennia/web/static/rest_framework/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/css/goldenlayout.css` & `evennia-2.1.0/evennia/web/static/webclient/css/goldenlayout.css`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/css/webclient.css` & `evennia-2.1.0/evennia/web/static/webclient/css/webclient.css`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff` & `evennia-2.1.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/evennia.js` & `evennia-2.1.0/evennia/web/static/webclient/js/evennia.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/clienthelp.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/clienthelp.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/default_in.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/default_in.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/default_out.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/default_out.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/font.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/font.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/goldenlayout.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/goldenlayout.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/history.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/history.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/hotbuttons.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/hotbuttons.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/html.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/html.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/iframe.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/iframe.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/message_routing.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/message_routing.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/multimedia.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/multimedia.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/notifications.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/notifications.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/oob.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/oob.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/options2.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/options2.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/popups.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/popups.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/plugins/text2html.js` & `evennia-2.1.0/evennia/web/static/webclient/js/plugins/text2html.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/js/webclient_gui.js` & `evennia-2.1.0/evennia/web/static/webclient/js/webclient_gui.js`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/webclient/media/notification.wav` & `evennia-2.1.0/evennia/web/static/webclient/media/notification.wav`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/website/css/website.css` & `evennia-2.1.0/evennia/web/static/website/css/website.css`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/website/images/evennia_logo.png` & `evennia-2.1.0/evennia/web/static/website/images/evennia_logo.png`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/website/images/evennia_logo_festive.png` & `evennia-2.1.0/evennia/web/static/website/images/evennia_logo_festive.png`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/static/website/images/favicon.ico` & `evennia-2.1.0/evennia/web/static/website/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/admin/app_list.html` & `evennia-2.1.0/evennia/web/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/admin/frontpage.html` & `evennia-2.1.0/evennia/web/templates/admin/frontpage.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/rest_framework/api.html` & `evennia-2.1.0/evennia/web/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/webclient/base.html` & `evennia-2.1.0/evennia/web/templates/webclient/base.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/webclient/webclient.html` & `evennia-2.1.0/evennia/web/templates/webclient/webclient.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/500.html` & `evennia-2.1.0/evennia/web/templates/website/500.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/_menu.html` & `evennia-2.1.0/evennia/web/templates/website/_menu.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/base.html` & `evennia-2.1.0/evennia/web/templates/website/base.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/channel_detail.html` & `evennia-2.1.0/evennia/web/templates/website/channel_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/channel_list.html` & `evennia-2.1.0/evennia/web/templates/website/channel_list.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/character_form.html` & `evennia-2.1.0/evennia/web/templates/website/character_form.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/character_list.html` & `evennia-2.1.0/evennia/web/templates/website/character_list.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/character_manage_list.html` & `evennia-2.1.0/evennia/web/templates/website/character_manage_list.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/generic_form.html` & `evennia-2.1.0/evennia/web/templates/website/generic_form.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/help_detail.html` & `evennia-2.1.0/evennia/web/templates/website/help_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/help_list.html` & `evennia-2.1.0/evennia/web/templates/website/help_list.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/index.html` & `evennia-2.1.0/evennia/web/templates/website/index.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/object_confirm_delete.html` & `evennia-2.1.0/evennia/web/templates/website/object_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/object_detail.html` & `evennia-2.1.0/evennia/web/templates/website/object_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/object_list.html` & `evennia-2.1.0/evennia/web/templates/website/object_list.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/pagination.html` & `evennia-2.1.0/evennia/web/templates/website/pagination.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/registration/logged_out.html` & `evennia-2.1.0/evennia/web/templates/website/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/registration/login.html` & `evennia-2.1.0/evennia/web/templates/website/registration/login.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/registration/password_change_done.html` & `evennia-2.1.0/evennia/web/templates/website/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/registration/password_change_form.html` & `evennia-2.1.0/evennia/web/templates/website/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/registration/password_reset_complete.html` & `evennia-2.1.0/evennia/web/templates/website/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/registration/password_reset_confirm.html` & `evennia-2.1.0/evennia/web/templates/website/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/registration/password_reset_done.html` & `evennia-2.1.0/evennia/web/templates/website/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/registration/password_reset_email.html` & `evennia-2.1.0/evennia/web/templates/website/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/registration/password_reset_form.html` & `evennia-2.1.0/evennia/web/templates/website/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/registration/register.html` & `evennia-2.1.0/evennia/web/templates/website/registration/register.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templates/website/tbi.html` & `evennia-2.1.0/evennia/web/templates/website/tbi.html`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/templatetags/addclass.py` & `evennia-2.1.0/evennia/web/templatetags/addclass.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/urls.py` & `evennia-2.1.0/evennia/web/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/utils/adminsite.py` & `evennia-2.1.0/evennia/web/utils/adminsite.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/utils/apache_wsgi.conf` & `evennia-2.1.0/evennia/web/utils/apache_wsgi.conf`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/utils/backends.py` & `evennia-2.1.0/evennia/web/utils/backends.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/utils/evennia_modpy_apache.conf` & `evennia-2.1.0/evennia/web/utils/evennia_modpy_apache.conf`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/utils/evennia_wsgi_apache.conf` & `evennia-2.1.0/evennia/web/utils/evennia_wsgi_apache.conf`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/utils/general_context.py` & `evennia-2.1.0/evennia/web/utils/general_context.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/utils/middleware.py` & `evennia-2.1.0/evennia/web/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/utils/tests.py` & `evennia-2.1.0/evennia/web/utils/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/webclient/views.py` & `evennia-2.1.0/evennia/web/webclient/views.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/website/forms.py` & `evennia-2.1.0/evennia/web/website/forms.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/website/tests.py` & `evennia-2.1.0/evennia/web/website/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/website/urls.py` & `evennia-2.1.0/evennia/web/website/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/website/views/accounts.py` & `evennia-2.1.0/evennia/web/website/views/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/website/views/channels.py` & `evennia-2.1.0/evennia/web/website/views/channels.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/website/views/characters.py` & `evennia-2.1.0/evennia/web/website/views/characters.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/website/views/help.py` & `evennia-2.1.0/evennia/web/website/views/help.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/website/views/index.py` & `evennia-2.1.0/evennia/web/website/views/index.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/website/views/mixins.py` & `evennia-2.1.0/evennia/web/website/views/mixins.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia/web/website/views/objects.py` & `evennia-2.1.0/evennia/web/website/views/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia.egg-info/PKG-INFO` & `evennia-2.1.0/evennia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evennia
-Version: 2.0.1
+Version: 2.1.0
 Summary: A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc).
 Maintainer-email: Griatch <griatch@gmail.com>
 License: BSD
 Project-URL: Homepage, https://www.evennia.com
 Project-URL: Github, https://github.com/evennia/evennia
 Project-URL: Documentation, https://www.evennia.com/docs/latest/index.html
 Project-URL: Live Demo, https://demo.evennia.com/
```

### Comparing `evennia-2.0.1/evennia.egg-info/SOURCES.txt` & `evennia-2.1.0/evennia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/evennia.egg-info/requires.txt` & `evennia-2.1.0/evennia.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `evennia-2.0.1/pyproject.toml` & `evennia-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "evennia"
-version = "2.0.1"
+version = "2.1.0"
 maintainers = [{ name = "Griatch", email = "griatch@gmail.com" }]
 description = "A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc)."
 requires-python = ">=3.10"
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { text = "BSD" }
 keywords = [
   "MUD",
```

### Comparing `evennia-2.0.1/setup.py` & `evennia-2.1.0/setup.py`

 * *Files identical despite different names*

