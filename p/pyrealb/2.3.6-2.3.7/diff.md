# Comparing `tmp/pyrealb-2.3.6.tar.gz` & `tmp/pyrealb-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrealb-2.3.6.tar", last modified: Fri Jun 16 20:41:07 2023, max compression
+gzip compressed data, was "pyrealb-2.3.7.tar", last modified: Fri Jul 14 18:47:48 2023, max compression
```

## Comparing `pyrealb-2.3.6.tar` & `pyrealb-2.3.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.372591 pyrealb-2.3.6/
--rw-r--r--   0 lapalme    (503) staff       (20)    35129 2021-12-01 22:24:50.000000 pyrealb-2.3.6/LICENSE
--rw-r--r--   0 lapalme    (503) staff       (20)       23 2022-01-27 01:45:34.000000 pyrealb-2.3.6/MANIFEST.in
--rw-r--r--   0 lapalme    (503) staff       (20)     7578 2023-06-16 20:41:07.372663 pyrealb-2.3.6/PKG-INFO
--rw-r--r--   0 lapalme    (503) staff       (20)     7081 2023-06-16 20:39:39.000000 pyrealb-2.3.6/README.md
--rw-r--r--   0 lapalme    (503) staff       (20)      104 2021-12-13 01:31:17.000000 pyrealb-2.3.6/pyproject.toml
--rw-r--r--   0 lapalme    (503) staff       (20)      649 2023-06-16 20:41:07.372888 pyrealb-2.3.6/setup.cfg
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.361863 pyrealb-2.3.6/src/
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.365967 pyrealb-2.3.6/src/pyrealb/
--rw-r--r--   0 lapalme    (503) staff       (20)    44540 2023-05-24 14:55:41.000000 pyrealb-2.3.6/src/pyrealb/Constituent.py
--rw-r--r--   0 lapalme    (503) staff       (20)    41365 2023-06-16 20:26:39.000000 pyrealb-2.3.6/src/pyrealb/Dependent.py
--rw-r--r--   0 lapalme    (503) staff       (20)     3050 2023-05-24 14:52:06.000000 pyrealb-2.3.6/src/pyrealb/Lexicon.py
--rw-r--r--   0 lapalme    (503) staff       (20)     7609 2023-05-25 19:51:40.000000 pyrealb-2.3.6/src/pyrealb/Number.py
--rw-r--r--   0 lapalme    (503) staff       (20)    58433 2023-06-16 20:18:10.000000 pyrealb-2.3.6/src/pyrealb/Phrase.py
--rw-r--r--   0 lapalme    (503) staff       (20)    37991 2023-06-16 20:21:55.000000 pyrealb-2.3.6/src/pyrealb/Terminal.py
--rw-r--r--   0 lapalme    (503) staff       (20)    14266 2023-03-27 13:03:50.000000 pyrealb-2.3.6/src/pyrealb/Warning.py
--rw-r--r--   0 lapalme    (503) staff       (20)      857 2023-05-24 14:58:21.000000 pyrealb-2.3.6/src/pyrealb/__init__.py
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.368821 pyrealb-2.3.6/src/pyrealb/data/
--rw-r--r--   0 lapalme    (503) staff       (20)  1324966 2023-06-02 03:26:46.000000 pyrealb-2.3.6/src/pyrealb/data/lexicon-en.json
--rw-r--r--   0 lapalme    (503) staff       (20)  2479817 2023-05-25 18:45:57.000000 pyrealb-2.3.6/src/pyrealb/data/lexicon-fr.json
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.372068 pyrealb-2.3.6/src/pyrealb/data/pyrealb.egg-info/
--rw-r--r--   0 lapalme    (503) staff       (20)     4155 2022-01-26 22:41:53.000000 pyrealb-2.3.6/src/pyrealb/data/pyrealb.egg-info/PKG-INFO
--rw-r--r--   0 lapalme    (503) staff       (20)        0 2022-01-26 22:41:53.000000 pyrealb-2.3.6/src/pyrealb/data/pyrealb.egg-info/SOURCES.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        1 2022-01-26 22:41:53.000000 pyrealb-2.3.6/src/pyrealb/data/pyrealb.egg-info/dependency_links.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        8 2022-01-26 22:41:53.000000 pyrealb-2.3.6/src/pyrealb/data/pyrealb.egg-info/top_level.txt
--rw-r--r--   0 lapalme    (503) staff       (20)    85976 2023-05-24 15:04:29.000000 pyrealb-2.3.6/src/pyrealb/data/rules-en.json
--rw-r--r--   0 lapalme    (503) staff       (20)   173554 2022-06-14 19:51:41.000000 pyrealb-2.3.6/src/pyrealb/data/rules-fr.json
--rw-r--r--   0 lapalme    (503) staff       (20)     2953 2023-06-16 20:39:56.000000 pyrealb-2.3.6/src/pyrealb/utils.py
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.366482 pyrealb-2.3.6/src/pyrealb.egg-info/
--rw-r--r--   0 lapalme    (503) staff       (20)     7578 2023-06-16 20:41:07.000000 pyrealb-2.3.6/src/pyrealb.egg-info/PKG-INFO
--rw-r--r--   0 lapalme    (503) staff       (20)      756 2023-06-16 20:41:07.000000 pyrealb-2.3.6/src/pyrealb.egg-info/SOURCES.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        1 2023-06-16 20:41:07.000000 pyrealb-2.3.6/src/pyrealb.egg-info/dependency_links.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        8 2023-06-16 20:41:07.000000 pyrealb-2.3.6/src/pyrealb.egg-info/top_level.txt
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.372467 pyrealb-2.3.6/tests/
--rw-r--r--   0 lapalme    (503) staff       (20)     1879 2023-03-04 13:28:19.000000 pyrealb-2.3.6/tests/test.py
--rw-r--r--   0 lapalme    (503) staff       (20)     2870 2023-02-24 19:49:08.000000 pyrealb-2.3.6/tests/testAll.py
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-07-14 18:47:48.960945 pyrealb-2.3.7/
+-rw-r--r--   0 lapalme    (503) staff       (20)    35129 2021-12-01 22:24:50.000000 pyrealb-2.3.7/LICENSE
+-rw-r--r--   0 lapalme    (503) staff       (20)       23 2022-01-27 01:45:34.000000 pyrealb-2.3.7/MANIFEST.in
+-rw-r--r--   0 lapalme    (503) staff       (20)     7665 2023-07-14 18:47:48.960991 pyrealb-2.3.7/PKG-INFO
+-rw-r--r--   0 lapalme    (503) staff       (20)     7168 2023-07-14 18:47:19.000000 pyrealb-2.3.7/README.md
+-rw-r--r--   0 lapalme    (503) staff       (20)      104 2021-12-13 01:31:17.000000 pyrealb-2.3.7/pyproject.toml
+-rw-r--r--   0 lapalme    (503) staff       (20)      649 2023-07-14 18:47:48.961189 pyrealb-2.3.7/setup.cfg
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-07-14 18:47:48.955567 pyrealb-2.3.7/src/
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-07-14 18:47:48.957433 pyrealb-2.3.7/src/pyrealb/
+-rw-r--r--   0 lapalme    (503) staff       (20)    44540 2023-07-06 17:15:58.000000 pyrealb-2.3.7/src/pyrealb/Constituent.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    41365 2023-06-16 20:26:39.000000 pyrealb-2.3.7/src/pyrealb/Dependent.py
+-rw-r--r--   0 lapalme    (503) staff       (20)     3050 2023-05-24 14:52:06.000000 pyrealb-2.3.7/src/pyrealb/Lexicon.py
+-rw-r--r--   0 lapalme    (503) staff       (20)     7609 2023-05-25 19:51:40.000000 pyrealb-2.3.7/src/pyrealb/Number.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    58434 2023-07-06 19:57:56.000000 pyrealb-2.3.7/src/pyrealb/Phrase.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    38089 2023-07-07 20:14:49.000000 pyrealb-2.3.7/src/pyrealb/Terminal.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    14266 2023-03-27 13:03:50.000000 pyrealb-2.3.7/src/pyrealb/Warning.py
+-rw-r--r--   0 lapalme    (503) staff       (20)      857 2023-05-24 14:58:21.000000 pyrealb-2.3.7/src/pyrealb/__init__.py
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-07-14 18:47:48.960091 pyrealb-2.3.7/src/pyrealb/data/
+-rw-r--r--   0 lapalme    (503) staff       (20)  1324966 2023-06-02 03:26:46.000000 pyrealb-2.3.7/src/pyrealb/data/lexicon-en.json
+-rw-r--r--   0 lapalme    (503) staff       (20)  2479817 2023-05-25 18:45:57.000000 pyrealb-2.3.7/src/pyrealb/data/lexicon-fr.json
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-07-14 18:47:48.960611 pyrealb-2.3.7/src/pyrealb/data/pyrealb.egg-info/
+-rw-r--r--   0 lapalme    (503) staff       (20)     4155 2022-01-26 22:41:53.000000 pyrealb-2.3.7/src/pyrealb/data/pyrealb.egg-info/PKG-INFO
+-rw-r--r--   0 lapalme    (503) staff       (20)        0 2022-01-26 22:41:53.000000 pyrealb-2.3.7/src/pyrealb/data/pyrealb.egg-info/SOURCES.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        1 2022-01-26 22:41:53.000000 pyrealb-2.3.7/src/pyrealb/data/pyrealb.egg-info/dependency_links.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        8 2022-01-26 22:41:53.000000 pyrealb-2.3.7/src/pyrealb/data/pyrealb.egg-info/top_level.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)    85976 2023-05-24 15:04:29.000000 pyrealb-2.3.7/src/pyrealb/data/rules-en.json
+-rw-r--r--   0 lapalme    (503) staff       (20)   173554 2022-06-14 19:51:41.000000 pyrealb-2.3.7/src/pyrealb/data/rules-fr.json
+-rw-r--r--   0 lapalme    (503) staff       (20)     2953 2023-07-14 18:47:19.000000 pyrealb-2.3.7/src/pyrealb/utils.py
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-07-14 18:47:48.957916 pyrealb-2.3.7/src/pyrealb.egg-info/
+-rw-r--r--   0 lapalme    (503) staff       (20)     7665 2023-07-14 18:47:48.000000 pyrealb-2.3.7/src/pyrealb.egg-info/PKG-INFO
+-rw-r--r--   0 lapalme    (503) staff       (20)      756 2023-07-14 18:47:48.000000 pyrealb-2.3.7/src/pyrealb.egg-info/SOURCES.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        1 2023-07-14 18:47:48.000000 pyrealb-2.3.7/src/pyrealb.egg-info/dependency_links.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        8 2023-07-14 18:47:48.000000 pyrealb-2.3.7/src/pyrealb.egg-info/top_level.txt
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-07-14 18:47:48.960837 pyrealb-2.3.7/tests/
+-rw-r--r--   0 lapalme    (503) staff       (20)     1879 2023-03-04 13:28:19.000000 pyrealb-2.3.7/tests/test.py
+-rw-r--r--   0 lapalme    (503) staff       (20)     2870 2023-02-24 19:49:08.000000 pyrealb-2.3.7/tests/testAll.py
```

### Comparing `pyrealb-2.3.6/LICENSE` & `pyrealb-2.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/PKG-INFO` & `pyrealb-2.3.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyrealb
-Version: 2.3.6
+Version: 2.3.7
 Summary: A French-English text realizer
 Home-page: https://github.com/lapalme/pyrealb
 Author: Guy Lapalme
 Author-email: lapalme@iro.umontreal.ca
 Project-URL: Bug Tracker, https://github.com/lapalme/pyrealb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *pyRealB* - A Python Bilingual Text Realizer
 
