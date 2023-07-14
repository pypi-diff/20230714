# Comparing `tmp/pybasekit-0.0.2.tar.gz` & `tmp/pybasekit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybasekit-0.0.2.tar", last modified: Mon Jun 26 19:00:40 2023, max compression
+gzip compressed data, was "pybasekit-1.0.2.tar", last modified: Fri Jul 14 00:47:26 2023, max compression
```

## Comparing `pybasekit-0.0.2.tar` & `pybasekit-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 19:00:40.681315 pybasekit-0.0.2/
--rw-rw-rw-   0        0        0     1083 2023-06-16 18:40:25.000000 pybasekit-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1673 2023-06-26 19:00:40.680314 pybasekit-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1216 2023-06-16 19:11:35.000000 pybasekit-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 19:00:40.670803 pybasekit-0.0.2/pybasekit/
--rw-rw-rw-   0        0        0    12289 2023-06-26 18:56:36.000000 pybasekit-0.0.2/pybasekit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 19:00:40.679313 pybasekit-0.0.2/pybasekit.egg-info/
--rw-rw-rw-   0        0        0     1673 2023-06-26 19:00:40.000000 pybasekit-0.0.2/pybasekit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-06-26 19:00:40.000000 pybasekit-0.0.2/pybasekit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 19:00:40.000000 pybasekit-0.0.2/pybasekit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-26 19:00:40.000000 pybasekit-0.0.2/pybasekit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 19:00:40.681315 pybasekit-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      943 2023-06-26 18:56:45.000000 pybasekit-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 00:47:26.625905 pybasekit-1.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-06-16 18:40:25.000000 pybasekit-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1673 2023-07-14 00:47:26.624905 pybasekit-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1216 2023-06-16 19:11:35.000000 pybasekit-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 00:47:26.612913 pybasekit-1.0.2/pybasekit/
+-rw-rw-rw-   0        0        0    13303 2023-07-14 00:46:47.000000 pybasekit-1.0.2/pybasekit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 00:47:26.622907 pybasekit-1.0.2/pybasekit.egg-info/
+-rw-rw-rw-   0        0        0     1673 2023-07-14 00:47:26.000000 pybasekit-1.0.2/pybasekit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-07-14 00:47:26.000000 pybasekit-1.0.2/pybasekit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 00:47:26.000000 pybasekit-1.0.2/pybasekit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-14 00:47:26.000000 pybasekit-1.0.2/pybasekit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 00:47:26.625905 pybasekit-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      943 2023-07-14 00:46:43.000000 pybasekit-1.0.2/setup.py
```

### Comparing `pybasekit-0.0.2/LICENSE` & `pybasekit-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybasekit-0.0.2/PKG-INFO` & `pybasekit-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybasekit
-Version: 0.0.2
+Version: 1.0.2
 Summary: Basic local database system
 Author: Because
 Author-email: 
 Keywords: python,db,database,storage
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pybasekit-0.0.2/README.md` & `pybasekit-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pybasekit-0.0.2/pybasekit/__init__.py` & `pybasekit-1.0.2/pybasekit/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# Full PybaseKit Code
-import os, random, json
+import os
+import random
+import json
 
 class Encryption:
     '''
-        This is a very simple encryption method not meant to be use outside home project.
-        If used outside home/personal projects use a diffrent method or you will be at risk
+    This is a very simple encryption method not meant to be used outside of home projects.
+    If used outside home/personal projects, use a different method or you will be at risk.
     '''
     @staticmethod
     def encrypt(text):
         encrypted_text = ""
         for c in text:
             block = str(ord(c) * 7719)
             block = "0" * (3 - len(block)) + block
