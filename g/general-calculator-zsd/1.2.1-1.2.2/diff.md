# Comparing `tmp/general_calculator_zsd-1.2.1.tar.gz` & `tmp/general_calculator_zsd-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general_calculator_zsd-1.2.1.tar", last modified: Wed Jun 28 03:34:24 2023, max compression
+gzip compressed data, was "general_calculator_zsd-1.2.2.tar", last modified: Fri Jul 14 05:52:41 2023, max compression
```

## Comparing `general_calculator_zsd-1.2.1.tar` & `general_calculator_zsd-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 03:34:24.158194 general_calculator_zsd-1.2.1/
--rw-rw-rw-   0        0        0     1089 2022-11-17 02:56:12.000000 general_calculator_zsd-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      418 2023-06-28 03:34:24.157195 general_calculator_zsd-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-03-30 02:25:01.000000 general_calculator_zsd-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 03:34:24.116483 general_calculator_zsd-1.2.1/general_calculator_zsd/
--rw-rw-rw-   0        0        0        0 2022-11-16 09:26:23.000000 general_calculator_zsd-1.2.1/general_calculator_zsd/__init__.py
--rw-rw-rw-   0        0        0    49969 2023-06-28 03:31:22.000000 general_calculator_zsd-1.2.1/general_calculator_zsd/general_calculator.py
--rw-rw-rw-   0        0        0    67692 2023-06-28 03:25:53.000000 general_calculator_zsd-1.2.1/general_calculator_zsd/mysql_transmit_data4all.py
-drwxrwxrwx   0        0        0        0 2023-06-28 03:34:24.154198 general_calculator_zsd-1.2.1/general_calculator_zsd.egg-info/
--rw-rw-rw-   0        0        0      418 2023-06-28 03:34:23.000000 general_calculator_zsd-1.2.1/general_calculator_zsd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-06-28 03:34:23.000000 general_calculator_zsd-1.2.1/general_calculator_zsd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 03:34:23.000000 general_calculator_zsd-1.2.1/general_calculator_zsd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-28 03:34:23.000000 general_calculator_zsd-1.2.1/general_calculator_zsd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 03:34:24.158194 general_calculator_zsd-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      531 2023-06-28 03:31:55.000000 general_calculator_zsd-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:52:41.805643 general_calculator_zsd-1.2.2/
+-rw-rw-rw-   0        0        0     1089 2022-11-17 02:56:12.000000 general_calculator_zsd-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0      487 2023-07-14 05:52:41.805643 general_calculator_zsd-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-03-30 02:25:01.000000 general_calculator_zsd-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 05:52:41.774394 general_calculator_zsd-1.2.2/general_calculator_zsd/
+-rw-rw-rw-   0        0        0        0 2022-11-16 09:26:23.000000 general_calculator_zsd-1.2.2/general_calculator_zsd/__init__.py
+-rw-rw-rw-   0        0        0    49969 2023-06-28 03:35:22.000000 general_calculator_zsd-1.2.2/general_calculator_zsd/general_calculator.py
+-rw-rw-rw-   0        0        0    70779 2023-07-14 05:21:34.000000 general_calculator_zsd-1.2.2/general_calculator_zsd/mysql_transmit_data4all.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:52:41.805643 general_calculator_zsd-1.2.2/general_calculator_zsd.egg-info/
+-rw-rw-rw-   0        0        0      487 2023-07-14 05:52:40.000000 general_calculator_zsd-1.2.2/general_calculator_zsd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-07-14 05:52:41.000000 general_calculator_zsd-1.2.2/general_calculator_zsd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 05:52:40.000000 general_calculator_zsd-1.2.2/general_calculator_zsd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-14 05:52:40.000000 general_calculator_zsd-1.2.2/general_calculator_zsd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 05:52:41.805643 general_calculator_zsd-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      600 2023-07-14 05:52:14.000000 general_calculator_zsd-1.2.2/setup.py
```

### Comparing `general_calculator_zsd-1.2.1/LICENSE` & `general_calculator_zsd-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `general_calculator_zsd-1.2.1/general_calculator_zsd/general_calculator.py` & `general_calculator_zsd-1.2.2/general_calculator_zsd/general_calculator.py`

 * *Files identical despite different names*

