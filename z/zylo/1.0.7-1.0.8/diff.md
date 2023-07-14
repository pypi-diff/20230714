# Comparing `tmp/zylo-1.0.7.tar.gz` & `tmp/zylo-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zylo-1.0.7.tar", last modified: Wed Jul 12 22:34:00 2023, max compression
+gzip compressed data, was "zylo-1.0.8.tar", last modified: Fri Jul 14 08:26:13 2023, max compression
```

## Comparing `zylo-1.0.7.tar` & `zylo-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:34:00.531790 zylo-1.0.7/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 22:34:00.531790 zylo-1.0.7/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      452 2023-07-12 21:43:58.000000 zylo-1.0.7/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-12 22:34:00.531790 zylo-1.0.7/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      999 2023-07-12 22:33:12.000000 zylo-1.0.7/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:34:00.527789 zylo-1.0.7/zylo/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-07-12 21:29:13.000000 zylo-1.0.7/zylo/JwT.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-12 22:27:01.000000 zylo-1.0.7/zylo/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5641 2023-07-12 21:37:58.000000 zylo-1.0.7/zylo/app.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1030 2023-07-12 19:00:56.000000 zylo-1.0.7/zylo/blueprint.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6491 2023-07-12 20:04:49.000000 zylo-1.0.7/zylo/chiper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-1.0.7/zylo/mailer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-07-12 16:44:47.000000 zylo-1.0.7/zylo/sessions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-12 22:34:00.531790 zylo-1.0.7/zylo.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-07-12 22:34:00.000000 zylo-1.0.7/zylo.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      294 2023-07-12 22:34:00.000000 zylo-1.0.7/zylo.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-12 22:34:00.000000 zylo-1.0.7/zylo.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       35 2023-07-12 22:34:00.000000 zylo-1.0.7/zylo.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-07-12 22:34:00.000000 zylo-1.0.7/zylo.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-12 22:34:00.000000 zylo-1.0.7/zylo.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 08:26:13.691396 zylo-1.0.8/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1672 2023-07-14 08:26:13.691396 zylo-1.0.8/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1046 2023-07-14 08:24:50.000000 zylo-1.0.8/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-14 08:26:13.691396 zylo-1.0.8/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      999 2023-07-14 06:14:40.000000 zylo-1.0.8/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 08:26:13.691396 zylo-1.0.8/zylo/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-07-14 08:14:27.000000 zylo-1.0.8/zylo/JwT.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-14 06:52:19.000000 zylo-1.0.8/zylo/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6002 2023-07-14 06:36:57.000000 zylo-1.0.8/zylo/app.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-14 06:48:09.000000 zylo-1.0.8/zylo/blueprint.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6341 2023-07-14 06:35:56.000000 zylo-1.0.8/zylo/chiper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2346 2023-07-14 06:25:13.000000 zylo-1.0.8/zylo/limiter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2847 2023-07-12 20:05:30.000000 zylo-1.0.8/zylo/mailer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-07-12 16:44:47.000000 zylo-1.0.8/zylo/sessions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-14 08:26:13.691396 zylo-1.0.8/zylo.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1672 2023-07-14 08:26:13.000000 zylo-1.0.8/zylo.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      310 2023-07-14 08:26:13.000000 zylo-1.0.8/zylo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-14 08:26:13.000000 zylo-1.0.8/zylo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       35 2023-07-14 08:26:13.000000 zylo-1.0.8/zylo.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-07-14 08:26:13.000000 zylo-1.0.8/zylo.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-07-14 08:26:13.000000 zylo-1.0.8/zylo.egg-info/top_level.txt
```

### Comparing `zylo-1.0.7/PKG-INFO` & `zylo-1.0.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 1.0.7
+Version: 1.0.8
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,9 +46,38 @@
 
 @app.route('/')
 def home(request):
     return 'Hello, World!'
 
 if __name__ == '__main__':
     app.run()
+ 
+```
+
+## changelogs
+
+- Beta version 1.0.8
+- Added Limiter ( from zylo.limiter import Limiter )
+- New init app=(__name__)
+- Function run() update --> run(host, port, debug)
+- JwT updated to vesion --> 1.0.2
+- Bug fixed with update --> 1.0.8
+- zylo-admin library added, usage will be disclosed soon
+- Improved session management
+
+
+```python
+
+from zylo.limiter import Limiter, render_template
 
+app = Zylo(__name__)
+limiter = Limiter(app)
+
+@app.route('/', methods=['GET', 'POST'])
+@limiter.limit('10/minutes')
+    return render_template('index.html')
+
+if __name__ == '__main__':
+    app.run()
+
+```
```

### Comparing `zylo-1.0.7/setup.py` & `zylo-1.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='zylo',
-    version='1.0.7',
+    version='1.0.8',
     description='A lightweight web framework made with love',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Pawan kumar',
     author_email='control@vvfin.in',
     url='https://github.com/E491K7/zylo',
     packages=find_packages(),
```

### Comparing `zylo-1.0.7/zylo/JwT.py` & `zylo-1.0.8/zylo/JwT.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,16 @@
         
     def create_payload(self, payload, algorithm='HS256', time_limit_hours=24):
         now = datetime.utcnow()
         payload['iat'] = now
         payload['exp'] = now + timedelta(hours=time_limit_hours)
         return self.encode(payload, algorithm, time_limit_hours)
 
