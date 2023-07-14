# Comparing `tmp/nonebot_plugin_simulator_xiuxian-0.5.21.tar.gz` & `tmp/nonebot_plugin_simulator_xiuxian-0.5.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_simulator_xiuxian-0.5.21.tar", last modified: Thu Mar 16 12:51:26 2023, max compression
+gzip compressed data, was "nonebot_plugin_simulator_xiuxian-0.5.22.tar", last modified: Fri Jul 14 19:51:33 2023, max compression
```

## Comparing `nonebot_plugin_simulator_xiuxian-0.5.21.tar` & `nonebot_plugin_simulator_xiuxian-0.5.22.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 12:51:26.125380 nonebot_plugin_simulator_xiuxian-0.5.21/
--rw-rw-rw-   0        0        0      264 2023-03-16 12:51:26.125380 nonebot_plugin_simulator_xiuxian-0.5.21/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-16 12:51:26.112974 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/
--rw-rw-rw-   0        0        0     2028 2023-03-16 11:20:54.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/__init__.py
--rw-rw-rw-   0        0        0     1960 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/cd_manager.py
--rw-rw-rw-   0        0        0      358 2023-03-13 16:40:54.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/config.py
--rw-rw-rw-   0        0        0     2849 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/data_source.py
--rw-rw-rw-   0        0        0     1787 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/exp_util.py
--rw-rw-rw-   0        0        0     1354 2023-03-15 09:22:16.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/help.py
--rw-rw-rw-   0        0        0     4430 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/item_json.py
--rw-rw-rw-   0        0        0    50728 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/player_fight.py
--rw-rw-rw-   0        0        0     8141 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/read_buff.py
--rw-rw-rw-   0        0        0     8555 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/utils.py
--rw-rw-rw-   0        0        0    55510 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py
--rw-rw-rw-   0        0        0     5784 2023-03-16 12:42:48.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/xiuxian_config.py
--rw-rw-rw-   0        0        0      787 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py
--rw-rw-rw-   0        0        0     2477 2023-03-15 09:16:32.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py
-drwxrwxrwx   0        0        0        0 2023-03-16 12:51:26.124177 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian.egg-info/
--rw-rw-rw-   0        0        0      264 2023-03-16 12:51:26.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-03-16 12:51:26.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 12:51:26.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-03-16 12:51:26.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-03-16 12:51:26.000000 nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-16 12:51:26.125380 nonebot_plugin_simulator_xiuxian-0.5.21/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-03-16 12:51:23.000000 nonebot_plugin_simulator_xiuxian-0.5.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 19:51:33.395007 nonebot_plugin_simulator_xiuxian-0.5.22/
+-rw-rw-rw-   0        0        0      264 2023-07-14 19:51:33.395007 nonebot_plugin_simulator_xiuxian-0.5.22/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 19:51:33.382964 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/
+-rw-rw-rw-   0        0        0     2028 2023-03-16 11:20:54.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/__init__.py
+-rw-rw-rw-   0        0        0     1960 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/cd_manager.py
+-rw-rw-rw-   0        0        0      358 2023-03-13 16:40:54.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/config.py
+-rw-rw-rw-   0        0        0     2849 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/data_source.py
+-rw-rw-rw-   0        0        0     1787 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/exp_util.py
+-rw-rw-rw-   0        0        0      101 2023-07-14 16:18:51.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/help.py
+-rw-rw-rw-   0        0        0     4430 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/item_json.py
+-rw-rw-rw-   0        0        0    50728 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/player_fight.py
+-rw-rw-rw-   0        0        0     8141 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/read_buff.py
+-rw-rw-rw-   0        0        0     8555 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/utils.py
+-rw-rw-rw-   0        0        0    55510 2023-06-22 17:42:27.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py
+-rw-rw-rw-   0        0        0     5814 2023-07-14 16:11:36.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/xiuxian_config.py
+-rw-rw-rw-   0        0        0      787 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py
+-rw-rw-rw-   0        0        0     2477 2023-07-14 19:33:45.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py
+drwxrwxrwx   0        0        0        0 2023-07-14 19:51:33.394054 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-07-14 19:51:33.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-07-14 19:51:33.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 19:51:33.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-14 19:51:33.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-07-14 19:51:33.000000 nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 19:51:33.395007 nonebot_plugin_simulator_xiuxian-0.5.22/setup.cfg
+-rw-rw-rw-   0        0        0      592 2023-07-14 19:35:09.000000 nonebot_plugin_simulator_xiuxian-0.5.22/setup.py
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/__init__.py` & `nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/cd_manager.py` & `nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/cd_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/data_source.py` & `nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/exp_util.py` & `nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/exp_util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/item_json.py` & `nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/item_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/player_fight.py` & `nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/player_fight.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/read_buff.py` & `nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/read_buff.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/utils.py` & `nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py` & `nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/xiuxian_config.py` & `nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/xiuxian_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,59 @@
     import ujson as json
 except ImportError:
     import json
 from pathlib import Path
 
 DATABASE = Path() / "data" / "xiuxian"
 
