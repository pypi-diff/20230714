# Comparing `tmp/neomaril-codex-1.0.3a0.tar.gz` & `tmp/neomaril-codex-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neomaril-codex-1.0.3a0.tar", last modified: Tue Jun 20 13:32:01 2023, max compression
+gzip compressed data, was "neomaril-codex-1.0.4.tar", last modified: Fri Jul 14 15:16:24 2023, max compression
```

## Comparing `neomaril-codex-1.0.3a0.tar` & `neomaril-codex-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-20 13:32:01.729350 neomaril-codex-1.0.3a0/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1060 2023-03-06 17:55:16.000000 neomaril-codex-1.0.3a0/LICENSE.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       24 2023-03-13 13:54:26.000000 neomaril-codex-1.0.3a0/MANIFEST.in
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1021 2023-06-20 13:32:01.729350 neomaril-codex-1.0.3a0/PKG-INFO
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      618 2023-03-15 18:53:09.000000 neomaril-codex-1.0.3a0/README.md
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       59 2023-06-20 13:15:46.000000 neomaril-codex-1.0.3a0/requirements.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       79 2023-06-20 13:32:01.733350 neomaril-codex-1.0.3a0/setup.cfg
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1029 2023-06-20 13:31:42.000000 neomaril-codex-1.0.3a0/setup.py
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-20 13:32:01.725350 neomaril-codex-1.0.3a0/src/
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-20 13:32:01.729350 neomaril-codex-1.0.3a0/src/neomaril_codex/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-02-08 17:56:54.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/__init__.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    12206 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/base.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      755 2023-02-08 17:56:54.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/exceptions.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     4487 2023-03-06 17:39:34.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/logging.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    44245 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/model.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    12562 2023-06-19 17:21:53.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/pipeline.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    32127 2023-06-20 13:15:32.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/training.py
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      655 2023-06-20 13:15:46.000000 neomaril-codex-1.0.3a0/src/neomaril_codex/utils.py
-drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-06-20 13:32:01.729350 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1021 2023-06-20 13:32:01.000000 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      558 2023-06-20 13:32:01.000000 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-06-20 13:32:01.000000 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-06-20 13:32:01.000000 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/not-zip-safe
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       60 2023-06-20 13:32:01.000000 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/requires.txt
--rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       15 2023-06-20 13:32:01.000000 neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/top_level.txt
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-07-14 15:16:24.358337 neomaril-codex-1.0.4/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1060 2023-03-06 17:55:16.000000 neomaril-codex-1.0.4/LICENSE.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       24 2023-03-13 13:54:26.000000 neomaril-codex-1.0.4/MANIFEST.in
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1018 2023-07-14 15:16:24.358337 neomaril-codex-1.0.4/PKG-INFO
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      618 2023-03-15 18:53:09.000000 neomaril-codex-1.0.4/README.md
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       59 2023-06-29 21:12:24.000000 neomaril-codex-1.0.4/requirements.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       79 2023-07-14 15:16:24.358337 neomaril-codex-1.0.4/setup.cfg
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1028 2023-07-14 15:16:22.000000 neomaril-codex-1.0.4/setup.py
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-07-14 15:16:24.354336 neomaril-codex-1.0.4/src/
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-07-14 15:16:24.358337 neomaril-codex-1.0.4/src/neomaril_codex/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-02-08 17:56:54.000000 neomaril-codex-1.0.4/src/neomaril_codex/__init__.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    12377 2023-07-14 15:16:22.000000 neomaril-codex-1.0.4/src/neomaril_codex/base.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      755 2023-02-08 17:56:54.000000 neomaril-codex-1.0.4/src/neomaril_codex/exceptions.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     4487 2023-03-06 17:39:34.000000 neomaril-codex-1.0.4/src/neomaril_codex/logging.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    44291 2023-07-14 15:16:22.000000 neomaril-codex-1.0.4/src/neomaril_codex/model.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    12562 2023-06-19 17:21:53.000000 neomaril-codex-1.0.4/src/neomaril_codex/pipeline.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)    32757 2023-07-14 15:16:22.000000 neomaril-codex-1.0.4/src/neomaril_codex/training.py
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      655 2023-06-29 21:12:24.000000 neomaril-codex-1.0.4/src/neomaril_codex/utils.py
+drwxrwxr-x   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        0 2023-07-14 15:16:24.358337 neomaril-codex-1.0.4/src/neomaril_codex.egg-info/
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)     1018 2023-07-14 15:16:24.000000 neomaril-codex-1.0.4/src/neomaril_codex.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)      558 2023-07-14 15:16:24.000000 neomaril-codex-1.0.4/src/neomaril_codex.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-07-14 15:16:24.000000 neomaril-codex-1.0.4/src/neomaril_codex.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)        1 2023-06-20 13:32:01.000000 neomaril-codex-1.0.4/src/neomaril_codex.egg-info/not-zip-safe
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       60 2023-07-14 15:16:24.000000 neomaril-codex-1.0.4/src/neomaril_codex.egg-info/requires.txt
+-rw-rw-r--   0 jonathan-carvalho  (1001) jonathan-carvalho  (1001)       15 2023-07-14 15:16:24.000000 neomaril-codex-1.0.4/src/neomaril_codex.egg-info/top_level.txt
```

### Comparing `neomaril-codex-1.0.3a0/LICENSE.txt` & `neomaril-codex-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3a0/PKG-INFO` & `neomaril-codex-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: neomaril-codex
-Version: 1.0.3a0
+Version: 1.0.4
 Summary: Python tools for interact with Neomaril
 Home-page: https://datarisk-io.github.io/mlops-neomaril-codex/
