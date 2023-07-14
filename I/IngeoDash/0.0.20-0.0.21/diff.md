# Comparing `tmp/IngeoDash-0.0.20.tar.gz` & `tmp/IngeoDash-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IngeoDash-0.0.20.tar", last modified: Thu Jul 13 16:46:58 2023, max compression
+gzip compressed data, was "IngeoDash-0.0.21.tar", last modified: Fri Jul 14 19:00:10 2023, max compression
```

## Comparing `IngeoDash-0.0.20.tar` & `IngeoDash-0.0.21.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:46:58.165298 IngeoDash-0.0.20/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:46:58.165298 IngeoDash-0.0.20/IngeoDash/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:46:58.165298 IngeoDash-0.0.20/IngeoDash/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/IngeoDash/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:46:58.165298 IngeoDash-0.0.20/IngeoDash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-13 16:46:58.000000 IngeoDash-0.0.20/IngeoDash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-13 16:46:58.000000 IngeoDash-0.0.20/IngeoDash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:46:58.000000 IngeoDash-0.0.20/IngeoDash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-13 16:46:58.000000 IngeoDash-0.0.20/IngeoDash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 16:46:58.000000 IngeoDash-0.0.20/IngeoDash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-13 16:46:58.165298 IngeoDash-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:46:58.165298 IngeoDash-0.0.20/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-13 16:45:05.000000 IngeoDash-0.0.20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:00:10.350079 IngeoDash-0.0.21/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:00:10.346079 IngeoDash-0.0.21/IngeoDash/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:00:10.350079 IngeoDash-0.0.21/IngeoDash/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/IngeoDash/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:00:10.350079 IngeoDash-0.0.21/IngeoDash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-14 19:00:10.000000 IngeoDash-0.0.21/IngeoDash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-14 19:00:10.000000 IngeoDash-0.0.21/IngeoDash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:00:10.000000 IngeoDash-0.0.21/IngeoDash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-14 19:00:10.000000 IngeoDash-0.0.21/IngeoDash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 19:00:10.000000 IngeoDash-0.0.21/IngeoDash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-14 19:00:10.350079 IngeoDash-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:00:10.350079 IngeoDash-0.0.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-14 18:58:10.000000 IngeoDash-0.0.21/setup.py
```

### Comparing `IngeoDash-0.0.20/IngeoDash/__init__.py` & `IngeoDash-0.0.21/IngeoDash/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.annotate import label_column, flip_label, store, similarity
 
-__version__ = '0.0.20'
+__version__ = '0.0.21'
```

### Comparing `IngeoDash-0.0.20/IngeoDash/__main__.py` & `IngeoDash-0.0.21/IngeoDash/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,29 +7,33 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from IngeoDash.app import table_next, download, progress, update_row, download_component, table, table_component
+from IngeoDash.app import table_next, download, progress, update_row, download_component, table, table_component, table_prev
 from IngeoDash.upload import upload, upload_component
 from IngeoDash.config import CONFIG
-from dash import dcc, Output, Input, callback, Dash, State
+from dash import dcc, Output, Input, callback, Dash, State, ctx
 import dash_bootstrap_components as dbc
 
 
 @callback(
     Output(CONFIG.store, 'data'),
     Input(CONFIG.next, 'n_clicks'),
+    Input(CONFIG.prev, 'n_clicks'),    
     State(CONFIG.store, 'data'),
-    prevent_initial_call=True)
-def table_next_callback(next, mem):
+    prevent_initial_call=True
+)
+def table_next_callback(next, prev, mem):
     mem = CONFIG(mem)
-    return table_next(mem)
+    if ctx.triggered_id == mem.next:
+        return table_next(mem)
+    return table_prev(mem)
 
 
 @callback(
     Output(CONFIG.center, 'children'),
     Input(CONFIG.store, 'data'),
     prevent_initial_call=True    
 )
