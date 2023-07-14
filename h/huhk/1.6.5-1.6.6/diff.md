# Comparing `tmp/huhk-1.6.5.tar.gz` & `tmp/huhk-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.6.5.tar", last modified: Thu Jul 13 08:03:46 2023, max compression
+gzip compressed data, was "huhk-1.6.6.tar", last modified: Fri Jul 14 10:02:02 2023, max compression
```

## Comparing `huhk-1.6.5.tar` & `huhk-1.6.6.tar`

### file list

```diff
@@ -1,47 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 08:03:46.424088 huhk-1.6.5/
--rw-rw-rw-   0        0        0      223 2023-07-13 08:03:46.423091 huhk-1.6.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 08:03:46.341335 huhk-1.6.5/huhk/
--rw-rw-rw-   0        0        0      931 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/__init__.py
--rw-rw-rw-   0        0        0      532 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 08:03:46.376216 huhk-1.6.5/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0     3072 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/case_project/base_project.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0      790 2023-07-13 02:39:46.000000 huhk-1.6.5/huhk/case_project/main.py
--rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-13 08:03:45.000000 huhk-1.6.5/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    29281 2023-07-13 01:55:03.000000 huhk-1.6.5/huhk/init_project.py
--rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-13 08:03:46.379215 huhk-1.6.5/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 08:03:46.421097 huhk-1.6.5/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.5/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7303 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      517 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1544 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2144 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      564 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2648 2023-07-13 01:44:43.000000 huhk-1.6.5/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1692 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1612 2023-07-12 02:24:22.000000 huhk-1.6.5/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      549 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22779 2023-07-12 02:54:58.000000 huhk-1.6.5/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    25687 2023-07-13 08:03:20.000000 huhk-1.6.5/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9212 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.5/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-13 08:03:46.355300 huhk-1.6.5/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-13 08:03:46.000000 huhk-1.6.5/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1077 2023-07-13 08:03:46.000000 huhk-1.6.5/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 08:03:46.000000 huhk-1.6.5/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-13 08:03:46.000000 huhk-1.6.5/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-13 08:03:46.000000 huhk-1.6.5/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-13 08:03:46.000000 huhk-1.6.5/huhk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 08:03:46.424088 huhk-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.327263 huhk-1.6.6/
+-rw-rw-rw-   0        0        0      223 2023-07-14 10:02:02.326264 huhk-1.6.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.207981 huhk-1.6.6/huhk/
+-rw-rw-rw-   0        0        0     1006 2023-07-14 07:11:08.000000 huhk-1.6.6/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.228927 huhk-1.6.6/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0     4863 2023-07-14 08:57:28.000000 huhk-1.6.6/huhk/case_project/base_project.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      790 2023-07-13 02:39:46.000000 huhk-1.6.6/huhk/case_project/main.py
+-rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-14 10:02:01.000000 huhk-1.6.6/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    29648 2023-07-14 08:31:42.000000 huhk-1.6.6/huhk/init_project.py
+-rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.230922 huhk-1.6.6/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.254455 huhk-1.6.6/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.6/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.6.6/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.6.6/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.6.6/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    25687 2023-07-13 08:03:20.000000 huhk-1.6.6/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9212 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.6/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.217957 huhk-1.6.6/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-14 10:02:02.000000 huhk-1.6.6/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1987 2023-07-14 10:02:02.000000 huhk-1.6.6/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 10:02:02.000000 huhk-1.6.6/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-14 10:02:02.000000 huhk-1.6.6/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-14 10:02:02.000000 huhk-1.6.6/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-14 10:02:02.000000 huhk-1.6.6/huhk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.256449 huhk-1.6.6/service/
+-rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.6.6/service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.268418 huhk-1.6.6/service/app_t/
+-rw-rw-rw-   0        0        0      403 2023-07-14 07:07:28.000000 huhk-1.6.6/service/app_t/__init__.py
+-rw-rw-rw-   0        0        0     7752 2023-07-14 01:51:05.000000 huhk-1.6.6/service/app_t/app_t_api.py
+-rw-rw-rw-   0        0        0     7301 2023-07-14 01:51:05.000000 huhk-1.6.6/service/app_t/app_t_api_fun.py
+-rw-rw-rw-   0        0        0     3353 2023-07-14 01:51:05.000000 huhk-1.6.6/service/app_t/app_t_assert.py
+-rw-rw-rw-   0        0        0      890 2023-07-14 01:51:05.000000 huhk-1.6.6/service/app_t/app_t_fun.py
+-rw-rw-rw-   0        0        0     4402 2023-07-14 01:51:05.000000 huhk-1.6.6/service/app_t/app_t_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.278391 huhk-1.6.6/service/demo/
+-rw-rw-rw-   0        0        0      407 2023-07-14 08:11:52.000000 huhk-1.6.6/service/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.280388 huhk-1.6.6/service/demo/api/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.6/service/demo/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.282380 huhk-1.6.6/service/demo/assert/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.6/service/demo/assert/__init__.py
+-rw-rw-rw-   0        0        0      871 2023-07-14 08:25:58.000000 huhk-1.6.6/service/demo/demo_api.py
+-rw-rw-rw-   0        0        0      828 2023-07-14 08:25:58.000000 huhk-1.6.6/service/demo/demo_api_fun.py
+-rw-rw-rw-   0        0        0      459 2023-07-14 08:25:58.000000 huhk-1.6.6/service/demo/demo_assert.py
+-rw-rw-rw-   0        0        0      721 2023-07-14 08:25:58.000000 huhk-1.6.6/service/demo/demo_fun.py
+-rw-rw-rw-   0        0        0      579 2023-07-14 08:25:58.000000 huhk-1.6.6/service/demo/demo_sql.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.287370 huhk-1.6.6/service/demo/fun/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.6/service/demo/fun/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.289363 huhk-1.6.6/service/demo/sql/
+-rw-rw-rw-   0        0        0        0 2023-07-14 08:11:52.000000 huhk-1.6.6/service/demo/sql/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-14 10:02:02.327263 huhk-1.6.6/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.292353 huhk-1.6.6/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.6/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.321277 huhk-1.6.6/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.6/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.6/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.6/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.6/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      523 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2632 2023-07-14 07:03:11.000000 huhk-1.6.6/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1651 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1571 2023-07-14 06:52:17.000000 huhk-1.6.6/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-07-14 06:52:16.000000 huhk-1.6.6/testcase/apache/test_to_string.py
+drwxrwxrwx   0        0        0        0 2023-07-14 10:02:02.324269 huhk-1.6.6/testcase/app_t/
+-rw-rw-rw-   0        0        0        0 2023-07-14 06:51:02.000000 huhk-1.6.6/testcase/app_t/__init__.py
+-rw-rw-rw-   0        0        0     1923 2023-07-14 01:51:05.000000 huhk-1.6.6/testcase/app_t/test_api.py
```

### Comparing `huhk-1.6.5/huhk/__init__.py` & `huhk-1.6.6/huhk/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,8 +13,9 @@
     projects_path = os.path.join(*projects_path_list[:projects_path_list.index("testcase")])
 if ":" in projects_path:
     projects_path = projects_path.replace(":", ":" + os.path.sep)
 else:
     projects_path = os.path.sep + projects_path
 files_path = os.path.join(projects_path, "files")
 service_path = os.path.join(projects_path, "service")
