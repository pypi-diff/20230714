# Comparing `tmp/ndp-app-deployment-1.3.tar.gz` & `tmp/ndp-app-deployment-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndp-app-deployment-1.3.tar", last modified: Tue Jul 11 06:34:25 2023, max compression
+gzip compressed data, was "ndp-app-deployment-1.4.tar", last modified: Fri Jul 14 03:33:03 2023, max compression
```

## Comparing `ndp-app-deployment-1.3.tar` & `ndp-app-deployment-1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-11 06:34:25.121306 ndp-app-deployment-1.3/
--rw-r--r--   0 harshal    (502) staff       (20)      714 2023-07-11 06:34:25.120976 ndp-app-deployment-1.3/PKG-INFO
--rwxrwxr-x   0 harshal    (502) staff       (20)      251 2023-07-11 06:30:24.000000 ndp-app-deployment-1.3/README.md
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-11 06:34:25.119740 ndp-app-deployment-1.3/ndp_app_deployment.egg-info/
--rw-r--r--   0 harshal    (502) staff       (20)      714 2023-07-11 06:34:24.000000 ndp-app-deployment-1.3/ndp_app_deployment.egg-info/PKG-INFO
--rw-r--r--   0 harshal    (502) staff       (20)      288 2023-07-11 06:34:25.000000 ndp-app-deployment-1.3/ndp_app_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 harshal    (502) staff       (20)        1 2023-07-11 06:34:24.000000 ndp-app-deployment-1.3/ndp_app_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 harshal    (502) staff       (20)       65 2023-07-11 06:34:24.000000 ndp-app-deployment-1.3/ndp_app_deployment.egg-info/requires.txt
--rw-r--r--   0 harshal    (502) staff       (20)       15 2023-07-11 06:34:24.000000 ndp-app-deployment-1.3/ndp_app_deployment.egg-info/top_level.txt
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-11 06:34:25.120337 ndp-app-deployment-1.3/ndp_deployment/
--rw-r--r--   0 harshal    (502) staff       (20)        0 2021-07-15 08:59:23.000000 ndp-app-deployment-1.3/ndp_deployment/__init__.py
--rw-r--r--   0 harshal    (502) staff       (20)    48802 2023-07-11 06:27:39.000000 ndp-app-deployment-1.3/ndp_deployment/fetch_metastore.py
--rw-r--r--   0 harshal    (502) staff       (20)       38 2023-07-11 06:34:25.121393 ndp-app-deployment-1.3/setup.cfg
--rwxrwxr-x   0 harshal    (502) staff       (20)     1432 2023-07-11 06:27:02.000000 ndp-app-deployment-1.3/setup.py
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 03:33:03.438071 ndp-app-deployment-1.4/
+-rw-r--r--   0 harshal    (502) staff       (20)      714 2023-07-14 03:33:03.437651 ndp-app-deployment-1.4/PKG-INFO
+-rwxrwxr-x   0 harshal    (502) staff       (20)      251 2023-07-14 03:32:35.000000 ndp-app-deployment-1.4/README.md
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 03:33:03.434438 ndp-app-deployment-1.4/ndp_app_deployment.egg-info/
+-rw-r--r--   0 harshal    (502) staff       (20)      714 2023-07-14 03:33:03.000000 ndp-app-deployment-1.4/ndp_app_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 harshal    (502) staff       (20)      288 2023-07-14 03:33:03.000000 ndp-app-deployment-1.4/ndp_app_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 harshal    (502) staff       (20)        1 2023-07-14 03:33:03.000000 ndp-app-deployment-1.4/ndp_app_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 harshal    (502) staff       (20)       65 2023-07-14 03:33:03.000000 ndp-app-deployment-1.4/ndp_app_deployment.egg-info/requires.txt
+-rw-r--r--   0 harshal    (502) staff       (20)       15 2023-07-14 03:33:03.000000 ndp-app-deployment-1.4/ndp_app_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 03:33:03.435140 ndp-app-deployment-1.4/ndp_deployment/
+-rw-r--r--   0 harshal    (502) staff       (20)        0 2021-07-15 08:59:23.000000 ndp-app-deployment-1.4/ndp_deployment/__init__.py
+-rw-r--r--   0 harshal    (502) staff       (20)    49066 2023-07-14 03:32:02.000000 ndp-app-deployment-1.4/ndp_deployment/fetch_metastore.py
+-rw-r--r--   0 harshal    (502) staff       (20)       38 2023-07-14 03:33:03.438175 ndp-app-deployment-1.4/setup.cfg
+-rwxrwxr-x   0 harshal    (502) staff       (20)     1432 2023-07-14 03:32:21.000000 ndp-app-deployment-1.4/setup.py
```

### Comparing `ndp-app-deployment-1.3/PKG-INFO` & `ndp-app-deployment-1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ndp-app-deployment
-Version: 1.3
+Version: 1.4
 Summary: Version Control Mechanism for Zetaris Platform (https://www.zetaris.com/)
 Home-page: https://github.com/zetaris/versioncontrol
 Author: Harshal Shah
 Author-email: harshal.shah@zetaris.com
 License: Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 ### Usage and Installation
 ```
-pip3 install install ndp-app-deployment==1.3
+pip3 install install ndp-app-deployment==1.4
 
 from ndp_deployment.fetch_metastore import object_deployment
 
 object_deployment(api_url,user_email,user_password,folder_path,option_for_backup,container_name,object_name)
 ```
```

### Comparing `ndp-app-deployment-1.3/ndp_app_deployment.egg-info/PKG-INFO` & `ndp-app-deployment-1.4/ndp_app_deployment.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ndp-app-deployment
-Version: 1.3
+Version: 1.4
 Summary: Version Control Mechanism for Zetaris Platform (https://www.zetaris.com/)
 Home-page: https://github.com/zetaris/versioncontrol
 Author: Harshal Shah
 Author-email: harshal.shah@zetaris.com
 License: Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 ### Usage and Installation
 ```
-pip3 install install ndp-app-deployment==1.3
+pip3 install install ndp-app-deployment==1.4
 
 from ndp_deployment.fetch_metastore import object_deployment
 
 object_deployment(api_url,user_email,user_password,folder_path,option_for_backup,container_name,object_name)
 ```
```

### Comparing `ndp-app-deployment-1.3/ndp_deployment/fetch_metastore.py` & `ndp-app-deployment-1.4/ndp_deployment/fetch_metastore.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,42 +172,42 @@
         set_api_base_url(api_url)
         login(lightning_username,lightning_pass)
     except:
         logger.info("\nCannot connect to Zetaris API\n")
         logger.info("Please try again.\n")
         serverDetails(api_url,lightning_username,lightning_pass,folder_path)
 #-------------------------------------------------------------------------#           
-def mainMenu(option,arg1,arg2,arg3,lightning_username):
+def mainMenu(option,arg1,arg2,arg3,lightning_username,folder_path):
     if option != 10000:
         print("\n Select the following option to migrate: \n")
         print("1. Data Pipeline container")
         print("2. Individual Data Pipeline")
         print("3. Data Quality container")
         print("4. Individual Data Quality Pipeline")
         print("5. Data Mart")
         print("6. Individual Table/View in the existing Datamart")
         print("7. Permanent Views")
         print("8. View the list of Container/Pipeline Name")
         print("9. Exit")
         try:
             option = int(str(arg1).lower().strip())
             if option == 1:
-                DataPipelineContainer_InsertQueries(arg1,arg2,arg3,lightning_username)
+                DataPipelineContainer_InsertQueries(arg1,arg2,arg3,lightning_username,folder_path)
             elif option == 2:
-                IndivdualDataPipeline_InsertQueries(arg1,arg2,arg3,lightning_username)
+                IndivdualDataPipeline_InsertQueries(arg1,arg2,arg3,lightning_username,folder_path)
             elif option == 3:
-                DataPipelineContainer_InsertQueries(arg1,arg2,arg3,lightning_username)
+                DataPipelineContainer_InsertQueries(arg1,arg2,arg3,lightning_username,folder_path)
             elif option == 4:
-                IndivdualDataPipeline_InsertQueries(arg1,arg2,arg3,lightning_username)
+                IndivdualDataPipeline_InsertQueries(arg1,arg2,arg3,lightning_username,folder_path)
             elif option == 5:
-                DataMart_InsertQueries(arg1,arg2,arg3,lightning_username)
+                DataMart_InsertQueries(arg1,arg2,arg3,lightning_username,folder_path)
             elif option == 6:
-                DataMart_IndTable_InsertQueries(arg1,arg2,arg3,lightning_username)
+                DataMart_IndTable_InsertQueries(arg1,arg2,arg3,lightning_username,folder_path)
             elif option == 7:
-                PermanentViews_InsertQueries(arg1,arg2,arg3,lightning_username)
+                PermanentViews_InsertQueries(arg1,arg2,arg3,lightning_username,folder_path)
             elif option == 9:
                 print("\nThanks for using the system")
                 exit
             else:
                 print("\n Invalid option\n")
                 print("\n Thanks for using the system")
                 exit
@@ -285,15 +285,15 @@
                 return True
         else:
             return False
     except Exception as e:
         logger.info("Checking View Name")
         logger.info(e)  
 #-------------------------------------------------------------------------#
-def DataPipelineContainer_InsertQueries(arg1,arg2,arg3,lightning_username):
+def DataPipelineContainer_InsertQueries(arg1,arg2,arg3,lightning_username,folder_path):
     try:
         container_name = str(arg2).strip()
         container_name = container_name.lower()
         chk_container_name= checkcontainername(container_name)
         if chk_container_name == False:
             logger.info("\nIncorrect container name. Please check the container name & try again.")
         else:
@@ -408,22 +408,22 @@
             sql_pipeline_simple_dq_rule = """SELECT 'INSERT INTO metastore.pipeline_simple_dq_rule (id, columns ,expression , filter , name,fk_pipeline_simple_dq_id  ) VALUES (' || id || ',''' ||CHAR(39)||COALESCE(columns, '')||CHAR(39) || ''',''' ||CHAR(34)|| COALESCE(expression, '')||CHAR(34) || ''',''' ||CHAR(34)|| COALESCE(filter, '')||CHAR(34) || ''',''' ||CHAR(39)|| COALESCE(name, '')||CHAR(39) || ''',' || COALESCE(fk_pipeline_simple_dq_id, 0) || ')' as sql_query_simdq_rule FROM metastore.pipeline_simple_dq_rule where fk_pipeline_simple_dq_id in (select id from metastore.pipeline_simple_dq where id in (select id from metastore.pipeline_node where fk_pipeline_relation_id in (select id from metastore.pipeline_relation where fk_pipeline_container_id in (select id from metastore.pipeline_container where name = '%s'))));"""%(container_name)
             res = exec_query_get_res(sql_pipeline_simple_dq_rule)
             if res:
                 if isinstance(res[0],dict):
                     for i in res:
                         list_queries.append(str(i['sql_query_simdq_rule']))
                         
-            generateSQLfile(list_queries,container_name,'pipeline','',lightning_username)
+            generateSQLfile(list_queries,container_name,'pipeline','',lightning_username,folder_path)
             print('Script Generated...')
     except Exception as e:
         print(e)
         logger.info("Inside Full Pipeline container backup function")
         logger.info(e)
 #-------------------------------------------------------------------------#
-def IndivdualDataPipeline_InsertQueries(arg1,arg2,arg3,lightning_username):
+def IndivdualDataPipeline_InsertQueries(arg1,arg2,arg3,lightning_username,folder_path):
     try:
         container_name = str(arg2).strip()
         container_name = container_name.lower()
         pipeline_name=str(arg3).strip()
         pipeline_name=pipeline_name.lower()
         chk_con_pipe_name= checkcontainer_pipeline_name(container_name,pipeline_name)
         if chk_con_pipe_name == False:
@@ -530,22 +530,22 @@
             sql_pipeline_simple_dq_rule = """SELECT 'INSERT INTO metastore.pipeline_simple_dq_rule (id, columns ,expression , filter , name,fk_pipeline_simple_dq_id  ) VALUES (' || id || ',''' ||CHAR(39)||COALESCE(columns, '')||CHAR(39)|| ''',''' ||CHAR(34)||COALESCE(expression, '')||CHAR(34) || ''',''' ||CHAR(34)|| COALESCE(filter, '')||CHAR(34) || ''',''' ||CHAR(39)||COALESCE(name, '')||CHAR(39)|| ''',' || COALESCE(fk_pipeline_simple_dq_id, 0) || ')' as sql_query_simdq_rule FROM metastore.pipeline_simple_dq_rule where fk_pipeline_simple_dq_id in (select id from metastore.pipeline_simple_dq where id in (select id from metastore.pipeline_node where fk_pipeline_relation_id in (select id from metastore.pipeline_relation where fk_pipeline_container_id in (select id from metastore.pipeline_container where name = '%s') and name='%s')));"""%(container_name,pipeline_name)
             res = exec_query_get_res(sql_pipeline_simple_dq_rule)
             if res:
                 if isinstance(res[0],dict):
                     for i in res:
                         list_queries.append(str(i['sql_query_simdq_rule']))
             
-            generateSQLfile(list_queries,container_name,pipeline_name,'Pipeline',lightning_username)
+            generateSQLfile(list_queries,container_name,pipeline_name,'Pipeline',lightning_username,folder_path)
             print('Script Generated...')
     except Exception as e:
         print(e)
         logger.info("Inside Individual Pipeline Backup Function")
         logger.info(e)
 #-------------------------------------------------------------------------#    
-def PermanentViews_InsertQueries(arg1,arg2,arg3,lightning_username):
+def PermanentViews_InsertQueries(arg1,arg2,arg3,lightning_username,folder_path):
     try:
         View_name=str(arg2).strip()
         View_name = View_name.upper().strip()
         chk_viewname= chk_view_name(View_name)
         if chk_viewname == False:
             print("\n Incorrect view name.")  
         else:
@@ -561,21 +561,21 @@
             sql_schema_store_view_schema = """select  'INSERT INTO metastore.schema_store_view_schema  (id, column_name  ,data_type , fk_schema_store_view_id) VALUES (' || id || ',''' || CHAR(39) || COALESCE(column_name, '') || CHAR(39) || ''',''' || CHAR(39) || COALESCE(data_type, '') || char(39) || ''',' || COALESCE(fk_schema_store_view_id, 0) || ')' as sql_query_pmvw_schema FROM metastore.schema_store_view_schema where fk_schema_store_view_id in (select id from metastore.schema_store_view where name = '%s');"""%(View_name)
             res = exec_query_get_res(sql_schema_store_view_schema)
             if res:
                 if isinstance(res[0],dict):
                     for i in res:
                         list_queries.append(str(i['sql_query_pmvw_schema']))
                         
-            generateSQLfile(list_queries,View_name,'Permanent_View','',lightning_username)
+            generateSQLfile(list_queries,View_name,'Permanent_View','',lightning_username,folder_path)
             print('Script Generated...')
     except Exception as e:
         logger.info("Inside Permanent View Backup Function")
         logger.info(e)
 #-------------------------------------------------------------------------#
-def DataMart_InsertQueries(arg1,arg2,arg3,lightning_username):
+def DataMart_InsertQueries(arg1,arg2,arg3,lightning_username,folder_path):
     try:
         datamart_name=str(arg2).strip()
         datamart_name = datamart_name.upper().strip()
         chk_dm_name= chk_datamart_name(datamart_name)
         if chk_dm_name == False:
             print("\n Incorrect data mart name.")  
         else:
@@ -597,21 +597,21 @@
             sql_data_mart_table_schema = """select  'INSERT INTO metastore.data_mart_table_schema (id, real_column_name , virtual_name, fk_data_mart_table_id)  VALUES (' || id || ',''' ||CHAR(39)||COALESCE(real_column_name, '')||CHAR(39) || ''',''' ||CHAR(39)|| COALESCE(virtual_name, '')||CHAR(39) ||''','|| COALESCE(fk_data_mart_table_id,0) ||')' as sql_query_dm_schema from metastore.data_mart_table_schema where fk_data_mart_table_id in (select id from metastore.data_mart_table where fk_data_mart_id in (select id from  metastore.data_mart where name = '%s'));"""%(datamart_name)
             res = exec_query_get_res(sql_data_mart_table_schema)
             if res:
                 if isinstance(res[0],dict):
                     for i in res:
                         list_queries.append(str(i['sql_query_dm_schema']))
 
-            generateSQLfile(list_queries,datamart_name,'DataMart','',lightning_username)
+            generateSQLfile(list_queries,datamart_name,'DataMart','',lightning_username,folder_path)
             print('Script Generated...')
     except Exception as e:
         logger.info("Inside Data Mart backup Function")
         logger.info(e)
 #-------------------------------------------------------------------------#        
-def DataMart_IndTable_InsertQueries(arg1,arg2,arg3,lightning_username):
+def DataMart_IndTable_InsertQueries(arg1,arg2,arg3,lightning_username,folder_path):
     try:
         datamart_name=str(arg2).strip()
         datamart_name = datamart_name.upper().strip()
         table_name=str(arg3).strip()
         table_name = table_name.upper().strip()
         chk_dm_name= chk_datamart_table_name(datamart_name,table_name)
         if chk_dm_name == False:
@@ -628,41 +628,41 @@
             sql_data_mart_table_schema = """select  'INSERT INTO metastore.data_mart_table_schema (id, real_column_name , virtual_name, fk_data_mart_table_id)  VALUES (' || id || ',''' ||CHAR(39)|| COALESCE(real_column_name, '')||CHAR(39) || ''',''' ||CHAR(39)|| COALESCE(virtual_name, '')||CHAR(39) ||''','|| COALESCE(fk_data_mart_table_id,0) ||')' as sql_query_dm_schema from metastore.data_mart_table_schema where fk_data_mart_table_id in (select id from metastore.data_mart_table where fk_data_mart_id in (select id from  metastore.data_mart where name = '%s')and name='%s');"""%(datamart_name,table_name)
             res = exec_query_get_res(sql_data_mart_table_schema)
             if res:
                 if isinstance(res[0],dict):
                     for i in res:
                         list_queries.append(str(i['sql_query_dm_schema']))
             
-            generateSQLfile(list_queries,datamart_name,table_name,'DataMart',lightning_username)
+            generateSQLfile(list_queries,datamart_name,table_name,'DataMart',lightning_username,folder_path,folder_path)
             print('Script Generated...')
     except Exception as e:
         logger.info("Inside Data Mart Individual Tables Backup Function")
         logger.info(e)
 #-------------------------------------------------------------------------#    
-def generateSQLfile(list_queries,filename1,filename2,filename3,lightning_username):
+def generateSQLfile(list_queries,filename1,filename2,filename3,lightning_username,folder_path):
     try:
         orgId = get_org_id_from_email(lightning_username)
         filename1=filename1.lower()
         filename2=filename2.lower()
         filename3=filename3.lower()
         if (len(filename3)>1):
             output_filename =filename1+'-'+filename2+ '-'+ filename3 +'-'+str(orgId)+'.sql'
         else:
             output_filename=filename1+'-'+filename2+'-'+str(orgId)+'.sql'
-        df = open(output_filename, 'w+')
+        df = open(folder_path+output_filename, 'w+')
         for i in range(len(list_queries)):
             df.write(list_queries[i])
             df.write('\n')
         df.close()
     except Exception as e:
         logger.info("Inside Generating Files with SQL Queries Function")
         logger.info(e)
 #-------------------------------------------------------------------------#    
 def object_deployment(api_url,lightning_username,lightning_pass,folder_path,arg1,arg2,arg3):
     try:
         serverDetails(api_url,lightning_username,lightning_pass,folder_path)
-        mainMenu('',arg1,arg2,arg3,lightning_username)
+        mainMenu('',arg1,arg2,arg3,lightning_username,folder_path)
     except Exception as e:
         print(e)
         logger.info("Inside Main Object Deployment / Backup of Metastore Main Function")
         logger.info(e)
 #-------------------------------------------------------------------------#
```

### Comparing `ndp-app-deployment-1.3/setup.py` & `ndp-app-deployment-1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
   
 setuptools.setup(
     # Here is the module name.
     name="ndp-app-deployment",
   
     # version of the module
-    version="1.3",
+    version="1.4",
   
     # Name of Author
     author="Harshal Shah",
 
     #License
     license="Proprietary",
```

