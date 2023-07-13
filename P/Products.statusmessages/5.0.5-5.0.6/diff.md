# Comparing `tmp/Products.statusmessages-5.0.5.tar.gz` & `tmp/Products.statusmessages-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Products.statusmessages-5.0.5.tar", last modified: Wed Apr 22 22:22:21 2020, max compression
+gzip compressed data, was "Products.statusmessages-5.0.6.tar", last modified: Thu Jul 13 22:16:36 2023, max compression
```

## Comparing `Products.statusmessages-5.0.5.tar` & `Products.statusmessages-5.0.6.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/
--rw-r--r--   0 maurits    (501) staff       (20)     9846 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products/statusmessages/
--rw-r--r--   0 maurits    (501) staff       (20)      760 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products/statusmessages/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      709 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products/statusmessages/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3647 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products/statusmessages/adapter.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products/statusmessages/tests/
--rw-r--r--   0 maurits    (501) staff       (20)      264 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products/statusmessages/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     1983 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products/statusmessages/tests/test_encoding.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products/statusmessages/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     8050 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products/statusmessages/tests/test_adapter.py
--rw-r--r--   0 maurits    (501) staff       (20)       60 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products/statusmessages/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3021 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products/statusmessages/message.py
--rw-r--r--   0 maurits    (501) staff       (20)       38 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/requirements.txt
--rw-r--r--   0 maurits    (501) staff       (20)       70 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      196 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/buildout.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      397 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      197 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/MANIFEST.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/docs/
--rw-r--r--   0 maurits    (501) staff       (20)      238 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/docs/CREDITS.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1527 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/docs/LICENSE.TXT
--rw-r--r--   0 maurits    (501) staff       (20)     1779 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products.statusmessages.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     9846 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products.statusmessages.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products.statusmessages.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)        9 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products.statusmessages.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)      871 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products.statusmessages.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)       85 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products.statusmessages.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products.statusmessages.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/Products.statusmessages.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      145 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1212 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5224 2020-04-22 22:22:21.000000 Products.statusmessages-5.0.5/CHANGES.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:16:36.605369 Products.statusmessages-5.0.6/
+-rw-r--r--   0 maurits    (501) staff       (20)     5333 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      197 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     7608 2023-07-13 22:16:36.605077 Products.statusmessages-5.0.6/PKG-INFO
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:16:36.599524 Products.statusmessages-5.0.6/Products/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/Products/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:16:36.603171 Products.statusmessages-5.0.6/Products/statusmessages/
+-rw-r--r--   0 maurits    (501) staff       (20)       36 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/Products/statusmessages/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3585 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/Products/statusmessages/adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)      716 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/Products/statusmessages/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      718 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/Products/statusmessages/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2839 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/Products/statusmessages/message.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:16:36.604267 Products.statusmessages-5.0.6/Products/statusmessages/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/Products/statusmessages/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8015 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/Products/statusmessages/tests/test_adapter.py
+-rw-r--r--   0 maurits    (501) staff       (20)      240 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/Products/statusmessages/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1901 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/Products/statusmessages/tests/test_encoding.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:16:36.601739 Products.statusmessages-5.0.6/Products.statusmessages.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     7608 2023-07-13 22:16:36.000000 Products.statusmessages-5.0.6/Products.statusmessages.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      831 2023-07-13 22:16:36.000000 Products.statusmessages-5.0.6/Products.statusmessages.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 22:16:36.000000 Products.statusmessages-5.0.6/Products.statusmessages.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2023-07-13 22:16:36.000000 Products.statusmessages-5.0.6/Products.statusmessages.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-13 22:16:36.000000 Products.statusmessages-5.0.6/Products.statusmessages.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-07-13 22:16:36.000000 Products.statusmessages-5.0.6/Products.statusmessages.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2023-07-13 22:16:36.000000 Products.statusmessages-5.0.6/Products.statusmessages.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1212 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-13 22:16:36.604768 Products.statusmessages-5.0.6/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)      238 2023-07-13 22:16:35.000000 Products.statusmessages-5.0.6/docs/CREDITS.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1527 2023-07-13 22:16:36.000000 Products.statusmessages-5.0.6/docs/LICENSE.TXT
+-rw-r--r--   0 maurits    (501) staff       (20)     4191 2023-07-13 22:16:36.000000 Products.statusmessages-5.0.6/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-07-13 22:16:36.605435 Products.statusmessages-5.0.6/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1786 2023-07-13 22:16:36.000000 Products.statusmessages-5.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Products.statusmessages-5.0.5/Products/statusmessages/interfaces.py` & `Products.statusmessages-5.0.6/Products/statusmessages/interfaces.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-# -*- coding: utf-8 -*-
 from zope.interface import Attribute
 from zope.interface import Interface
 
 
 class IMessage(Interface):
     """A single status message."""
 