+service_json_path = os.path.join(projects_path, "service", "service.json")
 testcase_path = os.path.join(projects_path, "testcase")
```

### Comparing `huhk-1.6.5/huhk/case_project/json_coder.py` & `huhk-1.6.6/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.5/huhk/case_project/main.py` & `huhk-1.6.6/huhk/case_project/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.5/huhk/case_project/setup_set.py` & `huhk-1.6.6/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.5/huhk/init_project.py` & `huhk-1.6.6/huhk/init_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,41 +39,46 @@
                             self.yapi_url = self.yapi_url[:-1]
                         self.value = project.get('api_settings')[0].get('token')
             else:
                 self.error = project.get('non_field_errors')[0]
         self.name = self.name or "demo"
         self.name2 = self.name.title()
 
-    def create_project(self):
+    def create_or_update_project(self):
         """
         创建项目
         """
         self.get_project()
-        if self.error:
-            print(self.error)
-            return False
         # 创建项目目录
         self.set_file_path()
         # 获取已维护api方法接口列表
         self.get_api_fun_list()
-        # 获取全量api接口列表
+        # 获取接口文档api接口列表
         self.get_api_list()
         # 添加api封装方法
         self.write_api_fun()
 
     def set_file_path(self):
-        """创建项目目录"""
+        """创建项目框架"""
         if not self.name:
             self.name = os.path.basename(sys.argv[0])
         self.service_dir = os.path.join(service_path, self.name)
         self.testcase_dir = os.path.join(testcase_path, self.name)
         FunBase.mkdir_file([self.service_dir, self.testcase_dir], is_py=False)
