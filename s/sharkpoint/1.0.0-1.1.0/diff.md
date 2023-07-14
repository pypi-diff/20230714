# Comparing `tmp/sharkpoint-1.0.0.tar.gz` & `tmp/sharkpoint-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharkpoint-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sharkpoint-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sharkpoint-1.0.0.tar` & `sharkpoint-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1059 2023-07-12 18:50:32.609034 sharkpoint-1.0.0/LICENSE
--rw-r--r--   0        0        0      508 2023-07-12 19:39:50.014951 sharkpoint-1.0.0/README.md
--rw-r--r--   0        0        0      813 2023-07-12 19:49:08.670314 sharkpoint-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-12 12:40:51.136407 sharkpoint-1.0.0/src/sharkpoint/__init__.py
--rw-r--r--   0        0        0     2740 2023-07-12 15:34:13.069270 sharkpoint-1.0.0/src/sharkpoint/sharepoint.py
--rw-r--r--   0        0        0     2401 2023-07-11 20:41:50.539221 sharkpoint-1.0.0/src/sharkpoint/sharepoint_file.py
--rw-r--r--   0        0        0     6192 2023-07-12 12:36:28.388493 sharkpoint-1.0.0/src/sharkpoint/sharepoint_site.py
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 sharkpoint-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-12 18:50:32.609034 sharkpoint-1.1.0/LICENSE
+-rw-r--r--   0        0        0      508 2023-07-12 19:39:50.014951 sharkpoint-1.1.0/README.md
+-rw-r--r--   0        0        0      966 2023-07-14 15:13:47.576074 sharkpoint-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      456 2023-07-14 15:01:59.270829 sharkpoint-1.1.0/src/sharkpoint/__init__.py
+-rw-r--r--   0        0        0     2832 2023-07-14 15:01:59.312373 sharkpoint-1.1.0/src/sharkpoint/sharepoint.py
+-rw-r--r--   0        0        0     2437 2023-07-14 15:01:59.309381 sharkpoint-1.1.0/src/sharkpoint/sharepoint_file.py
+-rw-r--r--   0        0        0     7810 2023-07-14 15:01:59.383631 sharkpoint-1.1.0/src/sharkpoint/sharepoint_site.py
+-rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 sharkpoint-1.1.0/PKG-INFO
```

### Comparing `sharkpoint-1.0.0/LICENSE` & `sharkpoint-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sharkpoint-1.0.0/pyproject.toml` & `sharkpoint-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sharkpoint"
-version = "1.0.0"
+version = "1.1.0"
 description = "A small Pythonic library for interacting with SharePoint document libraries"
 authors = [
   { name = "TheOtherOne" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
@@ -23,7 +23,18 @@
   "requests >=2.6",
   "azure-identity",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ThatsItForTheOtherOne/sharkpoint"
 "Bug Tracker" = "https://github.com/ThatsItForTheOtherOne/sharkpoint/issues"
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+addopts = "-ra -q"
+testpaths = [
+    "tests",
+]
+pythonpath = [
+  "src"
+]
+env_files = ".env_tests"
```

### Comparing `sharkpoint-1.0.0/src/sharkpoint/sharepoint.py` & `sharkpoint-1.1.0/src/sharkpoint/sharepoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import azure.identity
 import requests
 import json
-import sharepoint_site
+from . import sharepoint_site
 import azure.core.credentials
 
+
 class SharePoint:
     """
-    A class used to represent an organization's SharePoint instance using the SharePoint REST API v1. 
+    A class used to represent an organization's SharePoint instance using the SharePoint REST API v1.
     ...
-    
+
     Parameters
     ----------
     base_url : str
         The URL of a Sharepoint instance, ex. contoso.sharepoint.com
-    azure_identity : TokenCredential 
+    azure_identity : TokenCredential
         An azure-identity token credential.
 
     Attributes
     ----------
     sites : dict
         a dictionary of all sites in SharePoint, the key is the user-facing name and the value is the URL
     base_url : str
@@ -25,15 +26,19 @@
 
     Methods
     -------
     get_site(site_name)
         Returns a SharepointSite object for a specific SharePoint site
     """
 
-    def __init__(self, sharepoint_url: str, azure_identity: azure.core.credentials.TokenCredential) -> None:
+    def __init__(
+        self,
+        sharepoint_url: str,
+        azure_identity: azure.core.credentials.TokenCredential,
+    ) -> None:
         self.base_url = sharepoint_url
         self._scope = f"{self.base_url}/.default"
         self._identity = azure_identity
         self.sites = self._initalize_sites()
 
     @property
     def _token(self):
@@ -50,15 +55,15 @@
     def _initalize_sites(self):
         api_url = f"{self.base_url}/_api/search/query?querytext='contentclass:STS_Site contentclass:STS_Web'&selectproperties='Title,Path'"
         request = requests.get(api_url, headers=self._header).text
         request = json.loads(request)
         # fmt: off
         request = request["d"]["query"]["PrimaryQueryResult"]["RelevantResults"]["Table"]["Rows"]["results"]
         # fmt: on
-        
+
         sites = []
         for x in request:
             site_dict = {
                 "Site Name": x["Cells"]["results"][0]["Value"],
                 "Site Path": x["Cells"]["results"][1]["Value"],
             }
             sites.append(site_dict)
@@ -66,19 +71,23 @@
 
     def get_site(self, site_name):
         """
         Parameters
         ----------
         site_name : str
             The user-facing name of a SharePoint site
+
+        Raises
+        ------
+        KeyError
+            If the subsite does not exist
+
         """
 
         site_url = next(
             (item for item in self.sites if item["Site Name"] == site_name), None
         )
         if site_url is None:
             raise KeyError("Site not found.")
         else:
             site_url = site_url["Site Path"]
-        return sharepoint_site.SharepointSite(
-            site_name, site_url, self.base_url, self._header
-        )
+        return sharepoint_site.SharepointSite(site_url, self.base_url, self._header)
```

### Comparing `sharkpoint-1.0.0/src/sharkpoint/sharepoint_file.py` & `sharkpoint-1.1.0/src/sharkpoint/sharepoint_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
     Methods
     -------
     check_back_in()
         Manually check a file into SharePoint and remove the file lock
     """
 
-
     def __init__(self, header, sharepoint_site: str, filepath: str, checkout: bool):
         self._header = header
         self._site = sharepoint_site
         self._path, self._filename = self._get_filepath(filepath)
         self._checkout = checkout
         super().__init__(self._get_file())
 
@@ -46,21 +45,25 @@
             "Content-Length": str(file_size),
             "X-HTTP-Method": "PUT",
         }
 
         post_request.update(self._header)
         file_content = super().getvalue()
         requests.put(api_url, data=file_content, headers=post_request)
-    
+
     def check_back_in(self):
         if self._checkout:
             api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files('{self._filename}')/CheckIn(comment='Comment',checkintype=0)"
             requests.post(api_url, headers=self._header)
 
     def close(self) -> None:
         self.check_back_in()
         return super().close()
 
-    def __exit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
+    def __exit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
         self.check_back_in()
         return super().__exit__(exc_type, exc_val, exc_tb)
-
```

### Comparing `sharkpoint-1.0.0/src/sharkpoint/sharepoint_site.py` & `sharkpoint-1.1.0/src/sharkpoint/sharepoint_site.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 import json
 import requests
-import sharepoint_file
+from . import sharepoint_file
 
 
 class SharepointSite:
     """
     SharePointSite(sharepoint_site_name, sharepoint_site_url, sharepoint_base_url, header)
 
-    A class used to represent a SharePoint site using the SharePoint REST API v1. 
+    A class used to represent a SharePoint site using the SharePoint REST API v1.
     ...
-    
+
     Parameters
     ----------
-    sharepoint_site_name : str
-        The user-facing name of the Sharepoint site
-    sharepoint_site_url : str 
+    sharepoint_site_url : str
         The URL of the Sharepoint site
     sharepoint_base_url : str
         The URL of the Sharepoint instance
     header : dict
         The header for requests made to the API containing the Bearer token
-    
+
     Attributes
     ----------
     site_name : str
         The user-facing name of the Sharepoint site
+    description : str
+        The description of the Sharepoint site
+    subsites : dict
+        A list of dicts of Sharepoint subsites
 
     Methods
     -------
     listdir(path)
         Returns a list of directories in a document library
     mkdir(path)
         Creates a new directory in a document library
     open(path, checkout = False)
         Downloads a file from a document library and returns a SharepointFile object
+    get_subsite(site_name)
+        Returns a SharepointSite object for a subsite
     """
 
     def __init__(
         self,
-        sharepoint_site_name: str,
         sharepoint_site_url: str,
         sharepoint_base_url: str,
         header,
     ) -> None:
-        self.site_name = sharepoint_site_name
         self._site_url = sharepoint_site_url
         self._base_url = sharepoint_base_url
         self._header = header
         self._libraries = self._get_libraries()
 
     def _get_libraries(self):
         api_url = f"{self._site_url}/_api/web/lists?$select=Title,ServerRelativeUrl&$filter=BaseTemplate eq 101 and hidden eq false&$expand=RootFolder"
@@ -126,18 +128,18 @@
         """
 
         path_list = path.split("/")
         path_list = list(filter(None, path_list))
 
         if path_list[0] not in self._libraries:
             raise FileNotFoundError(f"Document Library {path_list[0]} not found.")
-        
+
         if path_list[-1] in self.listdir("/".join(path_list[:-1])):
             raise FileExistsError(f"Folder {path_list[-1]} exists.")
-        
+
         api_url = f"{self._site_url}/_api/web/folders"
         payload = json.dumps(
             {
                 "__metadata": {"type": "SP.Folder"},
                 "ServerRelativeUrl": "/".join(path_list),
             }
         )
@@ -169,7 +171,57 @@
 
         return sharepoint_file.SharepointFile(
             header=self._header,
             sharepoint_site=self._site_url,
             filepath=filepath,
             checkout=checkout,
         )
+
+    @property
+    def site_name(self):
+        api_url = f"{self._site_url}/_api/web/title"
+        request = json.loads(requests.get(api_url, headers=self._header).content)
+        return request["d"]["Title"]
+
+    @property
+    def description(self):
+        api_url = f"{self._site_url}/_api/web/description"
+        request = json.loads(requests.get(api_url, headers=self._header).content)
+        return request["d"]["Description"]
+
+    @property
+    def subsites(self):
+        api_url = f"{self._site_url}/_api/web/webs/?$select=title,Url"
+        request = requests.get(api_url, headers=self._header).text
+        request = json.loads(request)
+        request = request["d"]["results"]
+        sites = []
+        for x in request:
+            site_dict = {
+                "Site Name": x["Title"],
+                "Site Path": x["Url"],
+            }
+            sites.append(site_dict)
+        return sites
+
+    def get_subsite(self, site_name: str):
+        """Grab a subsite,
+
+        Parameters
+        ----------
+        site_name : str
+            The user-facing name of a SharePoint subsite
+
+        Raises
+        ------
+        KeyError
+            If the subsite does not exist.
+        """
+
+        site_url = next(
+            (item for item in self.sites if item["Site Name"] == site_name), None
+        )
+        if site_url is None:
+            raise KeyError("Site not found.")
+        else:
+            site_url = site_url["Site Path"]
+        return SharepointSite(site_url, self.base_url, self._header)
```

### Comparing `sharkpoint-1.0.0/PKG-INFO` & `sharkpoint-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharkpoint
-Version: 1.0.0
+Version: 1.1.0
 Summary: A small Pythonic library for interacting with SharePoint document libraries
 Author: TheOtherOne
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

