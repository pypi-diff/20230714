# Comparing `tmp/tva_utils-0.1.1.tar.gz` & `tmp/tva_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tva_utils-0.1.1.tar", max compression
+gzip compressed data, was "tva_utils-0.1.2.tar", max compression
```

## Comparing `tva_utils-0.1.1.tar` & `tva_utils-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.1/README.md
--rw-r--r--   0        0        0      325 2023-07-14 00:40:22.606743 tva_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       52 2023-07-14 00:02:24.445394 tva_utils-0.1.1/tva_utils/__init__.py
--rw-r--r--   0        0        0      133 2023-07-14 00:16:30.253118 tva_utils-0.1.1/tva_utils/db/__init__.py
--rw-r--r--   0        0        0      375 2023-07-14 00:16:33.202871 tva_utils-0.1.1/tva_utils/db/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9672 2023-07-14 00:30:09.267273 tva_utils-0.1.1/tva_utils/db/__pycache__/postgres.cpython-311.pyc
--rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.1/tva_utils/db/__pycache__/schemas.cpython-311.pyc
--rw-r--r--   0        0        0     4786 2023-07-14 00:32:32.607265 tva_utils-0.1.1/tva_utils/db/postgres.py
--rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.1/tva_utils/db/schemas.py
--rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 tva_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-13 23:17:23.166450 tva_utils-0.1.2/README.md
+-rw-r--r--   0        0        0      352 2023-07-14 00:51:10.088678 tva_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-07-14 00:50:32.767732 tva_utils-0.1.2/tva_utils/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-14 00:50:27.683031 tva_utils-0.1.2/tva_utils/postgres/__init__.py
+-rw-r--r--   0        0        0      430 2023-07-14 00:50:45.402621 tva_utils-0.1.2/tva_utils/postgres/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9650 2023-07-14 00:50:45.404384 tva_utils-0.1.2/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc
+-rw-r--r--   0        0        0     1887 2023-07-14 00:16:18.073842 tva_utils-0.1.2/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc
+-rw-r--r--   0        0        0     4809 2023-07-14 00:50:10.421521 tva_utils-0.1.2/tva_utils/postgres/postgres.py
+-rw-r--r--   0        0        0      655 2023-07-13 23:44:23.809176 tva_utils-0.1.2/tva_utils/postgres/schemas.py
+-rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 tva_utils-0.1.2/PKG-INFO
```

### Comparing `tva_utils-0.1.1/tva_utils/db/__pycache__/postgres.cpython-311.pyc` & `tva_utils-0.1.2/tva_utils/postgres/__pycache__/postgres.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,29 +1,29 @@
 magic:    0xa70d0d0a
-moddate:  0xe996b064 (Fri Jul 14 00:29:29 2023 UTC)
-files sz: 4786
+moddate:  0xc29bb064 (Fri Jul 14 00:50:10 2023 UTC)
+files sz: 4809
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a050100640064046c066d075a076d085a080100640064056c
       066d095a090100640064066c0a6d0b5a0b0100640064076c0c6d0d5a0d6d
       0e5a0e0100640064086c0c6d0f5a0f0100640064096c065a066400640a6c
       106d115a116d125a126d135a130100640064096c145a1402004700640b84
       00640ca6020000ab0200000000000000005a1502004700640d8400640ea6
       020000ab0200000000000000005a16640f65176410650b6604641184045a
-      1864095300
+      1802006515a6000000ab0000000000000000005a1964095300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('BaseModel',))
-                 6 IMPORT_NAME              0 (tva_utils.db.schemas)
+                 6 IMPORT_NAME              0 (tva_utils.postgres.schemas)
                  8 IMPORT_FROM              1 (BaseModel)
                 10 STORE_NAME               1 (BaseModel)
                 12 POP_TOP
    
      3          14 LOAD_CONST               0 (0)
                 16 LOAD_CONST               2 (('DBAPIError',))
                 18 IMPORT_NAME              2 (sqlalchemy.exc)
@@ -96,40 +96,46 @@
     13         134 LOAD_CONST               0 (0)
                136 LOAD_CONST               9 (None)
                138 IMPORT_NAME             20 (uuid)
                140 STORE_NAME              20 (uuid)
    
     16         142 PUSH_NULL
                144 LOAD_BUILD_CLASS
