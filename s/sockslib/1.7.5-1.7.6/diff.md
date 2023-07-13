# Comparing `tmp/sockslib-1.7.5.tar.gz` & `tmp/sockslib-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockslib-1.7.5.tar", last modified: Thu Jul 13 16:24:16 2023, max compression
+gzip compressed data, was "sockslib-1.7.6.tar", last modified: Thu Jul 13 22:26:13 2023, max compression
```

## Comparing `sockslib-1.7.5.tar` & `sockslib-1.7.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 16:24:16.554312 sockslib-1.7.5/
--rw-r--r--   0 coyote     (501) staff       (20)     1076 2023-07-13 14:22:00.000000 sockslib-1.7.5/LICENSE
--rw-r--r--   0 coyote     (501) staff       (20)       19 2023-07-13 14:22:00.000000 sockslib-1.7.5/MANIFEST.in
--rw-r--r--   0 coyote     (501) staff       (20)     7518 2023-07-13 16:24:16.553825 sockslib-1.7.5/PKG-INFO
--rw-r--r--   0 coyote     (501) staff       (20)     7106 2023-07-13 16:07:19.000000 sockslib-1.7.5/README.md
--rw-r--r--   0 coyote     (501) staff       (20)       38 2023-07-13 16:24:16.554466 sockslib-1.7.5/setup.cfg
--rw-r--r--   0 coyote     (501) staff       (20)      816 2023-07-13 16:18:09.000000 sockslib-1.7.5/setup.py
-drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 16:24:16.548996 sockslib-1.7.5/sockslib/
--rw-r--r--   0 coyote     (501) staff       (20)       85 2023-07-13 16:17:57.000000 sockslib-1.7.5/sockslib/__init__.py
--rw-r--r--   0 coyote     (501) staff       (20)    13617 2023-07-13 16:14:14.000000 sockslib-1.7.5/sockslib/socks.py
--rw-r--r--   0 coyote     (501) staff       (20)      948 2023-07-13 14:22:00.000000 sockslib-1.7.5/sockslib/socksauth.py
-drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 16:24:16.551027 sockslib-1.7.5/sockslib.egg-info/
--rw-r--r--   0 coyote     (501) staff       (20)     7518 2023-07-13 16:24:16.000000 sockslib-1.7.5/sockslib.egg-info/PKG-INFO
--rw-r--r--   0 coyote     (501) staff       (20)      272 2023-07-13 16:24:16.000000 sockslib-1.7.5/sockslib.egg-info/SOURCES.txt
--rw-r--r--   0 coyote     (501) staff       (20)        1 2023-07-13 16:24:16.000000 sockslib-1.7.5/sockslib.egg-info/dependency_links.txt
--rw-r--r--   0 coyote     (501) staff       (20)        9 2023-07-13 16:24:16.000000 sockslib-1.7.5/sockslib.egg-info/top_level.txt
-drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 16:24:16.552678 sockslib-1.7.5/tests/
--rw-r--r--   0 coyote     (501) staff       (20)     2999 2023-07-13 16:07:39.000000 sockslib-1.7.5/tests/test_socks.py
--rw-r--r--   0 coyote     (501) staff       (20)     1337 2023-07-13 15:09:21.000000 sockslib-1.7.5/tests/test_socks_ipv6.py
+drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 22:26:13.790996 sockslib-1.7.6/
+-rw-r--r--   0 coyote     (501) staff       (20)     1076 2023-07-13 22:07:08.000000 sockslib-1.7.6/LICENSE
+-rw-r--r--   0 coyote     (501) staff       (20)       19 2023-07-13 22:07:07.000000 sockslib-1.7.6/MANIFEST.in
+-rw-r--r--   0 coyote     (501) staff       (20)     7778 2023-07-13 22:26:13.790644 sockslib-1.7.6/PKG-INFO
+-rw-r--r--   0 coyote     (501) staff       (20)     7366 2023-07-13 22:22:37.000000 sockslib-1.7.6/README.md
+-rw-r--r--   0 coyote     (501) staff       (20)       38 2023-07-13 22:26:13.791083 sockslib-1.7.6/setup.cfg
+-rw-r--r--   0 coyote     (501) staff       (20)      816 2023-07-13 22:23:55.000000 sockslib-1.7.6/setup.py
+drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 22:26:13.786911 sockslib-1.7.6/sockslib/
+-rw-r--r--   0 coyote     (501) staff       (20)       85 2023-07-13 22:24:09.000000 sockslib-1.7.6/sockslib/__init__.py
+-rw-r--r--   0 coyote     (501) staff       (20)    13570 2023-07-13 22:14:45.000000 sockslib-1.7.6/sockslib/socks.py
+-rw-r--r--   0 coyote     (501) staff       (20)      948 2023-07-13 22:07:08.000000 sockslib-1.7.6/sockslib/socksauth.py
+drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 22:26:13.788678 sockslib-1.7.6/sockslib.egg-info/
+-rw-r--r--   0 coyote     (501) staff       (20)     7778 2023-07-13 22:26:13.000000 sockslib-1.7.6/sockslib.egg-info/PKG-INFO
+-rw-r--r--   0 coyote     (501) staff       (20)      272 2023-07-13 22:26:13.000000 sockslib-1.7.6/sockslib.egg-info/SOURCES.txt
+-rw-r--r--   0 coyote     (501) staff       (20)        1 2023-07-13 22:26:13.000000 sockslib-1.7.6/sockslib.egg-info/dependency_links.txt
+-rw-r--r--   0 coyote     (501) staff       (20)        9 2023-07-13 22:26:13.000000 sockslib-1.7.6/sockslib.egg-info/top_level.txt
+drwxr-xr-x   0 coyote     (501) staff       (20)        0 2023-07-13 22:26:13.789867 sockslib-1.7.6/tests/
+-rw-r--r--   0 coyote     (501) staff       (20)     2999 2023-07-13 22:07:08.000000 sockslib-1.7.6/tests/test_socks.py
+-rw-r--r--   0 coyote     (501) staff       (20)     1337 2023-07-13 22:07:33.000000 sockslib-1.7.6/tests/test_socks_ipv6.py
```

### Comparing `sockslib-1.7.5/LICENSE` & `sockslib-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sockslib-1.7.5/PKG-INFO` & `sockslib-1.7.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockslib
-Version: 1.7.5
+Version: 1.7.6
 Summary: Simple Socks proxy library
 Home-page: https://github.com/woo200/sockslib
 Author: Jack Woo
 Author-email: woo.jack.06@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -64,15 +64,15 @@
 
 #### Set a default proxy
 Default proxies can be useful for situations when other libraries use sockets to communicate and you want to force that library to use a proxy instead of a direct connection
 ```python
 sockslib.set_default_proxy(
 	('127.0.0.1', 0),      # Ip, Port
 	sockslib.Socks.SOCKS5, # SOCKS5/SOCKS4, (Optional) (Default SOCKS5)
-    socket.AF_INET,        # Default protocol (AF_INET, AF_INET6)
+	socket.AF_INET,        # Default protocol (AF_INET, AF_INET6)
 	authentication         # Array of authentication methods (Optional) (Default NoAuth)
 )
 ```
 
 #### URLLib Proxied
 ```python
 import urllib.request
@@ -84,15 +84,15 @@
 socket.socket = sockslib.SocksSocket # Make the default socket object a SocksSocket
 
 html = urllib.request.urlopen('https://myexternalip.com/raw').read() # Request the page
 print(html)
 ```
 
 ### IPv6
