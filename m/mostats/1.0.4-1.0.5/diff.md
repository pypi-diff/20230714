# Comparing `tmp/mostats-1.0.4-py3-none-any.whl.zip` & `tmp/mostats-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 16429 bytes, number of entries: 8
+Zip file size: 16847 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 08:19 mostats/__init__.py
--rw-r--r--  2.0 unx     6450 b- defN 23-Jul-14 10:35 mostats/getCluster.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-14 10:37 mostats-1.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2295 b- defN 23-Jul-14 10:37 mostats-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 10:37 mostats-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-14 10:37 mostats-1.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-14 10:37 mostats-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      632 b- defN 23-Jul-14 10:37 mostats-1.0.4.dist-info/RECORD
-8 files, 44678 bytes uncompressed, 15321 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx     6873 b- defN 23-Jul-14 10:59 mostats/getCluster.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-14 11:03 mostats-1.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3658 b- defN 23-Jul-14 11:03 mostats-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 11:03 mostats-1.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-14 11:03 mostats-1.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-14 11:03 mostats-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      632 b- defN 23-Jul-14 11:03 mostats-1.0.5.dist-info/RECORD
+8 files, 46464 bytes uncompressed, 15739 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: mostats/__init__.py
 Comment: 
 
 Filename: mostats/getCluster.py
 Comment: 
 
-Filename: mostats-1.0.4.dist-info/LICENSE
+Filename: mostats-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: mostats-1.0.4.dist-info/METADATA
+Filename: mostats-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: mostats-1.0.4.dist-info/WHEEL
+Filename: mostats-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: mostats-1.0.4.dist-info/entry_points.txt
+Filename: mostats-1.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: mostats-1.0.4.dist-info/top_level.txt
+Filename: mostats-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: mostats-1.0.4.dist-info/RECORD
+Filename: mostats-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mostats/getCluster.py

```diff
@@ -20,27 +20,30 @@
     argparser.add_argument('-n', '--name', nargs='+', default="",
                             help='Cluster name, default value first subdomain example: mongodb+srv://clustername.cl0.mongodb.net will be clustername. For multiple server please use the space and "" to seperate example:"cluster1" "cluster2"  \n')
     argparser.add_argument('-m', '--moreinfo', default=False,
                             help='Getting the host information, uptime, total number of command, read, and insert \n')
     args = argparser.parse_args()
     
     print('\nMostats - Get the MongoDB database statistic to a local CSV file\nPlease follow the instruction by run mostats -h\n')
-
-    print(f'Get the database information from : "{args.url}" and save to "{args.csv}"')
+    if args.name == "":
+        print(f'Get the database information from : "{args.url}" and save to "{args.csv}"')
+    else:
+        print(f'Get the database information from : "{args.url}" with cluster name "{args.name}" and save to "{args.csv}"')
     print('\n')
+    print("Please wait as it might take a while...")
     conn_pool = args.url
     more_info = args.moreinfo
-    
+    counter = 0    
     try:
         for conn in conn_pool:
             parsed_uri = urlparse(conn)
             if args.name == "":
                 cluster_name = parsed_uri.hostname.split('.')[0]
             else:
-                cluster_name = args.name
+                cluster_name = args.name[counter]
             client = MongoClient(conn)
             if more_info:               
                 data = client.admin.command("hostInfo")
                 cstat = {
                     "cluster_name" : cluster_name,
                     "hostname" : data["system"]["hostname"],
                     "memSizeMB" : data["system"]["memSizeMB"],
@@ -89,22 +92,24 @@
                                 "avg_obj_size_Bytes": avgObjSize,
                                 "num_doc": num_doc,
                                 "storage_size_MB": client[db].command("collStats", coll["name"], scale=1024*1024)["storageSize"],
                                 "num_idx": client[db].command("collStats", coll["name"])["nindexes"],
                                 "idx_size_MB": client[db].command("collStats", coll["name"], scale=1024*1024)["totalIndexSize"],
                                 "total_size_MB": client[db].command("collStats", coll["name"], scale=1024*1024)["totalSize"],
                             }
-                            output.append(coll_stat)
+                            output.append(coll_stat)                                                                                 
+            counter = counter + 1
             client.close()
 
         df = pd.json_normalize(output)
         df.to_csv(args.csv, quoting=csv.QUOTE_NONNUMERIC, index=False)
         if more_info:
             df = pd.json_normalize(cluster_stats)
             df.to_csv("cluster-info.csv", quoting=csv.QUOTE_NONNUMERIC, index=False)
+        print("Getting cluster information - completed successfully")
     except KeyboardInterrupt:
         shutdown()
     except Exception as e:
         print("Exception:", str(e))
 
 def shutdown():
     print()
```

## Comparing `mostats-1.0.4.dist-info/LICENSE` & `mostats-1.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

