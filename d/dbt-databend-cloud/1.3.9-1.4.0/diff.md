# Comparing `tmp/dbt_databend_cloud-1.3.9-py3-none-any.whl.zip` & `tmp/dbt_databend_cloud-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 19157 bytes, number of entries: 20
+Zip file size: 19172 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      545 b- defN 23-Feb-12 13:44 dbt/adapters/databend/__init__.py
--rw-r--r--  2.0 unx       18 b- defN 23-Jul-14 11:02 dbt/adapters/databend/__version__.py
+-rw-r--r--  2.0 unx       18 b- defN 23-Jul-14 13:11 dbt/adapters/databend/__version__.py
 -rw-r--r--  2.0 unx     1607 b- defN 23-Feb-12 13:44 dbt/adapters/databend/column.py
--rw-r--r--  2.0 unx     7119 b- defN 23-Feb-12 13:44 dbt/adapters/databend/connections.py
+-rw-r--r--  2.0 unx     7131 b- defN 23-Jul-14 13:07 dbt/adapters/databend/connections.py
 -rw-r--r--  2.0 unx    11247 b- defN 23-Feb-12 13:44 dbt/adapters/databend/impl.py
 -rw-r--r--  2.0 unx     2802 b- defN 23-Feb-12 13:44 dbt/adapters/databend/relation.py
 -rw-r--r--  2.0 unx       52 b- defN 23-Feb-12 13:44 dbt/include/databend/__init__.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-12 13:44 dbt/include/databend/dbt_project.yml
 -rw-r--r--  2.0 unx      185 b- defN 23-Feb-12 13:44 dbt/include/databend/profile_template.yml
 -rw-r--r--  2.0 unx     8965 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/adapters.sql
 -rw-r--r--  2.0 unx      796 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/catalog.sql
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/incremental.sql
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/snapshot.sql
 -rw-r--r--  2.0 unx      285 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/utils.sql
 -rw-r--r--  2.0 unx     1111 b- defN 23-Feb-12 13:44 dbt/include/databend/macros/materializations/seed.sql
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-14 11:02 dbt_databend_cloud-1.3.9.dist-info/LICENSE
--rw-r--r--  2.0 unx      856 b- defN 23-Jul-14 11:02 dbt_databend_cloud-1.3.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 11:02 dbt_databend_cloud-1.3.9.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Jul-14 11:02 dbt_databend_cloud-1.3.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1839 b- defN 23-Jul-14 11:02 dbt_databend_cloud-1.3.9.dist-info/RECORD
-20 files, 48957 bytes uncompressed, 16069 bytes compressed:  67.2%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-14 13:14 dbt_databend_cloud-1.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      856 b- defN 23-Jul-14 13:14 dbt_databend_cloud-1.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 13:14 dbt_databend_cloud-1.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-14 13:14 dbt_databend_cloud-1.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1839 b- defN 23-Jul-14 13:14 dbt_databend_cloud-1.4.0.dist-info/RECORD
+20 files, 48969 bytes uncompressed, 16084 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: dbt/include/databend/macros/utils.sql
 Comment: 
 
 Filename: dbt/include/databend/macros/materializations/seed.sql
 Comment: 
 
-Filename: dbt_databend_cloud-1.3.9.dist-info/LICENSE
+Filename: dbt_databend_cloud-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: dbt_databend_cloud-1.3.9.dist-info/METADATA
+Filename: dbt_databend_cloud-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: dbt_databend_cloud-1.3.9.dist-info/WHEEL
+Filename: dbt_databend_cloud-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: dbt_databend_cloud-1.3.9.dist-info/top_level.txt
+Filename: dbt_databend_cloud-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dbt_databend_cloud-1.3.9.dist-info/RECORD
+Filename: dbt_databend_cloud-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dbt/adapters/databend/__version__.py

```diff
@@ -1 +1 @@
-version = "1.3.9"
+version = "1.4.0"
```

## dbt/adapters/databend/connections.py

```diff
@@ -138,15 +138,15 @@
             # handle = mysql.connector.connect(
             #     # host=credentials.host,
             #     # port=credentials.port,
             #     # user=credentials.username,
             #     # password=credentials.password,
             # )
             handle = connector.connect(
-                f"https://{credentials.username}:{credentials.password}@{credentials.host}:{credentials.port}"
+                f"https://{credentials.username}:{credentials.password}@{credentials.host}:{credentials.port}?secure=true"
             )
         except Exception as e:
             logger.debug("Error opening connection: {}".format(e))
             connection.handle = None
             connection.state = "fail"
             raise dbt.exceptions.FailedToConnectException(str(e))
         connection.state = "open"
```

