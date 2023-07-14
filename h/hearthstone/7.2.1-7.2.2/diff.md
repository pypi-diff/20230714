# Comparing `tmp/hearthstone-7.2.1.tar.gz` & `tmp/hearthstone-7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-7.2.1.tar", last modified: Tue Jun 27 21:43:20 2023, max compression
+gzip compressed data, was "hearthstone-7.2.2.tar", last modified: Fri Jul 14 10:43:39 2023, max compression
```

## Comparing `hearthstone-7.2.1.tar` & `hearthstone-7.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:20.021071 hearthstone-7.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-27 21:43:13.000000 hearthstone-7.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-27 21:43:20.021071 hearthstone-7.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-27 21:43:13.000000 hearthstone-7.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:20.017071 hearthstone-7.2.1/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-27 21:43:13.000000 hearthstone-7.2.1/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-27 21:43:13.000000 hearthstone-7.2.1/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-06-27 21:43:13.000000 hearthstone-7.2.1/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-27 21:43:13.000000 hearthstone-7.2.1/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-27 21:43:13.000000 hearthstone-7.2.1/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-06-27 21:43:13.000000 hearthstone-7.2.1/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-06-27 21:43:13.000000 hearthstone-7.2.1/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-06-27 21:43:13.000000 hearthstone-7.2.1/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-27 21:43:13.000000 hearthstone-7.2.1/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-27 21:43:13.000000 hearthstone-7.2.1/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:20.021071 hearthstone-7.2.1/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-06-27 21:43:13.000000 hearthstone-7.2.1/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-27 21:43:13.000000 hearthstone-7.2.1/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:43:20.021071 hearthstone-7.2.1/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-27 21:43:19.000000 hearthstone-7.2.1/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-27 21:43:20.000000 hearthstone-7.2.1/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:43:19.000000 hearthstone-7.2.1/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 21:43:19.000000 hearthstone-7.2.1/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 21:43:19.000000 hearthstone-7.2.1/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:43:19.000000 hearthstone-7.2.1/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-27 21:43:20.021071 hearthstone-7.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-06-27 21:43:13.000000 hearthstone-7.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:43:39.641086 hearthstone-7.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-14 10:43:34.000000 hearthstone-7.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-14 10:43:39.641086 hearthstone-7.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-14 10:43:34.000000 hearthstone-7.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:43:39.637086 hearthstone-7.2.2/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61035 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:43:39.641086 hearthstone-7.2.2/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-14 10:43:34.000000 hearthstone-7.2.2/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:43:39.637086 hearthstone-7.2.2/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-14 10:43:39.000000 hearthstone-7.2.2/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-14 10:43:39.000000 hearthstone-7.2.2/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:43:39.000000 hearthstone-7.2.2/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 10:43:39.000000 hearthstone-7.2.2/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 10:43:39.000000 hearthstone-7.2.2/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:43:39.000000 hearthstone-7.2.2/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-14 10:43:39.641086 hearthstone-7.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-07-14 10:43:34.000000 hearthstone-7.2.2/setup.py
```

### Comparing `hearthstone-7.2.1/LICENSE` & `hearthstone-7.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.1/PKG-INFO` & `hearthstone-7.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 7.2.1
+Version: 7.2.2
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-7.2.1/README.md` & `hearthstone-7.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.1/hearthstone/bountyxml.py` & `hearthstone-7.2.2/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.1/hearthstone/cardxml.py` & `hearthstone-7.2.2/hearthstone/cardxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.1/hearthstone/dbf.py` & `hearthstone-7.2.2/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.1/hearthstone/deckstrings.py` & `hearthstone-7.2.2/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.1/hearthstone/entities.py` & `hearthstone-7.2.2/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.1/hearthstone/enums.py` & `hearthstone-7.2.2/hearthstone/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1116,14 +1116,15 @@
 			CardSet.THE_BARRENS,
 			CardSet.ALTERAC_VALLEY,
 			CardSet.LEGACY,
 			CardSet.THE_SUNKEN_CITY,
 			CardSet.RETURN_OF_THE_LICH_KING,
 			CardSet.PATH_OF_ARTHAS,
 			CardSet.BATTLE_OF_THE_BANDS,
+			CardSet.TITANS,
 		)
 
 	@property
 	def name_global(self):
 		# Newer sets use a 2-3 letter set code
 		from .utils import CARDSET_GLOBAL_STRING_MAP
 		custom = CARDSET_GLOBAL_STRING_MAP.get(self)
@@ -1135,15 +1136,15 @@
 
 	@property
 	def short_name_global(self):
 		return self.name_global + "_SHORT"
 
 	@property
 	def is_standard(self):
-		return self in ZodiacYear.HYDRA.standard_card_sets
+		return self in ZodiacYear.WOLF.standard_card_sets
 
 
 class CardType(IntEnum):
 	"""TAG_CARDTYPE"""
 
 	INVALID = 0
 	GAME = 1
```

### Comparing `hearthstone-7.2.1/hearthstone/mercenaryxml.py` & `hearthstone-7.2.2/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.1/hearthstone/stringsfile.py` & `hearthstone-7.2.2/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.1/hearthstone/utils/__init__.py` & `hearthstone-7.2.2/hearthstone/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.1/hearthstone/xmlutils.py` & `hearthstone-7.2.2/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.1/hearthstone.egg-info/PKG-INFO` & `hearthstone-7.2.2/hearthstone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 7.2.1
+Version: 7.2.2
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-7.2.1/hearthstone.egg-info/SOURCES.txt` & `hearthstone-7.2.2/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-7.2.1/setup.cfg` & `hearthstone-7.2.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 7.2.1
+version = 7.2.2
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