-    def verify_payload(self, access_token):
-        return self.verify_token(access_token)
+    def verify_payload(self, token):
+        return self.verify_token(token)
 
     def decode_payload(self, refresh_token, algorithm='HS256', time_limit_hours=24):
         try:
             payload = self.verify_token(refresh_token)
             if 'exp' in payload:
                 del payload['exp']
             if 'iat' in payload:
```

### Comparing `zylo-1.0.7/zylo/app.py` & `zylo-1.0.8/zylo/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import json
 from werkzeug.wrappers import Request, Response
 from werkzeug.routing import Map, Rule
 from werkzeug.exceptions import HTTPException, default_exceptions, NotFound, MethodNotAllowed
 from jinja2 import Environment, FileSystemLoader
 from .sessions import SessionManager
 from werkzeug.urls import url_encode
+from .limiter import Limiter
 import os
 import mimetypes
 
 class Zylo:
-    def __init__(self,  host='localhost', port=8000, debug=True):
-        self.host = host
-        self.port = port
-        self.debug = debug
+    def __init__(self, __name__={} ):
         self.url_map = Map()
         self.routes = {}
         self.template_env = Environment(loader=FileSystemLoader('views'))
         self.static_folder = 'static'
         self.session_manager = SessionManager()
         self.blueprints = []
         self.template_folder = None
+        self.limiter = Limiter()
+        self.before_request_funcs = []
+        self.after_request_funcs = []
+        self.__name__ = __name__
 
-    def route(self, rule, methods=['GET'], endpoint=None):
+    def route(self, rule, methods=['GET'], endpoint=None,):
         def decorator(func):
             self.routes[endpoint or func.__name__] = (rule, methods, func)
             return func
         return decorator
 
     def register_blueprint(self, blueprint):
         self.blueprints.append(blueprint)
@@ -37,17 +39,28 @@
     def serve_static(self, filename):
         static_path = os.path.join(self.static_folder, filename)
         if os.path.isfile(static_path):
             mimetype, _ = mimetypes.guess_type(static_path)
             if mimetype:
                 return Response(open(static_path, 'rb').read(), mimetype=mimetype)
         raise NotFound()
+    
+    def before_request(self, func):
+        self.before_request_funcs.append(func)
+        return func
+
+    def after_request(self, func):
+        self.after_request_funcs.append(func)
+        return func
 
-    def run(self):
+    def run(self, host='localhost', port=8000, debug=True):
         app = self
+        host = host
+        port = port
+        debug = debug
 
         @Request.application
         def application(request):
             try:
                 session_token = request.cookies.get('session_token')
                 session_data = app.session_manager.get_session(session_token)
                 request.session = session_data
@@ -82,27 +95,27 @@
                     app.session_manager.update_session(session_token, request.session)
 
                 return response
 
             except HTTPException as e:
                 return e
 
-        if self.debug:
+        if debug:
             from werkzeug.debug import DebuggedApplication
             application = DebuggedApplication(application, evalex=True)
 
         for endpoint, (rule, _, _) in self.routes.items():
             self.url_map.add(Rule(rule, endpoint=endpoint))
             print(f"Registered route: {rule} --> {endpoint}")
 
         for blueprint in self.blueprints:
             blueprint.register(self)
 
         from werkzeug.serving import run_simple
-        run_simple(self.host, self.port, application, use_reloader=self.debug)
+        run_simple(host, port, application, use_reloader=debug)
 
 app = Zylo()
 
 def render_template(template_name, **kwargs):
     template = app.template_env.get_template(template_name)
     kwargs['url_for_static'] = app.url_for_static
     return Response(template.render(**kwargs), mimetype='text/html')
```

### Comparing `zylo-1.0.7/zylo/chiper.py` & `zylo-1.0.8/zylo/chiper.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,11 +196,7 @@
 
 def sanitize_sql_input(input_string):
     return re.sub(r"[\'\";]", '', input_string)
 
 
 def sanitize_nosql_input(input_string):
     return input_string.replace('$', '').replace('.', '')
-
-input_string = ",& SELCET * FROM user WHERE name = 'name''"
-sanitized_input = sanitize_input(input_string)
-print("Sanitized input:", sanitized_input)
```

### Comparing `zylo-1.0.7/zylo/mailer.py` & `zylo-1.0.8/zylo/mailer.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.7/zylo/sessions.py` & `zylo-1.0.8/zylo/sessions.py`

 * *Files identical despite different names*

### Comparing `zylo-1.0.7/zylo.egg-info/PKG-INFO` & `zylo-1.0.8/zylo.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zylo
-Version: 1.0.7
+Version: 1.0.8
 Summary: A lightweight web framework made with love
 Home-page: https://github.com/E491K7/zylo
 Author: Pawan kumar
 Author-email: control@vvfin.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,9 +46,38 @@
 
 @app.route('/')
 def home(request):
     return 'Hello, World!'
 
 if __name__ == '__main__':
     app.run()
+ 
+```
+
+## changelogs
+
+- Beta version 1.0.8
+- Added Limiter ( from zylo.limiter import Limiter )
+- New init app=(__name__)
+- Function run() update --> run(host, port, debug)
+- JwT updated to vesion --> 1.0.2
+- Bug fixed with update --> 1.0.8
+- zylo-admin library added, usage will be disclosed soon
+- Improved session management
+
+
+```python
+
+from zylo.limiter import Limiter, render_template
 
+app = Zylo(__name__)
+limiter = Limiter(app)
+
+@app.route('/', methods=['GET', 'POST'])
+@limiter.limit('10/minutes')
+    return render_template('index.html')
+
+if __name__ == '__main__':
+    app.run()
+
+```
```