-*Version 2.3.6 - June 2023*
+*Version 2.3.7 - July 2023*
 
 *pyRealB* is a Python adaptation of the JavaScript [**jsRealB**](http://rali.iro.umontreal.ca/jsRealB) 
 text realizer with the same constituent and dependency syntax notation. 
 It facilitates its integration within Python applications by simply adding
 
 	from pyrealb import *
 
@@ -91,14 +91,15 @@
 * [`tests`](./tests) : unit tests of special features of *pyRealB* in both French and English. Files have the pattern `*_{en|fr}.py`
     * `test.py`: simplistic function to check if a function returns the expected answer and display appropriate message
     * `testAll.html` : run this file to run all tests
 
 ## Demos
 
 * `99bottlesofbeer/99bottlesofbeer.py` : simple generation of a classic repetitive text in English.
+* `basketball/sportsettsum.py` : generation of French and English basketball summaries
 * `dev_example/dev_example.py`: examples of English and French expressions to be realized and checked against expected output,  
 useful for debugging when adding a new expression and enabling tracing
 * `evenementsDemo/evenements.py` : Description (in French) of a list of events, it creates HTML.
 * `flight_infos/README.md` : development of a RASA NLG server giving information about flights, aircrafts, etc...
 * `gophypi/amr2text.py` : generate a literal reading of an AMR (Abstract Meaning Representation);
                           [paper describing the approach](gophypi/Doc/GoPhiPy.pdf) 
 * `inflectionDemo/inflection.py` : French or English conjugation and declension of a form.
```

### Comparing `pyrealb-2.3.6/README.md` & `pyrealb-2.3.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # *pyRealB* - A Python Bilingual Text Realizer
 
-*Version 2.3.6 - June 2023*
+*Version 2.3.7 - July 2023*
 
 *pyRealB* is a Python adaptation of the JavaScript [**jsRealB**](http://rali.iro.umontreal.ca/jsRealB) 
 text realizer with the same constituent and dependency syntax notation. 
 It facilitates its integration within Python applications by simply adding
 
 	from pyrealb import *
 
@@ -76,14 +76,15 @@
 * [`tests`](./tests) : unit tests of special features of *pyRealB* in both French and English. Files have the pattern `*_{en|fr}.py`
     * `test.py`: simplistic function to check if a function returns the expected answer and display appropriate message
     * `testAll.html` : run this file to run all tests
 
 ## Demos
 
 * `99bottlesofbeer/99bottlesofbeer.py` : simple generation of a classic repetitive text in English.
+* `basketball/sportsettsum.py` : generation of French and English basketball summaries
 * `dev_example/dev_example.py`: examples of English and French expressions to be realized and checked against expected output,  
 useful for debugging when adding a new expression and enabling tracing
 * `evenementsDemo/evenements.py` : Description (in French) of a list of events, it creates HTML.
 * `flight_infos/README.md` : development of a RASA NLG server giving information about flights, aircrafts, etc...
 * `gophypi/amr2text.py` : generate a literal reading of an AMR (Abstract Meaning Representation);
                           [paper describing the approach](gophypi/Doc/GoPhiPy.pdf) 
 * `inflectionDemo/inflection.py` : French or English conjugation and declension of a form.
```

### Comparing `pyrealb-2.3.6/setup.cfg` & `pyrealb-2.3.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyrealb
-version = 2.3.6
+version = 2.3.7
 author = Guy Lapalme
 author_email = lapalme@iro.umontreal.ca
 description = A French-English text realizer
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/lapalme/pyrealb
 project_urls =
```

### Comparing `pyrealb-2.3.6/src/pyrealb/Constituent.py` & `pyrealb-2.3.7/src/pyrealb/Constituent.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/src/pyrealb/Dependent.py` & `pyrealb-2.3.7/src/pyrealb/Dependent.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/src/pyrealb/Lexicon.py` & `pyrealb-2.3.7/src/pyrealb/Lexicon.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/src/pyrealb/Number.py` & `pyrealb-2.3.7/src/pyrealb/Number.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/src/pyrealb/Phrase.py` & `pyrealb-2.3.7/src/pyrealb/Phrase.py`

 * *Files 0% similar despite different names*

```diff
@@ -986,15 +986,15 @@
                 self.pronoun.props["n"] = gn["n"]
                 self.pronoun.props["pe"] = gn["pe"]
         return self.doFormat(res)
 
     def real(self):
         res = []
         if self.isA("CP"):
-            res = self.cpReal()
+            return self.cpReal()
         else:
             self.pronominalizeChildren()
             if "typ" in self.props:
                 self.processTyp(self.props["typ"])
             for e in self.elements:
                 if e.isA("CP"):
                     r = e.cpReal()
```

### Comparing `pyrealb-2.3.6/src/pyrealb/Terminal.py` & `pyrealb-2.3.7/src/pyrealb/Terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                         "nat":True,"det":True,"rtime":False}
         elif terminalType=="NO":
             if not isinstance(lemma,(str,int,float)):
                 self.warn("bad parameter",["str","int","float"],type(lemma).__name__)
                 self.lemma=0
             elif isinstance(lemma,str):
                 lexInfo = getLemma(self.lemma)
-                if "value" in lexInfo:
+                if lexInfo is not None and "value" in lexInfo:
                     self.lemma=self.value=lexInfo["value"]
                     self.nbDecimals=0
                     self.props["dOpt"] = {"nat":True}
                     self.addOptSource("nat",True)
                     return
                 # check if this looks like a legal number
                 else:
@@ -152,15 +152,15 @@
                             self.setProp(key,info,True)
         else:
             self.warn("not implemented",terminalType)
     
     def grammaticalNumber(self):
         if not self.isA("NO"):
             return self.warn("bad application","grammaticalNumber","NO",self.constType)
-        if "ord" in self.props and self.props["ord"]==True:
+        if "dOpt" in self.props and "ord" in self.props["dOpt"] and self.props["dOpt"]["ord"]:
             return "s"
         number=self.value
         if self.isFr():
             # according to http:#bdl.oqlf.gouv.qc.ca/bdl/gabarit_bdl.asp?id=1582
             return "s" if -2<number<2 else "p"
         else:
             # according to https://www.chicagomanualofstyle.org/book/ed17/part2/ch09/psec019.html
@@ -376,15 +376,16 @@
                 if not pc.isA("VP"):  # unless it is VP stop at the first sentence
                     return False
             pc=pc.parentConst
         return False
 
     
     def conjugate_fr(self):
-        pe=int(self.getProp("pe"))
+        pe = self.getProp("pe")
+        pe = 3 if pe is None else int(pe)
         g = self.getProp("g")
         n = self.getProp("n")
         t = self.getProp("t")
         if self.tab is None:
             return [self.morphoError("conjugate_fr:tab",{"pe":pe,"n":n,"t":t})] 
         if t in ["pc","pq","cp","pa","fa","spa","spq","bp"]: # temps composés
             tempsAux={"pc":"p","pq":"i","cp":"c","pa":"ps","fa":"f","spa":"s","spq":"si","bp":"b"}[t]
```

### Comparing `pyrealb-2.3.6/src/pyrealb/Warning.py` & `pyrealb-2.3.7/src/pyrealb/Warning.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/src/pyrealb/__init__.py` & `pyrealb-2.3.7/src/pyrealb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/src/pyrealb/data/lexicon-en.json` & `pyrealb-2.3.7/src/pyrealb/data/lexicon-en.json`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/src/pyrealb/data/lexicon-fr.json` & `pyrealb-2.3.7/src/pyrealb/data/lexicon-fr.json`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/src/pyrealb/data/pyrealb.egg-info/PKG-INFO` & `pyrealb-2.3.7/src/pyrealb/data/pyrealb.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/src/pyrealb/data/rules-en.json` & `pyrealb-2.3.7/src/pyrealb/data/rules-en.json`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/src/pyrealb/data/rules-fr.json` & `pyrealb-2.3.7/src/pyrealb/data/rules-fr.json`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/src/pyrealb/utils.py` & `pyrealb-2.3.7/src/pyrealb/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,9 +71,9 @@
 
 # useful variables for using expressions written originally for the javascript version
 false = False
 true = True
 null = None
 
 # version and date informations
-pyrealb_version = "2.3.6"
+pyrealb_version = "2.3.7"
 pyrealb_datecreated = datetime.datetime.today()
```

### Comparing `pyrealb-2.3.6/src/pyrealb.egg-info/PKG-INFO` & `pyrealb-2.3.7/src/pyrealb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyrealb
-Version: 2.3.6
+Version: 2.3.7
 Summary: A French-English text realizer
 Home-page: https://github.com/lapalme/pyrealb
 Author: Guy Lapalme
 Author-email: lapalme@iro.umontreal.ca
 Project-URL: Bug Tracker, https://github.com/lapalme/pyrealb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *pyRealB* - A Python Bilingual Text Realizer
 
-*Version 2.3.6 - June 2023*
+*Version 2.3.7 - July 2023*
 
 *pyRealB* is a Python adaptation of the JavaScript [**jsRealB**](http://rali.iro.umontreal.ca/jsRealB) 
 text realizer with the same constituent and dependency syntax notation. 
 It facilitates its integration within Python applications by simply adding
 
 	from pyrealb import *
 
@@ -91,14 +91,15 @@
 * [`tests`](./tests) : unit tests of special features of *pyRealB* in both French and English. Files have the pattern `*_{en|fr}.py`
     * `test.py`: simplistic function to check if a function returns the expected answer and display appropriate message
     * `testAll.html` : run this file to run all tests
 
 ## Demos
 
 * `99bottlesofbeer/99bottlesofbeer.py` : simple generation of a classic repetitive text in English.
+* `basketball/sportsettsum.py` : generation of French and English basketball summaries
 * `dev_example/dev_example.py`: examples of English and French expressions to be realized and checked against expected output,  
 useful for debugging when adding a new expression and enabling tracing
 * `evenementsDemo/evenements.py` : Description (in French) of a list of events, it creates HTML.
 * `flight_infos/README.md` : development of a RASA NLG server giving information about flights, aircrafts, etc...
 * `gophypi/amr2text.py` : generate a literal reading of an AMR (Abstract Meaning Representation);
                           [paper describing the approach](gophypi/Doc/GoPhiPy.pdf) 
 * `inflectionDemo/inflection.py` : French or English conjugation and declension of a form.
```

### Comparing `pyrealb-2.3.6/src/pyrealb.egg-info/SOURCES.txt` & `pyrealb-2.3.7/src/pyrealb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/tests/test.py` & `pyrealb-2.3.7/tests/test.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.6/tests/testAll.py` & `pyrealb-2.3.7/tests/testAll.py`

 * *Files identical despite different names*

