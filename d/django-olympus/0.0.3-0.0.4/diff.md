# Comparing `tmp/django-olympus-0.0.3.tar.gz` & `tmp/django-olympus-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-olympus-0.0.3.tar", last modified: Wed Mar 23 18:13:40 2022, max compression
+gzip compressed data, was "django-olympus-0.0.4.tar", last modified: Fri Jul 14 08:21:15 2023, max compression
```

## Comparing `django-olympus-0.0.3.tar` & `django-olympus-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:13:40.397706 django-olympus-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-03-23 18:13:26.000000 django-olympus-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-23 18:13:26.000000 django-olympus-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-03-23 18:13:40.397706 django-olympus-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-03-23 18:13:26.000000 django-olympus-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:13:40.397706 django-olympus-0.0.3/django_olympus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-03-23 18:13:40.000000 django-olympus-0.0.3/django_olympus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-03-23 18:13:40.000000 django-olympus-0.0.3/django_olympus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 18:13:40.000000 django-olympus-0.0.3/django_olympus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 18:13:40.000000 django-olympus-0.0.3/django_olympus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-03-23 18:13:40.000000 django-olympus-0.0.3/django_olympus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-03-23 18:13:40.000000 django-olympus-0.0.3/django_olympus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:13:40.397706 django-olympus-0.0.3/olympus/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-03-23 18:13:26.000000 django-olympus-0.0.3/olympus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-03-23 18:13:26.000000 django-olympus-0.0.3/olympus/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     5335 2022-03-23 18:13:26.000000 django-olympus-0.0.3/olympus/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:13:40.397706 django-olympus-0.0.3/olympus/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 18:13:26.000000 django-olympus-0.0.3/olympus/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:13:40.397706 django-olympus-0.0.3/olympus/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 18:13:26.000000 django-olympus-0.0.3/olympus/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3737 2022-03-23 18:13:26.000000 django-olympus-0.0.3/olympus/management/commands/push_to_es.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 18:13:40.397706 django-olympus-0.0.3/olympus/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-03-23 18:13:26.000000 django-olympus-0.0.3/olympus/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-03-23 18:13:40.401706 django-olympus-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-23 18:13:26.000000 django-olympus-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:15.875556 django-olympus-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-14 08:21:06.000000 django-olympus-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 08:21:06.000000 django-olympus-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-14 08:21:15.875556 django-olympus-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-14 08:21:06.000000 django-olympus-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:15.875556 django-olympus-0.0.4/django_olympus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-14 08:21:15.000000 django-olympus-0.0.4/django_olympus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-14 08:21:15.000000 django-olympus-0.0.4/django_olympus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:21:15.000000 django-olympus-0.0.4/django_olympus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:21:15.000000 django-olympus-0.0.4/django_olympus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-14 08:21:15.000000 django-olympus-0.0.4/django_olympus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 08:21:15.000000 django-olympus-0.0.4/django_olympus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:15.875556 django-olympus-0.0.4/olympus/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:15.875556 django-olympus-0.0.4/olympus/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:15.875556 django-olympus-0.0.4/olympus/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/management/commands/push_to_es.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:21:15.875556 django-olympus-0.0.4/olympus/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-14 08:21:06.000000 django-olympus-0.0.4/olympus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-14 08:21:15.875556 django-olympus-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 08:21:06.000000 django-olympus-0.0.4/setup.py
```

### Comparing `django-olympus-0.0.3/LICENSE` & `django-olympus-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-olympus-0.0.3/olympus/apps.py` & `django-olympus-0.0.4/olympus/apps.py`

 * *Files identical despite different names*

### Comparing `django-olympus-0.0.3/olympus/base.py` & `django-olympus-0.0.4/olympus/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
         super().__init__(hosts=hosts, **kwargs)
 
 
 class OlympusCollector:
     index_name: Optional[str] = None
     index_date_pattern: Optional[str] = None
+    index_lifecycle_name: Optional[str] = None
     chunk_size = 500
     alias_suffix = '-latest'
 
     @classmethod
     def __init_subclass__(cls):
         # register collectors - use metaclass if py < 3.6 support is required
         _collectors.append((cls.__module__.split('.')[0], cls.name(), cls))
@@ -54,15 +55,19 @@
         return self.index_name or self.name().lower()
 
     @classmethod
     def name(cls) -> str:
         return f"{cls.__module__.split('.')[0]}.{cls.__name__}"
 
     def create_index(self):
-        self.es.indices.create(index=self.get_index_name(), ignore=400)
+        body = dict()
+        if self.index_lifecycle_name:
+            body["settings"] = {"index.lifecycle.name": self.index_lifecycle_name}
+
+        self.es.indices.create(index=self.get_index_name(), body=body, ignore=400)
         if self.index_date_pattern and self.alias_suffix:
             # Create unique alias for latest index
             alias = self.__get_raw_index_name() + self.alias_suffix
             self.es.indices.delete_alias(index='_all', name=alias, ignore=404)
             self.es.indices.put_alias(index=self.get_index_name(), name=alias)
 
     def fake_push(
```

### Comparing `django-olympus-0.0.3/olympus/management/commands/push_to_es.py` & `django-olympus-0.0.4/olympus/management/commands/push_to_es.py`

 * *Files identical despite different names*

### Comparing `django-olympus-0.0.3/olympus/tests/__init__.py` & `django-olympus-0.0.4/olympus/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-olympus-0.0.3/setup.cfg` & `django-olympus-0.0.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	Topic :: Software Development
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	Django >= 3.0
+	Django >= 3.0, < 4
 	elasticsearch >= 6.8, < 7
 	tqdm >= 4, < 5
 	django-logbasecommand < 1
 python_requires = >=3.9
 
 [options.packages.find]
 exclude =
```