-Download-URL: https://github.com/datarisk-io/mlops-neomaril-codex/archive/refs/tags/v1.0.3a.tar.gz
+Download-URL: https://github.com/datarisk-io/mlops-neomaril-codex/archive/refs/tags/v1.0.4.tar.gz
 Author: Datarisk
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Neomaril Codex
```

### Comparing `neomaril-codex-1.0.3a0/README.md` & `neomaril-codex-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3a0/setup.py` & `neomaril-codex-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os.path import join
 
 from setuptools import setup, find_packages
 
 MODULE_NAME = 'neomaril-codex'
 MODULE_NAME_IMPORT = 'neomaril_codex'
 REPO_NAME = 'mlops-neomaril-codex'
-MODULE_VERSION='1.0.3a'
+MODULE_VERSION='1.0.4'
 
 def requirements_from_pip(filename='requirements.txt'):
     with open(filename, 'r') as pip:
         return [l.strip() for l in pip if not l.startswith('#') and l.strip()]
 
 
 setup(name=MODULE_NAME,
```

### Comparing `neomaril-codex-1.0.3a0/src/neomaril_codex/base.py` & `neomaril-codex-1.0.4/src/neomaril_codex/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,17 +148,18 @@
 		data = {"name": name, "description": description}
 
 		url = f"{self.base_url}/groups"
 		response = requests.post(url, data=data,
 								headers={'Authorization': 'Bearer ' + self.__credentials})
 
 		if response.status_code == 201:
-			logger.info(response.json()['Message'])
-			return True
+			logger.info(f"Group '{name}' inserted. Use the token for scoring. Carefully save it as we won't show it again.")
+			return response.json()['Token']
 		elif response.status_code < 500:
+			logger.error(response.text)
 			logger.error("Group already exist, nothing was changed.")
 			return False
 		else:
 			raise ServerError('Unexpected server error: ', response.text)
 
 	def refresh_group_token(self, name:str, force:bool=False) -> bool:
 		"""
@@ -199,15 +200,16 @@
 		"""
 
 		url = f"{self.base_url}/refresh/{name}"
 		response = requests.get(url, params={'force': str(force).lower()},
 														 headers={'Authorization': 'Bearer ' + self.__credentials})
 
 		if response.status_code == 201:
-				return response.json()['Message']
+				logger.info(f"Group '{name}' was refreshed")
+				return response.json()['Token']
 		else:
 				raise ServerError('Unexpected server error: ', response.text)
 		
 
 class NeomarilExecution(BaseNeomaril):
 	"""
 	Base class for Neomaril asynchronous model executions. With this class you can visualize the status of an execution and download the results after and execution has finished.
```

### Comparing `neomaril-codex-1.0.3a0/src/neomaril_codex/exceptions.py` & `neomaril-codex-1.0.4/src/neomaril_codex/exceptions.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3a0/src/neomaril_codex/logging.py` & `neomaril-codex-1.0.4/src/neomaril_codex/logging.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3a0/src/neomaril_codex/model.py` & `neomaril-codex-1.0.4/src/neomaril_codex/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,28 +339,29 @@
                     req = requests.post(url, files=[("input", (data.split('/')[-1], open(data, "rb")))],
                                                     headers={'Authorization': 'Bearer ' + group_token})
 
                     if req.status_code == 202:
                         message = req.json()
                         logger.info(message['Message'])
                         exec_id = message['ExecutionId']
-                        run = NeomarilExecution(self.model_id, 'AsyncModel', exec_id=exec_id, password=self.__credentials, 
-                                                url=self.base_url, group=self.group, group_token=group_token)
+                        run = NeomarilExecution(self.model_id, 'AsyncModel', group=self.group, exec_id=exec_id, password=self.__credentials, 
+                                                url=self.base_url, group_token=group_token)
                         response = run.get_status()
                         status = response['Status']
                         if wait_complete:
                             print('Wating the training run.', end='')
                             while status in ['Running', 'Requested']:
                                 sleep(30)
                                 print('.', end='', flush=True)
                                 response = run.get_status()
                                 status = response['Status']
                         if status == 'Failed':
                             logger.error(response['Message'])
                             raise ExecutionError("Training execution failed")
+                        return run
                     else:
                         raise ServerError(req.text)
                 
             else:
                 raise AuthenticationError("Group token not informed")
         else:
             url = f"{self.base_url}/model/describe/{self.group}/{self.model_id}"
@@ -398,54 +399,54 @@
 
         if self.operation == 'sync':
             payload = json.dumps({"Input": self.schema})
             base_url = self.base_url.replace('localhost:7070', 'localhost:7071') 
             if language == 'curl':
                 return f"""curl --request POST \\
                     --url {base_url}/model/sync/run/{self.group}/{self.model_id} \\
-                    --header 'Authorization: Bearer {self.__token}' \\
+                    --header 'Authorization: Bearer TOKEN' \\
                     --header 'Content-Type: application/json' \\
                     --data '{payload}'
                 """
             if language == 'python':
                 return f"""
                     import requests
 
                     url = "{base_url}/model/sync/run/{self.group}/{self.model_id}"
 
                     payload = {payload}
                     headers = {{
                         "Content-Type": "application/json",
-                        "Authorization": "Bearer {self.__token}"
+                        "Authorization": "Bearer TOKEN"
                     }}
 
                     response = requests.request("POST", url, json=payload, headers=headers)
 
                     print(response.text)
                 """
             if language == 'javascript':
                 return f"""
                     const options = {{
                     method: 'POST',
-                    headers: {{'Content-Type': 'application/json', Authorization: 'Bearer {self.__token}'}},
+                    headers: {{'Content-Type': 'application/json', Authorization: 'Bearer TOKEN'}},
                     body: '{payload}'
                     }};
 
                     fetch('{base_url}/model/sync/run/{self.group}/{self.model_id}', options)
                     .then(response => response.json())
                     .then(response => console.log(response))
                     .catch(err => console.error(err));
 
                 """
         if self.operation == 'async':
             if language == 'curl':
                 return f"""
                     curl --request POST \
                     --url {self.base_url}/model/async/run/{self.group}/{self.model_id} \\
-                    --header 'Authorization: Bearer {self.__token}' \\
+                    --header 'Authorization: Bearer TOKEN' \\
                     --header 'Content-Type: multipart/form-data' \\
                     --form "input=@/path/to/file"
                 """
             if language == 'python':
                 return f"""
                     import requests
 
@@ -453,15 +454,15 @@
 
                     upload_data = [
                         ("input", ('filename', open('/path/to/file', 'r'))),
                     ]
 
                     headers = {{
                         "Content-Type": "multipart/form-data",
-                        "Authorization": "Bearer {self.__token}"
+                        "Authorization": "Bearer TOKEN"
                     }}
 
                     response = requests.request("POST", url, files=upload_data, headers=headers)
 
                     print(response.text)
                 """
             if language == 'javascript':
@@ -469,15 +470,15 @@
                     const form = new FormData();
                     form.append("input", "/path/to/file");
 
                     const options = {{
                     method: 'POST',
                     headers: {{
                         'Content-Type': 'multipart/form-data',
-                        Authorization: 'Bearer {self.__token}'
+                        Authorization: 'Bearer TOKEN'
                     }}
                     }};
 
                     options.body = form;
 
                     fetch('{self.base_url}/model/async/run/{self.group}/{self.model_id}', options)
                     .then(response => response.json())
@@ -503,16 +504,18 @@
             If the user tries to get a execution from a Sync model 
 
         Example
         -------
         >>> model.get_model_execution('1')
         """
         if self.operation == 'async':
-            return NeomarilExecution(self.model_id, 'AsyncModel', exec_id, password=self.__credentials, 
-                                     url=self.base_url, group=self.group)
+            run = NeomarilExecution(self.model_id, 'AsyncModel', group=self.group, exec_id=exec_id, password=self.__credentials, 
+                                     url=self.base_url, group_token=self.__token)
+            run.get_status()
+            return run
         else:
             raise ModelError("Sync models don't have executions")
 
     def register_monitoring(self, preprocess_reference:str, shap_reference:str, configuration_file:Union[str, dict], preprocess_file:Optional[str]=None,
                             requirements_file:Optional[str]=None) -> str:
         """
         Register the model monitoring configuration at the database
@@ -1039,15 +1042,15 @@
         schema : Union[str, dict]
             Path to a JSON or XML file with a sample of the input for the entrypoint function. A dict with the sample input can be send as well. Mandatory for Sync models
         group : str
             Group the model is inserted. Default to 'datarisk' (public group)
         extra_files : list, optional
             A optional list with additional files paths that should be uploaded. If the scoring function refer to this file they will be on the same folder as the source file
         env : str, optional
-            Flag that choose which environment (dev, staging, production) of Neomaril you are using. Default is True
+            .env file to be used in your model enviroment. This will be encrypted in the server.
         python_version : str, optional
             Python version for the model environment. Avaliable versions are 3.7, 3.8, 3.9, 3.10. Defaults to '3.8'
         operation : str
             Defines wich kind operation is beeing executed (Sync or Async). Default value is Sync
         input_type : str
             The type of the input file that should be 'json', 'csv' or 'parquet'
         wait_for_ready : bool, optional
```

### Comparing `neomaril-codex-1.0.3a0/src/neomaril_codex/pipeline.py` & `neomaril-codex-1.0.4/src/neomaril_codex/pipeline.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3a0/src/neomaril_codex/training.py` & `neomaril-codex-1.0.4/src/neomaril_codex/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,22 @@
         load_dotenv()
         self.__credentials = os.getenv('NEOMARIL_TOKEN') if os.getenv('NEOMARIL_TOKEN') else password
 
         self.training_id = training_id
         self.group = group
     
         self.training_type = self.execution_data['TrainingType']
+        self.name = self.execution_data['ExperimentName']
         self.run_data = self.execution_data['RunData']
 
+
+    def __repr__(self) -> str:
+        return f"""Neomaril{self.exec_type}Execution(name="{self.name}",
+                                        exec_id="{self.exec_id}", status="{self.status}")"""
+    
     def __upload_model(self, model_name:str, model_reference:Optional[str]=None, source_file:Optional[str]=None, 
                                          schema:Optional[Union[str, dict]]=None, extra_files:Optional[list]=None, 
                                          env:Optional[str]=None, operation:str='Sync', input_type:str=None) -> str:
         """
         Upload the files to the server
 
         Arguments
@@ -367,15 +373,15 @@
 
     def __str__(self):
         return f'NEOMARIL training experiment "{self.experiment_name} (Group: {self.group}, Id: {self.training_id})"'
     
     def __upload_training(self, run_name:str, train_data:str, training_reference:Optional[str]=None, 
                                                 python_version:str='3.8', conf_dict:Optional[Union[str, dict]]=None,
                                                 source_file:Optional[str]=None, requirements_file:Optional[str]=None,
-                                                extra_files:Optional[list]=None) -> str:
+                                                env:Optional[str]=None, extra_files:Optional[list]=None) -> str:
         
         """
         Upload the files to the server
 
         Arguments
         ---------
         run_name : str
@@ -388,14 +394,16 @@
             Python version for the model environment. Avaliable versions are 3.7, 3.8, 3.9, 3.10. Defaults to '3.8'. Just used when training_type is Custom
         conf_dict : Union[str, dict], optional
             Path to a JSON file with a the AutoML configuration. A dict can be send as well. Just used when training_type is AutoML
         source_file : str, optional
             Path of the source file. The file must have a training function that accepts one parameter: model_path (absolute path of where the file is located). Just used when training_type is Custom
         requirements_file : str, optional
             Path of the requirements file. The packages versions must be fixed eg: pandas==1.0. Just used when training_type is Custom
+        env : str, optional
+            .env file to be used in your training enviroment. This will be encrypted in the server.
         extra_files : list, optional
             A optional list with additional files paths that should be uploaded. If the scoring function refer to this file they will be on the same folder as the source file. Just used when training_type is Custom
         
         Raises
         ------
         InputError
             Some input parameters its invalid
@@ -416,14 +424,17 @@
         
             file_extesions = {'py': 'app.py', 'ipynb': "notebook.ipynb"}
         
             upload_data = upload_data + [
                 ("source", (file_extesions[source_file.split('.')[-1]], open(source_file, "r"))),
                 ("requirements", ("requirements.txt", open(requirements_file, "r")))
             ]
+
+            if env:
+                upload_data.append(("env", (".env", env)))
          
             if extra_files:
                 extra_data = [('extra', (c.split('/')[-1], open(c, "r"))) for c in extra_files]
                 
                 upload_data += extra_data
                 
             form_data = {'run_name': run_name, 'training_reference': training_reference,
@@ -484,20 +495,21 @@
         if response.status_code == 404:
             raise ModelError(f'Experiment "{self.training_id}" not found.')
             
         elif response.status_code >= 500:
             raise ModelError(f'Unable to retrive experiment "{self.training_id}"')
     
         self.training_data = response.json()['Description']
-        self.executions = self.training_data['Executions']
+        self.executions = [c['Id'] for c in self.training_data['Executions']]
 
     def run_training(self, run_name:str, train_data:str, training_reference:Optional[str]=None, 
                      python_version:str='3.8', conf_dict:Optional[Union[str, dict]]=None,
                      source_file:Optional[str]=None, requirements_file:Optional[str]=None,
-                     extra_files:Optional[list]=None, wait_complete:Optional[bool]=False) -> Union[dict, NeomarilExecution]:
+                     extra_files:Optional[list]=None, env:Optional[str]=None,
+                     wait_complete:Optional[bool]=False) -> Union[dict, NeomarilExecution]:
         """
         Runs a prediction from the current model.
 
         Arguments
         ---------
         run_name : str
             The name of the model, in less than 32 characters
