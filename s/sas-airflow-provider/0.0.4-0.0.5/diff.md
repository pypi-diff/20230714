# Comparing `tmp/sas-airflow-provider-0.0.4.tar.gz` & `tmp/sas-airflow-provider-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sas-airflow-provider/sas-airflow-provider/dist/.tmp-d73ucuww/sas-airflow-provider-0.0.4.tar", last modified: Fri Jun  9 18:46:37 2023, max compression
+gzip compressed data, was "/home/runner/work/sas-airflow-provider/sas-airflow-provider/dist/.tmp-9djbkkx6/sas-airflow-provider-0.0.5.tar", last modified: Fri Jul 14 19:48:01 2023, max compression
```

## Comparing `sas-airflow-provider-0.0.4.tar` & `sas-airflow-provider-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/example_sas_studioflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/example_templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/hooks/sas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/operators/sas_jobexecution.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/operators/sas_studioflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/util/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-09 18:46:22.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 18:46:37.000000 sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_sas_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_studio_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/hooks/sas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_create_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_jobexecution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12575 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_studioflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-07-14 19:47:47.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-14 19:48:01.000000 sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/top_level.txt
```

### Comparing `sas-airflow-provider-0.0.4/LICENSE` & `sas-airflow-provider-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.4/PKG-INFO` & `sas-airflow-provider-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sas-airflow-provider
-Version: 0.0.4
+Version: 0.0.5
 Summary: Enables execution of Studio Flows and Jobs from Airflow
 Home-page: https://github.com/sassoftware/sas-airflow-provider
 Author: SAS
 Author-email: andrew.shakinovsky@sas.com
 Project-URL: Bug Tracker, https://github.com/sassoftware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -45,14 +45,16 @@
 #### Installing in a container
 There are a few ways to provide the package:
 - Environment variable: ```_PIP_ADDITIONAL_REQUIREMENTS``` Set this variable to the command line that will be passed to ```pip install```
 - Create a dockerfile that adds the pip install command to the base image and edit the docker-compose file to use "build" (there is a comment in the docker compose file where you can change it)
 
 ### Create a connection to SAS
 In order to connect to SAS Viya from the Airflow operator, you will need to create a connection. The easiest way to do this is to go into the Airflow UI under Admin/Connections and create a new connection using the blue + button. Select SAS from the list of connection types, and enter sas_default as the name. The applicable fields are host (http or https url to your SAS Viya install), login and password. It is also possible to specify an OAuth token by creating a json body in the extra field. For example `{"token": "oauth_token_here"}`. If a token is found it is used instead of the user/password.
+Please be aware of security considerations when storing sensitive information in a
+connection. Consult https://airflow.apache.org/docs/apache-airflow/stable/security/index.html for details.
 
 ### Running a DAG with a SAS provider
 See example files in the src/sas_airflow_provider/example_dags directory. These dags can be modified and 
 placed in your Airflow dags directory. 
 
 Mac note: If you are running Airflow standalone on a Mac, there is a known issue regarding how process forking works.
 This causes issues with the urllib which is used by the operator. To get around it set NO_PROXY=* in your environment
```

### Comparing `sas-airflow-provider-0.0.4/README.md` & `sas-airflow-provider-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 #### Installing in a container
 There are a few ways to provide the package:
 - Environment variable: ```_PIP_ADDITIONAL_REQUIREMENTS``` Set this variable to the command line that will be passed to ```pip install```
 - Create a dockerfile that adds the pip install command to the base image and edit the docker-compose file to use "build" (there is a comment in the docker compose file where you can change it)
 
 ### Create a connection to SAS
 In order to connect to SAS Viya from the Airflow operator, you will need to create a connection. The easiest way to do this is to go into the Airflow UI under Admin/Connections and create a new connection using the blue + button. Select SAS from the list of connection types, and enter sas_default as the name. The applicable fields are host (http or https url to your SAS Viya install), login and password. It is also possible to specify an OAuth token by creating a json body in the extra field. For example `{"token": "oauth_token_here"}`. If a token is found it is used instead of the user/password.
