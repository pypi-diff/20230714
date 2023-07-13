# Comparing `tmp/visionscript-0.0.3.tar.gz` & `tmp/visionscript-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionscript-0.0.3.tar", last modified: Mon Jul 10 18:00:26 2023, max compression
+gzip compressed data, was "visionscript-0.0.4.tar", last modified: Thu Jul 13 23:34:30 2023, max compression
```

## Comparing `visionscript-0.0.3.tar` & `visionscript-0.0.4.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-10 18:00:26.172846 visionscript-0.0.3/
--rw-r--r--   0 james      (501) staff       (20)     3167 2023-07-10 10:58:12.000000 visionscript-0.0.3/.gitignore
--rw-r--r--   0 james      (501) staff       (20)      188 2023-07-08 12:17:56.000000 visionscript-0.0.3/CITATION.cff
--rw-r--r--   0 james      (501) staff       (20)       16 2023-07-06 16:15:17.000000 visionscript-0.0.3/CNAME
--rw-r--r--   0 james      (501) staff       (20)     6604 2023-07-10 14:58:55.000000 visionscript-0.0.3/CONTRIBUTING.md
--rw-r--r--   0 james      (501) staff       (20)       41 2023-07-06 23:02:16.000000 visionscript-0.0.3/CONTRIBUTORS.md
--rw-r--r--   0 james      (501) staff       (20)     1056 2023-07-06 08:06:43.000000 visionscript-0.0.3/LICENSE
--rw-r--r--   0 james      (501) staff       (20)       24 2023-07-06 16:15:17.000000 visionscript-0.0.3/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)      297 2023-07-09 16:59:36.000000 visionscript-0.0.3/Makefile
--rw-r--r--   0 james      (501) staff       (20)     5384 2023-07-10 18:00:26.172622 visionscript-0.0.3/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     4867 2023-07-10 15:17:12.000000 visionscript-0.0.3/README.md
--rw-r--r--   0 james      (501) staff       (20)      288 2023-07-10 18:00:18.000000 visionscript-0.0.3/requirements.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-07-10 18:00:26.172910 visionscript-0.0.3/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1757 2023-07-10 12:24:17.000000 visionscript-0.0.3/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-10 18:00:26.165012 visionscript-0.0.3/tests/
--rw-r--r--   0 james      (501) staff       (20)     6148 2023-07-08 07:38:48.000000 visionscript-0.0.3/tests/.DS_Store
--rw-r--r--   0 james      (501) staff       (20)       53 2023-07-08 06:32:08.000000 visionscript-0.0.3/tests/classify_image.vic
--rw-r--r--   0 james      (501) staff       (20)       46 2023-07-06 23:35:58.000000 visionscript-0.0.3/tests/find_in_images.vic
--rw-r--r--   0 james      (501) staff       (20)       63 2023-07-08 06:31:57.000000 visionscript-0.0.3/tests/load_detect_save.vic
--rw-r--r--   0 james      (501) staff       (20)       97 2023-07-08 06:31:57.000000 visionscript-0.0.3/tests/replace_in_images.vic
--rw-r--r--   0 james      (501) staff       (20)       49 2023-07-08 06:32:08.000000 visionscript-0.0.3/tests/segment_image.vic
--rw-r--r--   0 james      (501) staff       (20)      602 2023-07-08 07:07:01.000000 visionscript-0.0.3/tests/test.py
--rw-r--r--   0 james      (501) staff       (20)       31 2023-07-06 23:35:53.000000 visionscript-0.0.3/tests/train_od.vic
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-10 18:00:26.167714 visionscript-0.0.3/visionscript/
--rw-r--r--   0 james      (501) staff       (20)     6148 2023-07-09 13:30:07.000000 visionscript-0.0.3/visionscript/.DS_Store
--rw-r--r--   0 james      (501) staff       (20)       55 2023-07-10 12:28:10.000000 visionscript-0.0.3/visionscript/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     3343 2023-07-10 17:51:02.000000 visionscript-0.0.3/visionscript/cloud.py
--rw-r--r--   0 james      (501) staff       (20)     3310 2023-07-10 13:00:15.000000 visionscript-0.0.3/visionscript/grammar.py
--rw-r--r--   0 james      (501) staff       (20)    45539 2023-07-10 17:09:28.000000 visionscript-0.0.3/visionscript/lang.py
--rw-r--r--   0 james      (501) staff       (20)     5753 2023-07-10 16:54:18.000000 visionscript-0.0.3/visionscript/notebook.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-10 18:00:26.170948 visionscript-0.0.3/visionscript/static/
--rw-r--r--   0 james      (501) staff       (20)     6148 2023-07-09 09:24:19.000000 visionscript-0.0.3/visionscript/static/.DS_Store
--rw-r--r--   0 james      (501) staff       (20)      814 2023-07-09 23:12:47.000000 visionscript-0.0.3/visionscript/static/examples.js
--rw-r--r--   0 james      (501) staff       (20)     7404 2023-07-10 08:38:39.000000 visionscript-0.0.3/visionscript/static/functions.js
--rw-r--r--   0 james      (501) staff       (20)    31429 2023-07-10 16:49:09.000000 visionscript-0.0.3/visionscript/static/main.js
--rw-r--r--   0 james      (501) staff       (20)     6645 2023-07-10 12:14:12.000000 visionscript-0.0.3/visionscript/static/styles.css
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-10 18:00:26.172152 visionscript-0.0.3/visionscript/templates/
--rw-r--r--   0 james      (501) staff       (20)     3583 2023-07-08 11:14:46.000000 visionscript-0.0.3/visionscript/templates/deployintro.html
--rw-r--r--   0 james      (501) staff       (20)     4574 2023-07-08 11:22:00.000000 visionscript-0.0.3/visionscript/templates/index.html
--rw-r--r--   0 james      (501) staff       (20)     4505 2023-07-10 12:18:15.000000 visionscript-0.0.3/visionscript/templates/notebook.html
--rw-r--r--   0 james      (501) staff       (20)     2216 2023-07-08 10:29:01.000000 visionscript-0.0.3/visionscript/usage.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-10 18:00:26.168923 visionscript-0.0.3/visionscript.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     5384 2023-07-10 18:00:26.000000 visionscript-0.0.3/visionscript.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      949 2023-07-10 18:00:26.000000 visionscript-0.0.3/visionscript.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-07-10 18:00:26.000000 visionscript-0.0.3/visionscript.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       56 2023-07-10 18:00:26.000000 visionscript-0.0.3/visionscript.egg-info/entry_points.txt
--rw-r--r--   0 james      (501) staff       (20)      294 2023-07-10 18:00:26.000000 visionscript-0.0.3/visionscript.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       13 2023-07-10 18:00:26.000000 visionscript-0.0.3/visionscript.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-13 23:34:30.428402 visionscript-0.0.4/
+-rw-r--r--   0 james      (501) staff       (20)     3134 2023-07-13 09:45:59.000000 visionscript-0.0.4/.gitignore
+-rw-r--r--   0 james      (501) staff       (20)      188 2023-07-08 12:17:56.000000 visionscript-0.0.4/CITATION.cff
+-rw-r--r--   0 james      (501) staff       (20)     6604 2023-07-10 14:58:55.000000 visionscript-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0 james      (501) staff       (20)       41 2023-07-06 23:02:16.000000 visionscript-0.0.4/CONTRIBUTORS.md
+-rw-r--r--   0 james      (501) staff       (20)     1056 2023-07-06 08:06:43.000000 visionscript-0.0.4/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)       24 2023-07-06 16:15:17.000000 visionscript-0.0.4/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)      297 2023-07-09 16:59:36.000000 visionscript-0.0.4/Makefile
+-rw-r--r--   0 james      (501) staff       (20)     5384 2023-07-13 23:34:30.428180 visionscript-0.0.4/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     4867 2023-07-10 15:17:12.000000 visionscript-0.0.4/README.md
+-rw-r--r--   0 james      (501) staff       (20)      307 2023-07-13 23:34:23.000000 visionscript-0.0.4/requirements.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-07-13 23:34:30.428455 visionscript-0.0.4/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1757 2023-07-13 09:45:59.000000 visionscript-0.0.4/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-13 23:34:30.420975 visionscript-0.0.4/tests/
+-rw-r--r--   0 james      (501) staff       (20)     6148 2023-07-08 07:38:48.000000 visionscript-0.0.4/tests/.DS_Store
+-rw-r--r--   0 james      (501) staff       (20)       53 2023-07-08 06:32:08.000000 visionscript-0.0.4/tests/classify_image.vic
+-rw-r--r--   0 james      (501) staff       (20)       46 2023-07-06 23:35:58.000000 visionscript-0.0.4/tests/find_in_images.vic
+-rw-r--r--   0 james      (501) staff       (20)       63 2023-07-08 06:31:57.000000 visionscript-0.0.4/tests/load_detect_save.vic
+-rw-r--r--   0 james      (501) staff       (20)       97 2023-07-08 06:31:57.000000 visionscript-0.0.4/tests/replace_in_images.vic
+-rw-r--r--   0 james      (501) staff       (20)       49 2023-07-08 06:32:08.000000 visionscript-0.0.4/tests/segment_image.vic
+-rw-r--r--   0 james      (501) staff       (20)      602 2023-07-08 07:07:01.000000 visionscript-0.0.4/tests/test.py
+-rw-r--r--   0 james      (501) staff       (20)       31 2023-07-06 23:35:53.000000 visionscript-0.0.4/tests/train_od.vic
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-13 23:34:30.423774 visionscript-0.0.4/visionscript/
+-rw-r--r--   0 james      (501) staff       (20)     6148 2023-07-09 13:30:07.000000 visionscript-0.0.4/visionscript/.DS_Store
+-rw-r--r--   0 james      (501) staff       (20)       55 2023-07-13 23:30:37.000000 visionscript-0.0.4/visionscript/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     6557 2023-07-13 21:14:41.000000 visionscript-0.0.4/visionscript/cloud.py
+-rw-r--r--   0 james      (501) staff       (20)     3634 2023-07-13 09:46:01.000000 visionscript-0.0.4/visionscript/grammar.py
+-rw-r--r--   0 james      (501) staff       (20)    51395 2023-07-13 23:10:12.000000 visionscript-0.0.4/visionscript/lang.py
+-rw-r--r--   0 james      (501) staff       (20)     8508 2023-07-13 22:46:20.000000 visionscript-0.0.4/visionscript/notebook.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-13 23:34:30.426705 visionscript-0.0.4/visionscript/static/
+-rw-r--r--   0 james      (501) staff       (20)     6148 2023-07-09 09:24:19.000000 visionscript-0.0.4/visionscript/static/.DS_Store
+-rw-r--r--   0 james      (501) staff       (20)      814 2023-07-09 23:12:47.000000 visionscript-0.0.4/visionscript/static/examples.js
+-rw-r--r--   0 james      (501) staff       (20)     7659 2023-07-13 09:46:01.000000 visionscript-0.0.4/visionscript/static/functions.js
+-rw-r--r--   0 james      (501) staff       (20)    31728 2023-07-13 23:25:57.000000 visionscript-0.0.4/visionscript/static/main.js
+-rw-r--r--   0 james      (501) staff       (20)     7442 2023-07-13 23:28:42.000000 visionscript-0.0.4/visionscript/static/styles.css
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-13 23:34:30.427778 visionscript-0.0.4/visionscript/templates/
+-rw-r--r--   0 james      (501) staff       (20)     4183 2023-07-13 09:46:01.000000 visionscript-0.0.4/visionscript/templates/deployintro.html
+-rw-r--r--   0 james      (501) staff       (20)     1326 2023-07-13 12:56:59.000000 visionscript-0.0.4/visionscript/templates/index.html
+-rw-r--r--   0 james      (501) staff       (20)     7290 2023-07-13 21:47:55.000000 visionscript-0.0.4/visionscript/templates/notebook.html
+-rw-r--r--   0 james      (501) staff       (20)     2216 2023-07-08 10:29:01.000000 visionscript-0.0.4/visionscript/usage.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-13 23:34:30.424920 visionscript-0.0.4/visionscript.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     5384 2023-07-13 23:34:30.000000 visionscript-0.0.4/visionscript.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      943 2023-07-13 23:34:30.000000 visionscript-0.0.4/visionscript.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-07-13 23:34:30.000000 visionscript-0.0.4/visionscript.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       56 2023-07-13 23:34:30.000000 visionscript-0.0.4/visionscript.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)      313 2023-07-13 23:34:30.000000 visionscript-0.0.4/visionscript.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       13 2023-07-13 23:34:30.000000 visionscript-0.0.4/visionscript.egg-info/top_level.txt
```

### Comparing `visionscript-0.0.3/.gitignore` & `visionscript-0.0.4/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -163,10 +163,8 @@
 *.jpg
 folder
 *.pt
 *.vic
 *.json
 tmp/*
 runs/*
-*.svg
-FastSAM/*
-visionscrtip/FastSAM/*
+*.svg
```

### Comparing `visionscript-0.0.3/CONTRIBUTING.md` & `visionscript-0.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.3/LICENSE` & `visionscript-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.3/PKG-INFO` & `visionscript-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionscript
-Version: 0.0.3
+Version: 0.0.4
 Summary: VisionScript is an abstract programming language for doing common computer vision tasks, fast.
 Home-page: https://github.com/capjamesg/visionscript
 Author: capjamesg
 Author-email: jamesg@jamesg.blog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `visionscript-0.0.3/README.md` & `visionscript-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.3/setup.py` & `visionscript-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.3/tests/.DS_Store` & `visionscript-0.0.4/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.3/tests/test.py` & `visionscript-0.0.4/tests/test.py`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.3/visionscript/.DS_Store` & `visionscript-0.0.4/visionscript/.DS_Store`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.3/visionscript/grammar.py` & `visionscript-0.0.4/visionscript/grammar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 grammar = """
 start: (expr | EOL | EOF | " ")*
 
-expr: (if | in | train | label | detect | countinregion | help | list | get | exit | read | compare | count | cutout | show | size | caption | say | save | load | use | replace | var | classify | segment | comment | contains | if | else | end | make | run | isita | find | describe | import | rotate | getcolours | getcolors | get_text | greyscale | select | paste | pasterandom | resize | blur | literal | setbrightness | search | similarity | readqr | reset | negate | BOOL | INT | equality | not_equality | input | deploy | getedges | setconfidence)
+expr: (if | in | train | label | detect | countinregion | help | list | get | exit | read | compare | count | cutout | show | size | caption | say | save | load | use | replace | var | classify | segment | comment | contains | if | else | end | make | run | isita | find | describe | import | rotate | getcolours | getcolors | get_text | greyscale | select | paste | pasterandom | resize | blur | literal | setbrightness | search | similarity | readqr | reset | negate | BOOL | INT | equality | not_equality | input | deploy | getedges | setconfidence | setregion | filterbyclass)
 classify: "Classify" "[" STRING ("," STRING)* "]"
 var: variable "=" expr
 replace: "Replace" "[" STRING "]"
 use: "Use" "[" STRING "]"
 load: "Load" "[" (STRING | input) "]" | "Load" ("[" "]")?
 save: "Save" "[" STRING "]"
 say: "Say" "[" STRING "]" | "Say" ("[" "]")?
 get_text: "GetText" ("[" "]")?
 greyscale: "Greyscale" ("[" "]")?
 search: "Search" "[" STRING "]"
 deploy: "Deploy" "[" STRING "]"
 getedges: "GetEdges"  ("[" "]")?
+filterbyclass: "FilterByClass" "[" STRING ("," STRING)* "]" | "FilterByClass" ("[" "]")?
 describe: "Describe" ("[" "]")?
+setregion: "SetRegion" "[" INT "," INT "," INT "," INT "]" | "SetRegion" ("[" "]")?
 readqr: "ReadQR" ("[" "]")?
-setconfidence: "SetConfidence" "[" INT "]"
+setconfidence: "SetConfidence" "[" FLOAT "]" | "SetConfidence" ("[" "]")?
 rotate: "Rotate" "[" (INT | STRING) "]"
 resize: "Resize" "[" INT "," INT "]"
 getcolors: "GetColors" ("[" "]")? | "GetColors" "[" INT "]"
 getcolours: "GetColours" ("[" "]")? | "GetColours" "[" INT "]"
 isita: "Is it a " (("," STRING)* | ("or" STRING)*)? EOL
 find: "Find" "[" STRING "]"
-args: ((STRING | INT | expr) ("," (STRING | INT | expr))*) | (STRING | INT | expr)?
+args: ((STRING | INT | FLOAT | expr) ("," (STRING | INT | FLOAT | expr))*) | (STRING | INT | FLOAT | expr)?
 make: "Make" literal ("[" args "]")? EOL (INDENT expr+)* EOL
 caption: "Caption" ("[" "]")?
 size: "Size" ("[" "]")?
 import: "Import" "[" STRING "]"
 run: "Run" "[" STRING "]"
 show: "Show" ("[" "]")?
 select: "Select" ("[" "]")? | "Select" "[" INT "]"
@@ -38,37 +40,38 @@
 input: "Input" ("[" STRING "]")?
 contains: "Contains" "[" STRING "]"
 compare: "Compare" ("[" "]")?
 setbrightness: "SetBrightness" "[" INT "]"
 read: "Read" ("[" "]")?
 exit: "Exit" ("[" "]")?
 blur: "Blur" ("[" "]")?
-similarity: "Similarity" ("[" INT "]")?
+similarity: "Similarity" ("[" (INT | FLOAT) "]")?
 get: "Get" "[" INT "]" EOL
 list: "[" ((STRING | INT | expr) "," | (STRING | INT | expr) )* "]" EOL
 help: "Help" "[" STRING "]"
 end: "End" ("[" "]")?
 countinregion: "CountInRegion" "[" INT "," INT "," INT "," INT "]"
 detect: "Detect" "[" input "]" | "Detect" "[" STRING ("," STRING)* "]" | "Detect" ("[" "]")?
 segment: "Segment" "[" STRING "]"
 else: "Else"
 in: "In" "[" STRING "]" EOL (INDENT expr+)* EOL 
 if: "If" "[" (expr+)* "]" EOL (INDENT expr+)* (EOL | EOF) (else EOL (INDENT expr+)* (EOL | EOF | " "))?
 reset: "Reset" ("[" "]")?
 negate: "Not" "[" expr "]"
 OPERAND: "+" | "-" | "*" | "/"
-equality: (INT | STRING | expr) "==" (INT | STRING | expr)
+equality: (INT | STRING | expr | FLOAT) "==" (INT | STRING | expr | FLOAT)
 not_equality: (INT | STRING | expr) "!=" (INT | STRING | expr)
 train: "Train" "[" STRING "," STRING "]" | "Train" "[" STRING "]"
 label: "Label" "[" STRING "," STRING ("," STRING )*  "]"
-literal: /([a-z][a-zA-Z0-9_]*)/ ( "[" (STRING | INT | expr) ("," (STRING | INT | expr))* "]" )? | /([a-z][a-zA-Z0-9_]*)/ "[" "]"
+literal: /([a-z][a-zA-Z0-9_]*)/ ( "[" (STRING | INT | FLOAT | expr) ("," (STRING | INT | FLOAT | expr))* "]" )? | /([a-z][a-zA-Z0-9_]*)/ "[" "]"
 variable: /[a-zA-Z_][a-zA-Z0-9_]*/