@@ -24,27 +25,29 @@
                 value = int(block) // 7719
                 decrypted_text += chr(value)
         return decrypted_text
 
 
 class Start:
     '''
-      Start class to start the services and hold all the other classes and functions, sets the main folder to hold all database information.
+    Start class to start the services and hold all the other classes and functions,
+    sets the main folder to hold all database information.
     '''
     Folder = "pybase_db"
 
     def __init__(self, folder_name=None):
         if folder_name is not None:
             self.__class__.Folder = folder_name
         if not os.path.exists(self.Folder):
             os.makedirs(self.Folder)
 
     class CreateDB:
         '''
-          User sets a key and class creates a new .pybase file with simple encrypted key and database base information returns 200 OK if runned correctly
+        User sets a key and class creates a new .pybase file with a simple encrypted key
+        and database base information. Returns "200 OK" if run correctly.
         '''
         def __init__(self, name, key):
             self.name = name
 
         def __new__(self, name, key):
             self.__key = key
             if os.path.exists(f"{Start.Folder}/{name}.pybase") == False:
@@ -55,49 +58,50 @@
                 start.write(f"{Encryption.encrypt(self.__key)}\n{build}")
                 return "200 OK"
             else:
                 return "404"
 
     class ConnectDB:
         '''
-          Connects to a .pybase file if access key is correct if not will return 401 if connects returns 200 OK
+        Connects to a .pybase file. Returns "200 OK" if access key is correct,
+        otherwise returns "Failed to connect: 401" or "Failed to connect: 404".
         '''
         def __init__(self, db_name, access_key):
             self.name = db_name
             self.key = access_key
 
         def VerifyAUTH(self):
             '''
-              Verifys thast the user is connected to the .pybase file if authed returns true else returns false. User should not usally use this function its just for the other functions to work correctly
+            Verifies that the user is connected to the .pybase file.
+            Returns True if authenticated, otherwise returns False.
             '''
             if os.path.exists(f"{Start.Folder}/{self.name}.pybase") == True:
                 data = open(f"{Start.Folder}/{self.name}.pybase", "r+")
-                if str(self.key) == str(
-                    Encryption.decrypt(data.readline().strip("\n"))
-                ):
+                if str(self.key) == str(Encryption.decrypt(data.readline().strip("\n"))):
                     return True
                 else:
                     return False
             else:
-                return "404"
+                return False
 
         def __str__(self):
-          # If Authed, connects
+            # If Authed, connects
             AUTH = self.VerifyAUTH()
-            if AUTH == "404":
+            if AUTH == False:
                 return "Failed to connect: 404"
             else:
                 if AUTH == True:
                     return "200 OK"
                 else:
                     return "Failed to connect: 401"
 
         def create_section(self, section_title):
             '''
-              Checked if authed is so creates a new section for the database if section is not already created.
+            Checks if authenticated, then creates a new section for the database
+            if the section is not already created.
             '''
             auth = self.VerifyAUTH()
             if auth == True:
                 lines = []
                 with open(f"{Start.Folder}/{self.name}.pybase") as Data:
                     lines = Data.readlines()[1:]
                     data = Encryption.decrypt(lines[0])
@@ -107,82 +111,86 @@
                         return "Section is already created"
                     else:
                         newValue = {
                             "DatabaseData": {
                                 "SectionTitles": {section_title: section_title}
                             }
                         }
-                        newValue2 = {"Data": {section_title: {}}}
-                        undata.update(newValue)
-                        undata.update(newValue2)
+                        undata["DatabaseData"]["SectionTitles"].update(newValue["DatabaseData"]["SectionTitles"])
+                        undata["Data"].update({section_title: {}})
                         t = open(f"{Start.Folder}/{self.name}.pybase", "w")
