# Comparing `tmp/launchpy-0.4.2.post1.tar.gz` & `tmp/launchpy-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchpy-0.4.2.post1.tar", last modified: Tue Jul  4 19:29:40 2023, max compression
+gzip compressed data, was "launchpy-0.4.3.tar", last modified: Fri Jul 14 10:53:37 2023, max compression
```

## Comparing `launchpy-0.4.2.post1.tar` & `launchpy-0.4.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 19:29:40.389595 launchpy-0.4.2.post1/
--rw-rw-rw-   0        0        0    35823 2021-10-20 19:49:46.000000 launchpy-0.4.2.post1/LICENSE
--rw-rw-rw-   0        0        0     2300 2023-07-04 19:29:40.382961 launchpy-0.4.2.post1/PKG-INFO
--rw-rw-rw-   0        0        0     1208 2023-06-22 12:01:59.000000 launchpy-0.4.2.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 19:29:40.182381 launchpy-0.4.2.post1/docs/
--rw-rw-rw-   0        0        0     3258 2022-07-13 12:52:02.000000 launchpy-0.4.2.post1/docs/admin.md
--rw-rw-rw-   0        0        0     3892 2021-10-20 19:49:46.000000 launchpy-0.4.2.post1/docs/getstarted.md
--rw-rw-rw-   0        0        0     3727 2021-10-20 19:49:46.000000 launchpy-0.4.2.post1/docs/library.md
--rw-rw-rw-   0        0        0     7521 2021-10-20 19:49:47.000000 launchpy-0.4.2.post1/docs/main.md
--rw-rw-rw-   0        0        0    16546 2023-05-10 18:11:54.000000 launchpy-0.4.2.post1/docs/property.md
--rw-rw-rw-   0        0        0     4657 2023-06-21 19:15:59.000000 launchpy-0.4.2.post1/docs/releases.md
--rw-rw-rw-   0        0        0     8286 2023-05-11 13:25:38.000000 launchpy-0.4.2.post1/docs/synchronizer.md
--rw-rw-rw-   0        0        0     4234 2023-05-10 18:06:32.000000 launchpy-0.4.2.post1/docs/translator.md
-drwxrwxrwx   0        0        0        0 2023-07-04 19:29:40.284768 launchpy-0.4.2.post1/launchpy/
--rw-rw-rw-   0        0        0      268 2022-11-08 13:23:21.000000 launchpy-0.4.2.post1/launchpy/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-04 19:28:41.000000 launchpy-0.4.2.post1/launchpy/__version__.py
--rw-rw-rw-   0        0        0    14165 2023-05-10 17:31:08.000000 launchpy-0.4.2.post1/launchpy/admin.py
--rw-rw-rw-   0        0        0      810 2023-06-21 19:22:23.000000 launchpy-0.4.2.post1/launchpy/config.py
--rw-rw-rw-   0        0        0     8022 2023-07-04 14:32:35.000000 launchpy-0.4.2.post1/launchpy/configs.py
--rw-rw-rw-   0        0        0    13613 2023-06-22 11:00:34.000000 launchpy-0.4.2.post1/launchpy/connector.py
--rw-rw-rw-   0        0        0    29268 2023-05-10 17:31:00.000000 launchpy-0.4.2.post1/launchpy/launchpy.py
--rw-rw-rw-   0        0        0    16796 2023-05-10 17:30:51.000000 launchpy-0.4.2.post1/launchpy/library.py
--rw-rw-rw-   0        0        0    74941 2023-05-10 17:30:38.000000 launchpy-0.4.2.post1/launchpy/property.py
--rw-rw-rw-   0        0        0    25209 2023-05-11 12:16:25.000000 launchpy-0.4.2.post1/launchpy/synchronizer.py
-drwxrwxrwx   0        0        0        0 2023-07-04 19:29:40.368764 launchpy-0.4.2.post1/launchpy.egg-info/
--rw-rw-rw-   0        0        0     2300 2023-07-04 19:29:39.000000 launchpy-0.4.2.post1/launchpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      564 2023-07-04 19:29:40.000000 launchpy-0.4.2.post1/launchpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 19:29:39.000000 launchpy-0.4.2.post1/launchpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-07-04 19:29:39.000000 launchpy-0.4.2.post1/launchpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 19:29:39.000000 launchpy-0.4.2.post1/launchpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1361 2023-06-22 12:02:18.000000 launchpy-0.4.2.post1/pyproject.toml
--rw-rw-rw-   0        0        0      101 2021-10-20 19:49:47.000000 launchpy-0.4.2.post1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 19:29:40.390114 launchpy-0.4.2.post1/setup.cfg
--rw-rw-rw-   0        0        0     1754 2021-10-20 19:49:47.000000 launchpy-0.4.2.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:53:37.585252 launchpy-0.4.3/
+-rw-rw-rw-   0        0        0    35823 2021-10-20 19:49:46.000000 launchpy-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0     2294 2023-07-14 10:53:37.585252 launchpy-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1208 2023-06-22 12:01:59.000000 launchpy-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 10:53:37.501665 launchpy-0.4.3/docs/
+-rw-rw-rw-   0        0        0     3258 2022-07-13 12:52:02.000000 launchpy-0.4.3/docs/admin.md
+-rw-rw-rw-   0        0        0     3892 2021-10-20 19:49:46.000000 launchpy-0.4.3/docs/getstarted.md
+-rw-rw-rw-   0        0        0     3727 2021-10-20 19:49:46.000000 launchpy-0.4.3/docs/library.md
+-rw-rw-rw-   0        0        0     7521 2021-10-20 19:49:47.000000 launchpy-0.4.3/docs/main.md
+-rw-rw-rw-   0        0        0    16546 2023-05-10 18:11:54.000000 launchpy-0.4.3/docs/property.md
+-rw-rw-rw-   0        0        0     4733 2023-07-11 06:50:50.000000 launchpy-0.4.3/docs/releases.md
+-rw-rw-rw-   0        0        0     8286 2023-05-11 13:25:38.000000 launchpy-0.4.3/docs/synchronizer.md
+-rw-rw-rw-   0        0        0     4162 2023-07-13 21:17:14.000000 launchpy-0.4.3/docs/translator.md
+drwxrwxrwx   0        0        0        0 2023-07-14 10:53:37.564157 launchpy-0.4.3/launchpy/
+-rw-rw-rw-   0        0        0      268 2022-11-08 13:23:21.000000 launchpy-0.4.3/launchpy/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-07-11 06:50:13.000000 launchpy-0.4.3/launchpy/__version__.py
+-rw-rw-rw-   0        0        0    14165 2023-05-10 17:31:08.000000 launchpy-0.4.3/launchpy/admin.py
+-rw-rw-rw-   0        0        0      810 2023-06-21 19:22:23.000000 launchpy-0.4.3/launchpy/config.py
+-rw-rw-rw-   0        0        0     8022 2023-07-04 14:32:35.000000 launchpy-0.4.3/launchpy/configs.py
+-rw-rw-rw-   0        0        0    13613 2023-06-22 11:00:34.000000 launchpy-0.4.3/launchpy/connector.py
+-rw-rw-rw-   0        0        0    28452 2023-07-14 06:45:39.000000 launchpy-0.4.3/launchpy/launchpy.py
+-rw-rw-rw-   0        0        0    16796 2023-05-10 17:30:51.000000 launchpy-0.4.3/launchpy/library.py
+-rw-rw-rw-   0        0        0    69778 2023-07-14 06:45:48.000000 launchpy-0.4.3/launchpy/property.py
+-rw-rw-rw-   0        0        0    25220 2023-07-13 21:38:36.000000 launchpy-0.4.3/launchpy/synchronizer.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:53:37.585252 launchpy-0.4.3/launchpy.egg-info/
+-rw-rw-rw-   0        0        0     2294 2023-07-14 10:53:37.000000 launchpy-0.4.3/launchpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      564 2023-07-14 10:53:37.000000 launchpy-0.4.3/launchpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 10:53:37.000000 launchpy-0.4.3/launchpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-07-14 10:53:37.000000 launchpy-0.4.3/launchpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 10:53:37.000000 launchpy-0.4.3/launchpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1361 2023-06-22 12:02:18.000000 launchpy-0.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-07-14 06:45:53.000000 launchpy-0.4.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 10:53:37.585252 launchpy-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1744 2023-07-14 06:46:12.000000 launchpy-0.4.3/setup.py
```

### Comparing `launchpy-0.4.2.post1/LICENSE` & `launchpy-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/PKG-INFO` & `launchpy-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchpy
-Version: 0.4.2.post1
+Version: 0.4.3
 Summary: Adobe Launch API wrapper
 Home-page: https://github.com/pitchmuc/launchpy
 Author: Julien Piccini
 Author-email: Julien Piccini <piccini.julien@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/pitchmuc/launchpy
 Project-URL: changelog, https://github.com/pitchmuc/launchpy/blob/master/docs/releases.md
