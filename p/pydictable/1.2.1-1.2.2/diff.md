# Comparing `tmp/pydictable-1.2.1.tar.gz` & `tmp/pydictable-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydictable-1.2.1.tar", last modified: Thu Jun 29 07:29:08 2023, max compression
+gzip compressed data, was "pydictable-1.2.2.tar", last modified: Fri Jul 14 12:18:29 2023, max compression
```

## Comparing `pydictable-1.2.1.tar` & `pydictable-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:08.670897 pydictable-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-29 07:28:59.000000 pydictable-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-29 07:29:08.670897 pydictable-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-29 07:28:59.000000 pydictable-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:08.666897 pydictable-1.2.1/pydictable/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 07:28:59.000000 pydictable-1.2.1/pydictable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-06-29 07:28:59.000000 pydictable-1.2.1/pydictable/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-06-29 07:28:59.000000 pydictable-1.2.1/pydictable/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    30771 2023-06-29 07:28:59.000000 pydictable-1.2.1/pydictable/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-29 07:28:59.000000 pydictable-1.2.1/pydictable/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-29 07:28:59.000000 pydictable-1.2.1/pydictable/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:08.670897 pydictable-1.2.1/pydictable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-29 07:29:08.000000 pydictable-1.2.1/pydictable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-29 07:29:08.000000 pydictable-1.2.1/pydictable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:29:08.000000 pydictable-1.2.1/pydictable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 07:29:08.000000 pydictable-1.2.1/pydictable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 07:29:08.670897 pydictable-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-29 07:28:59.000000 pydictable-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:29.561802 pydictable-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 12:18:18.000000 pydictable-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-14 12:18:29.561802 pydictable-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-14 12:18:18.000000 pydictable-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:29.561802 pydictable-1.2.2/pydictable/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-14 12:18:18.000000 pydictable-1.2.2/pydictable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-14 12:18:18.000000 pydictable-1.2.2/pydictable/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-07-14 12:18:18.000000 pydictable-1.2.2/pydictable/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31393 2023-07-14 12:18:18.000000 pydictable-1.2.2/pydictable/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-14 12:18:18.000000 pydictable-1.2.2/pydictable/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-14 12:18:18.000000 pydictable-1.2.2/pydictable/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:29.561802 pydictable-1.2.2/pydictable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-14 12:18:29.000000 pydictable-1.2.2/pydictable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-14 12:18:29.000000 pydictable-1.2.2/pydictable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:18:29.000000 pydictable-1.2.2/pydictable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 12:18:29.000000 pydictable-1.2.2/pydictable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:18:29.561802 pydictable-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-14 12:18:18.000000 pydictable-1.2.2/setup.py
```

### Comparing `pydictable-1.2.1/LICENSE` & `pydictable-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydictable-1.2.1/README.md` & `pydictable-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pydictable-1.2.1/pydictable/core.py` & `pydictable-1.2.2/pydictable/core.py`

 * *Files identical despite different names*

### Comparing `pydictable-1.2.1/pydictable/field.py` & `pydictable-1.2.2/pydictable/field.py`

 * *Files 5% similar despite different names*

```diff
@@ -352,14 +352,15 @@
     def from_dict(self, v):
         return v
 
     def to_dict(self, v):
         return v
 
     def validate_dict(self, field_name: str, v):
+        assert isinstance(v, str)
         assert re.match(self.regex_string, v), f"{v} for {field_name} should be in proper format"
 
     def validate(self, field_name: str, v):
         assert isinstance(v, str)
 
     def of(self):
         return {'regex': self.regex_string}
@@ -374,14 +375,15 @@
     def from_dict(self, v):
         return v
 
     def to_dict(self, v):
         return v
 
     def validate_dict(self, field_name: str, v):
+        assert isinstance(v, int)
         assert self.min_val <= v <= self.max_val, \
             f"{v} for {field_name} should be in range {self.min_val} to {self.max_val}"
 
     def validate(self, field_name: str, v):
         assert isinstance(v, int)
 
     def of(self):
@@ -397,14 +399,15 @@
     def from_dict(self, v):
         return v
 
     def to_dict(self, v):
         return v
 
     def validate_dict(self, field_name: str, v):
+        assert isinstance(v, float)
         assert self.min_val <= v <= self.max_val, \
             f"{v} for {field_name} should be in range {self.min_val} to {self.max_val}"
 
     def validate(self, field_name: str, v):
         assert isinstance(v, float)
 
     def of(self):
```

### Comparing `pydictable-1.2.1/pydictable/test_core.py` & `pydictable-1.2.2/pydictable/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -809,14 +809,19 @@
 
         try:
             Profile(dict={'email': 'xyz'})
         except DataValidationError as e:
             self.assertEqual(e.err, 'Pre check failed: xyz for email should be in proper format')
 
         try:
+            Profile(dict={'email': 1234567})
+        except DataValidationError as e:
+            self.assertEqual(e.err, 'Pre check failed: Invalid value 1234567 for field email')
+
+        try:
             Profile(dict={'email': 'abc@gmail.com', 'panNumber': '12345'})
         except DataValidationError as e:
             self.assertEqual(e.err, 'Pre check failed: 12345 for panNumber should be in proper format')
 
         profile = Profile(dict={'email': 'abc@gmail.com', 'panNumber': 'ABCDE1234H'})
 
         self.assertEqual(
@@ -838,19 +843,29 @@
 
         try:
             Profile(dict={'salary': 10000000})
         except DataValidationError as e:
             self.assertEqual(e.err, 'Pre check failed: 10000000 for salary should be in range 1000 to 100000')
 
         try:
+            Profile(dict={'salary': True})
+        except DataValidationError as e:
+            self.assertEqual(e.err, 'Pre check failed: True for salary should be in range 1000 to 100000')
+
+        try:
             Profile(dict={'salary': 10000, 'expenses': 100000.0})
         except DataValidationError as e:
             self.assertEqual(e.err, 'Pre check failed: 100000.0 for expenses should be in range 0.0 to 10000.0')
 
         try:
+            Profile(dict={'salary': 10000, 'expenses': '100000.0'})
+        except DataValidationError as e:
+            self.assertEqual(e.err, 'Pre check failed: Invalid value 100000.0 for field expenses')
+
+        try:
             Profile(dict={'salary': 100000, 'expenses': 1000.0, 'donation': 10.0})
         except DataValidationError as e:
             self.assertEqual(e.err, 'Pre check failed: 10.0 for donation should be in range 100.0 to inf')
 
         profile = Profile(dict={'salary': 10000, 'expenses': 1000.0, 'donation': 1000.0})
 
         self.assertEqual(
```

### Comparing `pydictable-1.2.1/pydictable/test_field.py` & `pydictable-1.2.2/pydictable/test_field.py`

 * *Files identical despite different names*

### Comparing `pydictable-1.2.1/pydictable/type.py` & `pydictable-1.2.2/pydictable/type.py`

 * *Files identical despite different names*

### Comparing `pydictable-1.2.1/setup.py` & `pydictable-1.2.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='pydictable',
-    version='1.2.1',
+    version='1.2.2',
     author='Pramod Kumar',
     author_email='pramodkumar.damam73@gmail.com',
     description='Make your classes from/to dict',
     url='https://github.com/pskd73/pydictable.git',
     packages=['pydictable'],
     include_package_data=True,
     long_description='A tool to create data modals from dict and convert it to dict. '
```