### Comparing `general_calculator_zsd-1.2.1/general_calculator_zsd/mysql_transmit_data4all.py` & `general_calculator_zsd-1.2.2/general_calculator_zsd/mysql_transmit_data4all.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,28 +55,31 @@
     'dongchedi_koubei_comment': ['etl_comment', 'comment_id', 600, 'BA_USING'],
     'dongchedi_user_info': ['etl_user', 'user_id', 600, 'BA_USING'],
     'xinchuxing_community_post': ['etl_post', 'post_id', 700, 'BA_USING'],
     'xinchuxing_comment': ['etl_comment', 'comment_id', 700, 'BA_USING'],
     'xinchuxing_user_info': ['etl_user', 'user_id', 700, 'BA_USING'],
     '42hao_community_post': ['etl_post', 'post_id', 800, 'BA_USING'],
     '42hao_comment': ['etl_comment', 'comment_id', 800, 'BA_USING'],
-    '42hao_user_info': ['etl_user', 'user_id', 800, 'BA_USING']
+    '42hao_user_info': ['etl_user', 'user_id', 800, 'BA_USING'],
+    'douyin_search_post': ['etl_post', 'post_id', 900, 'BA_USING'],
+    'douyin_comment': ['etl_comment', 'comment_id', 900, 'BA_USING'],
+    'douyin_user_info': ['etl_user', 'user_id', 900, 'BA_USING']
 }
 
 # insert_table与select_table对应关系
 post_list = ['autohome_wenzhang_post', 'autohome_luntan_post', 'autohome_koubei_post','dongchedi_wenzhang_post',
              'dongchedi_cheyouquan_post', 'dongchedi_koubei_post', 'bilibili_video_post',
              'weibo_auth_post', 'weibo_search_post', 'xiaohongshu_search_post', 'moment', 'xinchuxing_community_post',
-             '42hao_community_post']
+             '42hao_community_post', 'douyin_search_post']
 cmt_list = ['autohome_wenzhang_comment', 'autohome_luntan_comment', 'autohome_koubei_comment',
             'dongchedi_wenzhang_comment', 'dongchedi_cheyouquan_comment', 'dongchedi_koubei_comment',
             'bilibili_video_comment','bilibili_video_danmu', 'weibo_comment', 'xiaohongshu_comment',
-            'momentcomment', 'smart_tucaoba_comment', 'xinchuxing_comment', '42hao_comment']
+            'momentcomment', 'smart_tucaoba_comment', 'xinchuxing_comment', '42hao_comment', 'douyin_comment']
 user_list = ['autohome_user_info', 'dongchedi_user_info', 'weibo_user_info', 'xiaohongshu_user_info', 
-             'bilibili_user_info', 'user_base', 'xinchuxing_user_info', '42hao_user_info']
+             'bilibili_user_info', 'user_base', 'xinchuxing_user_info', '42hao_user_info', 'douyin_user_info']
 
 hobby_eng2chn = {
     'cheyouhui': '车友会',
     'finance': '金融',
     'play_car': '玩车',
     'parenting': '亲子',
     'read': '读书',
@@ -321,15 +324,15 @@
                 print(hobby_eng)
     hobby_str = '|'.join(hobby_list_chn)
     if hobby_str == '':
         hobby_str = None 
     return hobby_str
 
 
-def insert_json_sql(json_data, insert_ip, insert_table, select_table, cover_flag):  # sql 执行数据库语句
+def insert_json_sql2etl(json_data, insert_ip, insert_table, select_table, cover_flag, insert_mode = 'default'):  # sql 执行数据库语句
     # 连接导入数据库
     insert_conn = pymysql.connect(host=dic_connet[insert_ip]['host'], port=dic_connet[insert_ip]['port'], user=dic_connet[insert_ip]['user'], password=dic_connet[insert_ip]['password'], db=dic_connet[insert_ip]['database'])
     insert_cursor = insert_conn.cursor()
     insert_data = {}
     insert_data["upload_datetime"] = get_datetime_now()
     # 自定义部分——导入数据预处理（手动填写需要导入的字段名 及 对应的上游数据字段名）
     if select_table == 'autohome_wenzhang_comment':
@@ -983,14 +986,62 @@
         insert_data["user_summary"] = json_data['introduce']
         # insert_data["user_post_count"] = json_data["post_count"]
         insert_data["following_count"] = json_data["following_count"]
         insert_data["follower_count"] = json_data["follower_count"]
         insert_data["spider_datetime"] = json_data["spider_datetime"]
         insert_data["user_car_owned"] = json_data["author_car_info_paid"]
         insert_data["user_car_interested"] = json_data["author_car_info_intention"]
+    elif select_table == 'douyin_search_post':
+        insert_data["platform_id"] = json_data["platform_id"]
+        insert_data["post_id"] = json_data["post_id"]
+        insert_data["user_id"] = json_data["user_id"]
+        insert_data["account_name"] = json_data["account_name"]
+        insert_data["post_datetime"] = json_data["post_datetime"]
+        insert_data["post_content"] = json_data["post_content"]
+        # insert_data["read_count"] = json_data["view_count"]
+        insert_data["like_count"] = json_data["likes_count"]
+        insert_data["comment_count"] = json_data["comment_count"]
+        insert_data["repost_count"] = json_data["shared_count"]
+        insert_data["spider_datetime"] = json_data["spider_datetime"]
+        insert_data["keyword"] = json_data["search_keyword"]
+        insert_data["brand_id"] = json_data["brand_id"]
+        insert_data["series_id"] = json_data["series_id"]
+        insert_data["post_url"] = json_data["post_url"]
+        insert_data["hot_degree"] = 20*json_data["shared_count"] + 10*json_data["comment_count"] + json_data["likes_count"]
+    elif select_table == 'douyin_comment':
+        insert_data["platform_id"] = json_data["platform_id"]
+        insert_data["comment_id"] = json_data["comment_id"]
+        insert_data["user_id"] = json_data["user_id"]
+        insert_data["comment_datetime"] = json_data["comment_publish_time"]
+        insert_data['comment_country'] = json_data['comment_country']
+        insert_data["comment_province"] = json_data['comment_province']
+        insert_data["comment_content"] = json_data["comment_content"]
+        insert_data["comment_like_count"] = json_data["comment_like_count"]
+        insert_data["comment_reply_count"] = json_data["comment_reply_count"]
+        insert_data["comment_main_flag"] = json_data["main_comment_flag"]
+        insert_data["comment_main_id"] = json_data["main_comment_id"]
+        insert_data["post_id"] = json_data["post_id"]
+        insert_data["spider_datetime"] = json_data["spider_datetime"]
+    elif select_table == 'douyin_user_info':
+        insert_data["media_id"] = json_data["media_id"]
+        insert_data["user_id"] = json_data["user_id"]
+        insert_data["user_nickname"] = json_data["user_nickname"]
+        insert_data["user_gender"] = json_data["user_gender"]
+        insert_data["user_country"] = json_data["user_country"]
+        insert_data["user_province"] = json_data["user_province"]
+        insert_data["user_city"] = json_data["user_city"]
+        insert_data["user_work"] = json_data["user_work"]
+        insert_data["user_summary"] = json_data["user_summary"]
+        insert_data["verified_flag"] = json_data["verified_flag"]
+        insert_data["verified_reason"] = json_data["verified_reason"]
+        insert_data["user_post_count"] = json_data["note_count"]
+        insert_data["following_count"] = json_data["following_count"]
+        insert_data["follower_count"] = json_data["follower_count"]
+        insert_data["user_level"] = json_data["level"]
+        insert_data["spider_datetime"] = json_data["spider_datetime"]
     else:
         sys.exit()
     # 判断用户类型，抽取用户简介中的关键词
     feature_list = []
     type_list = []
     if select_table in user_list:
         # 检查方式1：检查昵称中是否包含某个异常类型关键词
@@ -1015,34 +1066,29 @@
             user_summary = insert_data["user_summary"]
             keyword_out = gc.keywords_extraction(user_summary, 3)
             for word_score in keyword_out:
                 keyword_list.append(word_score['word'])
             insert_data['summary_keyword'] = '|'.join(keyword_list)
         except:
             insert_data['summary_keyword'] = ''
-    # 当前只对本品进行情感打分
-    # if select_table in post_list and insert_data["brand_id"] == 45:
-    #     text_all = ''
-    #     if (insert_data["post_content"] is not None) and insert_data["post_content"] != '':
-    #         text_all += insert_data["post_content"]
-    #     if (insert_data["post_subject"] is not None) and insert_data["post_subject"] != '':
-    #         text_all += insert_data["post_subject"]
-    #     emo_score, emo_pn = gc.calculate_emotion_score(text_all)
-    #     insert_data['emo_score_neg'] = round(1 - emo_score, 2)
-    #     insert_data['emo_score_pos'] = round(emo_score, 2)
-    #     insert_data['emo_pn'] = emo_pn
-    # # comment因为架构很难改，所以暂时是对所有的文本做情感分析，有可能造成接口调用次数超过20000
-    # if select_table in cmt_list:
-    #     text_all = ''
-    #     if (insert_data["comment_content"] is not None) and insert_data["comment_content"] != '':
-    #         text_all += insert_data["comment_content"]
-    #     emo_score, emo_pn = gc.calculate_emotion_score(text_all)
-    #     insert_data['emo_score_neg'] = round(1 - emo_score, 2)
-    #     insert_data['emo_score_pos'] = round(emo_score, 2)
-    #     insert_data['emo_pn'] = emo_pn
+    # 对于实时化的插入，需要直接对一些需要实时处理的字段进行插入
+    if insert_mode == 'realtime':
+        text_all = ''
+        if select_table in post_list :
+            if (insert_data["post_content"] is not None) and insert_data["post_content"] != '':
+                text_all += insert_data["post_content"]
+            if (insert_data["post_subject"] is not None) and insert_data["post_subject"] != '':
+                text_all += insert_data["post_subject"]
+        if select_table in cmt_list:
+            if (insert_data["comment_content"] is not None) and insert_data["comment_content"] != '':
+                text_all += insert_data["comment_content"]
+        emo_score, emo_pn = gc.calculate_emotion_score(text_all)
+        insert_data['emo_score_neg'] = round(1 - emo_score, 2)
+        insert_data['emo_score_pos'] = round(emo_score, 2)
+        insert_data['emo_pn'] = emo_pn
     # 写入数据库
     keys = ", ".join(insert_data.keys())
     values = ", ".join(['%s'] * len(insert_data.keys()))
     if cover_flag:
         insert_sql = '''INSERT INTO {table}({keys}) VALUES ({values}) ON DUPLICATE KEY UPDATE'''.format(table=insert_table,
                                                                                                         keys=keys,
                                                                                                         values=values)
@@ -1070,15 +1116,15 @@
         for (k, v) in data.items():
             try:
                 if np.isnan(data[k]):
                     data[k] = None
             except:
                 continue
         try:
-            insert_json_sql(data, insert_ip, insert_tbl, select_tbl, cover_flag=True)
+            insert_json_sql2etl(data, insert_ip, insert_tbl, select_tbl, cover_flag=True)
         except:
             print('数据插入失败：', data)
 
 def mysql_transmit_data(select_ip, insert_ip, select_tbl, start_datetime, end_datetime, cover_flag):
     insert_tbl = insert_map_detail[select_tbl][0]
     print(f'\n-----当前将{select_tbl}导入{insert_tbl}中-----')
     res = select_sql_json(select_ip, select_tbl, start_datetime, end_datetime)
@@ -1089,10 +1135,10 @@
             for (k, v) in data.items():
                 try:
                     if np.isnan(data[k]):
                         data[k] = None
                 except:
                     continue
             try:
-                insert_json_sql(data, insert_ip, insert_tbl, select_tbl, cover_flag)
+                insert_json_sql2etl(data, insert_ip, insert_tbl, select_tbl, cover_flag)
             except:
                 print('数据插入失败：', data)
```

### Comparing `general_calculator_zsd-1.2.1/setup.py` & `general_calculator_zsd-1.2.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='general_calculator_zsd',
-    version='1.2.1',
+    version='1.2.2',
     author='colin zhang',
     author_email='zsd0830@163.com',
-    description='通用脚本及数据导入脚本，不定期按需更新。',
+    description='通用脚本及数据导入脚本，不定期按需更新。1.2.2-加入抖音数据导入；加入实时监测的情感识别。',
     long_description_content_type="""text/markdown""",
     url='',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

