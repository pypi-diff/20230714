# Comparing `tmp/tva_utils-0.1.5.tar.gz` & `tmp/tva_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tva_utils-0.1.5.tar", max compression
+gzip compressed data, was "tva_utils-0.1.6.tar", max compression
```

## Comparing `tva_utils-0.1.5.tar` & `tva_utils-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.5/README.md
--rw-r--r--   0        0        0      376 2023-07-14 01:27:23.581833 tva_utils-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      129 2023-07-14 01:27:00.735841 tva_utils-0.1.5/tva_utils/__init__.py
--rw-r--r--   0        0        0      191 2023-07-14 01:27:15.934581 tva_utils-0.1.5/tva_utils/postgres/__init__.py
--rw-r--r--   0        0        0      427 2023-07-14 01:08:02.963561 tva_utils-0.1.5/tva_utils/postgres/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9647 2023-07-14 01:08:02.965155 tva_utils-0.1.5/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc
--rw-r--r--   0        0        0     9650 2023-07-14 00:50:45.404384 tva_utils-0.1.5/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc
--rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.5/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc
--rw-r--r--   0        0        0     5141 2023-07-14 01:22:18.988402 tva_utils-0.1.5/tva_utils/postgres/funcs.py
--rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.5/tva_utils/postgres/schemas.py
--rw-r--r--   0        0        0       57 2023-07-14 01:26:54.473423 tva_utils-0.1.5/tva_utils/timers/__init__.py
--rw-r--r--   0        0        0     1251 2023-07-14 01:26:01.937830 tva_utils-0.1.5/tva_utils/timers/timers.py
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 tva_utils-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.6/README.md
+-rw-r--r--   0        0        0      376 2023-07-14 01:39:44.064644 tva_utils-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-07-14 01:27:00.735841 tva_utils-0.1.6/tva_utils/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-14 01:37:17.931047 tva_utils-0.1.6/tva_utils/logging/__init__.py
+-rw-r--r--   0        0        0      326 2023-07-14 01:37:19.727024 tva_utils-0.1.6/tva_utils/logging/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2361 2023-07-14 01:39:03.597655 tva_utils-0.1.6/tva_utils/logging/__pycache__/logging.cpython-311.pyc
+-rw-r--r--   0        0        0     1467 2023-07-14 01:39:36.474015 tva_utils-0.1.6/tva_utils/logging/logging.py
+-rw-r--r--   0        0        0      191 2023-07-14 01:27:15.934581 tva_utils-0.1.6/tva_utils/postgres/__init__.py
+-rw-r--r--   0        0        0      459 2023-07-14 01:36:40.919534 tva_utils-0.1.6/tva_utils/postgres/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9791 2023-07-14 01:36:40.921077 tva_utils-0.1.6/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc
+-rw-r--r--   0        0        0     9650 2023-07-14 00:50:45.404384 tva_utils-0.1.6/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc
+-rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.6/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc
+-rw-r--r--   0        0        0     5141 2023-07-14 01:22:18.988402 tva_utils-0.1.6/tva_utils/postgres/funcs.py
+-rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.6/tva_utils/postgres/schemas.py
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 tva_utils-0.1.6/PKG-INFO
```

### Comparing `tva_utils-0.1.5/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc` & `tva_utils-0.1.6/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd59fb064 (Fri Jul 14 01:07:33 2023 UTC)
+moddate:  0xc29bb064 (Fri Jul 14 00:50:10 2023 UTC)
 files sz: 4809
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -96,36 +96,36 @@
     13         134 LOAD_CONST               0 (0)
                136 LOAD_CONST               9 (None)
                138 IMPORT_NAME             20 (uuid)
                140 STORE_NAME              20 (uuid)
    
     16         142 PUSH_NULL
                144 LOAD_BUILD_CLASS
-               146 LOAD_CONST              11 (<code object DB, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 16>)
+               146 LOAD_CONST              11 (<code object DB, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 16>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST              12 ('DB')
                152 PRECALL                  2
                156 CALL                     2
                166 STORE_NAME              21 (DB)
    
     51         168 PUSH_NULL
                170 LOAD_BUILD_CLASS
-               172 LOAD_CONST              13 (<code object DBUtils, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 51>)
+               172 LOAD_CONST              13 (<code object DBUtils, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 51>)
                174 MAKE_FUNCTION            0
                176 LOAD_CONST              14 ('DBUtils')
                178 PRECALL                  2
                182 CALL                     2
                192 STORE_NAME              22 (DBUtils)
    
    154         194 LOAD_CONST              15 ('url')
                196 LOAD_NAME               23 (str)
                198 LOAD_CONST              16 ('return')
                200 LOAD_NAME               11 (Engine)
                202 BUILD_TUPLE              4
-               204 LOAD_CONST              17 (<code object get_engine, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 154>)
+               204 LOAD_CONST              17 (<code object get_engine, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 154>)
                206 MAKE_FUNCTION            4 (annotations)
                208 STORE_NAME              24 (get_engine)
    
    166         210 PUSH_NULL
                212 LOAD_NAME               21 (DB)
                214 PRECALL                  0
                218 CALL                     0
@@ -159,48 +159,48 @@
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DB')
                        8 STORE_NAME               2 (__qualname__)
          
           17          10 LOAD_CONST               1 ('url')
                       12 LOAD_NAME                3 (str)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object initialize, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 17>)
+                      16 LOAD_CONST               2 (<code object initialize, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 17>)
                       18 MAKE_FUNCTION            4 (annotations)
                       20 STORE_NAME               4 (initialize)
          
           27          22 LOAD_CONST               3 ('Bases')
                       24 LOAD_NAME                5 (List)
                       26 LOAD_NAME                6 (DeclarativeMeta)
                       28 BINARY_SUBSCR
                       38 LOAD_CONST               4 ('schemas')
                       40 LOAD_NAME                5 (List)
                       42 LOAD_NAME                3 (str)
                       44 BINARY_SUBSCR
                       54 BUILD_TUPLE              4
-                      56 LOAD_CONST               5 (<code object _create_tables, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 27>)
+                      56 LOAD_CONST               5 (<code object _create_tables, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 27>)
                       58 MAKE_FUNCTION            4 (annotations)
                       60 STORE_NAME               7 (_create_tables)
          
           37          62 LOAD_CONST               6 ('return')
                       64 LOAD_NAME                8 (Iterator)
                       66 LOAD_NAME                9 (Session)
                       68 BINARY_SUBSCR
                       78 BUILD_TUPLE              2
-                      80 LOAD_CONST               7 (<code object get_session, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 37>)
+                      80 LOAD_CONST               7 (<code object get_session, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 37>)
                       82 MAKE_FUNCTION            4 (annotations)
                       84 STORE_NAME              10 (get_session)
          
           44          86 LOAD_CONST               6 ('return')
                       88 LOAD_NAME               11 (scoped_session)
                       90 BUILD_TUPLE              2
-                      92 LOAD_CONST               8 (<code object get_session_scoped, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 44>)
+                      92 LOAD_CONST               8 (<code object get_session_scoped, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 44>)
                       94 MAKE_FUNCTION            4 (annotations)
                       96 STORE_NAME              12 (get_session_scoped)
          
-          47          98 LOAD_CONST               9 (<code object close, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 47>)
+          47          98 LOAD_CONST               9 (<code object close, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 47>)
                      100 MAKE_FUNCTION            0
                      102 STORE_NAME              13 (close)
                      104 LOAD_CONST              10 (None)
                      106 RETURN_VALUE
          consts
             'DB'
             'url'
@@ -258,15 +258,15 @@
                   None
                   False
                   ('autocommit', 'autoflush', 'bind')
                names      ('get_engine', 'engine', 'sessionmaker', 'SessionLocal', 'inspect', 'inspector', 'DBUtils', 'utils')
                varnames   ('cls', 'url')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'initialize'
                firstlineno 17
                lnotab 0x020128010c0110ff1c033201
             'Bases'
             'schemas'
             code
                argcount  : 3
@@ -368,15 +368,15 @@
                  334 to 342 -> 344 [2] lasti
                consts
                   None
                names      ('zip', 'inspector', 'get_schema_names', 'engine', 'execute', 'sqlalchemy', 'schema', 'CreateSchema', 'metadata', 'create_all', 'Exception', 'print')
                varnames   ('cls', 'Bases', 'schemas', 'Base', 'schema', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       '_create_tables'
                firstlineno 27
                lnotab 0x02022a01020136016e014201120130ff08fb
             'return'
             code
                argcount  : 1
                nlocals   : 2
@@ -457,15 +457,15 @@
                  192 to 192 -> 186 [3] lasti
                consts
                   None
                names      ('SessionLocal', 'close')
                varnames   ('cls', 'session')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'get_session'
                firstlineno 37
                lnotab 0x06012a01020108025efc
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -483,15 +483,15 @@
                             40 RETURN_VALUE
                consts
                   None
                names      ('scoped_session', 'SessionLocal')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'get_session_scoped'
                firstlineno 44
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
@@ -511,24 +511,24 @@
                             54 RETURN_VALUE
                consts
                   None
                names      ('engine', 'dispose')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'close'
                firstlineno 47
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'str', 'initialize', 'List', 'DeclarativeMeta', '_create_tables', 'Iterator', 'Session', 'get_session', 'scoped_session', 'get_session_scoped', 'close')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
          name       'DB'
          firstlineno 16
          lnotab 0x0a010c0a280a18070c03
       'DB'
       code
          argcount  : 0
          nlocals   : 0
@@ -549,33 +549,33 @@
             06641184045a1764085300
           51           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DBUtils')
                        8 STORE_NAME               2 (__qualname__)
          
