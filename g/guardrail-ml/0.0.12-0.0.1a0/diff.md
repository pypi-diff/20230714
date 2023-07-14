# Comparing `tmp/guardrail-ml-0.0.12.tar.gz` & `tmp/guardrail-ml-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guardrail-ml-0.0.12.tar", last modified: Fri Jul 14 20:59:40 2023, max compression
+gzip compressed data, was "guardrail-ml-0.0.1a0.tar", last modified: Fri Jul 14 20:15:51 2023, max compression
```

## Comparing `guardrail-ml-0.0.12.tar` & `guardrail-ml-0.0.1a0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 20:59:40.694114 guardrail-ml-0.0.12/
--rw-rw-rw-   0        0        0    11545 2023-06-16 13:48:47.000000 guardrail-ml-0.0.12/LICENSE.txt
--rw-rw-rw-   0        0        0     3743 2023-07-14 20:59:40.694114 guardrail-ml-0.0.12/PKG-INFO
--rw-rw-rw-   0        0        0     3266 2023-07-14 20:13:35.000000 guardrail-ml-0.0.12/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 20:59:40.592083 guardrail-ml-0.0.12/guardrail/
--rw-rw-rw-   0        0        0       58 2023-06-28 14:17:16.000000 guardrail-ml-0.0.12/guardrail/__init__.py
--rw-rw-rw-   0        0        0     3851 2023-07-14 20:43:28.000000 guardrail-ml-0.0.12/guardrail/client.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:59:40.607910 guardrail-ml-0.0.12/guardrail/dataset/
--rw-rw-rw-   0        0        0        0 2023-06-30 20:17:26.000000 guardrail-ml-0.0.12/guardrail/dataset/__init__.py
--rw-rw-rw-   0        0        0      747 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/dataset/convert_json.py
--rw-rw-rw-   0        0        0    11070 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/dataset/dataset_creation_local_api.py
--rw-rw-rw-   0        0        0     8017 2023-07-14 20:58:25.000000 guardrail-ml-0.0.12/guardrail/dataset/dataset_generator.py
--rw-rw-rw-   0        0        0        0 2023-07-01 15:36:20.000000 guardrail-ml-0.0.12/guardrail/dataset/helper.py
--rw-rw-rw-   0        0        0     4248 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/dataset/parse_pdf.py
--rw-rw-rw-   0        0        0      524 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/db.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:59:40.640485 guardrail-ml-0.0.12/guardrail/metrics/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:17:23.000000 guardrail-ml-0.0.12/guardrail/metrics/__init__.py
--rw-rw-rw-   0        0        0      600 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/metrics/bias.py
--rw-rw-rw-   0        0        0      245 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/metrics/custom.py
--rw-rw-rw-   0        0        0        0 2023-06-15 21:56:06.000000 guardrail-ml-0.0.12/guardrail/metrics/disinformation.py
--rw-rw-rw-   0        0        0        0 2023-06-15 21:56:43.000000 guardrail-ml-0.0.12/guardrail/metrics/domaintasks.py
--rw-rw-rw-   0        0        0        0 2023-06-15 21:52:25.000000 guardrail-ml-0.0.12/guardrail/metrics/eleutherai.py
--rw-rw-rw-   0        0        0        0 2023-07-12 22:28:36.000000 guardrail-ml-0.0.12/guardrail/metrics/hurtful.py
--rw-rw-rw-   0        0        0      606 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/metrics/injections.py
--rw-rw-rw-   0        0        0        0 2023-06-15 21:46:23.000000 guardrail-ml-0.0.12/guardrail/metrics/regexes.py
--rw-rw-rw-   0        0        0      814 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/metrics/relevance.py
--rw-rw-rw-   0        0        0      576 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/metrics/sentiment.py
--rw-rw-rw-   0        0        0     5600 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/metrics/textstat.py
--rw-rw-rw-   0        0        0        0 2023-06-15 21:48:00.000000 guardrail-ml-0.0.12/guardrail/metrics/topics.py
--rw-rw-rw-   0        0        0      831 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/metrics/toxicity.py
--rw-rw-rw-   0        0        0       25 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/metrics/truthfulness.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:59:40.646961 guardrail-ml-0.0.12/guardrail/streamlit/
--rw-rw-rw-   0        0        0     4236 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/streamlit/1_🏠_Evaluate.py
--rw-rw-rw-   0        0        0        0 2023-06-26 22:53:29.000000 guardrail-ml-0.0.12/guardrail/streamlit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:59:40.652962 guardrail-ml-0.0.12/guardrail/streamlit/helper/
--rw-rw-rw-   0        0        0        0 2023-06-26 22:53:15.000000 guardrail-ml-0.0.12/guardrail/streamlit/helper/__init__.py
--rw-rw-rw-   0        0        0      912 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/streamlit/helper/add_logo.py
--rw-rw-rw-   0        0        0     2053 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/streamlit/helper/agstyler.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:59:40.662052 guardrail-ml-0.0.12/guardrail/streamlit/pages/
--rw-rw-rw-   0        0        0      112 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/streamlit/pages/2_🤖_Benchmark.py
--rw-rw-rw-   0        0        0        0 2023-06-27 12:57:57.000000 guardrail-ml-0.0.12/guardrail/streamlit/pages/3_🗒️_Documentation.py
--rw-rw-rw-   0        0        0       47 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/guardrail/streamlit/pages/4_💬_Contact.py
--rw-rw-rw-   0        0        0        0 2023-06-26 22:53:22.000000 guardrail-ml-0.0.12/guardrail/streamlit/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:59:40.690730 guardrail-ml-0.0.12/guardrail_ml.egg-info/
--rw-rw-rw-   0        0        0     3743 2023-07-14 20:59:40.000000 guardrail-ml-0.0.12/guardrail_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1353 2023-07-14 20:59:40.000000 guardrail-ml-0.0.12/guardrail_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 20:59:40.000000 guardrail-ml-0.0.12/guardrail_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-07-14 20:59:40.000000 guardrail-ml-0.0.12/guardrail_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-14 20:59:40.000000 guardrail-ml-0.0.12/guardrail_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      218 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/pyproject.toml
--rw-rw-rw-   0        0        0      601 2023-07-14 20:59:40.697367 guardrail-ml-0.0.12/setup.cfg
--rw-rw-rw-   0        0        0     1086 2023-07-14 20:59:12.000000 guardrail-ml-0.0.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:59:40.691732 guardrail-ml-0.0.12/tests/
--rw-rw-rw-   0        0        0      874 2023-07-14 19:45:02.000000 guardrail-ml-0.0.12/tests/test_textstat.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:15:51.320144 guardrail-ml-0.0.1a0/
+-rw-rw-rw-   0        0        0    11545 2023-06-16 13:48:47.000000 guardrail-ml-0.0.1a0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3744 2023-07-14 20:15:51.320144 guardrail-ml-0.0.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0     3266 2023-07-14 20:13:35.000000 guardrail-ml-0.0.1a0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 20:15:51.164747 guardrail-ml-0.0.1a0/guardrail/
+-rw-rw-rw-   0        0        0       58 2023-06-28 14:17:16.000000 guardrail-ml-0.0.1a0/guardrail/__init__.py
+-rw-rw-rw-   0        0        0     3851 2023-07-14 20:14:47.000000 guardrail-ml-0.0.1a0/guardrail/client.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:15:51.183564 guardrail-ml-0.0.1a0/guardrail/dataset/
+-rw-rw-rw-   0        0        0        0 2023-06-30 20:17:26.000000 guardrail-ml-0.0.1a0/guardrail/dataset/__init__.py
+-rw-rw-rw-   0        0        0      747 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/dataset/convert_json.py
+-rw-rw-rw-   0        0        0    11070 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/dataset/dataset_creation_local_api.py
+-rw-rw-rw-   0        0        0     8005 2023-07-14 20:13:41.000000 guardrail-ml-0.0.1a0/guardrail/dataset/dataset_generator.py
+-rw-rw-rw-   0        0        0        0 2023-07-01 15:36:20.000000 guardrail-ml-0.0.1a0/guardrail/dataset/helper.py
+-rw-rw-rw-   0        0        0     4248 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/dataset/parse_pdf.py
+-rw-rw-rw-   0        0        0      524 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/db.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:15:51.261430 guardrail-ml-0.0.1a0/guardrail/metrics/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:17:23.000000 guardrail-ml-0.0.1a0/guardrail/metrics/__init__.py
+-rw-rw-rw-   0        0        0      600 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/metrics/bias.py
+-rw-rw-rw-   0        0        0      245 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/metrics/custom.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 21:56:06.000000 guardrail-ml-0.0.1a0/guardrail/metrics/disinformation.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 21:56:43.000000 guardrail-ml-0.0.1a0/guardrail/metrics/domaintasks.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 21:52:25.000000 guardrail-ml-0.0.1a0/guardrail/metrics/eleutherai.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 22:28:36.000000 guardrail-ml-0.0.1a0/guardrail/metrics/hurtful.py
+-rw-rw-rw-   0        0        0      606 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/metrics/injections.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 21:46:23.000000 guardrail-ml-0.0.1a0/guardrail/metrics/regexes.py
+-rw-rw-rw-   0        0        0      814 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/metrics/relevance.py
+-rw-rw-rw-   0        0        0      576 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/metrics/sentiment.py
+-rw-rw-rw-   0        0        0     5600 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/metrics/textstat.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 21:48:00.000000 guardrail-ml-0.0.1a0/guardrail/metrics/topics.py
+-rw-rw-rw-   0        0        0      831 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/metrics/toxicity.py
+-rw-rw-rw-   0        0        0       25 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/metrics/truthfulness.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:15:51.271600 guardrail-ml-0.0.1a0/guardrail/streamlit/
+-rw-rw-rw-   0        0        0     4236 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/streamlit/1_🏠_Evaluate.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 22:53:29.000000 guardrail-ml-0.0.1a0/guardrail/streamlit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:15:51.277601 guardrail-ml-0.0.1a0/guardrail/streamlit/helper/
+-rw-rw-rw-   0        0        0        0 2023-06-26 22:53:15.000000 guardrail-ml-0.0.1a0/guardrail/streamlit/helper/__init__.py
+-rw-rw-rw-   0        0        0      912 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/streamlit/helper/add_logo.py
+-rw-rw-rw-   0        0        0     2053 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/streamlit/helper/agstyler.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:15:51.288156 guardrail-ml-0.0.1a0/guardrail/streamlit/pages/
+-rw-rw-rw-   0        0        0      112 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/streamlit/pages/2_🤖_Benchmark.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 12:57:57.000000 guardrail-ml-0.0.1a0/guardrail/streamlit/pages/3_🗒️_Documentation.py
+-rw-rw-rw-   0        0        0       47 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/guardrail/streamlit/pages/4_💬_Contact.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 22:53:22.000000 guardrail-ml-0.0.1a0/guardrail/streamlit/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:15:51.316139 guardrail-ml-0.0.1a0/guardrail_ml.egg-info/
+-rw-rw-rw-   0        0        0     3744 2023-07-14 20:15:51.000000 guardrail-ml-0.0.1a0/guardrail_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1353 2023-07-14 20:15:51.000000 guardrail-ml-0.0.1a0/guardrail_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 20:15:51.000000 guardrail-ml-0.0.1a0/guardrail_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-07-14 20:15:51.000000 guardrail-ml-0.0.1a0/guardrail_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 20:15:51.000000 guardrail-ml-0.0.1a0/guardrail_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      218 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/pyproject.toml
+-rw-rw-rw-   0        0        0      601 2023-07-14 20:15:51.322142 guardrail-ml-0.0.1a0/setup.cfg
+-rw-rw-rw-   0        0        0     1091 2023-07-14 20:14:47.000000 guardrail-ml-0.0.1a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:15:51.318147 guardrail-ml-0.0.1a0/tests/
+-rw-rw-rw-   0        0        0      874 2023-07-14 19:45:02.000000 guardrail-ml-0.0.1a0/tests/test_textstat.py
```

### Comparing `guardrail-ml-0.0.12/LICENSE.txt` & `guardrail-ml-0.0.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/PKG-INFO` & `guardrail-ml-0.0.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guardrail-ml
-Version: 0.0.12
+Version: 0.0.1a0
 Summary: Monitor LLMs with custom metrics to scale with confidence
 Home-page: http://www.guardrailml.com
 Author: Kevin Wu
 Author-email: kevin@guardrailml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `guardrail-ml-0.0.12/README.md` & `guardrail-ml-0.0.1a0/README.md`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/client.py` & `guardrail-ml-0.0.1a0/guardrail/client.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/dataset/convert_json.py` & `guardrail-ml-0.0.1a0/guardrail/dataset/convert_json.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/dataset/dataset_creation_local_api.py` & `guardrail-ml-0.0.1a0/guardrail/dataset/dataset_creation_local_api.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/dataset/dataset_generator.py` & `guardrail-ml-0.0.1a0/guardrail/dataset/dataset_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,22 +20,22 @@
     def __init__(
         self,
         file_path: str,
         output_path: str,
         *,
         model="OpenAssistant/falcon-7b-sft-mix-2000",
         tokenizer="OpenAssistant/falcon-7b-sft-mix-2000b",
-        load_in_4bit=True,
+        load_4bit=True,
         debug: bool = False,
         max_array_length: int = 256,
         max_number_tokens: int = 64,
         temperature: float = 0.3,
         max_string_token_length: int = 1024,
     ):
