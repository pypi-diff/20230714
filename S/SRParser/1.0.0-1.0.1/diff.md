# Comparing `tmp/SRParser-1.0.0.tar.gz` & `tmp/SRParser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SRParser-1.0.0.tar", last modified: Sat Feb 25 18:35:49 2023, max compression
+gzip compressed data, was "SRParser-1.0.1.tar", last modified: Thu Jul 13 22:48:16 2023, max compression
```

## Comparing `SRParser-1.0.0.tar` & `SRParser-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-02-25 18:35:49.393523 SRParser-1.0.0/
--rw-rw-rw-   0        0        0    11510 2023-01-06 21:44:52.000000 SRParser-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2569 2023-02-25 18:35:49.394525 SRParser-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2028 2023-02-25 18:28:57.000000 SRParser-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-25 18:35:49.347516 SRParser-1.0.0/SRParser/
--rw-rw-rw-   0        0        0    17991 2023-02-25 18:19:00.000000 SRParser-1.0.0/SRParser/SnortParser.py
--rw-rw-rw-   0        0        0       88 2023-02-25 16:18:48.000000 SRParser-1.0.0/SRParser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-25 18:35:49.391522 SRParser-1.0.0/SRParser.egg-info/
--rw-rw-rw-   0        0        0     2569 2023-02-25 18:35:49.000000 SRParser-1.0.0/SRParser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-02-25 18:35:49.000000 SRParser-1.0.0/SRParser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-25 18:35:49.000000 SRParser-1.0.0/SRParser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-02-25 18:35:49.000000 SRParser-1.0.0/SRParser.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-25 18:35:49.000000 SRParser-1.0.0/SRParser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-02-25 18:35:49.400522 SRParser-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1089 2023-02-25 18:35:14.000000 SRParser-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 22:48:16.286486 SRParser-1.0.1/
+-rw-rw-rw-   0        0        0    11510 2023-07-13 22:44:31.000000 SRParser-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2584 2023-07-13 22:48:16.286486 SRParser-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2043 2023-07-13 22:44:31.000000 SRParser-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 22:48:16.273472 SRParser-1.0.1/SRParser/
+-rw-rw-rw-   0        0        0    17992 2023-07-13 22:44:47.000000 SRParser-1.0.1/SRParser/SnortParser.py
+-rw-rw-rw-   0        0        0       90 2023-07-13 22:44:31.000000 SRParser-1.0.1/SRParser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 22:48:16.285481 SRParser-1.0.1/SRParser.egg-info/
+-rw-rw-rw-   0        0        0     2584 2023-07-13 22:48:16.000000 SRParser-1.0.1/SRParser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-07-13 22:48:16.000000 SRParser-1.0.1/SRParser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 22:48:16.000000 SRParser-1.0.1/SRParser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 22:48:16.000000 SRParser-1.0.1/SRParser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-13 22:48:16.000000 SRParser-1.0.1/SRParser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-13 22:48:16.287485 SRParser-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2023-07-13 22:45:53.000000 SRParser-1.0.1/setup.py
```

### Comparing `SRParser-1.0.0/LICENSE` & `SRParser-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SRParser-1.0.0/PKG-INFO` & `SRParser-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: SRParser
-Version: 1.0.0
+Version: 1.0.1
 Summary: Parse and easily work with Snort rules.
 Home-page: https://www.github.com/jrbrawner/SnortParser
 Author: Joshua Brawner
 Author-email: jrbbrawner@gmail.com
 License: Apache Software License
 Keywords: snort rule parser
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Intro
-Snort rule tokenizer and parser written using PLY. This is my first tokenizer, parser and I may make improvements/changes as time goes on. The focus of this package currently is to allow programmatically working with snort rules, not necessarily detect the minutae of option combinations. If you have any suggestions, ideas, or improvements feel free to open an issue. Inspiration drawn from plyara. Thanks to David Beazley for his work on the PLY package.
+
+Snort rule tokenizer and parser written using PLY. This is my first tokenizer, parser and I may make improvements/changes as time goes on. The focus of this package currently is to allow programmatically working with snort rules, not necessarily detect the minutae of incorrect option combinations.
+
+If you have any suggestions, ideas, or improvements feel free to open an issue. Inspiration drawn from plyara. Thanks to David Beazley for his work on the PLY package.
 
 ## Usage
 
 ```python
 pip install SRParser
 ```