-comment: "#"
+comment: /#.*?\\n/
 EOL: "\\n"
 EOF: "\\Z"
 INT: /-?\d+/
+FLOAT: /-?\d+\.\d+/
 INDENT: "    " | "\\t"
 BOOL: "True" | "False"
 %import common.ESCAPED_STRING -> STRING
 %import common.WS_INLINE
 %ignore WS_INLINE
 """
```

### Comparing `visionscript-0.0.3/visionscript/lang.py` & `visionscript-0.0.4/visionscript/lang.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,28 +8,33 @@
 import math
 import mimetypes
 import os
 import random
 import string
 import sys
 import tempfile
+import time
 
 import click
 import cv2
 import lark
 import numpy as np
 import supervision as sv
+import torch
 from lark import Lark, UnexpectedCharacters, UnexpectedToken
 from PIL import Image
 from spellchecker import SpellChecker
 
 from visionscript.grammar import grammar
 from visionscript.usage import (USAGE, language_grammar_reference,
                                 lowercase_language_grammar_reference)
 
+DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
+MAX_FILE_SIZE = 10000000  # 10MB
+
 spell = SpellChecker()
 
 parser = Lark(grammar)
 
 SUPPORTED_INFERENCE_MODELS = {
     "classify": {
         "clip": "clip",
@@ -40,14 +45,18 @@
 
 SUPPORTED_TRAIN_MODELS = {
     "classify": {"vit": "autodistill_vit"},
     "detect": {"yolov8": "autodistill_yolov8"},
 }
 
 
+class InputNotProvided:
+    pass
+
+
 def handle_unexpected_characters(e, code):
     # raise error if class doesn't exist
     line = e.line
     column = e.column
 
     # check if function name in grammar
     function_name = code.strip().split("\n")[line - 1].split("[")[0].strip()
@@ -134,21 +143,24 @@
         "history": [],
         "search_index_stack": [],
         # "current_active_model": None,
         "output": None,
         "input_variables": {},
         "last_classes": [],
         "confidence": 50,
+        "active_region": None,
+        "active_filters": {"class": None, "region": None},
     }
 
 
 class VisionScript:
     """
     A VisionScript program.
     """
+
     def __init__(self, notebook=False):
         self.state = init_state()
         self.notebook = notebook
         self.code = ""
 
         self.function_calls = {
             "load": lambda x: self.load(x),
@@ -199,23 +211,44 @@
             "reset": lambda x: self.reset(x),
             "negate": lambda x: self.negate(x),
             "equality": lambda x: self.equality(x),
             "not_equality": lambda x: not self.equality(x),
             "input": lambda x: self.input_(x),
             "deploy": lambda x: self.deploy(x),
             "getedges": lambda x: self.get_edges(x),
+            "setregion": lambda x: self.set_region(x),
+            "setconfidence": lambda x: self.set_confidence(x),
+            "filterbyclass": lambda x: self.filter_by_class(x),
         }
 
+    def filter_by_class(self, args):
+        """
+        Filter detections by class.
+        """
+        if len(args) == 0:
+            self.state["active_filters"] = None
+        elif self.state["active_filters"].get("class") is None:
+            self.state["active_filters"]["class"] = args
+
+    def set_region(self, args):
+        if len(args) == 0:
+            self.state["active_filters"]["region"] = None
+            return
+
+        x0, y0, x1, y1 = args
+
+        self.state["active_filters"]["region"] = (x0, y0, x1, y1)
+
     def input_(self, key):
-        self.state["input_variables"][key] = "image"
-        if self.state.get(literal_eval(key)) is not None:
-            return self.state[literal_eval(key)]
+        if self.state["input_variables"].get(literal_eval(key)) is not None:
+            return self.state["input_variables"][literal_eval(key)]
         else:
-            print(f"Input {key} does not exist.")
-            exit()
+            return InputNotProvided()
+            # print(f"Input {key} does not exist.")
+            # exit()
 
     def equality(self, args):
         return args[0] == args[1]
 
     def negate(self, expr):
         return not expr
 
@@ -231,19 +264,26 @@
         """
         function_name = args[0].children[0].value.strip()
 
         function_body = lark.Tree("expr", args[1:])
 
         self.state["functions"][function_name] = function_body
 