-                        undata = Encryption.encrypt(str(undata))
+                        undata = Encryption.encrypt(json.dumps(undata))
                         tt = Encryption.encrypt(self.key)
                         t.write(tt + "\n" + undata)
                         return section_title
             else:
                 return "401"
 
         def insert_data(self, section, Data_Title, Data_Value):
             '''
-              If authed will insert data if data title is not already in section if the section is valid
+            If authenticated, inserts data if data title is not already in the section.
             '''
             AUTH = self.VerifyAUTH()
             if AUTH == True:
                 lines = []
                 with open(f"{Start.Folder}/{self.name}.pybase") as Data:
                     lines = Data.readlines()[1:]
                     data = Encryption.decrypt(lines[0])
                     data = data.replace("'", '"')
                     undata = json.loads(data)
                     if section in undata["DatabaseData"]["SectionTitles"]:
                         if str(Data_Title) not in undata["Data"][str(section)]:
-                            new = {"Data": {section: {Data_Title: Data_Value}}}
-                            undata.update(new)
+                            undata["Data"][str(section)][str(Data_Title)] = Data_Value
                             t = open(f"{Start.Folder}/{self.name}.pybase", "w")
                             t.write(
-                                f"{Encryption.encrypt(self.key)}\n{Encryption.encrypt(str(undata))}"
+                                f"{Encryption.encrypt(self.key)}\n{Encryption.encrypt(json.dumps(undata))}"
                             )
+                            return "200 OK"
                         else:
                             return "Data Title is already in section"
                     else:
                         return "Could not find section: 404"
-                return "200 OK"
             else:
                 return "401"
-            
+
         def insert_list(self, section, Data_Title, List):
+            '''
+            If authenticated, inserts a list into the section if the section exists.
+            '''
             AUTH = self.VerifyAUTH()
             if AUTH:
                 if type(List) == list:
                     lines = []
                     with open(f"{Start.Folder}/{self.name}.pybase") as Data:
                         lines = Data.readlines()[1:]
                         data = Encryption.decrypt(lines[0])
                         data = data.replace("'", '"')
                         undata = json.loads(data)
                         if section in undata["DatabaseData"]["SectionTitles"]:
                             if str(Data_Title) not in undata["Data"][str(section)]:
-                                new = {"Data": {section: {Data_Title: List}}}
-                                undata.update(new)
+                                undata["Data"][str(section)][str(Data_Title)] = List
                                 t = open(f"{Start.Folder}/{self.name}.pybase", "w")
                                 t.write(
-                                    f"{Encryption.encrypt(self.key)}\n{Encryption.encrypt(str(undata))}"
+                                    f"{Encryption.encrypt(self.key)}\n{Encryption.encrypt(json.dumps(undata))}"
                                 )
+                                return "200 OK"
                             else:
                                 return "Data Title is already in section"
                         else:
                             return "Could not find section: 404"
                     return "200 OK"
                 else:
-                    return f"List is not in correct format. Your type is currently at {type(List)}"
+                    return f"List is not in correct format. Your type is currently {type(List)}"
             else:
-                return "Error 401"
-            
+                return "401"
+
         def get_data(self, section, Data_Title):
+            '''
+            If authenticated, retrieves data from the specified section and data title.
+            '''
             AUTH = self.VerifyAUTH()
             if AUTH == True:
                 lines = []
                 with open(f"{Start.Folder}/{self.name}.pybase") as Data:
                     lines = Data.readlines()[1:]
                     data = Encryption.decrypt(lines[0])
                     data = data.replace("'", '"')
@@ -194,82 +202,107 @@
                             return "Could not find data: 404"
                     else:
                         return "Could not find section: 404"
             else:
                 return "401"
 
         def remove_data(self, section, Data_Title):
