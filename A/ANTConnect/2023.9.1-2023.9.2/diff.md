# Comparing `tmp/ANTConnect-2023.9.1.tar.gz` & `tmp/ANTConnect-2023.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ANTConnect-2023.9.1.tar", last modified: Thu Jun  1 08:30:52 2023, max compression
+gzip compressed data, was "dist\ANTConnect-2023.9.2.tar", last modified: Fri Jul 14 07:16:49 2023, max compression
```

## Comparing `ANTConnect-2023.9.1.tar` & `ANTConnect-2023.9.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 08:30:52.989902 ANTConnect-2023.9.1/
-drwxrwxrwx   0        0        0        0 2023-06-01 08:30:52.981921 ANTConnect-2023.9.1/ANTConnect.egg-info/
--rw-rw-rw-   0        0        0     1274 2023-06-01 08:30:52.000000 ANTConnect-2023.9.1/ANTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-06-01 08:30:52.000000 ANTConnect-2023.9.1/ANTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 08:30:52.000000 ANTConnect-2023.9.1/ANTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 08:30:52.000000 ANTConnect-2023.9.1/ANTConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-01 08:30:52.000000 ANTConnect-2023.9.1/ANTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1274 2023-06-01 08:30:52.989902 ANTConnect-2023.9.1/PKG-INFO
--rw-rw-rw-   0        0        0      586 2021-06-28 09:19:30.000000 ANTConnect-2023.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 08:30:52.984914 ANTConnect-2023.9.1/antconnect/
--rw-rw-rw-   0        0        0      144 2023-06-01 08:30:50.000000 ANTConnect-2023.9.1/antconnect/__init__.py
--rw-rw-rw-   0        0        0    50949 2023-06-01 05:52:54.000000 ANTConnect-2023.9.1/antconnect/api.py
--rw-rw-rw-   0        0        0      484 2023-06-01 08:30:52.992409 ANTConnect-2023.9.1/setup.cfg
--rw-rw-rw-   0        0        0      739 2023-06-01 08:30:31.000000 ANTConnect-2023.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:30:52.987906 ANTConnect-2023.9.1/tests/
--rw-rw-rw-   0        0        0        0 2020-12-10 14:04:13.000000 ANTConnect-2023.9.1/tests/__init__.py
--rw-rw-rw-   0        0        0      102 2020-12-10 14:04:13.000000 ANTConnect-2023.9.1/tests/test_ant.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:16:49.864042 ANTConnect-2023.9.2/
+drwxrwxrwx   0        0        0        0 2023-07-14 07:16:49.847091 ANTConnect-2023.9.2/ANTConnect.egg-info/
+-rw-rw-rw-   0        0        0     1017 2023-07-14 07:16:49.000000 ANTConnect-2023.9.2/ANTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-07-14 07:16:49.000000 ANTConnect-2023.9.2/ANTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:16:49.000000 ANTConnect-2023.9.2/ANTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 07:16:49.000000 ANTConnect-2023.9.2/ANTConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-14 07:16:49.000000 ANTConnect-2023.9.2/ANTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2022-12-21 12:12:30.000000 ANTConnect-2023.9.2/LICENSE
+-rw-rw-rw-   0        0        0     1017 2023-07-14 07:16:49.864042 ANTConnect-2023.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2022-12-21 12:12:30.000000 ANTConnect-2023.9.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 07:16:49.857062 ANTConnect-2023.9.2/antconnect/
+-rw-rw-rw-   0        0        0      146 2023-07-14 07:16:48.000000 ANTConnect-2023.9.2/antconnect/__init__.py
+-rw-rw-rw-   0        0        0    51077 2023-07-13 08:53:39.000000 ANTConnect-2023.9.2/antconnect/api.py
+-rw-rw-rw-   0        0        0      485 2023-07-14 07:16:49.870025 ANTConnect-2023.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      739 2023-07-14 07:16:48.000000 ANTConnect-2023.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:16:49.863044 ANTConnect-2023.9.2/tests/
+-rw-rw-rw-   0        0        0        0 2022-12-21 12:12:30.000000 ANTConnect-2023.9.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      102 2022-12-21 12:12:30.000000 ANTConnect-2023.9.2/tests/test_ant.py
```

### Comparing `ANTConnect-2023.9.1/ANTConnect.egg-info/PKG-INFO` & `ANTConnect-2023.9.2/ANTConnect.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: ANTConnect
-Version: 2023.9.1
+Version: 2023.9.2
 Summary: Python SDK for ANT Common Data Engineering
 Home-page: https://antcde.io
 Author: ANT CDE
 Author-email: info@antcde.io
