# Comparing `tmp/sa_app-0.0.0.tar.gz` & `tmp/sa_app-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sa_app-0.0.0.tar", max compression
+gzip compressed data, was "sa_app-0.0.1.tar", max compression
```

## Comparing `sa_app-0.0.0.tar` & `sa_app-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      597 2023-07-14 09:57:56.019233 sa_app-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-09 21:15:51.027113 sa_app-0.0.0/sa_app/__init__.py
--rw-r--r--   0        0        0     4323 2023-07-14 10:59:54.519169 sa_app-0.0.0/sa_app/app.py
--rw-r--r--   0        0        0        0 2023-07-09 21:15:51.035113 sa_app-0.0.0/sa_app/common/__init__.py
--rw-r--r--   0        0        0      907 2023-07-09 21:12:28.469460 sa_app-0.0.0/sa_app/common/utils.py
--rw-r--r--   0        0        0        0 2023-07-05 21:59:49.642256 sa_app-0.0.0/sa_app/data/__init__.py
--rw-r--r--   0        0        0     5633 2023-07-14 11:28:14.827213 sa_app-0.0.0/sa_app/data/data.py
--rw-r--r--   0        0        0     2456 2023-07-05 15:42:48.849737 sa_app-0.0.0/sa_app/data/data_cleaner.py
--rw-r--r--   0        0        0     2248 2023-07-05 13:49:12.964131 sa_app-0.0.0/sa_app/data/kaggle_dataset.py
--rw-r--r--   0        0        0        0 2023-07-05 21:00:18.938516 sa_app-0.0.0/sa_app/inference/__init__.py
--rw-r--r--   0        0        0     2033 2023-07-09 21:12:28.473460 sa_app-0.0.0/sa_app/inference/inference.py
--rw-r--r--   0        0        0        0 2023-07-01 14:33:52.363077 sa_app-0.0.0/sa_app/models/__init__.py
--rw-r--r--   0        0        0      415 2023-07-03 21:28:48.416607 sa_app-0.0.0/sa_app/models/model.py
--rw-r--r--   0        0        0        0 2023-07-01 14:34:08.146982 sa_app-0.0.0/sa_app/training/__init__.py
--rw-r--r--   0        0        0     4953 2023-07-14 11:34:21.137593 sa_app-0.0.0/sa_app/training/lightning_model_wrapper.py
--rw-r--r--   0        0        0     1515 2023-07-04 21:07:31.864810 sa_app-0.0.0/sa_app/training/optmizer.py
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 sa_app-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      659 2023-07-14 14:17:52.013941 sa_app-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 21:15:51.027113 sa_app-0.0.1/sa_app/__init__.py
+-rw-r--r--   0        0        0     4321 2023-07-14 11:40:37.096062 sa_app-0.0.1/sa_app/app.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:15:51.035113 sa_app-0.0.1/sa_app/common/__init__.py
+-rw-r--r--   0        0        0      907 2023-07-09 21:12:28.469460 sa_app-0.0.1/sa_app/common/utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:59:49.642256 sa_app-0.0.1/sa_app/data/__init__.py
+-rw-r--r--   0        0        0     5583 2023-07-14 11:40:37.104062 sa_app-0.0.1/sa_app/data/data.py
+-rw-r--r--   0        0        0     2456 2023-07-05 15:42:48.849737 sa_app-0.0.1/sa_app/data/data_cleaner.py
+-rw-r--r--   0        0        0     2248 2023-07-05 13:49:12.964131 sa_app-0.0.1/sa_app/data/kaggle_dataset.py
+-rw-r--r--   0        0        0        0 2023-07-05 21:00:18.938516 sa_app-0.0.1/sa_app/inference/__init__.py
+-rw-r--r--   0        0        0     2168 2023-07-14 14:10:19.971774 sa_app-0.0.1/sa_app/inference/inference.py
+-rw-r--r--   0        0        0      796 2023-07-14 14:10:19.975774 sa_app-0.0.1/sa_app/inference_app.py
+-rw-r--r--   0        0        0        0 2023-07-01 14:33:52.363077 sa_app-0.0.1/sa_app/models/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-03 21:28:48.416607 sa_app-0.0.1/sa_app/models/model.py
+-rw-r--r--   0        0        0        0 2023-07-01 14:34:08.146982 sa_app-0.0.1/sa_app/training/__init__.py
+-rw-r--r--   0        0        0     4953 2023-07-14 11:34:21.137593 sa_app-0.0.1/sa_app/training/lightning_model_wrapper.py
+-rw-r--r--   0        0        0     1515 2023-07-04 21:07:31.864810 sa_app-0.0.1/sa_app/training/optmizer.py
+-rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 sa_app-0.0.1/PKG-INFO
```

### Comparing `sa_app-0.0.0/pyproject.toml` & `sa_app-0.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sa_app"
-version = "0.0.0"
+version = "0.0.1"
 authors = ["prabhu <prabhupad26@gmail.com>"]
 description="Sentiment analyzer app"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -17,12 +17,14 @@
 python = "^3.10"
 transformers = "4.28.1"
 torch = "2.0.1"
 pandas = "1.5.1"
 pytorch-lightning = "2.0.4"
 wandb = "^0.14.2"
 nltk = "^3.8.1"