+            '''
+            If authenticated, removes data from the specified section and data title.
+            '''
             AUTH = self.VerifyAUTH()
             if AUTH == True:
                 lines = []
                 with open(f"{Start.Folder}/{self.name}.pybase") as Data:
                     lines = Data.readlines()[1:]
                     data = Encryption.decrypt(lines[0])
                     data = data.replace("'", '"')
                     undata = json.loads(data)
                     if section in undata["DatabaseData"]["SectionTitles"]:
                         if str(Data_Title) in undata["Data"][str(section)]:
                             del undata["Data"][str(section)][str(Data_Title)]
                             t = open(f"{Start.Folder}/{self.name}.pybase", "w")
                             t.write(
-                                f"{Encryption.encrypt(self.key)}\n{Encryption.encrypt(str(undata))}"
+                                f"{Encryption.encrypt(self.key)}\n{Encryption.encrypt(json.dumps(undata))}"
                             )
                             return "200 OK"
                         else:
                             return "Could not find data: 404"
                     else:
                         return "Could not find section: 404"
             else:
                 return "401"
-        
+
         def update_data_value(self, section, Data_Title, New_Value):
+            '''
+            If authenticated, updates the value of the specified data in the section.
+            '''
             AUTH = self.VerifyAUTH()
             if AUTH == True:
                 lines = []
                 with open(f"{Start.Folder}/{self.name}.pybase") as Data:
                     lines = Data.readlines()[1:]
                     data = Encryption.decrypt(lines[0])
                     data = data.replace("'", '"')
                     undata = json.loads(data)
                     if section in undata["DatabaseData"]["SectionTitles"]:
                         if str(Data_Title) in undata["Data"][str(section)]:
                             undata["Data"][str(section)][str(Data_Title)] = New_Value
                             t = open(f"{Start.Folder}/{self.name}.pybase", "w")
                             t.write(
-                                f"{Encryption.encrypt(self.key)}\n{Encryption.encrypt(str(undata))}"
+                                f"{Encryption.encrypt(self.key)}\n{Encryption.encrypt(json.dumps(undata))}"
                             )
                             return undata["Data"][str(section)][str(Data_Title)]
                         else:
                             return "Could not find data: 404"
                     else:
                         return "Could not find section: 404"
             else:
                 return "401"
-            
+
         def get_all_data(self):
+            '''
+            If authenticated, retrieves all data from the database.
+            '''
             AUTH = self.VerifyAUTH()
             if AUTH == True:
                 lines = []
                 with open(f"{Start.Folder}/{self.name}.pybase") as Data:
                     lines = Data.readlines()[1:]
                     data = Encryption.decrypt(lines[0])
                     data = data.replace("'", '"')
                     undata = json.loads(data)
                     return undata["Data"]
             else:
                 return "401"
 
         def get_section_data(self, section):
+            '''
+            If authenticated, retrieves data from the specified section.
+            '''
             AUTH = self.VerifyAUTH()
             if AUTH == True:
                 lines = []
                 with open(f"{Start.Folder}/{self.name}.pybase") as Data:
                     lines = Data.readlines()[1:]
                     data = Encryption.decrypt(lines[0])
                     data = data.replace("'", '"')
                     undata = json.loads(data)
                     if section in undata["DatabaseData"]["SectionTitles"]:
                         return undata["Data"][str(section)]
                     else:
                         return "Could not find section: 404"
             else:
-                return "401"
+                return "401"
+            
+
+'''
+
+    Once again this is not meant to be used outside personal project as it will put the information in the database you created at risk.
+    If you want to make it secure you can modify the code but with with the current encryption and decryption
+
+    Meant for personal learning and person softwares and thing like that.
+
+
+    Last module update: 7/13/23
+
+'''
```

### Comparing `pybasekit-0.0.2/pybasekit.egg-info/PKG-INFO` & `pybasekit-1.0.2/pybasekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybasekit
-Version: 0.0.2
+Version: 1.0.2
 Summary: Basic local database system
 Author: Because
 Author-email: 
 Keywords: python,db,database,storage
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pybasekit-0.0.2/setup.py` & `pybasekit-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '1.0.2'
 DESCRIPTION = 'Basic local database system'
 LONG_DESCRIPTION = 'A very basic database system for python and personal small projects.'
 
 # Setting up
 setup(
     name="pybasekit",
     version=VERSION,
```