-    def set_confidence(self, args):
+    def set_confidence(self, confidence):
         """
         Set the confidence level for use in filtering detections.
         """
-        self.state["confidence"] = args[0]
+        if not confidence:
+            confidence = 50
+
+        if confidence > 100 or confidence < 0:
+            print("Confidence must be between 0 and 100.")
+            return
+
+        self.state["confidence"] = confidence
 
     def load(self, filename):
         """
         Load an image or folder of images into state.
         """
         import requests
         import validators
@@ -266,15 +306,43 @@
 
             for image_filename in image_filenames:
                 self.load(image_filename)
 
             return
 
         if filename and validators.url(filename):
-            response = requests.get(filename)
+            try:
+                response = requests.get(filename, timeout=5, stream=True)
+            except requests.exceptions.ConnectionError:
+                self.state["last"] = "Could not connect to URL."
+                return
+            except requests.exceptions.ReadTimeout:
+                self.state["last"] = "Timeout."
+                return
+            except:
+                self.state["last"] = "There was an error loading the image."
+                return
+
+            # check length
+            if len(response.content) > MAX_FILE_SIZE:
+                self.state["last"] = "Image too large."
+                return
+
+            size = 0
+            start = time.time()
+
+            for chunk in response.iter_content(1024):
+                if time.time() - start > 5:
+                    raise ValueError("timeout reached")
+
+                size += len(chunk)
+
+                if size > MAX_FILE_SIZE:
+                    raise ValueError("response too large")
+
             file_extension = mimetypes.guess_extension(response.headers["content-type"])
 
             # if not image, error
             if file_extension not in (".png", ".jpg", ".jpeg"):
                 print(f"File {filename} does not represent a png, jpg, or jpeg image.")
                 return None
 
@@ -299,15 +367,17 @@
 
         # filename = filename.split("/")[-1]
 
         # filename = secure_filename(filename)
 
         self.state["last_loaded_image_name"] = filename
 
-        return np.array(Image.open(filename).convert("RGB"))[:, :, ::-1]
+        self.state["output"] = {"image": Image.open(filename).convert("RGB")}
+
+        return np.array(Image.open(filename).convert("RGB"))  # [:, :, ::-1]
 
     def size(self, _):
         return self.state["image_stack"][-1].shape[:2]
 
     def import_(self, args):
         """
         Import a module from another file.
@@ -346,15 +416,15 @@
         if self.state.get("last_function_type", None) in (
             "detect",
             "segment",
             "classify",
         ):
             detections = self.state["last"]
 
-            detections = detections[detections.confidence > self.state["confidence"]]
+            detections = self._filter_controller(detections)
 
             if len(args) == 0:
                 self.state["last"] = detections
             else:
                 self.state["last"] = detections[args[0]]
 
     def paste(self, args):
@@ -391,40 +461,37 @@
 
     def search(self, label):
         """
         Search for an image using a text label or image.
 
         On first run, this will create an index of all images on the loaded image stack.
         """
-        # embed
         import clip
-        import torch
 
-        device = "cuda" if torch.cuda.is_available() else "cpu"
-        model, preprocess = clip.load("ViT-B/32", device=device)
+        model, preprocess = clip.load("ViT-B/32", device=DEVICE)
 
         with torch.no_grad():
             # if label is a filename, load image
             if os.path.exists(label):
-                comparator = preprocess(Image.open(label)).unsqueeze(0).to(device)
+                comparator = preprocess(Image.open(label)).unsqueeze(0).to(DEVICE)
 
                 comparator = model.encode_image(comparator)
             else:
-                comparator = clip.tokenize([label]).to(device)
+                comparator = clip.tokenize([label]).to(DEVICE)
 
                 comparator = model.encode_text(comparator)
 
             if len(self.state["search_index_stack"]) == 0:
                 self._create_index()
 
                 for image in self.state["image_stack"]:
                     # turn cv2 image into PIL image
                     image = Image.fromarray(image)
 
-                    processed_image = preprocess(image).unsqueeze(0).to(device)
+                    processed_image = preprocess(image).unsqueeze(0).to(DEVICE)
                     embedded_image = model.encode_image(processed_image)
 
                     self._add_to_index(embedded_image)
 
         index = self.state["search_index_stack"][-1]
 
         results = index.search(comparator, 5)
@@ -465,16 +532,30 @@
             self.state["image_stack"][-1], (x, y)
         )
 
     def save(self, filename):
         """
         Save an image to a file.
         """
+        if not os.path.exists("tmp"):
+            os.makedirs("tmp")
+
+        if not os.path.exists("tmp/output"):
+            os.makedirs("tmp/output")
+
+        if not filename:
+            filename = os.path.join(
+                "tmp/output/",
+                "".join(random.choice(string.ascii_letters) for _ in range(10)),
+            )
+
         self.state["image_stack"].save(filename)
 
+        self.state["output"] = {"text": "Saved to " + filename}
+
     def count(self, args):
         """
         Count the number of detections in a sv.Detections object.
         """
         if len(args) == 0:
             return len(self.state["last"].xyxy)
         else:
@@ -490,28 +571,28 @@
         # turn to bgr
         image = image[:, :, ::-1].copy()
         image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
         self.state["image_stack"].append(image)
         # save to test.png
 
         self.state["image_stack"].append(image)
-        self.state["output"] = image
+        self.state["output"] = {"image": image}
 
     def deploy(self, app_name):
         """
         Deploy a script to a VisionScript Cloud web app.
         """
         # make POST to http://localhost:6999/create
         import string
 
         import requests
 
         app_slug = app_name.translate(
             str.maketrans("", "", string.punctuation.replace("-", ""))
-        )
+        ).replace(" ", "-")
 
         response = requests.post(
             "http://localhost:6999/create",
             json={
                 "api_key": "test",
                 "title": app_name,
                 "slug": app_slug,
@@ -548,15 +629,15 @@
         elif args == 180:
             image = cv2.rotate(image, cv2.ROTATE_180)
         elif args == 270:
             image = cv2.rotate(image, cv2.ROTATE_90_COUNTERCLOCKWISE)
         else:
             image = image
 
-        self.state["output"] = image
+        self.state["output"] = {"image": image}
         self.state["image_stack"].append(image)
 
     def getcolours(self, k):
         """
         Get the most common colours in an image.
         """
         if not k:
@@ -581,21 +662,49 @@
 
         for center in centers:
             try:
                 human_readable_colours.append(
                     _get_colour_name((int(center[0]), int(center[1]), int(center[2])))
                 )
             except ValueError as e:
-                print(e)
                 continue
 
         self.state["last"] = human_readable_colours[:k]
 
         return human_readable_colours[:k]
 
+    def _filter_controller(self, detections):
+        results = detections
+
+        if self.state["active_filters"]["region"]:
+            x0, y0, x1, y1 = self.state["active_filters"]["region"]
+
+            zone = sv.PolygonZone(
+                np.array([[x0, y0], [x1, y0], [x1, y1], [x0, y1]]),
+                frame_resolution_wh=(
+                    self.state["last"].shape[1],
+                    self.state["last"].shape[0],
+                ),
+            )
+
+            results_filtered_by_active_region = zone.trigger(detections=results)
+
+            results = results[results_filtered_by_active_region]
+
+        if self.state["active_filters"]["class"]:
+            results = results[
+                np.isin(results.class_id, self.state["active_filters"]["class"])
+            ]
+
+        results = results[results.confidence > self.state["confidence"] / 100]
+
+        # self.state["last"] = results
+
+        return results
+
     def detect(self, classes):
         """
         Run object detection on an image.
         """
         logging.disable(logging.CRITICAL)
 
         if (
@@ -676,36 +785,34 @@
             model = self.state["model"]
 
             results = model.predict(image)
 
             return results
 
         import clip
-        import torch
 
-        device = "cuda" if torch.cuda.is_available() else "cpu"
-        model, preprocess = clip.load("ViT-B/32", device=device)
+        model, preprocess = clip.load("ViT-B/32", device=DEVICE)
 
         image = (
             preprocess(Image.open(self.state["last_loaded_image_name"]))
             .unsqueeze(0)
-            .to(device)
+            .to(DEVICE)
         )
-        text = clip.tokenize(labels).to(device)
+        text = clip.tokenize(labels).to(DEVICE)
 
         with torch.no_grad():
             logits_per_image, _ = model(image, text)
             probs = logits_per_image.softmax(dim=-1).cpu().numpy()
 
             # get idx of the most likely label class
             label_idx = probs.argmax()
 
             label_name = labels[label_idx]
 
-        self.state["output"] = label_name
+        self.state["output"] = {"text": label_name}
 
         return label_name
 
     def segment(self, text_prompt):
         """
         Apply image segmentation and generate segmentation masks.
         """
@@ -716,15 +823,14 @@
         # get current path
         import os
 
         current_path = os.getcwd()
 
         model = FastSAM(os.path.join(current_path, "weights", "FastSAM.pt"))
 
-        DEVICE = "cpu"
         everything_results = model(
             self.state["last_loaded_image_name"],
             device=DEVICE,
             retina_masks=True,
             imgsz=1024,
             conf=0.4,
             iou=0.9,
@@ -754,40 +860,18 @@
         detections = sv.Detections(
             mask=np.array([item.mask[0] for item in results]),
             xyxy=np.array([item.xyxy[0] for item in results]),
             class_id=np.array(class_ids),
             confidence=np.array([1]),
         )
 
-        detections = detections[detections.confidence > self.state["confidence"]]
-
         self.state["detections_stack"].append(detections)
 
         return detections
 
-    def countInRegion(self, x1, y1, x2, y2):
-        """
-        Count the number of detections in a region.
-        """
-        detections = self.state["last"]
-
-        detections = detections[detections.confidence > self.state["confidence"]]
-
-        xyxy = detections.xyxy
-
-        counter = 0
-
-        for i in range(len(xyxy)):
-            x1_, y1_, x2_, y2_ = xyxy[i]
-
-            if x1_ >= x1 and y1_ >= y1 and x2_ <= x2 and y2_ <= y2:
-                counter += 1
-
-        return counter
-
     def read(self, _):
         if self.state.get("last_function_type", None) in ("detect", "segment"):
             last_args = self.state["last_function_args"]
             statement = "".join(
                 [
                     f"{last_args[0]} {self.state['last'].confidence[i]:.2f} {self.state['last'].xyxy[i]}\n"
                     for i in range(len(self.state["last"].xyxy))
@@ -804,26 +888,30 @@
         in a notebook.
         """
         if isinstance(self.state["last"], np.ndarray):
             self.show(None)
             return
 
         if isinstance(self.state["last"], (list, tuple)):
