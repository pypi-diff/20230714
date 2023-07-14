# Comparing `tmp/ezsmdeploy-1.9.dev0.tar.gz` & `tmp/ezsmdeploy-1.91.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezsmdeploy-1.9.dev0.tar", last modified: Thu Jul 13 20:56:03 2023, max compression
+gzip compressed data, was "ezsmdeploy-1.91.dev0.tar", last modified: Fri Jul 14 04:29:03 2023, max compression
```

## Comparing `ezsmdeploy-1.9.dev0.tar` & `ezsmdeploy-1.91.dev0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-13 20:56:03.279466 ezsmdeploy-1.9.dev0/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/MANIFEST.in
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16911 2023-07-13 20:56:03.279466 ezsmdeploy-1.9.dev0/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16422 2023-07-13 20:44:23.000000 ezsmdeploy-1.9.dev0/README.rst
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-13 20:56:03.275466 ezsmdeploy-1.9.dev0/ezsmdeploy/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    47399 2023-07-13 20:30:04.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-13 20:56:03.279466 ezsmdeploy-1.9.dev0/ezsmdeploy/data/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2100 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/Dockerfile
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1934 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/Dockerfile_flask
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1390 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/build-docker.sh
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1603 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/conversation.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1361 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/cost.csv
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      884 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/dockerd-entrypoint.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      576 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/instancetypes.csv
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1797 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/model_handler.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      719 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/nginx.conf
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2090 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/predictor.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2429 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/serve
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1409 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/smlocust.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      432 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/train
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      202 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/data/wsgi.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      733 2023-07-08 14:37:12.000000 ezsmdeploy-1.9.dev0/ezsmdeploy/modelscript_sklearn.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-13 20:56:03.279466 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16911 2023-07-13 20:56:03.000000 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      696 2023-07-13 20:56:03.000000 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-13 20:56:03.000000 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-13 20:11:33.000000 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/not-zip-safe
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      129 2023-07-13 20:56:03.000000 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       11 2023-07-13 20:56:03.000000 ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-13 20:56:03.279466 ezsmdeploy-1.9.dev0/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1273 2023-07-13 20:11:18.000000 ezsmdeploy-1.9.dev0/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-14 04:29:03.393658 ezsmdeploy-1.91.dev0/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    18905 2023-07-14 04:29:03.393658 ezsmdeploy-1.91.dev0/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    18415 2023-07-14 04:26:31.000000 ezsmdeploy-1.91.dev0/README.rst
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-14 04:29:03.389658 ezsmdeploy-1.91.dev0/ezsmdeploy/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    48543 2023-07-14 04:28:51.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-14 04:29:03.393658 ezsmdeploy-1.91.dev0/ezsmdeploy/data/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2100 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/Dockerfile
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1934 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/Dockerfile_flask
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1390 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/build-docker.sh
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1603 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/conversation.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1361 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/cost.csv
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      884 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/dockerd-entrypoint.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      576 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/instancetypes.csv
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1797 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/model_handler.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      719 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/nginx.conf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2090 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/predictor.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2429 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/serve
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1409 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/smlocust.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      432 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/train
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      202 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/data/wsgi.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      733 2023-07-08 14:37:12.000000 ezsmdeploy-1.91.dev0/ezsmdeploy/modelscript_sklearn.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-14 04:29:03.389658 ezsmdeploy-1.91.dev0/ezsmdeploy.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    18905 2023-07-14 04:29:03.000000 ezsmdeploy-1.91.dev0/ezsmdeploy.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      696 2023-07-14 04:29:03.000000 ezsmdeploy-1.91.dev0/ezsmdeploy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-14 04:29:03.000000 ezsmdeploy-1.91.dev0/ezsmdeploy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-13 20:11:33.000000 ezsmdeploy-1.91.dev0/ezsmdeploy.egg-info/not-zip-safe
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      129 2023-07-14 04:29:03.000000 ezsmdeploy-1.91.dev0/ezsmdeploy.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       11 2023-07-14 04:29:03.000000 ezsmdeploy-1.91.dev0/ezsmdeploy.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-14 04:29:03.393658 ezsmdeploy-1.91.dev0/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1274 2023-07-14 04:28:48.000000 ezsmdeploy-1.91.dev0/setup.py
```

### Comparing `ezsmdeploy-1.9.dev0/PKG-INFO` & `ezsmdeploy-1.91.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsmdeploy
-Version: 1.9.dev0
+Version: 1.91.dev0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -60,15 +60,14 @@
 4. Tested the following:
     - tiiuae/falcon-40b-instruct, ml.g4dn.12xlarge
     - tiiuae/falcon-7b-instruct, ml.g5.16xlarge
     - WizardLM/WizardLM-7B-V1.0", ml.g5.16xlarge
     - TheBloke/wizardLM-7B-HF, ml.g4dn.4xlarge
     - togethercomputer/RedPajama-INCITE-Chat-3B-v1, ml.g4dn.4xlarge
     - openchat/openchat, ml.g5.24xlarge