+        self.api_dir = os.path.join(self.service_dir, "api")
+        self.fun_dir = os.path.join(self.service_dir, "fun")
+        self.assert_dir = os.path.join(self.service_dir, "assert")
+        self.sql_dir = os.path.join(self.service_dir, "sql")
+        FunBase.mkdir_file([self.api_dir, self.fun_dir, self.assert_dir, self.sql_dir], is_py=True)
         if not os.path.exists(os.path.join(self.service_dir, "__init__.py")):
             FunBase.write_file(os.path.join(self.service_dir, "__init__.py"), value=self.get_init_value())
 
+
+
+
     def get_api_fun_list(self):
         """获取已维护方法列表，无则创建demo文件"""
         self.api_file_path = os.path.join(self.service_dir, self.name + "_api.py")
         if os.path.exists(self.api_file_path):
             self.api_file_str = FunBase.read_file(self.api_file_path)
         else:
             self.api_file_str = "import allure\n\nfrom service.%s import http_requester\n" \
@@ -539,11 +544,10 @@
             for tmp in re.findall(r'[( ]async[,=)]', _str):
                 tmp1 = str(tmp).replace('async', 'async1')
                 _str = _str.replace(tmp, tmp1)
         return _str
 
 
 
-
-
 if __name__ == '__main__':
-    GetApi(app_key="a63ca17b-3cf3-46cb-b8b6-9ad20518e1e1")
+    ga = GetApi(app_key="a63ca17b-3cf3-46cb-b8b6-9ad20518e1e1")
+    ga.set_service_value("new2", "a63ca17b-3cf3-46cb-b8b6-9ad20518e1e1")
```

### Comparing `huhk-1.6.5/huhk/testcase/apache/beam_class.py` & `huhk-1.6.6/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.5/huhk/testcase/apache/data.py` & `huhk-1.6.6/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.5/huhk/testcase/apache/par_do.py` & `huhk-1.6.6/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.5/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.6.6/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from huhk.testcase.apache.data import *
-from huhk.testcase.apache.beam_class import AverageFn, AverageFn2
+from testcase.apache.beam_class import AverageFn, AverageFn2
 from huhk.unit_apache_beam import ApacheFun
 
 
 class TestPolymerization:
     # 通过键聚合所有输入元素，并允许下游处理使用与键关联的所有值
     def test_polymerization_001(self):
         ApacheFun(data_type=data_type).co_group_by_key(icons=data_list_tuple3, durations=data_list_tuple4).print()
```

### Comparing `huhk-1.6.5/huhk/testcase/apache/test_fiter.py` & `huhk-1.6.6/huhk/testcase/apache/test_fiter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from huhk.testcase.apache.data import *
 from huhk.unit_apache_beam import ApacheFun
 
 
 class TestFiter:
     def setup(self):
         self.af = ApacheFun(data_list_dict, data_type=data_type)
```

### Comparing `huhk-1.6.5/huhk/testcase/apache/test_flatmap.py` & `huhk-1.6.6/huhk/testcase/apache/test_flatmap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from huhk.testcase.apache.data import *
 from huhk.unit_apache_beam import ApacheFun
 
 
 class TestFlatmap:
     def setup(self):
         self.af = ApacheFun(data_list_str, data_type=data_type)
```

### Comparing `huhk-1.6.5/huhk/testcase/apache/test_map.py` & `huhk-1.6.6/huhk/testcase/apache/test_map.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from huhk.testcase.apache.data import *
 from huhk.unit_apache_beam import ApacheFun
 
 
 class TestMap:
     # 带有预定义函数的 FlatMap
     def test_map_001(self):
         ApacheFun(data_list_str3, data_type=data_type).map(str.strip).print()
```

### Comparing `huhk-1.6.5/huhk/testcase/apache/test_par_do.py` & `huhk-1.6.6/huhk/testcase/apache/test_par_do.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import random
-from huhk.testcase.apache.data import *
 from huhk.unit_apache_beam import ApacheFun
-from huhk.testcase.apache.beam_class import SplitWords, AnalyzeElement, DoFnMethods
+from testcase.apache.beam_class import SplitWords, AnalyzeElement, DoFnMethods
 
 
 class TestParDo:
     # 有简单 DoFn 的 ParDo
     def test_par_do_001(self):
         ApacheFun(data_list_str2, data_type=data_type).par_do(SplitWords(',')).print()
 