```

### Comparing `launchpy-0.4.2.post1/README.md` & `launchpy-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/docs/admin.md` & `launchpy-0.4.3/docs/admin.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/docs/getstarted.md` & `launchpy-0.4.3/docs/getstarted.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/docs/library.md` & `launchpy-0.4.3/docs/library.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/docs/main.md` & `launchpy-0.4.3/docs/main.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/docs/property.md` & `launchpy-0.4.3/docs/property.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/docs/releases.md` & `launchpy-0.4.3/docs/releases.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Release for launchpy
 
 This page gathered the changes made between version of the launchpy module.\
 This has been started after the 0.3.0 release.\
 
+## 0.4.3
+* Refactor `Translator` class for removing `pandas` dependency
+
 ## 0.4.2
 * Supporting the Oauth Token V2 authentication
 
 ### 0.4.1
 * single component methods (getDataElement, getRule) will now return the definition directly and avoid that you need to access the `data` attibute.
 * introducing the `updateDataElementCode` method that update directly the code from a custom code data element based on the stringify code passed.
 * provide a possible configuration for Synchronizer via a Data Element name. (Link)[./synchronizer.md#dynamic-component-filter]
```

### Comparing `launchpy-0.4.2.post1/docs/synchronizer.md` & `launchpy-0.4.3/docs/synchronizer.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/docs/translator.md` & `launchpy-0.4.3/docs/translator.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 However, we can clearly imaigne that this methods can help you automate some copy paste.
 Also it is possible to use it not only between 2 properties but between 2 Organizations.
 
 ## Starting with translator class
 
 The instantiation of the translator class is very basic as you would just need to call for it.
-What is really required is the base property extensions and rules. The id of the elements from your “mother” property.
+What is really required is the base property extensions and rules. The id of the elements from your "mother" property.
 This is an assumption that I have when I created this facilitator, you would have a blueprint that you will use to copy elements from.
 The translator class provide 2 methods to add base rule and base extension ids:
 
 * **setBaseExtensions** : Pass all the extensions from the base property to start building the table. 
   Arguments: 
   * base_property : REQUIRED : list of all extensions retrieve through getExtensions method
   * property_name : REQUIRED : name of your base property.
@@ -21,15 +21,15 @@
 * **setBaseRules**: Pass all the rules from the base property to start building the table. 
   Arguments: 
   * base_property : REQUIRED : list of all rules retrieve through getExtensions method
   * property_name : REQUIRED : name of your base property.
 
 ## Set Target Rule and Extensions ids
 
-Once you have loaded the base Extension and Rules ids, the method will start to expand the table into multiple columns for matching. Underlying is the use of pandas dataframe to realize that matching.
+Once you have loaded the base Extension and Rules ids, the method will start to expand the table into multiple columns for matching.
 You will need to be consistent with the naming of your target in order for the method to work properly.
 The methods that allow extension of your table are the following:
 
 * extendExtensions:
   * new_property_extensions : REQUIRED : the extension list from your target property.
   * new_prop_name : REQUIRED : target property name.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `launchpy-0.4.2.post1/launchpy/admin.py` & `launchpy-0.4.3/launchpy/admin.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/launchpy/config.py` & `launchpy-0.4.3/launchpy/config.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/launchpy/configs.py` & `launchpy-0.4.3/launchpy/configs.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/launchpy/connector.py` & `launchpy-0.4.3/launchpy/connector.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/launchpy/launchpy.py` & `launchpy-0.4.3/launchpy/launchpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 from collections import defaultdict
 from copy import deepcopy
 # Non standard libraries
-import pandas as pd
 from pathlib import Path
 from typing import IO, Union
 from .configs import saveFile
 
 def extensionsInfo(data: list)->dict:
     """
     Return a dictionary from the list provided from the extensions request.
@@ -406,92 +405,78 @@
     --> You can use the translate method to translate Data Element settings 
     3. setBaseRules
     4. extendRules
     --> You can use the translate method to translate Rule Components settings 
     """
 
     def __init__(self):
-        self.rules = pd.DataFrame()
-        self.extensions = pd.DataFrame()
+        self.rules = {}
+        self.baseRuleIdName = {}
+        self.extensions = {}
+        self.baseExtensionIdName = {}
 
-    def setBaseExtensions(self, extensions: list=None, property_name: str=None)->None:
+    def setBaseExtensions(self, base_property_extensions: list, property_name: str):
         """
         Pass all the extensions from the base property to start building the table. 
         Arguments: 
-            extensions_base : REQUIRED : list of all extensions retrieve through getExtensions method
+            base_property_extensions : REQUIRED : list of all extensions retrieve through getExtensions method
             property_name : REQUIRED : name of your base property.
         """
-        if extensions is None or type(extensions)!= list:
-            raise ValueError("Require a list of extensions to be loaded")
-        if property_name is None:
-            raise ValueError("Require the main property name")
-        df = pd.DataFrame(extensionsInfo(extensions)).T
-        df = pd.DataFrame(df['id'])
-        df.columns = [property_name]
-        self.extensions = df
+        self.baseExtensionIdName = {ext['id'] : ext['attributes']['name'] for ext in base_property_extensions}
+        self.extensions = {ext['attributes']['name']:{property_name:ext['id']} for ext in base_property_extensions}
 
-    def extendExtensions(self, extensions: list=None, property_name: str=None)-> None:
+    def extendExtensions(self, new_property_extensions: list, new_prop_name: str)-> None:
         """
         Add the extensions id from a target property.
         Arguments: 
-            extensions: REQUIRED : the extension list from your target property. 
-            property_name : REQUIRED : target property name. 
+            new_property_extensions: REQUIRED : the extension list from your target property. 
+            new_prop_name : REQUIRED : target property name. 
         """
-        if extensions is None or type(extensions)!= list:
-            raise ValueError("Require a list of extensions to be loaded")
-        if property_name is None:
-            raise ValueError("Require the main property name")
-        df = pd.DataFrame(extensionsInfo(extensions)).T
-        df = pd.DataFrame(df['id'])
-        self.extensions[property_name] = df
+        for ext in new_property_extensions:
+            if ext['attributes']['name'] in list(self.extensions.keys()):
+                self.extensions[ext['attributes']['name']][new_prop_name] = ext['id']
         return self.extensions
 
-    def setBaseRules(self, rules: list=None, property_name: str=None)->None:
+    def setBaseRules(self, base_property_rules: list, property_name: str):
         """
         Pass all the rules from the base property to start building the table. 
         Arguments: 
-            rules : REQUIRED : list of all rules retrieve through getExtensions method
+            base_property : REQUIRED : list of all rules retrieve through getExtensions method
             property_name : REQUIRED : name of your base property.
         """
-        if rules is None or type(rules)!= list:
-            raise ValueError("Require a list of rules to be loaded")
-        if property_name is None:
-            raise ValueError("Require the main property name")
-        df = pd.DataFrame(rulesInfo(rules)).T
-        df = pd.DataFrame(df['id'])
-        df.columns = [property_name]
-        self.rules = df
+        self.baseRuleIdName = {rule['id']:rule['attributes']['name'] for rule in base_property_rules}
+        self.rules = {rule['attributes']['name']:{property_name:rule['id']} for rule in base_property_rules}
     
     def extendBaseRules(self,ruleName:str=None,ruleId:str=None,property_name: str=None)->None:
         """
         Add a new rule name in the translator mapping table.
         In case you have created the rule after instantiation of the Translator.
         Arguments:
             ruleName : REQUIRED : the name of the rule to create
             ruleId : REQUIRED : The ID of the rule to create
             property_name : REQUIRED : The base property used.
         """
         if ruleName is None:
             raise ValueError("Require a rule name to be loaded")
         if property_name is None:
             raise ValueError("Require the main property name")
-        temp_df = pd.DataFrame.from_dict({property_name:{ruleName:ruleId}})
-        self.rules = self.rules.append(temp_df)
+        self.baseRuleIdName[ruleId] = ruleName
+        self.rules[ruleName][property_name] = ruleId
         
 
-    def extendRules(self, rules: list=None, property_name: str=None):
+    def extendRules(self, new_property_rules: list, new_prop_name: str):
         """
-        Add the rule id from a target property.
+        Add the extensions id from a target property.
         Arguments: 
-            rules: REQUIRED : the rules list from your target property. 
-            property_name : REQUIRED : target property name. 
+            new_property_rules: REQUIRED : the rules list from your target property. 
+            new_prop_name : REQUIRED : target property name. 
         """
-        df = pd.DataFrame(rulesInfo(rules)).T
-        df = pd.DataFrame(df['id'])
-        self.rules[property_name] = df
+        for rule in new_property_rules:
+            if rule['attributes']['name'] in list(self.rules.keys()):
+                self.rules[rule['attributes']['name']][new_prop_name] = rule['id']
         return self.rules
     
     def extendTargetRules(self,ruleName:str=None,ruleId:str=None,property_name: str=None)->None:
         """
         Add a new rule name in the translator mapping table for the target property.
         In case you have created the rule after instantiation of the Translator.
         If the rule name is not present in the base property, the update will not happen.
@@ -500,59 +485,51 @@
             ruleId : REQUIRED : The ID of the rule to create
             property_name : REQUIRED : The base property used.
         """
         if ruleName is None:
             raise ValueError("Require a rule name to be loaded")
         if property_name is None:
             raise ValueError("Require the main property name")
-        temp_df = pd.DataFrame.from_dict({property_name:{ruleName:ruleId}})
-        self.rules.update(temp_df)
+        self.rules[ruleName][property_name] = ruleId
 
-    def translate(self, target_property: str=None, data_element: dict = None, rule_component: dict = None)->dict:
+    def translate(self, target_property: str, data_element: dict = None, rule_component: dict = None)->dict:
         """
         change the id from the base element to the new property. 
         Pre checked should be done beforehands (updating Extension & Rules elements)
         Arguments: 
             target_property : REQUIRED : property that is targeted to translate the element to
             data_element : OPTIONAL : if the elements passed are data elements
             rule_component : OPTIONAL : if the elements passed are rule components
         """
-        if target_property is None:
-            raise ValueError("Require the target property name")
-        if data_element is None and rule_component is None:
-            raise AttributeError("Require at least data element or rule component to be passed")
-        if self.extensions.empty == True:
+        if len(self.extensions) == 0:
             raise AttributeError(
                 "You didn't import the base extensions or the target extensions")
         if data_element is not None:
             new_de = deepcopy(data_element)
             base_id = new_de['extension']['id']
-            row = self.extensions[self.extensions.iloc[:, 0]
-                                  == base_id].index.values[0]
-            new_value = self.extensions.loc[row, target_property]
-            new_de['extension']['id'] = new_value
+            based_ext_name = self.baseExtensionIdName[base_id]
+            new_extension_id = self.extensions[based_ext_name][target_property]
+            new_de['extension']['id'] = new_extension_id
             return new_de
         elif rule_component is not None:
-            if self.rules.empty == True:
+            if len(self.rules) == 0:
                 raise AttributeError(
                     "The rules have not been imported, the rule id needs to be changed")
             new_rc = deepcopy(rule_component)
             base_id = new_rc['extension']['id']
-            row = self.extensions[self.extensions.eq(
-                base_id).any(1)].index.values[0]
-            new_value = self.extensions.loc[row, target_property]
-            new_rc['extension']['id'] = new_value
-            if self.rules.empty == False:
+            based_ext_name = self.baseExtensionIdName[base_id]
+            new_extension_id = self.extensions[based_ext_name][target_property]
+            new_rc['extension']['id'] = new_extension_id
+            if len(self.rules) > 0:
                 new_rc['rule_setting'] = {
                     'data': [{
-                        'id': self.rules.loc[rule_component['rule_name'], target_property],
+                        'id': self.rules[rule_component['rule_name']][target_property],
                         'type':'rules'}
                     ]}
-                new_rc['rule_id'] = self.rules.loc[rule_component['rule_name'],
-                                                   target_property]
+                new_rc['rule_id'] = self.rules[rule_component['rule_name']][target_property]
             else:
                 print(
                     "You didn't load the rules. Please use setExtensions and setRules, and extendExtensions and extendRules")
                 del new_rc['rules']
             return new_rc
```

### Comparing `launchpy-0.4.2.post1/launchpy/library.py` & `launchpy-0.4.3/launchpy/library.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/launchpy/property.py` & `launchpy-0.4.3/launchpy/property.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 from collections import defaultdict
 from concurrent import futures
 from copy import deepcopy
 # Non standard libraries
-import pandas as pd
 from launchpy import config, connector
 from typing import IO, Union
 from .library import Library
 from .configs import saveFile
 
 class Property:
     """
@@ -1488,126 +1487,14 @@
             'data': [{
                 'id': data['rule_id'],
                 'type':'rules'}
             ]}
     return obj
 
 
-class Translator:
-    """
-    A class to store the translator dataframe for extensions ids. 
-    It has multiple methods, you should set the Extensions and the Rules. 
-    1. setBaseExtensions
-    2. extendExtensions
-    --> You can use the translate method to translate Data Element settings 
-    3. setBaseRules
-    4. extendRules
-    --> You can use the translate method to translate Rule Components settings 
-    """
-
-    def __init__(self):
-        self.rules = pd.DataFrame()
-        self.extensions = pd.DataFrame()
-
-    def setBaseExtensions(self, base_property_extensions: object, property_name: str):
-        """
-        Pass all the extensions from the base property to start building the table. 
-        Arguments: 
-            base_property : REQUIRED : list of all extensions retrieve through getExtensions method
-            property_name : REQUIRED : name of your base property.
-        """
-        df = pd.DataFrame(extensionsInfo(base_property_extensions)).T
-        df = pd.DataFrame(df['id'])
-        df.columns = [property_name]
-        self.extensions = df
-
-    def extendExtensions(self, new_property_extensions: object, new_prop_name: str)-> None:
-        """
-        Add the extensions id from a target property.
-        Arguments: 
-            new_property_extensions: REQUIRED : the extension list from your target property. 
-            new_prop_name : REQUIRED : target property name. 
-        """
-        df = pd.DataFrame(extensionsInfo(new_property_extensions)).T
-        df = pd.DataFrame(df['id'])
-        self.extensions[new_prop_name] = df
-        return self.extensions
-
-    def setBaseRules(self, base_property_rules: object, property_name: str):
-        """
-        Pass all the rules from the base property to start building the table. 
-        Arguments: 
-            base_property : REQUIRED : list of all rules retrieve through getExtensions method
-            property_name : REQUIRED : name of your base property.
-        """
-        df = pd.DataFrame(rulesInfo(base_property_rules)).T
-        df = pd.DataFrame(df['id'])
-        df.columns = [property_name]
-        self.rules = df
-
-    def extendRules(self, new_property_rules: object, new_prop_name: str):
-        """
-        Add the extensions id from a target property.
-        Arguments: 
-            new_property_rules: REQUIRED : the rules list from your target property. 
-            new_prop_name : REQUIRED : target property name. 
-        """
-        df = pd.DataFrame(rulesInfo(new_property_rules)).T
-        df = pd.DataFrame(df['id'])
-        self.rules[new_prop_name] = df
-        return self.rules
-
-    def translate(self, target_property: str, data_element: dict = None, rule_component: dict = None)->dict:
-        """
-        change the id from the base element to the new property. 
-        Pre checked should be done beforehands (updating Extension & Rules elements)
-        Arguments: 
-            target_property : REQUIRED : property that is targeted to translate the element to
-            data_element : OPTIONAL : if the elements passed are data elements
-            rule_component : OPTIONAL : if the elements passed are rule components
-        """
-        if self.extensions.empty == True:
-            raise AttributeError(
-                "You didn't import the base extensions or the target extensions")
-        if data_element is not None:
-            new_de = deepcopy(data_element)
-            base_id = new_de['extension']['id']
-            row = self.extensions[self.extensions.iloc[:, 0]
-                                  == base_id].index.values[0]
-            new_value = self.extensions.loc[row, target_property]
-            new_de['extension']['id'] = new_value
-            return new_de
-        elif rule_component is not None:
-            if self.rules.empty == True:
-                print(
-                    "The rules have not been imported, the rule id needs to be changed")
-            new_rc = deepcopy(rule_component)
-            base_id = new_rc['extension']['id']
-            row = self.extensions[self.extensions.eq(
-                base_id).any(1)].index.values[0]
-            new_value = self.extensions.loc[row, target_property]
-            # print(f"name : {rule_component['rule_name']}")
-            # print(f"old_id : {base_id}")
-            # print(f"new_id : {new_value}")
-            new_rc['extension']['id'] = new_value
-            if self.rules.empty == False:
-                new_rc['rule_setting'] = {
-                    'data': [{
-                        'id': self.rules.loc[rule_component['rule_name'], target_property],
-                        'type':'rules'}
-                    ]}
-                new_rc['rule_id'] = self.rules.loc[rule_component['rule_name'],
-                                                   target_property]
-            else:
-                print(
-                    "You didn't load the rules. Please use setExtensions and setRules, and extendExtensions and extendRules")
-                del new_rc['rules']
-            return new_rc
-
-
 def extractAnalyticsCode(rcSettings: str, save: bool = False, filename: str = None,encoding:str='utf-8')->None:
     """
     Extract the custom code of the rule and save it in a file.
     Arguments:
         rcSettings: REQUIRED : it is the analytics rule component settings retrieved by the extractSettings method. 
         save : OPTIONAL : if you want to save the code as external js file. UTF-16. Default False. 
         filename : OPTIONAL : name of the file you want to use to save the code.
```

### Comparing `launchpy-0.4.2.post1/launchpy/synchronizer.py` & `launchpy-0.4.3/launchpy/synchronizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                 if len(self.target_configs.get(target,{}).get('inclComponents',[]))>0:
                     if any([bool(re.search(key,cmp_baseDict['name'])) for key in self.target_configs.get(target,{}).get('inclComponents',[])]):
                         flagAllowList = True
                 ## if there is no allow list for that property, or no match in the list of target properties, or component was allow
                 if len(self.target_configs.get(target,{}).get('inclComponents',[]))==0 or flagAllowList:
                     translatedComponent = self.translator.translate(target,data_element=cmp_baseDict['copy'])
                     ## if it does not exist
-                    if cmp_baseDict['name'] not in [de['attributes']['name'] for de in self.targets[target]['dataElements']]:
+                    if cmp_baseDict['name'] not in [de.get('attributes',{}).get('name') for de in self.targets[target]['dataElements']]:
                         comp = self.targets[target]['api'].createDataElement(
                             name=cmp_baseDict['name'],
                             descriptor= translatedComponent['descriptor'],
                             settings=translatedComponent['settings'],
                             extension=translatedComponent['extension'],
                             storage_duration = translatedComponent["storage_duration"],
                             force_lower_case = translatedComponent["force_lower_case"],
```

### Comparing `launchpy-0.4.2.post1/launchpy.egg-info/PKG-INFO` & `launchpy-0.4.3/launchpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchpy
-Version: 0.4.2.post1
+Version: 0.4.3
 Summary: Adobe Launch API wrapper
 Home-page: https://github.com/pitchmuc/launchpy
 Author: Julien Piccini
 Author-email: Julien Piccini <piccini.julien@gmail.com>
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/pitchmuc/launchpy
 Project-URL: changelog, https://github.com/pitchmuc/launchpy/blob/master/docs/releases.md
```

### Comparing `launchpy-0.4.2.post1/launchpy.egg-info/SOURCES.txt` & `launchpy-0.4.3/launchpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/pyproject.toml` & `launchpy-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.2.post1/setup.py` & `launchpy-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,10 +39,10 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Topic :: Utilities",
         "Topic :: Internet",
         "Topic :: Software Development :: Libraries",
         "Development Status :: 4 - Beta"
     ],
     python_requires='>=3.7',
-    install_requires=['pandas', "requests",
+    install_requires=["requests",
                       "PyJWT", "pathlib2", "pathlib", "PyJWT[crypto]"],
 )
```

