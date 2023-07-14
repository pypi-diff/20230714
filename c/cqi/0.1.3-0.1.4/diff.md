# Comparing `tmp/cqi-0.1.3.tar.gz` & `tmp/cqi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqi-0.1.3.tar", last modified: Tue Jul  4 07:07:36 2023, max compression
+gzip compressed data, was "cqi-0.1.4.tar", last modified: Fri Jul 14 10:35:42 2023, max compression
```

## Comparing `cqi-0.1.3.tar` & `cqi-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-04 07:07:36.728287 cqi-0.1.3/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1072 2023-06-22 07:21:07.000000 cqi-0.1.3/LICENSE
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1615 2023-07-04 07:07:36.728287 cqi-0.1.3/PKG-INFO
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1129 2023-07-04 07:07:09.000000 cqi-0.1.3/README.md
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-04 07:07:36.728287 cqi-0.1.3/cqi/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      166 2023-06-22 09:48:22.000000 cqi-0.1.3/cqi/__init__.py
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-04 07:07:36.728287 cqi-0.1.3/cqi/api/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       45 2023-06-22 09:48:22.000000 cqi-0.1.3/cqi/api/__init__.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    20426 2023-07-03 11:30:33.000000 cqi-0.1.3/cqi/api/client.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    12641 2023-06-22 09:48:22.000000 cqi-0.1.3/cqi/api/specification.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1798 2023-06-30 12:05:11.000000 cqi-0.1.3/cqi/client.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     4963 2023-07-03 10:18:41.000000 cqi-0.1.3/cqi/errors.py
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-04 07:07:36.728287 cqi-0.1.3/cqi/models/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 09:48:22.000000 cqi-0.1.3/cqi/models/__init__.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     7077 2023-07-04 06:47:57.000000 cqi-0.1.3/cqi/models/attributes.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2789 2023-07-04 07:00:23.000000 cqi-0.1.3/cqi/models/corpora.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2374 2023-07-04 06:58:38.000000 cqi-0.1.3/cqi/models/resource.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3911 2023-07-04 06:55:29.000000 cqi-0.1.3/cqi/models/subcorpora.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1077 2023-07-03 10:13:19.000000 cqi-0.1.3/cqi/status.py
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      145 2023-07-04 07:01:59.000000 cqi-0.1.3/cqi/version.py
-drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-04 07:07:36.728287 cqi-0.1.3/cqi.egg-info/
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1615 2023-07-04 07:07:36.000000 cqi-0.1.3/cqi.egg-info/PKG-INFO
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      388 2023-07-04 07:07:36.000000 cqi-0.1.3/cqi.egg-info/SOURCES.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        1 2023-07-04 07:07:36.000000 cqi-0.1.3/cqi.egg-info/dependency_links.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        4 2023-07-04 07:07:36.000000 cqi-0.1.3/cqi.egg-info/top_level.txt
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       38 2023-07-04 07:07:36.728287 cqi-0.1.3/setup.cfg
--rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      781 2023-06-22 07:21:07.000000 cqi-0.1.3/setup.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-14 10:35:42.620060 cqi-0.1.4/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1072 2023-06-22 07:21:07.000000 cqi-0.1.4/LICENSE
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1498 2023-07-14 10:35:42.620060 cqi-0.1.4/PKG-INFO
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1012 2023-07-14 10:29:35.000000 cqi-0.1.4/README.md
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-14 10:35:42.610060 cqi-0.1.4/cqi/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      166 2023-06-22 09:48:22.000000 cqi-0.1.4/cqi/__init__.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-14 10:35:42.620060 cqi-0.1.4/cqi/api/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       45 2023-06-22 09:48:22.000000 cqi-0.1.4/cqi/api/__init__.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    20355 2023-07-14 10:23:10.000000 cqi-0.1.4/cqi/api/client.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)    12641 2023-06-22 09:48:22.000000 cqi-0.1.4/cqi/api/specification.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1826 2023-07-14 10:26:07.000000 cqi-0.1.4/cqi/client.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     5141 2023-07-14 10:03:47.000000 cqi-0.1.4/cqi/errors.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-14 10:35:42.620060 cqi-0.1.4/cqi/models/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        0 2023-06-22 09:48:22.000000 cqi-0.1.4/cqi/models/__init__.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     7077 2023-07-13 06:38:32.000000 cqi-0.1.4/cqi/models/attributes.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2789 2023-07-04 07:00:23.000000 cqi-0.1.4/cqi/models/corpora.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     2374 2023-07-04 06:58:38.000000 cqi-0.1.4/cqi/models/resource.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     3911 2023-07-04 06:55:29.000000 cqi-0.1.4/cqi/models/subcorpora.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1180 2023-07-14 10:03:17.000000 cqi-0.1.4/cqi/status.py
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      145 2023-07-14 10:29:43.000000 cqi-0.1.4/cqi/version.py
+drwxr-xr-x   0 pjentsch  (1000) pjentsch  (1000)        0 2023-07-14 10:35:42.610060 cqi-0.1.4/cqi.egg-info/
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)     1498 2023-07-14 10:35:42.000000 cqi-0.1.4/cqi.egg-info/PKG-INFO
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      388 2023-07-14 10:35:42.000000 cqi-0.1.4/cqi.egg-info/SOURCES.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        1 2023-07-14 10:35:42.000000 cqi-0.1.4/cqi.egg-info/dependency_links.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)        4 2023-07-14 10:35:42.000000 cqi-0.1.4/cqi.egg-info/top_level.txt
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)       38 2023-07-14 10:35:42.620060 cqi-0.1.4/setup.cfg
+-rw-r--r--   0 pjentsch  (1000) pjentsch  (1000)      781 2023-06-22 07:21:07.000000 cqi-0.1.4/setup.py
```

### Comparing `cqi-0.1.3/LICENSE` & `cqi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cqi-0.1.3/PKG-INFO` & `cqi-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqi
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for the IMS Open Corpus Workbench (CWB) corpus query interface (CQi) API.
 Home-page: https://github.com/Pevtrick/cqi-py
 Author: Patrick Jentsch
 Author-email: patrickjentsch@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,18 +24,15 @@
 pip install cqi
 ```
 
 ## Version compatibility
 
 | Package version | Protocol version |
 |-----------------|------------------|
-| 0.1.0           | 0.1              |
-| 0.1.1           | 0.1              |
-| 0.1.2           | 0.1              |
-| 0.1.3           | 0.1              |
+| 0.1.0 - 0.1.4   | 0.1              |
 
 ## Usage
 
 ```python
 import cqi
