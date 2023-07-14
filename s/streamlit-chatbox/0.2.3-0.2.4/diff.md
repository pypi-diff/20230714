# Comparing `tmp/streamlit_chatbox-0.2.3-py3-none-any.whl.zip` & `tmp/streamlit_chatbox-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5106 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    10021 b- defN 23-Jul-13 08:41 streamlit_chatbox/__init__.py
--rw-rw-rw-  2.0 fat     2607 b- defN 23-Jul-13 09:14 streamlit_chatbox-0.2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 09:14 streamlit_chatbox-0.2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-13 09:14 streamlit_chatbox-0.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      425 b- defN 23-Jul-13 09:14 streamlit_chatbox-0.2.3.dist-info/RECORD
-5 files, 13163 bytes uncompressed, 4310 bytes compressed:  67.3%
+Zip file size: 5159 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    10140 b- defN 23-Jul-14 03:34 streamlit_chatbox/__init__.py
+-rw-rw-rw-  2.0 fat     2607 b- defN 23-Jul-14 03:35 streamlit_chatbox-0.2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 03:35 streamlit_chatbox-0.2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-14 03:35 streamlit_chatbox-0.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      425 b- defN 23-Jul-14 03:35 streamlit_chatbox-0.2.4.dist-info/RECORD
+5 files, 13282 bytes uncompressed, 4363 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: streamlit_chatbox/__init__.py
 Comment: 
 
-Filename: streamlit_chatbox-0.2.3.dist-info/METADATA
+Filename: streamlit_chatbox-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_chatbox-0.2.3.dist-info/WHEEL
+Filename: streamlit_chatbox-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_chatbox-0.2.3.dist-info/top_level.txt
+Filename: streamlit_chatbox-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_chatbox-0.2.3.dist-info/RECORD
+Filename: streamlit_chatbox-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_chatbox/__init__.py

```diff
@@ -173,19 +173,21 @@
                                         bg_color=bg_color,
 
                                         )
                 if not msg['is_user']:
                     self.last_response = empty
         return self.last_response
 
-    def update_last_box_text(self, msg):
+    def update_last_box_text(self, msg, cursor_pos="\n\n<details>"):
         if self.last_response is not None:
             self.history[-1]['content'] = msg
+            if cursor_pos:
+                msg = msg.replace(cursor_pos, " ▌" + cursor_pos, 1)
             self.last_response.markdown(
-                self.format_md(msg + '▌', False),
+                self.format_md(msg, False),
                 unsafe_allow_html=True
             )
 
     def robot_stream(self, msg, init_msg='', words_per_sec=10, max_seconds=10):
         step = max(words_per_sec, len(msg) // max_seconds + 1) // 5 + 1
         self.robot_say(init_msg)
         self.output_messages()
```

## Comparing `streamlit_chatbox-0.2.3.dist-info/METADATA` & `streamlit_chatbox-0.2.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chatbox
-Version: 0.2.3
+Version: 0.2.4
 Summary: A chat box used in streamlit
 Home-page: https://github.com/liunux4odoo/streamlit-chatbox
 Author: liunux
 Author-email: liunux@qq.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit
```