@@ -68,20 +72,23 @@
     return download(mem, filename)
 
 
 @callback(
     Output(CONFIG.store, 'data', allow_duplicate=True),
     Input(CONFIG.upload, 'contents'),
     State(CONFIG.lang, 'value'),
+    State(CONFIG.text, 'value'),
+    State(CONFIG.label_header, 'value'),
     State(CONFIG.store, 'data'),
     prevent_initial_call=True
 )
-def upload_callback(content, lang, mem):
+def upload_callback(content, lang, text, label, mem):
     mem = CONFIG(mem)
-    return upload(mem, content, lang=lang)
+    return upload(mem, content, lang=lang,
+                  text=text, label=label)
 
 
 def run():
     app = Dash(external_stylesheets=[dbc.themes.BOOTSTRAP],
                suppress_callback_exceptions=True)
 
     app.layout = dbc.Container([dcc.Loading(children=dcc.Store(CONFIG.store),
```

### Comparing `IngeoDash-0.0.20/IngeoDash/annotate.py` & `IngeoDash-0.0.21/IngeoDash/annotate.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.20/IngeoDash/app.py` & `IngeoDash-0.0.21/IngeoDash/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,29 +25,45 @@
 def mock_data():
     from EvoMSA.tests.test_base import TWEETS
     from microtc.utils import tweet_iterator
     return [{'text': x['text']}
             for x in tweet_iterator(TWEETS) if x['klass'] in ['P', 'N']]
 
 
-def table_next(mem: Config):
+def table_next(mem: Config, call_next=label_column):
     store(mem)
     db = CONFIG.db[mem[mem.username]]
-    init = mem[mem.n]
     data = db[mem.original]
     if len(data):
         rest = data[mem.n_value:]
         data = data[:mem.n_value]
-        mem[mem.n] = init + mem.n_value
     else:
         data = []
         rest = []
     db[mem.data] = data
     db[mem.original] = rest
-    label_column(mem)        
+    if call_next is not None:
+        call_next(mem)       
+    return json.dumps(mem.mem)
+
+
+def table_prev(mem: Config):
+    db = CONFIG.db[mem[mem.username]]
+    nvalue = mem.n_value
+    if mem.permanent not in db:
+        return json.dumps(mem.mem)
+    permanent = db[mem.permanent]
+    if len(permanent) == 0:
+        return json.dumps(mem.mem)
+    nvalue = nvalue if len(permanent) >= nvalue else len(permanent)
+    data = db[mem.data] if mem.data in db else []
+    original = db[mem.original] if mem.original in db else []
+    db[mem.original] = data + original
+    db[mem.data] = permanent[-nvalue:]
+    db[mem.permanent] = permanent[:-nvalue]
     return json.dumps(mem.mem)
 
 
 def table(mem: Config):
     if mem.username in mem:
         data = CONFIG.db[mem[mem.username]][mem.data]
     else:
@@ -58,21 +74,26 @@
                                             'height': 'auto'},
                                 style_header={'fontWeight': 'bold',
                                               'textAlign': 'left'},
                                 id=CONFIG.data)
 
 
 def table_component():
-    return dbc.Stack([dbc.Progress(value=0, id=CONFIG.progress),
-                      html.Div(id=CONFIG.center,
-                               children=table(CONFIG)),
+    buttons = dbc.ButtonGroup([dbc.Button('Previous',
+                                 color='secondary',
+                                 id=CONFIG.prev),
                       dbc.Button('Next', 
                                  color='primary', 
                                  id=CONFIG.next,
                                  n_clicks=0)])
+    return dbc.Stack([dbc.Progress(value=0, id=CONFIG.progress),
+                      html.Div(id=CONFIG.center,
+                               children=table(CONFIG)),
+                      buttons
+                      ])
 
 
 def user(mem: Config):
     try:
         username = mem[mem.username]
     except KeyError:
         for i in range(10):
@@ -86,21 +107,23 @@
     except KeyError:
         db = dict()
         CONFIG.db[username] = db
     return username, db
            
 
 def progress(mem: Config):
-    if mem.size not in mem:
+    if mem.username not in mem:
         return 0
-    tot = mem[mem.size]
+    db = CONFIG.db[mem[mem.username]]
+    data = len(db[mem.data]) if mem.data in db else 0
+    ori = len(db[mem.original]) if mem.original in db else 0
+    tot = mem[mem.size] if mem.size in mem else data + ori 
     if tot == 0:
-        return 100
-    n = mem[mem.n]
-    return np.ceil(100 * n / tot)
+        return 0
+    return np.ceil(100 * (tot - ori) / tot)
 
 
 def update_row(mem: Config, table: dict):
     data = flip_label(mem, k=table['row'])
     patch = Patch()
     del patch[table['row']]
     patch.insert(table['row'], data)
```

### Comparing `IngeoDash-0.0.20/IngeoDash/config.py` & `IngeoDash-0.0.21/IngeoDash/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,41 +24,41 @@
     label_header: str = 'klass'
     data: str = 'corpus'
     permanent: str = 'permanent'
     original: str = 'original'
     next: str = 'next'
     next_label: str = 'Next'
     n_value: int = 10
-    n: str = 'N'
     size: str = 'size'
     progress: str = 'progress'
     download: str = 'download'
     filename: str = 'filename'
     save: str = 'save'
     center: str = 'center'
     upload: str = 'upload'
     lang: str = 'lang'
     n_jobs: int = 1
     denseBoW: dict = field(default_factory=dict)
     db: dict = field(default_factory=dict)
     username: str = 'username'
     text: str = 'text'
     mem: dict = field(default_factory=dict)
+    prev: str='previous'
 
     def __getitem__(self, key):
         return self.mem[key]
     
     def __setitem__(self, key, value):
         self.mem[key] = value
 
     def __call__(self, value):
         cls = deepcopy(self)
         if value is not None:
             cls.mem = json.loads(value) if isinstance(value, str) else value
-        for key in ['label_header', 'text']:
+        for key in ['label_header', 'text', 'n_value']:
             if key in cls.mem:
                 setattr(cls, key, cls.mem[key])
         return cls
     
     def __contains__(self, key):
         return key in self.mem
```

### Comparing `IngeoDash-0.0.20/IngeoDash/tests/test_annotate.py` & `IngeoDash-0.0.21/IngeoDash/tests/test_annotate.py`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.20/IngeoDash/tests/test_app.py` & `IngeoDash-0.0.21/IngeoDash/tests/test_app.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from IngeoDash.app import mock_data, table_next, download, progress, user, update_row, download_component, table_component
+from IngeoDash.app import mock_data, table_next, download, progress, user, update_row, download_component, table_component, table_prev
 from IngeoDash.annotate import label_column
 from IngeoDash.config import Config
 from IngeoDash.config import CONFIG
 from EvoMSA.tests.test_base import TWEETS
 
 
 def test_mock_data():
@@ -35,30 +35,51 @@
     mem = CONFIG({CONFIG.username: username})
     username, db = user(mem)
     assert 'hola' in CONFIG.db[username]
 
 
 def test_table_next():
     D = mock_data()[:15]
-    mem = CONFIG({CONFIG.username: 'xxx',
-                  CONFIG.n: CONFIG.n_value})
+    mem = CONFIG({CONFIG.username: 'xxx'})
     CONFIG.db['xxx'] = {mem.data: D[:mem.n_value],
                         mem.original: D[mem.n_value:]}
     db = CONFIG.db['xxx']
     label_column(mem)
     size = len(D)
     _ = table_next(mem)
     assert len(db[mem.permanent]) == mem.n_value
-    assert mem[mem.n] == 2 * mem.n_value
     assert len(db[mem.data]) == 5
     _ = table_next(mem)
     assert len(db[mem.data]) == 0
     assert len(db[mem.original]) == 0
 
 
+def test_table_prev():
+    mem = CONFIG({CONFIG.username: 'xxx', 'n_value': 10})
+    CONFIG.db['xxx'] = {mem.permanent: [0] * 11,
+                        mem.data: [1] * 10,
+                        mem.original: [2] * 10}
+    table_prev(mem)
+    db = CONFIG.db['xxx']
+    assert len(db[mem.permanent]) == 1
+    assert db[mem.permanent] == [0]
+    assert len(db[mem.data]) ==  10 and db[mem.data] == [0] * 10
+    assert len(db[mem.original]) == 20
+    assert db[mem.original] == ([1] * 10) + ([2] * 10)
+    CONFIG.db['xxx'].update({mem.permanent: []})
+    table_prev(mem)
+    assert len(db[mem.permanent]) == 0
+    CONFIG.db['xxx'].update({mem.permanent: [0] * 5,
+                             mem.data: [1] * 10,
+                             mem.original: [2] * 10})
+    table_prev(mem)    
+    assert len(db[mem.permanent]) == 0
+    assert len(db[mem.data]) ==  5 and db[mem.data] == [0] * 5
+
+
 def test_download(): 
     D = mock_data()
     mem = CONFIG({CONFIG.username: 'xxx'})
     CONFIG.db['xxx'] = {mem.permanent: D[:11]}
     _ = download(mem, 'tmp.json')
     assert _['filename'] == 'tmp.json'
     assert len(_['content'].split('\n')) == 11
@@ -73,19 +94,20 @@
 def test_table_component():
     import dash_bootstrap_components as dbc
     element = table_component()
     assert isinstance(element, dbc.Stack)
 
 
 def test_progress():
-    mem = Config()
+    mem = CONFIG({})
     assert progress(mem) == 0
-    mem[mem.size] = 10
-    mem[mem.n] = 1
-    assert progress(mem) == 10
+    mem.mem.update({CONFIG.username: 'xxx'})
+    CONFIG.db['xxx'] = {mem.data: [None] * 10,
+                        mem.original: [None] * 10}    
+    assert progress(mem) == 50
 
 
 def test_update_row():
     from dash import Patch
     D = mock_data()
     mem = CONFIG({CONFIG.username: 'xxx'})
     CONFIG.db['xxx'] = {mem.data: D[:10]}
```

### Comparing `IngeoDash-0.0.20/IngeoDash/tests/test_config.py` & `IngeoDash-0.0.21/IngeoDash/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,29 +22,29 @@
                    label_header='klass',
                    data='corpus',
                    permanent='permanent',
                    original='original',
                    next='next',
                    next_label='Next',
                    n_value=10,
-                   n='N',
                    size='size',
                    progress='progress',
                    download='download',
                    filename='filename',
                    save='save',
                    center='center',
                    upload='upload',
                    lang='lang',
                    n_jobs=1,
                    denseBoW={},
                    db={},
                    username='username',
                    text='text',
-                   mem={})
+                   mem={},
+                   prev='previous')
     for k, v in default.items():
         assert v == getattr(conf, k)
 
 
 def test_Config_mem():
     config = Config()
 
@@ -62,15 +62,16 @@
     assert 'adios' not in xxx
     xxx['xxx'] = 3
     assert mem['xxx'] == 3
 
 
 def test_Config_call2():
     mem = CONFIG(dict(label_header='label',
-                      text='texto'))
+                      text='texto', n_value=12))
     assert mem.label_header == 'label'
     assert mem.text == 'texto'