+Please be aware of security considerations when storing sensitive information in a
+connection. Consult https://airflow.apache.org/docs/apache-airflow/stable/security/index.html for details.
 
 ### Running a DAG with a SAS provider
 See example files in the src/sas_airflow_provider/example_dags directory. These dags can be modified and 
 placed in your Airflow dags directory. 
 
 Mac note: If you are running Airflow standalone on a Mac, there is a known issue regarding how process forking works.
 This causes issues with the urllib which is used by the operator. To get around it set NO_PROXY=* in your environment
```

### Comparing `sas-airflow-provider-0.0.4/setup.cfg` & `sas-airflow-provider-0.0.5/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sas-airflow-provider
-version = 0.0.4
+version = 0.0.5
 author = SAS
 author_email = andrew.shakinovsky@sas.com
 description = Enables execution of Studio Flows and Jobs from Airflow
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sassoftware/sas-airflow-provider
 project_urls =
```

### Comparing `sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/__init__.py` & `sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py` & `sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_sas_jobexecution.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/example_sas_studioflow.py` & `sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_sas_studio.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from datetime import datetime
 from airflow import DAG
-from sas_airflow_provider.operators.sas_studioflow import SASStudioFlowOperator
+from sas_airflow_provider.operators.sas_studio import SASStudioOperator
 
 dag = DAG('demo_studio_flow_1', description='Executing Studio Flow for demo purposes',
           schedule_interval='0 12 * * *',
           start_date=datetime(2022, 6, 1), catchup=False)
 
 environment_vars = {
     "env1": "val1",
     "env2": "val2"
 }
 