-            self.state["output"] = ""
+            output = ""
+
             for item in self.state["last"]:
-                print(item)
                 # if list or tuple, join
                 if isinstance(item, (list, tuple)):
                     item = ", ".join([str(i) for i in item])
+                elif isinstance(item, int) or isinstance(item, float):
+                    item = str(item)
 
-                self.state["output"] += item + "\n"
+                output += item + "\n"
+
+            self.state["output"] = {"text": output}
 
             return
 
-        if isinstance(statement, int):
+        if isinstance(statement, int) or isinstance(statement, float):
             statement = str(statement)
 
         if statement and isinstance(statement, str):
             print(statement.strip())
             return
 
         if self.state.get("last_function_type", None) in ("detect", "segment"):
@@ -838,49 +926,72 @@
             statement = ", ".join([str(item) for item in self.state["last"]])
         else:
             statement = self.state["last"]
 
         if statement:
             print(statement.strip())
 
-        self.state["output"] = statement
+        self.state["output"] = {"text": statement}
 
     def blur(self, args):
         """
         Blur an image.
         """
         image = self.state["image_stack"][-1]
 
         image = cv2.blur(image, (args[0], args[0]))
 
         self.state["image_stack"].append(image)
 
-    def replace(self, color):
+    def replace(self, args):
         """
         Replace a detection or list of detections with an image or color.
         """
         detections = self.state["last"]
 
-        detections = detections[detections.confidence > self.state["confidence"]]
+        detections = self._filter_controller(detections)
 
         xyxy = detections.xyxy
 
-        if color is not None:
+        if os.path.exists(args):
+            print("Replacing with image.")
+            picture = cv2.imread(args)
+
+            # bgr to rgb
+            picture = picture[:, :, ::-1].copy()
+
+            image_at_top_of_stack = self.state["image_stack"][-1].copy()
+
+            for i in range(len(xyxy)):
+                x1, y1, x2, y2 = xyxy[i]
+
+                x1, y1, x2, y2 = int(x1), int(y1), int(x2), int(y2)
+
+                # resize picture to fit
+                picture = cv2.resize(picture, (x2 - x1, y2 - y1))
+
+                image_at_top_of_stack[y1:y2, x1:x2] = picture
+
+            self.state["image_stack"].append(image_at_top_of_stack)
+
+            return
+
+        color = args
+
+        if args is not None:
             import webcolors
 
             try:
                 color_to_rgb = webcolors.name_to_rgb(color)
             except ValueError:
                 print(f"Color {color} does not exist.")
                 return
 
             color_to_rgb = np.array(color_to_rgb)
 
-            print(color_to_rgb, xyxy)
-
             # convert to bgr
             color_to_rgb = color_to_rgb[::-1]
 
             for i in range(len(xyxy)):
                 x1, y1, x2, y2 = xyxy[i]
 
                 # cast all to int
@@ -971,15 +1082,15 @@
         self.greyscale(_)
 
         image = self.state["image_stack"][-1]
 
         sobelxy = cv2.Sobel(image, cv2.CV_64F, 1, 1, ksize=5)
 
         self.state["image_stack"].append(sobelxy)
-        self.state["output"] = sobelxy
+        self.state["output"] = {"image": sobelxy}
 
     def show(self, _):
         """
         Show the image in the notebook or in a new window.
 
         If a Detect or Segment function was run previously, this function shows the image with the bounding boxes.
         """
@@ -1006,14 +1117,15 @@
 
             grid_size = math.gcd(len(self.state["last"]), len(self.state["last"]))
 
             if len(self.state["last"]) == len(self.state["detections_stack"]):
                 for image, detections in zip(
                     self.state["last"], self.state["detections_stack"]
                 ):
+                    detections = self._filter_controller(self, detections)
                     if annotator and detections:
                         image = annotator.annotate(
                             np.array(image),
                             detections,
                             labels=self.state["last_classes"],
                         )
                     else:
@@ -1041,14 +1153,15 @@
             grid_size = math.gcd(
                 len(self.state["image_stack"]), len(self.state["image_stack"])
             )
 
             for image, detections in zip(
                 self.state["image_stack"], self.state["detections_stack"]
             ):
+                detections = self._filter_controller(self, detections)
                 if annotator and detections:
                     image = annotator.annotate(
                         np.array(image), detections, labels=self.state["last_classes"]
                     )
                 else:
                     image = np.array(image)
 
@@ -1064,15 +1177,15 @@
                 return
 
             # image = images[0]
 
         if annotator:
             image = annotator.annotate(
                 np.array(self.state["image_stack"][-1]),
-                detections=self.state["detections_stack"][-1],
+                detections=self._filter_controller(self.state["detections_stack"][-1]),
             )
         elif (
             self.state.get("last_loaded_image") is not None
             and not self.state.get("history", [])[-1] == "compare"
         ):
             image = self.state["image_stack"][-1]
         else:
@@ -1087,42 +1200,42 @@
             import matplotlib
 
             matplotlib.use("Agg")
             import matplotlib.pyplot as plt
 
             # show image
             if annotator:
-                print("annotator")
                 fig = plt.figure(figsize=(8, 8))
                 # if grey, show in grey
                 if len(image.shape) == 2:
                     plt.imshow(image, cmap="gray")
-                else:
-                    plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
+                # if bgr, show in rgb
+                elif image.shape[2] == 3:
+                    plt.imshow(image[:, :, ::-1])
 
                 fig.savefig(buffer, format="png")
                 buffer.seek(0)
 
                 image = Image.open(buffer)
 
                 img_str = {"image": base64.b64encode(buffer.getvalue()).decode("utf-8")}
 
-                self.state["output"] = img_str
+                self.state["output"] = {"image": img_str}
 
                 return
             else:
                 # if ndarray, convert to PIL
                 if isinstance(image, np.ndarray):
                     image = Image.fromarray(image)
                     # do bgr to rgb
-                    image = image.convert("RGB")
+                    # image = image.convert("RGB")
 
-                # convert to rgb if needed
-                if image.mode != "RGB":
-                    image = image.convert("RGB")
+                # # convert to rgb if needed
+                # if image.mode != "RGB":
+                #     image = image.convert("RGB")
 
                 # PIL to base64
                 buffered = io.BytesIO()
                 image.save(buffered, format="PNG")
                 img_str = base64.b64encode(buffered.getvalue()).decode("utf-8")
 
             self.state["output"] = {"image": img_str}
@@ -1142,24 +1255,21 @@
             n = 2
 
         if len(self.state["image_stack"]) < 2 or len(self.state["image_stack"]) < n:
             print("Not enough images to compare.")
             return
 
         import clip
-        import torch
-
-        device = "cuda" if torch.cuda.is_available() else "cpu"
 
-        model, preprocess = clip.load("ViT-B/32", device=device)
+        model, preprocess = clip.load("ViT-B/32", device=DEVICE)
 
         images = []
 
         for image in self.state["image_stack"][-n:]:
-            image = preprocess(Image.fromarray(image)).unsqueeze(0).to(device)
+            image = preprocess(Image.fromarray(image)).unsqueeze(0).to(DEVICE)
             images.append(image)
 
         embeddings = []
 
         with torch.no_grad():
             for image in images:
                 image = model.encode_image(image)
@@ -1204,40 +1314,55 @@
         v[v <= lim] += brightness
 
         final_hsv = cv2.merge((h, s, v))
 
         image = cv2.cvtColor(final_hsv, cv2.COLOR_HSV2BGR)
 
         self.state["image_stack"].append(image)
-        self.state["output"] = image
+        self.state["output"] = {"image": image}
 
     def contains(self, statement):
         """
         Check if a statement is contained in the last statement.
         """
         if isinstance(self.state["last"], str):
             return statement in self.state["last"]
         else:
             return False
 
+    def check_inputs(self, tree):
+        # get all INPUT tokens and save them to state
+        for node in tree.children:
+            # if node has children, recurse
+            if hasattr(node, "children") and len(node.children) > 0:
+                self.check_inputs(node)
+
+            if not hasattr(node, "data"):
+                continue
+
+            if node.data == "input":
+                self.state["input_variables"][node.children[0].value] = "image"
+
     def parse_tree(self, tree):
         """
         Abstract Syntax Tree (AST) parser for VisionScript.
         """
+
         if not hasattr(tree, "children"):
             if hasattr(tree, "value") and tree.value.isdigit():
                 return int(tree.value)
             elif isinstance(tree, str):
                 return literal_eval(tree)
+            elif hasattr(tree, "value") and tree.value.isfloat():
+                return float(tree.value)
 
         if hasattr(tree, "children") and tree.data == "input":
             return self.input_(tree.children[0].value)
 
         for node in tree.children:
-            print(node)
             if node == "True":
                 return True
             elif node == "False":
                 return False
             # if equality, check if equal
             # if rule is input
             elif hasattr(node, "data") and node.data == "equality":
@@ -1248,14 +1373,18 @@
                 return node
             elif hasattr(node, "data") and node.data == "list":
                 node = node
             elif (hasattr(node, "type") and node.type == "INT") or isinstance(
                 node, int
             ):
                 return int(node.value)
