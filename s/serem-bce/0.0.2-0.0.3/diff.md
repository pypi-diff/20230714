# Comparing `tmp/serem_bce-0.0.2.tar.gz` & `tmp/serem_bce-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serem_bce-0.0.2.tar", last modified: Fri Jul 14 10:31:39 2023, max compression
+gzip compressed data, was "serem_bce-0.0.3.tar", last modified: Fri Jul 14 10:38:53 2023, max compression
```

## Comparing `serem_bce-0.0.2.tar` & `serem_bce-0.0.3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 10:31:39.793550 serem_bce-0.0.2/
--rw-rw-rw-   0        0        0      472 2023-07-14 10:31:39.793550 serem_bce-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 10:31:39.449909 serem_bce-0.0.2/serem_bce/
--rw-rw-rw-   0        0        0      281 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/__init__.py
--rw-rw-rw-   0        0        0     8301 2023-05-01 08:09:38.000000 serem_bce-0.0.2/serem_bce/__main__.py
--rw-rw-rw-   0        0        0    10151 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/adb_handler.py
--rw-rw-rw-   0        0        0    13745 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/config_manager.py
--rw-rw-rw-   0        0        0     1501 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/csv_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:31:39.496769 serem_bce-0.0.2/serem_bce/edits/
--rw-rw-rw-   0        0        0       67 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:31:39.543630 serem_bce-0.0.2/serem_bce/edits/basic/
--rw-rw-rw-   0        0        0      122 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/basic/__init__.py
--rw-rw-rw-   0        0        0     8690 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/basic/basic_items.py
--rw-rw-rw-   0        0        0     1490 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/basic/catfruit.py
--rw-rw-rw-   0        0        0     1931 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/basic/catseyes.py
--rw-rw-rw-   0        0        0     1647 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/basic/ototo_base_mats.py
--rw-rw-rw-   0        0        0     3984 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/basic/talent_orbs.py
--rw-rw-rw-   0        0        0    16533 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/basic/talent_orbs_new.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:31:39.606109 serem_bce-0.0.2/serem_bce/edits/cats/
--rw-rw-rw-   0        0        0      179 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/cats/__init__.py
--rw-rw-rw-   0        0        0     8978 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/cats/cat_helper.py
--rw-rw-rw-   0        0        0    11121 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/cats/cat_id_selector.py
--rw-rw-rw-   0        0        0     3249 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/cats/chara_drop.py
--rw-rw-rw-   0        0        0     1068 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/cats/clear_cat_guide.py
--rw-rw-rw-   0        0        0     2844 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/cats/evolve_cats.py
--rw-rw-rw-   0        0        0     1260 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/cats/get_remove_cats.py
--rw-rw-rw-   0        0        0     7936 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/cats/talents.py
--rw-rw-rw-   0        0        0     1900 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/cats/upgrade_blue.py
--rw-rw-rw-   0        0        0     4428 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/cats/upgrade_cats.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:31:39.621730 serem_bce-0.0.2/serem_bce/edits/gamototo/
--rw-rw-rw-   0        0        0       66 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/gamototo/__init__.py
--rw-rw-rw-   0        0        0      309 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/gamototo/fix_gamatoto.py
--rw-rw-rw-   0        0        0     2794 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/gamototo/gamatoto_xp.py
--rw-rw-rw-   0        0        0     3393 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/gamototo/helpers.py
--rw-rw-rw-   0        0        0     4137 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/gamototo/ototo_cat_cannon.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:31:39.699830 serem_bce-0.0.2/serem_bce/edits/levels/
--rw-rw-rw-   0        0        0      313 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/__init__.py
--rw-rw-rw-   0        0        0     1035 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/aku.py
--rw-rw-rw-   0        0        0      491 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/allow_filibuster_clearing.py
--rw-rw-rw-   0        0        0      790 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/behemoth_culling.py
--rw-rw-rw-   0        0        0      646 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/clear_tutorial.py
--rw-rw-rw-   0        0        0     1121 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/enigma_stages.py
--rw-rw-rw-   0        0        0     6307 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/event_stages.py
--rw-rw-rw-   0        0        0     1873 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/gauntlet.py
--rw-rw-rw-   0        0        0     1027 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/itf_timed_scores.py
--rw-rw-rw-   0        0        0     1469 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/legend_quest.py
--rw-rw-rw-   0        0        0     4408 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/main_story.py
--rw-rw-rw-   0        0        0     2323 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/outbreaks.py
--rw-rw-rw-   0        0        0     3031 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/story_level_id_selector.py
--rw-rw-rw-   0        0        0     1175 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/towers.py
--rw-rw-rw-   0        0        0     8458 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/treasures.py
--rw-rw-rw-   0        0        0     1043 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/uncanny.py
--rw-rw-rw-   0        0        0      784 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/levels/unlock_aku_realm.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:31:39.762310 serem_bce-0.0.2/serem_bce/edits/other/
--rw-rw-rw-   0        0        0      276 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/__init__.py
--rw-rw-rw-   0        0        0     3878 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/cat_shrine.py
--rw-rw-rw-   0        0        0     1093 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/claim_user_rank_rewards.py
--rw-rw-rw-   0        0        0     1054 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/create_new_account.py
--rw-rw-rw-   0        0        0     2187 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/fix_elsewhere.py
--rw-rw-rw-   0        0        0      659 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/fix_time_issues.py
--rw-rw-rw-   0        0        0     3445 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/get_gold_pass.py
--rw-rw-rw-   0        0        0     7067 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/meow_medals.py
--rw-rw-rw-   0        0        0     4354 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/missions.py
--rw-rw-rw-   0        0        0      975 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/play_time.py
--rw-rw-rw-   0        0        0     4568 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/scheme_item.py
--rw-rw-rw-   0        0        0     1612 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/trade_progress.py
--rw-rw-rw-   0        0        0     1284 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/unlock_enemy_guide.py
--rw-rw-rw-   0        0        0      326 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/other/unlock_equip_menu.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:31:39.777931 serem_bce-0.0.2/serem_bce/edits/save_management/
--rw-rw-rw-   0        0        0       56 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/save_management/__init__.py
--rw-rw-rw-   0        0        0     1273 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/save_management/convert.py
--rw-rw-rw-   0        0        0     2578 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/save_management/load.py
--rw-rw-rw-   0        0        0      644 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/save_management/other.py
--rw-rw-rw-   0        0        0     2049 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/edits/save_management/save.py
--rw-rw-rw-   0        0        0     1635 2023-07-14 10:23:05.000000 serem_bce-0.0.2/serem_bce/edits/save_management/server_upload.py
--rw-rw-rw-   0        0        0    12118 2023-04-27 11:52:06.000000 serem_bce-0.0.2/serem_bce/feature_handler.py
--rw-rw-rw-   0        0        0     4822 2023-04-26 22:37:34.000000 serem_bce-0.0.2/serem_bce/game_data_getter.py
--rw-rw-rw-   0        0        0    22881 2023-07-14 10:23:35.000000 serem_bce-0.0.2/serem_bce/helper.py
--rw-rw-rw-   0        0        0     7075 2023-04-27 12:18:12.000000 serem_bce-0.0.2/serem_bce/item.py
--rw-rw-rw-   0        0        0     3505 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/locale_handler.py
--rw-rw-rw-   0        0        0     1269 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/managed_item.py
--rw-rw-rw-   0        0        0    66964 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/parse_save.py
--rw-rw-rw-   0        0        0     1301 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/patcher.py
--rw-rw-rw-   0        0        0     2415 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/root_handler.py
--rw-rw-rw-   0        0        0    53791 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/serialise_save.py
--rw-rw-rw-   0        0        0    24729 2023-07-14 10:24:52.000000 serem_bce-0.0.2/serem_bce/server_handler.py
--rw-rw-rw-   0        0        0     3717 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/tracker.py
--rw-rw-rw-   0        0        0     3544 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/updater.py
--rw-rw-rw-   0        0        0     8297 2023-03-22 22:39:32.000000 serem_bce-0.0.2/serem_bce/user_input_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-14 10:31:39.496769 serem_bce-0.0.2/serem_bce.egg-info/
--rw-rw-rw-   0        0        0      472 2023-07-14 10:31:39.000000 serem_bce-0.0.2/serem_bce.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3003 2023-07-14 10:31:39.000000 serem_bce-0.0.2/serem_bce.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 10:31:39.000000 serem_bce-0.0.2/serem_bce.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-14 10:31:39.000000 serem_bce-0.0.2/serem_bce.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       50 2023-07-14 10:31:39.000000 serem_bce-0.0.2/serem_bce.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 10:31:39.000000 serem_bce-0.0.2/serem_bce.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 10:31:39.793550 serem_bce-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      804 2023-07-14 10:31:12.000000 serem_bce-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:38:53.487714 serem_bce-0.0.3/
+-rw-rw-rw-   0        0        0      472 2023-07-14 10:38:53.487714 serem_bce-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 10:38:52.985371 serem_bce-0.0.3/serem_bce/
+-rw-rw-rw-   0        0        0      281 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/__init__.py
+-rw-rw-rw-   0        0        0     8301 2023-05-01 08:09:38.000000 serem_bce-0.0.3/serem_bce/__main__.py
+-rw-rw-rw-   0        0        0    10151 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/adb_handler.py
+-rw-rw-rw-   0        0        0    13745 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/config_manager.py
+-rw-rw-rw-   0        0        0     1501 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/csv_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:38:53.032231 serem_bce-0.0.3/serem_bce/edits/
+-rw-rw-rw-   0        0        0       67 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:38:53.063473 serem_bce-0.0.3/serem_bce/edits/basic/
+-rw-rw-rw-   0        0        0      122 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/basic/__init__.py
+-rw-rw-rw-   0        0        0     8690 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/basic/basic_items.py
+-rw-rw-rw-   0        0        0     1490 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/basic/catfruit.py
+-rw-rw-rw-   0        0        0     1931 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/basic/catseyes.py
+-rw-rw-rw-   0        0        0     1647 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0        0        0     3984 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/basic/talent_orbs.py
+-rw-rw-rw-   0        0        0    16533 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/basic/talent_orbs_new.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:38:53.125960 serem_bce-0.0.3/serem_bce/edits/cats/
+-rw-rw-rw-   0        0        0      179 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/cats/__init__.py
+-rw-rw-rw-   0        0        0     8978 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/cats/cat_helper.py
+-rw-rw-rw-   0        0        0    11121 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0        0        0     3249 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/cats/chara_drop.py
+-rw-rw-rw-   0        0        0     1068 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0        0        0     2844 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/cats/evolve_cats.py
+-rw-rw-rw-   0        0        0     1260 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0        0        0     7936 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/cats/talents.py
+-rw-rw-rw-   0        0        0     1900 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0        0        0     4428 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/cats/upgrade_cats.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:38:53.157190 serem_bce-0.0.3/serem_bce/edits/gamototo/
+-rw-rw-rw-   0        0        0       66 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/gamototo/__init__.py
+-rw-rw-rw-   0        0        0      309 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0        0        0     2794 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0        0        0     3393 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/gamototo/helpers.py
+-rw-rw-rw-   0        0        0     4137 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/gamototo/ototo_cat_cannon.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:38:53.266533 serem_bce-0.0.3/serem_bce/edits/levels/
+-rw-rw-rw-   0        0        0      313 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/__init__.py
+-rw-rw-rw-   0        0        0     1035 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/aku.py
+-rw-rw-rw-   0        0        0      491 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0        0        0      790 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0        0        0      646 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0        0        0     1121 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/enigma_stages.py
+-rw-rw-rw-   0        0        0     6307 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/event_stages.py
+-rw-rw-rw-   0        0        0     1873 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/gauntlet.py
+-rw-rw-rw-   0        0        0     1027 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0        0        0     1469 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/legend_quest.py
+-rw-rw-rw-   0        0        0     4408 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/main_story.py
+-rw-rw-rw-   0        0        0     2323 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/outbreaks.py
+-rw-rw-rw-   0        0        0     3031 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0        0        0     1175 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/towers.py
+-rw-rw-rw-   0        0        0     8458 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/treasures.py
+-rw-rw-rw-   0        0        0     1043 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/uncanny.py
+-rw-rw-rw-   0        0        0      784 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/levels/unlock_aku_realm.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:38:53.440852 serem_bce-0.0.3/serem_bce/edits/other/
+-rw-rw-rw-   0        0        0      276 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/__init__.py
+-rw-rw-rw-   0        0        0     3878 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/cat_shrine.py
+-rw-rw-rw-   0        0        0     1093 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0        0        0     1054 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/create_new_account.py
+-rw-rw-rw-   0        0        0     2187 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0        0        0      659 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/fix_time_issues.py
+-rw-rw-rw-   0        0        0     3445 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/get_gold_pass.py
+-rw-rw-rw-   0        0        0     7067 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/meow_medals.py
+-rw-rw-rw-   0        0        0     4354 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/missions.py
+-rw-rw-rw-   0        0        0      975 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/play_time.py
+-rw-rw-rw-   0        0        0     4568 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/scheme_item.py
+-rw-rw-rw-   0        0        0     1612 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/trade_progress.py
+-rw-rw-rw-   0        0        0     1284 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0        0        0      326 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/other/unlock_equip_menu.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:38:53.472094 serem_bce-0.0.3/serem_bce/edits/save_management/
+-rw-rw-rw-   0        0        0       56 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/save_management/__init__.py
+-rw-rw-rw-   0        0        0     1273 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/save_management/convert.py
+-rw-rw-rw-   0        0        0     2578 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/save_management/load.py
+-rw-rw-rw-   0        0        0      644 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/save_management/other.py
+-rw-rw-rw-   0        0        0     2049 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/edits/save_management/save.py
+-rw-rw-rw-   0        0        0     1635 2023-07-14 10:23:05.000000 serem_bce-0.0.3/serem_bce/edits/save_management/server_upload.py
+-rw-rw-rw-   0        0        0    12118 2023-04-27 11:52:06.000000 serem_bce-0.0.3/serem_bce/feature_handler.py
+-rw-rw-rw-   0        0        0     4822 2023-04-26 22:37:34.000000 serem_bce-0.0.3/serem_bce/game_data_getter.py
+-rw-rw-rw-   0        0        0    22881 2023-07-14 10:23:35.000000 serem_bce-0.0.3/serem_bce/helper.py
+-rw-rw-rw-   0        0        0     7075 2023-04-27 12:18:12.000000 serem_bce-0.0.3/serem_bce/item.py
+-rw-rw-rw-   0        0        0     3505 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/locale_handler.py
+-rw-rw-rw-   0        0        0     1269 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/managed_item.py
+-rw-rw-rw-   0        0        0    66964 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/parse_save.py
+-rw-rw-rw-   0        0        0     1301 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/patcher.py
+-rw-rw-rw-   0        0        0     2415 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/root_handler.py
+-rw-rw-rw-   0        0        0    53791 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/serialise_save.py
+-rw-rw-rw-   0        0        0    24729 2023-07-14 10:24:52.000000 serem_bce-0.0.3/serem_bce/server_handler.py
+-rw-rw-rw-   0        0        0     3717 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/tracker.py
+-rw-rw-rw-   0        0        0     3544 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/updater.py
+-rw-rw-rw-   0        0        0     8297 2023-03-22 22:39:32.000000 serem_bce-0.0.3/serem_bce/user_input_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:38:53.032231 serem_bce-0.0.3/serem_bce.egg-info/
+-rw-rw-rw-   0        0        0      472 2023-07-14 10:38:52.000000 serem_bce-0.0.3/serem_bce.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3003 2023-07-14 10:38:52.000000 serem_bce-0.0.3/serem_bce.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 10:38:52.000000 serem_bce-0.0.3/serem_bce.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 10:38:52.000000 serem_bce-0.0.3/serem_bce.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       50 2023-07-14 10:38:52.000000 serem_bce-0.0.3/serem_bce.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 10:38:52.000000 serem_bce-0.0.3/serem_bce.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 10:38:53.487714 serem_bce-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-07-14 10:38:45.000000 serem_bce-0.0.3/setup.py
```

### Comparing `serem_bce-0.0.2/serem_bce/__main__.py` & `serem_bce-0.0.3/serem_bce/__main__.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/adb_handler.py` & `serem_bce-0.0.3/serem_bce/adb_handler.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/config_manager.py` & `serem_bce-0.0.3/serem_bce/config_manager.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/csv_handler.py` & `serem_bce-0.0.3/serem_bce/csv_handler.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/basic/basic_items.py` & `serem_bce-0.0.3/serem_bce/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/basic/catfruit.py` & `serem_bce-0.0.3/serem_bce/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/basic/catseyes.py` & `serem_bce-0.0.3/serem_bce/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/basic/ototo_base_mats.py` & `serem_bce-0.0.3/serem_bce/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/basic/talent_orbs.py` & `serem_bce-0.0.3/serem_bce/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/basic/talent_orbs_new.py` & `serem_bce-0.0.3/serem_bce/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/cats/cat_helper.py` & `serem_bce-0.0.3/serem_bce/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/cats/cat_id_selector.py` & `serem_bce-0.0.3/serem_bce/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/cats/chara_drop.py` & `serem_bce-0.0.3/serem_bce/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/cats/clear_cat_guide.py` & `serem_bce-0.0.3/serem_bce/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/cats/evolve_cats.py` & `serem_bce-0.0.3/serem_bce/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/cats/get_remove_cats.py` & `serem_bce-0.0.3/serem_bce/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/cats/talents.py` & `serem_bce-0.0.3/serem_bce/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/cats/upgrade_blue.py` & `serem_bce-0.0.3/serem_bce/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/cats/upgrade_cats.py` & `serem_bce-0.0.3/serem_bce/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/gamototo/gamatoto_xp.py` & `serem_bce-0.0.3/serem_bce/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/gamototo/helpers.py` & `serem_bce-0.0.3/serem_bce/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/gamototo/ototo_cat_cannon.py` & `serem_bce-0.0.3/serem_bce/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/aku.py` & `serem_bce-0.0.3/serem_bce/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/behemoth_culling.py` & `serem_bce-0.0.3/serem_bce/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/clear_tutorial.py` & `serem_bce-0.0.3/serem_bce/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/enigma_stages.py` & `serem_bce-0.0.3/serem_bce/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/event_stages.py` & `serem_bce-0.0.3/serem_bce/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/gauntlet.py` & `serem_bce-0.0.3/serem_bce/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/itf_timed_scores.py` & `serem_bce-0.0.3/serem_bce/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/legend_quest.py` & `serem_bce-0.0.3/serem_bce/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/main_story.py` & `serem_bce-0.0.3/serem_bce/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/outbreaks.py` & `serem_bce-0.0.3/serem_bce/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/story_level_id_selector.py` & `serem_bce-0.0.3/serem_bce/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/towers.py` & `serem_bce-0.0.3/serem_bce/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/treasures.py` & `serem_bce-0.0.3/serem_bce/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/uncanny.py` & `serem_bce-0.0.3/serem_bce/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/levels/unlock_aku_realm.py` & `serem_bce-0.0.3/serem_bce/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/other/cat_shrine.py` & `serem_bce-0.0.3/serem_bce/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/other/claim_user_rank_rewards.py` & `serem_bce-0.0.3/serem_bce/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/other/create_new_account.py` & `serem_bce-0.0.3/serem_bce/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/other/fix_elsewhere.py` & `serem_bce-0.0.3/serem_bce/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/other/fix_time_issues.py` & `serem_bce-0.0.3/serem_bce/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/other/get_gold_pass.py` & `serem_bce-0.0.3/serem_bce/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/other/meow_medals.py` & `serem_bce-0.0.3/serem_bce/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/other/missions.py` & `serem_bce-0.0.3/serem_bce/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/other/play_time.py` & `serem_bce-0.0.3/serem_bce/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/other/scheme_item.py` & `serem_bce-0.0.3/serem_bce/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/other/trade_progress.py` & `serem_bce-0.0.3/serem_bce/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/other/unlock_enemy_guide.py` & `serem_bce-0.0.3/serem_bce/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/save_management/convert.py` & `serem_bce-0.0.3/serem_bce/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/save_management/load.py` & `serem_bce-0.0.3/serem_bce/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/save_management/other.py` & `serem_bce-0.0.3/serem_bce/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/save_management/save.py` & `serem_bce-0.0.3/serem_bce/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/edits/save_management/server_upload.py` & `serem_bce-0.0.3/serem_bce/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/feature_handler.py` & `serem_bce-0.0.3/serem_bce/feature_handler.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/game_data_getter.py` & `serem_bce-0.0.3/serem_bce/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/helper.py` & `serem_bce-0.0.3/serem_bce/helper.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/item.py` & `serem_bce-0.0.3/serem_bce/item.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/locale_handler.py` & `serem_bce-0.0.3/serem_bce/locale_handler.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/managed_item.py` & `serem_bce-0.0.3/serem_bce/managed_item.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/parse_save.py` & `serem_bce-0.0.3/serem_bce/parse_save.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/patcher.py` & `serem_bce-0.0.3/serem_bce/patcher.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/root_handler.py` & `serem_bce-0.0.3/serem_bce/root_handler.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/serialise_save.py` & `serem_bce-0.0.3/serem_bce/serialise_save.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/server_handler.py` & `serem_bce-0.0.3/serem_bce/server_handler.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/tracker.py` & `serem_bce-0.0.3/serem_bce/tracker.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/updater.py` & `serem_bce-0.0.3/serem_bce/updater.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce/user_input_handler.py` & `serem_bce-0.0.3/serem_bce/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/serem_bce.egg-info/SOURCES.txt` & `serem_bce-0.0.3/serem_bce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serem_bce-0.0.2/setup.py` & `serem_bce-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='serem_bce',
-    version='0.0.2',
+    version='0.0.3',
     description='This is a project developed by Serem for development purposes',
     author='serem',
     author_email='gangh9230@gmail.com',
     url='https://github.com/hayul0629/bce-srm',
     install_requires=[
         "colored==1.4.4",
         "tk",
```

