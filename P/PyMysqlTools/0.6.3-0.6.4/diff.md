# Comparing `tmp/PyMysqlTools-0.6.3.tar.gz` & `tmp/PyMysqlTools-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMysqlTools-0.6.3.tar", last modified: Thu Jul 13 10:02:42 2023, max compression
+gzip compressed data, was "PyMysqlTools-0.6.4.tar", last modified: Fri Jul 14 07:18:38 2023, max compression
```

## Comparing `PyMysqlTools-0.6.3.tar` & `PyMysqlTools-0.6.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 10:02:41.972197 PyMysqlTools-0.6.3/
--rw-rw-rw-   0        0        0     1083 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.3/LICENSE
--rw-rw-rw-   0        0        0      143 2023-02-06 01:25:52.000000 PyMysqlTools-0.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2601 2023-07-13 10:02:41.971223 PyMysqlTools-0.6.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 10:02:41.962233 PyMysqlTools-0.6.3/PyMysqlTools/
--rw-rw-rw-   0        0        0      424 2023-07-13 10:01:02.000000 PyMysqlTools-0.6.3/PyMysqlTools/__init__.py
--rw-rw-rw-   0        0        0      705 2023-07-13 09:00:04.000000 PyMysqlTools-0.6.3/PyMysqlTools/actuator.py
--rw-rw-rw-   0        0        0      431 2023-07-12 02:25:29.000000 PyMysqlTools-0.6.3/PyMysqlTools/exceptions.py
--rw-rw-rw-   0        0        0     6137 2023-07-13 08:59:01.000000 PyMysqlTools-0.6.3/PyMysqlTools/generator.py
--rw-rw-rw-   0        0        0    14535 2023-07-13 08:54:50.000000 PyMysqlTools-0.6.3/PyMysqlTools/main.py
--rw-rw-rw-   0        0        0     3871 2023-07-13 09:58:45.000000 PyMysqlTools-0.6.3/PyMysqlTools/result_set.py
--rw-rw-rw-   0        0        0      624 2023-07-12 02:58:20.000000 PyMysqlTools-0.6.3/PyMysqlTools/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-13 10:02:41.970201 PyMysqlTools-0.6.3/PyMysqlTools.egg-info/
--rw-rw-rw-   0        0        0     2601 2023-07-13 10:02:41.000000 PyMysqlTools-0.6.3/PyMysqlTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-07-13 10:02:41.000000 PyMysqlTools-0.6.3/PyMysqlTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 10:02:41.000000 PyMysqlTools-0.6.3/PyMysqlTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-13 10:02:41.000000 PyMysqlTools-0.6.3/PyMysqlTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-13 10:02:41.000000 PyMysqlTools-0.6.3/PyMysqlTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1998 2023-07-12 09:26:16.000000 PyMysqlTools-0.6.3/README.md
--rw-rw-rw-   0        0        0       50 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 10:02:41.972197 PyMysqlTools-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1359 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:18:38.210449 PyMysqlTools-0.6.4/
+-rw-rw-rw-   0        0        0     1083 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.4/LICENSE
+-rw-rw-rw-   0        0        0      143 2023-02-06 01:25:52.000000 PyMysqlTools-0.6.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2601 2023-07-14 07:18:38.208495 PyMysqlTools-0.6.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 07:18:38.186051 PyMysqlTools-0.6.4/PyMysqlTools/
+-rw-rw-rw-   0        0        0      424 2023-07-14 07:16:39.000000 PyMysqlTools-0.6.4/PyMysqlTools/__init__.py
+-rw-rw-rw-   0        0        0      705 2023-07-13 09:00:04.000000 PyMysqlTools-0.6.4/PyMysqlTools/actuator.py
+-rw-rw-rw-   0        0        0      431 2023-07-12 02:25:29.000000 PyMysqlTools-0.6.4/PyMysqlTools/exceptions.py
+-rw-rw-rw-   0        0        0     6137 2023-07-13 08:59:01.000000 PyMysqlTools-0.6.4/PyMysqlTools/generator.py
+-rw-rw-rw-   0        0        0    14535 2023-07-13 08:54:50.000000 PyMysqlTools-0.6.4/PyMysqlTools/main.py
+-rw-rw-rw-   0        0        0     3560 2023-07-14 07:15:44.000000 PyMysqlTools-0.6.4/PyMysqlTools/result_set.py
+-rw-rw-rw-   0        0        0      624 2023-07-12 02:58:20.000000 PyMysqlTools-0.6.4/PyMysqlTools/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:18:38.207520 PyMysqlTools-0.6.4/PyMysqlTools.egg-info/
+-rw-rw-rw-   0        0        0     2601 2023-07-14 07:18:37.000000 PyMysqlTools-0.6.4/PyMysqlTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-07-14 07:18:37.000000 PyMysqlTools-0.6.4/PyMysqlTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:18:37.000000 PyMysqlTools-0.6.4/PyMysqlTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-14 07:18:37.000000 PyMysqlTools-0.6.4/PyMysqlTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 07:18:37.000000 PyMysqlTools-0.6.4/PyMysqlTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1998 2023-07-12 09:26:16.000000 PyMysqlTools-0.6.4/README.md
+-rw-rw-rw-   0        0        0       50 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 07:18:38.211424 PyMysqlTools-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.4/setup.py
```

### Comparing `PyMysqlTools-0.6.3/LICENSE` & `PyMysqlTools-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.3/PKG-INFO` & `PyMysqlTools-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMysqlTools
-Version: 0.6.3
+Version: 0.6.4
 Summary: A library that makes MySQL operation more convenient.
 Home-page: https://gitee.com/uraurara/PyMysqlTools
 Author: ulala
 Author-email: 2713389652@qq.com
 License: MIT
 Keywords: mysql,client,mysqluitls,PyMysqlTools
 Platform: UNKNOWN