```

### Comparing `cqi-0.1.3/README.md` & `cqi-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,15 @@
 pip install cqi
 ```
 
 ## Version compatibility
 
 | Package version | Protocol version |
 |-----------------|------------------|
-| 0.1.0           | 0.1              |
-| 0.1.1           | 0.1              |
-| 0.1.2           | 0.1              |
-| 0.1.3           | 0.1              |
+| 0.1.0 - 0.1.4   | 0.1              |
 
 ## Usage
 
 ```python
 import cqi
```

### Comparing `cqi-0.1.3/cqi/api/client.py` & `cqi-0.1.4/cqi/api/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import List, Tuple
+from typing import Callable, Dict, List, Optional, Tuple
 import socket
 import struct
-import time
 from . import specification
 from .. import errors
 from .. import status
 
 
 class APIClient:
     '''
@@ -23,45 +22,47 @@
     259  # CQI_STATUS_BYE_OK
 
     Attributes:
     host (str): URL to the CQP server. For example,
         ``cqpserver.localhost`` or ``127.0.0.1``.
     port (int): Port the CQP server listens on. Default: ``4877``
     socket (socket.socket): Socket for communicating with a CQP server.
-    timeout (int): Default timeout for API calls, in seconds. Default: ``60``
+    timeout (float): Default timeout for API calls, in seconds.
+        Default: ``60.0``
     version (str): The version of the CQi protocol to use. Default: ``0.1``
     '''
 
     def __init__(
         self,
         host: str,
         port: int = 4877,
-        timeout: int = 60,
+        timeout: Optional[float] = 60.0,
         version: str = '0.1'
     ):
         self.host: str = host
         self.port: int = port
         self.socket: socket.socket = socket.socket()