-To connect to a proxy server via ipv6, you must explicitly specify the protocol by passing the `ip_protocol` parameter to the SocksSocket constructor. 
+To connect to a proxy server via ipv6, you must explicitly specify the protocol by passing the `ip_protocol` parameter to the SocksSocket constructor, OR by using the 3rd option of [set_default_proxy](#set-a-default-proxy).
 Here is an example of connecting to a remote IPv6 proxy:
 ```python
 import sockslib
 import socket # import socket for the protocol specifiers 
 
 with sockslib.SocksSocket(ip_protocol=socket.AF_INET6) as sock:
     sock.set_proxy(('::1', 9050)) # Set proxy
@@ -125,14 +125,15 @@
 
 with sockslib.SocksSocket(udp=True) as sock:
     sock.set_proxy(('127.0.0.1', 9050)) # Set proxy
 
     sock.initudp() # Connect to Server and bind a UDP port for communication
     sock.sendto(b"Hello, World", ("0.0.0.0", 12000)) # Send "Hello, World" to 0.0.0.0:12000 over UDP
 ```
+Due to the nature of UDP in the SOCKS5 protocol, it is reccomended to use the context manager, as the remote proxy server will not drop the UDP associate request until the socket is closed. 
 
 ### Using other authentication methods
 To use more authentication methods like User/Pass auth, you pass an array of authentication methods to the third parameter of `set_proxy` (Don't neglect to set the second parameter to the proxy type!)
 ```python
 import sockslib
 
 with sockslib.SocksSocket() as sock:
```

### Comparing `sockslib-1.7.5/README.md` & `sockslib-1.7.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 #### Set a default proxy
 Default proxies can be useful for situations when other libraries use sockets to communicate and you want to force that library to use a proxy instead of a direct connection
 ```python
 sockslib.set_default_proxy(
 	('127.0.0.1', 0),      # Ip, Port
 	sockslib.Socks.SOCKS5, # SOCKS5/SOCKS4, (Optional) (Default SOCKS5)
-    socket.AF_INET,        # Default protocol (AF_INET, AF_INET6)
+	socket.AF_INET,        # Default protocol (AF_INET, AF_INET6)
 	authentication         # Array of authentication methods (Optional) (Default NoAuth)
 )
 ```
 
 #### URLLib Proxied
 ```python
 import urllib.request
@@ -70,15 +70,15 @@
 socket.socket = sockslib.SocksSocket # Make the default socket object a SocksSocket
 
 html = urllib.request.urlopen('https://myexternalip.com/raw').read() # Request the page
 print(html)
 ```
 
 ### IPv6
-To connect to a proxy server via ipv6, you must explicitly specify the protocol by passing the `ip_protocol` parameter to the SocksSocket constructor. 
+To connect to a proxy server via ipv6, you must explicitly specify the protocol by passing the `ip_protocol` parameter to the SocksSocket constructor, OR by using the 3rd option of [set_default_proxy](#set-a-default-proxy).
 Here is an example of connecting to a remote IPv6 proxy:
 ```python
 import sockslib
 import socket # import socket for the protocol specifiers 
 
 with sockslib.SocksSocket(ip_protocol=socket.AF_INET6) as sock:
     sock.set_proxy(('::1', 9050)) # Set proxy
@@ -111,14 +111,15 @@
 
 with sockslib.SocksSocket(udp=True) as sock:
     sock.set_proxy(('127.0.0.1', 9050)) # Set proxy
 
     sock.initudp() # Connect to Server and bind a UDP port for communication
     sock.sendto(b"Hello, World", ("0.0.0.0", 12000)) # Send "Hello, World" to 0.0.0.0:12000 over UDP
 ```
+Due to the nature of UDP in the SOCKS5 protocol, it is reccomended to use the context manager, as the remote proxy server will not drop the UDP associate request until the socket is closed. 
 
 ### Using other authentication methods
 To use more authentication methods like User/Pass auth, you pass an array of authentication methods to the third parameter of `set_proxy` (Don't neglect to set the second parameter to the proxy type!)
 ```python
 import sockslib
 
 with sockslib.SocksSocket() as sock:
```

### Comparing `sockslib-1.7.5/setup.py` & `sockslib-1.7.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="sockslib",
-    version="1.7.5",
+    version="1.7.6",
     description="Simple Socks proxy library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/woo200/sockslib",
     author="Jack Woo",
     author_email="woo.jack.06@gmail.com",
     license="MIT",
```

### Comparing `sockslib-1.7.5/sockslib/socks.py` & `sockslib-1.7.6/sockslib/socks.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,17 +332,14 @@
             raise SocksException(f"Server denied connection request with response: {SocksErrors.request_denied(status)}")
 
         bndaddr = Socks5Address.readAddr(self)
         bndport, = struct.unpack("!H", self.recv(2))
 
         self.udpbind = (bndaddr, bndport)
 
-        if self.udp:
-            self.close()
-
         if self.debug:
             print(f"[DEBUG/INFO] (SOCKS5) [{'UDP' if self.udp else 'TCP'}] Server accepted connection. (*{bndaddr}:{bndport})")
 
     def __handshake_4(self, hp, auth=[Socks4Ident("")]):
         if self.udp:
             raise SocksException("Cannot use UDP port over SOCKS4")
```

### Comparing `sockslib-1.7.5/sockslib/socksauth.py` & `sockslib-1.7.6/sockslib/socksauth.py`

 * *Files identical despite different names*

### Comparing `sockslib-1.7.5/sockslib.egg-info/PKG-INFO` & `sockslib-1.7.6/sockslib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockslib
-Version: 1.7.5
+Version: 1.7.6
 Summary: Simple Socks proxy library
 Home-page: https://github.com/woo200/sockslib
 Author: Jack Woo
 Author-email: woo.jack.06@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -64,15 +64,15 @@
 
 #### Set a default proxy
 Default proxies can be useful for situations when other libraries use sockets to communicate and you want to force that library to use a proxy instead of a direct connection
 ```python
 sockslib.set_default_proxy(
 	('127.0.0.1', 0),      # Ip, Port
 	sockslib.Socks.SOCKS5, # SOCKS5/SOCKS4, (Optional) (Default SOCKS5)
-    socket.AF_INET,        # Default protocol (AF_INET, AF_INET6)
+	socket.AF_INET,        # Default protocol (AF_INET, AF_INET6)
 	authentication         # Array of authentication methods (Optional) (Default NoAuth)
 )
 ```
 
 #### URLLib Proxied
 ```python
 import urllib.request
@@ -84,15 +84,15 @@
 socket.socket = sockslib.SocksSocket # Make the default socket object a SocksSocket
 
 html = urllib.request.urlopen('https://myexternalip.com/raw').read() # Request the page
 print(html)
 ```
 
 ### IPv6
-To connect to a proxy server via ipv6, you must explicitly specify the protocol by passing the `ip_protocol` parameter to the SocksSocket constructor. 
+To connect to a proxy server via ipv6, you must explicitly specify the protocol by passing the `ip_protocol` parameter to the SocksSocket constructor, OR by using the 3rd option of [set_default_proxy](#set-a-default-proxy).
 Here is an example of connecting to a remote IPv6 proxy:
 ```python
 import sockslib
 import socket # import socket for the protocol specifiers 
 
 with sockslib.SocksSocket(ip_protocol=socket.AF_INET6) as sock:
     sock.set_proxy(('::1', 9050)) # Set proxy
@@ -125,14 +125,15 @@
 
 with sockslib.SocksSocket(udp=True) as sock:
     sock.set_proxy(('127.0.0.1', 9050)) # Set proxy
 
     sock.initudp() # Connect to Server and bind a UDP port for communication
     sock.sendto(b"Hello, World", ("0.0.0.0", 12000)) # Send "Hello, World" to 0.0.0.0:12000 over UDP
 ```
+Due to the nature of UDP in the SOCKS5 protocol, it is reccomended to use the context manager, as the remote proxy server will not drop the UDP associate request until the socket is closed. 
 
 ### Using other authentication methods
 To use more authentication methods like User/Pass auth, you pass an array of authentication methods to the third parameter of `set_proxy` (Don't neglect to set the second parameter to the proxy type!)
 ```python
 import sockslib
 
 with sockslib.SocksSocket() as sock:
```

### Comparing `sockslib-1.7.5/tests/test_socks.py` & `sockslib-1.7.6/tests/test_socks.py`

 * *Files identical despite different names*

### Comparing `sockslib-1.7.5/tests/test_socks_ipv6.py` & `sockslib-1.7.6/tests/test_socks_ipv6.py`

 * *Files identical despite different names*

