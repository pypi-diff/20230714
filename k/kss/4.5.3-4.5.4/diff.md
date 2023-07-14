# Comparing `tmp/kss-4.5.3.tar.gz` & `tmp/kss-4.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kss-4.5.3.tar", last modified: Wed May 17 03:08:27 2023, max compression
+gzip compressed data, was "kss-4.5.4.tar", last modified: Fri Jul 14 06:17:44 2023, max compression
```

## Comparing `kss-4.5.3.tar` & `kss-4.5.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-17 03:08:27.052070 kss-4.5.3/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1559 2023-05-16 17:34:32.000000 kss-4.5.3/LICENSE
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    74968 2023-05-17 03:08:27.052238 kss-4.5.3/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    74225 2023-05-17 03:08:23.000000 kss-4.5.3/README.md
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-17 03:08:27.047989 kss-4.5.3/kss/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      423 2023-05-17 03:04:59.000000 kss-4.5.3/kss/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-17 03:08:27.049412 kss-4.5.3/kss/_elements/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      120 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_elements/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4879 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_elements/element.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2693 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_elements/empty.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      360 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_elements/subclasses.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-17 03:08:27.049536 kss-4.5.3/kss/_modules/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      120 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_modules/__init__.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-17 03:08:27.050072 kss-4.5.3/kss/_modules/morphemes/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      120 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_modules/morphemes/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2563 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_modules/morphemes/analyzers.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1693 2023-05-17 03:04:30.000000 kss-4.5.3/kss/_modules/morphemes/split_morphemes.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3394 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_modules/morphemes/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-17 03:08:27.050855 kss-4.5.3/kss/_modules/sentences/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      120 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_modules/sentences/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     9325 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_modules/sentences/embracing_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    22889 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_modules/sentences/sentence_postprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6777 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_modules/sentences/sentence_preprocessor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2289 2023-05-16 18:03:59.000000 kss-4.5.3/kss/_modules/sentences/sentence_processor.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    30233 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_modules/sentences/sentence_splitter.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6463 2023-05-16 18:03:11.000000 kss-4.5.3/kss/_modules/sentences/split_sentences.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-17 03:08:27.051300 kss-4.5.3/kss/_modules/summarization/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_modules/summarization/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      820 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_modules/summarization/sentence.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3600 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_modules/summarization/summarize_sentences.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2727 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_modules/summarization/utils.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-17 03:08:27.051965 kss-4.5.3/kss/_utils/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      120 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_utils/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    10244 2023-05-16 18:03:47.000000 kss-4.5.3/kss/_utils/const.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1399 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_utils/emojis.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      260 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_utils/logging.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      943 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_utils/multiprocessing.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    12934 2023-05-16 17:34:32.000000 kss-4.5.3/kss/_utils/sanity_checks.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-17 03:08:27.048985 kss-4.5.3/kss.egg-info/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)    74968 2023-05-17 03:08:27.000000 kss-4.5.3/kss.egg-info/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1101 2023-05-17 03:08:27.000000 kss-4.5.3/kss.egg-info/SOURCES.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2023-05-17 03:08:27.000000 kss-4.5.3/kss.egg-info/dependency_links.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2023-05-16 17:37:38.000000 kss-4.5.3/kss.egg-info/not-zip-safe
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       34 2023-05-17 03:08:27.000000 kss-4.5.3/kss.egg-info/requires.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        4 2023-05-17 03:08:27.000000 kss-4.5.3/kss.egg-info/top_level.txt
--rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2023-05-17 03:08:27.052485 kss-4.5.3/setup.cfg
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     2063 2023-05-16 17:34:32.000000 kss-4.5.3/setup.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-07-14 06:17:44.317999 kss-4.5.4/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1559 2023-05-16 17:34:32.000000 kss-4.5.4/LICENSE
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    75831 2023-07-14 06:17:44.318144 kss-4.5.4/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    75088 2023-07-14 06:17:00.000000 kss-4.5.4/README.md
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-07-14 06:17:44.312089 kss-4.5.4/kss/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      423 2023-07-14 06:17:25.000000 kss-4.5.4/kss/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-07-14 06:17:44.313570 kss-4.5.4/kss/_elements/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      120 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_elements/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4879 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_elements/element.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2693 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_elements/empty.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      360 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_elements/subclasses.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-07-14 06:17:44.313749 kss-4.5.4/kss/_modules/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      120 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_modules/__init__.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-07-14 06:17:44.314400 kss-4.5.4/kss/_modules/morphemes/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      120 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_modules/morphemes/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2563 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_modules/morphemes/analyzers.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1693 2023-05-17 03:04:30.000000 kss-4.5.4/kss/_modules/morphemes/split_morphemes.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3394 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_modules/morphemes/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-07-14 06:17:44.316352 kss-4.5.4/kss/_modules/sentences/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      120 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_modules/sentences/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     9325 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_modules/sentences/embracing_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    22889 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_modules/sentences/sentence_postprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6777 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_modules/sentences/sentence_preprocessor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2289 2023-05-16 18:03:59.000000 kss-4.5.4/kss/_modules/sentences/sentence_processor.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    30233 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_modules/sentences/sentence_splitter.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6463 2023-05-16 18:03:11.000000 kss-4.5.4/kss/_modules/sentences/split_sentences.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-07-14 06:17:44.316935 kss-4.5.4/kss/_modules/summarization/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        0 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_modules/summarization/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      820 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_modules/summarization/sentence.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3600 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_modules/summarization/summarize_sentences.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2727 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_modules/summarization/utils.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-07-14 06:17:44.317872 kss-4.5.4/kss/_utils/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      120 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_utils/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    10244 2023-05-16 18:03:47.000000 kss-4.5.4/kss/_utils/const.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1399 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_utils/emojis.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      260 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_utils/logging.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      992 2023-07-14 06:17:00.000000 kss-4.5.4/kss/_utils/multiprocessing.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    12934 2023-05-16 17:34:32.000000 kss-4.5.4/kss/_utils/sanity_checks.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-07-14 06:17:44.312892 kss-4.5.4/kss.egg-info/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)    75831 2023-07-14 06:17:44.000000 kss-4.5.4/kss.egg-info/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1101 2023-07-14 06:17:44.000000 kss-4.5.4/kss.egg-info/SOURCES.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2023-07-14 06:17:44.000000 kss-4.5.4/kss.egg-info/dependency_links.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2023-05-16 17:37:38.000000 kss-4.5.4/kss.egg-info/not-zip-safe
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       34 2023-07-14 06:17:44.000000 kss-4.5.4/kss.egg-info/requires.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        4 2023-07-14 06:17:44.000000 kss-4.5.4/kss.egg-info/top_level.txt
+-rwxr-xr-x   0 hyunwoongko   (501) staff       (20)      160 2023-07-14 06:17:44.318346 kss-4.5.4/setup.cfg
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     2063 2023-05-16 17:34:32.000000 kss-4.5.4/setup.py
```

### Comparing `kss-4.5.3/LICENSE` & `kss-4.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/PKG-INFO` & `kss-4.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kss
-Version: 4.5.3
+Version: 4.5.4
 Summary: A Toolkit for Korean sentence segmentation
 Home-page: https://github.com/hyunwoongko/kss
 Author: Hyunwoong Ko
 Author-email: kevin.ko@tunib.ai
 License: BSD 3-Clause "New" or "Revised" License
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -830,14 +830,23 @@
   
   text = "회사 동료 분들과 다녀왔는데 분위기도 좋고 음식도 맛있었어요\n다만,\t강남 토끼정이 강남 쉑쉑버거 골목길로 쭉 올라가야 하는데 다들 쉑쉑버거의 유혹에 넘어갈 뻔 했답니다 강남역 맛집 토끼정의 외부 모습."
 
   kss.split_morphemes(text, drop_space=False)
   # [('회사', 'NNG'), (' ', 'SP'), ('동료', 'NNG'), (' ', 'SP'), ('분', 'NNB'), ('들', 'XSN'), ('과', 'JKB'), (' ', 'SP'), ('다녀왔', 'VV+EP'), ('는데', 'EC'), (' ', 'SP'), ('분위기', 'NNG'), ('도', 'JX'), (' ', 'SP'), ('좋', 'VA'), ('고', 'EC'), (' ', 'SP'), ('음식', 'NNG'), ('도', 'JX'), (' ', 'SP'), ('맛있', 'VA'), ('었', 'EP'), ('어요', 'EF'), ('\n', 'SP'), ('다만', 'MAJ'), (',', 'SC'), ('\t', 'SP'), ('강남', 'NNP'), (' ', 'SP'), ('토끼', 'NNG'), ('정', 'NNG'), ('이', 'JKS'), (' ', 'SP'), ('강남', 'NNP'), (' ', 'SP'), ('쉑쉑', 'MAG'), ('버거', 'NNG'), (' ', 'SP'), ('골목길', 'NNG'), ('로', 'JKB'), (' ', 'SP'), ('쭉', 'MAG'), (' ', 'SP'), ('올라가', 'VV'), ('야', 'EC'), (' ', 'SP'), ('하', 'VV'), ('는데', 'EC'), (' ', 'SP'), ('다', 'MAG'), ('들', 'XSN'), (' ', 'SP'), ('쉑쉑', 'MAG'), ('버거', 'NNG'), ('의', 'JKG'), (' ', 'SP'), ('유혹', 'NNG'), ('에', 'JKB'), (' ', 'SP'), ('넘어갈', 'VV+ETM'), (' ', 'SP'), ('뻔', 'NNB'), (' ', 'SP'), ('했', 'VV+EP'), ('답니다', 'EC'), (' ', 'SP'), ('강남역', 'NNP'), (' ', 'SP'), ('맛집', 'NNG'), (' ', 'SP'), ('토끼', 'NNG'), ('정의', 'NNG'), (' ', 'SP'), ('외부', 'NNG'), (' ', 'SP'), ('모습', 'NNG'), ('.', 'SF')]
   ```
 
+- Get result without POS tagging.
+  ```python
+  import kss
+  
+  text = "회사 동료 분들과 다녀왔는데 분위기도 좋고 음식도 맛있었어요\n다만,\t강남 토끼정이 강남 쉑쉑버거 골목길로 쭉 올라가야 하는데 다들 쉑쉑버거의 유혹에 넘어갈 뻔 했답니다 강남역 맛집 토끼정의 외부 모습."
+
+  kss.split_morphemes(text, return_pos=False)
+  # ['회사', '동료', '분', '들', '과', '다녀왔', '는데', '분위기', '도', '좋', '고', '음식', '도', '맛있', '었', '어요', '다만', ',', '강남', '토끼', '정', '이', '강남', '쉑쉑', '버거', '골목길', '로', '쭉', '올라가', '야', '하', '는데', '다', '들', '쉑쉑', '버거', '의', '유혹', '에', '넘어갈', '뻔', '했', '답니다', '강남역', '맛집', '토끼', '정의', '외부', '모습', '.']
+  ```
 </details>
 
 <br>
 
 
 #### 3) `summarize_sentences`: summarize text into important sentences
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kss Version: 4.5.3 Summary: A Toolkit for Korean
+Metadata-Version: 2.1 Name: kss Version: 4.5.4 Summary: A Toolkit for Korean
 sentence segmentation Home-page: https://github.com/hyunwoongko/kss Author:
 Hyunwoong Ko Author-email: kevin.ko@tunib.ai License: BSD 3-Clause "New" or
 "Revised" License Platform: any Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2 Classifier: Programming
 Language :: Python :: 3.3 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
@@ -737,15 +737,27 @@
 (' ', 'SP'), ('ì­', 'MAG'), (' ', 'SP'), ('ì¬ë¼ê°', 'VV'), ('ì¼', 'EC'),
 (' ', 'SP'), ('í', 'VV'), ('ëë°', 'EC'), (' ', 'SP'), ('ë¤', 'MAG'),
 ('ë¤', 'XSN'), (' ', 'SP'), ('ìì', 'MAG'), ('ë²ê±°', 'NNG'), ('ì',
 'JKG'), (' ', 'SP'), ('ì í¹', 'NNG'), ('ì', 'JKB'), (' ', 'SP'),
 ('ëì´ê°', 'VV+ETM'), (' ', 'SP'), ('ë»', 'NNB'), (' ', 'SP'), ('í',
 'VV+EP'), ('ëµëë¤', 'EC'), (' ', 'SP'), ('ê°ë¨ì­', 'NNP'), (' ', 'SP'),
 ('ë§ì§', 'NNG'), (' ', 'SP'), ('í ë¼', 'NNG'), ('ì ì', 'NNG'), (' ',
-'SP'), ('ì¸ë¶', 'NNG'), (' ', 'SP'), ('ëª¨ìµ', 'NNG'), ('.', 'SF')] ```
+'SP'), ('ì¸ë¶', 'NNG'), (' ', 'SP'), ('ëª¨ìµ', 'NNG'), ('.', 'SF')] ``` -
+Get result without POS tagging. ```python import kss text = "íì¬ ëë£
+ë¶ë¤ê³¼ ë¤ëìëë° ë¶ìê¸°ë ì¢ê³  ììë
+ë§ììì´ì\në¤ë§,\tê°ë¨ í ë¼ì ì´ ê°ë¨ ììë²ê±° ê³¨ëª©ê¸¸ë¡
+ì­ ì¬ë¼ê°ì¼ íëë° ë¤ë¤ ììë²ê±°ì ì í¹ì ëì´ê° ë»
+íëµëë¤ ê°ë¨ì­ ë§ì§ í ë¼ì ì ì¸ë¶ ëª¨ìµ." kss.split_morphemes
+(text, return_pos=False) # ['íì¬', 'ëë£', 'ë¶', 'ë¤', 'ê³¼',
+'ë¤ëì', 'ëë°', 'ë¶ìê¸°', 'ë', 'ì¢', 'ê³ ', 'ìì', 'ë',
+'ë§ì', 'ì', 'ì´ì', 'ë¤ë§', ',', 'ê°ë¨', 'í ë¼', 'ì ', 'ì´',
+'ê°ë¨', 'ìì', 'ë²ê±°', 'ê³¨ëª©ê¸¸', 'ë¡', 'ì­', 'ì¬ë¼ê°', 'ì¼',
+'í', 'ëë°', 'ë¤', 'ë¤', 'ìì', 'ë²ê±°', 'ì', 'ì í¹', 'ì',
+'ëì´ê°', 'ë»', 'í', 'ëµëë¤', 'ê°ë¨ì­', 'ë§ì§', 'í ë¼',
+'ì ì', 'ì¸ë¶', 'ëª¨ìµ', '.'] ```
 #### 3) `summarize_sentences`: summarize text into important sentences
 ```python from kss import summarize_sentences summarize_sentences( text: Union
 [str, List[str], Tuple[str]], backend: str = "auto", num_workers: Union[int,
 str] = "auto", max_sentences: int = 3, tolerance: float: 0.05, strip: bool =
 True, ignores: List[str] = None, ) ```  Parameters - **text: String or List/
 Tuple of strings** - string: single text segmentation - list/tuple of strings:
 batch texts segmentation - **backend: Morpheme analyzer backend.** -
```

