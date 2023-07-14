# Comparing `tmp/drug_list_ner-0.0.4.tar.gz` & `tmp/drug_list_ner-0.0.5.tar.gz`

## Comparing `drug_list_ner-0.0.4.tar` & `drug_list_ner-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/.DS_Store
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/Pipfile
--rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/Pipfile.lock
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/pyvenv.cfg
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/requirements.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/src/drug_list_ner/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/src/drug_list_ner/__init__.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/src/drug_list_ner/example.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/src/drug_list_ner/model2/.DS_Store
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/src/drug_list_ner/model2/config.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/src/drug_list_ner/tokenizer2/special_tokens_map.json
--rw-r--r--   0        0        0   716830 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/src/drug_list_ner/tokenizer2/tokenizer.json
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/src/drug_list_ner/tokenizer2/tokenizer_config.json
--rw-r--r--   0        0        0   227845 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/src/drug_list_ner/tokenizer2/vocab.txt
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/LICENSE
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/README.md
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 drug_list_ner-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/.DS_Store
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/Pipfile
+-rw-r--r--   0        0        0    33004 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/Pipfile.lock
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/pyvenv.cfg
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/src/drug_list_ner/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/src/drug_list_ner/__init__.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/src/drug_list_ner/example.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/src/drug_list_ner/model2/.DS_Store
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/src/drug_list_ner/model2/config.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/src/drug_list_ner/tokenizer2/special_tokens_map.json
+-rw-r--r--   0        0        0   716830 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/src/drug_list_ner/tokenizer2/tokenizer.json
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/src/drug_list_ner/tokenizer2/tokenizer_config.json
+-rw-r--r--   0        0        0   227845 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/src/drug_list_ner/tokenizer2/vocab.txt
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/LICENSE
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/README.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 drug_list_ner-0.0.5/PKG-INFO
```

### Comparing `drug_list_ner-0.0.4/.DS_Store` & `drug_list_ner-0.0.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.4/Pipfile.lock` & `drug_list_ner-0.0.5/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.4/requirements.txt` & `drug_list_ner-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.4/src/.DS_Store` & `drug_list_ner-0.0.5/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.4/src/drug_list_ner/.DS_Store` & `drug_list_ner-0.0.5/src/drug_list_ner/.DS_Store`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.4/src/drug_list_ner/example.py` & `drug_list_ner-0.0.5/src/drug_list_ner/example.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,10 +19,10 @@
             result.append(curr)
         res = [*set(result)]
     return (res)
 
 
 '''share/
 HF_DATASETS_OFFLINE=1 TRANSFORMERS_OFFLINE=1 \
-python3 main.py --pytorch_model.bin t5-small
+python3 example.py --pytorch_model.bin t5-small
 
 '''
```

### Comparing `drug_list_ner-0.0.4/src/drug_list_ner/model2/.DS_Store` & `drug_list_ner-0.0.5/src/drug_list_ner/model2/.DS_Store`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.4/src/drug_list_ner/model2/config.json` & `drug_list_ner-0.0.5/src/drug_list_ner/model2/config.json`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.4/src/drug_list_ner/tokenizer2/tokenizer.json` & `drug_list_ner-0.0.5/src/drug_list_ner/tokenizer2/tokenizer.json`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.4/src/drug_list_ner/tokenizer2/vocab.txt` & `drug_list_ner-0.0.5/src/drug_list_ner/tokenizer2/vocab.txt`

 * *Files identical despite different names*

### Comparing `drug_list_ner-0.0.4/LICENSE` & `drug_list_ner-0.0.5/LICENSE`

 * *Files identical despite different names*

