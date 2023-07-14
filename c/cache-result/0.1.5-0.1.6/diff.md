# Comparing `tmp/cache-result-0.1.5.tar.gz` & `tmp/cache-result-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cache-result-0.1.5.tar", last modified: Fri Jul 14 05:09:46 2023, max compression
+gzip compressed data, was "cache-result-0.1.6.tar", last modified: Fri Jul 14 05:15:53 2023, max compression
```

## Comparing `cache-result-0.1.5.tar` & `cache-result-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 05:09:46.979946 cache-result-0.1.5/
--rw-rw-rw-   0        0        0     1816 2023-07-14 05:09:46.978947 cache-result-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1527 2023-07-13 15:01:58.000000 cache-result-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 05:09:46.967943 cache-result-0.1.5/cache_result/
--rw-rw-rw-   0        0        0     3851 2023-07-14 04:57:38.000000 cache-result-0.1.5/cache_result/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:09:46.975945 cache-result-0.1.5/cache_result.egg-info/
--rw-rw-rw-   0        0        0     1816 2023-07-14 05:09:46.000000 cache-result-0.1.5/cache_result.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-07-14 05:09:46.000000 cache-result-0.1.5/cache_result.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 05:09:46.000000 cache-result-0.1.5/cache_result.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-14 05:09:46.000000 cache-result-0.1.5/cache_result.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 05:09:46.979946 cache-result-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-07-14 04:57:38.000000 cache-result-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:15:53.642766 cache-result-0.1.6/
+-rw-rw-rw-   0        0        0     1816 2023-07-14 05:15:53.641765 cache-result-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1527 2023-07-13 15:01:58.000000 cache-result-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 05:15:53.632766 cache-result-0.1.6/cache_result/
+-rw-rw-rw-   0        0        0     3807 2023-07-14 05:14:35.000000 cache-result-0.1.6/cache_result/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 05:15:53.639766 cache-result-0.1.6/cache_result.egg-info/
+-rw-rw-rw-   0        0        0     1816 2023-07-14 05:15:53.000000 cache-result-0.1.6/cache_result.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-07-14 05:15:53.000000 cache-result-0.1.6/cache_result.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 05:15:53.000000 cache-result-0.1.6/cache_result.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-14 05:15:53.000000 cache-result-0.1.6/cache_result.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 05:15:53.642766 cache-result-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-07-14 05:15:20.000000 cache-result-0.1.6/setup.py
```

### Comparing `cache-result-0.1.5/PKG-INFO` & `cache-result-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cache-result
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python decorator for caching the results of functions
 Author: glwhappen
 Author-email: 1597721684@qq.com
 Project-URL: Source Code, https://github.com/glwhappen/cache-result
 Description-Content-Type: text/markdown
 
 # Cache Function Result
```

### Comparing `cache-result-0.1.5/README.md` & `cache-result-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cache-result-0.1.5/cache_result/__init__.py` & `cache-result-0.1.6/cache_result/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,14 @@
             hash_key = []
             if 'func_name' not in exclude:
                 hash_key.append(func.__name__)
             if 'source_code' not in exclude:
                 tmp_source_code = source_code
                 if 'func_name' not in exclude:
                     tmp_source_code = remove_unused_code(tmp_source_code)
-                    print(tmp_source_code)
                     tmp_source_code = tmp_source_code.replace(func.__name__, '')
 
                 tmp_source_code = re.sub(r'\s', '', tmp_source_code)
                 hash_key.append(tmp_source_code)
             if 'args' not in exclude:
                 hash_key.append(str(args))
             if 'kwargs' not in exclude:
```

### Comparing `cache-result-0.1.5/cache_result.egg-info/PKG-INFO` & `cache-result-0.1.6/cache_result.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cache-result
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python decorator for caching the results of functions
 Author: glwhappen
 Author-email: 1597721684@qq.com
 Project-URL: Source Code, https://github.com/glwhappen/cache-result
 Description-Content-Type: text/markdown
 
 # Cache Function Result
```

### Comparing `cache-result-0.1.5/setup.py` & `cache-result-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # 读取README.md文件的内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cache-result',
-    version='0.1.5',
+    version='0.1.6',
     description='A python decorator for caching the results of functions',
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         'Source Code': 'https://github.com/glwhappen/cache-result',
     },
     author='glwhappen',
```

