# Comparing `tmp/PlanaPY-0.2.7.tar.gz` & `tmp/PlanaPY-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlanaPY-0.2.7.tar", last modified: Wed Jun 14 21:45:22 2023, max compression
+gzip compressed data, was "PlanaPY-0.2.8.tar", last modified: Thu Jul 13 22:32:07 2023, max compression
```

## Comparing `PlanaPY-0.2.7.tar` & `PlanaPY-0.2.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 21:45:22.961461 PlanaPY-0.2.7/
--rw-rw-rw-   0        0        0      286 2023-06-14 21:45:22.960683 PlanaPY-0.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 21:45:22.952093 PlanaPY-0.2.7/PlanaPY/
--rw-rw-rw-   0        0        0    16725 2023-06-14 21:23:23.000000 PlanaPY-0.2.7/PlanaPY/PlanaPY.py
--rw-rw-rw-   0        0        0       21 2023-06-09 20:22:08.000000 PlanaPY-0.2.7/PlanaPY/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 21:45:22.959512 PlanaPY-0.2.7/PlanaPY.egg-info/
--rw-rw-rw-   0        0        0      286 2023-06-14 21:45:22.000000 PlanaPY-0.2.7/PlanaPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-14 21:45:22.000000 PlanaPY-0.2.7/PlanaPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 21:45:22.000000 PlanaPY-0.2.7/PlanaPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-14 21:45:22.000000 PlanaPY-0.2.7/PlanaPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-14 21:45:22.000000 PlanaPY-0.2.7/PlanaPY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 21:45:22.961461 PlanaPY-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      485 2023-06-14 21:45:16.000000 PlanaPY-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 22:32:07.781454 PlanaPY-0.2.8/
+-rw-rw-rw-   0        0        0      286 2023-07-13 22:32:07.781454 PlanaPY-0.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 22:32:07.773721 PlanaPY-0.2.8/PlanaPY/
+-rw-rw-rw-   0        0        0    17304 2023-07-13 22:26:48.000000 PlanaPY-0.2.8/PlanaPY/PlanaPY.py
+-rw-rw-rw-   0        0        0       21 2023-06-09 20:22:08.000000 PlanaPY-0.2.8/PlanaPY/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 22:32:07.779721 PlanaPY-0.2.8/PlanaPY.egg-info/
+-rw-rw-rw-   0        0        0      286 2023-07-13 22:32:07.000000 PlanaPY-0.2.8/PlanaPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-07-13 22:32:07.000000 PlanaPY-0.2.8/PlanaPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 22:32:07.000000 PlanaPY-0.2.8/PlanaPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-13 22:32:07.000000 PlanaPY-0.2.8/PlanaPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 22:32:07.000000 PlanaPY-0.2.8/PlanaPY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-13 22:32:07.781454 PlanaPY-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      485 2023-07-13 22:29:02.000000 PlanaPY-0.2.8/setup.py
```

### Comparing `PlanaPY-0.2.7/PlanaPY/PlanaPY.py` & `PlanaPY-0.2.8/PlanaPY/PlanaPY.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,406 +1,408 @@
-import requests
-from requests.structures import CaseInsensitiveDict
-import json
-import pandas as pd
-from time import gmtime, strftime
-import time
-import io 
-
-class AnaplanAPI: 
-    def __init__(self):
-        self.headers = CaseInsensitiveDict()
-        self.headers['Content-Length'] = "0"
-        self.token = ""
-        self.response_results = dict()
-        self.api_url = "https://api.anaplan.com/2/0/"
-        self.token_url = "https://auth.anaplan.com/token/"
-        
-    def acquire_token(self, username, password):
-        URL = self.token_url + "authenticate"
-        
-        try:
-            self.resp = requests.post(
-                URL
-                ,auth=(username, password)
-            )
-            self.response_results = self.resp.json()
-            self.token = self.response_results['tokenInfo']['tokenValue']
-            self.headers['authorization'] = "AnaplanAuthToken {0}".format(self.token)
-
-        except Exception as e:
-            print('Error occurred: {0}'.format(e))
-        
-        return self.resp.status_code
-    
-    def token_check(self):
-        if not self.token:
-            print("No active token. Please first run the acquire_token function.")
-        return self.token
-        
-    def token_details(self):
-        URL = self.token_url + "validate"
-        
-        if not self.token_check():
-            return
-        
-        try:
-            self.resp = requests.get(URL, headers=self.headers)
-            self.response_results = self.resp.json()
-        except Exception as e:
-            print("Error occurred: {0}".format(e))
-        
-        print(self.resp.status_code)
-        return self.resp.json()
-    
-    def refresh_token(self):
-        URL = self.token_url + "refresh"
-
-        if not self.token_check():
-            return
-        
-        try:
-            self.resp = requests.post(URL, headers=self.headers)
-            self.response_results = self.resp.json()
-            self.token = self.response_results['tokenInfo']['tokenValue']
-        except Exception as e:
-            print("Error occurred: {0}".format(e))
-            
-        return self.resp.status_code
-    
-    def end_session(self):
-        URL = self.token_url + "logout"
-        
-        if not self.token_check():
-            return
-        
-        try:
-            self.resp = requests.post(URL, headers=self.headers)
-            print("Successfully ended session.")
-        except Exception as e:
-            print("Error occurred: {0}".format(e))
-            
-        return self.resp.status_code  
-		
-class AnaplanModels:
-    def __init__(self, api):
-        self.api = api
-        self.info = self.model_info()
-        self.models = self.get_models()
-        self.workspaces = { 
-            'workspace_id' : list(set([c['currentWorkspaceId'] for c in self.info['models']]))
-            ,'workspace_name' : list(set([c['currentWorkspaceName'] for c in self.info['models']]))
-        }
-    
-    def get_request(self, URL):
-        try:
-            self.resp = requests.get(URL, headers=self.api.headers)
-        except Exception as e:
-            print("Error occurred: {0}".format(e))
-            return self.resp.status_code
-            
-#         print(self.resp.status_code)    
-        
-        return self.resp.json()
-    
-    def put_request(self, URL, body):  
-        try:
-            self.api.headers['Content-Type'] = 'application/json'
-            self.resp = requests.put(URL, headers=self.api.headers, json=body)
-            self.api.headers.pop('Content-Type')
-        except Exception as e:
-            print("Error occurred: {0}".format(e))
-            return self.resp.status_code
-
-        print(self.resp.status_code)    
-        
-        return self.resp
-        
-    def model_info(self):
-        URL = self.api.api_url + "models"
-        return self.get_request(URL)
-    
-    def get_models(self):
-        mods = pd.json_normalize(self.info['models'])
-        return mods   
-        
-    def get_model_files(self, model, workspace):
-        file_dict = {}
-        
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        URL = self.api.api_url + "models/{0}/files".format(model_id)
-        files = self.get_request(URL)['files']
-        
-        for f in files:
-            file_dict[f['name']] = f
-        
-        return file_dict
-    
-    def import_file(self, model, workspace, file):
-        self.api.headers['Content-Type'] = 'application/octet-stream'
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        filename = file.split('\\')[-1]
-        file_id = self.get_model_files(model=model, workspace = workspace)[filename]['id']
-        
-        URL = self.api.api_url + "models/{0}/files/{1}".format(model_id, file_id)
-        body = {'upload-file': file}
-        
-        self.resp = requests.put(URL, headers=self.api.headers, data = open(file, 'rb'), json=body)
-        self.api.headers.pop('Content-Type')
-        
-        if self.resp.status_code == 204:
-            print("File {0} successfully uploaded to model {1}".format(file, model))
-        
-        return self.resp
-
-    def get_processes(self, model, workspace):
-        process_dict = {}
-        
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        URL = self.api.api_url + "models/{0}/processes".format(model_id)
-        
-        processes = self.get_request(URL)['processes']
-        
-        for p in processes:
-            process_dict[p['name']] = p
-        
-        return process_dict
-        
-    def run_process(self, model, workspace, process):
-        self.api.headers['Content-Type'] = 'application/json'
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        process_id = self.get_processes(model=model, workspace=workspace)[process]['id']
-        
-        URL = self.api.api_url + "models/{0}/processes/{1}/tasks".format(model_id, process_id)
-        body = {'localeName': 'en_US'}
-        
-        self.resp = requests.post(URL, headers=self.api.headers, json=body)
-        self.api.headers.pop('Content-Type')
-        
-        if self.resp.status_code == 204:
-            print("Process {0} successfully started in model {1}".format(file, model))
-              
-        ## Check Process Run status
-        start = time.time()
-        time_diff = 10 
-        
-        while True:            
-            tasks_dict = {}
-            tasks = self.get_request(URL)['tasks']
-            for t in tasks:
-                tasks_dict[t['taskId']] = t
-
-            complete_count = len(tasks_dict)
-            for t, v in tasks_dict.items():
-                if v['taskState'] == "COMPLETE":
-#                     print("Task {0} is complete.".format(t))
-                    complete_count -= 1
-                else:
-                    if time.time() - start > time_diff:
-                        print("""Task {0} in state {1}. 
-                              Checked at time {2}""".format(t, 
-                                                            v['taskState'], 
-                                                            strftime("%Y-%m-%d %H:%M:%S", gmtime())
-                                                            ))
-                        start += time_diff
-            if complete_count == 0:
-                print("task {0} in state {1} at time {2}".format(t, 
-                                                                 v['taskState'],
-                                                                 strftime("%Y-%m-%d %H:%M:%S", gmtime())
-                                                                ))
-                break
-                
-        return self.resp
-
-    def get_delete_actions(self, model, workspace):
-        actions_dict = {}
-        
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        URL = self.api.api_url + "models/{0}/actions".format(model_id)
-        
-        actions = self.get_request(URL)['actions']
-        
-        for a in actions:
-            actions_dict[a['name']] = a
-        
-        return actions_dict
-
-    def run_delete_action(self, model, workspace, action):
-        self.api.headers['Content-Type'] = 'application/json'
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        action_id = self.get_delete_actions(model=model, workspace=workspace)[action]['id']
-        
-        URL = self.api.api_url + "models/{0}/actions/{1}/tasks".format(model_id, action_id)
-        body = {'localeName': 'en_US'}
-        
-        self.resp = requests.post(URL, headers=self.api.headers, json=body)
-        self.api.headers.pop('Content-Type')
-        
-        if self.resp.status_code == 204:
-            print("Delete action {0} successfully ran in model {1}".format(file, model))
-        
-        return self.resp 
-    
-    def get_export_actions(self, model, workspace):
-        exports_dict = {}
-        
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        URL = self.api.api_url + "models/{0}/exports".format(model_id)
-        
-        actions = self.get_request(URL)['exports']
-        
-        for a in actions:
-            exports_dict[a['name']] = a
-        
-        return exports_dict
-    
-    def get_export_metadata(self, model, workspace, export):
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        export_id = self.get_export_actions(model=model, workspace=workspace)[export]['id']
-        
-        URL = self.api.api_url + "models/{0}/exports/{1}".format(model_id, export_id)
-        
-        metadata = self.get_request(URL)['exportMetadata']
-        
-        columns = metadata['headerNames']
-        #export_format = metadata['exportFormat']
-        delimiter = metadata['separator']
-                
-        return columns, delimiter
-    
-    def run_export_action(self, model, workspace, export):
-        self.api.headers['Content-Type'] = 'application/json'
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        action_id = self.get_export_actions(model=model, workspace=workspace)[export]['id']
-        
-        URL = self.api.api_url + "models/{0}/exports/{1}/tasks".format(model_id, action_id)
-        body = {'localeName': 'en_US'}
-        
-        self.resp = requests.post(URL, headers=self.api.headers, json=body)
-        self.api.headers.pop('Content-Type')
-        
-        if self.resp.status_code == 204:
-            print("Export action {0} successfully ran in model {1}".format(file, model))
-        
-        return self.resp 
-    
-    def export_data(self, model, workspace, export):
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        file_id = self.get_model_files(model=model, workspace = workspace)[export]['id']
-
-        columns, delimiter = self.get_export_metadata(model=model, workspace=workspace, export=export)
-        
-        URL = self.api.api_url + "models/{0}/files/{1}/chunks".format(model_id, file_id)
-
-        chunks = self.get_request(URL)['chunks']
-
-        chunk_list = []
-        
-        for c in chunks:
-            chunk_id = c['id']
-            chunk_URL = self.api.api_url + "models/{0}/files/{1}/chunks/{2}".format(model_id, file_id, chunk_id)
-            chunk = requests.get(chunk_URL, headers = self.api.headers).content
-            df = pd.read_csv(
-                io.StringIO(chunk.decode('utf-8')), 
-                header=None, 
-                sep=delimiter, 
-                error_bad_lines=False,
-                warn_bad_lines=True)
-            chunk_list.append(df)
-
-        all_chunks = pd.concat(chunk_list).reset_index()
-        all_chunks.columns = all_chunks.iloc[0]
-        #all_chunks.columns = columns
-        all_chunks.drop(all_chunks.index[0], inplace=True)
-        all_chunks = all_chunks.iloc[:,1:]
-        
-        return all_chunks       
-        
-    def change_model_status(self, model, workspace, status):
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        URL = self.api.api_url + "models/{0}/onlineStatus".format(model_id)
-        body = {'status': status}
-        
-        resp = self.put_request(URL, body)
-        
-        if resp.status_code == 204:
-            print("Model {0} successfully set to {1}".format(model, status))
-        
-        return resp
-    
-    def compatible_revisions(self, source_model, target_model, workspace):
-        s_model_id = self.models[(self.models.name == source_model) 
-                                            & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        t_model_id = self.models[(self.models.name == source_model) 
-                                 & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-
-        URL = self.api.api_url + "models/{0}/alm/syncableRevisions?sourceModelId={1}".format(t_model_id, s_model_id)
-        
-        return self.get_request(URL)
-    
-    def latest_revision(self, model, workspace):
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        URL = self.api.api_url + "models/{0}/alm/latestRevision".format(model_id)
-        
-        return self.get_request(URL)
-    
-    def all_revisions(self, model, workspace):
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        URL = self.api.api_url + "models/{0}/alm/revisions".format(model_id)
-        
-        return self.get_request(URL)
-    
-    def sync_models(self, source_model, target_model, workspace):
-        s_model_id = self.models[(self.models.name == source_model) 
-                                            & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        t_model_id = self.models[(self.models.name == source_model) 
-                                 & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-
-        URL = self.api.api_url + "models/{0}/alm/syncTasks".format(t_model_id)
-        
-        try:
-            body = {
-                "sourceRevisionId": self.compatible_revisions( ## most recent compatible revision
-                                        source_model = source_model, 
-                                        target_model = target_model)['revisions'][0]['id'],
-                "sourceModelId": s_model_id,
-                "targetRevisionId": self.latest_revision(target_model)['revisions'][0]['id'] ## most recent revivsion push
-            }
-            self.api.headers['Content-Type'] = 'application/json'
-            self.resp = requests.post(URL, headers=self.api.headers, json=body)
-            self.api.headers.pop('Content-Type')
-        except Exception as e:
-            print("Error occurred: {0}".format(e))
-            print("Unable to sync source model {0} with target model {1}".format(source_model, target_model))
-            return self.resp.status_code
-
-        print(self.resp.status_code)    
-        
-        return self.resp
-    
-    def sync_tasks_list(self, model, workspace):
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        URL = self.api.api_url + "models/{0}/alm/syncTasks".format(model_id)
-        
-        return self.get_request(URL)
-        
-#     def sync_status(self, model):
-#         model_id = self.models[model]['id']
-#         URL = self.api.api_url + "models/{0}/alm/syncTasks"
-        
-    def create_revision(self, model, workspace, rev_name, rev_desc):
-        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
-        URL = self.api.api_url + "models/{0}/alm/revisions".format(model_id)
-        
-        try:
-            body = {
-                "name": rev_name,
-                "description": rev_desc
-            }
-            self.api.headers['Content-Type'] = 'application/json'
-            self.resp = requests.post(URL, headers=self.api.headers, json=body)
-            self.api.headers.pop('Content-Type')
-        except Exception as e:
-            print("Error occurred: {0}".format(e))
-            return self.resp.status_code
-        
+import requests
+from requests.structures import CaseInsensitiveDict
+import json
+import pandas as pd
+from time import gmtime, strftime
+import time
+import io 
+
+class AnaplanAPI: 
+    def __init__(self):
+        self.headers = CaseInsensitiveDict()
+        self.headers['Content-Length'] = "0"
+        self.token = ""
+        self.response_results = dict()
+        self.api_url = "https://api.anaplan.com/2/0/"
+        self.token_url = "https://auth.anaplan.com/token/"
+        
+    def acquire_token(self, username, password):
+        URL = self.token_url + "authenticate"
+        
+        try:
+            self.resp = requests.post(
+                URL
+                ,auth=(username, password)
+            )
+            self.response_results = self.resp.json()
+            self.token = self.response_results['tokenInfo']['tokenValue']
+            self.headers['authorization'] = "AnaplanAuthToken {0}".format(self.token)
+
+        except Exception as e:
+            print('Error occurred: {0}'.format(e))
+        
+        return self.resp.status_code
+    
+    def token_check(self):
+        if not self.token:
+            print("No active token. Please first run the acquire_token function.")
+        return self.token
+        
+    def token_details(self):
+        URL = self.token_url + "validate"
+        
+        if not self.token_check():
+            return
+        
+        try:
+            self.resp = requests.get(URL, headers=self.headers)
+            self.response_results = self.resp.json()
+        except Exception as e:
+            print("Error occurred: {0}".format(e))
+        
+        print(self.resp.status_code)
+        return self.resp.json()
+    
+    def refresh_token(self):
+        URL = self.token_url + "refresh"
+
+        if not self.token_check():
+            return
+        
+        try:
+            self.resp = requests.post(URL, headers=self.headers)
+            self.response_results = self.resp.json()
+            self.token = self.response_results['tokenInfo']['tokenValue']
+        except Exception as e:
+            print("Error occurred: {0}".format(e))
+            
+        return self.resp.status_code
+    
+    def end_session(self):
+        URL = self.token_url + "logout"
+        
+        if not self.token_check():
+            return
+        
+        try:
+            self.resp = requests.post(URL, headers=self.headers)
+            print("Successfully ended session.")
+        except Exception as e:
+            print("Error occurred: {0}".format(e))
+            
+        return self.resp.status_code  
+		
+class AnaplanModels:
+    def __init__(self, api):
+        self.api = api
+        self.info = self.model_info()
+        self.models = self.get_models()
+        self.workspaces = { 
+            'workspace_id' : list(set([c['currentWorkspaceId'] for c in self.info['models']]))
+            ,'workspace_name' : list(set([c['currentWorkspaceName'] for c in self.info['models']]))
+        }
+    
+    def get_request(self, URL):
+        try:
+            self.resp = requests.get(URL, headers=self.api.headers)
+        except Exception as e:
+            print("Error occurred: {0}".format(e))
+            return self.resp.status_code
+            
+#         print(self.resp.status_code)    
+        
+        return self.resp.json()
+    
+    def put_request(self, URL, body):  
+        try:
+            self.api.headers['Content-Type'] = 'application/json'
+            self.resp = requests.put(URL, headers=self.api.headers, json=body)
+            self.api.headers.pop('Content-Type')
+        except Exception as e:
+            print("Error occurred: {0}".format(e))
+            return self.resp.status_code
+
+        print(self.resp.status_code)    
+        
+        return self.resp
+        
+    def model_info(self):
+        URL = self.api.api_url + "models"
+        return self.get_request(URL)
+    
+    def get_models(self):
+        mods = pd.json_normalize(self.info['models'])
+        return mods   
+        
+    def get_model_files(self, model, workspace):
+        file_dict = {}
+        
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        URL = self.api.api_url + "models/{0}/files".format(model_id)
+        files = self.get_request(URL)['files']
+        
+        for f in files:
+            file_dict[f['name']] = f
+        
+        return file_dict
+    
+    def import_file(self, model, workspace, file):
+        self.api.headers['Content-Type'] = 'application/octet-stream'
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        filename = file.split('\\')[-1]
+        file_id = self.get_model_files(model=model, workspace = workspace)[filename]['id']
+        
+        URL = self.api.api_url + "models/{0}/files/{1}".format(model_id, file_id)
+        body = {'upload-file': file}
+        
+        self.resp = requests.put(URL, headers=self.api.headers, data = open(file, 'rb'), json=body)
+        self.api.headers.pop('Content-Type')
+        
+        if self.resp.status_code == 204:
+            print("File {0} successfully uploaded to model {1}".format(file, model))
+        
+        return self.resp
+
+    def get_processes(self, model, workspace):
+        process_dict = {}
+        
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        URL = self.api.api_url + "models/{0}/processes".format(model_id)
+        
+        processes = self.get_request(URL)['processes']
+        
+        for p in processes:
+            process_dict[p['name']] = p
+        
+        return process_dict
+        
+    def run_process(self, model, workspace, process):
+        self.api.headers['Content-Type'] = 'application/json'
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        process_id = self.get_processes(model=model, workspace=workspace)[process]['id']
+        
+        URL = self.api.api_url + "models/{0}/processes/{1}/tasks".format(model_id, process_id)
+        body = {'localeName': 'en_US'}
+        
+        self.resp = requests.post(URL, headers=self.api.headers, json=body)
+        self.api.headers.pop('Content-Type')
+        
+        if self.resp.status_code == 204:
+            print("Process {0} successfully started in model {1}".format(file, model))
+              
+        ## Check Process Run status
+        start = time.time()
+        time_diff = 10 
+        
+        while True:            
+            tasks_dict = {}
+            tasks = self.get_request(URL)['tasks']
+            for t in tasks:
+                tasks_dict[t['taskId']] = t
+
+            complete_count = len(tasks_dict)
+            for t, v in tasks_dict.items():
+                if v['taskState'] == "COMPLETE":
+#                     print("Task {0} is complete.".format(t))
+                    complete_count -= 1
+                else:
+                    if time.time() - start > time_diff:
+                        print("""Task {0} in state {1}. 
+                              Checked at time {2}""".format(t, 
+                                                            v['taskState'], 
+                                                            strftime("%Y-%m-%d %H:%M:%S", gmtime())
+                                                            ))
+                        start += time_diff
+            if complete_count == 0:
+                print("task {0} in state {1} at time {2}".format(t, 
+                                                                 v['taskState'],
+                                                                 strftime("%Y-%m-%d %H:%M:%S", gmtime())
+                                                                ))
+                break
+                
+        return self.resp
+
+    def get_delete_actions(self, model, workspace):
+        actions_dict = {}
+        
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        URL = self.api.api_url + "models/{0}/actions".format(model_id)
+        
+        actions = self.get_request(URL)['actions']
+        
+        for a in actions:
+            actions_dict[a['name']] = a
+        
+        return actions_dict
+
+    def run_delete_action(self, model, workspace, action):
+        self.api.headers['Content-Type'] = 'application/json'
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        action_id = self.get_delete_actions(model=model, workspace=workspace)[action]['id']
+        
+        URL = self.api.api_url + "models/{0}/actions/{1}/tasks".format(model_id, action_id)
+        body = {'localeName': 'en_US'}
+        
+        self.resp = requests.post(URL, headers=self.api.headers, json=body)
+        self.api.headers.pop('Content-Type')
+        
+        if self.resp.status_code == 204:
+            print("Delete action {0} successfully ran in model {1}".format(file, model))
+        
+        return self.resp 
+    
+    def get_export_actions(self, model, workspace):
+        exports_dict = {}
+        
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        URL = self.api.api_url + "models/{0}/exports".format(model_id)
+        
+        actions = self.get_request(URL)['exports']
+        
+        for a in actions:
+            exports_dict[a['name']] = a
+        
+        return exports_dict
+    
+    def get_export_metadata(self, model, workspace, export):
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        export_id = self.get_export_actions(model=model, workspace=workspace)[export]['id']
+        
+        URL = self.api.api_url + "models/{0}/exports/{1}".format(model_id, export_id)
+        
+        metadata = self.get_request(URL)['exportMetadata']
+        
+        columns = metadata['headerNames']
+        #export_format = metadata['exportFormat']
+        delimiter = metadata['separator']
+                
+        return columns, delimiter
+    
+    def run_export_action(self, model, workspace, export):
+        self.api.headers['Content-Type'] = 'application/json'
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        action_id = self.get_export_actions(model=model, workspace=workspace)[export]['id']
+        
+        URL = self.api.api_url + "models/{0}/exports/{1}/tasks".format(model_id, action_id)
+        body = {'localeName': 'en_US'}
+        
+        self.resp = requests.post(URL, headers=self.api.headers, json=body)
+        self.api.headers.pop('Content-Type')
+        
+        if self.resp.status_code == 204:
+            print("Export action {0} successfully ran in model {1}".format(file, model))
+        
+        return self.resp 
+    
+    def export_data(self, model, workspace, export):
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        file_id = self.get_model_files(model=model, workspace = workspace)[export]['id']
+
+        columns, delimiter = self.get_export_metadata(model=model, workspace=workspace, export=export)
+        
+        URL = self.api.api_url + "models/{0}/files/{1}/chunks".format(model_id, file_id)
+
+        chunks = self.get_request(URL)['chunks']
+
+        chunk_list = []
+        
+        for c in chunks:
+            chunk_id = c['id']
+            chunk_URL = self.api.api_url + "models/{0}/files/{1}/chunks/{2}".format(model_id, file_id, chunk_id)
+            chunk = requests.get(chunk_URL, headers = self.api.headers).content
+            df = pd.read_csv(
+                io.StringIO(chunk.decode('utf-8')), 
+                header=None, 
+                sep=delimiter, 
+                error_bad_lines=False,
+                warn_bad_lines=True)
+            chunk_list.append(df)
+
+        all_chunks = pd.concat(chunk_list).reset_index()
+        all_chunks.columns = all_chunks.iloc[0]
+        #all_chunks.columns = columns
+        all_chunks.drop(all_chunks.index[0], inplace=True)
+        all_chunks = all_chunks.iloc[:,1:]
+        
+        return all_chunks       
+        
+    def change_model_status(self, model, workspace, status):
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        URL = self.api.api_url + "models/{0}/onlineStatus".format(model_id)
+        body = {'status': status}
+        
+        resp = self.put_request(URL, body)
+        
+        if resp.status_code == 204:
+            print("Model {0} successfully set to {1}".format(model, status))
+        
+        return resp
+    
+    def compatible_revisions(self, source_model, target_model, workspace):
+        s_model_id = self.models[(self.models.name == source_model) 
+                                            & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        t_model_id = self.models[(self.models.name == target_model) 
+                                 & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+
+        URL = self.api.api_url + "models/{0}/alm/syncableRevisions?sourceModelId={1}".format(t_model_id, s_model_id)
+
+        return self.get_request(URL)
+    
+    def latest_revision(self, model, workspace):
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        URL = self.api.api_url + "models/{0}/alm/latestRevision".format(model_id)
+        
+        return self.get_request(URL)
+    
+    def all_revisions(self, model, workspace):
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        URL = self.api.api_url + "models/{0}/alm/revisions".format(model_id)
+        
+        return self.get_request(URL)
+    
+    def sync_models(self, source_model, target_model, workspace):
+        s_model_id = self.models[(self.models.name == source_model) 
+                                            & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        t_model_id = self.models[(self.models.name == target_model) 
+                                 & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+
+        URL = self.api.api_url + "models/{0}/alm/syncTasks".format(t_model_id)
+        
+        try:
+            body = {
+                "sourceRevisionId": self.compatible_revisions( ## most recent compatible revision
+                                        source_model = source_model, 
+                                        target_model = target_model,
+                                        workspace = workspace)['revisions'][0]['id'],
+                "sourceModelId": s_model_id,
+                "targetRevisionId": self.latest_revision(target_model, workspace)['revisions'][0]['id'] ## most recent revivsion push
+            }
+            self.api.headers['Content-Type'] = 'application/json'
+            self.resp = requests.post(URL, headers=self.api.headers, json=body)
+            self.api.headers.pop('Content-Type')
+        except Exception as e:
+            print("Error occurred: {0}".format(e))
+            print("Unable to sync source model {0} with target model {1}".format(source_model, target_model))
+            return self.resp.status_code
+
+        if self.resp.status_code in (200, 201):
+            print("Model {0} successfully synced to model {1}".format(source_model, target_model))
+        
+        return self.resp
+    
+    def sync_tasks_list(self, model, workspace):
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        URL = self.api.api_url + "models/{0}/alm/syncTasks".format(model_id)
+        
+        return self.get_request(URL)
+        
+#     def sync_status(self, model):
+#         model_id = self.models[model]['id']
+#         URL = self.api.api_url + "models/{0}/alm/syncTasks"
+        
+    def create_revision(self, model, workspace, rev_name, rev_desc):
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        URL = self.api.api_url + "models/{0}/alm/revisions".format(model_id)
+        
+        try:
+            body = {
+                "name": rev_name,
+                "description": rev_desc
+            }
+            self.api.headers['Content-Type'] = 'application/json'
+            self.resp = requests.post(URL, headers=self.api.headers, json=body)
+            self.api.headers.pop('Content-Type')
+        except Exception as e:
+            print("Error occurred: {0}".format(e))
+            return self.resp.status_code
+        
         return self.resp
```