-task1 = SASStudioFlowOperator(task_id='demo_studio_flow_1.flw',
-                              flow_path_type='content',
-                              flow_path='/Public/Airflow/demo_studio_flow_1.flw',
-                              flow_exec_log=True,
+task1 = SASStudioOperator(task_id='demo_studio_flow_1.flw',
+                              path_type='content',
+                              path='/Public/Airflow/demo_studio_flow_1.flw',
+                              exec_log=True,
                               compute_context="SAS Studio compute context",
-                              flow_codegen_init_code=False,
-                              flow_codegen_wrap_code=False,
+                              codegen_init_code=False,
+                              codegen_wrap_code=False,
                               connection_name='sas_default',
                               env_vars=environment_vars,
                               dag=dag)
```

### Comparing `sas-airflow-provider-0.0.4/src/sas_airflow_provider/example_dags/example_templating.py` & `sas-airflow-provider-0.0.5/src/sas_airflow_provider/example_dags/example_templating.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.4/src/sas_airflow_provider/hooks/__init__.py` & `sas-airflow-provider-0.0.5/src/sas_airflow_provider/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.4/src/sas_airflow_provider/hooks/sas.py` & `sas-airflow-provider-0.0.5/src/sas_airflow_provider/hooks/sas.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.4/src/sas_airflow_provider/operators/__init__.py` & `sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.4/src/sas_airflow_provider/operators/sas_jobexecution.py` & `sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_jobexecution.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,25 +21,20 @@
 import urllib.parse
 
 from airflow.exceptions import AirflowFailException
 from airflow.models import BaseOperator
 from sas_airflow_provider.hooks.sas import SasHook
 from sas_airflow_provider.util.util import dump_logs
 
-JES_URI = "/jobExecution"
-JOB_URI = f"{JES_URI}/jobs"
-
-
 class SASJobExecutionOperator(BaseOperator):
     """
-    Executes a SAS Job
-
-    .. seealso::
-        For more information on how to use this operator, take a look at the guide:
-        :ref:`howto/operator:SASJobExecutionOperator`
+    Executes a SAS Job using /SASJobExecution endpoint. Job execution is documented here:
+    https://go.documentation.sas.com/doc/en/pgmsascdc/default/jobexecug/p1ct9uzl5c7omun1t2zy0gxhlqlc.htm
+    The specific endpoint /SASJobExecution is documented here:
+    https://go.documentation.sas.com/doc/en/pgmsascdc/default/jobexecug/n06tcybrt9wdeun1ko9bkjn0ko0b.htm
 
     :param connection_name: Name of the SAS Viya connection stored as an Airflow HTTP connection
     :param job_name: Name of the SAS Job to be run
     :param parameters Dictionary of all the parameters that should be passed to the
         SAS Job as SAS Macro variables
     :param job_exec_log: boolean. whether or not to dump out the log
     """
@@ -65,16 +60,14 @@
         print(f"Executing SAS job: {self.job_name}")
         # url escape the program name
         program_name = urllib.parse.quote(self.job_name)
         url_string = ""
         for key, value in self.parameters.items():
             url_string += f"&{key}={urllib.parse.quote(value)}"
 
-        # this endpoint is documented here:
-        # https://go.documentation.sas.com/doc/en/pgmsascdc/9.4_3.5/jobexecug/p1ct9uzl5c7omun1t2zy0gxhlqlc.htm
         url = f"/SASJobExecution/?_program={program_name}{url_string}"
 
         headers = {"Accept": "application/vnd.sas.job.execution.job+json"}
         response = session.post(url, headers=headers, verify=False)
 
         if response.status_code < 200 or response.status_code >= 300:
             raise AirflowFailException(f"SAS Job Execution HTTP status code {response.status_code}")
```

### Comparing `sas-airflow-provider-0.0.4/src/sas_airflow_provider/operators/sas_studioflow.py` & `sas-airflow-provider-0.0.5/src/sas_airflow_provider/operators/sas_studioflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,30 +16,29 @@
 # under the License.
 
 from __future__ import annotations
 
 import copy
 import json
 import time
+import warnings
 
 import requests
 
 from airflow.exceptions import AirflowFailException
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from sas_airflow_provider.hooks.sas import SasHook
 from sas_airflow_provider.util.util import dump_logs
 
+
 class SASStudioFlowOperator(BaseOperator):
     """
-    Executes a SAS Studio flow
-
-    .. seealso::
-        For more information on how to use this operator, take a look at the guide:
-        :ref:`howto/operator:SASStudioFlowOperator`
+    Executes a SAS Studio flow.
+    Note that this operator is deprecated. Please use SASStudioOperator instead
 
     :param flow_path_type: valid values are content or compute
     :param flow_path: path to the flow to execute. eg /Public/myflow.flw
     :param flow_exec_log: whether or not to output the execution log
     :param flow_codegen_init_code: Whether or not to generate init code
         (default value: False)
     :param flow_codegen_wrap_code: Whether or not to generate wrapper code
@@ -53,27 +52,28 @@
 
     ui_color = "#CCE5FF"
     ui_fgcolor = "black"
 
     template_fields: Sequence[str] = ("env_vars",)
 
     def __init__(
-        self,
-        flow_path_type: str,
-        flow_path: str,
-        flow_exec_log: bool,
-        flow_codegen_init_code=False,
-        flow_codegen_wrap_code=False,
-        connection_name=None,
-        compute_context="SAS Studio compute context",
-        env_vars=None,
-        **kwargs,
+            self,
+            flow_path_type: str,
+            flow_path: str,
+            flow_exec_log: bool,
+            flow_codegen_init_code=False,
+            flow_codegen_wrap_code=False,
+            connection_name=None,
+            compute_context="SAS Studio compute context",
+            env_vars=None,
+            **kwargs,
     ) -> None:
 
         super().__init__(**kwargs)
+        warnings.warn("SASStudioFlowOperator is deprecated. Please use SASStudioOperator instead.")
         if env_vars is None:
             env_vars = {}
         self.flow_path_type = flow_path_type
         self.flow_path = flow_path
         self.flow_exec_log = flow_exec_log
         self.flow_codegen_initCode = flow_codegen_init_code
         self.flow_codegen_wrapCode = flow_codegen_wrap_code
@@ -143,21 +143,21 @@
         if job_state == "timed out":
             raise AirflowException("SAS Studio Flow Execution has timed out. See log for details ")
 
         return 1
 
 
 def _generate_flow_code(
-    session,
-    artifact_type: str,
-    path: str,
-    init_code: bool,
-    wrap_code: bool,
-    session_id=None,
-    compute_context="SAS Studio compute context",
+        session,
+        artifact_type: str,
+        path: str,
+        init_code: bool,
+        wrap_code: bool,
+        session_id=None,
+        compute_context="SAS Studio compute context",
 ):
     # main API URI for Code Gen
     uri_base = "/studioDevelopment/code"
 
     # if type == compute then Compute session should be created
     if artifact_type == "compute":
         print("Code Generation for Studio Flow with Compute session")
@@ -237,17 +237,14 @@
 
     if response.status_code != 201:
         raise RuntimeError(f"Failed to create session: {response.text}")
 
     return response.json()
 
 
-
-
-
 JES_URI = "/jobExecution"
 JOB_URI = f"{JES_URI}/jobs"
 
 
 def _run_job_and_wait(session, job_request: dict, poll_interval: int) -> dict:
     uri = JOB_URI
     response = session.post(uri, json=job_request)
@@ -265,9 +262,7 @@
         response = session.get(uri)
         if response.status_code != 200:
             raise RuntimeError(f"Failed to get job: {response.text}")
         job = response.json()
         state = job["state"]
     print("Job request has completed execution with the status: " + str(state))
     return job
-
-
```

### Comparing `sas-airflow-provider-0.0.4/src/sas_airflow_provider/util/__init__.py` & `sas-airflow-provider-0.0.5/src/sas_airflow_provider/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/PKG-INFO` & `sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sas-airflow-provider
-Version: 0.0.4
+Version: 0.0.5
 Summary: Enables execution of Studio Flows and Jobs from Airflow
 Home-page: https://github.com/sassoftware/sas-airflow-provider
 Author: SAS
 Author-email: andrew.shakinovsky@sas.com
 Project-URL: Bug Tracker, https://github.com/sassoftware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -45,14 +45,16 @@
 #### Installing in a container
 There are a few ways to provide the package:
 - Environment variable: ```_PIP_ADDITIONAL_REQUIREMENTS``` Set this variable to the command line that will be passed to ```pip install```
 - Create a dockerfile that adds the pip install command to the base image and edit the docker-compose file to use "build" (there is a comment in the docker compose file where you can change it)
 
 ### Create a connection to SAS
 In order to connect to SAS Viya from the Airflow operator, you will need to create a connection. The easiest way to do this is to go into the Airflow UI under Admin/Connections and create a new connection using the blue + button. Select SAS from the list of connection types, and enter sas_default as the name. The applicable fields are host (http or https url to your SAS Viya install), login and password. It is also possible to specify an OAuth token by creating a json body in the extra field. For example `{"token": "oauth_token_here"}`. If a token is found it is used instead of the user/password.
+Please be aware of security considerations when storing sensitive information in a
+connection. Consult https://airflow.apache.org/docs/apache-airflow/stable/security/index.html for details.
 
 ### Running a DAG with a SAS provider
 See example files in the src/sas_airflow_provider/example_dags directory. These dags can be modified and 
 placed in your Airflow dags directory. 
 
 Mac note: If you are running Airflow standalone on a Mac, there is a known issue regarding how process forking works.
 This causes issues with the urllib which is used by the operator. To get around it set NO_PROXY=* in your environment
```

### Comparing `sas-airflow-provider-0.0.4/src/sas_airflow_provider.egg-info/SOURCES.txt` & `sas-airflow-provider-0.0.5/src/sas_airflow_provider.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 src/sas_airflow_provider.egg-info/PKG-INFO
 src/sas_airflow_provider.egg-info/SOURCES.txt
 src/sas_airflow_provider.egg-info/dependency_links.txt
 src/sas_airflow_provider.egg-info/entry_points.txt
 src/sas_airflow_provider.egg-info/top_level.txt
 src/sas_airflow_provider/example_dags/__init__.py
 src/sas_airflow_provider/example_dags/example_sas_jobexecution.py
-src/sas_airflow_provider/example_dags/example_sas_studioflow.py
+src/sas_airflow_provider/example_dags/example_sas_studio.py
+src/sas_airflow_provider/example_dags/example_studio_advanced.py
 src/sas_airflow_provider/example_dags/example_templating.py
 src/sas_airflow_provider/hooks/__init__.py
 src/sas_airflow_provider/hooks/sas.py
 src/sas_airflow_provider/operators/__init__.py
+src/sas_airflow_provider/operators/sas_create_session.py
 src/sas_airflow_provider/operators/sas_jobexecution.py
+src/sas_airflow_provider/operators/sas_studio.py
 src/sas_airflow_provider/operators/sas_studioflow.py
 src/sas_airflow_provider/util/__init__.py
 src/sas_airflow_provider/util/util.py
```