@@ -509,14 +521,16 @@
             Python version for the model environment. Avaliable versions are 3.7, 3.8, 3.9, 3.10. Defaults to '3.8'. Just used when training_type is Custom
         conf_dict : Union[str, dict]
             Path to a JSON file with a the AutoML configuration. A dict can be send as well. Just used when training_type is AutoML
         source_file : str, optional
             Path of the source file. The file must have a training function that accepts one parameter: model_path (absolute path of where the file is located). Just used when training_type is Custom
         requirements_file : str
             Path of the requirements file. The packages versions must be fixed eg: pandas==1.0. Just used when training_type is Custom
+        env : str, optional
+            .env file to be used in your training enviroment. This will be encrypted in the server.
         extra_files : list, optional
             A optional list with additional files paths that should be uploaded. If the scoring function refer to this file they will be on the same folder as the source file. Just used when training_type is Custom
         wait_complete : bool, optional
             Boolean that informs if a model training is completed (True) or not (False). Default value is False
         
         Raises
         ------
@@ -533,16 +547,16 @@
         >>> execution = run = training.run_training('First test', data_path+'dados.csv', training_reference='train_model', python_version='3.9', requirements_file=data_path+'requirements.txt', wait_complete=True)
         """
         if python_version not in ['3.7', '3.8', '3.9', '3.10']:
             raise InputError('Invalid python version. Avaliable versions are 3.7, 3.8, 3.9, 3.10')
 
         if self.training_type == 'Custom':
             exec_id = self.__upload_training(run_name, train_data, training_reference=training_reference,
-                                                                            python_version=python_version, source_file=source_file,
-                                                                            requirements_file=requirements_file, extra_files=extra_files)
+                                            python_version=python_version, source_file=source_file, env=env,
+                                            requirements_file=requirements_file, extra_files=extra_files)
 
         elif self.training_type == 'AutoML':
             exec_id = self.__upload_training(run_name, train_data, conf_dict=conf_dict)
 
         else:
             raise InputError('Invalid training type')
```

### Comparing `neomaril-codex-1.0.3a0/src/neomaril_codex/utils.py` & `neomaril-codex-1.0.4/src/neomaril_codex/utils.py`

 * *Files identical despite different names*

### Comparing `neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/PKG-INFO` & `neomaril-codex-1.0.4/src/neomaril_codex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: neomaril-codex
-Version: 1.0.3a0
+Version: 1.0.4
 Summary: Python tools for interact with Neomaril
 Home-page: https://datarisk-io.github.io/mlops-neomaril-codex/
-Download-URL: https://github.com/datarisk-io/mlops-neomaril-codex/archive/refs/tags/v1.0.3a.tar.gz
+Download-URL: https://github.com/datarisk-io/mlops-neomaril-codex/archive/refs/tags/v1.0.4.tar.gz
 Author: Datarisk
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Neomaril Codex
```

### Comparing `neomaril-codex-1.0.3a0/src/neomaril_codex.egg-info/SOURCES.txt` & `neomaril-codex-1.0.4/src/neomaril_codex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