-License: UNKNOWN
-Description: # ANTConnect
-        
-        Provides access to an ANT CDE
-        For more details, visit [docs.antcde.io](https://docs.antcde.io/)
-        
-        ## Release notes
-        
-        ### Version 2021.05.1
-        - Updates Tasks API Calls and includes download files
-        
-        ### Version 2021.04
-        - Adds Tasks API calls to the SDK
-        
-        ### Version 2020.20.5
-        - Adds multiple options in column create and column update
-        
-        ### Version 2020.20.2
-        - Complements update of API on ANTCDE
-        
-        ### Version 2020.18.1
-        - Added more consistancy
-        
-        ### Version 0.1.3
-        - Bugfix
-        
-        ### Version 0.1.2
-        - Bugfix Column Create
-        
-        ### Version 0.1.0
-        - Initial version
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ANTConnect
+
+Provides access to an ANT CDE
+For more details, visit [docs.antcde.io](https://docs.antcde.io/)
+
+## Release notes
+
+### Version 2021.05.1
+- Updates Tasks API Calls and includes download files
+
+### Version 2021.04
+- Adds Tasks API calls to the SDK
+
+### Version 2020.20.5
+- Adds multiple options in column create and column update
+
+### Version 2020.20.2
+- Complements update of API on ANTCDE
+
+### Version 2020.18.1
+- Added more consistancy
+
+### Version 0.1.3
+- Bugfix
+
+### Version 0.1.2
+- Bugfix Column Create
+
+### Version 0.1.0
+- Initial version
```

### Comparing `ANTConnect-2023.9.1/PKG-INFO` & `ANTConnect-2023.9.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: ANTConnect
-Version: 2023.9.1
+Version: 2023.9.2
 Summary: Python SDK for ANT Common Data Engineering
 Home-page: https://antcde.io
 Author: ANT CDE
 Author-email: info@antcde.io
-License: UNKNOWN
-Description: # ANTConnect
-        
-        Provides access to an ANT CDE
-        For more details, visit [docs.antcde.io](https://docs.antcde.io/)
-        
-        ## Release notes
-        
-        ### Version 2021.05.1
-        - Updates Tasks API Calls and includes download files
-        
-        ### Version 2021.04
-        - Adds Tasks API calls to the SDK
-        
-        ### Version 2020.20.5
-        - Adds multiple options in column create and column update
-        
-        ### Version 2020.20.2
-        - Complements update of API on ANTCDE
-        
-        ### Version 2020.18.1
-        - Added more consistancy
-        
-        ### Version 0.1.3
-        - Bugfix
-        
-        ### Version 0.1.2
-        - Bugfix Column Create
-        
-        ### Version 0.1.0
-        - Initial version
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ANTConnect
+
+Provides access to an ANT CDE
+For more details, visit [docs.antcde.io](https://docs.antcde.io/)
+
+## Release notes
+
+### Version 2021.05.1
+- Updates Tasks API Calls and includes download files
+
+### Version 2021.04
+- Adds Tasks API calls to the SDK
+
+### Version 2020.20.5
+- Adds multiple options in column create and column update
+
+### Version 2020.20.2
+- Complements update of API on ANTCDE
+
+### Version 2020.18.1
+- Added more consistancy
+
+### Version 0.1.3
+- Bugfix
+
+### Version 0.1.2
+- Bugfix Column Create
+
+### Version 0.1.0
+- Initial version
```

### Comparing `ANTConnect-2023.9.1/README.md` & `ANTConnect-2023.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ANTConnect-2023.9.1/antconnect/api.py` & `ANTConnect-2023.9.2/antconnect/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,19 @@
         response = self._make_request('oauth/token', 'POST', {
             "grant_type": "password",
             "username": username,
             "password": password,
             "client_id": client_id,
             "client_secret": client_secret
         })
+
         if self._logging:
             print('New login call at {}, returned with code {}'.format(datetime.now(), response.status_code))
         if response.status_code != 200:
-            print("The response was: {}".format(response.status_code))
+            print("The response was: {}".format(response.reason))
             return False
         else:
             parsed_response = response.json()
             # print(parsed_response)
             if 'access_token' not in parsed_response:
                 raise SystemError("Please check credentials")
             now = datetime.now()
@@ -115,15 +116,14 @@
             self._authenticated = False
             self._access_token = ""
             self._refresh_token = ""
             self._expires_at = ""
             return False
 
         if response.status_code == 500:
-            print("Server error raised")
             return False
 
         if response.status_code == 400:
             print("An error occured: {}".format(response.json()['message']))
             return False
 
         # set new time
@@ -275,14 +275,19 @@
     def table_delete(self, project_id: str, table_id: str) -> dict:
         """ Delete a table in a project """
         path = 'table/{}'.format(table_id)
         return self._make_api_request(path, 'DELETE', {
             "project[id]": project_id
         })
 
+    def tables_query(self, project_id: str, queryBody):
+        """ Get all columns in a table """
+        path = 'project/{}/tables/query'.format(project_id)
+        return self._make_api_request(path, 'POST', queryBody)
+
     def columns_read(self, project_id: str, table_id: str):
         """ Get all columns in a table """
         path = 'columns'
         return self._make_api_request(path, 'GET', {
             "project[id]": project_id,
             "table[id]": table_id
         })
@@ -800,27 +805,26 @@
         if user != "":
             filters.append({"column": "assigned_to", "operator": "=", "values": [user]})
         return self._make_api_request(path, 'POST', {
             "advanced_filters": filters
         })
 
     def task_create(self, project_id: str, name: str, description: str, status: str, due_date: str, assigned_user: str,
-                    start_date: str = "", appendix: object = {}, license: str = "", end_date: str = "", priority="normal") -> dict:
+                    start_date: str = "", appendix: object = {}, license: str = "", end_date: str = "") -> dict:
         """ Create a task in a project """
-        path = 'tasks-create'
+        path = 'task-create'
         license = selectLicense(license, self._licenses)
         depreciationMessage("param", "status", "01-02-2023", "taken")
         body = {
             # required
             "license": license,
             "project": project_id,
             "title": name,
             "assigned_to": assigned_user,
             "due": due_date,
-            "priority": priority,
 
             # optional
             "description": description,
             "planned_start": start_date,
             "planned_end": end_date,
         }
         if appendix != {}:
```

### Comparing `ANTConnect-2023.9.1/setup.py` & `ANTConnect-2023.9.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ANTConnect", # Replace with your own username
-    version="2023.9.1",
+    version="2023.9.2",
     author="ANT CDE",
     author_email="info@antcde.io",
     description="Python SDK for ANT Common Data Engineering",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://antcde.io",
     packages=setuptools.find_packages(),
```

