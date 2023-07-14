# Comparing `tmp/mostats-1.0.3-py3-none-any.whl.zip` & `tmp/mostats-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15945 bytes, number of entries: 8
+Zip file size: 16429 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 08:19 mostats/__init__.py
--rw-r--r--  2.0 unx     3786 b- defN 23-Jul-02 17:13 mostats/getCluster.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-03 12:24 mostats-1.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2295 b- defN 23-Jul-03 12:24 mostats-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 12:24 mostats-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-03 12:24 mostats-1.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-03 12:24 mostats-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      632 b- defN 23-Jul-03 12:24 mostats-1.0.3.dist-info/RECORD
-8 files, 42014 bytes uncompressed, 14837 bytes compressed:  64.7%
+-rw-r--r--  2.0 unx     6450 b- defN 23-Jul-14 10:35 mostats/getCluster.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-14 10:37 mostats-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2295 b- defN 23-Jul-14 10:37 mostats-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 10:37 mostats-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-14 10:37 mostats-1.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-14 10:37 mostats-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      632 b- defN 23-Jul-14 10:37 mostats-1.0.4.dist-info/RECORD
+8 files, 44678 bytes uncompressed, 15321 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: mostats/__init__.py
 Comment: 
 
 Filename: mostats/getCluster.py
 Comment: 
 
-Filename: mostats-1.0.3.dist-info/LICENSE
+Filename: mostats-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: mostats-1.0.3.dist-info/METADATA
+Filename: mostats-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: mostats-1.0.3.dist-info/WHEEL
+Filename: mostats-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: mostats-1.0.3.dist-info/entry_points.txt
+Filename: mostats-1.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: mostats-1.0.3.dist-info/top_level.txt
+Filename: mostats-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mostats-1.0.3.dist-info/RECORD
+Filename: mostats-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mostats/getCluster.py

```diff
@@ -3,41 +3,74 @@
 import pandas as pd
 import csv
 import argparse
 import sys
 import os
 
 output = []
+cluster_stats = []
 
 def main():
 
     argparser = argparse.ArgumentParser(description='Get the MongoDB database statistic '
                                                     'to a local CSV file')
-    argparser.add_argument('-u', '--url', default="mongodb://127.0.0.1",
-                            help='MongoDB cluster URL, default is "mongodb://127.0.0.1". \nExample: mongodb+srv://<<username>>:<<password>>@cluster.zqqqy.mongodb.net/?retryWrites=true&w=majority')
+    argparser.add_argument('-u', '--url', nargs='+', default="mongodb://127.0.0.1",
+                            help='MongoDB cluster URL, default is "mongodb://127.0.0.1". \nExample: "mongodb+srv://<<username>>:<<password>>@cluster.zqqqy.mongodb.net/?retryWrites=true&w=majority". For multiple server please use the space and "" to seperate example:"mongodb+srv://<<username>>:<<password>>@cluster1.zqqqy.mongodb.net/?retryWrites=true&w=majority" "mongodb+srv://<<username>>:<<password>>@cluster2.zqqqy.mongodb.net/?retryWrites=true&w=majority" ')
     argparser.add_argument('-c', '--csv', default="cluster-data.csv",
                             help='CSV filename, default "cluster-data.csv" \n')
-    argparser.add_argument('-n', '--name', default="",
-                            help='Cluster name, default value first subdomain example: mongodb+srv://clustername.cl0.mongodb.net will be clustername \n')
+    argparser.add_argument('-n', '--name', nargs='+', default="",
+                            help='Cluster name, default value first subdomain example: mongodb+srv://clustername.cl0.mongodb.net will be clustername. For multiple server please use the space and "" to seperate example:"cluster1" "cluster2"  \n')
+    argparser.add_argument('-m', '--moreinfo', default=False,
+                            help='Getting the host information, uptime, total number of command, read, and insert \n')
     args = argparser.parse_args()
     
     print('\nMostats - Get the MongoDB database statistic to a local CSV file\nPlease follow the instruction by run mostats -h\n')
 
     print(f'Get the database information from : "{args.url}" and save to "{args.csv}"')
     print('\n')
-    conn_pool = []
-    conn_pool.append(args.url)
+    conn_pool = args.url
+    more_info = args.moreinfo
+    
     try:
         for conn in conn_pool:
             parsed_uri = urlparse(conn)
             if args.name == "":
                 cluster_name = parsed_uri.hostname.split('.')[0]
             else:
                 cluster_name = args.name
             client = MongoClient(conn)
+            if more_info:               
+                data = client.admin.command("hostInfo")
+                cstat = {
+                    "cluster_name" : cluster_name,
+                    "hostname" : data["system"]["hostname"],
+                    "memSizeMB" : data["system"]["memSizeMB"],
+                    "numCores" : data["system"]["numCores"], 
+                    "numPhysicalCores" : data["system"]["numPhysicalCores"],
+                    "cpuArch" : data["system"]["cpuArch"]            
+                }
+                server_status = client.admin.command("serverStatus")
+
+                cstat.update({
+                    "uptime" : server_status["uptime"],
+                    "opc_insert" : server_status["opcounters"]["insert"], 
+                    "opc_query" : server_status["opcounters"]["query"],
+                    "opc_update" : server_status["opcounters"]["update"],
+                    "opc_delete" : server_status["opcounters"]["delete"], 
+                    "opc_getmore" : server_status["opcounters"]["getmore"],
+                    "opc_command" : server_status["opcounters"]["command"],
+                    "est_insert_per_sec" : round((server_status["opcounters"]["insert"])/ server_status["uptime"],2),
+                    "est_query_per_sec" : round((server_status["opcounters"]["query"])/ server_status["uptime"],2),
+                    "est_update_per_sec" : round((server_status["opcounters"]["update"])/ server_status["uptime"],2),
+                    "est_delete_per_sec" : round((server_status["opcounters"]["delete"])/ server_status["uptime"],2),
+                    "est_getmore_per_sec" : round((server_status["opcounters"]["getmore"])/ server_status["uptime"],2),
+                    "est_command_per_sec" : round((server_status["opcounters"]["command"])/ server_status["uptime"],2),           
+                })
+                cluster_stats.append(cstat)
+
             for db in client.list_database_names():
                 if db not in ["admin", "config", "local"]:
                     for coll in client[db].list_collections():
                         if (coll["name"] not in ["system.views"]) and (coll["type"] != "view"):
                             try:
                                 avgObjSize = client[db].command(
                                     "collStats", coll["name"], scale=1024*1024)["avgObjSize"]
@@ -61,14 +94,17 @@
                                 "total_size_MB": client[db].command("collStats", coll["name"], scale=1024*1024)["totalSize"],
                             }
                             output.append(coll_stat)
             client.close()
 
         df = pd.json_normalize(output)
         df.to_csv(args.csv, quoting=csv.QUOTE_NONNUMERIC, index=False)
+        if more_info:
+            df = pd.json_normalize(cluster_stats)
+            df.to_csv("cluster-info.csv", quoting=csv.QUOTE_NONNUMERIC, index=False)
     except KeyboardInterrupt:
         shutdown()
     except Exception as e:
         print("Exception:", str(e))
 
 def shutdown():
     print()
```

## Comparing `mostats-1.0.3.dist-info/LICENSE` & `mostats-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mostats-1.0.3.dist-info/METADATA` & `mostats-1.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mostats
-Version: 1.0.3
+Version: 1.0.4
 Summary: Get the MongoDB database statistic to a local CSV file
 Home-page: https://github.com/pix3lize/mostats
 Author: Hendri Tjipto
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