### Comparing `kss-4.5.3/README.md` & `kss-4.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -809,14 +809,23 @@
   
   text = "회사 동료 분들과 다녀왔는데 분위기도 좋고 음식도 맛있었어요\n다만,\t강남 토끼정이 강남 쉑쉑버거 골목길로 쭉 올라가야 하는데 다들 쉑쉑버거의 유혹에 넘어갈 뻔 했답니다 강남역 맛집 토끼정의 외부 모습."
 
   kss.split_morphemes(text, drop_space=False)
   # [('회사', 'NNG'), (' ', 'SP'), ('동료', 'NNG'), (' ', 'SP'), ('분', 'NNB'), ('들', 'XSN'), ('과', 'JKB'), (' ', 'SP'), ('다녀왔', 'VV+EP'), ('는데', 'EC'), (' ', 'SP'), ('분위기', 'NNG'), ('도', 'JX'), (' ', 'SP'), ('좋', 'VA'), ('고', 'EC'), (' ', 'SP'), ('음식', 'NNG'), ('도', 'JX'), (' ', 'SP'), ('맛있', 'VA'), ('었', 'EP'), ('어요', 'EF'), ('\n', 'SP'), ('다만', 'MAJ'), (',', 'SC'), ('\t', 'SP'), ('강남', 'NNP'), (' ', 'SP'), ('토끼', 'NNG'), ('정', 'NNG'), ('이', 'JKS'), (' ', 'SP'), ('강남', 'NNP'), (' ', 'SP'), ('쉑쉑', 'MAG'), ('버거', 'NNG'), (' ', 'SP'), ('골목길', 'NNG'), ('로', 'JKB'), (' ', 'SP'), ('쭉', 'MAG'), (' ', 'SP'), ('올라가', 'VV'), ('야', 'EC'), (' ', 'SP'), ('하', 'VV'), ('는데', 'EC'), (' ', 'SP'), ('다', 'MAG'), ('들', 'XSN'), (' ', 'SP'), ('쉑쉑', 'MAG'), ('버거', 'NNG'), ('의', 'JKG'), (' ', 'SP'), ('유혹', 'NNG'), ('에', 'JKB'), (' ', 'SP'), ('넘어갈', 'VV+ETM'), (' ', 'SP'), ('뻔', 'NNB'), (' ', 'SP'), ('했', 'VV+EP'), ('답니다', 'EC'), (' ', 'SP'), ('강남역', 'NNP'), (' ', 'SP'), ('맛집', 'NNG'), (' ', 'SP'), ('토끼', 'NNG'), ('정의', 'NNG'), (' ', 'SP'), ('외부', 'NNG'), (' ', 'SP'), ('모습', 'NNG'), ('.', 'SF')]
   ```
 
+- Get result without POS tagging.
+  ```python
+  import kss
+  
+  text = "회사 동료 분들과 다녀왔는데 분위기도 좋고 음식도 맛있었어요\n다만,\t강남 토끼정이 강남 쉑쉑버거 골목길로 쭉 올라가야 하는데 다들 쉑쉑버거의 유혹에 넘어갈 뻔 했답니다 강남역 맛집 토끼정의 외부 모습."
+
+  kss.split_morphemes(text, return_pos=False)
+  # ['회사', '동료', '분', '들', '과', '다녀왔', '는데', '분위기', '도', '좋', '고', '음식', '도', '맛있', '었', '어요', '다만', ',', '강남', '토끼', '정', '이', '강남', '쉑쉑', '버거', '골목길', '로', '쭉', '올라가', '야', '하', '는데', '다', '들', '쉑쉑', '버거', '의', '유혹', '에', '넘어갈', '뻔', '했', '답니다', '강남역', '맛집', '토끼', '정의', '외부', '모습', '.']
+  ```
 </details>
 
 <br>
 
 
 #### 3) `summarize_sentences`: summarize text into important sentences
```