+            elif (hasattr(node, "type") and node.type == "FLOAT") or isinstance(
+                node, float
+            ):
+                return float(node.value)
             elif not hasattr(node, "children") or len(node.children) == 0:
                 node = node
             elif self.state.get("ctx") and (
                 self.state["ctx"].get("in") or self.state["ctx"].get("if")
             ):
                 node = node
             # if string
@@ -1312,16 +1441,14 @@
 
                 # if equality, check if equal
 
                 statement = node.children[0]
 
                 statement = self.parse_tree(statement)
 
-                print(statement, "xxx")
-
                 if statement is None:
                     continue
 
                 if statement is False:
                     return
 
                 self.state["last"] = last_state_before_if
@@ -1332,16 +1459,14 @@
 
             if token.value == None:
                 continue
 
             if token.value == "run":
                 function_name = node.children[0].value
 
-                print(f"Running {function_name}...")
-
                 if function_name not in self.state["functions"]:
                     print(f"Function {function_name} does not exist.")
                     exit(1)
 
                 function_args = self.state["functions"][function_name]
 
                 for item in function_args:
@@ -1351,15 +1476,16 @@
 
             if token.value == "literal":
                 func = self.state["functions"][node.children[0].value]
             else:
                 func = self.function_calls[token.value]
 
             if token.value == "negate" or token.value == "input":
-                return func(self.parse_tree(node.children[0]))
+                result = self.parse_tree(node.children[0])
+                return func(result)
 
             if token.value == "get":
                 continue
 
             self.state["history"].append(token.value)
 
             if token.value == "say":
@@ -1367,26 +1493,27 @@
                 func(value)
                 continue
             elif token.value == "contains":
                 return func(literal_eval(node.children[0]))
             else:
                 # convert children to strings
                 for item in node.children:
-                    print(item, "eeee")
                     if hasattr(item, "value"):
                         if item.value.startswith('"') and item.value.endswith('"'):
                             item.value = literal_eval(item.value)
                         elif item.type in ("EOL", "INDENT", "DEDENT"):
                             continue
                         elif item.type == "STRING":
                             item.value = literal_eval(item.value)
                         elif item.type == "INT":
                             item.value = int(item.value)
                         elif item.type == "input":
                             item.value = self.parse_tree(item.value)
+                        elif item.type == "FLOAT":
+                            item.value = float(item.value)
 
             if token.value == "in":
                 self.state["ctx"] = {
                     "in": os.listdir(node.children[0].value),
                 }
 
                 for file_name in self.state["ctx"]["in"]:
@@ -1418,15 +1545,15 @@
             if token.value == "literal":
                 result = self.parse_tree(self.state["functions"][value])
             else:
                 result = func(value)
 
             if result is not None:
                 self.state["last"] = result
-                self.state["output"] = result
+                self.state["output"] = {"text": result}
 
             self.state["last_function_type"] = token.value
             self.state["last_function_args"] = [value]
 
             if token.value == "load":
                 self.state["image_stack"].append(result)
 
@@ -1456,15 +1583,45 @@
 @click.option("--validate", default=False, help="")
 @click.option("--ref", default=False, help="Name of the file")
 @click.option("--debug", default=False, help="To debug")
 @click.option("--file", default=None, help="Name of the file")
 @click.option("--repl", default=None, help="To enter to visionscript console")
 @click.option("--notebook/--no-notebook", help="Start a notebook environment")
 @click.option("--cloud/--no-cloud", help="Start a cloud deployment environment")
-def main(validate, ref, debug, file, repl, notebook, cloud) -> None:
+@click.option("--deploy", help="Deploy a .vic file", default=None)
+@click.option(
+    "--name",
+    help="Application name (used if you are deploying your app via --deploy)",
+    default=None,
+)
+@click.option(
+    "--description",
+    help="Application description (used if you are deploying your app via --deploy)",
+    default=None,
+)
+@click.option("--api-key", help="API key for deploying your app", default=None)
+@click.option(
+    "--api-url",
+    help="API url for deploying your app",
+    default="http://localhost:6999/create",
+)
+def main(
+    validate,
+    ref,
+    debug,
+    file,
+    repl,
+    notebook,
+    cloud,
+    deploy,
+    name,
+    description,
+    api_key,
+    api_url,
+) -> None:
     if validate:
         print("Script is a valid VisionScript program.")
         exit(0)
 
     if ref:
         print(USAGE.strip())
 
@@ -1495,18 +1652,45 @@
 
         if debug:
             print(tree.pretty())
             exit()
 
         session = VisionScript()
 
-        # args = {"image": "./indieweb.jpg"}
+        if deploy:
+            if not name or not description or not api_key or not api_url:
+                print("Please provide a name, description, api key, and api url.")
+                return
+
+            session.notebook = True
 
-        # # merge state and args
-        # session.state = {**session.state, **args}
+            session.check_inputs(code)
+
+            import requests
+
+            app_slug = name.translate(
+                str.maketrans("", "", string.punctuation.replace("-", ""))
+            ).replace(" ", "-")
+
+            deploy_request = requests.post(
+                api_url,
+                json={
+                    "title": name,
+                    "slug": app_slug,
+                    "api_key": api_key,
+                    "description": description,
+                    "script": code,
+                    "variables": session.state["input_variables"],
+                },
+            )
+
+            if deploy_request.ok:
+                print("App deployed to", deploy_request.json()["url"])
+
+            return
 
         session.parse_tree(tree)
 
     if repl == "console":
         activate_console(parser)
```

### Comparing `visionscript-0.0.3/visionscript/static/.DS_Store` & `visionscript-0.0.4/visionscript/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.3/visionscript/static/examples.js` & `visionscript-0.0.4/visionscript/static/examples.js`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.3/visionscript/static/functions.js` & `visionscript-0.0.4/visionscript/static/functions.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -43,15 +43,15 @@
         "SetBrightness": {
             "args": ["amount"],
             "description": "Adjust the brightness of an image",
             "example": "SetBrightness[50]",
             "supports_arguments": true
         },
         "Replace": {
-            "args": ["color"],
+            "args": ["file"],
             "description": "Replace part of an image",
             "example": "Replace[\"red\"]",
             "supports_arguments": true,
             "argument_default": "\"\""
         },
         "Cutout": {
             "args": ["x", "y", "width", "height"],
@@ -70,14 +70,28 @@
             "args": ["amount"],
             "description": "Adjust the contrast of an image",
             "example": "Contrast[1.5]",
             "supports_arguments": true
         }
     },
     "Find": {
+        "SetRegion": {
+            "args": ["x", "y", "width", "height"],
+            "description": "Set the region to search for objects in (use before Detect[] or Segment[])",
+            "example": "SetRegion[0, 0, 100, 100]",
+            "supports_arguments": true,
+            "argument_default": "0, 0, 0, 0"
+        },
+        "FilterByClass": {
+            "args": ["object"],
+            "description": "Filter objects by class",
+            "example": "FilterByClass[\"person\"]",
+            "supports_arguments": true,
+            "argument_default": "\"\""
+        },
         "Classify": {
             "args": ["object"],
             "description": "Classify an image",
             "example": "Classify[\"person\", \"cat\"]",
             "supports_arguments": true,
             "argument_default": "\"\", \"\""
         },
@@ -110,21 +124,14 @@
         },
         "Count": {
             "args": ["object"],
             "description": "Count objects in an image",
             "example": "Count[]",
             "supports_arguments": false
         },
-        "CountInRegion": {
-            "args": ["object", "x", "y", "width", "height"],
-            "description": "Count objects in a region of an image",
-            "example": "CountInRegion[\"person\", 0, 0, 100, 100]",
-            "supports_arguments": true,
-            "argument_default": "\"\", 0, 0, 0, 0"
-        },
         "ReadQR": {
             "args": [],
             "description": "Read a QR code in an image",
             "example": "ReadQR[]",
             "supports_arguments": false
         },
         "GetText": {
```

### Comparing `visionscript-0.0.3/visionscript/static/main.js` & `visionscript-0.0.4/visionscript/static/main.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,32 @@
 var mode = "interactive";
 
+function rerun(cell_number) {
+    var cells = document.getElementById("cells");
+    var cell = cells.children[cell_number - 1];
+
+    var textarea = cell.getElementsByTagName("textarea")[0];
+    textarea.value = textarea.value.trim();
+    var output = cell.getElementsByTagName("pre")[0];
+    output.innerText = "";
+    var output = document.getElementById("output");
+    output.style.display = "block";
+
+    executeCode(textarea.value, false, cell.id);
+}
+
+function show_toast(message) {
+    var toast = document.getElementById("toast");
+    toast.innerText = message;
+    toast.style.display = "block";
+    setTimeout(function() {
+        toast.style.display = "none";
+    }, 3000);
+}
+
 function switch_mode() {
     if (mode == "interactive") {
         document.getElementById("mode_switch").innerText = "Use Interactive Mode 📝";
         mode = "code";
     } else {
         document.getElementById("mode_switch").innerText = "Use Code Mode 📝";
         mode = "interactive";
@@ -42,58 +65,71 @@
             function_element.style.display = "block";
         } else {
             function_element.style.display = "none";
         }
     }
 }
 
+
+document.addEventListener("keydown", function(event) {
+    // Command + Enter should run
+    if (event.code == "Enter" && event.metaKey) {
+        var code = getCodeFromInteractiveEnvironment();
+        executeCode(code);
+        return;
+    }
+    // Command + S should save
+    if (event.key == "s" && event.metaKey) {
+        event.preventDefault();
+        export_vicnb();
+        return;
+    }
+});
+
 // if user hits enter, take top result
 // listen for key
 document.addEventListener("keydown", function(event) {
     var search = document.getElementById("search");
 
     if (search != document.activeElement) {
         return;
     }
 
 
-    // Command + Enter should run
-    if (event.key == "Enter" && event.metaKey) {
-        var code = getCodeFromInteractiveEnvironment();
-        executeCode(code);
-        return;
-    }
-
     if (event.key == "Enter") {
         // set background color
         document.getElementById("drag_drop_notebook").style.background = "white";
         var functions = document.getElementsByClassName("function");
         var function_element = functions[0];
         var function_name = function_element.id;
         var code = function_name + "[]";
         var color = function_element.firstElementChild.style.color;
 
         var html = "";
 
         var cell_count = cells.children.length + 1;
 
-        html = `
-            <div class="cell" draggable="true" id="${function_name}_${cell_count}" style="background-color: ${color};">
-                <p>${function_name}[]</p>
-            </div>
-        `;
+        if (mapped_functions[function_name].supports_arguments) {
+            html = `
+                <div class="cell" draggable="true" id="${function_name}_${cell_count}" style="background-color: ${color}; margin-left: 20px;">
+                    <p>${function_name}[<input type="text" class="argument_block" id="cell_${cell_count}" />]</p>
+                </div>
+            `;
+        } else {
+            html = `
+                <div class="cell" draggable="true" id="${function_name}_${cell_count}" style="background-color: ${color}; margin-left: 20px;">
+                    <p>${function_name}[]</p>
+                </div>
+            `;
+        }
 
         notebook.appendChild(document.createRange().createContextualFragment(html));
     }
 });
 
