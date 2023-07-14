# Comparing `tmp/cache-result-0.1.7.tar.gz` & `tmp/cache-result-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cache-result-0.1.7.tar", last modified: Fri Jul 14 06:10:30 2023, max compression
+gzip compressed data, was "cache-result-0.1.8.tar", last modified: Fri Jul 14 12:48:49 2023, max compression
```

## Comparing `cache-result-0.1.7.tar` & `cache-result-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 06:10:30.903357 cache-result-0.1.7/
--rw-rw-rw-   0        0        0     3032 2023-07-14 06:10:30.902359 cache-result-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2743 2023-07-14 06:08:46.000000 cache-result-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 06:10:30.893355 cache-result-0.1.7/cache_result/
--rw-rw-rw-   0        0        0     3718 2023-07-14 05:18:56.000000 cache-result-0.1.7/cache_result/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:10:30.900356 cache-result-0.1.7/cache_result.egg-info/
--rw-rw-rw-   0        0        0     3032 2023-07-14 06:10:30.000000 cache-result-0.1.7/cache_result.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-07-14 06:10:30.000000 cache-result-0.1.7/cache_result.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 06:10:30.000000 cache-result-0.1.7/cache_result.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-14 06:10:30.000000 cache-result-0.1.7/cache_result.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 06:10:30.903357 cache-result-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-07-14 06:08:57.000000 cache-result-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:48:49.360849 cache-result-0.1.8/
+-rw-rw-rw-   0        0        0     3032 2023-07-14 12:48:49.359849 cache-result-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2743 2023-07-14 06:08:46.000000 cache-result-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 12:48:49.343850 cache-result-0.1.8/cache_result/
+-rw-rw-rw-   0        0        0     3972 2023-07-14 12:18:29.000000 cache-result-0.1.8/cache_result/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:48:49.356850 cache-result-0.1.8/cache_result.egg-info/
+-rw-rw-rw-   0        0        0     3032 2023-07-14 12:48:48.000000 cache-result-0.1.8/cache_result.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-07-14 12:48:49.000000 cache-result-0.1.8/cache_result.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 12:48:48.000000 cache-result-0.1.8/cache_result.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 12:48:48.000000 cache-result-0.1.8/cache_result.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 12:48:48.000000 cache-result-0.1.8/cache_result.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 12:48:49.360849 cache-result-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      666 2023-07-14 12:48:02.000000 cache-result-0.1.8/setup.py
```

### Comparing `cache-result-0.1.7/PKG-INFO` & `cache-result-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cache-result
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python decorator for caching the results of functions
 Author: glwhappen
 Author-email: 1597721684@qq.com
 Project-URL: Source Code, https://github.com/glwhappen/cache-result
 Description-Content-Type: text/markdown
 
 # Cache Function Result
```

### Comparing `cache-result-0.1.7/README.md` & `cache-result-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cache-result-0.1.7/cache_result/__init__.py` & `cache-result-0.1.8/cache_result/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import pickle
 import hashlib
 import inspect
 import re
+import time
+
 from colorama import Fore, Back, Style
 
 def remove_unused_code(source_code):
     # 删除单行注释
     source_code = re.sub(r'#.*$', "", source_code, flags=re.MULTILINE)
     # 删除print语句
     source_code = re.sub(r'print\(.*\)', "", source_code)
@@ -14,15 +16,15 @@
     source_code = re.sub(r'@cache\(.*\)', '', source_code)
     return source_code
 
 def cache(cache_dir, exclude=None, is_print=True):
     """
     缓存函数的装饰器
     :param cache_dir: 缓存目录
-    :param exclude: 排除的参数 ['func_name', 'source_code', 'args', 'kwargs']
+    :param exclude: 排除的参数 ['func_name', 'source_code', 'args'] 函数名、源代码、函数参数
 
     """
     if exclude is None:
         exclude = []
 
     def decorator(func):
         def wrapper(*args, **kwargs):