```

### Comparing `SRParser-1.0.0/README.md` & `SRParser-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 ## Intro
-Snort rule tokenizer and parser written using PLY. This is my first tokenizer, parser and I may make improvements/changes as time goes on. The focus of this package currently is to allow programmatically working with snort rules, not necessarily detect the minutae of option combinations. If you have any suggestions, ideas, or improvements feel free to open an issue. Inspiration drawn from plyara. Thanks to David Beazley for his work on the PLY package.
+
+Snort rule tokenizer and parser written using PLY. This is my first tokenizer, parser and I may make improvements/changes as time goes on. The focus of this package currently is to allow programmatically working with snort rules, not necessarily detect the minutae of incorrect option combinations.
+
+If you have any suggestions, ideas, or improvements feel free to open an issue. Inspiration drawn from plyara. Thanks to David Beazley for his work on the PLY package.
 
 ## Usage
 
 ```python
 pip install SRParser
 ```
```

### Comparing `SRParser-1.0.0/SRParser/SnortParser.py` & `SRParser-1.0.1/SRParser/SnortParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
     def t_newline(t: LexToken):
         r"\n+"
         t.lexer.lineno += len(t.value)
 
     # Error handling rule
     @staticmethod
     def t_error(t: LexToken):
-        print("Illegal character '%s'" % t.value[0])
+        #print("Illegal character '%s'" % t.value[0])
         t.lexer.skip(1)
 
     @staticmethod
     def t_ACTION(t: LexToken):
         r"(alert|block|drop|log|pass|react|reject|rewrite)"
         return t
```

### Comparing `SRParser-1.0.0/SRParser.egg-info/PKG-INFO` & `SRParser-1.0.1/SRParser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: SRParser
-Version: 1.0.0
+Version: 1.0.1
 Summary: Parse and easily work with Snort rules.
 Home-page: https://www.github.com/jrbrawner/SnortParser
 Author: Joshua Brawner
 Author-email: jrbbrawner@gmail.com
 License: Apache Software License
 Keywords: snort rule parser
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Intro
-Snort rule tokenizer and parser written using PLY. This is my first tokenizer, parser and I may make improvements/changes as time goes on. The focus of this package currently is to allow programmatically working with snort rules, not necessarily detect the minutae of option combinations. If you have any suggestions, ideas, or improvements feel free to open an issue. Inspiration drawn from plyara. Thanks to David Beazley for his work on the PLY package.
+
+Snort rule tokenizer and parser written using PLY. This is my first tokenizer, parser and I may make improvements/changes as time goes on. The focus of this package currently is to allow programmatically working with snort rules, not necessarily detect the minutae of incorrect option combinations.
+
+If you have any suggestions, ideas, or improvements feel free to open an issue. Inspiration drawn from plyara. Thanks to David Beazley for his work on the PLY package.
 
 ## Usage
 
 ```python
 pip install SRParser
 ```
```

### Comparing `SRParser-1.0.0/setup.py` & `SRParser-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "SRParser",
-    version = "1.0.0",
+    version = "1.0.1",
     author = "Joshua Brawner",
     author_email = "jrbbrawner@gmail.com",
     description = ("Parse and easily work with Snort rules."),
     license = "Apache Software License",
     keywords = "snort rule parser",
     long_description_content_type = 'text/markdown',
     url = "https://www.github.com/jrbrawner/SnortParser",
```

