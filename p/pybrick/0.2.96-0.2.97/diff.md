# Comparing `tmp/pybrick-0.2.96-py3-none-any.whl.zip` & `tmp/pybrick-0.2.97-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6398 bytes, number of entries: 7
+Zip file size: 6469 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-30 13:40 pybrick/__init__.py
 -rw-rw-rw-  2.0 fat       88 b- defN 23-Jun-29 01:19 pybrick/ptest.csv
--rw-rw-rw-  2.0 fat    14580 b- defN 23-Jul-01 02:11 pybrick/pybrick.py
--rw-rw-rw-  2.0 fat      322 b- defN 23-Jul-01 02:11 pybrick-0.2.96.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-01 02:11 pybrick-0.2.96.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-01 02:11 pybrick-0.2.96.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      521 b- defN 23-Jul-01 02:11 pybrick-0.2.96.dist-info/RECORD
-7 files, 15611 bytes uncompressed, 5472 bytes compressed:  64.9%
+-rw-rw-rw-  2.0 fat    15032 b- defN 23-Jul-14 17:45 pybrick/pybrick.py
+-rw-rw-rw-  2.0 fat      322 b- defN 23-Jul-14 17:45 pybrick-0.2.97.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 17:45 pybrick-0.2.97.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-14 17:45 pybrick-0.2.97.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      521 b- defN 23-Jul-14 17:45 pybrick-0.2.97.dist-info/RECORD
+7 files, 16063 bytes uncompressed, 5543 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pybrick/ptest.csv
 Comment: 
 
 Filename: pybrick/pybrick.py
 Comment: 
 
-Filename: pybrick-0.2.96.dist-info/METADATA
+Filename: pybrick-0.2.97.dist-info/METADATA
 Comment: 
 
-Filename: pybrick-0.2.96.dist-info/WHEEL
+Filename: pybrick-0.2.97.dist-info/WHEEL
 Comment: 
 
-Filename: pybrick-0.2.96.dist-info/top_level.txt
+Filename: pybrick-0.2.97.dist-info/top_level.txt
 Comment: 
 
-Filename: pybrick-0.2.96.dist-info/RECORD
+Filename: pybrick-0.2.97.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pybrick/pybrick.py

