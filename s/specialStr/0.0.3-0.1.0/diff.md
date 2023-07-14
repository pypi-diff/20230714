# Comparing `tmp/specialStr-0.0.3.tar.gz` & `tmp/specialStr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specialStr-0.0.3.tar", last modified: Sun Jun 25 16:34:23 2023, max compression
+gzip compressed data, was "specialStr-0.1.0.tar", last modified: Fri Jul 14 15:15:38 2023, max compression
```

## Comparing `specialStr-0.0.3.tar` & `specialStr-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 16:34:23.926436 specialStr-0.0.3/
--rw-rw-rw-   0        0        0     1170 2023-06-25 16:34:23.926436 specialStr-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      458 2023-06-25 16:32:05.000000 specialStr-0.0.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-25 16:34:23.926436 specialStr-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1041 2023-06-25 16:33:52.000000 specialStr-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 16:34:23.919437 specialStr-0.0.3/specialStr/
--rw-rw-rw-   0        0        0      537 2023-06-11 05:30:11.000000 specialStr-0.0.3/specialStr/__init__.py
--rw-rw-rw-   0        0        0     2494 2023-06-25 16:10:29.000000 specialStr-0.0.3/specialStr/checker.py
--rw-rw-rw-   0        0        0     6770 2023-06-25 16:10:04.000000 specialStr-0.0.3/specialStr/main.py
-drwxrwxrwx   0        0        0        0 2023-06-25 16:34:23.925435 specialStr-0.0.3/specialStr.egg-info/
--rw-rw-rw-   0        0        0     1170 2023-06-25 16:34:23.000000 specialStr-0.0.3/specialStr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-06-25 16:34:23.000000 specialStr-0.0.3/specialStr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 16:34:23.000000 specialStr-0.0.3/specialStr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-25 16:34:23.000000 specialStr-0.0.3/specialStr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-25 16:34:23.000000 specialStr-0.0.3/specialStr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 15:15:38.471708 specialStr-0.1.0/
+-rw-rw-rw-   0        0        0     1170 2023-07-14 15:15:38.470709 specialStr-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2023-06-25 16:32:05.000000 specialStr-0.1.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-14 15:15:38.472708 specialStr-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2023-07-14 15:15:09.000000 specialStr-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:15:38.380262 specialStr-0.1.0/specialStr/
+-rw-rw-rw-   0        0        0      537 2023-06-11 05:30:11.000000 specialStr-0.1.0/specialStr/__init__.py
+-rw-rw-rw-   0        0        0     2494 2023-07-14 15:08:09.000000 specialStr-0.1.0/specialStr/checker.py
+-rw-rw-rw-   0        0        0     7113 2023-07-14 15:14:49.000000 specialStr-0.1.0/specialStr/main.py
+drwxrwxrwx   0        0        0        0 2023-07-14 15:15:38.468707 specialStr-0.1.0/specialStr.egg-info/
+-rw-rw-rw-   0        0        0     1170 2023-07-14 15:15:38.000000 specialStr-0.1.0/specialStr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-07-14 15:15:38.000000 specialStr-0.1.0/specialStr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 15:15:38.000000 specialStr-0.1.0/specialStr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-14 15:15:38.000000 specialStr-0.1.0/specialStr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 15:15:38.000000 specialStr-0.1.0/specialStr.egg-info/top_level.txt
```

### Comparing `specialStr-0.0.3/PKG-INFO` & `specialStr-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specialStr
-Version: 0.0.3
+Version: 0.1.0
 Summary: Manage strings more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: string
 Platform: windows
```

### Comparing `specialStr-0.0.3/setup.py` & `specialStr-0.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 setup(
     name = 'specialStr',
-    version = '0.0.3',
+    version = '0.1.0',
     keywords = ['string'],
     description = 'Manage strings more easily',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/do-folder/",
     install_requires = [
```

### Comparing `specialStr-0.0.3/specialStr/__init__.py` & `specialStr-0.1.0/specialStr/__init__.py`

 * *Files identical despite different names*

### Comparing `specialStr-0.0.3/specialStr/checker.py` & `specialStr-0.1.0/specialStr/checker.py`

 * *Files identical despite different names*

### Comparing `specialStr-0.0.3/specialStr/main.py` & `specialStr-0.1.0/specialStr/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
 MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
 See the Mulan PSL v2 for more details.
 """
 import os
 from .checker import *
 from typing import Any, Dict,List,Union,Tuple,Union
-from typing_extensions import Literal
+from typing_extensions import Literal, SupportsIndex
 import copy
 __all__=["Url","Path","Email","Version"]
 class SpecialStr(str):
     checker=Checker() #type: Checker
     def __new__(cls, value):
         var=str(value)
         if not all([i.match(var)!=None for i in cls.checker.tester]):
@@ -27,14 +27,22 @@
                 if name in i:
                     values=self.checker.finder[i].findall(self)[0] #type: Union[Tuple[str,...],str]
                     if type(values)==str:
                         return values
                     if type(values)==tuple:
                         return values[i.index(name)]
         return super().__getattribute__(name)
+    def __getitem__(self, __key: Any) -> str:
+        try:
+            return super().__getitem__(__key)
+        except:
+            try:
+                return self.__getattribute__(__key)
+            except:
+                raise NameError("No such attribute or index: %s"%__key)
 class Url(SpecialStr):
     """
     ## This class represents a URL and inherits from the SpecialStr class.
     ### Attributes:
         - checker (UrlChecker): An instance of the UrlChecker class used to validate URLs.
         - shame (str): A string representing any shameful content associated with the URL.
         - domain (str): The domain name of the URL.
@@ -74,18 +82,18 @@
     def __new__(cls, value):
         var=str(value)
         if var.startswith("."):
             var=os.path.abspath(var)
         var=var.replace("\\","/")
         return super().__new__(cls,var)
     @property
-    def partition(self)->List[str]:
+    def partition(self,removeEmpty:bool=True)->List[str]:
         """split the path into list"""
         li=self.path.split("/")
-        while "" in li:
+        while "" in li and removeEmpty:
             li.remove("")
         return li
     @property
     def name(self)->str:
         """The name of the path points to"""
         return self.partition[-1] if len(self.partition) else self.driver+"/"
     def add(self, value:str):
```

### Comparing `specialStr-0.0.3/specialStr.egg-info/PKG-INFO` & `specialStr-0.1.0/specialStr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specialStr
-Version: 0.0.3
+Version: 0.1.0
 Summary: Manage strings more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: string
 Platform: windows
```