#### html2text {}

```diff
@@ -727,15 +727,27 @@
 (' ', 'SP'), ('ì­', 'MAG'), (' ', 'SP'), ('ì¬ë¼ê°', 'VV'), ('ì¼', 'EC'),
 (' ', 'SP'), ('í', 'VV'), ('ëë°', 'EC'), (' ', 'SP'), ('ë¤', 'MAG'),
 ('ë¤', 'XSN'), (' ', 'SP'), ('ìì', 'MAG'), ('ë²ê±°', 'NNG'), ('ì',
 'JKG'), (' ', 'SP'), ('ì í¹', 'NNG'), ('ì', 'JKB'), (' ', 'SP'),
 ('ëì´ê°', 'VV+ETM'), (' ', 'SP'), ('ë»', 'NNB'), (' ', 'SP'), ('í',
 'VV+EP'), ('ëµëë¤', 'EC'), (' ', 'SP'), ('ê°ë¨ì­', 'NNP'), (' ', 'SP'),
 ('ë§ì§', 'NNG'), (' ', 'SP'), ('í ë¼', 'NNG'), ('ì ì', 'NNG'), (' ',
-'SP'), ('ì¸ë¶', 'NNG'), (' ', 'SP'), ('ëª¨ìµ', 'NNG'), ('.', 'SF')] ```
+'SP'), ('ì¸ë¶', 'NNG'), (' ', 'SP'), ('ëª¨ìµ', 'NNG'), ('.', 'SF')] ``` -
+Get result without POS tagging. ```python import kss text = "íì¬ ëë£
+ë¶ë¤ê³¼ ë¤ëìëë° ë¶ìê¸°ë ì¢ê³  ììë
+ë§ììì´ì\në¤ë§,\tê°ë¨ í ë¼ì ì´ ê°ë¨ ììë²ê±° ê³¨ëª©ê¸¸ë¡
+ì­ ì¬ë¼ê°ì¼ íëë° ë¤ë¤ ììë²ê±°ì ì í¹ì ëì´ê° ë»
+íëµëë¤ ê°ë¨ì­ ë§ì§ í ë¼ì ì ì¸ë¶ ëª¨ìµ." kss.split_morphemes
+(text, return_pos=False) # ['íì¬', 'ëë£', 'ë¶', 'ë¤', 'ê³¼',
+'ë¤ëì', 'ëë°', 'ë¶ìê¸°', 'ë', 'ì¢', 'ê³ ', 'ìì', 'ë',
+'ë§ì', 'ì', 'ì´ì', 'ë¤ë§', ',', 'ê°ë¨', 'í ë¼', 'ì ', 'ì´',
+'ê°ë¨', 'ìì', 'ë²ê±°', 'ê³¨ëª©ê¸¸', 'ë¡', 'ì­', 'ì¬ë¼ê°', 'ì¼',
+'í', 'ëë°', 'ë¤', 'ë¤', 'ìì', 'ë²ê±°', 'ì', 'ì í¹', 'ì',
+'ëì´ê°', 'ë»', 'í', 'ëµëë¤', 'ê°ë¨ì­', 'ë§ì§', 'í ë¼',
+'ì ì', 'ì¸ë¶', 'ëª¨ìµ', '.'] ```
 #### 3) `summarize_sentences`: summarize text into important sentences
 ```python from kss import summarize_sentences summarize_sentences( text: Union
 [str, List[str], Tuple[str]], backend: str = "auto", num_workers: Union[int,
 str] = "auto", max_sentences: int = 3, tolerance: float: 0.05, strip: bool =
 True, ignores: List[str] = None, ) ```  Parameters - **text: String or List/
 Tuple of strings** - string: single text segmentation - list/tuple of strings:
 batch texts segmentation - **backend: Morpheme analyzer backend.** -
```