## Comparing `dbt_databend_cloud-1.3.9.dist-info/LICENSE` & `dbt_databend_cloud-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dbt_databend_cloud-1.3.9.dist-info/METADATA` & `dbt_databend_cloud-1.4.0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dbt-databend-cloud
-Version: 1.3.9
+Version: 1.4.0
 Summary: The Databend adapter plugin for dbt
 Home-page: https://github.com/databendcloud/dbt-databend.git
 Author: Databend Cloud Team
 Author-email: zhangzhihan@datafuselabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: dbt-core (~=1.3.0)
-Requires-Dist: databend-py (~=0.3.5)
-Requires-Dist: databend-sqlalchemy (~=0.1.6)
+Requires-Dist: dbt-core (~=1.5.0)
+Requires-Dist: databend-py (~=0.4.6)
+Requires-Dist: databend-sqlalchemy (~=0.2.4)
 
 The Databend adapter plugin for dbt
```

## Comparing `dbt_databend_cloud-1.3.9.dist-info/RECORD` & `dbt_databend_cloud-1.4.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 dbt/adapters/databend/__init__.py,sha256=SvHY_N6iQvLzzJNhLWeWP9su1lEfVliXN4NzmFQgzwA,545
-dbt/adapters/databend/__version__.py,sha256=S4484zKxazmCEjR_tzIaYTqk-8UR8cU_9f_6D0z7bfg,18
+dbt/adapters/databend/__version__.py,sha256=0kccNYBMuNA3PIhlESWmh8xP1TWpNtIEzS0d-x80SC0,18
 dbt/adapters/databend/column.py,sha256=l0FNfQwJP1kuRtU7OebBH9mhI9LF3sJHN9Kyo76_RGk,1607
-dbt/adapters/databend/connections.py,sha256=F3Nxh_joLVBJQ8uZnR1ehKjAmi8RfnWmkbDVVpNw-Ts,7119
+dbt/adapters/databend/connections.py,sha256=QfnMHhkauKxr9pKzDiywIZw3r1CoPZp18Un8e-Q8MWo,7131
 dbt/adapters/databend/impl.py,sha256=3IRK-vDdhkl8NsWUqIbEAsw7MBNYqRGq-YSNNJRF66c,11247
 dbt/adapters/databend/relation.py,sha256=52y6AXCl-4sgPfY3c7R0Ktjqb0Dj4ipSBAzUC7Kc22M,2802
 dbt/include/databend/__init__.py,sha256=vBGWeG-dHHkimfnX8axBJ4IgAowFw8xADmo6Auzn2xc,52
 dbt/include/databend/dbt_project.yml,sha256=s8hSnilCRK8ICItNQ_B2qOwsC13yHkSj3XkiMWNwefc,77
 dbt/include/databend/profile_template.yml,sha256=_Q0973TJHhTwumKY63JaGVmBrCNkDrWTUk7QNSDiu_0,185
 dbt/include/databend/macros/adapters.sql,sha256=HaYFM1J5KfKyUnmoNDuOeiWbrw4eK7HFB5Gd7TEgvV8,8965
 dbt/include/databend/macros/catalog.sql,sha256=vcEQgzo9t6JSd3hLMb4MWgjsp87D4UjXa967r63l1FA,796
 dbt/include/databend/macros/incremental.sql,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dbt/include/databend/macros/snapshot.sql,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dbt/include/databend/macros/utils.sql,sha256=RIu7q-44BE2gU10miSNJr11A9X_D9KfNI-HvE7lEa1c,285
 dbt/include/databend/macros/materializations/seed.sql,sha256=f8_gtCILvU5nSsp3WgMccVvDvGB4whpntB17-_rTgOE,1111
-dbt_databend_cloud-1.3.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-dbt_databend_cloud-1.3.9.dist-info/METADATA,sha256=2JddBlGOtOuOSvFsEz_1LPCQazU0-lwAuCsSkscL_yA,856
-dbt_databend_cloud-1.3.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dbt_databend_cloud-1.3.9.dist-info/top_level.txt,sha256=B2YH4he17ajilEWOGCKHbRcEJlCuZKwCcgFcLPntLsE,4
-dbt_databend_cloud-1.3.9.dist-info/RECORD,,
+dbt_databend_cloud-1.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+dbt_databend_cloud-1.4.0.dist-info/METADATA,sha256=F4D9rhZXq1wehhbULmfiNtMJWhJDX28Piy_D9OMCfs4,856
+dbt_databend_cloud-1.4.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dbt_databend_cloud-1.4.0.dist-info/top_level.txt,sha256=B2YH4he17ajilEWOGCKHbRcEJlCuZKwCcgFcLPntLsE,4
+dbt_databend_cloud-1.4.0.dist-info/RECORD,,
```