@@ -30,14 +32,17 @@
             source_code = inspect.getsource(func)
 
             # 获取函数的参数名
             params = inspect.signature(func).parameters
             # 创建一个字典，将参数名和值对应起来
             args_dict = {name: kwargs.get(name, param.default) if param.default is not inspect.Parameter.empty else args[i] for i, (name, param) in enumerate(params.items())}
             args_dict.update(kwargs)
+            # print('args_dict:', str(args_dict))
+            # print('args:', args)
+            # print('kwargs:', kwargs)
 
             # 使用参数值来修改路径
             modified_cache_dir = cache_dir.format(**args_dict)
 
 
             hash_key = []
             if 'func_name' not in exclude:
@@ -47,39 +52,40 @@
                 if 'func_name' not in exclude:
                     tmp_source_code = remove_unused_code(tmp_source_code)
                     tmp_source_code = tmp_source_code.replace(func.__name__, '')
 
                 tmp_source_code = re.sub(r'\s', '', tmp_source_code)
                 hash_key.append(tmp_source_code)
             if 'args' not in exclude:
-                hash_key.append(str(args))
-            if 'kwargs' not in exclude:
-                hash_key.append(str(kwargs))
+                hash_key.append(str(args_dict))
 
             # 创建一个唯一的文件名，基于函数名、源代码和参数
             key = pickle.dumps(hash_key)
             file_name = hashlib.sha256(key).hexdigest() + '.pickle'
             file_path = os.path.join(modified_cache_dir, file_name)
 
             # 创建缓存目录
             os.makedirs(modified_cache_dir, exist_ok=True)
 
             # 如果缓存文件存在，直接读取并返回结果
             if os.path.exists(file_path):
+                start = time.time()
+                if is_print:
+                    print(Fore.GREEN +f'{func.__name__} Loading from cache', Style.RESET_ALL, end=' ')
                 with open(file_path, 'rb') as f:
                     try:
                         result = pickle.load(f)
                     except: # 如果pickle文件损坏，重新运行函数
                         result = func(*args, **kwargs)
                         with open(file_path, 'wb') as f:
                             pickle.dump(result, f)
                         if is_print:
                             print(Fore.YELLOW + f'{func.__name__} Saved to cache', os.path.join(os.getcwd(), modified_cache_dir), Style.RESET_ALL)
                 if is_print:
-                    print(Fore.GREEN +f'{func.__name__} Loaded from cache', Style.RESET_ALL)
+                    print(Fore.RED +f'{(time.time() - start):.1f}s ok', Style.RESET_ALL)
             else:
                 # 否则，运行函数并保存结果
                 result = func(*args, **kwargs)
                 with open(file_path, 'wb') as f:
                     pickle.dump(result, f)
                 if is_print:
                     print(Fore.YELLOW + f'{func.__name__} Saved to cache', os.path.join(os.getcwd(), modified_cache_dir), Style.RESET_ALL)
```

### Comparing `cache-result-0.1.7/cache_result.egg-info/PKG-INFO` & `cache-result-0.1.8/cache_result.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cache-result
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python decorator for caching the results of functions
 Author: glwhappen
 Author-email: 1597721684@qq.com
 Project-URL: Source Code, https://github.com/glwhappen/cache-result
 Description-Content-Type: text/markdown
 
 # Cache Function Result
```

### Comparing `cache-result-0.1.7/setup.py` & `cache-result-0.1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 # 读取README.md文件的内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cache-result',
-    version='0.1.7',
+    version='0.1.8',
     description='A python decorator for caching the results of functions',
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         'Source Code': 'https://github.com/glwhappen/cache-result',
     },
     author='glwhappen',
     author_email='1597721684@qq.com',
     packages=find_packages(),
-    install_requires=[],
+    install_requires=[
+        'colorama',  # 控制台输出颜色
+    ],
 )
```