-    message = Attribute('The text of this message. Usally a Message object.')
+    message = Attribute("The text of this message. Usually a Message object.")
 
-    type = Attribute('The type of this message.')
+    type = Attribute("The type of this message.")
 
 
 class IStatusMessage(Interface):
     """An adapter for the BrowserRequest to handle status messages."""
 
-    def addStatusMessage(text, type=u'info'):
+    def addStatusMessage(text, type="info"):
         """Add a status message."""
 
-    def add(text, type=u'info'):
+    def add(text, type="info"):
         """Add a status message."""
 
     def showStatusMessages():
-        """Removes all status messages and returns them for display.
-        """
+        """Removes all status messages and returns them for display."""
+
     def show():
-        """Removes all status messages and returns them for display.
-        """
+        """Removes all status messages and returns them for display."""
```

### Comparing `Products.statusmessages-5.0.5/Products/statusmessages/configure.zcml` & `Products.statusmessages-5.0.6/Products/statusmessages/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-<configure xmlns="http://namespaces.zope.org/zope"
-    xmlns:zcml="http://namespaces.zope.org/zcml">
+<configure
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    >
 
   <adapter
-      for="zope.publisher.interfaces.browser.IBrowserRequest"
-      provides=".interfaces.IStatusMessage"
       factory=".adapter.StatusMessage"
+      provides=".interfaces.IStatusMessage"
+      for="zope.publisher.interfaces.browser.IBrowserRequest"
       />
 
   <class class=".message.Message">
-      <allow interface=".interfaces.IMessage" />
+    <allow interface=".interfaces.IMessage" />
   </class>
 
   <!-- We need to make the request annotatable for this to work -->
 
   <configure zcml:condition="installed ZPublisher">
 
     <include package="zope.annotation" />
```

### Comparing `Products.statusmessages-5.0.5/Products/statusmessages/adapter.py` & `Products.statusmessages-5.0.6/Products/statusmessages/adapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,53 @@
-# -*- coding: utf-8 -*-
 from Products.statusmessages import STATUSMESSAGEKEY
 from Products.statusmessages.interfaces import IStatusMessage
 from Products.statusmessages.message import decode
 from Products.statusmessages.message import Message
 from zope.annotation.interfaces import IAnnotations
 from zope.i18n import translate
 from zope.interface import implementer
 
 import binascii
 import logging
 
 
-logger = logging.getLogger('statusmessages')
+logger = logging.getLogger("statusmessages")
 
 
 @implementer(IStatusMessage)
-class StatusMessage(object):
+class StatusMessage:
     """Adapter for the BrowserRequest to handle status messages.
 
     Let's make sure that this implementation actually fulfills the
     'IStatusMessage' API::
 
         >>> from zope.interface.verify import verifyClass
         >>> verifyClass(IStatusMessage, StatusMessage)
         True
     """
 
     def __init__(self, context):
         self.context = context  # the context must be the request
 
-    def add(self, text, type=u'info'):
-        """Add a status message.
-        """
+    def add(self, text, type="info"):
+        """Add a status message."""
         context = self.context
         text = translate(text, context=context)
         annotations = IAnnotations(context)
 
         old = annotations.get(
             STATUSMESSAGEKEY,
             context.cookies.get(STATUSMESSAGEKEY),
         )
         value = _encodeCookieValue(text, type, old=old)
-        context.response.setCookie(STATUSMESSAGEKEY, value, path='/')
+        context.response.setCookie(STATUSMESSAGEKEY, value, path="/")
         annotations[STATUSMESSAGEKEY] = value
 
     def show(self):
-        """Removes all status messages and returns them for display.
-        """
+        """Removes all status messages and returns them for display."""
         context = self.context
         annotations = IAnnotations(context)
         value = annotations.get(
             STATUSMESSAGEKEY,
             context.cookies.get(STATUSMESSAGEKEY),
         )
         if value is None:
@@ -59,55 +56,54 @@
 
         # clear the existing cookie entries, except on responses that don't
         # actually render in the browser (really, these shouldn't render
         # anything so we shouldn't get to this message, but some templates
         # are sloppy).
         if self.context.response.getStatus() not in (301, 302, 304):
             context.cookies[STATUSMESSAGEKEY] = None
-            context.response.expireCookie(STATUSMESSAGEKEY, path='/')
+            context.response.expireCookie(STATUSMESSAGEKEY, path="/")
             annotations[STATUSMESSAGEKEY] = None
 
         return value
 
     # BBB
     addStatusMessage = add
     showStatusMessages = show
 
 
 def _encodeCookieValue(text, type, old=None):
     """Encodes text and type to a list of Messages. If there is already some old
-       existing list, add the new Message at the end but don't add duplicate
-       messages.
+    existing list, add the new Message at the end but don't add duplicate
+    messages.
     """
     results = []
     message = Message(text, type=type)
 
     if old is not None:
         results = _decodeCookieValue(old)
     if message not in results:
         results.append(message)
 
-    messages = b''.join([r.encode() for r in results])
+    messages = b"".join([r.encode() for r in results])
     bin_value = binascii.b2a_base64(messages).rstrip()
     # remove the stupid b that will lead to values like "b'AYR...'"
-    return bin_value.decode('utf-8')
+    return bin_value.decode("utf-8")
 
 
 def _decodeCookieValue(string):
-    """Decode a cookie value to a list of Messages.
-    """
+    """Decode a cookie value to a list of Messages."""
     results = []
     # Return nothing if the cookie is marked as deleted
-    if string == 'deleted':
+    if string == "deleted":
         return results
     # Try to decode the cookie value
     try:
         value = binascii.a2b_base64(string)
         while len(value) > 1:  # at least 2 bytes of data
             message, value = decode(value)
             if message is not None:
                 results.append(message)
     except (binascii.Error, UnicodeEncodeError):
-        logger.exception('Unexpected value in statusmessages cookie')
+        logger.exception("Unexpected value in statusmessages cookie")
         return []
 
     return results
```

### Comparing `Products.statusmessages-5.0.5/Products/statusmessages/tests/test_encoding.py` & `Products.statusmessages-5.0.6/Products/statusmessages/tests/test_encoding.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,73 @@
-# -*- coding: UTF-8 -*-
-from __future__ import unicode_literals
-
 import unittest
 
 
 class TestEncoding(unittest.TestCase):
-
     def test_encoding_msg_with_type(self):
-        """Test message encoding:
-        """
-        from Products.statusmessages.message import Message
+        """Test message encoding:"""
         from Products.statusmessages.message import decode
-        m = Message('späm', 'eggs')
+        from Products.statusmessages.message import Message
+
+        m = Message("späm", "eggs")
         self.assertEqual(
             m.encode(),
-            b'\x00\xa4sp\xc3\xa4meggs',
+            b"\x00\xa4sp\xc3\xa4meggs",
         )
         self.assertEqual(decode(m.encode())[0], m)
 
     def test_encoding_msg_without_type(self):
-        from Products.statusmessages.message import Message
         from Products.statusmessages.message import decode
-        m = Message('späm')
+        from Products.statusmessages.message import Message
+
+        m = Message("späm")
         self.assertEqual(
             m,
-            Message('späm'),
+            Message("späm"),
         )
-        self.assertEqual(m.encode(), b'\x00\xa0sp\xc3\xa4m')
+        self.assertEqual(m.encode(), b"\x00\xa0sp\xc3\xa4m")
         self.assertEqual(decode(m.encode())[0], m)
 
     def test_decoding(self):
-        """Test message decoding:
-        """
+        """Test message decoding:"""
         from Products.statusmessages.message import decode
 
         # Craft a wrong value:
-        m, rem = decode(b'\x01\x84spameggs')
+        m, rem = decode(b"\x01\x84spameggs")
         self.assertEqual(
             m.message,
-            'spameggs',
+            "spameggs",
         )
         self.assertEqual(
             m.type,
-            '',
+            "",
         )
-        self.assertEqual(rem, b'')
+        self.assertEqual(rem, b"")
 
         # Craft another wrong value:
-        m, rem = decode(b'\x00\x24spameggs')
+        m, rem = decode(b"\x00\x24spameggs")
         self.assertEqual(
             m.message,
-            's',
+            "s",
         )
         self.assertEqual(
             m.type,
-            'pame',
+            "pame",
         )
-        self.assertEqual(rem, b'ggs')
+        self.assertEqual(rem, b"ggs")
 
         # And another wrong value:
-        m, rem = decode(b'\x00spameggs')
+        m, rem = decode(b"\x00spameggs")
         self.assertEqual(
             m.message,
-            'pam',
+            "pam",
         )
         self.assertEqual(
             m.type,
-            'eggs',
+            "eggs",
         )
-        self.assertEqual(rem, b'')
+        self.assertEqual(rem, b"")
 
         # And yet another wrong value:
-        m, rem = decode('')
+        m, rem = decode("")
 
         self.assertIs(m, None)
-        self.assertEqual(rem, b'')
+        self.assertEqual(rem, b"")
```

### Comparing `Products.statusmessages-5.0.5/Products/statusmessages/tests/test_adapter.py` & `Products.statusmessages-5.0.6/Products/statusmessages/tests/test_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# -*- coding: UTF-8 -*-
 """ StatusMessage adapter tests. """
 import unittest
 
 
 class TestAdapter(unittest.TestCase):
-
     def test_directives(self):
         """
         Test status messages
 
         First some boilerplate.
 
           >>> from zope.component.testing import setUp
@@ -207,15 +205,15 @@
 
         Messages are stored as base64-ed cookie values, so we must make sure we
         create proper header values; all ascii characters, and no newlines:
 
           >>> status.add(u'täst' * 40, type=u'info')
           >>> cookies = [c['value'] for c in request.response.cookies.values()]
           >>> cookies = ''.join(cookies)
-          >>> cookies == six.text_type(cookies).encode('ASCII')
+          >>> cookies == str(cookies).encode('ASCII')
           True
           >>> '\\n' in cookies
           False
 
           >>> from zope.component.testing import tearDown
           >>> tearDown()
         """
```

### Comparing `Products.statusmessages-5.0.5/Products/statusmessages/message.py` & `Products.statusmessages-5.0.6/Products/statusmessages/message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals
 from Products.statusmessages.interfaces import IMessage
 from zope.interface import implementer
 
-import six
 import struct
 
 
 def _utf8(value):
-    if isinstance(value, six.text_type):
-        return value.encode('utf-8')
-    elif isinstance(value, six.binary_type):
+    if isinstance(value, str):
+        return value.encode("utf-8")
+    elif isinstance(value, bytes):
         return value
-    return b''
+    return b""
 
 
 def _unicode(value):
-    return six.text_type(value, 'utf-8', 'ignore')
+    return str(value, "utf-8", "ignore")
 
 
 @implementer(IMessage)
-class Message(object):
+class Message:
     """A single status message.
 
     Let's make sure that this implementation actually fulfills the
     'IMessage' API.
 
       >>> from zope.interface.verify import verifyClass
       >>> verifyClass(IMessage, Message)
@@ -56,15 +53,15 @@
       True
 
       >>> status.message.domain == u'test'
       True
 
     """
 
-    def __init__(self, message, type=''):
+    def __init__(self, message, type=""):
         self.message = message
         self.type = type
 
     def __eq__(self, other):
         if not isinstance(other, Message):
             return False
         if self.message == other.message and self.type == other.type:
@@ -75,18 +72,15 @@
         """
         Encode to a cookie friendly format.
 
         The format consists of a two bytes length header of 11 bits for the
         message length and 5 bits for the type length followed by two values.
         """
 
-        if six.PY3:
-            fmt_tpl = '!H{0}s{1}s'
-        else:
-            fmt_tpl = b'!H{0}s{1}s'
+        fmt_tpl = "!H{0}s{1}s"
         message = _utf8(self.message)[:0x3FF]  # we can store 2^11 bytes
         type_ = _utf8(self.type)[:0x1F]  # we can store 2^5 bytes
         size = (len(message) << 5) + (len(type_) & 31)  # pack into 16 bits
         fmt = fmt_tpl.format(len(message), len(type_))
         return struct.pack(fmt, size, message, type_)
 
 