+    assert mem.n_value == 12
 
 
 def test_CONFIG():
     from IngeoDash.config import CONFIG
     assert isinstance(CONFIG, Config)
```

### Comparing `IngeoDash-0.0.20/IngeoDash/tests/test_upload.py` & `IngeoDash-0.0.21/IngeoDash/tests/test_upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from IngeoDash.upload import upload, upload_component
 from IngeoDash.annotate import label_column
 from IngeoDash.config import CONFIG
 from microtc.utils import tweet_iterator
 from EvoMSA.tests.test_base import TWEETS
+import numpy as np
 import base64
 import json
 
 
 def test_upload():
     mem = CONFIG({CONFIG.username: 'xxx'})
     mem.label_header = 'klass'
@@ -30,34 +31,54 @@
     content_str = str(base64.b64encode(bytes('\n'.join(_),
                                        encoding='utf-8')),
                       encoding='utf-8')
     content = f'NA,{content_str}'
     _ = upload(mem, content, 'es')
     info = json.loads(_)
     db = CONFIG.db[info[mem.username]]
+    assert info[mem.size] == 50 + len(D1)
     assert len(db[mem.data]) == mem.n_value
     assert len(db[mem.permanent]) == 51
     assert len(db[mem.data]) + len(db[mem.original]) + len(db[mem.permanent]) == len(D) + 1
     for a, b in zip(db[mem.data], D[50:]):
         assert a['text'] == b['text'] and mem.label_header in a
