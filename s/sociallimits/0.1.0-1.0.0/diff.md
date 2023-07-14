# Comparing `tmp/sociallimits-0.1.0-py3-none-any.whl.zip` & `tmp/sociallimits-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2593 bytes, number of entries: 6
--rw-r--r--  2.0 unx      548 b- defN 23-Jul-12 04:39 sociallimits/__init__.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-12 04:39 sociallimits-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      939 b- defN 23-Jul-12 04:39 sociallimits-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 04:39 sociallimits-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Jul-12 04:39 sociallimits-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      490 b- defN 23-Jul-12 04:39 sociallimits-0.1.0.dist-info/RECORD
-6 files, 3151 bytes uncompressed, 1699 bytes compressed:  46.1%
+Zip file size: 2592 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      582 b- defN 23-Jul-14 04:04 sociallimits/__init__.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-14 04:04 sociallimits-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      939 b- defN 23-Jul-14 04:04 sociallimits-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 04:04 sociallimits-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Jul-14 04:04 sociallimits-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      490 b- defN 23-Jul-14 04:04 sociallimits-1.0.0.dist-info/RECORD
+6 files, 3185 bytes uncompressed, 1698 bytes compressed:  46.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: sociallimits/__init__.py
 Comment: 
 
-Filename: sociallimits-0.1.0.dist-info/LICENSE
+Filename: sociallimits-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: sociallimits-0.1.0.dist-info/METADATA
+Filename: sociallimits-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: sociallimits-0.1.0.dist-info/WHEEL
+Filename: sociallimits-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: sociallimits-0.1.0.dist-info/top_level.txt
+Filename: sociallimits-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: sociallimits-0.1.0.dist-info/RECORD
+Filename: sociallimits-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sociallimits/__init__.py

```diff
@@ -1,19 +1,19 @@
-__version__ = "0.1.0"
+__version__ = "1.0.0"
 
 
 class SocialPlatform:
     def __init__(self, caption_limit=None, tag_limit=None):
         self.caption_limit = caption_limit
         self.tag_limit = tag_limit
 
 
 all_platforms = {
     "FACEBOOK": SocialPlatform(caption_limit=2200),
-    "INSTAGRAM": SocialPlatform(tag_limit=30),
-    "PINTEREST": SocialPlatform(caption_limit=2200),
+    "INSTAGRAM": SocialPlatform(caption_limit=2200, tag_limit=30),
+    "PINTEREST": SocialPlatform(caption_limit=2200, tag_limit=20),
     "TUMBLR": SocialPlatform(caption_limit=2200, tag_limit=20),
     "TWITTER": SocialPlatform(caption_limit=280),
 }
 
 for name, platform in all_platforms.items():
     locals()[name] = platform
```

## Comparing `sociallimits-0.1.0.dist-info/LICENSE` & `sociallimits-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sociallimits-0.1.0.dist-info/METADATA` & `sociallimits-1.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sociallimits
-Version: 0.1.0
+Version: 1.0.0
 Summary: Various limits on different social media platforms
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/sociallimits
 Keywords: sociallimits,social,limits,media,platform
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