### Comparing `kss-4.5.3/kss/_elements/element.py` & `kss-4.5.4/kss/_elements/element.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_elements/empty.py` & `kss-4.5.4/kss/_elements/empty.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_modules/morphemes/analyzers.py` & `kss-4.5.4/kss/_modules/morphemes/analyzers.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_modules/morphemes/split_morphemes.py` & `kss-4.5.4/kss/_modules/morphemes/split_morphemes.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_modules/morphemes/utils.py` & `kss-4.5.4/kss/_modules/morphemes/utils.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_modules/sentences/embracing_processor.py` & `kss-4.5.4/kss/_modules/sentences/embracing_processor.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_modules/sentences/sentence_postprocessor.py` & `kss-4.5.4/kss/_modules/sentences/sentence_postprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_modules/sentences/sentence_preprocessor.py` & `kss-4.5.4/kss/_modules/sentences/sentence_preprocessor.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_modules/sentences/sentence_processor.py` & `kss-4.5.4/kss/_modules/sentences/sentence_processor.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_modules/sentences/sentence_splitter.py` & `kss-4.5.4/kss/_modules/sentences/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_modules/sentences/split_sentences.py` & `kss-4.5.4/kss/_modules/sentences/split_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_modules/summarization/sentence.py` & `kss-4.5.4/kss/_modules/summarization/sentence.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_modules/summarization/summarize_sentences.py` & `kss-4.5.4/kss/_modules/summarization/summarize_sentences.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_modules/summarization/utils.py` & `kss-4.5.4/kss/_modules/summarization/utils.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_utils/const.py` & `kss-4.5.4/kss/_utils/const.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_utils/emojis.py` & `kss-4.5.4/kss/_utils/emojis.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss/_utils/multiprocessing.py` & `kss-4.5.4/kss/_utils/multiprocessing.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,8 +26,10 @@
             output = func(inputs)
         else:
             output = [func(i) for i in inputs]
         return output
     else:
         with mp.Pool(num_workers) as pool:
             output = pool.map(func, inputs)