-    - new model
 
 
 V 1.x release notes
 -------------------
 1. Updated to use >v2.x of SageMaker SDK
 2. Fixed failing docker builds
 3. Tested with test notebook
@@ -300,14 +299,73 @@
     
     return out
 
 
 Note that when using the Multi model mode, the payload comes in as a dictionary and the raw bytes sent in can be accessed using payload[0]['body']; In flask based deployments, you can just use payload as it is (comes in as bytes)
 
 
+Large Language models
+~~~~~~~~~~~~~~~~~~~~~
+
+EzSMDeploy supports deploying foundation models through Jumpstart as well as huggingface:
+
+To deploy models using Jumpstart:
+
+::
+
+    ezonsm = ezsmdeploy.Deploy(model = "huggingface-text2text-flan-ul2-bf16",
+                               foundation_model=True)
+                               
+Note that with Jumpstart models, we can automatically retrieve default/suggested instances from SageMaker                               
+
+
+
+To deploy a huggingface LLM model (this uses the huggingface llm container):
+
+::
+
+    ezonsm = ezsmdeploy.Deploy(model = "tiiuae/falcon-40b-instruct",
+                               foundation_model=True,
+                               huggingface_model=True,
+                               huggingface_model_task='text-generation',
+                               instance_type="ml.g4dn.12xlarge"
+                               )
+                               
+(See release notes for models we have tested so far with instances that worked)
+
+Note that at the time of writing this, officially supported model architectures for LLMs on Huggingface are currently:
+
+    - BLOOM / BLOOMZ
+    - MT0-XXL
+    - Galactica
+    - SantaCoder
+    - GPT-Neox 20B (joi, pythia, lotus, rosey, chip, RedPajama, open assistant)
+    - FLAN-T5-XXL (T5-11B)
+    - Llama (vicuna, alpaca, koala)
+    - Starcoder / SantaCoder
+    - Falcon 7B / Falcon 40B
+
+
+
+
+
+Serverless inference
+~~~~~~~~~~~~~~~~~~~~
+
+Simply do `serverless=True`. Make sure you size your serverless endpoint correctly using `serverless_memory` and `serverless_concurrency`. You can combine other features as well, for example, to deploy a huggingface model on serverless use:
+
+::
+
+    ezonsm = ezsmdeploy.Deploy(model = "distilbert-base-uncased-finetuned-sst-2-english",
+                               huggingface_model=True,
+                               huggingface_model_task='text-classification',
+                               serverless=True
+                               )
+
+
 Supported Operating Systems
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Ezsmdeploy SDK has been tested on Unix/Linux.
 
 Supported Python Versions
 ~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `ezsmdeploy-1.9.dev0/README.rst` & `ezsmdeploy-1.91.dev0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 4. Tested the following:
     - tiiuae/falcon-40b-instruct, ml.g4dn.12xlarge
     - tiiuae/falcon-7b-instruct, ml.g5.16xlarge
     - WizardLM/WizardLM-7B-V1.0", ml.g5.16xlarge
     - TheBloke/wizardLM-7B-HF, ml.g4dn.4xlarge
     - togethercomputer/RedPajama-INCITE-Chat-3B-v1, ml.g4dn.4xlarge
     - openchat/openchat, ml.g5.24xlarge
-    - new model
 
 
 V 1.x release notes
 -------------------
 1. Updated to use >v2.x of SageMaker SDK
 2. Fixed failing docker builds
 3. Tested with test notebook
@@ -285,14 +284,73 @@
     
     return out
 
 
 Note that when using the Multi model mode, the payload comes in as a dictionary and the raw bytes sent in can be accessed using payload[0]['body']; In flask based deployments, you can just use payload as it is (comes in as bytes)
 
 
+Large Language models
+~~~~~~~~~~~~~~~~~~~~~
+
+EzSMDeploy supports deploying foundation models through Jumpstart as well as huggingface:
+
+To deploy models using Jumpstart:
+
+::
+
+    ezonsm = ezsmdeploy.Deploy(model = "huggingface-text2text-flan-ul2-bf16",
+                               foundation_model=True)
+                               
+Note that with Jumpstart models, we can automatically retrieve default/suggested instances from SageMaker                               
+
+
+
+To deploy a huggingface LLM model (this uses the huggingface llm container):
+
+::
+
+    ezonsm = ezsmdeploy.Deploy(model = "tiiuae/falcon-40b-instruct",
+                               foundation_model=True,
+                               huggingface_model=True,
+                               huggingface_model_task='text-generation',
+                               instance_type="ml.g4dn.12xlarge"
+                               )
+                               
+(See release notes for models we have tested so far with instances that worked)
+
+Note that at the time of writing this, officially supported model architectures for LLMs on Huggingface are currently:
+
+    - BLOOM / BLOOMZ
+    - MT0-XXL
+    - Galactica
+    - SantaCoder
+    - GPT-Neox 20B (joi, pythia, lotus, rosey, chip, RedPajama, open assistant)
+    - FLAN-T5-XXL (T5-11B)
+    - Llama (vicuna, alpaca, koala)
+    - Starcoder / SantaCoder
+    - Falcon 7B / Falcon 40B
+
+
+
+
+
+Serverless inference
+~~~~~~~~~~~~~~~~~~~~
+
+Simply do `serverless=True`. Make sure you size your serverless endpoint correctly using `serverless_memory` and `serverless_concurrency`. You can combine other features as well, for example, to deploy a huggingface model on serverless use:
+
+::
+
+    ezonsm = ezsmdeploy.Deploy(model = "distilbert-base-uncased-finetuned-sst-2-english",
+                               huggingface_model=True,
+                               huggingface_model_task='text-classification',
+                               serverless=True
+                               )
+
+
 Supported Operating Systems
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Ezsmdeploy SDK has been tested on Unix/Linux.
 
 Supported Python Versions
 ~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/__init__.py` & `ezsmdeploy-1.91.dev0/ezsmdeploy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         framework=None,
         requirements=None,
         name=None,
         autoscale=False,
         autoscaletarget=1000,
         serverless=False,
         serverless_memory=4096,
-        serverless_concurrency=100,
+        serverless_concurrency=10,
         wait=True,
         bucket=None,
         prefix='',
         session=None,
         image=None,
         dockerfilepath=None,
         instance_type=None,
@@ -330,26 +330,35 @@
 
         
         
         aws_role = sagemaker.get_execution_role()
         endpoint_name = name="hf-model-" + self.name
         
         # create Hugging Face Model Class
-        self.sagemakermodel = HuggingFaceModel(
-           image_uri=get_huggingface_llm_image_uri("huggingface"),
-           env=hub,                                                # configuration for loading model from Hub
-           role=aws_role,                                          # IAM role with permissions to create an endpoint
-           name=endpoint_name,
-           transformers_version="4.26",                             # Transformers version used
-           pytorch_version="1.13",                                  # PyTorch version used
-           py_version='py39',                                      # Python version used
-        )
+        if not self.serverless and self.foundation_model and self.huggingface_model: #Basically just for large models
+            self.sagemakermodel = HuggingFaceModel(
+               image_uri=get_huggingface_llm_image_uri("huggingface"),
+               env=hub,                                                # configuration for loading model from Hub
+               role=aws_role,                                          # IAM role with permissions to create an endpoint
+               name=endpoint_name,
+               transformers_version="4.26",                             # Transformers version used
+               pytorch_version="1.13",                                  # PyTorch version used
+               py_version='py39',                                      # Python version used
+            )
+        else:
+            self.sagemakermodel = HuggingFaceModel(
+                env=hub,                      # configuration for loading model from Hub
+                role=aws_role,                    # iam role with permissions to create an Endpoint
+                transformers_version="4.26",  # transformers version used
+                pytorch_version="1.13",        # pytorch version used
+                py_version='py39',            # python version used
+                )
     
     def deploy_foundation_model(self):
-        # print("start")
+        # Assume foundation model on Jumpstart here
 
         
         from sagemaker import image_uris, instance_types, model_uris, script_uris
         self.model = self.model[0]
         # print("self.model = ", self.model)
         instance_type = instance_types.retrieve_default(
             model_id=self.model, model_version=self.foundation_model_version, scope="inference"
@@ -595,39 +604,50 @@
                     volume_size = 256 
                 else:
                     volume_size = None
         else:
             volume_size = None 
             
         
-        if self.foundation_model:
+        if self.foundation_model and not self.huggingface_model:
             # deploy the Model. Note that we need to pass Predictor class when we deploy model through Model class,
             # for being able to run inference through the sagemaker API.
 
             self.predictor = self.sagemakermodel.deploy(
                 initial_instance_count=self.instance_count,
                 instance_type=self.instance_type,
                 predictor_cls=sagemaker.predictor.Predictor,
                 endpoint_name="ezsm-foundation-endpoint-" + self.name,
                 volume_size=volume_size,
                 # serverless_inference_config=self.serverless_config, #ignoring serverless inference
                 wait=self.wait
             )
-        elif self.huggingface_model:
+        elif self.foundation_model and self.huggingface_model:
             
             
             self.predictor = self.sagemakermodel.deploy(
                 initial_instance_count=self.instance_count,
                 instance_type=self.instance_type,
                 endpoint_name="ezsm-hf-endpoint-" + self.name,
                 volume_size=volume_size,
-                serverless_inference_config=self.serverless_config,
                 wait=self.wait,
                 container_startup_health_check_timeout=300,
             )
+            
+        elif self.huggingface_model and not self.foundation_model:
+            
+            
+            self.predictor = self.sagemakermodel.deploy(
+                initial_instance_count=self.instance_count,
+                instance_type=self.instance_type,
+                endpoint_name="ezsm-hf-endpoint-" + self.name,
+                volume_size=volume_size,
+                serverless_inference_config=self.serverless_config,
+                wait=self.wait
+            )
                 
             
         else:
             self.predictor = self.sagemakermodel.deploy(
                 initial_instance_count=self.instance_count,
                 instance_type=self.instance_type,
                 accelerator_type=self.ei,
```

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/data/Dockerfile` & `ezsmdeploy-1.91.dev0/ezsmdeploy/data/Dockerfile`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/data/Dockerfile_flask` & `ezsmdeploy-1.91.dev0/ezsmdeploy/data/Dockerfile_flask`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/data/build-docker.sh` & `ezsmdeploy-1.91.dev0/ezsmdeploy/data/build-docker.sh`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/data/conversation.py` & `ezsmdeploy-1.91.dev0/ezsmdeploy/data/conversation.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/data/cost.csv` & `ezsmdeploy-1.91.dev0/ezsmdeploy/data/cost.csv`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/data/dockerd-entrypoint.py` & `ezsmdeploy-1.91.dev0/ezsmdeploy/data/dockerd-entrypoint.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/data/instancetypes.csv` & `ezsmdeploy-1.91.dev0/ezsmdeploy/data/instancetypes.csv`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/data/model_handler.py` & `ezsmdeploy-1.91.dev0/ezsmdeploy/data/model_handler.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/data/nginx.conf` & `ezsmdeploy-1.91.dev0/ezsmdeploy/data/nginx.conf`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/data/predictor.py` & `ezsmdeploy-1.91.dev0/ezsmdeploy/data/predictor.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/data/serve` & `ezsmdeploy-1.91.dev0/ezsmdeploy/data/serve`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/data/smlocust.py` & `ezsmdeploy-1.91.dev0/ezsmdeploy/data/smlocust.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy/modelscript_sklearn.py` & `ezsmdeploy-1.91.dev0/ezsmdeploy/modelscript_sklearn.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/PKG-INFO` & `ezsmdeploy-1.91.dev0/ezsmdeploy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsmdeploy
-Version: 1.9.dev0
+Version: 1.91.dev0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -60,15 +60,14 @@
 4. Tested the following:
     - tiiuae/falcon-40b-instruct, ml.g4dn.12xlarge
     - tiiuae/falcon-7b-instruct, ml.g5.16xlarge
     - WizardLM/WizardLM-7B-V1.0", ml.g5.16xlarge
     - TheBloke/wizardLM-7B-HF, ml.g4dn.4xlarge
     - togethercomputer/RedPajama-INCITE-Chat-3B-v1, ml.g4dn.4xlarge
     - openchat/openchat, ml.g5.24xlarge
-    - new model
 
 
 V 1.x release notes
 -------------------
 1. Updated to use >v2.x of SageMaker SDK
 2. Fixed failing docker builds
 3. Tested with test notebook
@@ -300,14 +299,73 @@
     
     return out
 
 
 Note that when using the Multi model mode, the payload comes in as a dictionary and the raw bytes sent in can be accessed using payload[0]['body']; In flask based deployments, you can just use payload as it is (comes in as bytes)
 
 
+Large Language models
+~~~~~~~~~~~~~~~~~~~~~
+
+EzSMDeploy supports deploying foundation models through Jumpstart as well as huggingface:
+
+To deploy models using Jumpstart:
+
+::
+
+    ezonsm = ezsmdeploy.Deploy(model = "huggingface-text2text-flan-ul2-bf16",
+                               foundation_model=True)
+                               
+Note that with Jumpstart models, we can automatically retrieve default/suggested instances from SageMaker                               
+
+
+
+To deploy a huggingface LLM model (this uses the huggingface llm container):
+
+::
+
+    ezonsm = ezsmdeploy.Deploy(model = "tiiuae/falcon-40b-instruct",
+                               foundation_model=True,
+                               huggingface_model=True,
+                               huggingface_model_task='text-generation',
+                               instance_type="ml.g4dn.12xlarge"
+                               )
+                               
+(See release notes for models we have tested so far with instances that worked)
+
+Note that at the time of writing this, officially supported model architectures for LLMs on Huggingface are currently:
+
+    - BLOOM / BLOOMZ
+    - MT0-XXL
+    - Galactica
+    - SantaCoder
+    - GPT-Neox 20B (joi, pythia, lotus, rosey, chip, RedPajama, open assistant)
+    - FLAN-T5-XXL (T5-11B)
+    - Llama (vicuna, alpaca, koala)
+    - Starcoder / SantaCoder
+    - Falcon 7B / Falcon 40B
+
+
+
+
+
+Serverless inference
+~~~~~~~~~~~~~~~~~~~~
+
+Simply do `serverless=True`. Make sure you size your serverless endpoint correctly using `serverless_memory` and `serverless_concurrency`. You can combine other features as well, for example, to deploy a huggingface model on serverless use:
+
+::
+
+    ezonsm = ezsmdeploy.Deploy(model = "distilbert-base-uncased-finetuned-sst-2-english",
+                               huggingface_model=True,
+                               huggingface_model_task='text-classification',
+                               serverless=True
+                               )
+
+
 Supported Operating Systems
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Ezsmdeploy SDK has been tested on Unix/Linux.
 
 Supported Python Versions
 ~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `ezsmdeploy-1.9.dev0/ezsmdeploy.egg-info/SOURCES.txt` & `ezsmdeploy-1.91.dev0/ezsmdeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.9.dev0/setup.py` & `ezsmdeploy-1.91.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 extras = {
     'locust': [
         'locustio==0.14.5'
     ]
 }
 
 setup(name='ezsmdeploy',
-      version='1.9dev',
+      version='1.91dev',
       description='SageMaker custom deployments made easy',
       url='https://pypi.python.org/pypi/ezsmdeploy',
       #scripts=['Dockerfile','dockerd-entrypoint.py','model_handler.py','build-docker.sh'],
       author='Shreyas Subramanian',
       author_email='subshrey@amazon.com',
       license='MIT',
       packages=['ezsmdeploy'],
```