```diff
@@ -1,8 +1,8 @@
-__version__="0.2.96"
+__version__="0.2.97"
 __doc__="""
 pybrick uses sqlalchemy to provide a convenient connection to Yellowbrick.
 """
 import pdb
 import os
 import sys
 import subprocess
@@ -15,14 +15,15 @@
 from io import StringIO
 
 class YbConnector:
     """ A pytezza-esque connector to Yellowbrick. """
     def __init__(self,host,db,user,pw="",psql_compatible_version='13.7',ybhosts=None):
         """ """
         self.orig_host=host
+        self.ybhosts=ybhosts
         self.host=self._resolveHost(host,ybhosts)
         self.db=db
         self.user=user
         self.pw=pw if pw else os.environ.get('YBPASSWORD')
         
         self.psql_compatible_version=psql_compatible_version
         self.dry_run_mode=False
@@ -140,22 +141,37 @@
     
     def disconnect(self):
         """ """
         if self.connection:
             self.connection.close()
         return
     
+    
+    def switchHost(self,newhost):
+        """ """
+        print(f"Switching Yellowbrick host from {self.host} to {newhost}")
+        self.__init__(newhost,
+                      self.db,
+                      self.user,
+                      self.pw,
+                      self.psql_compatible_version,
+                      ybhosts=self.ybhosts)
+        return
+    
+    
     def query(self,query_to_run,dryRun=False,dumpTo=None,dumpAppend=False,printQuery=False):
         """ Query implies fetch data. """
         return self._query(query_to_run,withData=True,dryRun=dryRun,dumpTo=dumpTo,dumpAppend=dumpAppend,printQuery=printQuery)
-        
+    
+    
     def execute(self,query_to_run,dryRun=False,dumpTo=None,dumpAppend=False,printQuery=False):
         """ Execute implies don't fetch data. """
         return self._query(query_to_run,withData=False,dryRun=dryRun,dumpTo=dumpTo,dumpAppend=dumpAppend,printQuery=printQuery)
     
+    
     def _query(self,query_to_run,withResults=False,withData=False,dryRun=False,dumpTo=None,dumpAppend=False,printQuery=False):
         """ Query Yellowbrick, optionally returning a dataframe of results. """
         self._checkConnection(reconnect=True)
         
         df=None
         if dumpTo:
             mode="a+" if dumpAppend else "w+"
@@ -181,35 +197,38 @@
             else:
                 self.connection.execute(sa.text(query_to_run))
         except Exception as e:
             raise RuntimeError(f"There was an error while executing the SQL:\n{e}")
         
         return df
     
+    
     def tableExists(self,table):
         """ """
         (db,tbl)=table.split(".")
         q=f"""
             select count(*) as rc
             from information_schema.tables
             where upper(table_schema)=upper('{db}')
               and upper(table_name)=upper('{tbl}')
         """
         d=self.query(q)
         return d.rc[0]>0
     
+    
     def tableRowCount(self,table):
         """ """
         q=f"""
             select count(*) as rc
             from {table}
         """
         d=self.query(q)
         return d.rc[0]
     
+    
     def sample(self,table,fields=None,limit=10,orderby=None):
        """ """
        h="Sample of "+table
        print(h+"\n"+("-"*len(h)))
        return self.query(f"select {fields if fields else '*'} from {table} order by {orderby if orderby else 'random()'} limit {limit}")
     
     
@@ -222,14 +241,15 @@
         ddl = ""
         for i in range(len(src.columns)):
             #New DDL line for each element.  Trickiness to handle no-comma for last element.
             ddl+='    "%s" %s%s\n'%(src.columns[i],ybTypes[i],(i<len(src.columns)-1)*",")
             
         return ddl
     
+    
     def loadBySio(self,src,target):
         """ """
         #Initialize and load a string buffer.
         buf = StringIO()
         sz=buf.write(src.to_csv(index=None,header=True))
         buf.seek(0)
         print("Buffer size in characters:",sz)
@@ -240,39 +260,39 @@
         #Write the data into Yellowbrick.
         conn = self.engine.raw_connection()
         with conn.cursor() as c:
             c.copy_expert(f"COPY {target} FROM STDIN WITH CSV HEADER",buf)
         conn.commit()
         conn.close()
         
-        print(f"Loaded {self.tableRowCount(target)} rows into {target}.")
+        print(f"Loaded {self.tableRowCount(target)} rows into {target}")
         assert src.shape[0]==self.tableRowCount(target),"Loaded count does not match source count!"
         return
-
+    
     
     def dfToYb(self,src,target,distribute_on="random",clobber=False,ybTypes=None,verbose=False,ignoreLoadErrors=False,lite=False):
         """ Given a pandas df, push that table to yellowbrick, optionally replace the existing table in yellowbrick.
             If ybTypes immutable is provided, use those types and to hell with the consequences.
             Otherwise, infer the types.
         """
         def vprint(s):
             if verbose:
                 print(s)
         
-        print(f"Loading {src.shape[0]} rows and {src.shape[1]} columns into {target}.")
+        print(f"Loading {src.shape[0]} rows and {src.shape[1]} columns into {target}")
         print(f"Dataframe size is approximately {src.memory_usage().sum()/1024/1024:0.2f} MB.")
         vprint(f"Here is a sample of the source data:\n{src.head(5)}")
         
         #If were weren't supplied types, guess them ourselves.
         if not ybTypes:
             ybTypes=self.getYbTypesFromDf(src)
         
         #Drop the table if we're instructed to clobber.
         if clobber:
-            vprint(f"Dropping {target}.")
+            vprint(f"Dropping {target}")
             self.execute(f"drop table if exists {target};")
         
         #Use columns and datatypes to make a create-table statement.
         ddl = f"create table {target} ({self.getDfDDL(src,ybTypes)})"
         
         #Create the empty table if it doesn't exist.
         if not self.tableExists(target):
@@ -322,15 +342,15 @@
                 raise RuntimeError(f"There was a problem running ybload.  Make sure it's installed, is on your PATH, and that Java is installed:\n{e}")
             
             lrows = self.tableRowCount(target)
             if len(src)==lrows or clobber==False:
                 print("YBload successful")
                 vprint(f"Dumped {len(src)} rows, and then loaded {lrows} rows.")
             else:
-                print("WARNING: The number of rows in {target} doesn't match the size of {src}.")
+                print("WARNING: The number of rows in {target} doesn't match the size of {src}")
         
         return
     
     #Alias
     df2Yb=dfToYb
     
     def getYbTypesFromDf(self,df):
```

## Comparing `pybrick-0.2.96.dist-info/RECORD` & `pybrick-0.2.97.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 pybrick/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pybrick/ptest.csv,sha256=PW9pOhU3Z_p4s2Lt5AIwIMUr0AKDazv-5optEIwyxIY,88
-pybrick/pybrick.py,sha256=RUxLy4yIN36EelVnT2HnI5zGmS3vXf5UopK0aUNIDXI,14580
-pybrick-0.2.96.dist-info/METADATA,sha256=6q3mYAdv5ha09pR_P-IkSOVrerjk9VkEDFB49xN6Yeg,322
-pybrick-0.2.96.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-pybrick-0.2.96.dist-info/top_level.txt,sha256=Z7wcH2t0g3rREg2OMtuWYUypr2KBR3Jpkkt34YFzxXc,8
-pybrick-0.2.96.dist-info/RECORD,,
+pybrick/pybrick.py,sha256=v1h6BPM92s95pb_dqTrvLHawTodGZarCkE8cWb-a24k,15032
+pybrick-0.2.97.dist-info/METADATA,sha256=uBmuZE2NSsx93Je6nKmu3a-ydepDwkS-1ip1iZAQCgA,322
+pybrick-0.2.97.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+pybrick-0.2.97.dist-info/top_level.txt,sha256=Z7wcH2t0g3rREg2OMtuWYUypr2KBR3Jpkkt34YFzxXc,8
+pybrick-0.2.97.dist-info/RECORD,,
```

