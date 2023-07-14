# Comparing `tmp/LogTranslate-1.2.3.tar.gz` & `tmp/LogTranslate-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogTranslate-1.2.3.tar", last modified: Thu Jul  6 17:16:38 2023, max compression
+gzip compressed data, was "LogTranslate-1.2.6.tar", last modified: Fri Jul 14 13:53:50 2023, max compression
```

## Comparing `LogTranslate-1.2.3.tar` & `LogTranslate-1.2.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 17:16:38.083648 LogTranslate-1.2.3/
--rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 17:16:38.072684 LogTranslate-1.2.3/LogTranslate.egg-info/
--rw-rw-rw-   0        0        0     3183 2023-07-06 17:16:37.000000 LogTranslate-1.2.3/LogTranslate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2023-07-06 17:16:38.000000 LogTranslate-1.2.3/LogTranslate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 17:16:37.000000 LogTranslate-1.2.3/LogTranslate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-06 17:16:37.000000 LogTranslate-1.2.3/LogTranslate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-06 17:16:37.000000 LogTranslate-1.2.3/LogTranslate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3183 2023-07-06 17:16:38.082652 LogTranslate-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 17:16:38.077667 LogTranslate-1.2.3/log_translate/
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 17:16:38.080659 LogTranslate-1.2.3/log_translate/business/
--rw-rw-rw-   0        0        0      618 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/business/AndroidCrashPattern_translator.py
--rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/business/__init__.py
--rw-rw-rw-   0        0        0     3893 2023-06-30 11:21:05.000000 LogTranslate-1.2.3/log_translate/business/bluetooth_translator.py
--rw-rw-rw-   0        0        0      329 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/config_default.py
--rw-rw-rw-   0        0        0     1349 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/data_struct.py
--rw-rw-rw-   0        0        0       11 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/gloable.py
--rw-rw-rw-   0        0        0     4448 2023-07-03 13:31:40.000000 LogTranslate-1.2.3/log_translate/log_translator.py
--rw-rw-rw-   0        0        0     3162 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/read_log_file.py
-drwxrwxrwx   0        0        0        0 2023-07-06 17:16:38.081656 LogTranslate-1.2.3/log_translate/res/
--rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/log_translate/res/log_logo.ico
--rw-rw-rw-   0        0        0     7561 2023-07-06 17:13:36.000000 LogTranslate-1.2.3/log_translate/ui_pyqt6.py
--rw-rw-rw-   0        0        0     7491 2023-07-06 17:14:47.000000 LogTranslate-1.2.3/log_translate/ui_pyside2.py
--rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 17:16:38.083648 LogTranslate-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     2199 2023-07-06 17:16:35.000000 LogTranslate-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:50.806163 LogTranslate-1.2.6/
+-rw-rw-rw-   0        0        0     1079 2023-06-28 15:23:37.000000 LogTranslate-1.2.6/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:50.791569 LogTranslate-1.2.6/LogTranslate.egg-info/
+-rw-rw-rw-   0        0        0     3183 2023-07-14 13:53:50.000000 LogTranslate-1.2.6/LogTranslate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-07-14 13:53:50.000000 LogTranslate-1.2.6/LogTranslate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 13:53:50.000000 LogTranslate-1.2.6/LogTranslate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-14 13:53:50.000000 LogTranslate-1.2.6/LogTranslate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-14 13:53:50.000000 LogTranslate-1.2.6/LogTranslate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3183 2023-07-14 13:53:50.805361 LogTranslate-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2474 2023-06-28 15:23:37.000000 LogTranslate-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:50.798618 LogTranslate-1.2.6/log_translate/
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.6/log_translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:50.803353 LogTranslate-1.2.6/log_translate/business/
+-rw-rw-rw-   0        0        0      618 2023-06-28 15:23:37.000000 LogTranslate-1.2.6/log_translate/business/AndroidCrashPattern_translator.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 15:23:37.000000 LogTranslate-1.2.6/log_translate/business/__init__.py
+-rw-rw-rw-   0        0        0     3893 2023-06-30 11:21:05.000000 LogTranslate-1.2.6/log_translate/business/bluetooth_translator.py
+-rw-rw-rw-   0        0        0      329 2023-06-28 15:23:37.000000 LogTranslate-1.2.6/log_translate/config_default.py
+-rw-rw-rw-   0        0        0     1349 2023-06-28 15:23:37.000000 LogTranslate-1.2.6/log_translate/data_struct.py
+-rw-rw-rw-   0        0        0       11 2023-06-28 15:23:37.000000 LogTranslate-1.2.6/log_translate/gloable.py
+-rw-rw-rw-   0        0        0     4448 2023-07-03 13:31:40.000000 LogTranslate-1.2.6/log_translate/log_translator.py
+-rw-rw-rw-   0        0        0     3465 2023-07-14 13:52:44.000000 LogTranslate-1.2.6/log_translate/read_log_file.py
+drwxrwxrwx   0        0        0        0 2023-07-14 13:53:50.803353 LogTranslate-1.2.6/log_translate/res/
+-rw-rw-rw-   0        0        0    10687 2023-06-28 15:23:37.000000 LogTranslate-1.2.6/log_translate/res/log_logo.ico
+-rw-rw-rw-   0        0        0     7561 2023-07-06 17:13:36.000000 LogTranslate-1.2.6/log_translate/ui_pyqt6.py
+-rw-rw-rw-   0        0        0     7491 2023-07-06 17:14:47.000000 LogTranslate-1.2.6/log_translate/ui_pyside2.py
+-rw-rw-rw-   0        0        0      393 2023-06-28 15:23:37.000000 LogTranslate-1.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 13:53:50.806163 LogTranslate-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2199 2023-07-14 13:53:41.000000 LogTranslate-1.2.6/setup.py
```

### Comparing `LogTranslate-1.2.3/LICENSE.txt` & `LogTranslate-1.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.3/LogTranslate.egg-info/PKG-INFO` & `LogTranslate-1.2.6/LogTranslate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.2.3
+Version: 1.2.6
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.2.3/LogTranslate.egg-info/SOURCES.txt` & `LogTranslate-1.2.6/LogTranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.3/PKG-INFO` & `LogTranslate-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogTranslate
-Version: 1.2.3
+Version: 1.2.6
 Summary: A Python library for translate log from log files
 Home-page: https://github.com/5hmlA/PyTools
 Author: 5hmlA
 Author-email: jonas.jzy@gmail.com
 License: MIT Licence
 Keywords: tools log translate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LogTranslate-1.2.3/README.md` & `LogTranslate-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.3/log_translate/business/AndroidCrashPattern_translator.py` & `LogTranslate-1.2.6/log_translate/business/AndroidCrashPattern_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.3/log_translate/business/bluetooth_translator.py` & `LogTranslate-1.2.6/log_translate/business/bluetooth_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.3/log_translate/data_struct.py` & `LogTranslate-1.2.6/log_translate/data_struct.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.3/log_translate/log_translator.py` & `LogTranslate-1.2.6/log_translate/log_translator.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.3/log_translate/read_log_file.py` & `LogTranslate-1.2.6/log_translate/read_log_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from os import cpu_count
 
 from rx.subject import Subject
 
 from log_translate.config_default import translators
 from log_translate.data_struct import Log
 