-function importNotebookToInteractiveCode(notebook) {
-
-}
-
 var colors = {
     "Input": "#a2d2ff",
     "Process": "#cdb4db",
     "Find": "#ccd5ae",
     "Output": "lavender",
     "Logic": "#ffdf6b"
 };
@@ -123,20 +159,39 @@
 
 for (var i = 0; i < functions.length; i++) {
     var function_element = functions[i];
     function_element.addEventListener("dragstart", function(event) {
         event.dataTransfer.setData("text/plain", event.target.id);
     });
 
+    console.log("function", functions[i]);
+
     // on mobile tap, add to notebook
     function_element.addEventListener("touchstart", function(event) {
         event.preventDefault();
         // set background color
+        // ACCESS functinos from parent
+
         document.getElementById("drag_drop_notebook").style.background = "white";
+
+        // get function name
         var function_name = event.target.id;
+
+        // if no id, traverse up
+        if (!function_name) {
+            while (!function_name) {
+                function_name = event.target.parentElement.id;
+                // break if element is <html>
+                if (event.target.parentElement.tagName == "HTML") {
+                    break;
+                }
+            }
+        }
+
+
         var function_element = document.getElementById(function_name);
 
         var color = function_element.firstElementChild.style.color;
 
         var html = "";
 
         var cell_count = cells.children.length + 1;
@@ -153,14 +208,32 @@
                     <p>${function_name}[]</p>
                 </div>
             `;
         }
 
         notebook.appendChild(document.createRange().createContextualFragment(html));
 
+        function doubleTap(element) {
+            var lastTap = 0;
+            return function(event) {
+                var currentTime = new Date().getTime();
+                var tapLength = currentTime - lastTap;
+                event.preventDefault();
+                if (tapLength < 500 && tapLength > 0) {
+                    // double tap
+                    element.remove();
+                }
+                lastTap = currentTime;
+            };
+        }
+        // if double tap, delete block
+        var cell = document.getElementById(`${function_name}_${cell_count}`);
+
+        cell.addEventListener("touchstart", doubleTap(cell));
+
         // if argument block, allow tap on block to upload file
         if (mapped_functions[function_name].supports_arguments && mapped_functions[function_name].args.includes("file")) {
             var argument_block = document.getElementsByClassName("argument_block");
             var argument_block = argument_block[argument_block.length - 1];
             argument_block.addEventListener("click", function(event) {
                 event.preventDefault();
                 var file_input = document.createElement("input");
@@ -182,15 +255,15 @@
                         var error_message = document.getElementById("error_message");
                         error_message.innerText = "Your file could not be uploaded. Please make sure you have uploaded a supported format.";
                         dialog.showModal();
                         return;
                     }
 
                     // post to /notebook/upload with state id
-                    fetch(`http://localhost:5001/notebook/upload?state_id=${STATE_ID}`, {
+                    fetch(`${API_URL}/notebook/upload?state_id=${STATE_ID}`, {
                             method: 'POST',
                             body: body
                         })
                         .then(response => response.json())
                         .then(data => {
                             var cell = document.getElementById("cell_" + argument_block.id.split("_")[1]);
                             cell.value = data.file_name;
@@ -198,16 +271,21 @@
                             var img = document.createElement("img");
                             img.src = reader.result;
                             img.style.width = "100px";
                             img.style.height = "100px";
                             argument_block.innerHTML = "";
                             img.dataset.filename = data.file_name;
                             img.classList.add("argument_block");
-                            // replace cell with image
                             cell.replaceWith(img);
+
+                            if (file.name.endsWith(".vicnb")) {
+                                show_toast("Your notebook has been imported.");
+                            } else {
+                                show_toast("Your file has been uploaded.");
+                            }
                         });
                 });
             });
         }
     });
 }
 
@@ -231,20 +309,24 @@
     // if cell has an argumetn_block, don't do anything
     // if hovered outside of drag_drop_notebook, delete
     if (cells.children.length > 0) {
         if (cells.children[cells.children.length - 1].id == "argument_block") {
             return;
         }
     }
-    // get "text/plain" cata
+    // get "text/plain" data
     var function_name = event.dataTransfer.getData("text/plain");
     var function_element = document.getElementById(function_name);
 
+    // skip Input[]
+    if (function_name == "Input") {
+        return;
+    }
     // if is cell, don't do anything
-    if (function_element.classList.contains("cell")) {
+    if (function_element && function_element.classList.contains("cell")) {
         // move cell in list
         var cell = function_element;
         var cell_index = Array.prototype.indexOf.call(cells.children, cell);
         var cell_count = cells.children.length;
         // move under closest cell
         var closest_cell = null;
         var closest_cell_index = null;
@@ -283,15 +365,14 @@
             cells.insertBefore(cell, closest_cell);
         }
         return;
     }
     // last cell
     var margin = 20;
     var nested = false;
-    // con
     if (cells.children.length > 0) {
         // if last cell function was an If or In
         if (cells.children[cells.children.length - 1].id.includes("If") || cells.children[cells.children.length - 1].id.includes("In")) {
             var last_cell = cells.children[cells.children.length - 1];
             var last_cell_rect = last_cell.getBoundingClientRect();
             if (event.clientY > last_cell_rect.top && event.clientY < last_cell_rect.bottom) {
                 margin = 40;
@@ -319,15 +400,14 @@
 
         notebook.appendChild(document.createRange().createContextualFragment(html));
         return;
     }
 
     var function_name = event.dataTransfer.getData("text/plain");
     var function_element = document.getElementById(function_name);
-    var code = function_name + "[]";
     var color = function_element.firstElementChild.style.color;
 
     var html = "";
 
     var cell_count = cells.children.length + 1;
 
     if (mapped_functions[function_name].supports_arguments) {
@@ -375,44 +455,49 @@
         argument_block.addEventListener("dragleave", function(event) {
             event.preventDefault();
             argument_block.style.backgroundColor = "white";
         });
         argument_block.addEventListener("drop", function(event) {
             // replace <input> with Input[]
             var function_name = event.dataTransfer.getData("text/plain");
-            var function_element = document.getElementById(function_name);
-            var code = function_name + "[]";
             // if it is a cell, don't do anything
             // replace event.target with Input[]
             if (function_name == "Input") {
                 var argument_block = event.target;
                 // replace argument_block
                 var argument_block = document.getElementById("cell_" + argument_block.id.split("_")[1]);
                 var input_field = event.target;
                 // replace with p
                 var p = document.createElement("p");
-                p.innerText = "Input[]";
+                p.innerText = "Input[";
                 p.style.display = "inline-block";
-                p.style.margin = "0";
-                p.style.padding = "0";
+                p.style.margin = "10px";
+                p.style.padding = "5px;";
                 p.style.backgroundColor = "white";
                 p.classList.add("argument_block");
 
                 // create input and append to argument block
                 var input = document.createElement("input");
                 input.type = "text";
                 input.classList.add("argument_block");
                 input.id = "cell_" + argument_block.id.split("_")[1];
-                input.style.display = "inline-block";
-                input.style.margin = "0";
-                input.style.padding = "0";
                 input.style.backgroundColor = "white";
+                input.style.margin = "10px";
+                // add "]" after input
+                var p2 = document.createElement("p");
+                p2.innerText = "]";
+                p2.style.display = "inline-block";
+                p2.style.margin = "0";
+                p2.style.padding = "0";
+                p2.style.backgroundColor = "white";
                 p.appendChild(input);
+                p.appendChild(p2);
                 // replace
                 argument_block.replaceWith(p);
+                argument_block.style.margin = "10px";
             }
         });
     }
 });
 
 function getCodeFromInteractiveEnvironment() {
     var code = "";
@@ -469,15 +554,14 @@
             argument = argument.replace(/\"\"/g, "");
 
             // if nested, start w/ indent
             if (function_element.dataset.nested) {
                 code += "    ";
                 in_nested_context = true;
             }
-
             code += function_name + "[" + argument + " ]" + "\n";
         } else {
             code += function_name + "[]" + "\n";
         }
     }
 
     // if code doesn't end with Say[], add it
@@ -488,49 +572,62 @@
     return code;
 }
 
 var run = document.getElementById("run");
 
 run.addEventListener("click", function(event) {
     event.preventDefault();
-    var output = document.getElementById("output");
     var code = getCodeFromInteractiveEnvironment();
     executeCode(code);
 });
 
+function deploy_code(publish_as_noninteractive_webpage) {
+    fetch(`${API_URL}/notebook/deploy`, {
+            method: 'POST',
+            headers: {
+                'Content-Type': 'application/json'
+            },
+            body: JSON.stringify({
+                state_id: STATE_ID,
+                name: document.getElementById("name").value,
+                api_url: document.getElementById("api_url").value,
+                api_key: document.getElementById("api_key").value,
+                description: document.getElementById("description").value,
+                publish_as_noninteractive_webpage: publish_as_noninteractive_webpage
+            })
+        })
+        .then(response => response.json())
+        .then(data => {
+            var deploy_message = document.getElementById("deploy_message");
+            deploy_message.innerText = data.message;
+            deploy_message.style.display = "block";
+        })
+        .catch((error) => {
+            var deploy_message = document.getElementById("deploy_message");
+            deploy_message.innerText = "Your app could not be deployed. Please make sure your app code is valid and you have filled out the deployment form in full.";
+            // show deploy_message
+            deploy_message.style.display = "block";
+            // add error class
+            deploy_message.classList.add("error");
+        });
+}
+
 function deploy() {
     var deploy = document.getElementById("deploy");
     deploy.showModal();
     var deploy_form = document.getElementById("deploy_form");
     deploy_form.addEventListener("submit", function(event) {
         event.preventDefault();
-        fetch('http://localhost:5001/notebook/deploy', {
-                method: 'POST',
-                headers: {
-                    'Content-Type': 'application/json'
-                },
-                body: JSON.stringify({
-                    state_id: STATE_ID,
-                    name: document.getElementById("name").value
-                })
-            })
-            .then(response => response.json())
-            .then(data => {
-                var deploy_message = document.getElementById("deploy_message");
-                deploy_message.innerText = data.message;
-            })
-            .catch((error) => {
-                var deploy_message = document.getElementById("deploy_message");
-                deploy_message.innerText = "Your app could not be deployed. Please make sure your app code is valid.";
-            });
+        deploy_code(false);
     });
 }
 var cells = document.getElementById("cells");
 
 function startLoading(loading) {
+    loading.style.display = "block";
     var timer = setInterval(function() {
         if (loading.innerText == "Loading") {
             loading.innerText = "Loading.";
         } else if (loading.innerText == "Loading.") {
             loading.innerText = "Loading..";
         } else if (loading.innerText == "Loading..") {
             loading.innerText = "Loading...";
@@ -539,135 +636,195 @@
         } else {
             loading.innerText = "Loading";
         }
     }, 500);
     return timer;
 }
 