+    
 
 
 def test_upload_unique():
-    mem = CONFIG({CONFIG.username: 'xxx', 'label_header': 'class'})
+    mem = CONFIG({CONFIG.username: 'xxx'})
     D = list(tweet_iterator(TWEETS))
     for x in D:
         x['class'] = 1
     CONFIG.db['xxx'] = {mem.data: D, mem.permanent: []}
     _ = [json.dumps(x) for x in D[:15]]
     content_str = str(base64.b64encode(bytes('\n'.join(_),
                                        encoding='utf-8')),
                       encoding='utf-8')
     content = f'NA,{content_str}'
-    _ = upload(mem, content, 'es')
+    _ = upload(mem, content, lang='es', label='class')
     db = CONFIG.db['xxx']
     assert len(db[mem.permanent]) == 0
 
 
+def test_upload_labels():
+    mem = CONFIG({CONFIG.username: 'xxx'})
+    D = list(tweet_iterator(TWEETS))
+    _ = [json.dumps(x) for x in D]
+    content_str = str(base64.b64encode(bytes('\n'.join(_),
+                                       encoding='utf-8')),
+                      encoding='utf-8')
+    content = f'NA,{content_str}'
+    _ = upload(mem, content, lang='es')
+    db = CONFIG.db['xxx']
+    assert len(db[mem.data]) == 0
+    assert len(db[mem.original]) == 0
+    klasses = np.unique([x['klass'] for x in D])
+    mem = CONFIG(_)
+    assert mem[mem.labels] == klasses.tolist()
+
+
+
 def test_upload_component():
     import dash_bootstrap_components as dbc
     component = upload_component()
     assert isinstance(component, dbc.InputGroup)