+from log_translate.log_translate.data_struct import Level
+
 
 # //必须定义在使用者前面
 class LogReader(object):
     def __init__(self,
                  chunk_size=1024 * 1024 * 10,
                  process_num_for_log_parsing=cpu_count()):
         self.log_unparsed_queue = deque()  # 用于存储未解析日志
@@ -53,21 +55,22 @@
                         if result:
                             print(result)
                             result.origin = str
                             self.log_stream.on_next(result)
                             break
                     except Exception as e:
                         print('日志翻译发生异常：', e)
-                        print(str)
                         traceback.print_exc()
-                        raise e
+                        self.log_stream.on_next(
+                            Log(translated="日志翻译发生异常：%s \n%s" % (str, traceback.format_exc()), level=Level.e)
+                        )
             except Exception as e:
                 print('文件解析发生异常：', e)
                 traceback.print_exc()
-                raise e
+                self.log_stream.on_next(Log(translated="文件解析发生异常：%s" % traceback.format_exc(), level=Level.e))
         self.log_stream.on_next(Log(translated=None))
 
     def concurrency(self, log_files):
         # 多线程 解析
         for file in log_files:
             abspath = os.path.abspath(file)
             print(abspath)
```

### Comparing `LogTranslate-1.2.3/log_translate/res/log_logo.ico` & `LogTranslate-1.2.6/log_translate/res/log_logo.ico`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.3/log_translate/ui_pyqt6.py` & `LogTranslate-1.2.6/log_translate/ui_pyqt6.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.3/log_translate/ui_pyside2.py` & `LogTranslate-1.2.6/log_translate/ui_pyside2.py`

 * *Files identical despite different names*

### Comparing `LogTranslate-1.2.3/setup.py` & `LogTranslate-1.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # PACKAGE_NAME主要在使用的时候用到 pkg_resources.resource_filename('log_translate', 'res/log_logo.ico')
 PACKAGE_NAME = 'log_translate'
 # 需要写清楚路径
 ICON_PATH = 'res/*.ico'
 
 setup(
     name='LogTranslate',
-    version='1.2.3',
+    version='1.2.6',
     author='5hmlA',
     author_email='jonas.jzy@gmail.com',
     # 指定运行时需要的Python版本
     python_requires='>=3.6',
     # 找到当前目录下有哪些包 当前(setup.py)目录下的文件夹 当前目录的py不包含 打包的是把所有代码放一个文件夹下文件名为库名字
     packages=find_packages(),
     # 配置readme
```

