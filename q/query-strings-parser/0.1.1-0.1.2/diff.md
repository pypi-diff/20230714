# Comparing `tmp/query_strings_parser-0.1.1.tar.gz` & `tmp/query_strings_parser-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/query_strings_parser-0.1.1.tar", last modified: Fri Jul  7 10:32:46 2023, max compression
+gzip compressed data, was "query_strings_parser-0.1.2.tar", last modified: Fri Jul 14 17:55:51 2023, max compression
```

## Comparing `query_strings_parser-0.1.1.tar` & `query_strings_parser-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:32:46.517933 query_strings_parser-0.1.1/
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)    11357 2023-07-07 10:17:08.000000 query_strings_parser-0.1.1/LICENSE
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      306 2023-07-07 10:32:46.517933 query_strings_parser-0.1.1/PKG-INFO
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)     5375 2023-07-07 10:17:08.000000 query_strings_parser-0.1.1/README.md
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      103 2023-07-07 10:32:46.517933 query_strings_parser-0.1.1/setup.cfg
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      415 2023-07-07 10:32:17.000000 query_strings_parser-0.1.1/setup.py
-drwxrwxr-x   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:32:46.517933 query_strings_parser-0.1.1/src/
-drwxrwxr-x   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:32:46.517933 query_strings_parser-0.1.1/src/query_strings_parser/
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:17:08.000000 query_strings_parser-0.1.1/src/query_strings_parser/__init__.py
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)     2854 2023-07-07 10:17:08.000000 query_strings_parser-0.1.1/src/query_strings_parser/query_parser.py
-drwxrwxr-x   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:32:46.517933 query_strings_parser-0.1.1/src/query_strings_parser.egg-info/
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      306 2023-07-07 10:32:46.000000 query_strings_parser-0.1.1/src/query_strings_parser.egg-info/PKG-INFO
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      306 2023-07-07 10:32:46.000000 query_strings_parser-0.1.1/src/query_strings_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        1 2023-07-07 10:32:46.000000 query_strings_parser-0.1.1/src/query_strings_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)       21 2023-07-07 10:32:46.000000 query_strings_parser-0.1.1/src/query_strings_parser.egg-info/top_level.txt
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 17:55:51.293203 query_strings_parser-0.1.2/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)    11357 2023-07-14 16:38:29.000000 query_strings_parser-0.1.2/LICENSE
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      340 2023-07-14 17:55:51.293203 query_strings_parser-0.1.2/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     5878 2023-07-14 17:27:48.000000 query_strings_parser-0.1.2/README.md
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      103 2023-07-14 17:55:51.293203 query_strings_parser-0.1.2/setup.cfg
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      415 2023-07-14 17:27:48.000000 query_strings_parser-0.1.2/setup.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 17:55:51.289203 query_strings_parser-0.1.2/src/
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 17:55:51.293203 query_strings_parser-0.1.2/src/query_strings_parser/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 16:38:29.000000 query_strings_parser-0.1.2/src/query_strings_parser/__init__.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3076 2023-07-14 17:27:48.000000 query_strings_parser-0.1.2/src/query_strings_parser/query_parser.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 17:55:51.293203 query_strings_parser-0.1.2/src/query_strings_parser.egg-info/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      340 2023-07-14 17:55:51.000000 query_strings_parser-0.1.2/src/query_strings_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      306 2023-07-14 17:55:51.000000 query_strings_parser-0.1.2/src/query_strings_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-14 17:55:51.000000 query_strings_parser-0.1.2/src/query_strings_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       21 2023-07-14 17:55:51.000000 query_strings_parser-0.1.2/src/query_strings_parser.egg-info/top_level.txt
```

### Comparing `query_strings_parser-0.1.1/LICENSE` & `query_strings_parser-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `query_strings_parser-0.1.1/README.md` & `query_strings_parser-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -155,14 +155,38 @@
 #             "lorem_ipsum_2",
 #             "lorem_ipsum_3"
 #          ]
 #       }
 #    }
 ```
 
+In addition to OR, the lib supports AND filters through the semicolon character.
+
+```
+https://localhost:4001/v1/predictions/?attr_1=lorem_ipsum
+
+# Result:
+#    "filters":{
+#       "attr_1":"lorem_ipsum"
+#    }
+
+https://localhost:4001/v1/predictions/?attr_1=lorem_ipsum&...&attr_2=lorem_ipsum_2;lorem_ipsum_3
+
+# Result:
+#    "filters":{
+#       "attr_1":"lorem_ipsum",
+#       "attr_2":{
+#          "$and":[
+#             "lorem_ipsum_2",
+#             "lorem_ipsum_3"
+#          ]
+#       }
+#    }
+```
+
 It also supports filtering with search through asterisks as follows:
 
 - Search where `attr` starts with **"value"**.
 
 ```
 https://localhost:4001/v1/predictions/?attr=value*
```

### Comparing `query_strings_parser-0.1.1/src/query_strings_parser/query_parser.py` & `query_strings_parser-0.1.2/src/query_strings_parser/query_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,18 @@
             elif (param == 'limit'):
                 pagination['limit'] = value
             else:
                 if (value.find(",") != -1):
                     value_temp = {}
                     value_temp["$or"] = [process_value(item) for item in value.split(",")]
                     filters[param] = value_temp
+                elif (value.find(";") != -1):
+                    value_temp = {}
+                    value_temp["$and"] = [process_value(item) for item in value.split(";")]
+                    filters[param] = value_temp
                 else:
                     filters[param] = process_value(value)
 
     if (len(fields)):
         result['fields'] = fields
     if (len(sort)):
         result['sort'] = sort
```