-        self.timeout: int = timeout
+        self.timeout: Optional[float] = timeout
         self.version: str = version
+        self.socket.settimeout(self.timeout)
 
     def ctrl_connect(
         self,
         username: str,
         password: str
     ) -> status.StatusConnectOk:
         self.socket.connect((self.host, self.port))
         self.__send_WORD(specification.CTRL_CONNECT)
         self.__send_STRING(username)
         self.__send_STRING(password)
         return self.__recv_response()
 
     def ctrl_bye(self) -> status.StatusByeOk:
         self.__send_WORD(specification.CTRL_BYE)
-        response = self.__recv_response()
+        response: status.StatusByeOk = self.__recv_response()
         self.socket.close()
         return response
 
     def ctrl_user_abort(self):
         self.__send_WORD(specification.CTRL_USER_ABORT)
 
     def ctrl_ping(self) -> status.StatusPingOk:
@@ -161,15 +162,21 @@
         valid lexicon IDs range from 0 .. (lexicon_size - 1)
         '''
         self.__send_WORD(specification.CL_LEXICON_SIZE)
         self.__send_STRING(attribute)
         return self.__recv_response()
 
     def cl_drop_attribute(self, attribute: str) -> status.StatusOk:
-        ''' unload attribute from memory '''
+        '''
+        unload attribute from memory
+
+        Note: Not implemented on the server side:
+              https://sourceforge.net/p/cwb/code/HEAD/tree/cwb/trunk/CQi/cqpserver.c#l356
+        '''
+        raise NotImplementedError
         self.__send_WORD(specification.CL_DROP_ATTRIBUTE)
         self.__send_STRING(attribute)
         return self.__recv_response()
 
     '''
     ' NOTE: simple (scalar) mappings are applied to lists (the returned list
     '       has exactly the same length as the list passed as an argument)