-spacy = "3.5.4"
+spacy = "3.6.0"
+flask = "^2.3.2"
 
 
 [project.scripts]
-sa_app = "sa_app.app:main"
+sa_app = "sa_app.app:main"
+inference_app = "sa_app.inference_app:main"
```

### Comparing `sa_app-0.0.0/sa_app/app.py` & `sa_app-0.0.1/sa_app/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytorch_lightning as pl
 import torch
 import wandb
 import yaml
 from pytorch_lightning.callbacks import LearningRateMonitor, ModelCheckpoint
 from pytorch_lightning.loggers import WandbLogger
 from sa_app.common.utils import init_model_loggers, parse_args
-from sa_app.data.data import SentimentIterableDataset, InitializeDataset
+from sa_app.data.data import InitializeDataset, SentimentIterableDataset
 from sa_app.models.model import Model
 from sa_app.training.lightning_model_wrapper import LightningModelWrapper
 from transformers import AutoConfig, AutoModelForSequenceClassification, AutoTokenizer
 
 
 def init_model_callbacks(training_params: dict) -> List:
     model_checkpoint = ModelCheckpoint(
@@ -105,16 +105,14 @@
 
     # Trainer initialization
     trainer = get_trainer(loggers, devices, accelerator, callbacks, training_params)
 
     # Initiate trainer
     trainer.fit(model=model_wrapped, train_dataloaders=train_dataset, val_dataloaders=valid_dataset, ckpt_path="last")
 
-
-
     wandb.finish()
 
 
 def main():
     args = parse_args()
     config = yaml.safe_load(open(args.config, "r"))
     device = "cuda" if torch.cuda.is_available() else "cpu"
```

### Comparing `sa_app-0.0.0/sa_app/common/utils.py` & `sa_app-0.0.1/sa_app/common/utils.py`

 * *Files identical despite different names*

### Comparing `sa_app-0.0.0/sa_app/data/data.py` & `sa_app-0.0.1/sa_app/data/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 import os.path
+from glob import glob
 from typing import Dict, Generator, List, Optional, Tuple
 
 import pandas as pd
 import torch
 from sa_app.data.data_cleaner import StackedPreprocessor
 from sa_app.data.kaggle_dataset import get_dataset_length, get_file_names, split_dataset
 from torch.utils.data import IterableDataset
 from tqdm import tqdm
 from transformers import AutoTokenizer
-from glob import glob
 
 
 def kaggle_dataset_iterator(file_map: dict, chunk_size=1000, split_type="train") -> pd.DataFrame:
     dataset_path = file_map[split_type]
     return pd.read_csv(dataset_path, encoding="latin-1", chunksize=chunk_size)
 
 
 class InitializeDataset:
     def __init__(self, dataset_params):
         self.dataset_params = dataset_params
 
     def __call__(self, *args, **kwargs) -> Tuple[str, str]:
-        if self.dataset_params.get('wandb_storage') is not None:
-            wandb_storage = self.dataset_params.get('wandb_storage')
+        if self.dataset_params.get("wandb_storage") is not None:
+            wandb_storage = self.dataset_params.get("wandb_storage")
             wandb_user_id = wandb_storage.get("wandb_user_id")
             wandb_project_name = wandb_storage.get("wandb_project_name")
             wandb_artifact_name = wandb_storage.get("wandb_artifact_name")
             wandb_artifact_type = wandb_storage.get("wandb_artifact_type")
             wandb_file_type = wandb_storage.get("training_file_type")
             wandb_artifact_version = wandb_storage.get("wandb_artifact_version")
             labels_mapping_file_name = wandb_storage.get("labels_mapping_file_name")
             import wandb
-            run = wandb.init(entity=wandb_user_id,
-                             project=wandb_project_name,
-                             job_type='download_dataset')
-            artifact = run.use_artifact(f'{wandb_user_id}/{wandb_project_name}/{wandb_artifact_name}:{wandb_artifact_version}',
-                                        type=f'{wandb_artifact_type}')
+
+            run = wandb.init(entity=wandb_user_id, project=wandb_project_name, job_type="download_dataset")
+            artifact = run.use_artifact(
+                f"{wandb_user_id}/{wandb_project_name}/{wandb_artifact_name}:{wandb_artifact_version}",
+                type=f"{wandb_artifact_type}",
+            )
             artifact_dir = artifact.download()
             assert len(glob(f"{artifact_dir}/*.{wandb_file_type}")) > 0, "CSV file download failed"
             csv_file = glob(f"{artifact_dir}/*.{wandb_file_type}")[0]
             mapping_file = os.path.join(artifact_dir, labels_mapping_file_name)
             assert os.path.isfile(mapping_file) is True, "Label mapping file download failed"
             return csv_file, mapping_file
-        elif self.dataset_params.get('local_storage') is not None:
+        elif self.dataset_params.get("local_storage") is not None:
             local_storage = self.dataset_params.get("local_storage")
             csv_file = local_storage.get("raw_dataset_file")
             mapping_file = local_storage.get("labels_mapping")
             return csv_file, mapping_file
         else:
             raise NotImplementedError(f"Either of wandb_storage or local_storage should be defined in app_cfg.yml")
```

### Comparing `sa_app-0.0.0/sa_app/data/data_cleaner.py` & `sa_app-0.0.1/sa_app/data/data_cleaner.py`

 * *Files identical despite different names*

### Comparing `sa_app-0.0.0/sa_app/data/kaggle_dataset.py` & `sa_app-0.0.1/sa_app/data/kaggle_dataset.py`

 * *Files identical despite different names*

### Comparing `sa_app-0.0.0/sa_app/inference/inference.py` & `sa_app-0.0.1/sa_app/inference/inference.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from typing import Dict
 
 import torch
 import yaml
 from sa_app.common.utils import load_mapping, parse_args
+from sa_app.data.data import InitializeDataset
 from sa_app.data.data_cleaner import StackedPreprocessor
 from transformers import AutoModelForSequenceClassification, AutoTokenizer
 
 
 class InferenceEngine:
     def __init__(self, inference_params: Dict, training_params: Dict, dataset_params: Dict, device: str):
         # Set the device to CPU or GPU
         self.device = device
 
         # Load the trained model and tokenizer
         self.model_path = inference_params["model_dir"]
         self.model = AutoModelForSequenceClassification.from_pretrained(self.model_path).to(self.device)
         self.tokenizer = AutoTokenizer.from_pretrained(training_params["tokenizer"])
         self.preprocessors = StackedPreprocessor(dataset_params["preprocessors"])
-        self.label_mapping = load_mapping(dataset_params["labels_mapping"])
+        dataset_obj = InitializeDataset(dataset_params)
+        _, label_mapping_path = dataset_obj()
+        self.label_mapping = load_mapping(label_mapping_path)
 
     def perform_inference(self, sentence):
         # Preprocess the input sentence
         sentence = self.preprocessors([sentence])[0]
 
         # Tokenize the input sentence
         inputs = self.tokenizer(sentence, truncation=True, padding=True, return_tensors="pt")
```

### Comparing `sa_app-0.0.0/sa_app/training/lightning_model_wrapper.py` & `sa_app-0.0.1/sa_app/training/lightning_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `sa_app-0.0.0/sa_app/training/optmizer.py` & `sa_app-0.0.1/sa_app/training/optmizer.py`

 * *Files identical despite different names*

### Comparing `sa_app-0.0.0/PKG-INFO` & `sa_app-0.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: sa-app
-Version: 0.0.0
+Version: 0.0.1
 Summary: Sentiment analyzer app
 Author: prabhu
 Author-email: prabhupad26@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: pandas (==1.5.1)
 Requires-Dist: pytorch-lightning (==2.0.4)
-Requires-Dist: spacy (==3.5.4)
+Requires-Dist: spacy (==3.6.0)
 Requires-Dist: torch (==2.0.1)
 Requires-Dist: transformers (==4.28.1)
 Requires-Dist: wandb (>=0.14.2,<0.15.0)
```

