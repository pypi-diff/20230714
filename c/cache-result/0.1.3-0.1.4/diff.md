# Comparing `tmp/cache-result-0.1.3.tar.gz` & `tmp/cache-result-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cache-result-0.1.3.tar", last modified: Thu Jul 13 15:46:14 2023, max compression
+gzip compressed data, was "cache-result-0.1.4.tar", last modified: Fri Jul 14 04:43:58 2023, max compression
```

## Comparing `cache-result-0.1.3.tar` & `cache-result-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 15:46:14.278815 cache-result-0.1.3/
--rw-rw-rw-   0        0        0     1740 2023-07-13 15:46:14.277815 cache-result-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1527 2023-07-13 15:01:58.000000 cache-result-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 15:46:14.264824 cache-result-0.1.3/cache_result/
--rw-rw-rw-   0        0        0     2676 2023-07-13 15:42:42.000000 cache-result-0.1.3/cache_result/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 15:46:14.274815 cache-result-0.1.3/cache_result.egg-info/
--rw-rw-rw-   0        0        0     1740 2023-07-13 15:46:13.000000 cache-result-0.1.3/cache_result.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-07-13 15:46:14.000000 cache-result-0.1.3/cache_result.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 15:46:13.000000 cache-result-0.1.3/cache_result.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-13 15:46:13.000000 cache-result-0.1.3/cache_result.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 15:46:14.278815 cache-result-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      510 2023-07-13 15:45:45.000000 cache-result-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:43:58.877354 cache-result-0.1.4/
+-rw-rw-rw-   0        0        0     1816 2023-07-14 04:43:58.876354 cache-result-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1527 2023-07-13 15:01:58.000000 cache-result-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 04:43:58.866354 cache-result-0.1.4/cache_result/
+-rw-rw-rw-   0        0        0     3743 2023-07-14 04:34:33.000000 cache-result-0.1.4/cache_result/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 04:43:58.874354 cache-result-0.1.4/cache_result.egg-info/
+-rw-rw-rw-   0        0        0     1816 2023-07-14 04:43:58.000000 cache-result-0.1.4/cache_result.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-07-14 04:43:58.000000 cache-result-0.1.4/cache_result.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 04:43:58.000000 cache-result-0.1.4/cache_result.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 04:43:58.000000 cache-result-0.1.4/cache_result.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 04:43:58.877354 cache-result-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-07-14 04:42:39.000000 cache-result-0.1.4/setup.py
```

### Comparing `cache-result-0.1.3/PKG-INFO` & `cache-result-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: cache-result
-Version: 0.1.3
-Summary: A decorator for caching the results of functions
+Version: 0.1.4
+Summary: A python decorator for caching the results of functions
 Author: glwhappen
 Author-email: 1597721684@qq.com
+Project-URL: Source Code, https://github.com/glwhappen/cache-result
 Description-Content-Type: text/markdown
 
 # Cache Function Result
 
 ## Description
 
 这是一个Python包，它提供了一个装饰器用于缓存函数的返回结果。缓存的结果可以指定任意位置，非常的自由，缓存的键则是根据函数名、源代码和参数来控制的。你可以选择排除某些元素，例如函数名、源代码、参数或者关键字参数。
```

### Comparing `cache-result-0.1.3/README.md` & `cache-result-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cache-result-0.1.3/cache_result/__init__.py` & `cache-result-0.1.4/cache_result/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 import os
 import pickle
 import hashlib
 import inspect
 import re
+from colorama import Fore, Back, Style
 
+def remove_comments_and_prints(source_code):
+    # 删除单行注释
+    source_code = re.sub(r'#.*$', "", source_code, flags=re.MULTILINE)
+    # 删除print语句
+    source_code = re.sub(r'print\(.*\)', "", source_code)
+    return source_code
 
-def cache(cache_dir, exclude=None, is_print=False):
+def cache(cache_dir, exclude=None, is_print=True):
     """
     缓存函数的装饰器
     :param cache_dir: 缓存目录
     :param exclude: 排除的参数 ['func_name', 'source_code', 'args', 'kwargs']
 
     """
     if exclude is None:
@@ -32,15 +39,16 @@
 
             hash_key = []
             if 'func_name' not in exclude:
                 hash_key.append(func.__name__)
             if 'source_code' not in exclude:
                 tmp_source_code = source_code
                 if 'func_name' not in exclude:
-                    tmp_source_code = source_code.replace(func.__name__, '')
+                    tmp_source_code = remove_comments_and_prints(tmp_source_code)
+                    tmp_source_code = tmp_source_code.replace(func.__name__, '')
 
                 tmp_source_code = re.sub(r'\s', '', tmp_source_code)
                 hash_key.append(tmp_source_code)
             if 'args' not in exclude:
                 hash_key.append(str(args))
             if 'kwargs' not in exclude:
                 hash_key.append(str(kwargs))
@@ -52,20 +60,30 @@
 
             # 创建缓存目录
             os.makedirs(modified_cache_dir, exist_ok=True)
 
             # 如果缓存文件存在，直接读取并返回结果
             if os.path.exists(file_path):
                 with open(file_path, 'rb') as f:
-                    result = pickle.load(f)
+                    try:
+                        result = pickle.load(f)
+                    except: # 如果pickle文件损坏，重新运行函数
+                        result = func(*args, **kwargs)
+                        with open(file_path, 'wb') as f:
+                            pickle.dump(result, f)
+                        if is_print:
+                            print(Fore.YELLOW + f'{func.__name__} Saved to cache', os.path.join(os.getcwd(), modified_cache_dir))
+                            print(Style.RESET_ALL)
                 if is_print:
-                    print('Loaded from cache')
+                    print(Fore.GREEN +f'{func.__name__} Loaded from cache')
+                    print(Style.RESET_ALL)
             else:
                 # 否则，运行函数并保存结果
                 result = func(*args, **kwargs)
                 with open(file_path, 'wb') as f:
                     pickle.dump(result, f)
                 if is_print:
-                    print('Saved to cache')
+                    print(Fore.YELLOW + f'{func.__name__} Saved to cache', os.path.join(os.getcwd(), modified_cache_dir))
+                    print(Style.RESET_ALL)
             return result
         return wrapper
     return decorator
```

### Comparing `cache-result-0.1.3/cache_result.egg-info/PKG-INFO` & `cache-result-0.1.4/cache_result.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: cache-result
-Version: 0.1.3
-Summary: A decorator for caching the results of functions
+Version: 0.1.4
+Summary: A python decorator for caching the results of functions
 Author: glwhappen
 Author-email: 1597721684@qq.com
+Project-URL: Source Code, https://github.com/glwhappen/cache-result
 Description-Content-Type: text/markdown
 
 # Cache Function Result
 
 ## Description
 
 这是一个Python包，它提供了一个装饰器用于缓存函数的返回结果。缓存的结果可以指定任意位置，非常的自由，缓存的键则是根据函数名、源代码和参数来控制的。你可以选择排除某些元素，例如函数名、源代码、参数或者关键字参数。
```