@@ -307,15 +314,20 @@
         returns start and end corpus positions of structure region <struc>
         '''
         self.__send_WORD(specification.CL_STRUC2CPOS)
         self.__send_STRING(attribute)
         self.__send_INT(struc)
         return self.__recv_response()
 
-    def cl_alg2cpos(self, attribute: str, alg: int) -> Tuple[int, int, int, int]:
+    def cl_alg2cpos(
+        self,
+        attribute:
+        str,
+        alg: int
+    ) -> Tuple[int, int, int, int]:
         ''' returns (src_start, src_end, target_start, target_end) '''
         self.__send_WORD(specification.CL_ALG2CPOS)
         self.__send_STRING(attribute)
         self.__send_INT(alg)
         return self.__recv_response()
 
     def cqp_query(self,
@@ -424,103 +436,80 @@
         self.__send_BYTE(field1)
         self.__send_STRING(attribute1)
         self.__send_BYTE(field2)
         self.__send_STRING(attribute2)
         return self.__recv_response()
 
     def __recv_response(self):
-        byte_data = self.__recv_WORD()
-        response_type = byte_data >> 8
+        byte_data: int = self.__recv_WORD()
+        response_type: int = byte_data >> 8
         if response_type == specification.DATA:
-            return self.__recv_DATA(byte_data)
+            try:
+                return self.__recv_DATA_method_lookup[byte_data](self)
+            except KeyError:
+                raise errors.CQiException(f'Unknown data type: {byte_data}')
         elif response_type == specification.STATUS:
-            return status.lookup[byte_data]()
+            try:
+                return status.lookup[byte_data]()
+            except KeyError:
+                raise errors.CQiException(f'Unknown status code: {byte_data}')
+        elif response_type == specification.ERROR:
+            try:
+                raise errors.lookup[byte_data]()
+            except KeyError:
+                raise errors.CQiException(f'Unknown error code: {byte_data}')
         else:
-            raise errors.lookup.get(byte_data, errors.CQiException)()
-
-    def __recv_DATA(self, data_type):
-        if data_type == specification.DATA_BYTE:
-            return self.__recv_DATA_BYTE()
-        elif data_type == specification.DATA_BOOL:
-            return self.__recv_DATA_BOOL()
-        elif data_type == specification.DATA_INT:
-            return self.__recv_DATA_INT()
-        elif data_type == specification.DATA_STRING:
-            return self.__recv_DATA_STRING()
-        elif data_type == specification.DATA_BYTE_LIST:
-            return self.__recv_DATA_BYTE_LIST()
-        elif data_type == specification.DATA_BOOL_LIST:
-            return self.__recv_DATA_BOOL_LIST()
-        elif data_type == specification.DATA_INT_LIST:
-            return self.__recv_DATA_INT_LIST()
-        elif data_type == specification.DATA_STRING_LIST:
-            return self.__recv_DATA_STRING_LIST()
-        elif data_type == specification.DATA_INT_INT:
-            return self.__recv_DATA_INT_INT()
-        elif data_type == specification.DATA_INT_INT_INT_INT:
-            return self.__recv_DATA_INT_INT_INT_INT()
-        elif data_type == specification.DATA_INT_TABLE:
-            return self.__recv_DATA_INT_TABLE()
-        else:
-            raise errors.CQiException(f'Unknown data type: {data_type}')
-
-    def __recv_wrapper(self, bufsize: int) -> bytes:
-        start_time = time.time()
-        while time.time() - start_time < self.timeout:
-            # Check if the server already sent over the desired number of bytes
-            if len(self.socket.recv(bufsize, socket.MSG_PEEK)) == bufsize:
-                return self.socket.recv(bufsize)
-            time.sleep(0.05)
-        else:
-            raise errors.CQiException('Timeout: Not enough bytes')
+            raise errors.CQiException(
+                f'Unknown response type: {response_type}'
+            )
 
     def __recv_DATA_BYTE(self) -> int:
-        byte_data = self.__recv_wrapper(1)
+        byte_data: bytes = self.socket.recv(1, socket.MSG_WAITALL)
         return struct.unpack('!B', byte_data)[0]
 
     def __recv_DATA_BOOL(self) -> bool:
-        byte_data = self.__recv_wrapper(1)
+        byte_data: bytes = self.socket.recv(1, socket.MSG_WAITALL)
         return struct.unpack('!?', byte_data)[0]
 
     def __recv_DATA_INT(self) -> int:
-        byte_data = self.__recv_wrapper(4)
+        byte_data: bytes = self.socket.recv(4, socket.MSG_WAITALL)
         return struct.unpack('!i', byte_data)[0]
 
     def __recv_DATA_STRING(self) -> str:
-        n = self.__recv_WORD()
-        byte_data = self.__recv_wrapper(n)
+        n: int = self.__recv_WORD()
+        byte_data: bytes = self.socket.recv(n, socket.MSG_WAITALL)
         return struct.unpack(f'!{n}s', byte_data)[0].decode()
 
     def __recv_DATA_BYTE_LIST(self) -> List[int]:
-        data = []
-        n = self.__recv_DATA_INT()
+        data: List[int] = []
+        n: int = self.__recv_DATA_INT()
         while n > 0:
             data.append(self.__recv_DATA_BYTE())
             n -= 1
         return data
 
     def __recv_DATA_BOOL_LIST(self) -> List[bool]:
-        data = []
-        n = self.__recv_DATA_INT()
+        data: List[bool] = []
+        n: int = self.__recv_DATA_INT()
         while n > 0:
             data.append(self.__recv_DATA_BOOL())
             n -= 1
         return data
 
     def __recv_DATA_INT_LIST(self) -> List[int]:
-        data = []
-        n = self.__recv_DATA_INT()
+        data: List[int] = []
+        n: int = self.__recv_DATA_INT()
         while n > 0:
             data.append(self.__recv_DATA_INT())
             n -= 1
         return data
 
     def __recv_DATA_STRING_LIST(self) -> List[str]:
-        data = []
-        n = self.__recv_DATA_INT()
+        data: List[str] = []
+        n: int = self.__recv_DATA_INT()
         while n > 0:
             data.append(self.__recv_DATA_STRING())
             n -= 1
         return data
 
     def __recv_DATA_INT_INT(self) -> Tuple[int, int]:
         return (self.__recv_DATA_INT(), self.__recv_DATA_INT())
@@ -530,54 +519,68 @@
             self.__recv_DATA_INT(),
             self.__recv_DATA_INT(),
             self.__recv_DATA_INT(),
             self.__recv_DATA_INT()
         )
 
     def __recv_DATA_INT_TABLE(self) -> List[List[int]]:
-        rows = self.__recv_DATA_INT()
-        columns = self.__recv_DATA_INT()
-        data = []
+        rows: int = self.__recv_DATA_INT()
+        columns: int = self.__recv_DATA_INT()
+        data: List[List[int]] = []
         for i in range(0, rows):
-            row = []
+            row: List[int] = []
             for j in range(0, columns):
                 row.append(self.__recv_DATA_INT())
             data.append(row)
         return data
 
+    __recv_DATA_method_lookup: Dict[int, Callable] = {
+        769: __recv_DATA_BYTE,
+        770: __recv_DATA_BOOL,
+        771: __recv_DATA_INT,
+        772: __recv_DATA_STRING,
+        773: __recv_DATA_BYTE_LIST,
+        774: __recv_DATA_BOOL_LIST,
+        775: __recv_DATA_INT_LIST,
+        776: __recv_DATA_STRING_LIST,
+        777: __recv_DATA_INT_INT,
+        778: __recv_DATA_INT_INT_INT_INT,
+        779: __recv_DATA_INT_TABLE
+    }
+
     def __recv_WORD(self) -> int:
-        byte_data = self.__recv_wrapper(2)
+        byte_data: bytes = self.socket.recv(2, socket.MSG_WAITALL)
         return struct.unpack('!H', byte_data)[0]
 
     def __send_BYTE(self, byte_data: int):
-        data = struct.pack('!B', byte_data)
+        data: bytes = struct.pack('!B', byte_data)
         self.socket.sendall(data)
 
     def __send_BOOL(self, bool_data: bool):
-        data = struct.pack('!?', bool_data)
+        data: bytes = struct.pack('!?', bool_data)
         self.socket.sendall(data)
 
     def __send_INT(self, int_data: int):
-        data = struct.pack('!i', int_data)
+        data: bytes = struct.pack('!i', int_data)
         self.socket.sendall(data)
 
     def __send_STRING(self, string_data: str):
-        encoded_string_data = string_data.encode('utf-8')
-        n = len(encoded_string_data)
-        data = struct.pack(f'!H{n}s', n, encoded_string_data)
+        encoded_string_data: bytes = string_data.encode('utf-8')
+        n: int = len(encoded_string_data)
+        data: bytes = struct.pack(f'!H{n}s', n, encoded_string_data)
         self.socket.sendall(data)
 
     def __send_INT_LIST(self, int_list_data: List[int]):
-        n = len(int_list_data)
+        n: int = len(int_list_data)
         self.__send_INT(n)
         for int_data in int_list_data:
             self.__send_INT(int_data)
 
     def __send_STRING_LIST(self, string_list_data: List[str]):
-        n = len(string_list_data)
+        n: int = len(string_list_data)
         self.__send_INT(n)
         for string_data in string_list_data:
             self.__send_STRING(string_data)
 
     def __send_WORD(self, word_data: int):
-        data = struct.pack('!H', word_data)
+        data: bytes = struct.pack('!H', word_data)
         self.socket.sendall(data)
```

### Comparing `cqi-0.1.3/cqi/api/specification.py` & `cqi-0.1.4/cqi/api/specification.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.3/cqi/client.py` & `cqi-0.1.4/cqi/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING
+from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from .status import StatusByeOk, StatusConnectOk, StatusPingOk
 from .api import APIClient
 from .models.corpora import CorpusCollection
 
 
 
@@ -24,25 +24,25 @@
     api (APIClient): An API client pointing to the specified CQP server.
     '''
 
     def __init__(
         self,
         host: str,
         port: int = 4877,
-        timeout: int = 60,
+        timeout: Optional[float] = 60.0,
         version: str = '0.1'
     ):
         '''
         CQiClient constructor
 
         Args:
         host (str): URL to the CQP server. For example,
             ``cqpserver.localhost`` or ``127.0.0.1``.
         port (int): Port the CQP server listens on. Default: ``4877``
-        timeout (int): Default timeout for API calls, in seconds. Default: ``60``
+        timeout (float): Default timeout for API calls, in seconds. Default: ``60.0``
         version (str): The version of the CQi protocol to use. Default: ``0.1``
         '''
         self.api: APIClient = APIClient(
             host,
             port=port,
             timeout=timeout,
             version=version
```

### Comparing `cqi-0.1.3/cqi/errors.py` & `cqi-0.1.4/cqi/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,143 +1,143 @@
+from typing import Dict, Optional, Type
 from .api import specification
 
 
 class CQiException(Exception):
     '''
     A base class from which all other exceptions inherit.
     If you want to catch all errors that the CQi package might raise,
     catch this base exception.
     '''
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = None
-        self.description = None
+        self.code: Optional[int] = None
+        self.description: Optional[str] = None
 
 
 class Error(CQiException):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.ERROR
+        self.code: int = specification.ERROR
 
 
 class ErrorGeneralError(Error):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.ERROR_GENERAL_ERROR
+        self.code: int = specification.ERROR_GENERAL_ERROR
 
 
 class ErrorConnectRefused(Error):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.ERROR_CONNECT_REFUSED
+        self.code: int = specification.ERROR_CONNECT_REFUSED
 
 
 class ErrorUserAbort(Error):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.ERROR_USER_ABORT
+        self.code: int = specification.ERROR_USER_ABORT
 
 
 class ErrorSyntaxError(Error):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.ERROR_SYNTAX_ERROR
+        self.code: int = specification.ERROR_SYNTAX_ERROR
 
 
 class CLError(CQiException):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.CL_ERROR
+        self.code: int = specification.CL_ERROR
 
 
 class CLErrorNoSuchAttribute(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.CL_ERROR_NO_SUCH_ATTRIBUTE
-        self.description = 'CQi server couldn\'t open attribute'
+        self.code: int = specification.CL_ERROR_NO_SUCH_ATTRIBUTE
+        self.description: str = "CQi server couldn't open attribute"
 
 
 class CLErrorWrongAttributeType(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.CL_ERROR_WRONG_ATTRIBUTE_TYPE
+        self.code: int = specification.CL_ERROR_WRONG_ATTRIBUTE_TYPE
 
 
 class CLErrorOutOfRange(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.CL_ERROR_OUT_OF_RANGE
+        self.code: int = specification.CL_ERROR_OUT_OF_RANGE
 
 
 class CLErrorRegex(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.CL_ERROR_REGEX
+        self.code: int = specification.CL_ERROR_REGEX
 
 
 class CLErrorCorpusAccess(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.CL_ERROR_CORPUS_ACCESS
-        self.description = ''
+        self.code: int = specification.CL_ERROR_CORPUS_ACCESS
 
 
 class CLErrorOutOfMemory(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.CL_ERROR_OUT_OF_MEMORY
-        self.description = (
+        self.code: int = specification.CL_ERROR_OUT_OF_MEMORY
+        self.description: str = (
             'CQi server has run out of memory; try discarding some other '
             'corpora and/or subcorpora'
         )
 
 
 class CLErrorInternal(CLError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.CL_ERROR_INTERNAL
-        self.description = (
-            'The classical \'please contact technical support\' error'
+        self.code: int = specification.CL_ERROR_INTERNAL
+        self.description: str = (
+            "The classical 'please contact technical support' error"
         )
 
 
 class CQPError(CQiException):
     # CQP error messages yet to be defined
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.CQP_ERROR
+        self.code: int = specification.CQP_ERROR
 
 
 class CQPErrorGeneral(CQPError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.CQP_ERROR_GENERAL
+        self.code: int = specification.CQP_ERROR_GENERAL
 
 
 class CQPErrorNoSuchCorpus(CQPError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.CQP_ERROR_NO_SUCH_CORPUS
+        self.code: int = specification.CQP_ERROR_NO_SUCH_CORPUS
 
 
 class CQPErrorInvalidField(CQPError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.CQP_ERROR_INVALID_FIELD
+        self.code: int = specification.CQP_ERROR_INVALID_FIELD
 
 
 class CQPErrorOutOfRange(CQPError):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.code = specification.CQP_ERROR_OUT_OF_RANGE
-        self.description = 'A number is out of range'
+        self.code: int = specification.CQP_ERROR_OUT_OF_RANGE
+        self.description: str = 'A number is out of range'
 
 
-lookup = {
+lookup: Dict[int, Type[CQiException]] = {
     specification.ERROR: Error,
     specification.ERROR_GENERAL_ERROR: ErrorGeneralError,
     specification.ERROR_CONNECT_REFUSED: ErrorConnectRefused,
     specification.ERROR_USER_ABORT: ErrorUserAbort,
     specification.ERROR_SYNTAX_ERROR: ErrorSyntaxError,
     specification.CL_ERROR: CLError,
     specification.CL_ERROR_NO_SUCH_ATTRIBUTE: CLErrorNoSuchAttribute,
```

### Comparing `cqi-0.1.3/cqi/models/attributes.py` & `cqi-0.1.4/cqi/models/attributes.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.3/cqi/models/corpora.py` & `cqi-0.1.4/cqi/models/corpora.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.3/cqi/models/resource.py` & `cqi-0.1.4/cqi/models/resource.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.3/cqi/models/subcorpora.py` & `cqi-0.1.4/cqi/models/subcorpora.py`

 * *Files identical despite different names*

### Comparing `cqi-0.1.3/cqi.egg-info/PKG-INFO` & `cqi-0.1.4/cqi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqi
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for the IMS Open Corpus Workbench (CWB) corpus query interface (CQi) API.
 Home-page: https://github.com/Pevtrick/cqi-py
 Author: Patrick Jentsch
 Author-email: patrickjentsch@gmx.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,18 +24,15 @@
 pip install cqi
 ```
 
 ## Version compatibility
 
 | Package version | Protocol version |
 |-----------------|------------------|
-| 0.1.0           | 0.1              |
-| 0.1.1           | 0.1              |
-| 0.1.2           | 0.1              |
-| 0.1.3           | 0.1              |
+| 0.1.0 - 0.1.4   | 0.1              |
 
 ## Usage
 
 ```python
 import cqi
```

### Comparing `cqi-0.1.3/setup.py` & `cqi-0.1.4/setup.py`

 * *Files identical despite different names*