-               146 LOAD_CONST              11 (<code object DB, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 16>)
+               146 LOAD_CONST              11 (<code object DB, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 16>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST              12 ('DB')
                152 PRECALL                  2
                156 CALL                     2
                166 STORE_NAME              21 (DB)
    
     51         168 PUSH_NULL
                170 LOAD_BUILD_CLASS
-               172 LOAD_CONST              13 (<code object DBUtils, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 51>)
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
-               204 LOAD_CONST              17 (<code object get_engine, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 154>)
+               204 LOAD_CONST              17 (<code object get_engine, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 154>)
                206 MAKE_FUNCTION            4 (annotations)
                208 STORE_NAME              24 (get_engine)
-               210 LOAD_CONST               9 (None)
-               212 RETURN_VALUE
+   
+   166         210 PUSH_NULL
+               212 LOAD_NAME               21 (DB)
+               214 PRECALL                  0
+               218 CALL                     0
+               228 STORE_NAME              25 (db)
+               230 LOAD_CONST               9 (None)
+               232 RETURN_VALUE
    consts
       0
       ('BaseModel',)
       ('DBAPIError',)
       ('Session',)
       ('text', 'inspect')
       ('create_engine',)
@@ -153,48 +159,48 @@
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DB')
                        8 STORE_NAME               2 (__qualname__)
          
           17          10 LOAD_CONST               1 ('url')
                       12 LOAD_NAME                3 (str)
                       14 BUILD_TUPLE              2
-                      16 LOAD_CONST               2 (<code object initialize, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 17>)
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
-                      56 LOAD_CONST               5 (<code object _create_tables, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 27>)
+                      56 LOAD_CONST               5 (<code object _create_tables, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 27>)
                       58 MAKE_FUNCTION            4 (annotations)
                       60 STORE_NAME               7 (_create_tables)
          
           37          62 LOAD_CONST               6 ('return')
                       64 LOAD_NAME                8 (Iterator)
                       66 LOAD_NAME                9 (Session)
                       68 BINARY_SUBSCR
                       78 BUILD_TUPLE              2
-                      80 LOAD_CONST               7 (<code object get_session, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 37>)
+                      80 LOAD_CONST               7 (<code object get_session, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 37>)
                       82 MAKE_FUNCTION            4 (annotations)
                       84 STORE_NAME              10 (get_session)
          
           44          86 LOAD_CONST               6 ('return')
                       88 LOAD_NAME               11 (scoped_session)
                       90 BUILD_TUPLE              2
-                      92 LOAD_CONST               8 (<code object get_session_scoped, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 44>)
+                      92 LOAD_CONST               8 (<code object get_session_scoped, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 44>)
                       94 MAKE_FUNCTION            4 (annotations)
                       96 STORE_NAME              12 (get_session_scoped)
          
-          47          98 LOAD_CONST               9 (<code object close, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 47>)
+          47          98 LOAD_CONST               9 (<code object close, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 47>)
                      100 MAKE_FUNCTION            0
                      102 STORE_NAME              13 (close)
                      104 LOAD_CONST              10 (None)
                      106 RETURN_VALUE
          consts
             'DB'
             'url'
@@ -206,16 +212,15 @@
                code
                   0x97007401000000000000000000007c01a6010000ab0100000000000000
                   007c005f010000000000000000740500000000000000000000640164017c
                   006a010000000000000000ac02a6030000ab0300000000000000007c005f
                   0300000000000000007409000000000000000000007c006a010000000000
                   000000a6010000ab0100000000000000007c005f05000000000000000074
                   0d00000000000000000000a6000000ab0000000000000000007c005f0700
-                  000000000000007c00a00800000000000000000000000000000000000000
-                  00a6000000ab000000000000000000010064005300
+                  0000000000000064005300
                 17           0 RESUME                   0
                
                 18           2 LOAD_GLOBAL              1 (NULL + get_engine)
                             14 LOAD_FAST                1 (url)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 LOAD_FAST                0 (cls)
@@ -243,34 +248,28 @@
                            138 STORE_ATTR               5 (inspector)
                
                 23         148 LOAD_GLOBAL             13 (NULL + DBUtils)
                            160 PRECALL                  0
                            164 CALL                     0
                            174 LOAD_FAST                0 (cls)
                            176 STORE_ATTR               7 (utils)
-               
-                25         186 LOAD_FAST                0 (cls)
-                           188 LOAD_METHOD              8 (_create_tables)
-                           210 PRECALL                  0
-                           214 CALL                     0
-                           224 POP_TOP
-                           226 LOAD_CONST               0 (None)
-                           228 RETURN_VALUE
+                           186 LOAD_CONST               0 (None)
+                           188 RETURN_VALUE
                consts
                   None
                   False
                   ('autocommit', 'autoflush', 'bind')
-               names      ('get_engine', 'engine', 'sessionmaker', 'SessionLocal', 'inspect', 'inspector', 'DBUtils', 'utils', '_create_tables')
+               names      ('get_engine', 'engine', 'sessionmaker', 'SessionLocal', 'inspect', 'inspector', 'DBUtils', 'utils')
                varnames   ('cls', 'url')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'initialize'
                firstlineno 17
-               lnotab 0x020128010c0110ff1c0332012602
+               lnotab 0x020128010c0110ff1c033201
             'Bases'
             'schemas'
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 6
                flags     : 3
@@ -369,15 +368,15 @@
                  334 to 342 -> 344 [2] lasti
                consts
                   None
                names      ('zip', 'inspector', 'get_schema_names', 'engine', 'execute', 'sqlalchemy', 'schema', 'CreateSchema', 'metadata', 'create_all', 'Exception', 'print')
                varnames   ('cls', 'Bases', 'schemas', 'Base', 'schema', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       '_create_tables'
                firstlineno 27
                lnotab 0x02022a01020136016e014201120130ff08fb
             'return'
             code
                argcount  : 1
                nlocals   : 2
@@ -458,15 +457,15 @@
                  192 to 192 -> 186 [3] lasti
                consts
                   None
                names      ('SessionLocal', 'close')
                varnames   ('cls', 'session')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'get_session'
                firstlineno 37
                lnotab 0x06012a01020108025efc
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -484,15 +483,15 @@
                             40 RETURN_VALUE
                consts
                   None
                names      ('scoped_session', 'SessionLocal')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'get_session_scoped'
                firstlineno 44
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
@@ -512,24 +511,24 @@
                             54 RETURN_VALUE
                consts
                   None
                names      ('engine', 'dispose')
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'close'
                firstlineno 47
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'str', 'initialize', 'List', 'DeclarativeMeta', '_create_tables', 'Iterator', 'Session', 'get_session', 'scoped_session', 'get_session_scoped', 'close')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
          name       'DB'
          firstlineno 16
          lnotab 0x0a010c0a280a18070c03
       'DB'
       code
          argcount  : 0
          nlocals   : 0
@@ -550,33 +549,33 @@
             06641184045a1764085300
           51           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DBUtils')
                        8 STORE_NAME               2 (__qualname__)
          
-          53          10 LOAD_CONST               1 (<code object __init__, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 53>)
+          53          10 LOAD_CONST               1 (<code object __init__, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 53>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
           56          16 LOAD_CONST               2 ('session')
                       18 LOAD_NAME                4 (Session)
                       20 BUILD_TUPLE              2
-                      22 LOAD_CONST               3 (<code object initialize, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 56>)
+                      22 LOAD_CONST               3 (<code object initialize, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 56>)
                       24 MAKE_FUNCTION            4 (annotations)
                       26 STORE_NAME               5 (initialize)
          
           59          28 LOAD_NAME                6 (staticmethod)
          
           60          30 LOAD_CONST               4 ('stmt')
                       32 LOAD_NAME                7 (str)
                       34 LOAD_CONST               5 ('return')
                       36 LOAD_NAME                8 (text)
                       38 BUILD_TUPLE              4
-                      40 LOAD_CONST               6 (<code object wrap_to_json, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 59>)
+                      40 LOAD_CONST               6 (<code object wrap_to_json, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 59>)
                       42 MAKE_FUNCTION            4 (annotations)
          
           59          44 PRECALL                  0
                       48 CALL                     0
          
           60          58 STORE_NAME               9 (wrap_to_json)
          
@@ -587,28 +586,28 @@
                       68 LOAD_NAME               11 (List)
                       70 LOAD_NAME               12 (dict)
                       72 BINARY_SUBSCR
                       82 LOAD_CONST               8 (None)
                       84 BUILD_TUPLE              2
                       86 BINARY_SUBSCR
                       96 BUILD_TUPLE              4
-                      98 LOAD_CONST               9 (<code object select_stmt_raw_sql, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 65>)
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
-                     130 LOAD_CONST              10 (<code object execute_stmt_raw_sql, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 76>)
+                     130 LOAD_CONST              10 (<code object execute_stmt_raw_sql, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 76>)
                      132 MAKE_FUNCTION            4 (annotations)
                      134 STORE_NAME              15 (execute_stmt_raw_sql)
          
           86         136 LOAD_CONST               7 ('sql')
          
           88         138 LOAD_NAME                7 (str)
          
@@ -623,26 +622,26 @@
                      150 LOAD_NAME               12 (dict)
                      152 BINARY_SUBSCR
                      162 LOAD_CONST               8 (None)
                      164 BUILD_TUPLE              2
                      166 BINARY_SUBSCR
          
           86         176 BUILD_TUPLE              6
-                     178 LOAD_CONST              12 (<code object select_stmt_raw_sql_params, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 86>)
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
-                     206 LOAD_CONST              13 (<code object add_record_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 104>)
+                     206 LOAD_CONST              13 (<code object add_record_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 104>)
                      208 MAKE_FUNCTION            4 (annotations)
                      210 STORE_NAME              18 (add_record_sync)
          
          116         212 LOAD_CONST              14 ('model')
          
          117         214 LOAD_NAME               19 (BaseModel)
          
@@ -662,15 +661,15 @@
                      260 LOAD_NAME               11 (List)
                      262 LOAD_NAME               19 (BaseModel)
                      264 BINARY_SUBSCR
                      274 BUILD_TUPLE              2
                      276 BINARY_SUBSCR
          
          116         286 BUILD_TUPLE              6
-                     288 LOAD_CONST              16 (<code object add_records_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 116>)
+                     288 LOAD_CONST              16 (<code object add_records_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 116>)
                      290 MAKE_FUNCTION            4 (annotations)
                      292 STORE_NAME              22 (add_records_sync)
          
          138         294 LOAD_CONST              14 ('model')
          
          139         296 LOAD_NAME               19 (BaseModel)
          
@@ -682,15 +681,15 @@
                      314 BINARY_SUBSCR
          
          138         324 LOAD_CONST               5 ('return')
          
          140         326 LOAD_NAME               14 (bool)
          
          138         328 BUILD_TUPLE              6
-                     330 LOAD_CONST              17 (<code object remove_records_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 138>)
+                     330 LOAD_CONST              17 (<code object remove_records_sync, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 138>)
                      332 MAKE_FUNCTION            4 (annotations)
                      334 STORE_NAME              23 (remove_records_sync)
                      336 LOAD_CONST               8 (None)
                      338 RETURN_VALUE
          consts
             'DBUtils'
             code
@@ -708,15 +707,15 @@
                             18 RETURN_VALUE
                consts
                   None
                names      ('session',)
                varnames   ('cls',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       '__init__'
                firstlineno 53
                lnotab 0x0201
             'session'
             code
                argcount  : 2
                nlocals   : 2
@@ -732,15 +731,15 @@
                             18 RETURN_VALUE
                consts
                   None
                names      ('session',)
                varnames   ('cls', 'session')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'initialize'
                firstlineno 56
                lnotab 0x0201
             'stmt'
             'return'
             code
                argcount  : 1
@@ -776,15 +775,15 @@
                   ''
                   'SELECT json_agg(t) FROM ('
                   ') t'
                names      ('replace', 'text')
                varnames   ('stmt',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'wrap_to_json'
                firstlineno 59
                lnotab 0x02022c01
             'sql'
             None
             code
                argcount  : 2
@@ -858,15 +857,15 @@
                consts
                   None
                   0
                names      ('wrap_to_json', 'session', 'execute', 'fetchone', 'DBAPIError')
                varnames   ('cls', 'sql', 'stmt', 'results', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'select_stmt_raw_sql'
                firstlineno 65
                lnotab 0x020102012a01640104010402060112010cff
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
@@ -923,15 +922,15 @@
                consts
                   None
                   True
                names      ('text', 'session', 'execute', 'DBAPIError')
                varnames   ('cls', 'sql', 'stmt', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'execute_stmt_raw_sql'
                firstlineno 76
                lnotab 0x020102011e013402060112010cff
             'params'
             code
                argcount  : 3
                nlocals   : 6
@@ -1007,15 +1006,15 @@
                   None
                   ('params',)
                   0
                names      ('wrap_to_json', 'session', 'execute', 'fetchone', 'DBAPIError')
                varnames   ('cls', 'sql', 'params', 'stmt', 'results', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'select_stmt_raw_sql_params'
                firstlineno 86
                lnotab 0x020502012a01680204010402060112020cfe
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 5
@@ -1096,15 +1095,15 @@
                consts
                   None
                   ()
                names      ('session', 'add', 'commit', 'DBAPIError', 'rollback')
                varnames   ('cls', 'model', 'kwargs', 'obj', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'add_record_sync'
                firstlineno 104
                lnotab 0x0201020110013401320106011202320114fd
             'model'
             'records'
             code
                argcount  : 3
@@ -1132,15 +1131,15 @@
                119           4 NOP
                
                120           6 BUILD_LIST               0
                              8 STORE_FAST               3 (inserted_ids)
                
                122          10 LOAD_CLOSURE             1 (model)
                             12 BUILD_TUPLE              1
-                            14 LOAD_CONST               1 (<code object <listcomp>, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 122>)
+                            14 LOAD_CONST               1 (<code object <listcomp>, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 122>)
                             16 MAKE_FUNCTION            8 (closure)
                             18 LOAD_FAST                2 (records)
                             20 GET_ITER
                             22 PRECALL                  0
                             26 CALL                     0
                             36 STORE_FAST               4 (records_to_insert)
                
@@ -1155,15 +1154,15 @@
                125          90 LOAD_FAST                0 (cls)
                             92 LOAD_ATTR                0 (session)
                            102 LOAD_METHOD              2 (flush)
                            124 PRECALL                  0
                            128 CALL                     0
                            138 POP_TOP
                
-               127         140 LOAD_CONST               2 (<code object <listcomp>, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py", line 127>)
+               127         140 LOAD_CONST               2 (<code object <listcomp>, file "/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py", line 127>)
                            142 MAKE_FUNCTION            0
                            144 LOAD_FAST                4 (records_to_insert)
                            146 GET_ITER
                            148 PRECALL                  0
                            152 CALL                     0
                            162 STORE_FAST               2 (records)
                
@@ -1259,15 +1258,15 @@
                              >>   30 RETURN_VALUE
                      consts
                         ()
                      names      ()
                      varnames   ('.0', 'record')
                      freevars   ('model',)
                      cellvars   ()
-                     filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+                     filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                      name       '<listcomp>'
                      firstlineno 122
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
@@ -1288,23 +1287,23 @@
                                   50 JUMP_BACKWARD           23 (to 6)
                              >>   52 RETURN_VALUE
                      consts
                      names      ('to_dict',)
                      varnames   ('.0', 'record')
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+                     filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                      name       '<listcomp>'
                      firstlineno 127
                      lnotab 0x
                names      ('session', 'add_all', 'flush', 'append', 'uuid', 'commit', 'DBAPIError', 'rollback')
                varnames   ('cls', 'model', 'records', 'inserted_ids', 'records_to_insert', 'record', 'e')
                freevars   ()
                cellvars   ('model',)
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'add_records_sync'
                firstlineno 116
                lnotab 0x0403020104021c023401320218010801360132010a01120132021afd
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 5
@@ -1398,23 +1397,23 @@
                   False
                   ('synchronize_session',)
                   True
                names      ('session', 'query', 'filter', 'uuid', 'in_', 'delete', 'commit', 'DBAPIError', 'rollback')
                varnames   ('cls', 'model', 'records', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+               filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
                name       'remove_records_sync'
                firstlineno 138
                lnotab 0x020302019e0102ff1203320206011201320214fd
          names      ('__name__', '__module__', '__qualname__', '__init__', 'Session', 'initialize', 'staticmethod', 'str', 'text', 'wrap_to_json', 'Union', 'List', 'dict', 'select_stmt_raw_sql', 'bool', 'execute_stmt_raw_sql', 'select_stmt_raw_sql_params', 'object', 'add_record_sync', 'BaseModel', 'uuid', 'UUID', 'add_records_sync', 'remove_records_sync')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
          name       'DBUtils'
          firstlineno 51
          lnotab
             0x0a0206030c0302010eff0e0102052c0b200a020202fe020302fd02041e
             fc08121c0c020102ff02010eff020234fe0816020102ff020118ff020202
             fe
       'DBUtils'
@@ -1476,21 +1475,21 @@
             0
             True
             ('pool_size', 'max_overflow', 'pool_pre_ping')
          names      ('create_engine', 'DBAPIError')
          varnames   ('url', 'e')
          freevars   ()
          cellvars   ()
-         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+         filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
          name       'get_engine'
          firstlineno 154
          lnotab 0x020102010c0102010201020102fc140612020cfe
-   names      ('tva_utils.db.schemas', 'BaseModel', 'sqlalchemy.exc', 'DBAPIError', 'sqlalchemy.orm.session', 'Session', 'sqlalchemy', 'text', 'inspect', 'create_engine', 'sqlalchemy.engine.base', 'Engine', 'sqlalchemy.orm', 'sessionmaker', 'scoped_session', 'DeclarativeMeta', 'typing', 'List', 'Union', 'Iterator', 'uuid', 'DB', 'DBUtils', 'str', 'get_engine')
+   names      ('tva_utils.postgres.schemas', 'BaseModel', 'sqlalchemy.exc', 'DBAPIError', 'sqlalchemy.orm.session', 'Session', 'sqlalchemy', 'text', 'inspect', 'create_engine', 'sqlalchemy.engine.base', 'Engine', 'sqlalchemy.orm', 'sessionmaker', 'scoped_session', 'DeclarativeMeta', 'typing', 'List', 'Union', 'Iterator', 'uuid', 'DB', 'DBUtils', 'str', 'get_engine', 'db')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/db/postgres.py'
+   filename   '/Users/jsaied/DataCrunch/tva-utils/tva_utils/postgres/postgres.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c020c010c0110010c010c0110010c010802140108031a231a
-      67
+      67100c
```

### Comparing `tva_utils-0.1.1/tva_utils/db/__pycache__/schemas.cpython-311.pyc` & `tva_utils-0.1.2/tva_utils/postgres/__pycache__/schemas.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tva_utils-0.1.1/tva_utils/db/postgres.py` & `tva_utils-0.1.2/tva_utils/postgres/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tva_utils.db.schemas import BaseModel
+from tva_utils.postgres.schemas import BaseModel
 
 from sqlalchemy.exc import DBAPIError
 from sqlalchemy.orm.session import Session
 from sqlalchemy import text, inspect
 from sqlalchemy import create_engine
 from sqlalchemy.engine.base import Engine
 from sqlalchemy.orm import sessionmaker, scoped_session
@@ -18,15 +18,15 @@
         cls.engine: Engine = get_engine(url)
         cls.SessionLocal = sessionmaker(
             autocommit=False, autoflush=False, bind=cls.engine
         )
         cls.inspector = inspect(cls.engine)
         cls.utils = DBUtils()
 
-        cls._create_tables()
+        # cls._create_tables()
 
     def _create_tables(cls, Bases: List[DeclarativeMeta], schemas: List[str]):
 
         for Base, schema in zip(Bases, schemas):
             try:
                 if schema not in cls.inspector.get_schema_names():
                     cls.engine.execute(sqlalchemy.schema.CreateSchema(schema))
@@ -157,8 +157,10 @@
             url,
             pool_size=5,
             max_overflow=0,
             pool_pre_ping=True,
         )
     except DBAPIError as e:
         # logger.info(f"Error in get_engine: {e}")
-        raise e
+        raise e
+    
+db = DB()
```

### Comparing `tva_utils-0.1.1/tva_utils/db/schemas.py` & `tva_utils-0.1.2/tva_utils/postgres/schemas.py`

 * *Files identical despite different names*

