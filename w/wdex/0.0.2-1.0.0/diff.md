# Comparing `tmp/wdex-0.0.2.tar.gz` & `tmp/wdex-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wdex-0.0.2.tar", last modified: Fri Jul 14 11:04:33 2023, max compression
+gzip compressed data, was "wdex-1.0.0.tar", last modified: Fri Jul 14 11:11:30 2023, max compression
```

## Comparing `wdex-0.0.2.tar` & `wdex-1.0.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:33.777391 wdex-0.0.2/
--rw-rw-rw-   0        0        0      464 2023-07-14 11:04:33.772423 wdex-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-14 11:04:33.778384 wdex-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      796 2023-07-14 11:04:11.000000 wdex-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:33.192317 wdex-0.0.2/wdex/
--rw-rw-rw-   0        0        0      281 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/__init__.py
--rw-rw-rw-   0        0        0     8301 2023-05-01 08:09:38.000000 wdex-0.0.2/wdex/__main__.py
--rw-rw-rw-   0        0        0    10151 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/adb_handler.py
--rw-rw-rw-   0        0        0    13745 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/config_manager.py
--rw-rw-rw-   0        0        0     1501 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/csv_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:33.251918 wdex-0.0.2/wdex/edits/
--rw-rw-rw-   0        0        0       67 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:33.318470 wdex-0.0.2/wdex/edits/basic/
--rw-rw-rw-   0        0        0      122 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/basic/__init__.py
--rw-rw-rw-   0        0        0     8690 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/basic/basic_items.py
--rw-rw-rw-   0        0        0     1490 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/basic/catfruit.py
--rw-rw-rw-   0        0        0     1931 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/basic/catseyes.py
--rw-rw-rw-   0        0        0     1647 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/basic/ototo_base_mats.py
--rw-rw-rw-   0        0        0     3984 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/basic/talent_orbs.py
--rw-rw-rw-   0        0        0    16533 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/basic/talent_orbs_new.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:33.495284 wdex-0.0.2/wdex/edits/cats/
--rw-rw-rw-   0        0        0      179 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/cats/__init__.py
--rw-rw-rw-   0        0        0     8978 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/cats/cat_helper.py
--rw-rw-rw-   0        0        0    11121 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/cats/cat_id_selector.py
--rw-rw-rw-   0        0        0     3249 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/cats/chara_drop.py
--rw-rw-rw-   0        0        0     1068 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/cats/clear_cat_guide.py
--rw-rw-rw-   0        0        0     2844 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/cats/evolve_cats.py
--rw-rw-rw-   0        0        0     1260 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/cats/get_remove_cats.py
--rw-rw-rw-   0        0        0     7936 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/cats/talents.py
--rw-rw-rw-   0        0        0     1900 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/cats/upgrade_blue.py
--rw-rw-rw-   0        0        0     4428 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/cats/upgrade_cats.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:33.533031 wdex-0.0.2/wdex/edits/gamototo/
--rw-rw-rw-   0        0        0       66 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/gamototo/__init__.py
--rw-rw-rw-   0        0        0      309 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/gamototo/fix_gamatoto.py
--rw-rw-rw-   0        0        0     2794 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/gamototo/gamatoto_xp.py
--rw-rw-rw-   0        0        0     3393 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/gamototo/helpers.py
--rw-rw-rw-   0        0        0     4137 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/gamototo/ototo_cat_cannon.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:33.636339 wdex-0.0.2/wdex/edits/levels/
--rw-rw-rw-   0        0        0      313 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/__init__.py
--rw-rw-rw-   0        0        0     1035 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/aku.py
--rw-rw-rw-   0        0        0      491 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/allow_filibuster_clearing.py
--rw-rw-rw-   0        0        0      790 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/behemoth_culling.py
--rw-rw-rw-   0        0        0      646 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/clear_tutorial.py
--rw-rw-rw-   0        0        0     1121 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/enigma_stages.py
--rw-rw-rw-   0        0        0     6307 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/event_stages.py
--rw-rw-rw-   0        0        0     1873 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/gauntlet.py
--rw-rw-rw-   0        0        0     1027 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/itf_timed_scores.py
--rw-rw-rw-   0        0        0     1469 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/legend_quest.py
--rw-rw-rw-   0        0        0     4408 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/main_story.py
--rw-rw-rw-   0        0        0     2323 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/outbreaks.py
--rw-rw-rw-   0        0        0     3031 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/story_level_id_selector.py
--rw-rw-rw-   0        0        0     1175 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/towers.py
--rw-rw-rw-   0        0        0     8458 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/treasures.py
--rw-rw-rw-   0        0        0     1043 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/uncanny.py
--rw-rw-rw-   0        0        0      784 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/levels/unlock_aku_realm.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:33.725738 wdex-0.0.2/wdex/edits/other/
--rw-rw-rw-   0        0        0      276 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/__init__.py
--rw-rw-rw-   0        0        0     3878 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/cat_shrine.py
--rw-rw-rw-   0        0        0     1093 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/claim_user_rank_rewards.py
--rw-rw-rw-   0        0        0     1054 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/create_new_account.py
--rw-rw-rw-   0        0        0     2187 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/fix_elsewhere.py
--rw-rw-rw-   0        0        0      659 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/fix_time_issues.py
--rw-rw-rw-   0        0        0     3445 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/get_gold_pass.py
--rw-rw-rw-   0        0        0     7067 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/meow_medals.py
--rw-rw-rw-   0        0        0     4354 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/missions.py
--rw-rw-rw-   0        0        0      975 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/play_time.py
--rw-rw-rw-   0        0        0     4568 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/scheme_item.py
--rw-rw-rw-   0        0        0     1612 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/trade_progress.py
--rw-rw-rw-   0        0        0     1284 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/unlock_enemy_guide.py
--rw-rw-rw-   0        0        0      326 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/other/unlock_equip_menu.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:33.766465 wdex-0.0.2/wdex/edits/save_management/
--rw-rw-rw-   0        0        0       56 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/save_management/__init__.py
--rw-rw-rw-   0        0        0     1273 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/save_management/convert.py
--rw-rw-rw-   0        0        0     2578 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/save_management/load.py
--rw-rw-rw-   0        0        0      644 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/save_management/other.py
--rw-rw-rw-   0        0        0     2049 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/edits/save_management/save.py
--rw-rw-rw-   0        0        0     1635 2023-07-14 10:23:05.000000 wdex-0.0.2/wdex/edits/save_management/server_upload.py
--rw-rw-rw-   0        0        0    12118 2023-04-27 11:52:06.000000 wdex-0.0.2/wdex/feature_handler.py
--rw-rw-rw-   0        0        0     4822 2023-04-26 22:37:34.000000 wdex-0.0.2/wdex/game_data_getter.py
--rw-rw-rw-   0        0        0    22881 2023-07-14 10:58:00.000000 wdex-0.0.2/wdex/helper.py
--rw-rw-rw-   0        0        0     7075 2023-04-27 12:18:12.000000 wdex-0.0.2/wdex/item.py
--rw-rw-rw-   0        0        0     3505 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/locale_handler.py
--rw-rw-rw-   0        0        0     1269 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/managed_item.py
--rw-rw-rw-   0        0        0    66964 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/parse_save.py
--rw-rw-rw-   0        0        0     1301 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/patcher.py
--rw-rw-rw-   0        0        0     2415 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/root_handler.py
--rw-rw-rw-   0        0        0    53791 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/serialise_save.py
--rw-rw-rw-   0        0        0    24729 2023-07-14 10:24:52.000000 wdex-0.0.2/wdex/server_handler.py
--rw-rw-rw-   0        0        0     3717 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/tracker.py
--rw-rw-rw-   0        0        0     2855 2023-07-14 10:59:45.000000 wdex-0.0.2/wdex/updater.py
--rw-rw-rw-   0        0        0     8297 2023-03-22 22:39:32.000000 wdex-0.0.2/wdex/user_input_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-14 11:04:33.247944 wdex-0.0.2/wdex.egg-info/
--rw-rw-rw-   0        0        0      464 2023-07-14 11:04:32.000000 wdex-0.0.2/wdex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2578 2023-07-14 11:04:32.000000 wdex-0.0.2/wdex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 11:04:32.000000 wdex-0.0.2/wdex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-14 11:04:32.000000 wdex-0.0.2/wdex.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       50 2023-07-14 11:04:32.000000 wdex-0.0.2/wdex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-14 11:04:32.000000 wdex-0.0.2/wdex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 11:11:30.231497 wdex-1.0.0/
+-rw-rw-rw-   0        0        0      464 2023-07-14 11:11:30.229511 wdex-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-14 11:11:30.232492 wdex-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      796 2023-07-14 11:11:17.000000 wdex-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:11:29.871912 wdex-1.0.0/wdex/
+-rw-rw-rw-   0        0        0      281 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/__init__.py
+-rw-rw-rw-   0        0        0     8301 2023-05-01 08:09:38.000000 wdex-1.0.0/wdex/__main__.py
+-rw-rw-rw-   0        0        0    10151 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/adb_handler.py
+-rw-rw-rw-   0        0        0    13745 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/config_manager.py
+-rw-rw-rw-   0        0        0     1501 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/csv_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:11:29.920585 wdex-1.0.0/wdex/edits/
+-rw-rw-rw-   0        0        0       67 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:11:29.952373 wdex-1.0.0/wdex/edits/basic/
+-rw-rw-rw-   0        0        0      122 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/basic/__init__.py
+-rw-rw-rw-   0        0        0     8690 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/basic/basic_items.py
+-rw-rw-rw-   0        0        0     1490 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/basic/catfruit.py
+-rw-rw-rw-   0        0        0     1931 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/basic/catseyes.py
+-rw-rw-rw-   0        0        0     1647 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0        0        0     3984 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/basic/talent_orbs.py
+-rw-rw-rw-   0        0        0    16533 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/basic/talent_orbs_new.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:11:29.994091 wdex-1.0.0/wdex/edits/cats/
+-rw-rw-rw-   0        0        0      179 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/cats/__init__.py
+-rw-rw-rw-   0        0        0     8978 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/cats/cat_helper.py
+-rw-rw-rw-   0        0        0    11121 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0        0        0     3249 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/cats/chara_drop.py
+-rw-rw-rw-   0        0        0     1068 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0        0        0     2844 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/cats/evolve_cats.py
+-rw-rw-rw-   0        0        0     1260 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0        0        0     7936 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/cats/talents.py
+-rw-rw-rw-   0        0        0     1900 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0        0        0     4428 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/cats/upgrade_cats.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:11:30.013959 wdex-1.0.0/wdex/edits/gamototo/
+-rw-rw-rw-   0        0        0       66 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/gamototo/__init__.py
+-rw-rw-rw-   0        0        0      309 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0        0        0     2794 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0        0        0     3393 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/gamototo/helpers.py
+-rw-rw-rw-   0        0        0     4137 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/gamototo/ototo_cat_cannon.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:11:30.096407 wdex-1.0.0/wdex/edits/levels/
+-rw-rw-rw-   0        0        0      313 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/__init__.py
+-rw-rw-rw-   0        0        0     1035 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/aku.py
+-rw-rw-rw-   0        0        0      491 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0        0        0      790 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0        0        0      646 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0        0        0     1121 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/enigma_stages.py
+-rw-rw-rw-   0        0        0     6307 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/event_stages.py
+-rw-rw-rw-   0        0        0     1873 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/gauntlet.py
+-rw-rw-rw-   0        0        0     1027 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0        0        0     1469 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/legend_quest.py
+-rw-rw-rw-   0        0        0     4408 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/main_story.py
+-rw-rw-rw-   0        0        0     2323 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/outbreaks.py
+-rw-rw-rw-   0        0        0     3031 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0        0        0     1175 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/towers.py
+-rw-rw-rw-   0        0        0     8458 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/treasures.py
+-rw-rw-rw-   0        0        0     1043 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/uncanny.py
+-rw-rw-rw-   0        0        0      784 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/levels/unlock_aku_realm.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:11:30.190771 wdex-1.0.0/wdex/edits/other/
+-rw-rw-rw-   0        0        0      276 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/__init__.py
+-rw-rw-rw-   0        0        0     3878 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/cat_shrine.py
+-rw-rw-rw-   0        0        0     1093 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0        0        0     1054 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/create_new_account.py
+-rw-rw-rw-   0        0        0     2187 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0        0        0      659 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/fix_time_issues.py
+-rw-rw-rw-   0        0        0     3445 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/get_gold_pass.py
+-rw-rw-rw-   0        0        0     7067 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/meow_medals.py
+-rw-rw-rw-   0        0        0     4354 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/missions.py
+-rw-rw-rw-   0        0        0      975 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/play_time.py
+-rw-rw-rw-   0        0        0     4568 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/scheme_item.py
+-rw-rw-rw-   0        0        0     1612 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/trade_progress.py
+-rw-rw-rw-   0        0        0     1284 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0        0        0      326 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/other/unlock_equip_menu.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:11:30.224546 wdex-1.0.0/wdex/edits/save_management/
+-rw-rw-rw-   0        0        0       56 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/save_management/__init__.py
+-rw-rw-rw-   0        0        0     1273 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/save_management/convert.py
+-rw-rw-rw-   0        0        0     2578 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/save_management/load.py
+-rw-rw-rw-   0        0        0      644 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/save_management/other.py
+-rw-rw-rw-   0        0        0     2049 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/edits/save_management/save.py
+-rw-rw-rw-   0        0        0     1635 2023-07-14 10:23:05.000000 wdex-1.0.0/wdex/edits/save_management/server_upload.py
+-rw-rw-rw-   0        0        0    12118 2023-04-27 11:52:06.000000 wdex-1.0.0/wdex/feature_handler.py
+-rw-rw-rw-   0        0        0     4822 2023-04-26 22:37:34.000000 wdex-1.0.0/wdex/game_data_getter.py
+-rw-rw-rw-   0        0        0    22881 2023-07-14 10:58:00.000000 wdex-1.0.0/wdex/helper.py
+-rw-rw-rw-   0        0        0     7075 2023-04-27 12:18:12.000000 wdex-1.0.0/wdex/item.py
+-rw-rw-rw-   0        0        0     3505 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/locale_handler.py
+-rw-rw-rw-   0        0        0     1269 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/managed_item.py
+-rw-rw-rw-   0        0        0    66964 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/parse_save.py
+-rw-rw-rw-   0        0        0     1301 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/patcher.py
+-rw-rw-rw-   0        0        0     2415 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/root_handler.py
+-rw-rw-rw-   0        0        0    53791 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/serialise_save.py
+-rw-rw-rw-   0        0        0    24729 2023-07-14 10:24:52.000000 wdex-1.0.0/wdex/server_handler.py
+-rw-rw-rw-   0        0        0     3717 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/tracker.py
+-rw-rw-rw-   0        0        0     2815 2023-07-14 11:10:55.000000 wdex-1.0.0/wdex/updater.py
+-rw-rw-rw-   0        0        0     8297 2023-03-22 22:39:32.000000 wdex-1.0.0/wdex/user_input_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:11:29.916612 wdex-1.0.0/wdex.egg-info/
+-rw-rw-rw-   0        0        0      464 2023-07-14 11:11:29.000000 wdex-1.0.0/wdex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2578 2023-07-14 11:11:29.000000 wdex-1.0.0/wdex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 11:11:29.000000 wdex-1.0.0/wdex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 11:11:29.000000 wdex-1.0.0/wdex.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       50 2023-07-14 11:11:29.000000 wdex-1.0.0/wdex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-14 11:11:29.000000 wdex-1.0.0/wdex.egg-info/top_level.txt
```

### Comparing `wdex-0.0.2/setup.py` & `wdex-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wdex',
-    version='0.0.2',
+    version='1.0.0',
     description='This is a project developed by Serem for development purposes',
     author='serem',
     author_email='gangh9230@gmail.com',
     url='https://github.com/hayul0629/wdex',
     install_requires=[
         "colored==1.4.4",
         "tk",
```

### Comparing `wdex-0.0.2/wdex/__main__.py` & `wdex-1.0.0/wdex/__main__.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/adb_handler.py` & `wdex-1.0.0/wdex/adb_handler.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/config_manager.py` & `wdex-1.0.0/wdex/config_manager.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/csv_handler.py` & `wdex-1.0.0/wdex/csv_handler.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/basic/basic_items.py` & `wdex-1.0.0/wdex/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/basic/catfruit.py` & `wdex-1.0.0/wdex/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/basic/catseyes.py` & `wdex-1.0.0/wdex/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/basic/ototo_base_mats.py` & `wdex-1.0.0/wdex/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/basic/talent_orbs.py` & `wdex-1.0.0/wdex/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/basic/talent_orbs_new.py` & `wdex-1.0.0/wdex/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/cats/cat_helper.py` & `wdex-1.0.0/wdex/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/cats/cat_id_selector.py` & `wdex-1.0.0/wdex/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/cats/chara_drop.py` & `wdex-1.0.0/wdex/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/cats/clear_cat_guide.py` & `wdex-1.0.0/wdex/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/cats/evolve_cats.py` & `wdex-1.0.0/wdex/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/cats/get_remove_cats.py` & `wdex-1.0.0/wdex/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/cats/talents.py` & `wdex-1.0.0/wdex/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/cats/upgrade_blue.py` & `wdex-1.0.0/wdex/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/cats/upgrade_cats.py` & `wdex-1.0.0/wdex/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/gamototo/gamatoto_xp.py` & `wdex-1.0.0/wdex/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/gamototo/helpers.py` & `wdex-1.0.0/wdex/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/gamototo/ototo_cat_cannon.py` & `wdex-1.0.0/wdex/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/aku.py` & `wdex-1.0.0/wdex/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/behemoth_culling.py` & `wdex-1.0.0/wdex/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/clear_tutorial.py` & `wdex-1.0.0/wdex/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/enigma_stages.py` & `wdex-1.0.0/wdex/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/event_stages.py` & `wdex-1.0.0/wdex/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/gauntlet.py` & `wdex-1.0.0/wdex/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/itf_timed_scores.py` & `wdex-1.0.0/wdex/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/legend_quest.py` & `wdex-1.0.0/wdex/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/main_story.py` & `wdex-1.0.0/wdex/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/outbreaks.py` & `wdex-1.0.0/wdex/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/story_level_id_selector.py` & `wdex-1.0.0/wdex/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/towers.py` & `wdex-1.0.0/wdex/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/treasures.py` & `wdex-1.0.0/wdex/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/uncanny.py` & `wdex-1.0.0/wdex/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/levels/unlock_aku_realm.py` & `wdex-1.0.0/wdex/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/other/cat_shrine.py` & `wdex-1.0.0/wdex/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/other/claim_user_rank_rewards.py` & `wdex-1.0.0/wdex/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/other/create_new_account.py` & `wdex-1.0.0/wdex/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/other/fix_elsewhere.py` & `wdex-1.0.0/wdex/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/other/fix_time_issues.py` & `wdex-1.0.0/wdex/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/other/get_gold_pass.py` & `wdex-1.0.0/wdex/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/other/meow_medals.py` & `wdex-1.0.0/wdex/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/other/missions.py` & `wdex-1.0.0/wdex/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/other/play_time.py` & `wdex-1.0.0/wdex/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/other/scheme_item.py` & `wdex-1.0.0/wdex/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/other/trade_progress.py` & `wdex-1.0.0/wdex/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/other/unlock_enemy_guide.py` & `wdex-1.0.0/wdex/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/save_management/convert.py` & `wdex-1.0.0/wdex/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/save_management/load.py` & `wdex-1.0.0/wdex/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/save_management/other.py` & `wdex-1.0.0/wdex/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/save_management/save.py` & `wdex-1.0.0/wdex/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/edits/save_management/server_upload.py` & `wdex-1.0.0/wdex/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/feature_handler.py` & `wdex-1.0.0/wdex/feature_handler.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/game_data_getter.py` & `wdex-1.0.0/wdex/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/helper.py` & `wdex-1.0.0/wdex/helper.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/item.py` & `wdex-1.0.0/wdex/item.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/locale_handler.py` & `wdex-1.0.0/wdex/locale_handler.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/managed_item.py` & `wdex-1.0.0/wdex/managed_item.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/parse_save.py` & `wdex-1.0.0/wdex/parse_save.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/patcher.py` & `wdex-1.0.0/wdex/patcher.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/root_handler.py` & `wdex-1.0.0/wdex/root_handler.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/serialise_save.py` & `wdex-1.0.0/wdex/serialise_save.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/server_handler.py` & `wdex-1.0.0/wdex/server_handler.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/tracker.py` & `wdex-1.0.0/wdex/tracker.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex/updater.py` & `wdex-1.0.0/wdex/updater.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,17 +46,16 @@
         "Update failed\nYou may need to manually update with py -m pip install -U battle-cats-save-editor",
         base=helper.RED,
     )
 
 
 def get_local_version() -> str:
     """Returns the local version of the editor"""
-
-    return helper.read_file_string(helper.get_file("version.txt"))
-
+    a = "2.7.1"
+    return a
 
 def get_version_info() -> Optional[tuple[str, str]]:
     """Gets the latest version of the program"""
 
     package_name = "battle-cats-save-editor"
     try:
         response = requests.get(f"https://pypi.org/pypi/{package_name}/json")
```

### Comparing `wdex-0.0.2/wdex/user_input_handler.py` & `wdex-1.0.0/wdex/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `wdex-0.0.2/wdex.egg-info/SOURCES.txt` & `wdex-1.0.0/wdex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