```

### Comparing `PyMysqlTools-0.6.3/PyMysqlTools/actuator.py` & `PyMysqlTools-0.6.4/PyMysqlTools/actuator.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.3/PyMysqlTools/generator.py` & `PyMysqlTools-0.6.4/PyMysqlTools/generator.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.3/PyMysqlTools/main.py` & `PyMysqlTools-0.6.4/PyMysqlTools/main.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.3/PyMysqlTools/result_set.py` & `PyMysqlTools-0.6.4/PyMysqlTools/result_set.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,18 +66,14 @@
 
     def all(self):
         """
         获取结果集, 并将结果集转换为一个方便迭代的结构(List)
 
         :return: List结果集
         """
-        if self._type == list and not isinstance(self._result, list):
-            return [self._result]
-        if self._type == dict:
-            return [self._result]
         return self._result
 
     def get(self, index: int = 0):
         """
         获取特定索引位置的结果
 
         :param index: 索引
@@ -91,16 +87,14 @@
     def limit(self, num: int = 1):
         """
         截取结果集的前n个结果
 
         :param num: 需要截取的结果的数量
         :return: 截取后的结果集
         """
-        if not isinstance(self._result, list):
-            raise ValueError('结果集结构类型不为 `list`, 不支持使用limit')
         if num > 0:
             return self._result[: num]
         else:
             raise ParameterError("'num' 参数的值必须大于 0 ！")
 
     def next(self):
         """
```

### Comparing `PyMysqlTools-0.6.3/PyMysqlTools/settings.py` & `PyMysqlTools-0.6.4/PyMysqlTools/settings.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.3/PyMysqlTools.egg-info/PKG-INFO` & `PyMysqlTools-0.6.4/PyMysqlTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMysqlTools
-Version: 0.6.3
+Version: 0.6.4
 Summary: A library that makes MySQL operation more convenient.
 Home-page: https://gitee.com/uraurara/PyMysqlTools
 Author: ulala
 Author-email: 2713389652@qq.com
 License: MIT
 Keywords: mysql,client,mysqluitls,PyMysqlTools
 Platform: UNKNOWN
```

### Comparing `PyMysqlTools-0.6.3/README.md` & `PyMysqlTools-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.3/setup.py` & `PyMysqlTools-0.6.4/setup.py`

 * *Files identical despite different names*