```

### Comparing `IngeoDash-0.0.20/IngeoDash/upload.py` & `IngeoDash-0.0.21/IngeoDash/upload.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,22 +24,25 @@
 
 def read_json(mem: Config, data):
     _ = io.StringIO(data.decode('utf-8'))
     return [json.loads(x) for x in _]
 
 
 def upload(mem: Config, content, lang='es', 
-           type='json', call_next=label_column):
+           type='json', text='text', label='klass',
+           call_next=label_column):
     def _label(x):
         if mem.label_header in x:
             ele = x[mem.label_header]
             if ele is not None and len(f'{ele}'):
                 return True
         return False
-    
+    mem.mem.update(dict(label_header=label, text=text))
+    mem.label_header = label
+    mem.text = text
     content_type, content_string = content.split(',')
     decoded = base64.b64decode(content_string)
     data = globals()[f'read_{type}'](mem, decoded)
     username, db = user(mem)
     labels = np.unique([x[mem.label_header]
                         for x in data if _label(x)])
     if labels.shape[0] > 1:
@@ -48,25 +51,32 @@
         permanent.extend([x for x in data if _label(x)])
     else:
         original = data
         permanent = []
     db[mem.data] = original[:mem.n_value]
     db[mem.permanent] = permanent
     db[mem.original] = original[mem.n_value:]