-function executeCode(code) {
-    // make loading wheel
-
-    cells.innerHTML += `
-        <li class="cell" id="loading">Loading</li>
-    `;
+function executeCode(code, comment = false, existing_cell = null) {
     var loading = document.getElementById("loading");
     var output = document.getElementById("output");
-    // show output
+
     output.style.display = "block";
+
     var timer = startLoading(loading);
     var output_timer = startLoading(output);
 
     var error_cell = document.getElementById("error");
 
     error_cell.innerText = "";
     error_cell.style.display = "none";
 
-    fetch('http://localhost:5001/notebook', {
+    var is_text_cell = comment;
+
+    fetch(`${API_URL}/notebook`, {
             method: 'POST',
             headers: {
                 'Content-Type': 'application/json'
             },
             body: JSON.stringify({
                 code: code,
-                state_id: STATE_ID
+                state_id: STATE_ID,
+                is_text_cell: is_text_cell
             })
         })
         .then(response => response.json())
-        .then(data => {
-            if (data.output == null) {
-                data.output = "";
-            }
+        .then((data) => {
+            var data = data;
+            var is_image = false;
+
             if (data.output.image) {
-                data.output = `<img src="data:image/png;base64,${data.output.image}">`;
+                is_image = true;
+                data.output = `<img src="data:image/png;base64,${data.output.image}" />`;
+            } else if (is_text_cell) {
+                data.output = DOMPurify.sanitize(marked.parse(code));
+            } else if (data.output.text) {
+                data.output = data.output.text;
+            } else {
+                data.output = data.output;
             }
             var time = data.time;
-            // delete loading cell
-            cells.removeChild(loading);
+            // hide loading cell
+            loading.style.display = "none";
             clearInterval(timer);
             clearInterval(output_timer);
 
+            if (existing_cell) {
+                var cell = document.getElementById(existing_cell);
+                if (is_image) {
+                    cell.innerHTML = `
+                    <p class="time">#${existing_cell} (${time}s) - <a href="#" onclick="rerun(${existing_cell})">Rerun</a></p>
+                    <textarea rows="${row_count}">${code}</textarea>
+                    <p>${data.output}</p>
+                `;
+                    return;
+                }
+                cell.innerHTML = `
+                <p class="time">#${existing_cell} (${time}s) - <a href="#" onclick="rerun(${existing_cell})">Rerun</a></p>
+                <textarea rows="${row_count}">${data.output}</textarea>
+                <pre ${data.error ? 'class="error_cell"' : ''}>${data.error ? data.error : data.output}</pre>
+            `;
+                return;
+            }
+
             var row_count = (code.match(/\n/g) || []).length + 1;
 
             // if interactive mode, show in #output
             if (mode == "interactive") {
                 var output = document.getElementById("output");
                 output.innerHTML = data.output;
                 return;
             }
 
-            cells.innerHTML += `
-            <li class="cell">
-                <p class="time">#${cells.children.length + 1} (${time}s)</p>
-                <textarea rows="${row_count}" readonly class="cell_run">${code}</textarea>
-                <pre ${data.error ? 'class="error_cell"' : ''}>${data.error ? data.error : data.output}</pre>
-            </li>
-        `;
+            if (!is_text_cell) {
+                cells.innerHTML += `
+                <li class="cell" id="${cells.children.length + 1}">
+                    <p class="time">#${cells.children.length + 1} (${time}s) - <a href="#" onclick="rerun(${cells.children.length + 1})">Rerun</a></p>
+                    <textarea rows="${row_count}">${code}</textarea>
+                    <pre ${data.error ? 'class="error_cell"' : ''}>${data.error ? data.error : data.output}</pre>
+                </li>
+            `;
+            } else {
+                cells.innerHTML += `
+                <li class="cell" id="${cells.children.length + 1}">
+                    <p class="time">#${cells.children.length + 1}</p>
+                    ${data.output}
+                </li>
+            `;
+            }
 
             document.getElementById("current_count").innerHTML = `#${cells.children.length + 1}`;
-
-            // click to copy to clipboard
-            for (var i = 0; i < cells.children.length; i++) {
-                var cell = cells.children[i];
-                var textarea = cell.getElementsByTagName("textarea")[0];
-                textarea.addEventListener("click", function(event) {
-                    event.preventDefault();
-                    var text = event.target.value;
-                    navigator.clipboard.writeText(text);
-                    alert("Copied to clipboard");
-                });
-            }
         })
         .catch((error) => {
             clearInterval(timer);
             clearInterval(output_timer);
 
             var error_cell = document.getElementById("error");
             error_cell.innerText = "There was an error running your code. Please make sure your code is valid.";
             error_cell.style.display = "block";
             // hide output
             output.style.display = "none";
+            var loading = document.getElementById("loading");
+            loading.style.display = "none";
         });
 }
 
 var form = document.getElementById("new");
+var create_comment = document.getElementById("create_comment");
 
 form.addEventListener("submit", function(event) {
     event.preventDefault();
     var data = new FormData(form);
     var code = data.get("jscode");
     executeCode(code);
 });
 
+create_comment.addEventListener("click", function(event) {
+    event.preventDefault();
+    var data = new FormData(form);
+    var code = data.get("jscode");
+    executeCode(code, comment = true);
+});
+
 // auto-expand textarea
 var textarea = document.getElementById("jscode");
 
 textarea.addEventListener("input", function(event) {
     textarea.style.height = "auto";
     textarea.style.height = textarea.scrollHeight + "px";
 });
 
-var export_vic = document.getElementById("export_vic");
+function exportNotebook() {
+    var export_modal = document.getElementById("export");
+    export_modal.showModal();
+}
+
+function export_vic() {
+    var data = new FormData();
 
-export_vic.addEventListener("click", function(event) {
-    event.preventDefault();
-    var data = new FormData(form);
     if (mode == "interactive") {
         var code = getCodeFromInteractiveEnvironment();
         data.set("jscode", code);
     }
+
     var code = data.get("jscode");
     var blob = new Blob([code], {
         type: "text/plain;charset=utf-8"
     });
     // download
     var a = document.createElement("a");
     a.href = URL.createObjectURL(blob);
     a.download = "notebook.vic";
     a.click();
-});
+}
+
+function export_vicnb() {
+    fetch(`${API_URL}/notebook/save`, {
+            method: 'POST',
+            headers: {
+                'Content-Type': 'application/json'
+            },
+            body: JSON.stringify({
+                state_id: STATE_ID
+            })
+        }).then(response => response.json())
+        .then(data => {
+            var data = JSON.stringify(data);
+
+            var blob = new Blob([data], {
+                type: "text/plain;charset=utf-8"
+            });
+            blob.name = "notebook.vicnb";
+
+            var a = document.createElement("a");
+            a.href = URL.createObjectURL(blob);
+            a.download = "notebook.vicnb";
+            a.click();
+        });
+}
 
 var dropzone = document.getElementsByTagName("body")[0];
 
 dropzone.addEventListener("dragover", function(event) {
     event.preventDefault();
 });
 
@@ -681,166 +838,50 @@
 dropzone.addEventListener("drop", function(event) {
     if (event.target.id == "drag_drop_notebook") {
         return;
     }
     // if function box, delete the function box
     // read data channel
     var readData = event.dataTransfer.getData("text/plain");
-    if (readData) {
+    if (readData && readData.startsWith("function_box")) {
         // delete element
         var element = document.getElementById(readData);
         element.parentNode.removeChild(element);
         return;
     }
     event.preventDefault();
     dropzone.style.backgroundColor = "white";
+
     var file = event.dataTransfer.files[0];
-    var body = new FormData();
-    body.append("file", file)
-    body.append("state_id", STATE_ID);
-    // base64 file
-    var reader = new FileReader();
-    // read file
-    reader.readAsDataURL(file);
 
     // only allow jpeg, jpg, png, or .vicnb
     if (!file.name.endsWith(".jpg") && !file.name.endsWith(".jpeg") && !file.name.endsWith(".png") && !file.name.endsWith(".vicnb")) {
         var dialog = document.getElementById("dialog");
         var error_message = document.getElementById("error_message");
         error_message.innerText = "Your file could not be uploaded. Please make sure you have uploaded a supported format.";
         dialog.showModal();
         return;
     }
 
-    // post to /notebook/upload with state id
-    fetch(`http://localhost:5001/notebook/upload?state_id=${STATE_ID}`, {
-            method: 'POST',
-            body: body
-        })
-        .then(response => response.json())
-        .then(data => {
-            if (data.cells) {
-                if (mode == "code") {
-                    data.cells.forEach(function(cell) {
-                        var code = cell.cell;
-                        var output = cell.output;
-                        if (output == null) {
-                            output = "";
-                        }
-                        if (output.image) {
-                            output = `<img src="data:image/png;base64,${output.image}">`;
-                        }
-                        cells.innerHTML += `
-                        <li class="cell">
-                            <p>#${cells.children.length + 1}</p>
-                            <textarea rows="3" disabled>${code}</textarea>
-                            <pre>${output}</pre>
-                        </li>
-                    `;
-                    });
-                    return;
-                } else {
-                    var interactive_notebook = document.getElementById("drag_drop_notebook");
-
-                    data.cells.forEach(function(cell) {
-                        var code = cell.cell;
-                        // for item in newline
-                        var code = code.split("\n");
-                        for (var i = 0; i < code.length; i++) {
-                            // set background to white
-                            interactive_notebook.style.background = "white";
-                            var line = code[i];
-                            var function_name = line.split("[")[0];
-                            var argument = line.split("[")[1];
-                            if (argument) {
-                                argument = argument.split("]")[0];
-                            }
-                            var color = mapped_functions[function_name].element.firstElementChild.style.color;
-                            var html = "";
-                            if (mapped_functions[function_name].supports_arguments) {
-                                html = `
-                                <div class="cell" draggable="true" id="${function_name}_${i + 1}" style="background-color: ${color}; margin-left: 20px;">
-                                    <p>${function_name}[<input type="text" class="argument_block" id="cell_${i + 1}" value="${argument}">]</p>
-                                </div>
-                            `;
-                            } else {
-                                html = `
-                                <div class="cell" draggable="true" id="${function_name}_${i + 1}" style="background-color: ${color}; margin-left: 20px;">
-                                    <p>${function_name}[]</p>
-                                </div>
-                            `;
-                            }
-                            interactive_notebook.appendChild(document.createRange().createContextualFragment(html));
-                        }
-                    }).catch((error) => {
-                        return;
-                    });
-                }
-            }
-            var file_name = data.file_name;
-            var files = document.getElementById("files");
-            var files_section = document.getElementById("files_section");
-
-            files_section.style.display = "block";
-
-            var base64 = reader.result;
-
-            // if already exists, don't add
-            var file_names = document.getElementsByClassName("file_name");
-
-            for (var i = 0; i < file_names.length; i++) {
-                var file_name_element = file_names[i];
-                if (file_name_element.innerText == file_name) {
-                    return;
-                }
-            }
-
-            files.innerHTML += `
-            <li><img src="${base64}" alt="${file_name}" height=100 width=100 data-filename="${file_name}" style="display: block;">${file_name}</li>
-        `;
-            // if dragged over an Load statement, add iamge to the argument block
-
-            if (event.target.classList.contains("argument_block")) {
-                // replace argument block
-                var argument_block = event.target;
-                var new_element = `
-                <img src="${base64}" alt="${file_name}" height=100 width=100 class="argument_block" data-filename="${file_name}">
-            `;
-
-                // add before argument block
-                argument_block.insertAdjacentHTML("beforebegin", new_element);
-
-                // remove argument block
-                argument_block.parentNode.removeChild(argument_block);
-            }
-        })
-        .catch(err => {
-            var dialog = document.getElementById("dialog");
-            var error_message = document.getElementById("error_message");
-            // if file ends with .vicnb
-            console.log(err);
-            if (file.name.endsWith(".vicnb")) {
-                error_message.innerText = "Please import your notebook in interactive mode.";
-                dialog.showModal();
-                return;
-            }
-
-            error_message.innerText = "Your file could not be uploaded. Please make sure you have uploaded a supported format.";
-            dialog.showModal();
-        });
+    uploadNotebook(event, mode);
 });
 
 function resetNotebook() {
     var code = "Reset[]\n";
     executeCode(code);
-    // show dialog
-    var dialog = document.getElementById("dialog");
-    var error_message = document.getElementById("error_message");
-    error_message.innerText = "Your notebook has been reset.";
-    dialog.showModal();
+    // show toast
+    show_toast("Your notebook has been reset.");
+    // delete all cells
+    var cells = document.getElementById("cells");
+    cells.innerHTML = "";
+    // delete all interactive cells
+    var notebook = document.getElementById("drag_drop_notebook");
+    notebook.innerHTML = "";
+    // set background back to image
+    document.getElementById("drag_drop_notebook").style.background = "url('/static/drag_and_drop.png')";
 }
 
 function toggle_menu() {
     var menu = document.getElementById("nav_menu");
     if (menu.style.display != "none") {
         menu.style.display = "flex";
     } else {
```

### Comparing `visionscript-0.0.3/visionscript/static/styles.css` & `visionscript-0.0.4/visionscript/static/styles.css`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,18 @@
     box-sizing: border-box;
     padding: 0;
     margin: 0;
 }
 html {
     background-color: #f7f7f7;
 }
+a {
+    color: darkgreen;
+    text-decoration: none;
+}
 ul {
     list-style-type: none;
     padding: 0;
 }
 .cell {
     background-color: #eee;
     padding: 1rem;
@@ -21,24 +25,25 @@
     width: 100%;
     border: 1px solid #ccc;
     resize: none;
     border-radius: 0.5rem;
     padding: 0.5rem;
     display: block;
 }
-input[type="submit"] {
+input[type="submit"], #create_comment {
     margin-top: 0.5rem;
     background-color: darkgreen;
     color: white;
     border: none;
     padding: 0.5rem 1rem;
     border-radius: 0.5rem;
     cursor: pointer;
     resize: none;
     overflow: hidden;
+    width: 100%;
 }
 img {
     max-width: 100%;
 }
 nav {
     background-color: darkgreen;
     color: white;
@@ -49,20 +54,19 @@
     font-size: 2rem;
     margin-bottom: 0.5rem;
 }
 h3 {
     font-size: 14px;
     margin-bottom: 0.5rem;
 }
-section {
+section, #notebook {
     padding: 1rem;
     max-width: 50em;
     margin: 0 auto;
     flex: 1;
-    min-height: 1000px;
 }
 #current_count {
     font-size: 1rem;
     font-weight: bold;
     margin-bottom: 0.5rem;
 }
 main {
@@ -135,20 +139,20 @@
     background-position: center;
     background-size: 100%;
 }
 #function_box, #files_section {
     width: 20em;
     padding: 1rem;
     background-color: white;
-    border-radius: 0 0 0 1rem;
     overflow-y: scroll;
-    max-height: 100vh;
-    border: 1px solid lightgrey;
-    min-height: 100em;
+    border: 1px solid #d3d3d3;
+    height: 100vh;
     line-height: 1.5em;
+    position: sticky;
+    top: 0;
 }
 #function_box h2 {
     font-size: 18px;
     margin-bottom: 10px;
 }
 #function_box h3 {
     font-size: 16px;
@@ -194,15 +198,15 @@
 }
 .argument_block {
     background: white;
     padding: 7.5px;
     border-radius: 5px;
     margin-left: 10px;
 }
-#error {
+#error, .error {
     display: none;
     background-color: lightcoral;
     border-radius: 5px;
     padding: 10px;
     margin-top: 10px;
 }
 #run input {
@@ -213,17 +217,23 @@
     margin-top: 10px;
     border: 1px solid darkgreen;
     border-radius: 5px;
     padding: 10px;
 }
 dialog {
     border-radius: 5px;
-    padding: 10px;
+    padding: 50px;
     background-color: white;
     margin: auto;
+    max-width: 40em;
+    min-width: 20em;
+    top: 0;
+    left: 0;
+    right: 0;
+    bottom: 0;
 }
 dialog h2 {
     font-size: 18px;
     margin-bottom: 10px;
 }
 dialog section {
     margin: auto;
@@ -238,15 +248,15 @@
     cursor: pointer;
     resize: none;
     overflow: hidden;
     margin-top: 10px;
     width: 100%;
 }
 dialog input {
-    margin-top: 20px;
+    margin-top: 5px;
     width: 100%;
     border: 1px solid #ccc;
     resize: none;
     border-radius: 0.5rem;
     padding: 0.5rem;
     display: block;
     margin-bottom: 10px;
@@ -281,34 +291,68 @@
 }
 #toggle_menu {
     display: none;
 }
 .hide_on_mobile {
     display: block;
 }
+.hide_on_desktop {
+    display: none;
+}
 #nav_menu {
     display: flex;
     justify-content: space-between;
     align-items: center;
 }
+#toast {
+    position: fixed;
+    top: 0;
+    right: 0;
+    margin: 10px;
+    padding: 10px;
+    border-radius: 5px;
+    background-color: white;
+    border: 1px solid lightgrey;
+    box-shadow: 0 0 10px lightgrey;
+    z-index: 100;
+    display: none;
+}
+#deploy_message {
+    display: none;
+    margin-bottom: 10px;
+    border: 1px solid lightgrey;
+    padding: 10px;
+}
+dialog p {
+    margin-bottom: 10px;
+}
+label {
+    display: block;
+    font-weight: bold;
+}
 @media screen and (max-width: 800px) {
     #nav_menu {
         display: none;
     }
     #files_section {
         display: none;
     }
     #function_box {
-        display: block;
         position: fixed;
         bottom: 0;
         left: 0;
         width: 100%;
-        height: 300px;
-        min-height: 300px;
+        background-color: white;
+        z-index: 100;
+        justify-content: center;
+        align-items: center;
+        flex-direction: column;
+        padding: 50px;
+        top: initial;
+        height: 500px;
     }
     #function_box h2 {
         display: none;
     }
     #nav_menu {
         display: none;
         position: fixed;
```

### Comparing `visionscript-0.0.3/visionscript/templates/deployintro.html` & `visionscript-0.0.4/visionscript/templates/deployintro.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <title>VisionScript Notebook</title>
+    <title>VisionScript Deploy</title>
     <style>
         * {
             font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
             box-sizing: border-box;
             padding: 0;
             margin: 0;
             line-height: 1.5;
@@ -104,39 +104,52 @@
             margin-bottom: 10px;
         }
         pre {
             margin-top: 0.5rem;
             white-space: pre-wrap;
             word-wrap: break-word;
         }
-        .time {
-            font-size: 12px;
-            color: grey;
-            margin-bottom: 0.5rem;
-        }
         main {
             min-height: 100vh;
         }
-        .cell_run {
-            background-color: #eee;
-            padding: 1rem;
+        .cta {
+            border: 3px solid darkgreen;
             border-radius: 0.5rem;
             margin-bottom: 1rem;
-            cursor: pointer;
+            padding: 10px;
+            display: block;
+            margin-top: 20px;
         }
-        .cell_run:focus {
-            outline: none;
+        .cta a {
+            background-color: darkgreen;
+            color: white;
+            border: none;
+            padding: 0.5rem 1rem;
+            border-radius: 0.5rem;
+            cursor: pointer;
+            resize: none;
+            overflow: hidden;
+            text-decoration: none;
+            display: block;
+            margin-top: 20px;
         }
     </style>
+
+    <link rel="manifest" href="/assets/deploy_manifest.json">
 </head>
 <body>
     <nav>
         <ul>
             VisionScript Deploy
         </ul>
     </nav>
     <main>
         <h1>VisionScript Deploy</h1>
-        <p>Run VisionScript applications via a web application and API.</p>
+        <p>Run VisionScript code via a web application and API.</p>
+        <section class="cta">
+            <h2>Build your own VisionScript apps</h2>
+            <p>Using VisionScript you can build computer vision apps with a drag-and-drop interface, or a concise programming language.</p>
+            <a href="https://visionscript.org" target="_blank">Get started ➡️</a>
+        </section>
     </main>
 </body>
 </html>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,5 +1,10 @@
 
+
     * VisionScript Deploy
 
 ****** VisionScript Deploy ******
-Run VisionScript applications via a web application and API.
+Run VisionScript code via a web application and API.
+***** Build your own VisionScript apps *****
+Using VisionScript you can build computer vision apps with a drag-and-drop
+interface, or a concise programming language.
+Get_started_â¡ï¸
```

### Comparing `visionscript-0.0.3/visionscript/usage.py` & `visionscript-0.0.4/visionscript/usage.py`

 * *Files identical despite different names*

### Comparing `visionscript-0.0.3/visionscript.egg-info/PKG-INFO` & `visionscript-0.0.4/visionscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionscript
-Version: 0.0.3
+Version: 0.0.4
 Summary: VisionScript is an abstract programming language for doing common computer vision tasks, fast.
 Home-page: https://github.com/capjamesg/visionscript
 Author: capjamesg
 Author-email: jamesg@jamesg.blog
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `visionscript-0.0.3/visionscript.egg-info/SOURCES.txt` & `visionscript-0.0.4/visionscript.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .gitignore
 CITATION.cff
-CNAME
 CONTRIBUTING.md
 CONTRIBUTORS.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 requirements.txt
```

