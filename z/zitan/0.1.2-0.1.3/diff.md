# Comparing `tmp/zitan-0.1.2.tar.gz` & `tmp/zitan-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zitan-0.1.2.tar", last modified: Thu Jul 13 09:55:51 2023, max compression
+gzip compressed data, was "dist\zitan-0.1.3.tar", last modified: Fri Jul 14 11:00:54 2023, max compression
```

## Comparing `zitan-0.1.2.tar` & `zitan-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 09:55:51.000000 zitan-0.1.2/
--rw-rw-rw-   0        0        0     1088 2023-07-12 11:41:48.000000 zitan-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      704 2023-07-13 09:55:51.000000 zitan-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-07-12 11:42:42.000000 zitan-0.1.2/README.txt
--rw-rw-rw-   0        0        0       78 2023-07-12 09:34:05.000000 zitan-0.1.2/main.py
--rw-rw-rw-   0        0        0       42 2023-07-13 09:55:51.000000 zitan-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     4164 2023-07-13 09:54:48.000000 zitan-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 09:55:51.000000 zitan-0.1.2/zitan.egg-info/
--rw-rw-rw-   0        0        0      704 2023-07-13 09:55:50.000000 zitan-0.1.2/zitan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      155 2023-07-13 09:55:50.000000 zitan-0.1.2/zitan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 09:55:50.000000 zitan-0.1.2/zitan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 09:55:50.000000 zitan-0.1.2/zitan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 11:00:54.000000 zitan-0.1.3/
+-rw-rw-rw-   0        0        0     1088 2023-07-12 11:41:48.000000 zitan-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      704 2023-07-14 11:00:54.000000 zitan-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-07-12 11:42:42.000000 zitan-0.1.3/README.txt
+-rw-rw-rw-   0        0        0       78 2023-07-12 09:34:05.000000 zitan-0.1.3/main.py
+-rw-rw-rw-   0        0        0       42 2023-07-14 11:00:54.000000 zitan-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     4164 2023-07-14 10:57:16.000000 zitan-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:00:54.000000 zitan-0.1.3/zitan/
+-rw-rw-rw-   0        0        0       26 2023-07-13 09:40:50.000000 zitan-0.1.3/zitan/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 11:00:54.000000 zitan-0.1.3/zitan.egg-info/
+-rw-rw-rw-   0        0        0      704 2023-07-14 11:00:54.000000 zitan-0.1.3/zitan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-07-14 11:00:54.000000 zitan-0.1.3/zitan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 11:00:54.000000 zitan-0.1.3/zitan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-14 11:00:54.000000 zitan-0.1.3/zitan.egg-info/top_level.txt
```

### Comparing `zitan-0.1.2/LICENSE.txt` & `zitan-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zitan-0.1.2/PKG-INFO` & `zitan-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zitan
-Version: 0.1.2
+Version: 0.1.3
 Summary: This project is used to display ...
 Home-page: https://github.com/你的github账户/test(项目文件夹名称)
 Author: xxx
 Author-email: xxx@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `zitan-0.1.2/setup.py` & `zitan-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Package meta-data.
 NAME = 'zitan'  # 项目的名称，即包的分发名称
 DESCRIPTION = 'This project is used to display ...'  # 项目的简短描述
 URL = 'https://github.com/你的github账户/test(项目文件夹名称)'
 EMAIL = 'xxx@gmail.com'  # 项目作者的邮件
 AUTHOR = 'xxx'  # 项目作者的名字
 REQUIRES_PYTHON = '>=3.6.0'  # 项目支持的版本
-VERSION = '0.1.2'  # 项目的版本,如果后续代码有了任何更改，再次上传需要增加版本号
+VERSION = '0.1.3'  # 项目的版本,如果后续代码有了任何更改，再次上传需要增加版本号
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
@@ -100,17 +100,17 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    # packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
-    py_modules=['test_pkg'],
+    # py_modules=['test_pkg'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
```

### Comparing `zitan-0.1.2/zitan.egg-info/PKG-INFO` & `zitan-0.1.3/zitan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zitan
-Version: 0.1.2
+Version: 0.1.3
 Summary: This project is used to display ...
 Home-page: https://github.com/你的github账户/test(项目文件夹名称)
 Author: xxx
 Author-email: xxx@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