@@ -28,26 +27,26 @@
             return durations.index(plant['duration']) if plant['duration'] in durations else len(durations)
 
         out = ApacheFun(data_list_dict, data_type=data_type).partition(by_duration, 4)
         # out.print("'{}: {}'.format(x['duration'], x)")
         out.value[0].print("'annual: {}'.format(x)")
         out.value[1].print("'biennial: {}'.format(x)")
         out.value[2].print("'perennial: {}'.format(x)")
-        out.create_project()
+        out.create_or_update_project()
 
     # 使用 lambda 函数进行分区
     def test_par_do_005(self):
         durations = ['annual', 'biennial', 'perennial']
         out = ApacheFun(data_list_dict, data_type=data_type).partition(
             lambda plant, num_partitions:
             durations.index(plant['duration']) if plant['duration'] in durations else len(durations), 4)
         out.value[0].print("'annual: {}'.format(x)")
         out.value[1].print("'biennial: {}'.format(x)")
         out.value[2].print("'perennial: {}'.format(x)")
-        out.create_project()
+        out.create_or_update_project()
 
     # 具有多个参数的分区
     def test_par_do_006(self):
 
         def split_dataset(plant, num_partitions, ratio):
             assert num_partitions == len(ratio)
             bucket = random.randint(0, sum(ratio)-1)
@@ -57,8 +56,8 @@
                 if bucket < total:
                     return i
             return len(ratio) - 1
 
         out = ApacheFun(data_list_dict*3).partition(split_dataset, 2, ratio=[10, 20])
         out.value[0].print("'1: {}'.format(x)")
         out.value[1].print("'2: {}'.format(x)")
-        out.create_project()
+        out.create_or_update_project()
```

### Comparing `huhk-1.6.5/huhk/testcase/apache/test_regex.py` & `huhk-1.6.6/huhk/testcase/apache/test_regex.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from huhk.testcase.apache.data import *
 from huhk.unit_apache_beam import ApacheFun
 
 
 class TestRegex:
     # 正则表达式匹配
     def test_regex_001(self):
         ApacheFun(data_list_str4, data_type=data_type).regex_matches(r'(?P<icon>[^\s,]+), *(\w+), *(\w+)').print()
```

### Comparing `huhk-1.6.5/huhk/testcase/apache/test_time.py` & `huhk-1.6.6/huhk/testcase/apache/test_time.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from huhk.testcase.apache.data import *
 from huhk.unit_apache_beam import ApacheFun
 
 
 class TestTimes:
     # 按事件时间标记时间戳
     def test_times_001(self):
         ApacheFun(data_list_dict3, data_type=data_type).timestamped_value("season").print()
```

### Comparing `huhk-1.6.5/huhk/unit_apache_beam.py` & `huhk-1.6.6/huhk/unit_apache_beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 import datetime
-import json
 import time
 import pandas as pd
 import apache_beam as beam
 import uuid
 
 from apache_beam import PCollection
-from apache_beam.coders import Coder, StrUtf8Coder
 from apache_beam.io import fileio
 from apache_beam.pvalue import DoOutputsTuple
 from apache_beam.transforms import window
 
-from huhk.case_project.json_coder import JsonCoder
-
 
 class ApacheFun:
     window = window
 
     def __init__(self, data=None, name="", out=None, data_type=1):
         """data_type: 1 管道， 2 数据"""
 
@@ -516,11 +512,10 @@
             self.value = self.out = self.pipeline | self._name() >> beam.io.ReadFromJson(path, dtype=False, encodings='utf-8')
 
         return self
 
 
 
 if __name__ == '__main__':
-    from huhk.testcase.apache.data import *
     path = r"C:\Users\hangkai.hu\Desktop\测试\雷达用例\111.txt"
     path = r"C:\Users\hangkai.hu\Desktop\测试\雷达用例\222.json"
     ApacheFun().read_file(path).print()
```

### Comparing `huhk-1.6.5/huhk/unit_dict.py` & `huhk-1.6.6/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.5/huhk/unit_encryption.py` & `huhk-1.6.6/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.5/huhk/unit_fun.py` & `huhk-1.6.6/huhk/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.5/huhk/unit_logger.py` & `huhk-1.6.6/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.5/huhk/unit_request.py` & `huhk-1.6.6/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.5/huhk/unit_tasks.py` & `huhk-1.6.6/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.5/huhk/常用命令.py` & `huhk-1.6.6/huhk/常用命令.py`

 * *Files identical despite different names*