-          53          10 LOAD_CONST               1 (<code object __init__, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 53>)
+          53          10 LOAD_CONST               1 (<code object __init__, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 53>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
           56          16 LOAD_CONST               2 ('session')
                       18 LOAD_NAME                4 (Session)
                       20 BUILD_TUPLE              2
-                      22 LOAD_CONST               3 (<code object initialize, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 56>)
+                      22 LOAD_CONST               3 (<code object initialize, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 56>)
                       24 MAKE_FUNCTION            4 (annotations)
                       26 STORE_NAME               5 (initialize)
          
           59          28 LOAD_NAME                6 (staticmethod)
          
           60          30 LOAD_CONST               4 ('stmt')
                       32 LOAD_NAME                7 (str)
                       34 LOAD_CONST               5 ('return')
                       36 LOAD_NAME                8 (text)
                       38 BUILD_TUPLE              4
-                      40 LOAD_CONST               6 (<code object wrap_to_json, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 59>)
+                      40 LOAD_CONST               6 (<code object wrap_to_json, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 59>)
                       42 MAKE_FUNCTION            4 (annotations)
          
           59          44 PRECALL                  0
                       48 CALL                     0
          
           60          58 STORE_NAME               9 (wrap_to_json)
          
@@ -586,28 +586,28 @@
                       68 LOAD_NAME               11 (List)
                       70 LOAD_NAME               12 (dict)
                       72 BINARY_SUBSCR
                       82 LOAD_CONST               8 (None)
                       84 BUILD_TUPLE              2
                       86 BINARY_SUBSCR
                       96 BUILD_TUPLE              4
-                      98 LOAD_CONST               9 (<code object select_stmt_raw_sql, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 65>)
+                      98 LOAD_CONST               9 (<code object select_stmt_raw_sql, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 65>)
                      100 MAKE_FUNCTION            4 (annotations)
                      102 STORE_NAME              13 (select_stmt_raw_sql)
          
           76         104 LOAD_CONST               7 ('sql')
                      106 LOAD_NAME                7 (str)
                      108 LOAD_CONST               5 ('return')
                      110 LOAD_NAME               10 (Union)
                      112 LOAD_NAME               14 (bool)
                      114 LOAD_CONST               8 (None)
                      116 BUILD_TUPLE              2
                      118 BINARY_SUBSCR
                      128 BUILD_TUPLE              4
-                     130 LOAD_CONST              10 (<code object execute_stmt_raw_sql, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 76>)
+                     130 LOAD_CONST              10 (<code object execute_stmt_raw_sql, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 76>)
                      132 MAKE_FUNCTION            4 (annotations)
                      134 STORE_NAME              15 (execute_stmt_raw_sql)
          
           86         136 LOAD_CONST               7 ('sql')
          
           88         138 LOAD_NAME                7 (str)
          
@@ -622,26 +622,26 @@
                      150 LOAD_NAME               12 (dict)
                      152 BINARY_SUBSCR
                      162 LOAD_CONST               8 (None)
                      164 BUILD_TUPLE              2
                      166 BINARY_SUBSCR
          
           86         176 BUILD_TUPLE              6
-                     178 LOAD_CONST              12 (<code object select_stmt_raw_sql_params, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 86>)
+                     178 LOAD_CONST              12 (<code object select_stmt_raw_sql_params, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 86>)
                      180 MAKE_FUNCTION            4 (annotations)
                      182 STORE_NAME              16 (select_stmt_raw_sql_params)
          
          104         184 LOAD_CONST               5 ('return')
                      186 LOAD_NAME               10 (Union)
                      188 LOAD_NAME               17 (object)
                      190 LOAD_CONST               8 (None)
                      192 BUILD_TUPLE              2
                      194 BINARY_SUBSCR
                      204 BUILD_TUPLE              2
-                     206 LOAD_CONST              13 (<code object add_record_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 104>)
+                     206 LOAD_CONST              13 (<code object add_record_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 104>)
                      208 MAKE_FUNCTION            4 (annotations)
                      210 STORE_NAME              18 (add_record_sync)
          
          116         212 LOAD_CONST              14 ('model')
          
          117         214 LOAD_NAME               19 (BaseModel)
          
@@ -661,15 +661,15 @@
                      260 LOAD_NAME               11 (List)
                      262 LOAD_NAME               19 (BaseModel)
                      264 BINARY_SUBSCR
                      274 BUILD_TUPLE              2
                      276 BINARY_SUBSCR
          
          116         286 BUILD_TUPLE              6
-                     288 LOAD_CONST              16 (<code object add_records_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 116>)
+                     288 LOAD_CONST              16 (<code object add_records_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 116>)
                      290 MAKE_FUNCTION            4 (annotations)
                      292 STORE_NAME              22 (add_records_sync)
          
          138         294 LOAD_CONST              14 ('model')
          
          139         296 LOAD_NAME               19 (BaseModel)
          
@@ -681,15 +681,15 @@
                      314 BINARY_SUBSCR
          
          138         324 LOAD_CONST               5 ('return')
          
          140         326 LOAD_NAME               14 (bool)
          
          138         328 BUILD_TUPLE              6
-                     330 LOAD_CONST              17 (<code object remove_records_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 138>)
+                     330 LOAD_CONST              17 (<code object remove_records_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 138>)
                      332 MAKE_FUNCTION            4 (annotations)
                      334 STORE_NAME              23 (remove_records_sync)
                      336 LOAD_CONST               8 (None)
                      338 RETURN_VALUE
          consts
             'DBUtils'
             code
@@ -707,15 +707,15 @@
                             18 RETURN_VALUE
                consts
                   None
                names      ('session',)
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       '__init__'
                firstlineno 53
                lnotab 0x0201
             'session'
             code
                argcount  : 2
                nlocals   : 2
@@ -731,15 +731,15 @@
                             18 RETURN_VALUE
                consts
                   None
                names      ('session',)
                varnames   ('cls', 'session')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'initialize'
                firstlineno 56
                lnotab 0x0201
             'stmt'
             'return'
             code
                argcount  : 1
@@ -775,15 +775,15 @@
                   ''
                   'SELECT json_agg(t) FROM ('
                   ') t'
                names      ('replace', 'text')
                varnames   ('stmt',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'wrap_to_json'
                firstlineno 59
                lnotab 0x02022c01
             'sql'
             None
             code
                argcount  : 2
@@ -857,15 +857,15 @@
                consts
                   None
                   0
                names      ('wrap_to_json', 'session', 'execute', 'fetchone', 'DBAPIError')
                varnames   ('cls', 'sql', 'stmt', 'results', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'select_stmt_raw_sql'
                firstlineno 65
                lnotab 0x020102012a01640104010402060112010cff
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
@@ -922,15 +922,15 @@
                consts
                   None
                   True
                names      ('text', 'session', 'execute', 'DBAPIError')
                varnames   ('cls', 'sql', 'stmt', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'execute_stmt_raw_sql'
                firstlineno 76
                lnotab 0x020102011e013402060112010cff
             'params'
             code
                argcount  : 3
                nlocals   : 6
@@ -1006,15 +1006,15 @@
                   None
                   ('params',)
                   0
                names      ('wrap_to_json', 'session', 'execute', 'fetchone', 'DBAPIError')
                varnames   ('cls', 'sql', 'params', 'stmt', 'results', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'select_stmt_raw_sql_params'
                firstlineno 86
                lnotab 0x020502012a01680204010402060112020cfe
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 5
@@ -1095,15 +1095,15 @@
                consts
                   None
                   ()
                names      ('session', 'add', 'commit', 'DBAPIError', 'rollback')
                varnames   ('cls', 'model', 'kwargs', 'obj', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'add_record_sync'
                firstlineno 104
                lnotab 0x0201020110013401320106011202320114fd
             'model'
             'records'
             code
                argcount  : 3
@@ -1131,15 +1131,15 @@
                119           4 NOP
                
                120           6 BUILD_LIST               0
                              8 STORE_FAST               3 (inserted_ids)
                
                122          10 LOAD_CLOSURE             1 (model)
                             12 BUILD_TUPLE              1
-                            14 LOAD_CONST               1 (<code object <listcomp>, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 122>)
+                            14 LOAD_CONST               1 (<code object <listcomp>, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 122>)
                             16 MAKE_FUNCTION            8 (closure)
                             18 LOAD_FAST                2 (records)
                             20 GET_ITER
                             22 PRECALL                  0
                             26 CALL                     0
                             36 STORE_FAST               4 (records_to_insert)
                
@@ -1154,15 +1154,15 @@
                125          90 LOAD_FAST                0 (cls)
                             92 LOAD_ATTR                0 (session)
                            102 LOAD_METHOD              2 (flush)
                            124 PRECALL                  0
                            128 CALL                     0
                            138 POP_TOP
                
-               127         140 LOAD_CONST               2 (<code object <listcomp>, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 127>)
+               127         140 LOAD_CONST               2 (<code object <listcomp>, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 127>)
                            142 MAKE_FUNCTION            0
                            144 LOAD_FAST                4 (records_to_insert)
                            146 GET_ITER
                            148 PRECALL                  0
                            152 CALL                     0
                            162 STORE_FAST               2 (records)
                
@@ -1258,15 +1258,15 @@
                              >>   30 RETURN_VALUE
                      consts
                         ()
                      names      ()
                      varnames   ('.0', 'record')
                      freevars   ('model',)
                      cellvars   ()
-                     filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+                     filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                      name       '<listcomp>'
                      firstlineno 122
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
@@ -1287,23 +1287,23 @@
                                   50 JUMP_BACKWARD           23 (to 6)
                              >>   52 RETURN_VALUE
                      consts
                      names      ('to_dict',)
                      varnames   ('.0', 'record')
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+                     filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                      name       '<listcomp>'
                      firstlineno 127
                      lnotab 0x
                names      ('session', 'add_all', 'flush', 'append', 'uuid', 'commit', 'DBAPIError', 'rollback')
                varnames   ('cls', 'model', 'records', 'inserted_ids', 'records_to_insert', 'record', 'e')
                freevars   ()
                cellvars   ('model',)
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'add_records_sync'
                firstlineno 116
                lnotab 0x0403020104021c023401320218010801360132010a01120132021afd
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 5
@@ -1397,23 +1397,23 @@
                   False
                   ('synchronize_session',)
                   True
                names      ('session', 'query', 'filter', 'uuid', 'in_', 'delete', 'commit', 'DBAPIError', 'rollback')
                varnames   ('cls', 'model', 'records', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'remove_records_sync'
                firstlineno 138
                lnotab 0x020302019e0102ff1203320206011201320214fd
          names      ('__name__', '__module__', '__qualname__', '__init__', 'Session', 'initialize', 'staticmethod', 'str', 'text', 'wrap_to_json', 'Union', 'List', 'dict', 'select_stmt_raw_sql', 'bool', 'execute_stmt_raw_sql', 'select_stmt_raw_sql_params', 'object', 'add_record_sync', 'BaseModel', 'uuid', 'UUID', 'add_records_sync', 'remove_records_sync')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
          name       'DBUtils'
          firstlineno 51
          lnotab
             0x0a0206030c0302010eff0e0102052c0b200a020202fe020302fd02041e
             fc08121c0c020102ff02010eff020234fe0816020102ff020118ff020202
             fe
       'DBUtils'
@@ -1475,21 +1475,21 @@
             0
             True
             ('pool_size', 'max_overflow', 'pool_pre_ping')
          names      ('create_engine', 'DBAPIError')
          varnames   ('url', 'e')
          freevars   ()
          cellvars   ()
-         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
          name       'get_engine'
          firstlineno 154
          lnotab 0x020102010c0102010201020102fc140612020cfe
    names      ('tva_utils.postgres.schemas', 'BaseModel', 'sqlalchemy.exc', 'DBAPIError', 'sqlalchemy.orm.session', 'Session', 'sqlalchemy', 'text', 'inspect', 'create_engine', 'sqlalchemy.engine.base', 'Engine', 'sqlalchemy.orm', 'sessionmaker', 'scoped_session', 'DeclarativeMeta', 'typing', 'List', 'Union', 'Iterator', 'uuid', 'DB', 'DBUtils', 'str', 'get_engine', 'db')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+   filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c020c010c0110010c010c0110010c010802140108031a231a
       67100c
```

### Comparing `tva_utils-0.1.5/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc` & `tva_utils-0.1.6/tva_utils/postgres/__pycache__/funcs.cpython-311.pyc`

 * *Files 16% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xc29bb064 (Fri Jul 14 00:50:10 2023 UTC)
-files sz: 4809
+moddate:  0x4aa3b064 (Fri Jul 14 01:22:18 2023 UTC)
+files sz: 5141
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -96,40 +96,40 @@
     13         134 LOAD_CONST               0 (0)
                136 LOAD_CONST               9 (None)
                138 IMPORT_NAME             20 (uuid)
                140 STORE_NAME              20 (uuid)
    
     16         142 PUSH_NULL
                144 LOAD_BUILD_CLASS
-               146 LOAD_CONST              11 (<code object DB, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 16>)
+               146 LOAD_CONST              11 (<code object DB, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 16>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST              12 ('DB')
                152 PRECALL                  2
                156 CALL                     2
                166 STORE_NAME              21 (DB)
    
-    51         168 PUSH_NULL
+    57         168 PUSH_NULL
                170 LOAD_BUILD_CLASS
-               172 LOAD_CONST              13 (<code object DBUtils, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 51>)
+               172 LOAD_CONST              13 (<code object DBUtils, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 57>)
                174 MAKE_FUNCTION            0
                176 LOAD_CONST              14 ('DBUtils')
                178 PRECALL                  2
                182 CALL                     2
                192 STORE_NAME              22 (DBUtils)
    
-   154         194 LOAD_CONST              15 ('url')
+   161         194 LOAD_CONST              15 ('url')
                196 LOAD_NAME               23 (str)
                198 LOAD_CONST              16 ('return')
                200 LOAD_NAME               11 (Engine)
                202 BUILD_TUPLE              4
-               204 LOAD_CONST              17 (<code object get_engine, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 154>)
+               204 LOAD_CONST              17 (<code object get_engine, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 161>)
                206 MAKE_FUNCTION            4 (annotations)
                208 STORE_NAME              24 (get_engine)
    
-   166         210 PUSH_NULL
+   174         210 PUSH_NULL
                212 LOAD_NAME               21 (DB)
                214 PRECALL                  0
                218 CALL                     0
                228 STORE_NAME              25 (db)
                230 LOAD_CONST               9 (None)
                232 RETURN_VALUE
    consts
@@ -143,276 +143,312 @@
       ('sessionmaker', 'scoped_session')
       ('DeclarativeMeta',)
       None
       ('List', 'Union', 'Iterator')
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 5
+         stacksize : 6
          flags     : 0
          code
-            0x970065005a0164005a02640165036602640284045a0464036505650619
-            000000000000000000640465056503190000000000000000006604640584
-            045a07640665086509190000000000000000006602640784045a0a640665
-            0b6602640884045a0c640984005a0d640a5300
+            0x970065005a0164005a02640165036602640284045a0464036701660164
+            046505650619000000000000000000640565056503190000000000000000
+            006604640684055a07640765086509190000000000000000006602640884
+            045a0a6407650b6602640984045a0c640a84005a0d640b5300
           16           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DB')
                        8 STORE_NAME               2 (__qualname__)
          
           17          10 LOAD_CONST               1 ('url')
                       12 LOAD_NAME                3 (str)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object initialize, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 17>)
+                      16 LOAD_CONST               2 (<code object initialize, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 17>)
                       18 MAKE_FUNCTION            4 (annotations)
                       20 STORE_NAME               4 (initialize)
          
-          27          22 LOAD_CONST               3 ('Bases')
-                      24 LOAD_NAME                5 (List)
-                      26 LOAD_NAME                6 (DeclarativeMeta)
-                      28 BINARY_SUBSCR
-                      38 LOAD_CONST               4 ('schemas')
-                      40 LOAD_NAME                5 (List)
-                      42 LOAD_NAME                3 (str)
-                      44 BINARY_SUBSCR
-                      54 BUILD_TUPLE              4
-                      56 LOAD_CONST               5 (<code object _create_tables, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 27>)
-                      58 MAKE_FUNCTION            4 (annotations)
-                      60 STORE_NAME               7 (_create_tables)
-         
-          37          62 LOAD_CONST               6 ('return')
-                      64 LOAD_NAME                8 (Iterator)
-                      66 LOAD_NAME                9 (Session)
-                      68 BINARY_SUBSCR
-                      78 BUILD_TUPLE              2
-                      80 LOAD_CONST               7 (<code object get_session, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 37>)
-                      82 MAKE_FUNCTION            4 (annotations)
-                      84 STORE_NAME              10 (get_session)
-         
-          44          86 LOAD_CONST               6 ('return')
-                      88 LOAD_NAME               11 (scoped_session)
-                      90 BUILD_TUPLE              2
-                      92 LOAD_CONST               8 (<code object get_session_scoped, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 44>)
-                      94 MAKE_FUNCTION            4 (annotations)
-                      96 STORE_NAME              12 (get_session_scoped)
-         
-          47          98 LOAD_CONST               9 (<code object close, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 47>)
-                     100 MAKE_FUNCTION            0
-                     102 STORE_NAME              13 (close)
-                     104 LOAD_CONST              10 (None)
-                     106 RETURN_VALUE
+          25          22 LOAD_CONST               3 ('public')
+                      24 BUILD_LIST               1
+                      26 BUILD_TUPLE              1
+                      28 LOAD_CONST               4 ('Bases')
+                      30 LOAD_NAME                5 (List)
+                      32 LOAD_NAME                6 (DeclarativeMeta)
+                      34 BINARY_SUBSCR
+                      44 LOAD_CONST               5 ('schemas')
+                      46 LOAD_NAME                5 (List)
+                      48 LOAD_NAME                3 (str)
+                      50 BINARY_SUBSCR
+                      60 BUILD_TUPLE              4
+                      62 LOAD_CONST               6 (<code object create_tables, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 25>)
+                      64 MAKE_FUNCTION            5 (defaults, annotations)
+                      66 STORE_NAME               7 (create_tables)
+         
+          43          68 LOAD_CONST               7 ('return')
+                      70 LOAD_NAME                8 (Iterator)
+                      72 LOAD_NAME                9 (Session)
+                      74 BINARY_SUBSCR
+                      84 BUILD_TUPLE              2
+                      86 LOAD_CONST               8 (<code object get_session, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 43>)
+                      88 MAKE_FUNCTION            4 (annotations)
+                      90 STORE_NAME              10 (get_session)
+         
+          50          92 LOAD_CONST               7 ('return')
+                      94 LOAD_NAME               11 (scoped_session)
+                      96 BUILD_TUPLE              2
+                      98 LOAD_CONST               9 (<code object get_session_scoped, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 50>)
+                     100 MAKE_FUNCTION            4 (annotations)
+                     102 STORE_NAME              12 (get_session_scoped)
+         
+          53         104 LOAD_CONST              10 (<code object close, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 53>)
+                     106 MAKE_FUNCTION            0
+                     108 STORE_NAME              13 (close)
+                     110 LOAD_CONST              11 (None)
+                     112 RETURN_VALUE
          consts
             'DB'
             'url'
             code
                argcount  : 2
-               nlocals   : 2
+               nlocals   : 3
                stacksize : 5
-               flags     : 3
+               flags     : 11
                code
-                  0x97007401000000000000000000007c01a6010000ab0100000000000000
-                  007c005f010000000000000000740500000000000000000000640164017c
-                  006a010000000000000000ac02a6030000ab0300000000000000007c005f
-                  0300000000000000007409000000000000000000007c006a010000000000
-                  000000a6010000ab0100000000000000007c005f05000000000000000074
-                  0d00000000000000000000a6000000ab0000000000000000007c005f0700
-                  0000000000000064005300
+                  0x97007401000000000000000000007c01660169007c02a4018e017c005f
+                  010000000000000000740500000000000000000000640164017c006a0100
+                  00000000000000ac02a6030000ab0300000000000000007c005f03000000
+                  00000000007409000000000000000000007c006a010000000000000000a6
+                  010000ab0100000000000000007c005f050000000000000000740d000000
+                  00000000000000a6000000ab0000000000000000007c005f070000000000
+                  00000064005300
                 17           0 RESUME                   0
                
                 18           2 LOAD_GLOBAL              1 (NULL + get_engine)
                             14 LOAD_FAST                1 (url)
-                            16 PRECALL                  1
-                            20 CALL                     1
-                            30 LOAD_FAST                0 (cls)
-                            32 STORE_ATTR               1 (engine)
-               
-                19          42 LOAD_GLOBAL              5 (NULL + sessionmaker)
-               
-                20          54 LOAD_CONST               1 (False)
-                            56 LOAD_CONST               1 (False)
-                            58 LOAD_FAST                0 (cls)
-                            60 LOAD_ATTR                1 (engine)
-               
-                19          70 KW_NAMES                 2
-                            72 PRECALL                  3
-                            76 CALL                     3
-                            86 LOAD_FAST                0 (cls)
-                            88 STORE_ATTR               3 (SessionLocal)
-               
-                22          98 LOAD_GLOBAL              9 (NULL + inspect)
-                           110 LOAD_FAST                0 (cls)
-                           112 LOAD_ATTR                1 (engine)
-                           122 PRECALL                  1
-                           126 CALL                     1
-                           136 LOAD_FAST                0 (cls)
-                           138 STORE_ATTR               5 (inspector)
-               
-                23         148 LOAD_GLOBAL             13 (NULL + DBUtils)
-                           160 PRECALL                  0
-                           164 CALL                     0
-                           174 LOAD_FAST                0 (cls)
-                           176 STORE_ATTR               7 (utils)
-                           186 LOAD_CONST               0 (None)
-                           188 RETURN_VALUE
+                            16 BUILD_TUPLE              1
+                            18 BUILD_MAP                0
+                            20 LOAD_FAST                2 (kwargs)
+                            22 DICT_MERGE               1
+                            24 CALL_FUNCTION_EX         1
+                            26 LOAD_FAST                0 (cls)
+                            28 STORE_ATTR               1 (engine)
+               
+                19          38 LOAD_GLOBAL              5 (NULL + sessionmaker)
+               
+                20          50 LOAD_CONST               1 (False)
+                            52 LOAD_CONST               1 (False)
+                            54 LOAD_FAST                0 (cls)
+                            56 LOAD_ATTR                1 (engine)
+               
+                19          66 KW_NAMES                 2
+                            68 PRECALL                  3
+                            72 CALL                     3
+                            82 LOAD_FAST                0 (cls)
+                            84 STORE_ATTR               3 (SessionLocal)
+               
+                22          94 LOAD_GLOBAL              9 (NULL + inspect)
+                           106 LOAD_FAST                0 (cls)
+                           108 LOAD_ATTR                1 (engine)
+                           118 PRECALL                  1
+                           122 CALL                     1
+                           132 LOAD_FAST                0 (cls)
+                           134 STORE_ATTR               5 (inspector)
+               
+                23         144 LOAD_GLOBAL             13 (NULL + DBUtils)
+                           156 PRECALL                  0
+                           160 CALL                     0
+                           170 LOAD_FAST                0 (cls)
+                           172 STORE_ATTR               7 (utils)
+                           182 LOAD_CONST               0 (None)
+                           184 RETURN_VALUE
                consts
                   None
                   False
                   ('autocommit', 'autoflush', 'bind')
                names      ('get_engine', 'engine', 'sessionmaker', 'SessionLocal', 'inspect', 'inspector', 'DBUtils', 'utils')
-               varnames   ('cls', 'url')
+               varnames   ('cls', 'url', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                name       'initialize'
                firstlineno 17
-               lnotab 0x020128010c0110ff1c033201
+               lnotab 0x020124010c0110ff1c033201
+            'public'
             'Bases'
             'schemas'
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 6
                flags     : 3
                code
-                  0x97007401000000000000000000007c017c02a6020000ab020000000000
-                  00000044005d9d5c0200007d037d0409007c047c006a0100000000000000
-                  00a0020000000000000000000000000000000000000000a6000000ab0000
-                  00000000000000760172377c006a030000000000000000a0040000000000
-                  000000000000000000000000000000740a000000000000000000006a0600
-                  00000000000000a00700000000000000000000000000000000000000007c
-                  04a6010000ab010000000000000000a6010000ab01000000000000000001
-                  007c036a080000000000000000a009000000000000000000000000000000
-                  00000000007c006a030000000000000000a6010000ab0100000000000000
-                  0001008c782300741400000000000000000000240072197d057417000000
-                  000000000000007c05a6010000ab0100000000000000000100590064007d
-                  057e058c9664007d057e057701770078035900770164005300
-                27           0 RESUME                   0
+                  0x97007401000000000000000000007c01a6010000ab0100000000000000
+                  007402000000000000000000006b030000000072037c0167017d01740100
+                  0000000000000000007c02a6010000ab0100000000000000007402000000
+                  000000000000006b030000000072037c0267017d02740500000000000000
+                  0000007c017c02a6020000ab02000000000000000044005d9d5c0200007d
+                  037d0409007c047c006a030000000000000000a004000000000000000000
+                  0000000000000000000000a6000000ab000000000000000000760172377c
+                  006a050000000000000000a0060000000000000000000000000000000000
+                  000000740e000000000000000000006a080000000000000000a009000000
+                  00000000000000000000000000000000007c04a6010000ab010000000000
+                  000000a6010000ab01000000000000000001007c036a0a00000000000000
+                  00a00b00000000000000000000000000000000000000007c006a05000000
+                  0000000000a6010000ab01000000000000000001008c7823007418000000
+                  00000000000000240072197d05741b000000000000000000007c05a60100
+                  00ab0100000000000000000100590064017d057e058c9664017d057e0577
+                  01770078035900770164015300
+                25           0 RESUME                   0
                
-                29           2 LOAD_GLOBAL              1 (NULL + zip)
+                29           2 LOAD_GLOBAL              1 (NULL + type)
                             14 LOAD_FAST                1 (Bases)
-                            16 LOAD_FAST                2 (schemas)
-                            18 PRECALL                  2
-                            22 CALL                     2
-                            32 GET_ITER
-                       >>   34 FOR_ITER               157 (to 350)
-                            36 UNPACK_SEQUENCE          2
-                            40 STORE_FAST               3 (Base)
-                            42 STORE_FAST               4 (schema)
-               
-                30          44 NOP
-               
-                31          46 LOAD_FAST                4 (schema)
-                            48 LOAD_FAST                0 (cls)
-                            50 LOAD_ATTR                1 (inspector)
-                            60 LOAD_METHOD              2 (get_schema_names)
-                            82 PRECALL                  0
-                            86 CALL                     0
-                            96 CONTAINS_OP              1
-                            98 POP_JUMP_FORWARD_IF_FALSE    55 (to 210)
+                            16 PRECALL                  1
+                            20 CALL                     1
+                            30 LOAD_GLOBAL              2 (list)
+                            42 COMPARE_OP               3 (!=)
+                            48 POP_JUMP_FORWARD_IF_FALSE     3 (to 56)
+               
+                30          50 LOAD_FAST                1 (Bases)
+                            52 BUILD_LIST               1
+                            54 STORE_FAST               1 (Bases)
                
-                32         100 LOAD_FAST                0 (cls)
-                           102 LOAD_ATTR                3 (engine)
-                           112 LOAD_METHOD              4 (execute)
-                           134 LOAD_GLOBAL             10 (sqlalchemy)
-                           146 LOAD_ATTR                6 (schema)
-                           156 LOAD_METHOD              7 (CreateSchema)
-                           178 LOAD_FAST                4 (schema)
-                           180 PRECALL                  1
-                           184 CALL                     1
-                           194 PRECALL                  1
-                           198 CALL                     1
-                           208 POP_TOP
-               
-                33     >>  210 LOAD_FAST                3 (Base)
-                           212 LOAD_ATTR                8 (metadata)
-                           222 LOAD_METHOD              9 (create_all)
-                           244 LOAD_FAST                0 (cls)
-                           246 LOAD_ATTR                3 (engine)
-                           256 PRECALL                  1
-                           260 CALL                     1
-                           270 POP_TOP
-                           272 JUMP_BACKWARD          120 (to 34)
-                       >>  274 PUSH_EXC_INFO
-               
-                34         276 LOAD_GLOBAL             20 (Exception)
-                           288 CHECK_EXC_MATCH
-                           290 POP_JUMP_FORWARD_IF_FALSE    25 (to 342)
-                           292 STORE_FAST               5 (e)
-               
-                35         294 LOAD_GLOBAL             23 (NULL + print)
-                           306 LOAD_FAST                5 (e)
-                           308 PRECALL                  1
-                           312 CALL                     1
-                           322 POP_TOP
-                           324 POP_EXCEPT
-                           326 LOAD_CONST               0 (None)
-                           328 STORE_FAST               5 (e)
-                           330 DELETE_FAST              5 (e)
-                           332 JUMP_BACKWARD          150 (to 34)
-                       >>  334 LOAD_CONST               0 (None)
-                           336 STORE_FAST               5 (e)
-                           338 DELETE_FAST              5 (e)
-                           340 RERAISE                  1
-               
-                34     >>  342 RERAISE                  0
-                       >>  344 COPY                     3
-                           346 POP_EXCEPT
-                           348 RERAISE                  1
+                32     >>   56 LOAD_GLOBAL              1 (NULL + type)
+                            68 LOAD_FAST                2 (schemas)
+                            70 PRECALL                  1
+                            74 CALL                     1
+                            84 LOAD_GLOBAL              2 (list)
+                            96 COMPARE_OP               3 (!=)
+                           102 POP_JUMP_FORWARD_IF_FALSE     3 (to 110)
+               
+                33         104 LOAD_FAST                2 (schemas)
+                           106 BUILD_LIST               1
+                           108 STORE_FAST               2 (schemas)
+               
+                35     >>  110 LOAD_GLOBAL              5 (NULL + zip)
+                           122 LOAD_FAST                1 (Bases)
+                           124 LOAD_FAST                2 (schemas)
+                           126 PRECALL                  2
+                           130 CALL                     2
+                           140 GET_ITER
+                       >>  142 FOR_ITER               157 (to 458)
+                           144 UNPACK_SEQUENCE          2
+                           148 STORE_FAST               3 (Base)
+                           150 STORE_FAST               4 (schema)
+               
+                36         152 NOP
+               
+                37         154 LOAD_FAST                4 (schema)
+                           156 LOAD_FAST                0 (cls)
+                           158 LOAD_ATTR                3 (inspector)
+                           168 LOAD_METHOD              4 (get_schema_names)
+                           190 PRECALL                  0
+                           194 CALL                     0
+                           204 CONTAINS_OP              1
+                           206 POP_JUMP_FORWARD_IF_FALSE    55 (to 318)
+               
+                38         208 LOAD_FAST                0 (cls)
+                           210 LOAD_ATTR                5 (engine)
+                           220 LOAD_METHOD              6 (execute)
+                           242 LOAD_GLOBAL             14 (sqlalchemy)
+                           254 LOAD_ATTR                8 (schema)
+                           264 LOAD_METHOD              9 (CreateSchema)
+                           286 LOAD_FAST                4 (schema)
+                           288 PRECALL                  1
+                           292 CALL                     1
+                           302 PRECALL                  1
+                           306 CALL                     1
+                           316 POP_TOP
+               
+                39     >>  318 LOAD_FAST                3 (Base)
+                           320 LOAD_ATTR               10 (metadata)
+                           330 LOAD_METHOD             11 (create_all)
+                           352 LOAD_FAST                0 (cls)
+                           354 LOAD_ATTR                5 (engine)
+                           364 PRECALL                  1
+                           368 CALL                     1
+                           378 POP_TOP
+                           380 JUMP_BACKWARD          120 (to 142)
+                       >>  382 PUSH_EXC_INFO
+               
+                40         384 LOAD_GLOBAL             24 (Exception)
+                           396 CHECK_EXC_MATCH
+                           398 POP_JUMP_FORWARD_IF_FALSE    25 (to 450)
+                           400 STORE_FAST               5 (e)
+               
+                41         402 LOAD_GLOBAL             27 (NULL + print)
+                           414 LOAD_FAST                5 (e)
+                           416 PRECALL                  1
+                           420 CALL                     1
+                           430 POP_TOP
+                           432 POP_EXCEPT
+                           434 LOAD_CONST               1 (None)
+                           436 STORE_FAST               5 (e)
+                           438 DELETE_FAST              5 (e)
+                           440 JUMP_BACKWARD          150 (to 142)
+                       >>  442 LOAD_CONST               1 (None)
+                           444 STORE_FAST               5 (e)
+                           446 DELETE_FAST              5 (e)
+                           448 RERAISE                  1
+               
+                40     >>  450 RERAISE                  0
+                       >>  452 COPY                     3
+                           454 POP_EXCEPT
+                           456 RERAISE                  1
                
-                29     >>  350 LOAD_CONST               0 (None)
-                           352 RETURN_VALUE
+                35     >>  458 LOAD_CONST               1 (None)
+                           460 RETURN_VALUE
                ExceptionTable:
-                 46 to 270 -> 274 [1]
-                 274 to 292 -> 344 [2] lasti
-                 294 to 322 -> 334 [2] lasti
-                 334 to 342 -> 344 [2] lasti
+                 154 to 378 -> 382 [1]
+                 382 to 400 -> 452 [2] lasti
+                 402 to 430 -> 442 [2] lasti
+                 442 to 450 -> 452 [2] lasti
                consts
+                  '\n        Creates tables for all the models in the list of Bases\n        '
                   None
-               names      ('zip', 'inspector', 'get_schema_names', 'engine', 'execute', 'sqlalchemy', 'schema', 'CreateSchema', 'metadata', 'create_all', 'Exception', 'print')
+               names      ('type', 'list', 'zip', 'inspector', 'get_schema_names', 'engine', 'execute', 'sqlalchemy', 'schema', 'CreateSchema', 'metadata', 'create_all', 'Exception', 'print')
                varnames   ('cls', 'Bases', 'schemas', 'Base', 'schema', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
-               name       '_create_tables'
-               firstlineno 27
-               lnotab 0x02022a01020136016e014201120130ff08fb
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
+               name       'create_tables'
+               firstlineno 25
+               lnotab 0x020430010602300106022a01020136016e014201120130ff08fb
             'return'
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 6
                flags     : 35
                code
                   0x4b00010097007c00a00000000000000000000000000000000000000000
                   00a6000000ab00000000000000000035007d0109007c015600970101007c
                   01a0010000000000000000000000000000000000000000a6000000ab0000
                   0000000000000001006e1923007c01a00100000000000000000000000000
                   00000000000000a6000000ab000000000000000000010077007803590077
                   010900640064006400a6020000ab02000000000000000001006400530023
                   00310073047702780359007701010059000100010064005300
-                37           0 RETURN_GENERATOR
+                43           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                38           6 LOAD_FAST                0 (cls)
+                44           6 LOAD_FAST                0 (cls)
                              8 LOAD_METHOD              0 (SessionLocal)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 BEFORE_WITH
                             46 STORE_FAST               1 (session)
                
-                39          48 NOP
+                45          48 NOP
                
-                40          50 LOAD_FAST                1 (session)
+                46          50 LOAD_FAST                1 (session)
                             52 YIELD_VALUE
                             54 RESUME                   1
                             56 POP_TOP
                
-                42          58 LOAD_FAST                1 (session)
+                48          58 LOAD_FAST                1 (session)
                             60 LOAD_METHOD              1 (close)
                             82 PRECALL                  0
                             86 CALL                     0
                             96 POP_TOP
                             98 JUMP_FORWARD            25 (to 150)
                        >>  100 PUSH_EXC_INFO
                            102 LOAD_FAST                1 (session)
@@ -422,15 +458,15 @@
                            140 POP_TOP
                            142 RERAISE                  0
                        >>  144 COPY                     3
                            146 POP_EXCEPT
                            148 RERAISE                  1
                        >>  150 NOP
                
-                38         152 LOAD_CONST               0 (None)
+                44         152 LOAD_CONST               0 (None)
                            154 LOAD_CONST               0 (None)
                            156 LOAD_CONST               0 (None)
                            158 PRECALL                  2
                            162 CALL                     2
                            172 POP_TOP
                            174 LOAD_CONST               0 (None)
                            176 RETURN_VALUE
@@ -457,314 +493,333 @@
                  192 to 192 -> 186 [3] lasti
                consts
                   None
                names      ('SessionLocal', 'close')
                varnames   ('cls', 'session')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                name       'get_session'
-               firstlineno 37
+               firstlineno 43
                lnotab 0x06012a01020108025efc
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                44           0 RESUME                   0
+                50           0 RESUME                   0
                
-                45           2 LOAD_GLOBAL              1 (NULL + scoped_session)
+                51           2 LOAD_GLOBAL              1 (NULL + scoped_session)
                             14 LOAD_FAST                0 (cls)
                             16 LOAD_ATTR                1 (SessionLocal)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('scoped_session', 'SessionLocal')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                name       'get_session_scoped'
-               firstlineno 44
+               firstlineno 50
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab000000000000000000010064005300
-                47           0 RESUME                   0
+                53           0 RESUME                   0
                
-                48           2 LOAD_FAST                0 (cls)
+                54           2 LOAD_FAST                0 (cls)
                              4 LOAD_ATTR                0 (engine)
                             14 LOAD_METHOD              1 (dispose)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 POP_TOP
                             52 LOAD_CONST               0 (None)
                             54 RETURN_VALUE
                consts
                   None
                names      ('engine', 'dispose')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                name       'close'
-               firstlineno 47
+               firstlineno 53
                lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', 'str', 'initialize', 'List', 'DeclarativeMeta', '_create_tables', 'Iterator', 'Session', 'get_session', 'scoped_session', 'get_session_scoped', 'close')
+         names      ('__name__', '__module__', '__qualname__', 'str', 'initialize', 'List', 'DeclarativeMeta', 'create_tables', 'Iterator', 'Session', 'get_session', 'scoped_session', 'get_session_scoped', 'close')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
          name       'DB'
          firstlineno 16
-         lnotab 0x0a010c0a280a18070c03
+         lnotab 0x0a010c082e1218070c03
       'DB'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 9
+         stacksize : 11
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640265046602640384045a0565
             066404650764056508660464068404a6000000ab0000000000000000005a
-            09640765076405650a650b650c1900000000000000000064086602190000
-            000000000000006604640984045a0d640765076405650a650e6408660219
-            0000000000000000006604640a84045a0f64076507640b650c6405650a65
-            0b650c190000000000000000006408660219000000000000000000660664
-            0c84045a106405650a651164086602190000000000000000006602640d84
-            045a12640e6513640f650b650c190000000000000000006405650a650b65
-            146a15000000000000000019000000000000000000650b65131900000000
-            00000000006602190000000000000000006606641084045a16640e651364
-            0f650b65146a150000000000000000190000000000000000006405650e66
-            06641184045a1764085300
-          51           0 RESUME                   0
+            0964026504640765076405650a650b650c19000000000000000000640866
+            02190000000000000000006606640984045a0d6402650464076507640565
+            0a650e64086602190000000000000000006606640a84045a0f6402650464
+            076507640b650c6405650a650b650c190000000000000000006408660219
+            0000000000000000006608640c84045a10640265046405650a6511640866
+            02190000000000000000006604640d84045a1264026504640e6513640f65
+            0b650c190000000000000000006405650a650b65146a1500000000000000
+            0019000000000000000000650b6513190000000000000000006602190000
+            000000000000006608641084045a1664026504640e6513640f650b65146a
+            150000000000000000190000000000000000006405650e6608641184045a
+            1764085300
+          57           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DBUtils')
                        8 STORE_NAME               2 (__qualname__)
          
-          53          10 LOAD_CONST               1 (<code object __init__, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 53>)
+          59          10 LOAD_CONST               1 (<code object __init__, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 59>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-          56          16 LOAD_CONST               2 ('session')
+          62          16 LOAD_CONST               2 ('session')
                       18 LOAD_NAME                4 (Session)
                       20 BUILD_TUPLE              2
-                      22 LOAD_CONST               3 (<code object initialize, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 56>)
+                      22 LOAD_CONST               3 (<code object initialize, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 62>)
                       24 MAKE_FUNCTION            4 (annotations)
                       26 STORE_NAME               5 (initialize)
          
-          59          28 LOAD_NAME                6 (staticmethod)
+          65          28 LOAD_NAME                6 (staticmethod)
          
-          60          30 LOAD_CONST               4 ('stmt')
+          66          30 LOAD_CONST               4 ('stmt')
                       32 LOAD_NAME                7 (str)
                       34 LOAD_CONST               5 ('return')
                       36 LOAD_NAME                8 (text)
                       38 BUILD_TUPLE              4
-                      40 LOAD_CONST               6 (<code object wrap_to_json, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 59>)
+                      40 LOAD_CONST               6 (<code object wrap_to_json, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 65>)
                       42 MAKE_FUNCTION            4 (annotations)
          
-          59          44 PRECALL                  0
+          65          44 PRECALL                  0
                       48 CALL                     0
          
-          60          58 STORE_NAME               9 (wrap_to_json)
+          66          58 STORE_NAME               9 (wrap_to_json)
          
-          65          60 LOAD_CONST               7 ('sql')
-                      62 LOAD_NAME                7 (str)
-                      64 LOAD_CONST               5 ('return')
-                      66 LOAD_NAME               10 (Union)
-                      68 LOAD_NAME               11 (List)
-                      70 LOAD_NAME               12 (dict)
-                      72 BINARY_SUBSCR
-                      82 LOAD_CONST               8 (None)
-                      84 BUILD_TUPLE              2
-                      86 BINARY_SUBSCR
-                      96 BUILD_TUPLE              4
-                      98 LOAD_CONST               9 (<code object select_stmt_raw_sql, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 65>)
-                     100 MAKE_FUNCTION            4 (annotations)
-                     102 STORE_NAME              13 (select_stmt_raw_sql)
-         
-          76         104 LOAD_CONST               7 ('sql')
-                     106 LOAD_NAME                7 (str)
-                     108 LOAD_CONST               5 ('return')
-                     110 LOAD_NAME               10 (Union)
-                     112 LOAD_NAME               14 (bool)
-                     114 LOAD_CONST               8 (None)
-                     116 BUILD_TUPLE              2
-                     118 BINARY_SUBSCR
-                     128 BUILD_TUPLE              4
-                     130 LOAD_CONST              10 (<code object execute_stmt_raw_sql, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 76>)
-                     132 MAKE_FUNCTION            4 (annotations)
-                     134 STORE_NAME              15 (execute_stmt_raw_sql)
-         
-          86         136 LOAD_CONST               7 ('sql')
-         
-          88         138 LOAD_NAME                7 (str)
-         
-          86         140 LOAD_CONST              11 ('params')
-         
-          89         142 LOAD_NAME               12 (dict)
-         
-          86         144 LOAD_CONST               5 ('return')
-         
-          90         146 LOAD_NAME               10 (Union)
-                     148 LOAD_NAME               11 (List)
-                     150 LOAD_NAME               12 (dict)
-                     152 BINARY_SUBSCR
-                     162 LOAD_CONST               8 (None)
-                     164 BUILD_TUPLE              2
-                     166 BINARY_SUBSCR
-         
-          86         176 BUILD_TUPLE              6
-                     178 LOAD_CONST              12 (<code object select_stmt_raw_sql_params, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 86>)
-                     180 MAKE_FUNCTION            4 (annotations)
-                     182 STORE_NAME              16 (select_stmt_raw_sql_params)
-         
-         104         184 LOAD_CONST               5 ('return')
-                     186 LOAD_NAME               10 (Union)
-                     188 LOAD_NAME               17 (object)
-                     190 LOAD_CONST               8 (None)
-                     192 BUILD_TUPLE              2
-                     194 BINARY_SUBSCR
-                     204 BUILD_TUPLE              2
-                     206 LOAD_CONST              13 (<code object add_record_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 104>)
-                     208 MAKE_FUNCTION            4 (annotations)
-                     210 STORE_NAME              18 (add_record_sync)
-         
-         116         212 LOAD_CONST              14 ('model')
-         
-         117         214 LOAD_NAME               19 (BaseModel)
-         
-         116         216 LOAD_CONST              15 ('records')
-         
-         117         218 LOAD_NAME               11 (List)
-                     220 LOAD_NAME               12 (dict)
-                     222 BINARY_SUBSCR
-         
-         116         232 LOAD_CONST               5 ('return')
-         
-         118         234 LOAD_NAME               10 (Union)
-                     236 LOAD_NAME               11 (List)
-                     238 LOAD_NAME               20 (uuid)
-                     240 LOAD_ATTR               21 (UUID)
-                     250 BINARY_SUBSCR
-                     260 LOAD_NAME               11 (List)
-                     262 LOAD_NAME               19 (BaseModel)
-                     264 BINARY_SUBSCR
-                     274 BUILD_TUPLE              2
-                     276 BINARY_SUBSCR
-         
-         116         286 BUILD_TUPLE              6
-                     288 LOAD_CONST              16 (<code object add_records_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 116>)
-                     290 MAKE_FUNCTION            4 (annotations)
-                     292 STORE_NAME              22 (add_records_sync)
-         
-         138         294 LOAD_CONST              14 ('model')
-         
-         139         296 LOAD_NAME               19 (BaseModel)
-         
-         138         298 LOAD_CONST              15 ('records')
-         
-         139         300 LOAD_NAME               11 (List)
-                     302 LOAD_NAME               20 (uuid)
-                     304 LOAD_ATTR               21 (UUID)
-                     314 BINARY_SUBSCR
-         
-         138         324 LOAD_CONST               5 ('return')
-         
-         140         326 LOAD_NAME               14 (bool)
-         
-         138         328 BUILD_TUPLE              6
-                     330 LOAD_CONST              17 (<code object remove_records_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 138>)
-                     332 MAKE_FUNCTION            4 (annotations)
-                     334 STORE_NAME              23 (remove_records_sync)
-                     336 LOAD_CONST               8 (None)
-                     338 RETURN_VALUE
+          71          60 LOAD_CONST               2 ('session')
+                      62 LOAD_NAME                4 (Session)
+                      64 LOAD_CONST               7 ('sql')
+                      66 LOAD_NAME                7 (str)
+                      68 LOAD_CONST               5 ('return')
+                      70 LOAD_NAME               10 (Union)
+                      72 LOAD_NAME               11 (List)
+                      74 LOAD_NAME               12 (dict)
+                      76 BINARY_SUBSCR
+                      86 LOAD_CONST               8 (None)
+                      88 BUILD_TUPLE              2
+                      90 BINARY_SUBSCR
+                     100 BUILD_TUPLE              6
+                     102 LOAD_CONST               9 (<code object select_stmt_raw_sql, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 71>)
+                     104 MAKE_FUNCTION            4 (annotations)
+                     106 STORE_NAME              13 (select_stmt_raw_sql)
+         
+          82         108 LOAD_CONST               2 ('session')
+                     110 LOAD_NAME                4 (Session)
+                     112 LOAD_CONST               7 ('sql')
+                     114 LOAD_NAME                7 (str)
+                     116 LOAD_CONST               5 ('return')
+                     118 LOAD_NAME               10 (Union)
+                     120 LOAD_NAME               14 (bool)
+                     122 LOAD_CONST               8 (None)
+                     124 BUILD_TUPLE              2
+                     126 BINARY_SUBSCR
+                     136 BUILD_TUPLE              6
+                     138 LOAD_CONST              10 (<code object execute_stmt_raw_sql, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 82>)
+                     140 MAKE_FUNCTION            4 (annotations)
+                     142 STORE_NAME              15 (execute_stmt_raw_sql)
+         
+          92         144 LOAD_CONST               2 ('session')
+         
+          94         146 LOAD_NAME                4 (Session)
+         
+          92         148 LOAD_CONST               7 ('sql')
+         
+          95         150 LOAD_NAME                7 (str)
+         
+          92         152 LOAD_CONST              11 ('params')
+         
+          96         154 LOAD_NAME               12 (dict)
+         
+          92         156 LOAD_CONST               5 ('return')
+         
+          97         158 LOAD_NAME               10 (Union)
+                     160 LOAD_NAME               11 (List)
+                     162 LOAD_NAME               12 (dict)
+                     164 BINARY_SUBSCR
+                     174 LOAD_CONST               8 (None)
+                     176 BUILD_TUPLE              2
+                     178 BINARY_SUBSCR
+         
+          92         188 BUILD_TUPLE              8
+                     190 LOAD_CONST              12 (<code object select_stmt_raw_sql_params, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 92>)
+                     192 MAKE_FUNCTION            4 (annotations)
+                     194 STORE_NAME              16 (select_stmt_raw_sql_params)
+         
+         111         196 LOAD_CONST               2 ('session')
+                     198 LOAD_NAME                4 (Session)
+                     200 LOAD_CONST               5 ('return')
+                     202 LOAD_NAME               10 (Union)
+                     204 LOAD_NAME               17 (object)
+                     206 LOAD_CONST               8 (None)
+                     208 BUILD_TUPLE              2
+                     210 BINARY_SUBSCR
+                     220 BUILD_TUPLE              4
+                     222 LOAD_CONST              13 (<code object add_record_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 111>)
+                     224 MAKE_FUNCTION            4 (annotations)
+                     226 STORE_NAME              18 (add_record_sync)
+         
+         123         228 LOAD_CONST               2 ('session')
+         
+         124         230 LOAD_NAME                4 (Session)
+         
+         123         232 LOAD_CONST              14 ('model')
+         
+         124         234 LOAD_NAME               19 (BaseModel)
+         
+         123         236 LOAD_CONST              15 ('records')
+         
+         124         238 LOAD_NAME               11 (List)
+                     240 LOAD_NAME               12 (dict)
+                     242 BINARY_SUBSCR
+         
+         123         252 LOAD_CONST               5 ('return')
+         
+         125         254 LOAD_NAME               10 (Union)
+                     256 LOAD_NAME               11 (List)
+                     258 LOAD_NAME               20 (uuid)
+                     260 LOAD_ATTR               21 (UUID)
+                     270 BINARY_SUBSCR
+                     280 LOAD_NAME               11 (List)
+                     282 LOAD_NAME               19 (BaseModel)
+                     284 BINARY_SUBSCR
+                     294 BUILD_TUPLE              2
+                     296 BINARY_SUBSCR
+         
+         123         306 BUILD_TUPLE              8
+                     308 LOAD_CONST              16 (<code object add_records_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 123>)
+                     310 MAKE_FUNCTION            4 (annotations)
+                     312 STORE_NAME              22 (add_records_sync)
+         
+         145         314 LOAD_CONST               2 ('session')
+         
+         146         316 LOAD_NAME                4 (Session)
+         
+         145         318 LOAD_CONST              14 ('model')
+         
+         146         320 LOAD_NAME               19 (BaseModel)
+         
+         145         322 LOAD_CONST              15 ('records')
+         
+         146         324 LOAD_NAME               11 (List)
+                     326 LOAD_NAME               20 (uuid)
+                     328 LOAD_ATTR               21 (UUID)
+                     338 BINARY_SUBSCR
+         
+         145         348 LOAD_CONST               5 ('return')
+         
+         147         350 LOAD_NAME               14 (bool)
+         
+         145         352 BUILD_TUPLE              8
+                     354 LOAD_CONST              17 (<code object remove_records_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 145>)
+                     356 MAKE_FUNCTION            4 (annotations)
+                     358 STORE_NAME              23 (remove_records_sync)
+                     360 LOAD_CONST               8 (None)
+                     362 RETURN_VALUE
          consts
             'DBUtils'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code 0x970064007c005f00000000000000000064005300
-                53           0 RESUME                   0
+                59           0 RESUME                   0
                
-                54           2 LOAD_CONST               0 (None)
+                60           2 LOAD_CONST               0 (None)
                              4 LOAD_FAST                0 (cls)
                              6 STORE_ATTR               0 (session)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                names      ('session',)
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                name       '__init__'
-               firstlineno 53
+               firstlineno 59
                lnotab 0x0201
             'session'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x97007c017c005f00000000000000000064005300
-                56           0 RESUME                   0
+                62           0 RESUME                   0
                
-                57           2 LOAD_FAST                1 (session)
+                63           2 LOAD_FAST                1 (session)
                              4 LOAD_FAST                0 (cls)
                              6 STORE_ATTR               0 (session)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                names      ('session',)
                varnames   ('cls', 'session')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                name       'initialize'
-               firstlineno 56
+               firstlineno 62
                lnotab 0x0201
             'stmt'
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   02a6020000ab0200000000000000007d0074030000000000000000000064
                   037c009b0064049d03a6010000ab0100000000000000005300
-                59           0 RESUME                   0
+                65           0 RESUME                   0
                
-                61           2 LOAD_FAST                0 (stmt)
+                67           2 LOAD_FAST                0 (stmt)
                              4 LOAD_METHOD              0 (replace)
                             26 LOAD_CONST               1 (';')
                             28 LOAD_CONST               2 ('')
                             30 PRECALL                  2
                             34 CALL                     2
                             44 STORE_FAST               0 (stmt)
                
-                62          46 LOAD_GLOBAL              3 (NULL + text)
+                68          46 LOAD_GLOBAL              3 (NULL + text)
                             58 LOAD_CONST               3 ('SELECT json_agg(t) FROM (')
                             60 LOAD_FAST                0 (stmt)
                             62 FORMAT_VALUE             0
                             64 LOAD_CONST               4 (') t')
                             66 BUILD_STRING             3
                             68 PRECALL                  1
                             72 CALL                     1
@@ -775,477 +830,466 @@
                   ''
                   'SELECT json_agg(t) FROM ('
                   ') t'
                names      ('replace', 'text')
                varnames   ('stmt',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                name       'wrap_to_json'
-               firstlineno 59
+               firstlineno 65
                lnotab 0x02022c01
             'sql'
             None
             code
-               argcount  : 2
-               nlocals   : 5
+               argcount  : 3
+               nlocals   : 6
                stacksize : 4
                flags     : 3
                code
                   0x970009007c00a00000000000000000000000000000000000000000007c
-                  01a6010000ab0100000000000000007d027c006a010000000000000000a0
-                  0200000000000000000000000000000000000000007c02a6010000ab0100
-                  00000000000000a0030000000000000000000000000000000000000000a6
-                  000000ab0000000000000000006401190000000000000000007d037c0380
-                  02670053007c0353002300740800000000000000000000240072077d047c
-                  04820164007d047e0477017700780359007701
-                65           0 RESUME                   0
+                  02a6010000ab0100000000000000007d037c01a001000000000000000000
+                  00000000000000000000007c03a6010000ab010000000000000000a00200
+                  00000000000000000000000000000000000000a6000000ab000000000000
+                  0000006401190000000000000000007d047c048002670053007c04530023
+                  00740600000000000000000000240072077d057c05820164007d057e0577
+                  017700780359007701
+                71           0 RESUME                   0
                
-                66           2 NOP
+                72           2 NOP
                
-                67           4 LOAD_FAST                0 (cls)
+                73           4 LOAD_FAST                0 (cls)
                              6 LOAD_METHOD              0 (wrap_to_json)
-                            28 LOAD_FAST                1 (sql)
+                            28 LOAD_FAST                2 (sql)
                             30 PRECALL                  1
                             34 CALL                     1
-                            44 STORE_FAST               2 (stmt)
-               
-                68          46 LOAD_FAST                0 (cls)
-                            48 LOAD_ATTR                1 (session)
-                            58 LOAD_METHOD              2 (execute)
-                            80 LOAD_FAST                2 (stmt)
-                            82 PRECALL                  1
-                            86 CALL                     1
-                            96 LOAD_METHOD              3 (fetchone)
-                           118 PRECALL                  0
-                           122 CALL                     0
-                           132 LOAD_CONST               1 (0)
-                           134 BINARY_SUBSCR
-                           144 STORE_FAST               3 (results)
-               
-                69         146 LOAD_FAST                3 (results)
-                           148 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 154)
-               
-                70         150 BUILD_LIST               0
-                           152 RETURN_VALUE
-               
-                72     >>  154 LOAD_FAST                3 (results)
-                           156 RETURN_VALUE
-                       >>  158 PUSH_EXC_INFO
-               
-                73         160 LOAD_GLOBAL              8 (DBAPIError)
-                           172 CHECK_EXC_MATCH
-                           174 POP_JUMP_FORWARD_IF_FALSE     7 (to 190)
-                           176 STORE_FAST               4 (e)
-               
-                74         178 LOAD_FAST                4 (e)
-                           180 RAISE_VARARGS            1
-                       >>  182 LOAD_CONST               0 (None)
-                           184 STORE_FAST               4 (e)
-                           186 DELETE_FAST              4 (e)
-                           188 RERAISE                  1
+                            44 STORE_FAST               3 (stmt)
                
-                73     >>  190 RERAISE                  0
-                       >>  192 COPY                     3
-                           194 POP_EXCEPT
-                           196 RERAISE                  1
+                74          46 LOAD_FAST                1 (session)
+                            48 LOAD_METHOD              1 (execute)
+                            70 LOAD_FAST                3 (stmt)
+                            72 PRECALL                  1
+                            76 CALL                     1
+                            86 LOAD_METHOD              2 (fetchone)
+                           108 PRECALL                  0
+                           112 CALL                     0
+                           122 LOAD_CONST               1 (0)
+                           124 BINARY_SUBSCR
+                           134 STORE_FAST               4 (results)
+               
+                75         136 LOAD_FAST                4 (results)
+                           138 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 144)
+               
+                76         140 BUILD_LIST               0
+                           142 RETURN_VALUE
+               
+                78     >>  144 LOAD_FAST                4 (results)
+                           146 RETURN_VALUE
+                       >>  148 PUSH_EXC_INFO
+               
+                79         150 LOAD_GLOBAL              6 (DBAPIError)
+                           162 CHECK_EXC_MATCH
+                           164 POP_JUMP_FORWARD_IF_FALSE     7 (to 180)
+                           166 STORE_FAST               5 (e)
+               
+                80         168 LOAD_FAST                5 (e)
+                           170 RAISE_VARARGS            1
+                       >>  172 LOAD_CONST               0 (None)
+                           174 STORE_FAST               5 (e)
+                           176 DELETE_FAST              5 (e)
+                           178 RERAISE                  1
+               
+                79     >>  180 RERAISE                  0
+                       >>  182 COPY                     3
+                           184 POP_EXCEPT
+                           186 RERAISE                  1
                ExceptionTable:
-                 4 to 150 -> 158 [0]
-                 154 to 154 -> 158 [0]
-                 158 to 176 -> 192 [1] lasti
-                 178 to 180 -> 182 [1] lasti
-                 182 to 190 -> 192 [1] lasti
+                 4 to 140 -> 148 [0]
+                 144 to 144 -> 148 [0]
+                 148 to 166 -> 182 [1] lasti
+                 168 to 170 -> 172 [1] lasti
+                 172 to 180 -> 182 [1] lasti
                consts
                   None
                   0
-               names      ('wrap_to_json', 'session', 'execute', 'fetchone', 'DBAPIError')
-               varnames   ('cls', 'sql', 'stmt', 'results', 'e')
+               names      ('wrap_to_json', 'execute', 'fetchone', 'DBAPIError')
+               varnames   ('cls', 'session', 'sql', 'stmt', 'results', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                name       'select_stmt_raw_sql'
-               firstlineno 65
-               lnotab 0x020102012a01640104010402060112010cff
+               firstlineno 71
+               lnotab 0x020102012a015a0104010402060112010cff
             code
-               argcount  : 2
-               nlocals   : 4
+               argcount  : 3
+               nlocals   : 5
                stacksize : 4
                flags     : 3
                code
-                  0x970009007401000000000000000000007c01a6010000ab010000000000
-                  0000007d027c006a010000000000000000a0020000000000000000000000
-                  0000000000000000007c02a6010000ab0100000000000000000100640153
-                  002300740600000000000000000000240072077d037c03820164007d037e
-                  0377017700780359007701
-                76           0 RESUME                   0
+                  0x970009007401000000000000000000007c02a6010000ab010000000000
+                  0000007d037c01a00100000000000000000000000000000000000000007c
+                  03a6010000ab010000000000000000010064015300230074040000000000
+                  0000000000240072077d047c04820164007d047e04770177007803590077
+                  01
+                82           0 RESUME                   0
                
-                77           2 NOP
+                83           2 NOP
                
-                78           4 LOAD_GLOBAL              1 (NULL + text)
-                            16 LOAD_FAST                1 (sql)
+                84           4 LOAD_GLOBAL              1 (NULL + text)
+                            16 LOAD_FAST                2 (sql)
                             18 PRECALL                  1
                             22 CALL                     1
-                            32 STORE_FAST               2 (stmt)
-               
-                79          34 LOAD_FAST                0 (cls)
-                            36 LOAD_ATTR                1 (session)
-                            46 LOAD_METHOD              2 (execute)
-                            68 LOAD_FAST                2 (stmt)
-                            70 PRECALL                  1
-                            74 CALL                     1
-                            84 POP_TOP
+                            32 STORE_FAST               3 (stmt)
                
-                81          86 LOAD_CONST               1 (True)
-                            88 RETURN_VALUE
-                       >>   90 PUSH_EXC_INFO
-               
-                82          92 LOAD_GLOBAL              6 (DBAPIError)
-                           104 CHECK_EXC_MATCH
-                           106 POP_JUMP_FORWARD_IF_FALSE     7 (to 122)
-                           108 STORE_FAST               3 (e)
-               
-                83         110 LOAD_FAST                3 (e)
-                           112 RAISE_VARARGS            1
-                       >>  114 LOAD_CONST               0 (None)
-                           116 STORE_FAST               3 (e)
-                           118 DELETE_FAST              3 (e)
-                           120 RERAISE                  1
-               
-                82     >>  122 RERAISE                  0
-                       >>  124 COPY                     3
-                           126 POP_EXCEPT
-                           128 RERAISE                  1
+                85          34 LOAD_FAST                1 (session)
+                            36 LOAD_METHOD              1 (execute)
+                            58 LOAD_FAST                3 (stmt)
+                            60 PRECALL                  1
+                            64 CALL                     1
+                            74 POP_TOP
+               
+                87          76 LOAD_CONST               1 (True)
+                            78 RETURN_VALUE
+                       >>   80 PUSH_EXC_INFO
+               
+                88          82 LOAD_GLOBAL              4 (DBAPIError)
+                            94 CHECK_EXC_MATCH
+                            96 POP_JUMP_FORWARD_IF_FALSE     7 (to 112)
+                            98 STORE_FAST               4 (e)
+               
+                89         100 LOAD_FAST                4 (e)
+                           102 RAISE_VARARGS            1
+                       >>  104 LOAD_CONST               0 (None)
+                           106 STORE_FAST               4 (e)
+                           108 DELETE_FAST              4 (e)
+                           110 RERAISE                  1
+               
+                88     >>  112 RERAISE                  0
+                       >>  114 COPY                     3
+                           116 POP_EXCEPT
+                           118 RERAISE                  1
                ExceptionTable:
-                 4 to 84 -> 90 [0]
-                 90 to 108 -> 124 [1] lasti
-                 110 to 112 -> 114 [1] lasti
-                 114 to 122 -> 124 [1] lasti
+                 4 to 74 -> 80 [0]
+                 80 to 98 -> 114 [1] lasti
+                 100 to 102 -> 104 [1] lasti
+                 104 to 112 -> 114 [1] lasti
                consts
                   None
                   True
-               names      ('text', 'session', 'execute', 'DBAPIError')
-               varnames   ('cls', 'sql', 'stmt', 'e')
+               names      ('text', 'execute', 'DBAPIError')
+               varnames   ('cls', 'session', 'sql', 'stmt', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                name       'execute_stmt_raw_sql'
-               firstlineno 76
-               lnotab 0x020102011e013402060112010cff
+               firstlineno 82
+               lnotab 0x020102011e012a02060112010cff
             'params'
             code
-               argcount  : 3
-               nlocals   : 6
+               argcount  : 4
+               nlocals   : 7
                stacksize : 4
                flags     : 3
                code
                   0x970009007c00a00000000000000000000000000000000000000000007c
-                  01a6010000ab0100000000000000007d037c006a010000000000000000a0
-                  0200000000000000000000000000000000000000007c037c02ac01a60200
-                  00ab020000000000000000a0030000000000000000000000000000000000
-                  000000a6000000ab0000000000000000006402190000000000000000007d
-                  047c048002670053007c0453002300740800000000000000000000240072
-                  077d057c05820164007d057e0577017700780359007701
-                86           0 RESUME                   0
+                  02a6010000ab0100000000000000007d047c01a001000000000000000000
+                  00000000000000000000007c047c03ac01a6020000ab0200000000000000
+                  00a0020000000000000000000000000000000000000000a6000000ab0000
+                  000000000000006402190000000000000000007d057c058002670053007c
+                  0553002300740600000000000000000000240072077d067c06820164007d
+                  067e0677017700780359007701
+                92           0 RESUME                   0
                
-                91           2 NOP
+                98           2 NOP
                
-                92           4 LOAD_FAST                0 (cls)
+                99           4 LOAD_FAST                0 (cls)
                              6 LOAD_METHOD              0 (wrap_to_json)
-                            28 LOAD_FAST                1 (sql)
+                            28 LOAD_FAST                2 (sql)
                             30 PRECALL                  1
                             34 CALL                     1
-                            44 STORE_FAST               3 (stmt)
+                            44 STORE_FAST               4 (stmt)
                
-                93          46 LOAD_FAST                0 (cls)
-                            48 LOAD_ATTR                1 (session)
-                            58 LOAD_METHOD              2 (execute)
-                            80 LOAD_FAST                3 (stmt)
-                            82 LOAD_FAST                2 (params)
-                            84 KW_NAMES                 1
-                            86 PRECALL                  2
-                            90 CALL                     2
-                           100 LOAD_METHOD              3 (fetchone)
-                           122 PRECALL                  0
-                           126 CALL                     0
-                           136 LOAD_CONST               2 (0)
-                           138 BINARY_SUBSCR
-                           148 STORE_FAST               4 (results)
-               
-                95         150 LOAD_FAST                4 (results)
-                           152 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 158)
-               
-                96         154 BUILD_LIST               0
-                           156 RETURN_VALUE
-               
-                98     >>  158 LOAD_FAST                4 (results)
-                           160 RETURN_VALUE
-                       >>  162 PUSH_EXC_INFO
-               
-                99         164 LOAD_GLOBAL              8 (DBAPIError)
-                           176 CHECK_EXC_MATCH
-                           178 POP_JUMP_FORWARD_IF_FALSE     7 (to 194)
-                           180 STORE_FAST               5 (e)
-               
-               101         182 LOAD_FAST                5 (e)
-                           184 RAISE_VARARGS            1
-                       >>  186 LOAD_CONST               0 (None)
-                           188 STORE_FAST               5 (e)
-                           190 DELETE_FAST              5 (e)
-                           192 RERAISE                  1
+               100          46 LOAD_FAST                1 (session)
+                            48 LOAD_METHOD              1 (execute)
+                            70 LOAD_FAST                4 (stmt)
+                            72 LOAD_FAST                3 (params)
+                            74 KW_NAMES                 1
+                            76 PRECALL                  2
+                            80 CALL                     2
+                            90 LOAD_METHOD              2 (fetchone)
+                           112 PRECALL                  0
+                           116 CALL                     0
+                           126 LOAD_CONST               2 (0)
+                           128 BINARY_SUBSCR
+                           138 STORE_FAST               5 (results)
+               
+               102         140 LOAD_FAST                5 (results)
+                           142 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 148)
+               
+               103         144 BUILD_LIST               0
+                           146 RETURN_VALUE
+               
+               105     >>  148 LOAD_FAST                5 (results)
+                           150 RETURN_VALUE
+                       >>  152 PUSH_EXC_INFO
+               
+               106         154 LOAD_GLOBAL              6 (DBAPIError)
+                           166 CHECK_EXC_MATCH
+                           168 POP_JUMP_FORWARD_IF_FALSE     7 (to 184)
+                           170 STORE_FAST               6 (e)
+               
+               108         172 LOAD_FAST                6 (e)
+                           174 RAISE_VARARGS            1
+                       >>  176 LOAD_CONST               0 (None)
+                           178 STORE_FAST               6 (e)
+                           180 DELETE_FAST              6 (e)
+                           182 RERAISE                  1
                
-                99     >>  194 RERAISE                  0
-                       >>  196 COPY                     3
-                           198 POP_EXCEPT
-                           200 RERAISE                  1
+               106     >>  184 RERAISE                  0
+                       >>  186 COPY                     3
+                           188 POP_EXCEPT
+                           190 RERAISE                  1
                ExceptionTable:
-                 4 to 154 -> 162 [0]
-                 158 to 158 -> 162 [0]
-                 162 to 180 -> 196 [1] lasti
-                 182 to 184 -> 186 [1] lasti
-                 186 to 194 -> 196 [1] lasti
+                 4 to 144 -> 152 [0]
+                 148 to 148 -> 152 [0]
+                 152 to 170 -> 186 [1] lasti
+                 172 to 174 -> 176 [1] lasti
+                 176 to 184 -> 186 [1] lasti
                consts
                   None
                   ('params',)
                   0
-               names      ('wrap_to_json', 'session', 'execute', 'fetchone', 'DBAPIError')
-               varnames   ('cls', 'sql', 'params', 'stmt', 'results', 'e')
+               names      ('wrap_to_json', 'execute', 'fetchone', 'DBAPIError')
+               varnames   ('cls', 'session', 'sql', 'params', 'stmt', 'results', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                name       'select_stmt_raw_sql_params'
-               firstlineno 86
-               lnotab 0x020502012a01680204010402060112020cfe
+               firstlineno 92
+               lnotab 0x020602012a015e0204010402060112020cfe
             code
-               argcount  : 3
-               nlocals   : 5
+               argcount  : 4
+               nlocals   : 6
                stacksize : 5
                flags     : 3
                code
-                  0x9700090002007c01640169007c02a4018e017d037c006a000000000000
-                  000000a00100000000000000000000000000000000000000007c03a60100
-                  00ab01000000000000000001007c006a000000000000000000a002000000
-                  0000000000000000000000000000000000a6000000ab0000000000000000
-                  0001007c0353002300740600000000000000000000240072247d047c006a
-                  000000000000000000a00400000000000000000000000000000000000000
-                  00a6000000ab0000000000000000000100590064007d047e046400530064
-                  007d047e0477017700780359007701
-               104           0 RESUME                   0
+                  0x9700090002007c02640169007c03a4018e017d047c01a0000000000000
+                  0000000000000000000000000000007c04a6010000ab0100000000000000
+                  0001007c01a0010000000000000000000000000000000000000000a60000
+                  00ab00000000000000000001007c04530023007404000000000000000000
+                  002400721f7d057c01a00300000000000000000000000000000000000000
+                  00a6000000ab0000000000000000000100590064007d057e056400530064
+                  007d057e0577017700780359007701
+               111           0 RESUME                   0
                
-               105           2 NOP
+               112           2 NOP
                
-               106           4 PUSH_NULL
-                             6 LOAD_FAST                1 (model)
+               113           4 PUSH_NULL
+                             6 LOAD_FAST                2 (model)
                              8 LOAD_CONST               1 (())
                             10 BUILD_MAP                0
-                            12 LOAD_FAST                2 (kwargs)
+                            12 LOAD_FAST                3 (kwargs)
                             14 DICT_MERGE               1
                             16 CALL_FUNCTION_EX         1
-                            18 STORE_FAST               3 (obj)
+                            18 STORE_FAST               4 (obj)
                
-               107          20 LOAD_FAST                0 (cls)
-                            22 LOAD_ATTR                0 (session)
-                            32 LOAD_METHOD              1 (add)
-                            54 LOAD_FAST                3 (obj)
-                            56 PRECALL                  1
-                            60 CALL                     1
-                            70 POP_TOP
-               
-               108          72 LOAD_FAST                0 (cls)
-                            74 LOAD_ATTR                0 (session)
-                            84 LOAD_METHOD              2 (commit)
-                           106 PRECALL                  0
-                           110 CALL                     0
-                           120 POP_TOP
-               
-               109         122 LOAD_FAST                3 (obj)
-                           124 RETURN_VALUE
-                       >>  126 PUSH_EXC_INFO
-               
-               110         128 LOAD_GLOBAL              6 (DBAPIError)
-                           140 CHECK_EXC_MATCH
-                           142 POP_JUMP_FORWARD_IF_FALSE    36 (to 216)
-                           144 STORE_FAST               4 (e)
-               
-               112         146 LOAD_FAST                0 (cls)
-                           148 LOAD_ATTR                0 (session)
-                           158 LOAD_METHOD              4 (rollback)
-                           180 PRECALL                  0
-                           184 CALL                     0
-                           194 POP_TOP
-               
-               113         196 POP_EXCEPT
-                           198 LOAD_CONST               0 (None)
-                           200 STORE_FAST               4 (e)
-                           202 DELETE_FAST              4 (e)
-                           204 LOAD_CONST               0 (None)
-                           206 RETURN_VALUE
-                       >>  208 LOAD_CONST               0 (None)
-                           210 STORE_FAST               4 (e)
-                           212 DELETE_FAST              4 (e)
-                           214 RERAISE                  1
-               
-               110     >>  216 RERAISE                  0
-                       >>  218 COPY                     3
-                           220 POP_EXCEPT
-                           222 RERAISE                  1
+               114          20 LOAD_FAST                1 (session)
+                            22 LOAD_METHOD              0 (add)
+                            44 LOAD_FAST                4 (obj)
+                            46 PRECALL                  1
+                            50 CALL                     1
+                            60 POP_TOP
+               
+               115          62 LOAD_FAST                1 (session)
+                            64 LOAD_METHOD              1 (commit)
+                            86 PRECALL                  0
+                            90 CALL                     0
+                           100 POP_TOP
+               
+               116         102 LOAD_FAST                4 (obj)
+                           104 RETURN_VALUE
+                       >>  106 PUSH_EXC_INFO
+               
+               117         108 LOAD_GLOBAL              4 (DBAPIError)
+                           120 CHECK_EXC_MATCH
+                           122 POP_JUMP_FORWARD_IF_FALSE    31 (to 186)
+                           124 STORE_FAST               5 (e)
+               
+               119         126 LOAD_FAST                1 (session)
+                           128 LOAD_METHOD              3 (rollback)
+                           150 PRECALL                  0
+                           154 CALL                     0
+                           164 POP_TOP
+               
+               120         166 POP_EXCEPT
+                           168 LOAD_CONST               0 (None)
+                           170 STORE_FAST               5 (e)
+                           172 DELETE_FAST              5 (e)
+                           174 LOAD_CONST               0 (None)
+                           176 RETURN_VALUE
+                       >>  178 LOAD_CONST               0 (None)
+                           180 STORE_FAST               5 (e)
+                           182 DELETE_FAST              5 (e)
+                           184 RERAISE                  1
+               
+               117     >>  186 RERAISE                  0
+                       >>  188 COPY                     3
+                           190 POP_EXCEPT
+                           192 RERAISE                  1
                ExceptionTable:
-                 4 to 122 -> 126 [0]
-                 126 to 144 -> 218 [1] lasti
-                 146 to 194 -> 208 [1] lasti
-                 208 to 216 -> 218 [1] lasti
+                 4 to 102 -> 106 [0]
+                 106 to 124 -> 188 [1] lasti
+                 126 to 164 -> 178 [1] lasti
+                 178 to 186 -> 188 [1] lasti
                consts
                   None
                   ()
-               names      ('session', 'add', 'commit', 'DBAPIError', 'rollback')
-               varnames   ('cls', 'model', 'kwargs', 'obj', 'e')
+               names      ('add', 'commit', 'DBAPIError', 'rollback')
+               varnames   ('cls', 'session', 'model', 'kwargs', 'obj', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                name       'add_record_sync'
-               firstlineno 104
-               lnotab 0x0201020110013401320106011202320114fd
+               firstlineno 111
+               lnotab 0x0201020110012a01280106011202280114fd
             'model'
             'records'
             code
-               argcount  : 3
-               nlocals   : 7
+               argcount  : 4
+               nlocals   : 8
                stacksize : 4
                flags     : 3
                code
-                  0x87019700090067007d0388016601640184087c024400a6000000ab0000
-                  000000000000007d047c006a000000000000000000a00100000000000000
-                  000000000000000000000000007c04a6010000ab01000000000000000001
-                  007c006a000000000000000000a002000000000000000000000000000000
-                  0000000000a6000000ab0000000000000000000100640284007c044400a6
-                  000000ab0000000000000000007d027c0444005d1c7d057c03a003000000
-                  00000000000000000000000000000000007c056a040000000000000000a6
-                  010000ab01000000000000000001008c1d7c006a000000000000000000a0
-                  050000000000000000000000000000000000000000a6000000ab00000000
-                  000000000001007c037c02660253002300740c0000000000000000000024
-                  0072277d067c006a000000000000000000a0070000000000000000000000
+                  0x87029700090067007d0488026601640184087c034400a6000000ab0000
+                  000000000000007d057c01a0000000000000000000000000000000000000
+                  0000007c05a6010000ab01000000000000000001007c01a0010000000000
+                  000000000000000000000000000000a6000000ab00000000000000000001
+                  00640284007c054400a6000000ab0000000000000000007d037c0544005d
+                  1c7d067c04a00200000000000000000000000000000000000000007c066a
+                  030000000000000000a6010000ab01000000000000000001008c1d7c01a0
+                  040000000000000000000000000000000000000000a6000000ab00000000
+                  000000000001007c047c03660253002300740a0000000000000000000024
+                  0072277d077c006a060000000000000000a0070000000000000000000000
                   000000000000000000a6000000ab00000000000000000001006700670066
-                  026302590064007d067e06530064007d067e0677017700780359007701
-                             0 MAKE_CELL                1 (model)
+                  026302590064007d077e07530064007d077e0777017700780359007701
+                             0 MAKE_CELL                2 (model)
                
-               116           2 RESUME                   0
+               123           2 RESUME                   0
                
-               119           4 NOP
+               126           4 NOP
                
-               120           6 BUILD_LIST               0
-                             8 STORE_FAST               3 (inserted_ids)
+               127           6 BUILD_LIST               0
+                             8 STORE_FAST               4 (inserted_ids)
                
-               122          10 LOAD_CLOSURE             1 (model)
+               129          10 LOAD_CLOSURE             2 (model)
                             12 BUILD_TUPLE              1
-                            14 LOAD_CONST               1 (<code object <listcomp>, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 122>)
+                            14 LOAD_CONST               1 (<code object <listcomp>, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 129>)
                             16 MAKE_FUNCTION            8 (closure)
-                            18 LOAD_FAST                2 (records)
+                            18 LOAD_FAST                3 (records)
                             20 GET_ITER
                             22 PRECALL                  0
                             26 CALL                     0
-                            36 STORE_FAST               4 (records_to_insert)
+                            36 STORE_FAST               5 (records_to_insert)
+               
+               131          38 LOAD_FAST                1 (session)
+                            40 LOAD_METHOD              0 (add_all)
+                            62 LOAD_FAST                5 (records_to_insert)
+                            64 PRECALL                  1
+                            68 CALL                     1
+                            78 POP_TOP
+               
+               132          80 LOAD_FAST                1 (session)
+                            82 LOAD_METHOD              1 (flush)
+                           104 PRECALL                  0
+                           108 CALL                     0
+                           118 POP_TOP
+               
+               134         120 LOAD_CONST               2 (<code object <listcomp>, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py", line 134>)
+                           122 MAKE_FUNCTION            0
+                           124 LOAD_FAST                5 (records_to_insert)
+                           126 GET_ITER
+                           128 PRECALL                  0
+                           132 CALL                     0
+                           142 STORE_FAST               3 (records)
                
-               124          38 LOAD_FAST                0 (cls)
-                            40 LOAD_ATTR                0 (session)
-                            50 LOAD_METHOD              1 (add_all)
-                            72 LOAD_FAST                4 (records_to_insert)
-                            74 PRECALL                  1
-                            78 CALL                     1
-                            88 POP_TOP
-               
-               125          90 LOAD_FAST                0 (cls)
-                            92 LOAD_ATTR                0 (session)
-                           102 LOAD_METHOD              2 (flush)
-                           124 PRECALL                  0
-                           128 CALL                     0
-                           138 POP_TOP
-               
-               127         140 LOAD_CONST               2 (<code object <listcomp>, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 127>)
-                           142 MAKE_FUNCTION            0
-                           144 LOAD_FAST                4 (records_to_insert)
+               135         144 LOAD_FAST                5 (records_to_insert)
                            146 GET_ITER
-                           148 PRECALL                  0
-                           152 CALL                     0
-                           162 STORE_FAST               2 (records)
-               
-               128         164 LOAD_FAST                4 (records_to_insert)
-                           166 GET_ITER
-                       >>  168 FOR_ITER                28 (to 226)
-                           170 STORE_FAST               5 (record)
-               
-               129         172 LOAD_FAST                3 (inserted_ids)
-                           174 LOAD_METHOD              3 (append)
-                           196 LOAD_FAST                5 (record)
-                           198 LOAD_ATTR                4 (uuid)
-                           208 PRECALL                  1
-                           212 CALL                     1
-                           222 POP_TOP
-                           224 JUMP_BACKWARD           29 (to 168)
-               
-               130     >>  226 LOAD_FAST                0 (cls)
-                           228 LOAD_ATTR                0 (session)
-                           238 LOAD_METHOD              5 (commit)
-                           260 PRECALL                  0
-                           264 CALL                     0
-                           274 POP_TOP
+                       >>  148 FOR_ITER                28 (to 206)
+                           150 STORE_FAST               6 (record)
                
-               131         276 LOAD_FAST                3 (inserted_ids)
-                           278 LOAD_FAST                2 (records)
-                           280 BUILD_TUPLE              2
-                           282 RETURN_VALUE
-                       >>  284 PUSH_EXC_INFO
-               
-               132         286 LOAD_GLOBAL             12 (DBAPIError)
-                           298 CHECK_EXC_MATCH
-                           300 POP_JUMP_FORWARD_IF_FALSE    39 (to 380)
-                           302 STORE_FAST               6 (e)
-               
-               133         304 LOAD_FAST                0 (cls)
-                           306 LOAD_ATTR                0 (session)
-                           316 LOAD_METHOD              7 (rollback)
-                           338 PRECALL                  0
-                           342 CALL                     0
-                           352 POP_TOP
-               
-               135         354 BUILD_LIST               0
-                           356 BUILD_LIST               0
-                           358 BUILD_TUPLE              2
-                           360 SWAP                     2
-                           362 POP_EXCEPT
-                           364 LOAD_CONST               0 (None)
-                           366 STORE_FAST               6 (e)
-                           368 DELETE_FAST              6 (e)
-                           370 RETURN_VALUE
-                       >>  372 LOAD_CONST               0 (None)
-                           374 STORE_FAST               6 (e)
-                           376 DELETE_FAST              6 (e)
-                           378 RERAISE                  1
-               
-               132     >>  380 RERAISE                  0
-                       >>  382 COPY                     3
-                           384 POP_EXCEPT
-                           386 RERAISE                  1
+               136         152 LOAD_FAST                4 (inserted_ids)
+                           154 LOAD_METHOD              2 (append)
+                           176 LOAD_FAST                6 (record)
+                           178 LOAD_ATTR                3 (uuid)
+                           188 PRECALL                  1
+                           192 CALL                     1
+                           202 POP_TOP
+                           204 JUMP_BACKWARD           29 (to 148)
+               
+               137     >>  206 LOAD_FAST                1 (session)
+                           208 LOAD_METHOD              4 (commit)
+                           230 PRECALL                  0
+                           234 CALL                     0
+                           244 POP_TOP
+               
+               138         246 LOAD_FAST                4 (inserted_ids)
+                           248 LOAD_FAST                3 (records)
+                           250 BUILD_TUPLE              2
+                           252 RETURN_VALUE
+                       >>  254 PUSH_EXC_INFO
+               
+               139         256 LOAD_GLOBAL             10 (DBAPIError)
+                           268 CHECK_EXC_MATCH
+                           270 POP_JUMP_FORWARD_IF_FALSE    39 (to 350)
+                           272 STORE_FAST               7 (e)
+               
+               140         274 LOAD_FAST                0 (cls)
+                           276 LOAD_ATTR                6 (session)
+                           286 LOAD_METHOD              7 (rollback)
+                           308 PRECALL                  0
+                           312 CALL                     0
+                           322 POP_TOP
+               
+               142         324 BUILD_LIST               0
+                           326 BUILD_LIST               0
+                           328 BUILD_TUPLE              2
+                           330 SWAP                     2
+                           332 POP_EXCEPT
+                           334 LOAD_CONST               0 (None)
+                           336 STORE_FAST               7 (e)
+                           338 DELETE_FAST              7 (e)
+                           340 RETURN_VALUE
+                       >>  342 LOAD_CONST               0 (None)
+                           344 STORE_FAST               7 (e)
+                           346 DELETE_FAST              7 (e)
+                           348 RERAISE                  1
+               
+               139     >>  350 RERAISE                  0
+                       >>  352 COPY                     3
+                           354 POP_EXCEPT
+                           356 RERAISE                  1
                ExceptionTable:
-                 6 to 280 -> 284 [0]
-                 284 to 302 -> 382 [1] lasti
-                 304 to 358 -> 372 [1] lasti
-                 360 to 360 -> 382 [1] lasti
-                 372 to 380 -> 382 [1] lasti
+                 6 to 250 -> 254 [0]
+                 254 to 272 -> 352 [1] lasti
+                 274 to 328 -> 342 [1] lasti
+                 330 to 330 -> 352 [1] lasti
+                 342 to 350 -> 352 [1] lasti
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 7
                      flags     : 19
                      code
                         0x9501970067007c005d0a7d0102008902640069007c01a4018e0191028c
                         0b5300
                                    0 COPY_FREE_VARS           1
                      
-                     122           2 RESUME                   0
+                     129           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                10 (to 30)
                                   10 STORE_FAST               1 (record)
                                   12 PUSH_NULL
                                   14 LOAD_DEREF               2 (model)
                                   16 LOAD_CONST               0 (())
@@ -1258,27 +1302,27 @@
                              >>   30 RETURN_VALUE
                      consts
                         ()
                      names      ()
                      varnames   ('.0', 'record')
                      freevars   ('model',)
                      cellvars   ()
-                     filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+                     filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                      name       '<listcomp>'
-                     firstlineno 122
+                     firstlineno 129
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d167d017c01a000000000000000000000000000000000
                         0000000000a6000000ab00000000000000000091028c175300
-                     127           0 RESUME                   0
+                     134           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                22 (to 52)
                                    8 STORE_FAST               1 (record)
                                   10 LOAD_FAST                1 (record)
                                   12 LOAD_METHOD              0 (to_dict)
                                   34 PRECALL                  0
@@ -1287,209 +1331,199 @@
                                   50 JUMP_BACKWARD           23 (to 6)
                              >>   52 RETURN_VALUE
                      consts
                      names      ('to_dict',)
                      varnames   ('.0', 'record')
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+                     filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                      name       '<listcomp>'
-                     firstlineno 127
+                     firstlineno 134
                      lnotab 0x
-               names      ('session', 'add_all', 'flush', 'append', 'uuid', 'commit', 'DBAPIError', 'rollback')
-               varnames   ('cls', 'model', 'records', 'inserted_ids', 'records_to_insert', 'record', 'e')
+               names      ('add_all', 'flush', 'append', 'uuid', 'commit', 'DBAPIError', 'session', 'rollback')
+               varnames   ('cls', 'session', 'model', 'records', 'inserted_ids', 'records_to_insert', 'record', 'e')
                freevars   ()
                cellvars   ('model',)
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                name       'add_records_sync'
-               firstlineno 116
-               lnotab 0x0403020104021c023401320218010801360132010a01120132021afd
+               firstlineno 123
+               lnotab 0x0403020104021c022a01280218010801360128010a01120132021afd
             code
-               argcount  : 3
-               nlocals   : 4
+               argcount  : 4
+               nlocals   : 5
                stacksize : 5
                flags     : 3
                code
-                  0x970009007c006a000000000000000000a0010000000000000000000000
-                  0000000000000000007c01a6010000ab010000000000000000a002000000
-                  00000000000000000000000000000000007c016a030000000000000000a0
-                  0400000000000000000000000000000000000000007c02a6010000ab0100
-                  00000000000000a6010000ab010000000000000000a00500000000000000
-                  000000000000000000000000006401ac02a6010000ab0100000000000000
-                  0001007c006a000000000000000000a00600000000000000000000000000
-                  00000000000000a6000000ab000000000000000000010064035300230074
-                  0e00000000000000000000240072247d037c006a000000000000000000a0
-                  080000000000000000000000000000000000000000a6000000ab00000000
-                  00000000000100590064007d037e036401530064007d037e037701770078
+                  0x970009007c01a00000000000000000000000000000000000000000007c
+                  02a6010000ab010000000000000000a00100000000000000000000000000
+                  000000000000007c026a020000000000000000a003000000000000000000
+                  00000000000000000000007c03a6010000ab010000000000000000a60100
+                  00ab010000000000000000a0040000000000000000000000000000000000
+                  0000006401ac02a6010000ab01000000000000000001007c01a005000000
+                  0000000000000000000000000000000000a6000000ab0000000000000000
+                  000100640353002300740c000000000000000000002400721f7d047c01a0
+                  070000000000000000000000000000000000000000a6000000ab00000000
+                  00000000000100590064007d047e046401530064007d047e047701770078
                   0359007701
-               138           0 RESUME                   0
+               145           0 RESUME                   0
+               
+               148           2 NOP
                
-               141           2 NOP
+               149           4 LOAD_FAST                1 (session)
+                             6 LOAD_METHOD              0 (query)
+                            28 LOAD_FAST                2 (model)
+                            30 PRECALL                  1
+                            34 CALL                     1
+                            44 LOAD_METHOD              1 (filter)
+                            66 LOAD_FAST                2 (model)
+                            68 LOAD_ATTR                2 (uuid)
+                            78 LOAD_METHOD              3 (in_)
+                           100 LOAD_FAST                3 (records)
+                           102 PRECALL                  1
+                           106 CALL                     1
+                           116 PRECALL                  1
+                           120 CALL                     1
+                           130 LOAD_METHOD              4 (delete)
+               
+               150         152 LOAD_CONST               1 (False)
+               
+               149         154 KW_NAMES                 2
+                           156 PRECALL                  1
+                           160 CALL                     1
+                           170 POP_TOP
+               
+               152         172 LOAD_FAST                1 (session)
+                           174 LOAD_METHOD              5 (commit)
+                           196 PRECALL                  0
+                           200 CALL                     0
+                           210 POP_TOP
+               
+               154         212 LOAD_CONST               3 (True)
+                           214 RETURN_VALUE
+                       >>  216 PUSH_EXC_INFO
+               
+               155         218 LOAD_GLOBAL             12 (DBAPIError)
+                           230 CHECK_EXC_MATCH
+                           232 POP_JUMP_FORWARD_IF_FALSE    31 (to 296)
+                           234 STORE_FAST               4 (e)
+               
+               156         236 LOAD_FAST                1 (session)
+                           238 LOAD_METHOD              7 (rollback)
+                           260 PRECALL                  0
+                           264 CALL                     0
+                           274 POP_TOP
                
-               142           4 LOAD_FAST                0 (cls)
-                             6 LOAD_ATTR                0 (session)
-                            16 LOAD_METHOD              1 (query)
-                            38 LOAD_FAST                1 (model)
-                            40 PRECALL                  1
-                            44 CALL                     1
-                            54 LOAD_METHOD              2 (filter)
-                            76 LOAD_FAST                1 (model)
-                            78 LOAD_ATTR                3 (uuid)
-                            88 LOAD_METHOD              4 (in_)
-                           110 LOAD_FAST                2 (records)
-                           112 PRECALL                  1
-                           116 CALL                     1
-                           126 PRECALL                  1
-                           130 CALL                     1
-                           140 LOAD_METHOD              5 (delete)
-               
-               143         162 LOAD_CONST               1 (False)
-               
-               142         164 KW_NAMES                 2
-                           166 PRECALL                  1
-                           170 CALL                     1
-                           180 POP_TOP
-               
-               145         182 LOAD_FAST                0 (cls)
-                           184 LOAD_ATTR                0 (session)
-                           194 LOAD_METHOD              6 (commit)
-                           216 PRECALL                  0
-                           220 CALL                     0
-                           230 POP_TOP
-               
-               147         232 LOAD_CONST               3 (True)
-                           234 RETURN_VALUE
-                       >>  236 PUSH_EXC_INFO
-               
-               148         238 LOAD_GLOBAL             14 (DBAPIError)
-                           250 CHECK_EXC_MATCH
-                           252 POP_JUMP_FORWARD_IF_FALSE    36 (to 326)
-                           254 STORE_FAST               3 (e)
-               
-               149         256 LOAD_FAST                0 (cls)
-                           258 LOAD_ATTR                0 (session)
-                           268 LOAD_METHOD              8 (rollback)
-                           290 PRECALL                  0
-                           294 CALL                     0
-                           304 POP_TOP
-               
-               151         306 POP_EXCEPT
-                           308 LOAD_CONST               0 (None)
-                           310 STORE_FAST               3 (e)
-                           312 DELETE_FAST              3 (e)
-                           314 LOAD_CONST               1 (False)
-                           316 RETURN_VALUE
-                       >>  318 LOAD_CONST               0 (None)
-                           320 STORE_FAST               3 (e)
-                           322 DELETE_FAST              3 (e)
-                           324 RERAISE                  1
-               
-               148     >>  326 RERAISE                  0
-                       >>  328 COPY                     3
-                           330 POP_EXCEPT
-                           332 RERAISE                  1
+               158         276 POP_EXCEPT
+                           278 LOAD_CONST               0 (None)
+                           280 STORE_FAST               4 (e)
+                           282 DELETE_FAST              4 (e)
+                           284 LOAD_CONST               1 (False)
+                           286 RETURN_VALUE
+                       >>  288 LOAD_CONST               0 (None)
+                           290 STORE_FAST               4 (e)
+                           292 DELETE_FAST              4 (e)
+                           294 RERAISE                  1
+               
+               155     >>  296 RERAISE                  0
+                       >>  298 COPY                     3
+                           300 POP_EXCEPT
+                           302 RERAISE                  1
                ExceptionTable:
-                 4 to 230 -> 236 [0]
-                 236 to 254 -> 328 [1] lasti
-                 256 to 304 -> 318 [1] lasti
-                 318 to 326 -> 328 [1] lasti
+                 4 to 210 -> 216 [0]
+                 216 to 234 -> 298 [1] lasti
+                 236 to 274 -> 288 [1] lasti
+                 288 to 296 -> 298 [1] lasti
                consts
                   None
                   False
                   ('synchronize_session',)
                   True
-               names      ('session', 'query', 'filter', 'uuid', 'in_', 'delete', 'commit', 'DBAPIError', 'rollback')
-               varnames   ('cls', 'model', 'records', 'e')
+               names      ('query', 'filter', 'uuid', 'in_', 'delete', 'commit', 'DBAPIError', 'rollback')
+               varnames   ('cls', 'session', 'model', 'records', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
                name       'remove_records_sync'
-               firstlineno 138
-               lnotab 0x020302019e0102ff1203320206011201320214fd
+               firstlineno 145
+               lnotab 0x02030201940102ff1203280206011201280214fd
          names      ('__name__', '__module__', '__qualname__', '__init__', 'Session', 'initialize', 'staticmethod', 'str', 'text', 'wrap_to_json', 'Union', 'List', 'dict', 'select_stmt_raw_sql', 'bool', 'execute_stmt_raw_sql', 'select_stmt_raw_sql_params', 'object', 'add_record_sync', 'BaseModel', 'uuid', 'UUID', 'add_records_sync', 'remove_records_sync')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
          name       'DBUtils'
-         firstlineno 51
+         firstlineno 57
          lnotab
-            0x0a0206030c0302010eff0e0102052c0b200a020202fe020302fd02041e
-            fc08121c0c020102ff02010eff020234fe0816020102ff020118ff020202
-            fe
+            0x0a0206030c0302010eff0e010205300b240a020202fe020302fd020402
+            fc02051efb0813200c020102ff020102ff02010eff020234fe0816020102
+            ff020102ff020118ff020202fe
       'DBUtils'
       'url'
       'return'
       code
          argcount  : 1
-         nlocals   : 2
-         stacksize : 6
-         flags     : 3
+         nlocals   : 3
+         stacksize : 5
+         flags     : 11
          code
-            0x970009007401000000000000000000007c00640164026403ac04a60400
-            00ab04000000000000000053002300740200000000000000000000240072
-            077d017c01820164007d017e0177017700780359007701
-         154           0 RESUME                   0
-         
-         155           2 NOP
-         
-         156           4 LOAD_GLOBAL              1 (NULL + create_engine)
-         
-         157          16 LOAD_FAST                0 (url)
-         
-         158          18 LOAD_CONST               1 (5)
-         
-         159          20 LOAD_CONST               2 (0)
-         
-         160          22 LOAD_CONST               3 (True)
-         
-         156          24 KW_NAMES                 4
-                      26 PRECALL                  4
-                      30 CALL                     4
-                      40 RETURN_VALUE
-                 >>   42 PUSH_EXC_INFO
-         
-         162          44 LOAD_GLOBAL              2 (DBAPIError)
-                      56 CHECK_EXC_MATCH
-                      58 POP_JUMP_FORWARD_IF_FALSE     7 (to 74)
-                      60 STORE_FAST               1 (e)
-         
-         164          62 LOAD_FAST                1 (e)
-                      64 RAISE_VARARGS            1
-                 >>   66 LOAD_CONST               0 (None)
-                      68 STORE_FAST               1 (e)
-                      70 DELETE_FAST              1 (e)
-                      72 RERAISE                  1
-         
-         162     >>   74 RERAISE                  0
-                 >>   76 COPY                     3
-                      78 POP_EXCEPT
-                      80 RERAISE                  1
+            0x970009007401000000000000000000007c00660169007c01a4018e0153
+            002300740200000000000000000000240072077d027c02820164007d027e
+            0277017700780359007701
+         161           0 RESUME                   0
+         
+         162           2 NOP
+         
+         163           4 LOAD_GLOBAL              1 (NULL + create_engine)
+         
+         164          16 LOAD_FAST                0 (url)
+         
+         163          18 BUILD_TUPLE              1
+                      20 BUILD_MAP                0
+         
+         165          22 LOAD_FAST                1 (kwargs)
+         
+         163          24 DICT_MERGE               1
+                      26 CALL_FUNCTION_EX         1
+                      28 RETURN_VALUE
+                 >>   30 PUSH_EXC_INFO
+         
+         170          32 LOAD_GLOBAL              2 (DBAPIError)
+                      44 CHECK_EXC_MATCH
+                      46 POP_JUMP_FORWARD_IF_FALSE     7 (to 62)
+                      48 STORE_FAST               2 (e)
+         
+         172          50 LOAD_FAST                2 (e)
+                      52 RAISE_VARARGS            1
+                 >>   54 LOAD_CONST               0 (None)
+                      56 STORE_FAST               2 (e)
+                      58 DELETE_FAST              2 (e)
+                      60 RERAISE                  1
+         
+         170     >>   62 RERAISE                  0
+                 >>   64 COPY                     3
+                      66 POP_EXCEPT
+                      68 RERAISE                  1
          ExceptionTable:
-           4 to 38 -> 42 [0]
-           42 to 60 -> 76 [1] lasti
-           62 to 64 -> 66 [1] lasti
-           66 to 74 -> 76 [1] lasti
+           4 to 26 -> 30 [0]
+           30 to 48 -> 64 [1] lasti
+           50 to 52 -> 54 [1] lasti
+           54 to 62 -> 64 [1] lasti
          consts
             None
-            5
-            0
-            True
-            ('pool_size', 'max_overflow', 'pool_pre_ping')
          names      ('create_engine', 'DBAPIError')
-         varnames   ('url', 'e')
+         varnames   ('url', 'kwargs', 'e')
          freevars   ()
          cellvars   ()
-         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
          name       'get_engine'
-         firstlineno 154
-         lnotab 0x020102010c0102010201020102fc140612020cfe
+         firstlineno 161
+         lnotab 0x020102010c0102ff040202fe080712020cfe
    names      ('tva_utils.postgres.schemas', 'BaseModel', 'sqlalchemy.exc', 'DBAPIError', 'sqlalchemy.orm.session', 'Session', 'sqlalchemy', 'text', 'inspect', 'create_engine', 'sqlalchemy.engine.base', 'Engine', 'sqlalchemy.orm', 'sessionmaker', 'scoped_session', 'DeclarativeMeta', 'typing', 'List', 'Union', 'Iterator', 'uuid', 'DB', 'DBUtils', 'str', 'get_engine', 'db')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
+   filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/funcs.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c020c010c0110010c010c0110010c010802140108031a231a
-      67100c
+      0x00ff02010c020c010c0110010c010c0110010c010802140108031a291a
+      68100d
```

### Comparing `tva_utils-0.1.5/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc` & `tva_utils-0.1.6/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.5/tva_utils/postgres/funcs.py` & `tva_utils-0.1.6/tva_utils/postgres/funcs.py`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.5/tva_utils/postgres/schemas.py` & `tva_utils-0.1.6/tva_utils/postgres/schemas.py`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.5/tva_utils/timers/timers.py` & `tva_utils-0.1.6/tva_utils/logging/logging.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 import logging
 import time
 from stringcolor import bold
 
-logger = logging.getLogger()
 
-def timer_decorator(func):
-    def wrapper(*args, **kwargs):
-        start_time = time.perf_counter()  # get current time before function execution
-        result = func(*args, **kwargs)  # function execution
-        end_time = time.perf_counter()  # get current time after function execution
-        run_time = end_time - start_time  # calculate execution time
-        run_time = f"{run_time:.4f}"
-        func_name = bold(func.__name__).cs("blue")
-        run_time = bold(run_time).cs("green")
-
-        logger.info(f"Finished {func_name} in {run_time} seconds")
-        return result
-
-    return wrapper
-
-
-def timer_decorator_async(func):
-    async def wrapper(*args, **kwargs):
-        start_time = time.perf_counter()
-        result = await func(*args, **kwargs)
-        end_time = time.perf_counter()  # get current time after function execution
-        run_time = end_time - start_time  # calculate execution time
-        run_time = f"{run_time:.4f}"
-        func_name = bold(func.__name__).cs("blue")
-        run_time = bold(run_time).cs("green")
 
-        logger.info(f"Finished {func_name} in {run_time} seconds")
-        return result
+def timer_decorator(logger: logging.Logger):
+    def actual_decorator(func):
+        def wrapper(*args, **kwargs):
+            start_time = time.perf_counter()  # get current time before function execution
+            result = func(*args, **kwargs)  # function execution
+            end_time = time.perf_counter()  # get current time after function execution
+            run_time = end_time - start_time  # calculate execution time
+            run_time = f"{run_time:.4f}"
+            func_name = bold(func.__name__).cs("blue")
+            run_time = bold(run_time).cs("green")
+
+            logger.info(f"Finished {func_name} in {run_time} seconds")
+            return result
+
+        return wrapper
+    return actual_decorator
+
+
+def timer_decorator_async(logger: logging.Logger):
+    def actual_decorator(func):
+        async def wrapper(*args, **kwargs):
+            start_time = time.perf_counter()
+            result = await func(*args, **kwargs)
+            end_time = time.perf_counter()  # get current time after function execution
+            run_time = end_time - start_time  # calculate execution time
+            run_time = f"{run_time:.4f}"
+            func_name = bold(func.__name__).cs("blue")
+            run_time = bold(run_time).cs("green")
 
-    return wrapper
+            logger.info(f"Finished {func_name} in {run_time} seconds")
+            return result
+
+        return wrapper
+    return actual_decorator
```

### Comparing `tva_utils-0.1.5/PKG-INFO` & `tva_utils-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tva-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: jsaied99
 Author-email: jsaied99@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