-    mem.mem = {mem.n: mem.n_value,
-               mem.lang: lang,
-               mem.size: len(original), 
-               mem.username: username}
+    mem.mem.update({mem.lang: lang,
+                    mem.size: len(data),
+                    mem.username: username})
     if call_next is not None:
         call_next(mem)
     return json.dumps(mem.mem)
 
 
 def upload_component():
     lang = dbc.Select(id=CONFIG.lang, value='es',
                       options=[dict(label=x, value=x) for x in MODEL_LANG])
-
     upload = dbc.InputGroup([dbc.InputGroupText('Language:'),
-                             lang, dcc.Upload(id=CONFIG.upload, 
-                                              children=dbc.Button('Upload'))])
+                             lang, 
+                             dbc.InputGroupText('Text Column:'),
+                             dcc.Input(id=CONFIG.text,
+                                       value='text',
+                                       type='text'),
+                             dbc.InputGroupText('Text Label:'),
+                             dcc.Input(id=CONFIG.label_header,
+                                       value='klass',
+                                       type='text'),
+                             dcc.Upload(id=CONFIG.upload, 
+                                        children=dbc.Button('Upload'))])
     return upload
```

### Comparing `IngeoDash-0.0.20/IngeoDash.egg-info/PKG-INFO` & `IngeoDash-0.0.21/IngeoDash.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.0.20
+Version: 0.0.21
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -16,12 +16,12 @@
 .. image:: https://coveralls.io/repos/github/INGEOTEC/IngeoDash/badge.svg?branch=develop
 		:target: https://coveralls.io/github/INGEOTEC/IngeoDash?branch=develop
 
 .. image:: https://badge.fury.io/py/IngeoDash.svg
 		:target: https://badge.fury.io/py/IngeoDash
 
 .. image:: https://colab.research.google.com/assets/colab-badge.svg
-		:target: https://colab.research.google.com/github/INGEOTEC/IngeoDash/blob/docs/docs/IngeoDash.ipynb 
+		:target: https://colab.research.google.com/github/INGEOTEC/IngeoDash/blob/master/docs/IngeoDash.ipynb 
 
 .. code-block:: bash
 
     python -m IngeoDash
```

### Comparing `IngeoDash-0.0.20/LICENSE` & `IngeoDash-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `IngeoDash-0.0.20/PKG-INFO` & `IngeoDash-0.0.21/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IngeoDash
-Version: 0.0.20
+Version: 0.0.21
 Summary: IngeoDash can help to label a dataset
 Author-email: Mario Graff <mgraffg@ieee.org>
 License: Apache License Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -16,12 +16,12 @@
 .. image:: https://coveralls.io/repos/github/INGEOTEC/IngeoDash/badge.svg?branch=develop
 		:target: https://coveralls.io/github/INGEOTEC/IngeoDash?branch=develop
 
 .. image:: https://badge.fury.io/py/IngeoDash.svg
 		:target: https://badge.fury.io/py/IngeoDash
 
 .. image:: https://colab.research.google.com/assets/colab-badge.svg
-		:target: https://colab.research.google.com/github/INGEOTEC/IngeoDash/blob/docs/docs/IngeoDash.ipynb 
+		:target: https://colab.research.google.com/github/INGEOTEC/IngeoDash/blob/master/docs/IngeoDash.ipynb 
 
 .. code-block:: bash
 
     python -m IngeoDash
```

### Comparing `IngeoDash-0.0.20/setup.py` & `IngeoDash-0.0.21/setup.py`

 * *Files identical despite different names*