-        if load_in_4bit:
+        if load_4bit:
             print("Loading in 4bit...")
             bnb_config = BitsAndBytesConfig(
                 load_in_4bit=True,
                 bnb_4bit_quant_type="nf4",
                 bnb_4bit_compute_dtype=torch.float16,
             )
             self.model = AutoModelForCausalLM.from_pretrained(
@@ -121,15 +121,15 @@
                 )
                 output = builder()
                 qa_pairs_arr.append(output)
                 print(output)
                 print("Size of array: ", len(qa_pairs_arr))
         return qa_pairs_arr
 
-    def generate_prompt(self, input):
+    def generate_prompt(input):
         prompt_intro = "Below is an instruction that describes a task. Write a response that appropriately completes the request."
         prompt_instruction = """
 
         ### Instruction:
         Heed the following rules:
         - Generate a highly contextual question and answer pairs from the following context
         - Avoid leading questions, or questions with the answer explicitly in them
```

### Comparing `guardrail-ml-0.0.12/guardrail/dataset/parse_pdf.py` & `guardrail-ml-0.0.1a0/guardrail/dataset/parse_pdf.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/db.py` & `guardrail-ml-0.0.1a0/guardrail/db.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/metrics/bias.py` & `guardrail-ml-0.0.1a0/guardrail/metrics/bias.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/metrics/injections.py` & `guardrail-ml-0.0.1a0/guardrail/metrics/injections.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/metrics/relevance.py` & `guardrail-ml-0.0.1a0/guardrail/metrics/relevance.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/metrics/sentiment.py` & `guardrail-ml-0.0.1a0/guardrail/metrics/sentiment.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/metrics/textstat.py` & `guardrail-ml-0.0.1a0/guardrail/metrics/textstat.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/metrics/toxicity.py` & `guardrail-ml-0.0.1a0/guardrail/metrics/toxicity.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/streamlit/1_🏠_Evaluate.py` & `guardrail-ml-0.0.1a0/guardrail/streamlit/1_🏠_Evaluate.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/streamlit/helper/add_logo.py` & `guardrail-ml-0.0.1a0/guardrail/streamlit/helper/add_logo.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail/streamlit/helper/agstyler.py` & `guardrail-ml-0.0.1a0/guardrail/streamlit/helper/agstyler.py`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/guardrail_ml.egg-info/PKG-INFO` & `guardrail-ml-0.0.1a0/guardrail_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guardrail-ml
-Version: 0.0.12
+Version: 0.0.1a0
 Summary: Monitor LLMs with custom metrics to scale with confidence
 Home-page: http://www.guardrailml.com
 Author: Kevin Wu
 Author-email: kevin@guardrailml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `guardrail-ml-0.0.12/guardrail_ml.egg-info/SOURCES.txt` & `guardrail-ml-0.0.1a0/guardrail_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/setup.cfg` & `guardrail-ml-0.0.1a0/setup.cfg`

 * *Files identical despite different names*

### Comparing `guardrail-ml-0.0.12/setup.py` & `guardrail-ml-0.0.1a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="guardrail-ml",
-    version="0.0.12",
+    version="0.0.1-alpha",
     packages=find_packages(exclude=["tests", "guardrailmlev", "examples", "docs", "env", "dist"]),
     author="Kevin Wu",
     author_email="kevin@guardrailml.com",
     description="Monitor LLMs with custom metrics to scale with confidence",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://www.guardrailml.com",
```

### Comparing `guardrail-ml-0.0.12/tests/test_textstat.py` & `guardrail-ml-0.0.1a0/tests/test_textstat.py`

 * *Files identical despite different names*

