# Comparing `tmp/django_auth_dingding-0.0.2.tar.gz` & `tmp/django_auth_dingding-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_auth_dingding-0.0.2.tar", last modified: Wed May 24 09:11:48 2023, max compression
+gzip compressed data, was "django_auth_dingding-0.0.3.tar", last modified: Fri Jul 14 02:33:32 2023, max compression
```

## Comparing `django_auth_dingding-0.0.2.tar` & `django_auth_dingding-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 09:11:48.429118 django_auth_dingding-0.0.2/
--rw-rw-rw-   0        0        0     1556 2023-05-24 06:39:11.000000 django_auth_dingding-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1951 2023-05-24 09:11:48.429118 django_auth_dingding-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1395 2023-05-24 08:53:31.000000 django_auth_dingding-0.0.2/README.md
--rw-rw-rw-   0        0        0      634 2023-05-24 09:11:31.000000 django_auth_dingding-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 09:11:48.429118 django_auth_dingding-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 09:11:48.409576 django_auth_dingding-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 09:11:48.423246 django_auth_dingding-0.0.2/src/django_auth_dingding/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.2/src/django_auth_dingding/__init__.py
--rw-rw-rw-   0        0        0      170 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.2/src/django_auth_dingding/apps.py
--rw-rw-rw-   0        0        0     1787 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.2/src/django_auth_dingding/auth.py
--rw-rw-rw-   0        0        0       57 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.2/src/django_auth_dingding/models.py
--rw-rw-rw-   0        0        0       60 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.2/src/django_auth_dingding/tests.py
--rw-rw-rw-   0        0        0      628 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.2/src/django_auth_dingding/urls.py
--rw-rw-rw-   0        0        0      507 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.2/src/django_auth_dingding/utils.py
--rw-rw-rw-   0        0        0     5974 2023-05-24 09:06:21.000000 django_auth_dingding-0.0.2/src/django_auth_dingding/views.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:11:48.428128 django_auth_dingding-0.0.2/src/django_auth_dingding.egg-info/
--rw-rw-rw-   0        0        0     1951 2023-05-24 09:11:48.000000 django_auth_dingding-0.0.2/src/django_auth_dingding.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      497 2023-05-24 09:11:48.000000 django_auth_dingding-0.0.2/src/django_auth_dingding.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 09:11:48.000000 django_auth_dingding-0.0.2/src/django_auth_dingding.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-24 09:11:48.000000 django_auth_dingding-0.0.2/src/django_auth_dingding.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 02:33:32.285858 django_auth_dingding-0.0.3/
+-rw-rw-rw-   0        0        0     1556 2023-05-24 06:39:11.000000 django_auth_dingding-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1951 2023-07-14 02:33:32.284878 django_auth_dingding-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1395 2023-05-24 08:53:31.000000 django_auth_dingding-0.0.3/README.md
+-rw-rw-rw-   0        0        0      634 2023-07-14 02:27:27.000000 django_auth_dingding-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-14 02:33:32.285858 django_auth_dingding-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 02:33:32.265349 django_auth_dingding-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 02:33:32.279996 django_auth_dingding-0.0.3/src/django_auth_dingding/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.3/src/django_auth_dingding/__init__.py
+-rw-rw-rw-   0        0        0      170 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.3/src/django_auth_dingding/apps.py
+-rw-rw-rw-   0        0        0     1787 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.3/src/django_auth_dingding/auth.py
+-rw-rw-rw-   0        0        0       57 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.3/src/django_auth_dingding/models.py
+-rw-rw-rw-   0        0        0       60 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.3/src/django_auth_dingding/tests.py
+-rw-rw-rw-   0        0        0      628 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.3/src/django_auth_dingding/urls.py
+-rw-rw-rw-   0        0        0      507 2023-05-24 06:31:51.000000 django_auth_dingding-0.0.3/src/django_auth_dingding/utils.py
+-rw-rw-rw-   0        0        0     6006 2023-07-14 02:27:08.000000 django_auth_dingding-0.0.3/src/django_auth_dingding/views.py
+drwxrwxrwx   0        0        0        0 2023-07-14 02:33:32.283902 django_auth_dingding-0.0.3/src/django_auth_dingding.egg-info/
+-rw-rw-rw-   0        0        0     1951 2023-07-14 02:33:32.000000 django_auth_dingding-0.0.3/src/django_auth_dingding.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2023-07-14 02:33:32.000000 django_auth_dingding-0.0.3/src/django_auth_dingding.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 02:33:32.000000 django_auth_dingding-0.0.3/src/django_auth_dingding.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-14 02:33:32.000000 django_auth_dingding-0.0.3/src/django_auth_dingding.egg-info/top_level.txt
```

### Comparing `django_auth_dingding-0.0.2/LICENSE` & `django_auth_dingding-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_auth_dingding-0.0.2/PKG-INFO` & `django_auth_dingding-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_auth_dingding
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Dingding auth Django app.
 Author-email: quanbisen <1769128867@qq.com>
 Project-URL: Homepage, https://github.com/quanbisen/django-dingding-auth
 Project-URL: Bug Tracker, https://github.com/quanbisen/django-dingding-auth/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `django_auth_dingding-0.0.2/README.md` & `django_auth_dingding-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django_auth_dingding-0.0.2/pyproject.toml` & `django_auth_dingding-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_auth_dingding"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="quanbisen", email="1769128867@qq.com" },
 ]
 description = "A simple Dingding auth Django app."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_auth_dingding-0.0.2/src/django_auth_dingding/auth.py` & `django_auth_dingding-0.0.3/src/django_auth_dingding/auth.py`

 * *Files identical despite different names*

### Comparing `django_auth_dingding-0.0.2/src/django_auth_dingding/urls.py` & `django_auth_dingding-0.0.3/src/django_auth_dingding/urls.py`

 * *Files identical despite different names*

### Comparing `django_auth_dingding-0.0.2/src/django_auth_dingding/views.py` & `django_auth_dingding-0.0.3/src/django_auth_dingding/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,13 +133,14 @@
 
         params = {
             "response_type": "code",
             "scope": "openid",
             "client_id": self.AUTH_DINGDING_APP_KEY,
             "redirect_uri": callback_url,
             "state": "dddd",
+            "prompt": "consent"
         }
         query = urlencode(params)
         redirect_url = "{url}?{query}".format(
             url=self.AUTH_DINGDING_AUTHORIZATION_ENDPOINT, query=query
         )
         return HttpResponseRedirect(redirect_url)
```

### Comparing `django_auth_dingding-0.0.2/src/django_auth_dingding.egg-info/PKG-INFO` & `django_auth_dingding-0.0.3/src/django_auth_dingding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-auth-dingding
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Dingding auth Django app.
 Author-email: quanbisen <1769128867@qq.com>
 Project-URL: Homepage, https://github.com/quanbisen/django-dingding-auth
 Project-URL: Bug Tracker, https://github.com/quanbisen/django-dingding-auth/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