@@ -96,15 +90,15 @@
 
     We return the decoded message object, and the remainder of the cookie
     value as bytes (it can contain further messages).
 
     We expect at least 2 bytes (size information).
     """
     if len(value) >= 2:
-        size = struct.unpack(b'!H', value[:2])[0]
+        size = struct.unpack(b"!H", value[:2])[0]
         msize, tsize = (size >> 5, size & 31)
         message = Message(
-            _unicode(value[2:msize + 2]),
-            _unicode(value[msize + 2:msize + tsize + 2]),
+            _unicode(value[2 : msize + 2]),
+            _unicode(value[msize + 2 : msize + tsize + 2]),
         )
-        return message, value[msize + tsize + 2:]
-    return None, b''
+        return message, value[msize + tsize + 2 :]
+    return None, b""
```

### Comparing `Products.statusmessages-5.0.5/docs/LICENSE.TXT` & `Products.statusmessages-5.0.6/docs/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `Products.statusmessages-5.0.5/setup.py` & `Products.statusmessages-5.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,59 @@
-# -*- coding: utf-8 -*-
+from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '5.0.5'
+version = "5.0.6"
+
+long_description = (
+    f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
+)
 
 setup(
-    name='Products.statusmessages',
+    name="Products.statusmessages",
     version=version,
-    description='statusmessages provides an easy way of handling '
-                'internationalized status messages managed via an '
-                'BrowserRequest adapter storing status messages in '
-                'client-side cookies.',
-    long_description=(open('README.rst').read() + '\n' +
-                      open('CHANGES.rst').read()),
+    description="statusmessages provides an easy way of handling "
+    "internationalized status messages managed via an "
+    "BrowserRequest adapter storing status messages in "
+    "client-side cookies.",
+    long_description=long_description,
+    long_description_content_type="text/x-rst",
+    # Get more strings from
+    # https://pypi.org/classifiers/
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Framework :: Plone',
-        'Framework :: Plone :: 5.0',
-        'Framework :: Plone :: 5.1',
-        'Framework :: Plone :: 5.2',
-        'Framework :: Plone :: Core',
-        'Framework :: Zope2',
-        'Framework :: Zope :: 4',
-        'License :: OSI Approved :: BSD License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Web Environment",
+        "Framework :: Plone",
+        "Framework :: Plone :: 6.0",
+        "Framework :: Plone :: Core",
+        "Framework :: Zope :: 5",
+        "License :: OSI Approved :: BSD License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    keywords='Zope CMF Plone status messages i18n',
-    author='Hanno Schlichting',
-    author_email='plone-developers@lists.sourceforge.net',
-    url='https://pypi.org/project/Products.statusmessages',
-    license='BSD',
+    keywords="Zope CMF Plone status messages i18n",
+    author="Hanno Schlichting",
+    author_email="plone-developers@lists.sourceforge.net",
+    url="https://pypi.org/project/Products.statusmessages",
+    license="BSD",
     packages=find_packages(),
-    namespace_packages=['Products'],
+    namespace_packages=["Products"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     extras_require=dict(
         test=[
-            'zope.component',
-            'Zope2',
+            "Zope",
         ],
     ),
     install_requires=[
-        'setuptools',
-        'six',
-        'zope.annotation',
-        'zope.i18n',
-        'zope.interface',
+        "setuptools",
+        "zope.annotation",
+        "zope.i18n",
+        "zope.interface",
+        "zope.publisher",
     ],
 )
```

### Comparing `Products.statusmessages-5.0.5/Products.statusmessages.egg-info/SOURCES.txt` & `Products.statusmessages-5.0.6/Products.statusmessages.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
-buildout.cfg
 pyproject.toml
-requirements.txt
-setup.cfg
 setup.py
 Products/__init__.py
 Products.statusmessages.egg-info/PKG-INFO
 Products.statusmessages.egg-info/SOURCES.txt
 Products.statusmessages.egg-info/dependency_links.txt
 Products.statusmessages.egg-info/namespace_packages.txt
 Products.statusmessages.egg-info/not-zip-safe
```

### Comparing `Products.statusmessages-5.0.5/README.rst` & `Products.statusmessages-5.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `Products.statusmessages-5.0.5/CHANGES.rst` & `Products.statusmessages-5.0.6/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.6 (2023-07-14)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (cc314a2b)
+
+
 5.0.5 (2020-04-23)
 ------------------
 
 Bug fixes:
 
 
 - Minor packaging updates. (#1)
```

