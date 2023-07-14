# Comparing `tmp/envutil-0.2.1.tar.gz` & `tmp/envutil-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envutil-0.2.1.tar", max compression
+gzip compressed data, was "envutil-0.2.3.tar", max compression
```

## Comparing `envutil-0.2.1.tar` & `envutil-0.2.3.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     1881 2023-06-03 20:11:41.633075 envutil-0.2.1/README.md
--rw-r--r--   0        0        0     1826 2023-06-03 17:31:11.833293 envutil-0.2.1/envutil/__init__.py
--rw-r--r--   0        0        0      470 2023-06-03 20:25:46.606889 envutil-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 envutil-0.2.1/setup.py
--rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 envutil-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-03 20:27:17.158850 envutil-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1881 2023-06-03 20:11:41.633075 envutil-0.2.3/README.md
+-rw-r--r--   0        0        0     1826 2023-06-03 17:31:11.833293 envutil-0.2.3/envutil/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 03:09:02.219246 envutil-0.2.3/py.typed
+-rw-r--r--   0        0        0      511 2023-07-14 03:12:06.379826 envutil-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2639 1970-01-01 00:00:00.000000 envutil-0.2.3/setup.py
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 envutil-0.2.3/PKG-INFO
```

### Comparing `envutil-0.2.1/README.md` & `envutil-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `envutil-0.2.1/envutil/__init__.py` & `envutil-0.2.3/envutil/__init__.py`

 * *Files identical despite different names*

### Comparing `envutil-0.2.1/setup.py` & `envutil-0.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,32 @@
 
 packages = \
 ['envutil']
 
 package_data = \
 {'': ['*']}
 
+modules = \
+['py']
 install_requires = \
 ['python-dotenv>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'envutil',
-    'version': '0.2.1',
+    'version': '0.2.3',
     'description': '',
     'long_description': "# Python Environment Variable Helper\n\nThis Python package provides an easy way to interact with environment variables in your Python applications. It is designed to simplify the process of loading and parsing various data types from environment variables.\n\n## Features\n\n- Auto load environment variables from .env files based on application environment (`dev` or `test`).\n- Provide easy-to-use functions to access environment variables with type hinting.\n- Support different data types including strings, lists, dictionaries, integers and booleans.\n- Allow defaults for environment variables.\n- Provide decorator `@depends_on_env` for user-defined functions to ensure environment variables are loaded.\n\n## Installation\n\nInstall the package from PyPi using pip:\n\n```shell\npip install envutil\n```\n\n## Usage\n\nImport the package in your Python code as follows:\n\n```python\nfrom envutil import env_str, env_csv, env_int, env_bool, env_list, env_dict\n```\n\nAccess your environment variables:\n\n```python\n# Access string variable\nmy_var = env_str('MY_VAR', default='default-value')\n\n# Access comma separated value as a list\nmy_csv = env_csv('MY_CSV', default=[])\n\n# Access integer variable\nmy_int = env_int('MY_INT', default=0)\n\n# Access boolean variable\nmy_bool = env_bool('MY_BOOL', default=False)\n\n# Access list variable\nmy_list = env_list('MY_LIST', default=[])\n\n# Access dictionary variable\nmy_dict = env_dict('MY_DICT', default={})\n```\n\n## Environment Configuration\n\nBy default, this package loads `.env` file. If the `APP_ENV` is set to `test`, it will load `.env.test` file. You can also specify a custom environment file by setting the `APP_ENV_FILE` environment variable.\n\n## Contributing\n\nYour contributions are always welcome! Please have a look at the [contribution guidelines](CONTRIBUTING.md) first. 🎉\n\n## License\n\nThis package is released under the [MIT License](LICENSE).",
     'author': 'Berke Arslan',
     'author_email': 'berke@kwilabs.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
+    'py_modules': modules,
     'install_requires': install_requires,
     'python_requires': '>=3.11,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `envutil-0.2.1/PKG-INFO` & `envutil-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envutil
-Version: 0.2.1
+Version: 0.2.3
 Summary: 
 Author: Berke Arslan
 Author-email: berke@kwilabs.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
```

