# Comparing `tmp/keras_eo-2023.7.14.tar.gz` & `tmp/keras_eo-2023.7.14.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_eo-2023.7.14.tar", max compression
+gzip compressed data, was "keras_eo-2023.7.14.post2.tar", max compression
```

## Comparing `keras_eo-2023.7.14.tar` & `keras_eo-2023.7.14.post2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       57 2023-07-14 10:18:40.980916 keras_eo-2023.7.14/README.md
--rw-r--r--   0        0        0       24 2023-07-14 10:23:40.569522 keras_eo-2023.7.14/keras_eo/__init__.py
--rw-r--r--   0        0        0       50 2023-07-14 10:22:04.205354 keras_eo-2023.7.14/keras_eo/hello.py
--rw-r--r--   0        0        0      351 2023-07-14 10:19:56.287692 keras_eo-2023.7.14/pyproject.toml
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 keras_eo-2023.7.14/setup.py
--rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 keras_eo-2023.7.14/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-07-14 10:28:08.407296 keras_eo-2023.7.14.post2/README.md
+-rw-r--r--   0        0        0       24 2023-07-14 10:23:40.569522 keras_eo-2023.7.14.post2/keras_eo/__init__.py
+-rw-r--r--   0        0        0       50 2023-07-14 10:22:04.205354 keras_eo-2023.7.14.post2/keras_eo/hello.py
+-rw-r--r--   0        0        0      352 2023-07-14 10:36:06.374908 keras_eo-2023.7.14.post2/pyproject.toml
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 keras_eo-2023.7.14.post2/setup.py
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 keras_eo-2023.7.14.post2/PKG-INFO
```

### Comparing `keras_eo-2023.7.14/setup.py` & `keras_eo-2023.7.14.post2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 ['keras_eo']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'keras-eo',
-    'version': '2023.7.14',
+    'version': '2023.7.14.post2',
     'description': 'Deep Learning for Earth Observation with Keras',
-    'long_description': '# kerasEO\nDeep learning for Earth Observation with Keras\n',
+    'long_description': '# KerasEO\n\nDeep learning for Earth Observation with Keras\n',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

