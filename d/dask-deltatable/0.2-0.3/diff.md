# Comparing `tmp/dask-deltatable-0.2.tar.gz` & `tmp/dask-deltatable-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-deltatable-0.2.tar", last modified: Thu Oct 14 07:22:51 2021, max compression
+gzip compressed data, was "dask-deltatable-0.3.tar", last modified: Fri Jul 14 12:40:13 2023, max compression
```

## Comparing `dask-deltatable-0.2.tar` & `dask-deltatable-0.3.tar`

### file list

```diff
@@ -1,15 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 07:22:51.005545 dask-deltatable-0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2021-10-14 07:22:51.005545 dask-deltatable-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1315 2021-10-14 07:21:55.000000 dask-deltatable-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 07:22:51.005545 dask-deltatable-0.2/dask_deltatable/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-10-14 07:21:55.000000 dask-deltatable-0.2/dask_deltatable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9448 2021-10-14 07:21:55.000000 dask-deltatable-0.2/dask_deltatable/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-14 07:22:51.005545 dask-deltatable-0.2/dask_deltatable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2021-10-14 07:22:50.000000 dask-deltatable-0.2/dask_deltatable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      312 2021-10-14 07:22:50.000000 dask-deltatable-0.2/dask_deltatable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-14 07:22:50.000000 dask-deltatable-0.2/dask_deltatable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-14 07:22:50.000000 dask-deltatable-0.2/dask_deltatable.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-10-14 07:22:50.000000 dask-deltatable-0.2/dask_deltatable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-10-14 07:22:50.000000 dask-deltatable-0.2/dask_deltatable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-14 07:22:51.005545 dask-deltatable-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      687 2021-10-14 07:21:55.000000 dask-deltatable-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:13.605814 dask-deltatable-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-14 12:39:27.000000 dask-deltatable-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 12:39:27.000000 dask-deltatable-0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-14 12:40:13.605814 dask-deltatable-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-14 12:39:27.000000 dask-deltatable-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:13.601814 dask-deltatable-0.3/dask_deltatable/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13508 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-14 12:39:27.000000 dask-deltatable-0.3/dask_deltatable/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:13.605814 dask-deltatable-0.3/dask_deltatable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-14 12:40:13.000000 dask-deltatable-0.3/dask_deltatable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-14 12:40:13.000000 dask-deltatable-0.3/dask_deltatable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:40:13.000000 dask-deltatable-0.3/dask_deltatable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:40:13.000000 dask-deltatable-0.3/dask_deltatable.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-14 12:40:13.000000 dask-deltatable-0.3/dask_deltatable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 12:40:13.000000 dask-deltatable-0.3/dask_deltatable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-14 12:39:27.000000 dask-deltatable-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 12:39:27.000000 dask-deltatable-0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:40:13.605814 dask-deltatable-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-14 12:39:27.000000 dask-deltatable-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:40:13.605814 dask-deltatable-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-14 12:39:27.000000 dask-deltatable-0.3/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-07-14 12:39:27.000000 dask-deltatable-0.3/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-14 12:39:27.000000 dask-deltatable-0.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-14 12:39:27.000000 dask-deltatable-0.3/tests/test_write.py
```

### Comparing `dask-deltatable-0.2/PKG-INFO` & `dask-deltatable-0.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,84 @@
-Metadata-Version: 2.1
-Name: dask-deltatable
-Version: 0.2
-Summary: Dask + Delta Table 
-Home-page: UNKNOWN
-Maintainer: rajagurunath
-Maintainer-email: gurunathrajagopal@gmail.com
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+## Dask-DeltaTable
 
-## Dask Deltatable Reader
+Reading and writing to Delta Lake using Dask engine.
 
-Reads a Delta Table from directory using Dask engine.
+### Installation
 
-To Try out the package:
+To install the package:
 
 ```
 pip install dask-deltatable
 ```
 
 ### Features:
-1. Reads the parquet files based on delta logs parallely using dask engine
-2. Supports all three filesystem like s3, azurefs, gcsfs
-3. Supports some delta features like
+
+1. Read the parquet files from Delta Lake and parallelize with Dask
+2. Write Dask dataframes to Delta Lake (limited support)
+3. Supports multiple filesystems (s3, azurefs, gcsfs)
+4. Subset of Delta Lake features:
    - Time Travel
    - Schema evolution
-   - parquet filters
+   - Parquet filters
      - row filter
      - partition filter
-4. Query Delta commit info - History
-5. vacuum the old/ unused parquet files
-6. load different versions of data using datetime.
 
-### Usage:
+### Not supported
 
-```
+1. Writing to Delta Lake is still in development.
+2. `optimize` API to run a bin-packing operation on a Delta Table.
+
+### Reading from Delta Lake
+
+```python
 import dask_deltatable as ddt
 
 # read delta table
-ddt.read_delta_table("delta_path")
+ddt.read_deltalake("delta_path")
 
-# read delta table for specific version
-ddt.read_delta_table("delta_path",version=3)
+# with specific version
+ddt.read_deltalake("delta_path", version=3)
 
-# read delta table for specific datetime
-ddt.read_delta_table("delta_path",datetime="2018-12-19T16:39:57-08:00")
+# with specific datetime
+ddt.read_deltalake("delta_path", datetime="2018-12-19T16:39:57-08:00")
+```
+
+### Accessing remote file systems
 
+To be able to read from S3, azure, gcsfs, and other remote filesystems,
+you ensure the credentials are properly configured in environment variables
+or config files. For AWS, you may need `~/.aws/credential`; for gcsfs,
+`GOOGLE_APPLICATION_CREDENTIALS`. Refer to your cloud provider documentation
+to configure these.
 
-# read delta complete history
-ddt.read_delta_history("delta_path")
+```python
+ddt.read_deltalake("s3://bucket_name/delta_path", version=3)
+```
 
-# read delta history upto given limit
-ddt.read_delta_history("delta_path",limit=5)
+### Accessing AWS Glue catalog
 
-# read delta history to delete the files
-ddt.vacuum("delta_path",dry_run=False)
+`dask-deltatable` can connect to AWS Glue catalog to read the delta table.
+The method will look for `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY`
+environment variables, and if those are not available, fall back to
+`~/.aws/credentials`.
 
-# Can read from S3,azure,gcfs etc.
-ddt.read_delta_table("s3://bucket_name/delta_path",version=3)
-# please ensure the credentials are properly configured as environment variable or
-# configured as in ~/.aws/credential
+Example:
+
+```python
+ddt.read_deltalake(catalog="glue", database_name="science", table_name="physics")
 ```
 
+### Writing to Delta Lake
+
+To write a Dask dataframe to Delta Lake, use `to_deltalake` method.
+
+```python
+import dask.dataframe as dd
+import dask_deltatable as ddt
+
+df = dd.read_csv("s3://bucket_name/data.csv")
+# do some processing on the dataframe...
+ddt.to_deltalake(df, "s3://bucket_name/delta_path")
+```
 
+Writing to Delta Lake is still in development, so be aware that some features
+may not work.
```

