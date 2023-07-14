# Comparing `tmp/cache-result-0.1.6.tar.gz` & `tmp/cache-result-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cache-result-0.1.6.tar", last modified: Fri Jul 14 05:15:53 2023, max compression
+gzip compressed data, was "cache-result-0.1.7.tar", last modified: Fri Jul 14 06:10:30 2023, max compression
```

## Comparing `cache-result-0.1.6.tar` & `cache-result-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 05:15:53.642766 cache-result-0.1.6/
--rw-rw-rw-   0        0        0     1816 2023-07-14 05:15:53.641765 cache-result-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1527 2023-07-13 15:01:58.000000 cache-result-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 05:15:53.632766 cache-result-0.1.6/cache_result/
--rw-rw-rw-   0        0        0     3807 2023-07-14 05:14:35.000000 cache-result-0.1.6/cache_result/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:15:53.639766 cache-result-0.1.6/cache_result.egg-info/
--rw-rw-rw-   0        0        0     1816 2023-07-14 05:15:53.000000 cache-result-0.1.6/cache_result.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-07-14 05:15:53.000000 cache-result-0.1.6/cache_result.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 05:15:53.000000 cache-result-0.1.6/cache_result.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-14 05:15:53.000000 cache-result-0.1.6/cache_result.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 05:15:53.642766 cache-result-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-07-14 05:15:20.000000 cache-result-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:10:30.903357 cache-result-0.1.7/
+-rw-rw-rw-   0        0        0     3032 2023-07-14 06:10:30.902359 cache-result-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2743 2023-07-14 06:08:46.000000 cache-result-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 06:10:30.893355 cache-result-0.1.7/cache_result/
+-rw-rw-rw-   0        0        0     3718 2023-07-14 05:18:56.000000 cache-result-0.1.7/cache_result/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:10:30.900356 cache-result-0.1.7/cache_result.egg-info/
+-rw-rw-rw-   0        0        0     3032 2023-07-14 06:10:30.000000 cache-result-0.1.7/cache_result.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-07-14 06:10:30.000000 cache-result-0.1.7/cache_result.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 06:10:30.000000 cache-result-0.1.7/cache_result.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 06:10:30.000000 cache-result-0.1.7/cache_result.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 06:10:30.903357 cache-result-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-07-14 06:08:57.000000 cache-result-0.1.7/setup.py
```

### Comparing `cache-result-0.1.6/cache_result/__init__.py` & `cache-result-0.1.7/cache_result/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,23 +69,20 @@
                     try:
                         result = pickle.load(f)
                     except: # 如果pickle文件损坏，重新运行函数
                         result = func(*args, **kwargs)
                         with open(file_path, 'wb') as f:
                             pickle.dump(result, f)
                         if is_print:
-                            print(Fore.YELLOW + f'{func.__name__} Saved to cache', os.path.join(os.getcwd(), modified_cache_dir))
-                            print(Style.RESET_ALL)
+                            print(Fore.YELLOW + f'{func.__name__} Saved to cache', os.path.join(os.getcwd(), modified_cache_dir), Style.RESET_ALL)
                 if is_print:
-                    print(Fore.GREEN +f'{func.__name__} Loaded from cache')
-                    print(Style.RESET_ALL)
+                    print(Fore.GREEN +f'{func.__name__} Loaded from cache', Style.RESET_ALL)
             else:
                 # 否则，运行函数并保存结果
                 result = func(*args, **kwargs)
                 with open(file_path, 'wb') as f:
                     pickle.dump(result, f)
                 if is_print:
-                    print(Fore.YELLOW + f'{func.__name__} Saved to cache', os.path.join(os.getcwd(), modified_cache_dir))
-                    print(Style.RESET_ALL)
+                    print(Fore.YELLOW + f'{func.__name__} Saved to cache', os.path.join(os.getcwd(), modified_cache_dir), Style.RESET_ALL)
             return result
         return wrapper
     return decorator
```

### Comparing `cache-result-0.1.6/setup.py` & `cache-result-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # 读取README.md文件的内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cache-result',
-    version='0.1.6',
+    version='0.1.7',
     description='A python decorator for caching the results of functions',
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         'Source Code': 'https://github.com/glwhappen/cache-result',
     },
     author='glwhappen',
```

