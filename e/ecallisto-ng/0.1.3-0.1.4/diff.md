# Comparing `tmp/ecallisto_ng-0.1.3.tar.gz` & `tmp/ecallisto_ng-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.1.3.tar", last modified: Thu Jul 13 18:04:42 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.1.4.tar", last modified: Fri Jul 14 19:02:46 2023, max compression
```

## Comparing `ecallisto_ng-0.1.3.tar` & `ecallisto_ng-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.362043 ecallisto_ng-0.1.3/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.1.3/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-13 18:04:42.362043 ecallisto_ng-0.1.3/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2967 2023-07-11 14:51:23.000000 ecallisto_ng-0.1.3/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      836 2023-07-13 18:04:24.000000 ecallisto_ng-0.1.3/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-13 18:04:42.362043 ecallisto_ng-0.1.3/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.340377 ecallisto_ng-0.1.3/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.351210 ecallisto_ng-0.1.3/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.351210 ecallisto_ng-0.1.3/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/data_fetching/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     6471 2023-07-13 18:03:37.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/data_fetching/get_data.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2006 2023-07-13 17:59:20.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/data_fetching/get_information.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.362043 ecallisto_ng-0.1.3/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/data_processing/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.362043 ecallisto_ng-0.1.3/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/plotting/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.1.3/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 18:04:42.351210 ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-13 18:04:42.000000 ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-13 18:04:42.000000 ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-13 18:04:42.000000 ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      113 2023-07-13 18:04:42.000000 ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-13 18:04:42.000000 ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.1.4/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2967 2023-07-11 14:51:23.000000 ecallisto_ng-0.1.4/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-14 19:02:25.000000 ecallisto_ng-0.1.4/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.860868 ecallisto_ng-0.1.4/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.860868 ecallisto_ng-0.1.4/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/data_fetching/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     6006 2023-07-14 19:01:04.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/data_fetching/get_data.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2006 2023-07-13 17:59:20.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/data_fetching/get_information.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/data_processing/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/plotting/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.1.4/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-14 19:02:46.870868 ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3548 2023-07-14 19:02:46.000000 ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-14 19:02:46.000000 ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-14 19:02:46.000000 ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-14 19:02:46.000000 ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-14 19:02:46.000000 ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.1.3/LICENSE` & `ecallisto_ng-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.3/PKG-INFO` & `ecallisto_ng-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto_ng
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.1.3/README.md` & `ecallisto_ng-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.3/pyproject.toml` & `ecallisto_ng-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
@@ -16,14 +16,15 @@
     'ipython>=8.14.0',
     'nbformat>=5.9.0',
     'numpy>=1.25.0',
     'pandas>=2.0.3',
     'plotly>=5.15.0',
     'requests>=2.31.0',
     'scikit-image>=0.21.0',
+    'pyarrow>=12.0.1'
 
 ]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `ecallisto_ng-0.1.3/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.1.4/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 
 
 def get_data(
     instrument_name,
     start_datetime,
     end_datetime,
     timebucket=None,
-    agg_function=None,
-    return_type="json",
-    verbose=False,
+    agg_function=None
 ):
     """
     Get data from the eCallisto API. See: https://v000792.fhnw.ch/api/redoc
     Of course, this is just a wrapper around the requests.post function.
     Depending on the size, the request can take a while. For example, two
     weeks of data, aggregated in a specific way, can take around 20 seconds.
 
@@ -31,74 +29,63 @@
     end_datetime : str
         The end datetime of the data to get.
     timebucket : str
         In what time frame the data should be grouped (see timescaledb
         "timebucket" function)
     agg_function : str
         The aggregation function to use (see timescaledb "timebucket" function)
-    return_type : str
-        The type of data to return. Either 'json' or 'fits'. If 'json', the
-        data is returned as a pandas DataFrame. If 'fits', the data is
-        downloaded as a fits file and the filename is returned.
     verbose : bool
         Whether to print out the response from the API.
     Returns
     -------
     pandas.DataFrame
         A DataFrame containing the data from the eCallisto API.
     """
     data = {
         "instrument_name": instrument_name,
         "start_datetime": start_datetime,
         "end_datetime": end_datetime,
         "timebucket": timebucket,
-        "agg_function": agg_function,
-        "return_type": return_type,
+        "agg_function": agg_function
     }
 
     assert pd.to_datetime(start_datetime) <= pd.to_datetime(end_datetime), (
         f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
     )
 
+    file_path = f"{instrument_name}_{start_datetime}_{end_datetime}_{timebucket}_{agg_function}.parquet"
+    if os.path.exists(file_path):
+        print(f"Reading data from {file_path}")
+        return pd.read_parquet(file_path)
     response = requests.post(BASE_URL + "/api/data", json=data, timeout=180)
 
+    # Check if the request was successful
     if response.status_code == 200:
-        url = (
-            response.json()["json_url"]
-            if return_type == "json"
-            else response.json()["fits_url"]
-        )
-        url = BASE_URL + url
+        # Get the URL for the parquet file
+        parquet_url = response.json()["data_parquet_url"]
+
+        # Now we can start polling the URL until the parquet file is ready for download
         while True:
-            # Sleep for a short period of time to allow the data to be fetched
-            time.sleep(5)
-            # Check if the file is available yet
-            file_response = requests.get(url)
+            # Try to download the parquet file
+            file_response = requests.get(BASE_URL + parquet_url)
+            
+            # If the file is available, save it to disk
             if file_response.status_code == 200:
-                # If the file is available, return the data
-                respone_json = file_response.json()
-                if 'error' in respone_json.keys():
-                    raise ValueError(respone_json['error'])
-                if return_type == "json":
-                    df = pd.DataFrame(file_response.json())
-                    return df
-                else:
-                    fits_path = (
-                        f"{instrument_name}_{start_datetime}_{end_datetime}.fits"
-                    )
-                    with open(fits_path, "wb") as f:
-                        f.write(file_response.content)
-                    return fits_path
+                with open(file_path, "wb") as f:
+                    f.write(file_response.content)
+                return pd.read_parquet(file_path)
             elif file_response.status_code == 404:
-                # If the file is not found, continue waiting
-                continue
+                # If the file is not found, sleep for a short period and try again
+                print("File not ready yet, waiting...")
+                time.sleep(5)
             else:
-                raise ValueError(f"Error getting file from API: {file_response.text}")
+                print(f"Error downloading file: {file_response.status_code}")
+                break
     else:
-        raise ValueError(f"Error getting data from API: {response.text}")
+        print(f"Error starting data retrieval: {response.status_code}")
 
 
 # Because of SQL limitation, the names of the tables do not perfectly match the instrument names.
 # This function converts the instrument name to the table name.
 def extract_instrument_name(file_path):
     """
     Because of SQL limitation, the names of the tables do not perfectly match the instrument names.
```

### Comparing `ecallisto_ng-0.1.3/src/ecallisto_ng/data_fetching/get_information.py` & `ecallisto_ng-0.1.4/src/ecallisto_ng/data_fetching/get_information.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.3/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.1.4/src/ecallisto_ng/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.3/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.1.4/src/ecallisto_ng/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto-ng
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.1.3/src/ecallisto_ng.egg-info/SOURCES.txt` & `ecallisto_ng-0.1.4/src/ecallisto_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