+
+USERRANK = {
+    '江湖好手':50,
+    '练气境初期':49,
+    '练气境中期':48,
+    '练气境圆满':47,
+    '筑基境初期':46,
+    '筑基境中期':45,
+    '筑基境圆满':44,
+    '结丹境初期':43,
+    '结丹境中期':42,
+    '结丹境圆满':41,
+    '元婴境初期':40,
+    '元婴境中期':39,
+    '元婴境圆满':38,
+    '化神境初期':37,
+    '化神境中期':36,
+    '化神境圆满':35,
+    '炼虚境初期':34,
+    '炼虚境中期':33,
+    '炼虚境圆满':32,
+    '合体境初期':31,
+    '合体境中期':30,
+    '合体境圆满':29,
+    '大乘境初期':28,
+    '大乘境中期':27,
+    '大乘境圆满':26,
+    '渡劫境初期':25,
+    '渡劫境中期':24,
+    '渡劫境圆满':23,
+    '半步真仙':22,
+    '真仙境初期':21,
+    '真仙境中期':20,
+    '真仙境圆满':19,
+    '金仙境初期':18,
+    '金仙境中期':17,
+    '金仙境圆满':16,
+    '太乙境初期':15,
+    '太乙境中期':14,
+    '太乙境圆满':13,
+    '真仙境初期':12,
+    '悟道境': 11,
+}
+
+
 class XiuConfig:
 
     def __init__(self):
 
 
         self.level = list(USERRANK.keys())
         self.level_up_cd = 60  # 突破CD(分钟)
@@ -29,15 +74,15 @@
         self.sect_min_level = "渡劫境初期"  # 创建宗门的最低修为等级要求
         self.sect_create_cost = 25  # 创建宗门的最低修为等级要求
         self.user_info_cd = 10  # 我的修仙信息查询cd
         self.user_info_cd_msg = 5
         self.dufang_cd_msg = 5
         self.tou_cd = 5  # 偷灵石CD
         self.battle_boss_cd = 60  # 讨伐bossCD
-        self.version = "xiuxian_1.1"
+        self.version = "xinxian_1.1"
 
         self.sql_table = ["user_xiuxian", "user_cd", "sects", "back", "BuffInfo"]  # 数据库表校验
         self.sql_user_xiuxian = ["level_up_rate","sect_id","sect_position"
                                  ,"hp", "mp", "atk", "atkpractice", "sect_task",
                                 "sect_contribution","sect_elixir_get", 
                                 "blessed_spot_flag","blessed_spot_name"]   # 数据库字段校验
         self.sql_sects = ["sect_materials", "mainbuff", "secbuff", "elixir_room_level"]
@@ -91,55 +136,15 @@
                         return False
             except KeyError:
                 json_data['group'] = [group_id]
 
         with open(self.config_jsonpath, 'w', encoding='utf-8') as f:
             json.dump(json_data, f)
 
-USERRANK = {
-    '江湖好手':50,
-    '练气境初期':49,
-    '练气境中期':48,
-    '练气境圆满':47,
-    '筑基境初期':46,
-    '筑基境中期':45,
-    '筑基境圆满':44,
-    '结丹境初期':43,
-    '结丹境中期':42,
-    '结丹境圆满':41,
-    '元婴境初期':40,
-    '元婴境中期':39,
-    '元婴境圆满':38,
-    '化神境初期':37,
-    '化神境中期':36,
-    '化神境圆满':35,
-    '炼虚境初期':34,
-    '炼虚境中期':33,
-    '炼虚境圆满':32,
-    '合体境初期':31,
-    '合体境中期':30,
-    '合体境圆满':29,
-    '大乘境初期':28,
-    '大乘境中期':27,
-    '大乘境圆满':26,
-    '渡劫境初期':25,
-    '渡劫境中期':24,
-    '渡劫境圆满':23,
-    '半步真仙':22,
-    '真仙境初期':21,
-    '真仙境中期':20,
-    '真仙境圆满':19,
-    '金仙境初期':18,
-    '金仙境中期':17,
-    '金仙境圆满':16,
-    '太乙境初期':15,
-    '太乙境中期':14,
-    '太乙境圆满':13,
-    '渡劫境初期':25,
-}
+
 
 if __name__ == '__main__':
     pathname = r""
     with open(pathname, 'r', encoding='utf-8') as e:
         data = json.load(e)
 
     key = 4
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py` & `nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py` & `nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt` & `nonebot_plugin_simulator_xiuxian-0.5.22/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.21/setup.py` & `nonebot_plugin_simulator_xiuxian-0.5.22/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages,find_packages
 
 setup(
 name='nonebot_plugin_simulator_xiuxian',
-version='0.5.21',
+version='0.5.22',
 description='修仙',
 #long_description=open('README.md','r').read(),
 author='luoyefufeng',
 author_email='2859385794@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_simulator_xiuxian"]),
```