+            pool.close()
+            pool.join()
             return output
```

### Comparing `kss-4.5.3/kss/_utils/sanity_checks.py` & `kss-4.5.4/kss/_utils/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/kss.egg-info/PKG-INFO` & `kss-4.5.4/kss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kss
-Version: 4.5.3
+Version: 4.5.4
 Summary: A Toolkit for Korean sentence segmentation
 Home-page: https://github.com/hyunwoongko/kss
 Author: Hyunwoong Ko
 Author-email: kevin.ko@tunib.ai
 License: BSD 3-Clause "New" or "Revised" License
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -830,14 +830,23 @@
   
   text = "회사 동료 분들과 다녀왔는데 분위기도 좋고 음식도 맛있었어요\n다만,\t강남 토끼정이 강남 쉑쉑버거 골목길로 쭉 올라가야 하는데 다들 쉑쉑버거의 유혹에 넘어갈 뻔 했답니다 강남역 맛집 토끼정의 외부 모습."
 
   kss.split_morphemes(text, drop_space=False)
   # [('회사', 'NNG'), (' ', 'SP'), ('동료', 'NNG'), (' ', 'SP'), ('분', 'NNB'), ('들', 'XSN'), ('과', 'JKB'), (' ', 'SP'), ('다녀왔', 'VV+EP'), ('는데', 'EC'), (' ', 'SP'), ('분위기', 'NNG'), ('도', 'JX'), (' ', 'SP'), ('좋', 'VA'), ('고', 'EC'), (' ', 'SP'), ('음식', 'NNG'), ('도', 'JX'), (' ', 'SP'), ('맛있', 'VA'), ('었', 'EP'), ('어요', 'EF'), ('\n', 'SP'), ('다만', 'MAJ'), (',', 'SC'), ('\t', 'SP'), ('강남', 'NNP'), (' ', 'SP'), ('토끼', 'NNG'), ('정', 'NNG'), ('이', 'JKS'), (' ', 'SP'), ('강남', 'NNP'), (' ', 'SP'), ('쉑쉑', 'MAG'), ('버거', 'NNG'), (' ', 'SP'), ('골목길', 'NNG'), ('로', 'JKB'), (' ', 'SP'), ('쭉', 'MAG'), (' ', 'SP'), ('올라가', 'VV'), ('야', 'EC'), (' ', 'SP'), ('하', 'VV'), ('는데', 'EC'), (' ', 'SP'), ('다', 'MAG'), ('들', 'XSN'), (' ', 'SP'), ('쉑쉑', 'MAG'), ('버거', 'NNG'), ('의', 'JKG'), (' ', 'SP'), ('유혹', 'NNG'), ('에', 'JKB'), (' ', 'SP'), ('넘어갈', 'VV+ETM'), (' ', 'SP'), ('뻔', 'NNB'), (' ', 'SP'), ('했', 'VV+EP'), ('답니다', 'EC'), (' ', 'SP'), ('강남역', 'NNP'), (' ', 'SP'), ('맛집', 'NNG'), (' ', 'SP'), ('토끼', 'NNG'), ('정의', 'NNG'), (' ', 'SP'), ('외부', 'NNG'), (' ', 'SP'), ('모습', 'NNG'), ('.', 'SF')]
   ```
 
+- Get result without POS tagging.
+  ```python
+  import kss
+  
+  text = "회사 동료 분들과 다녀왔는데 분위기도 좋고 음식도 맛있었어요\n다만,\t강남 토끼정이 강남 쉑쉑버거 골목길로 쭉 올라가야 하는데 다들 쉑쉑버거의 유혹에 넘어갈 뻔 했답니다 강남역 맛집 토끼정의 외부 모습."
+
+  kss.split_morphemes(text, return_pos=False)
+  # ['회사', '동료', '분', '들', '과', '다녀왔', '는데', '분위기', '도', '좋', '고', '음식', '도', '맛있', '었', '어요', '다만', ',', '강남', '토끼', '정', '이', '강남', '쉑쉑', '버거', '골목길', '로', '쭉', '올라가', '야', '하', '는데', '다', '들', '쉑쉑', '버거', '의', '유혹', '에', '넘어갈', '뻔', '했', '답니다', '강남역', '맛집', '토끼', '정의', '외부', '모습', '.']
+  ```
 </details>
 
 <br>
 
 
 #### 3) `summarize_sentences`: summarize text into important sentences
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kss Version: 4.5.3 Summary: A Toolkit for Korean
+Metadata-Version: 2.1 Name: kss Version: 4.5.4 Summary: A Toolkit for Korean
 sentence segmentation Home-page: https://github.com/hyunwoongko/kss Author:
 Hyunwoong Ko Author-email: kevin.ko@tunib.ai License: BSD 3-Clause "New" or
 "Revised" License Platform: any Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2 Classifier: Programming
 Language :: Python :: 3.3 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
@@ -737,15 +737,27 @@
 (' ', 'SP'), ('ì­', 'MAG'), (' ', 'SP'), ('ì¬ë¼ê°', 'VV'), ('ì¼', 'EC'),
 (' ', 'SP'), ('í', 'VV'), ('ëë°', 'EC'), (' ', 'SP'), ('ë¤', 'MAG'),
 ('ë¤', 'XSN'), (' ', 'SP'), ('ìì', 'MAG'), ('ë²ê±°', 'NNG'), ('ì',
 'JKG'), (' ', 'SP'), ('ì í¹', 'NNG'), ('ì', 'JKB'), (' ', 'SP'),
 ('ëì´ê°', 'VV+ETM'), (' ', 'SP'), ('ë»', 'NNB'), (' ', 'SP'), ('í',
 'VV+EP'), ('ëµëë¤', 'EC'), (' ', 'SP'), ('ê°ë¨ì­', 'NNP'), (' ', 'SP'),
 ('ë§ì§', 'NNG'), (' ', 'SP'), ('í ë¼', 'NNG'), ('ì ì', 'NNG'), (' ',
-'SP'), ('ì¸ë¶', 'NNG'), (' ', 'SP'), ('ëª¨ìµ', 'NNG'), ('.', 'SF')] ```
+'SP'), ('ì¸ë¶', 'NNG'), (' ', 'SP'), ('ëª¨ìµ', 'NNG'), ('.', 'SF')] ``` -
+Get result without POS tagging. ```python import kss text = "íì¬ ëë£
+ë¶ë¤ê³¼ ë¤ëìëë° ë¶ìê¸°ë ì¢ê³  ììë
+ë§ììì´ì\në¤ë§,\tê°ë¨ í ë¼ì ì´ ê°ë¨ ììë²ê±° ê³¨ëª©ê¸¸ë¡
+ì­ ì¬ë¼ê°ì¼ íëë° ë¤ë¤ ììë²ê±°ì ì í¹ì ëì´ê° ë»
+íëµëë¤ ê°ë¨ì­ ë§ì§ í ë¼ì ì ì¸ë¶ ëª¨ìµ." kss.split_morphemes
+(text, return_pos=False) # ['íì¬', 'ëë£', 'ë¶', 'ë¤', 'ê³¼',
+'ë¤ëì', 'ëë°', 'ë¶ìê¸°', 'ë', 'ì¢', 'ê³ ', 'ìì', 'ë',
+'ë§ì', 'ì', 'ì´ì', 'ë¤ë§', ',', 'ê°ë¨', 'í ë¼', 'ì ', 'ì´',
+'ê°ë¨', 'ìì', 'ë²ê±°', 'ê³¨ëª©ê¸¸', 'ë¡', 'ì­', 'ì¬ë¼ê°', 'ì¼',
+'í', 'ëë°', 'ë¤', 'ë¤', 'ìì', 'ë²ê±°', 'ì', 'ì í¹', 'ì',
+'ëì´ê°', 'ë»', 'í', 'ëµëë¤', 'ê°ë¨ì­', 'ë§ì§', 'í ë¼',
+'ì ì', 'ì¸ë¶', 'ëª¨ìµ', '.'] ```
 #### 3) `summarize_sentences`: summarize text into important sentences
 ```python from kss import summarize_sentences summarize_sentences( text: Union
 [str, List[str], Tuple[str]], backend: str = "auto", num_workers: Union[int,
 str] = "auto", max_sentences: int = 3, tolerance: float: 0.05, strip: bool =
 True, ignores: List[str] = None, ) ```  Parameters - **text: String or List/
 Tuple of strings** - string: single text segmentation - list/tuple of strings:
 batch texts segmentation - **backend: Morpheme analyzer backend.** -
```

### Comparing `kss-4.5.3/kss.egg-info/SOURCES.txt` & `kss-4.5.4/kss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kss-4.5.3/setup.py` & `kss-4.5.4/setup.py`

 * *Files identical despite different names*

