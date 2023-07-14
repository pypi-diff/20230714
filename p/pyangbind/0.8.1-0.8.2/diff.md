# Comparing `tmp/pyangbind-0.8.1.tar.gz` & `tmp/pyangbind-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyangbind-0.8.1.tar", last modified: Wed May 16 20:40:12 2018, max compression
+gzip compressed data, was "pyangbind-0.8.2.tar", last modified: Fri Jul 14 05:46:30 2023, max compression
```

## Comparing `pyangbind-0.8.1.tar` & `pyangbind-0.8.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-16 20:40:12.000000 pyangbind-0.8.1/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-16 20:40:12.000000 pyangbind-0.8.1/pyangbind/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-16 20:40:12.000000 pyangbind-0.8.1/pyangbind/helpers/
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-05-16 20:39:22.000000 pyangbind-0.8.1/pyangbind/helpers/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5065 2018-05-16 20:39:22.000000 pyangbind-0.8.1/pyangbind/helpers/identity.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1984 2018-05-16 20:39:22.000000 pyangbind-0.8.1/pyangbind/helpers/misc.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-16 20:40:12.000000 pyangbind-0.8.1/pyangbind/lib/
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-05-16 20:39:22.000000 pyangbind-0.8.1/pyangbind/lib/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3555 2018-05-16 20:39:22.000000 pyangbind-0.8.1/pyangbind/lib/base.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5965 2018-05-16 20:39:22.000000 pyangbind-0.8.1/pyangbind/lib/pybindJSON.py
--rw-r--r--   0 travis    (2000) travis    (2000)    21008 2018-05-16 20:39:22.000000 pyangbind-0.8.1/pyangbind/lib/serialise.py
--rw-r--r--   0 travis    (2000) travis    (2000)    12596 2018-05-16 20:39:22.000000 pyangbind-0.8.1/pyangbind/lib/xpathhelper.py
--rw-r--r--   0 travis    (2000) travis    (2000)    44823 2018-05-16 20:39:22.000000 pyangbind-0.8.1/pyangbind/lib/yangtypes.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-16 20:40:12.000000 pyangbind-0.8.1/pyangbind/plugin/
--rw-r--r--   0 travis    (2000) travis    (2000)        0 2018-05-16 20:39:22.000000 pyangbind-0.8.1/pyangbind/plugin/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)    67663 2018-05-16 20:39:22.000000 pyangbind-0.8.1/pyangbind/plugin/pybind.py
--rw-r--r--   0 travis    (2000) travis    (2000)       22 2018-05-16 20:39:22.000000 pyangbind-0.8.1/pyangbind/__init__.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-05-16 20:40:12.000000 pyangbind-0.8.1/pyangbind.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     4306 2018-05-16 20:40:12.000000 pyangbind-0.8.1/pyangbind.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      638 2018-05-16 20:40:12.000000 pyangbind-0.8.1/pyangbind.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-05-16 20:40:12.000000 pyangbind-0.8.1/pyangbind.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-05-16 20:40:12.000000 pyangbind-0.8.1/pyangbind.egg-info/not-zip-safe
--rw-r--r--   0 travis    (2000) travis    (2000)       37 2018-05-16 20:40:12.000000 pyangbind-0.8.1/pyangbind.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       10 2018-05-16 20:40:12.000000 pyangbind-0.8.1/pyangbind.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)     1721 2018-05-16 20:39:22.000000 pyangbind-0.8.1/CONTRIBUTING.md
--rw-r--r--   0 travis    (2000) travis    (2000)      663 2018-05-16 20:39:22.000000 pyangbind-0.8.1/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)       43 2018-05-16 20:39:22.000000 pyangbind-0.8.1/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)    17126 2018-05-16 20:39:22.000000 pyangbind-0.8.1/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)     2947 2018-05-16 20:39:22.000000 pyangbind-0.8.1/README.rst
--rw-r--r--   0 travis    (2000) travis    (2000)       69 2018-05-16 20:39:22.000000 pyangbind-0.8.1/requirements.DEVELOPER.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       37 2018-05-16 20:39:22.000000 pyangbind-0.8.1/requirements.txt
--rw-r--r--   0 travis    (2000) travis    (2000)      152 2018-05-16 20:40:12.000000 pyangbind-0.8.1/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)     1969 2018-05-16 20:39:22.000000 pyangbind-0.8.1/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4306 2018-05-16 20:40:12.000000 pyangbind-0.8.1/PKG-INFO
+drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-14 05:46:30.948363 pyangbind-0.8.2/
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     1381 2023-07-14 05:46:04.000000 pyangbind-0.8.2/CONTRIBUTING.md
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)      663 2023-07-09 09:56:01.000000 pyangbind-0.8.2/LICENSE
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       43 2023-07-09 09:56:01.000000 pyangbind-0.8.2/MANIFEST.in
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     4084 2023-07-14 05:46:30.949363 pyangbind-0.8.2/PKG-INFO
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    17961 2023-07-09 09:56:01.000000 pyangbind-0.8.2/README.md
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     2947 2023-07-09 09:56:01.000000 pyangbind-0.8.2/README.rst
+drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-14 05:46:30.928353 pyangbind-0.8.2/pyangbind/
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       22 2023-07-14 05:44:13.000000 pyangbind-0.8.2/pyangbind/__init__.py
+drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-14 05:46:30.939358 pyangbind-0.8.2/pyangbind/helpers/
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/helpers/__init__.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     5749 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/helpers/identity.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     1980 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/helpers/misc.py
+drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-14 05:46:30.944361 pyangbind-0.8.2/pyangbind/lib/
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/lib/__init__.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     4260 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/lib/base.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     6298 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/lib/pybindJSON.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    35984 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/lib/serialise.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    13400 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/lib/xpathhelper.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    51329 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/lib/yangtypes.py
+drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-14 05:46:30.946362 pyangbind-0.8.2/pyangbind/plugin/
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/plugin/__init__.py
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)    74162 2023-07-09 09:56:01.000000 pyangbind-0.8.2/pyangbind/plugin/pybind.py
+drwxr-xr-x   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        0 2023-07-14 05:46:30.936357 pyangbind-0.8.2/pyangbind.egg-info/
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     4084 2023-07-14 05:46:30.000000 pyangbind-0.8.2/pyangbind.egg-info/PKG-INFO
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)      644 2023-07-14 05:46:30.000000 pyangbind-0.8.2/pyangbind.egg-info/SOURCES.txt
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        1 2023-07-14 05:46:30.000000 pyangbind-0.8.2/pyangbind.egg-info/dependency_links.txt
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)        1 2023-07-09 12:06:51.000000 pyangbind-0.8.2/pyangbind.egg-info/not-zip-safe
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       37 2023-07-14 05:46:30.000000 pyangbind-0.8.2/pyangbind.egg-info/requires.txt
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       10 2023-07-14 05:46:30.000000 pyangbind-0.8.2/pyangbind.egg-info/top_level.txt
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       99 2023-07-14 05:46:04.000000 pyangbind-0.8.2/pyproject.toml
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)      114 2023-07-14 05:46:04.000000 pyangbind-0.8.2/requirements.DEVELOPER.txt
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)       37 2023-07-09 09:56:01.000000 pyangbind-0.8.2/requirements.txt
+-rw-r--r--   0 joseignaciotamayo  (1000) joseignaciotamayo  (1000)     1425 2023-07-14 05:46:30.950364 pyangbind-0.8.2/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyangbind-0.8.1/pyangbind/helpers/identity.py` & `pyangbind-0.8.2/pyangbind/helpers/identity.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,143 +17,144 @@
 """
 
 from pyang import util
 from .misc import module_import_prefixes
 
 
 class Identity(object):
-  def __init__(self, name):
-    self.name = name
-    self.source_module = None
-    self._imported_prefixes = []
-    self.source_namespace = None
-    self.base = None
-    self.children = []
-
-  def add_prefix(self, prefix):
-    if prefix not in self._imported_prefixes:
-      self._imported_prefixes.append(prefix)
-
-  def add_child(self, child):
-    if not isinstance(child, Identity):
-      raise ValueError("Must supply a identity as a child")
-    self.children.append(child)
 
-  def __str__(self):
-    return "%s:%s" % (self.source_module, self.name)
+    def __init__(self, name):
+        self.name = name
+        self.source_module = None
+        self._imported_prefixes = []
+        self.source_namespace = None
+        self.base = None
+        self.children = []
+
+    def add_prefix(self, prefix):
+        if prefix not in self._imported_prefixes:
+            self._imported_prefixes.append(prefix)
+
+    def add_child(self, child):
+        if not isinstance(child, Identity):
+            raise ValueError("Must supply a identity as a child")
+        self.children.append(child)
 
-  def prefixes(self):
-    return self._imported_prefixes
+    def __str__(self):
+        return "%s:%s" % (self.source_module, self.name)
+
+    def prefixes(self):
+        return self._imported_prefixes
 
 
 class IdentityStore(object):
-  def __init__(self):
-    self._store = []
 
-  def find_identity_by_source_name(self, s, n):
-    for i in self._store:
-      if i.source_module == s and i.name == n:
-        return i
-
-  def add_identity(self, i):
-    if isinstance(i, Identity):
-      if not self.find_identity_by_source_name(i.source_module, i.name):
-        self._store.append(i)
-    else:
-      raise ValueError("Must specify an identity")
-
-  def identities(self):
-    return ["%s:%s" % (i.source_module, i.name) for i in self._store]
-
-  def __iter__(self):
-    return iter(self._store)
-
-  def build_store_from_definitions(self, ctx, defnd):
-    unresolved_identities = list(defnd.keys())
-    unresolved_identity_count = {k: 0 for k in defnd}
-    error_ids = []
-
-    mod_ref_prefixes = module_import_prefixes(ctx)
-
-    while len(unresolved_identities):
-      this_id = unresolved_identities.pop(0)
-      iddef = defnd[this_id]
-
-      base = iddef.search_one('base')
-      try:
-        mainmod = iddef.main_module()
-      except AttributeError:
-        mainmod = None
-      if mainmod is not None:
-        defmod = mainmod
-
-      defining_module = defmod.arg
-      namespace = defmod.search_one('namespace').arg
-      prefix = defmod.search_one('prefix').arg
-
-      if base is None:
-        # Add a new identity which can be a base
-        tid = Identity(iddef.arg)
-        tid.source_module = defining_module
-        tid.source_namespace = namespace
-        tid.add_prefix(prefix)
-        self.add_identity(tid)
-
-        if defining_module in mod_ref_prefixes:
-          for i in mod_ref_prefixes[defining_module]:
-            tid.add_prefix(i)
-
-      else:
-        # Determine what the name of the base and the prefix for
-        # the base should be
-        if ":" in base.arg:
-          base_pfx, base_name = base.arg.split(":")
+    def __init__(self):
+        self._store = []
+
+    def find_identity_by_source_name(self, s, n):
+        for i in self._store:
+            if i.source_module == s and i.name == n:
+                return i
+
+    def add_identity(self, i):
+        if isinstance(i, Identity):
+            if not self.find_identity_by_source_name(i.source_module, i.name):
+                self._store.append(i)
         else:
-          base_pfx, base_name = prefix, base.arg
+            raise ValueError("Must specify an identity")
 
-        parent_module = util.prefix_to_module(defmod, base_pfx,
-                                  base.pos, ctx.errors)
+    def identities(self):
+        return ["%s:%s" % (i.source_module, i.name) for i in self._store]
 
-        # Find whether we have the base in the store
-        base_id = self.find_identity_by_source_name(parent_module.arg, base_name)
+    def __iter__(self):
+        return iter(self._store)
 
-        if base_id is None:
-          # and if not, then push this identity back onto the stack
-          unresolved_identities.append(this_id)
-          unresolved_identity_count[this_id] += 1
-          # FIXME(Joey Wilhelm): `unresolved_idc` and `ident` are both undefined. What is the intent of this code?
-          # if unresolved_identity_count[this_id] > 1000:
-          #   if unresolved_idc[ident] > 1000:
-          #     sys.stderr.write("could not find a match for %s base: %s\n" %
-          #       (iddef.arg, base_name))
-          #     error_ids.append(ident)
-        else:
-          # Check we don't already have this identity defined
-          if self.find_identity_by_source_name(defining_module, iddef.arg) is None:
-            # otherwise, create a new identity that reflects this one
-            tid = Identity(iddef.arg)
-            tid.source_module = defining_module
-            tid.source_namespace = namespace
-            tid.add_prefix(prefix)
-            base_id.add_child(tid)
-            self.add_identity(tid)
-
-            if defining_module in mod_ref_prefixes:
-              for i in mod_ref_prefixes[defining_module]:
-                tid.add_prefix(i)
-
-      if error_ids:
-        raise TypeError("could not resolve identities %s" % error_ids)
-
-    self._build_inheritance()
-
-  def _recurse_children(self, identity, children):
-    for child in identity.children:
-      children.append(child)
-      self._recurse_children(child, children)
-    return children
-
-  def _build_inheritance(self):
-    for i in self._store:
-      ch = list()
-      self._recurse_children(i, ch)
-      i.children = ch
+    def build_store_from_definitions(self, ctx, defnd):
+        unresolved_identities = list(defnd.keys())
+        unresolved_identity_count = {k: 0 for k in defnd}
+        error_ids = []
+
+        mod_ref_prefixes = module_import_prefixes(ctx)
+
+        while len(unresolved_identities):
+            this_id = unresolved_identities.pop(0)
+            iddef = defnd[this_id]
+
+            base = iddef.search_one("base")
+            try:
+                mainmod = iddef.main_module()
+            except AttributeError:
+                mainmod = None
+            if mainmod is not None:
+                defmod = mainmod
+
+            defining_module = defmod.arg
+            namespace = defmod.search_one("namespace").arg
+            prefix = defmod.search_one("prefix").arg
+
+            if base is None:
+                # Add a new identity which can be a base
+                tid = Identity(iddef.arg)
+                tid.source_module = defining_module
+                tid.source_namespace = namespace
+                tid.add_prefix(prefix)
+                self.add_identity(tid)
+
+                if defining_module in mod_ref_prefixes:
+                    for i in mod_ref_prefixes[defining_module]:
+                        tid.add_prefix(i)
+
+            else:
+                # Determine what the name of the base and the prefix for
+                # the base should be
+                if ":" in base.arg:
+                    base_pfx, base_name = base.arg.split(":")
+                else:
+                    base_pfx, base_name = prefix, base.arg
+
+                parent_module = util.prefix_to_module(defmod, base_pfx, base.pos, ctx.errors)
+
+                # Find whether we have the base in the store
+                base_id = self.find_identity_by_source_name(parent_module.arg, base_name)
+
+                if base_id is None:
+                    # and if not, then push this identity back onto the stack
+                    unresolved_identities.append(this_id)
+                    unresolved_identity_count[this_id] += 1
+                    # FIXME(Joey Wilhelm): `unresolved_idc` and `ident` are both undefined. What is the intent of this code?
+                    # if unresolved_identity_count[this_id] > 1000:
+                    #   if unresolved_idc[ident] > 1000:
+                    #     sys.stderr.write("could not find a match for %s base: %s\n" %
+                    #       (iddef.arg, base_name))
+                    #     error_ids.append(ident)
+                else:
+                    # Check we don't already have this identity defined
+                    if self.find_identity_by_source_name(defining_module, iddef.arg) is None:
+                        # otherwise, create a new identity that reflects this one
+                        tid = Identity(iddef.arg)
+                        tid.source_module = defining_module
+                        tid.source_namespace = namespace
+                        tid.add_prefix(prefix)
+                        base_id.add_child(tid)
+                        self.add_identity(tid)
+
+                        if defining_module in mod_ref_prefixes:
+                            for i in mod_ref_prefixes[defining_module]:
+                                tid.add_prefix(i)
+
+            if error_ids:
+                raise TypeError("could not resolve identities %s" % error_ids)
+
+        self._build_inheritance()
+
+    def _recurse_children(self, identity, children):
+        for child in identity.children:
+            children.append(child)
+            self._recurse_children(child, children)
+        return children
+
+    def _build_inheritance(self):
+        for i in self._store:
+            ch = list()
+            self._recurse_children(i, ch)
+            i.children = ch
```

### Comparing `pyangbind-0.8.1/pyangbind/helpers/misc.py` & `pyangbind-0.8.2/pyangbind/helpers/misc.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,45 +16,41 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import sys
 
 
 def module_import_prefixes(ctx):
-  mod_ref_prefixes = {}
-  for mod in ctx.modules:
-    m = ctx.search_module(0, mod[0])
-    for importstmt in m.search('import'):
-      if importstmt.arg not in mod_ref_prefixes:
-        mod_ref_prefixes[importstmt.arg] = []
-      mod_ref_prefixes[importstmt.arg].append(importstmt.search_one('prefix').arg)
-  return mod_ref_prefixes
+    mod_ref_prefixes = {}
+    for mod in ctx.modules:
+        m = ctx.search_module(0, mod[0])
+        for importstmt in m.search("import"):
+            if importstmt.arg not in mod_ref_prefixes:
+                mod_ref_prefixes[importstmt.arg] = []
+            mod_ref_prefixes[importstmt.arg].append(importstmt.search_one("prefix").arg)
+    return mod_ref_prefixes
 
 
 def find_child_definitions(obj, defn, prefix, definitions):
-  for i in obj.search(defn):
-    if i.arg in definitions:
-      sys.stderr.write("WARNING: duplicate definition of %s" % i.arg)
-    else:
-      definitions["%s:%s" % (prefix, i.arg)] = i
-
-  possible_parents = [
-                        'grouping', 'container',
-                        'list', 'rpc', 'input',
-                        'output', 'notification'
-                      ]
-
-  for parent_type in possible_parents:
-    for ch in obj.search(parent_type):
-      if ch.i_children:
-        find_child_definitions(ch, defn, prefix, definitions)
+    for i in obj.search(defn):
+        if i.arg in definitions:
+            sys.stderr.write("WARNING: duplicate definition of %s" % i.arg)
+        else:
+            definitions["%s:%s" % (prefix, i.arg)] = i
+
+    possible_parents = ["grouping", "container", "list", "rpc", "input", "output", "notification"]
+
+    for parent_type in possible_parents:
+        for ch in obj.search(parent_type):
+            if ch.i_children:
+                find_child_definitions(ch, defn, prefix, definitions)
 
-  return definitions
+    return definitions
 
 
 def find_definitions(defn, ctx, module, prefix):
-  # Find the statements within a module that map to a particular type of
-  # statement, for instance - find typedefs, or identities, and reutrn them
-  # as a dictionary to the calling function.
-  definitions = {}
-  defin = find_child_definitions(module, defn, prefix, definitions)
-  return defin
+    # Find the statements within a module that map to a particular type of
+    # statement, for instance - find typedefs, or identities, and reutrn them
+    # as a dictionary to the calling function.
+    definitions = {}
+    defin = find_child_definitions(module, defn, prefix, definitions)
+    return defin
```

### Comparing `pyangbind-0.8.1/pyangbind/lib/base.py` & `pyangbind-0.8.2/pyangbind/lib/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,93 +17,96 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 
 class PybindBase(object):
 
-  __slots__ = ()
+    __slots__ = ()
 
-  def elements(self):
-    return self._pyangbind_elements
+    def elements(self):
+        return self._pyangbind_elements
 
-  def __str__(self):
-    return str(self.elements())
+    def __str__(self):
+        return str(self.elements())
 
-  def get(self, filter=False):
-    def error():
-      return NameError, "element does not exist"
-
-    d = {}
-    # for each YANG element within this container.
-    for element_name in self._pyangbind_elements:
-      element = getattr(self, element_name, error)
-      if hasattr(element, "yang_name"):
-        # retrieve the YANG name method
-        yang_name = getattr(element, "yang_name", error)
-        element_id = yang_name()
-      else:
-        element_id = element_name
-
-      if hasattr(element, "get"):
-        # this is a YANG container that has its own
-        # get method
-        d[element_id] = element.get(filter=filter)
-        if filter is True:
-          # if the element hadn't changed but we were
-          # filtering unchanged elements, remove it
-          # from the dictionary
-          if isinstance(d[element_id], dict):
-            for entry in d[element_id].keys():
-              changed, present = False, False
-
-              if hasattr(d[element_id][entry], "_changed"):
-                if d[element_id][entry]._changed():
-                  changed = True
-              else:
-                changed = None
-
-              if hasattr(d[element_id][entry], "_present"):
-                if not d[element_id][entry]._present() is True:
-                  present = True
-              else:
-                present = None
-
-              if present is False and changed is False:
-                del d[element_id][entry]
-
-            if len(d[element_id]) == 0:
-              if element._presence and element._present():
-                pass
-              else:
-                del d[element_id]
-          elif isinstance(d[element_id], list):
-            for list_entry in d[element_id]:
-              if hasattr(list_entry, "_changed"):
-                if not list_entry._changed():
-                  d[element_id].remove(list_entry)
-            if len(d[element_id]) == 0:
-              del d[element_id]
-      else:
-        # this is an attribute that does not have get()
-        # method
-        if filter is False and not element._changed() and not element._present() is True:
-          if element._default is not False and element._default:
-            d[element_id] = element._default
-          else:
-            d[element_id] = element
-        elif element._changed() or element._present() is True:
-          d[element_id] = element
-        else:
-          # changed = False, and filter = True
-          pass
-    return d
-
-  def __getitem__(self, k):
-    def error():
-      raise KeyError("Key %s does not exist" % k)
-    element = getattr(self, k, error)
-    return element()
-
-  def __iter__(self):
-    for elem in self._pyangbind_elements:
-      yield (elem, getattr(self, elem))
+    def get(self, filter=False):
+
+        def error():
+            return NameError, "element does not exist"
+
+        d = {}
+        # for each YANG element within this container.
+        for element_name in self._pyangbind_elements:
+            element = getattr(self, element_name, error)
+            if hasattr(element, "yang_name"):
+                # retrieve the YANG name method
+                yang_name = getattr(element, "yang_name", error)
+                element_id = yang_name()
+            else:
+                element_id = element_name
+
+            if hasattr(element, "get"):
+                # this is a YANG container that has its own
+                # get method
+                d[element_id] = element.get(filter=filter)
+                if filter is True:
+                    # if the element hadn't changed but we were
+                    # filtering unchanged elements, remove it
+                    # from the dictionary
+                    if isinstance(d[element_id], dict):
+                        for entry in d[element_id].keys():
+                            changed, present = False, False
+
+                            if hasattr(d[element_id][entry], "_changed"):
+                                if d[element_id][entry]._changed():
+                                    changed = True
+                            else:
+                                changed = None
+
+                            if hasattr(d[element_id][entry], "_present"):
+                                if not d[element_id][entry]._present() is True:
+                                    present = True
+                            else:
+                                present = None
+
+                            if present is False and changed is False:
+                                del d[element_id][entry]
+
+                        if len(d[element_id]) == 0:
+                            if element._presence and element._present():
+                                pass
+                            else:
+                                del d[element_id]
+                    elif isinstance(d[element_id], list):
+                        for list_entry in d[element_id]:
+                            if hasattr(list_entry, "_changed"):
+                                if not list_entry._changed():
+                                    d[element_id].remove(list_entry)
+                        if len(d[element_id]) == 0:
+                            del d[element_id]
+            else:
+                # this is an attribute that does not have get()
+                # method
+                if filter is False and not element._changed() and not element._present() is True:
+                    if element._default is not False and element._default:
+                        d[element_id] = element._default
+                    else:
+                        d[element_id] = element
+                elif element._changed() or element._present() is True:
+                    d[element_id] = element
+                else:
+                    # changed = False, and filter = True
+                    pass
+        return d
+
+    def __getitem__(self, k):
+
+        def error():
+            raise KeyError("Key %s does not exist" % k)
+
+        element = getattr(self, k, error)
+        return element()
+
+    def __iter__(self):
+        for elem in self._pyangbind_elements:
+            yield (elem, getattr(self, elem))
```

### Comparing `pyangbind-0.8.1/pyangbind/lib/pybindJSON.py` & `pyangbind-0.8.2/pyangbind/lib/pybindJSON.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,151 +25,144 @@
 
 import six
 
 from pyangbind.lib.serialise import pybindIETFJSONEncoder, pybindJSONDecoder, pybindJSONEncoder, pybindJSONIOError
 
 
 def remove_path(tree, path):
-  this_part = path.pop(0)
-  if len(path) == 0:
+    this_part = path.pop(0)
+    if len(path) == 0:
+        try:
+            del tree[this_part]
+            return tree
+        except KeyError:
+            # ignore missing dictionary key
+            pass
+    else:
+        try:
+            tree[this_part] = remove_path(tree[this_part], path)
+        except KeyError:
+            pass
+    return tree
+
+
+def loads(d, parent_pymod, yang_base, path_helper=None, extmethods=None, overwrite=False):
+    # This check is not really logical - since one would expect 'd' to be
+    # a string, given that this is loads. However, a previous issue meant
+    # that this really expected a dict, so this check simply makes sure
+    # that if the user really did give us a string, we're happy with that
+    # without breaking other code.
+    if isinstance(d, six.string_types + (six.text_type,)):
+        d = json.loads(d, object_pairs_hook=OrderedDict)
+    return pybindJSONDecoder.load_json(
+        d, parent_pymod, yang_base, path_helper=path_helper, extmethods=extmethods, overwrite=overwrite
+    )
+
+
+def loads_ietf(d, parent_pymod, yang_base, path_helper=None, extmethods=None, overwrite=False):
+    # Same as above, to allow for load_ietf to work the same way
+    if isinstance(d, six.string_types + (six.text_type,)):
+        d = json.loads(d, object_pairs_hook=OrderedDict)
+    return pybindJSONDecoder.load_ietf_json(
+        d, parent_pymod, yang_base, path_helper=path_helper, extmethods=extmethods, overwrite=overwrite
+    )
+
+
+def load(fn, parent_pymod, yang_module, path_helper=None, extmethods=None, overwrite=False):
     try:
-      del tree[this_part]
-      return tree
-    except KeyError:
-      # ignore missing dictionary key
-      pass
-  else:
+        with open(fn, "r") as fp:
+            f = json.load(fp, object_pairs_hook=OrderedDict)
+    except IOError as m:
+        raise pybindJSONIOError("could not open file to read: %s" % m)
+    return loads(f, parent_pymod, yang_module, path_helper=path_helper, extmethods=extmethods, overwrite=overwrite)
+
+
+def load_ietf(fn, parent_pymod, yang_module, path_helper=None, extmethods=None, overwrite=False):
     try:
-      tree[this_part] = remove_path(tree[this_part], path)
-    except KeyError:
-      pass
-  return tree
-
-
-def loads(d, parent_pymod, yang_base, path_helper=None, extmethods=None,
-          overwrite=False):
-  # This check is not really logical - since one would expect 'd' to be
-  # a string, given that this is loads. However, a previous issue meant
-  # that this really expected a dict, so this check simply makes sure
-  # that if the user really did give us a string, we're happy with that
-  # without breaking other code.
-  if isinstance(d, six.string_types + (six.text_type,)):
-    d = json.loads(d, object_pairs_hook=OrderedDict)
-  return pybindJSONDecoder.load_json(d, parent_pymod, yang_base,
-          path_helper=path_helper, extmethods=extmethods, overwrite=overwrite)
-
-
-def loads_ietf(d, parent_pymod, yang_base, path_helper=None,
-                extmethods=None, overwrite=False):
-  # Same as above, to allow for load_ietf to work the same way
-  if isinstance(d, six.string_types + (six.text_type,)):
-    d = json.loads(d, object_pairs_hook=OrderedDict)
-  return pybindJSONDecoder.load_ietf_json(d, parent_pymod, yang_base,
-          path_helper=path_helper, extmethods=extmethods, overwrite=overwrite)
-
-
-def load(fn, parent_pymod, yang_module, path_helper=None, extmethods=None,
-             overwrite=False):
-  try:
-    with open(fn, 'r') as fp:
-      f = json.load(fp, object_pairs_hook=OrderedDict)
-  except IOError as m:
-    raise pybindJSONIOError("could not open file to read: %s" % m)
-  return loads(f, parent_pymod, yang_module, path_helper=path_helper,
-                extmethods=extmethods, overwrite=overwrite)
-
-
-def load_ietf(fn, parent_pymod, yang_module, path_helper=None,
-              extmethods=None, overwrite=False):
-  try:
-    f = json.load(open(fn, 'r'), object_pairs_hook=OrderedDict)
-  except IOError as m:
-    raise pybindJSONIOError("Could not open file to read: %s" % m)
-  return loads_ietf(f, parent_pymod, yang_module, path_helper,
-            extmethods=extmethods, overwrite=overwrite)
-
-
-def dumps(obj, indent=4, filter=True, skip_subtrees=[], select=False,
-            mode="default", with_defaults=None):
-  def lookup_subdict(dictionary, key):
-    if not isinstance(key, list):
-      raise AttributeError('keys should be a list')
-    unresolved_dict = {}
-    for k, v in six.iteritems(dictionary):
-      if ":" in k:
-        k = k.split(":")[1]
-      unresolved_dict[k] = v
-
-    if not key[0] in unresolved_dict:
-      raise KeyError("requested non-existent key (%s)" % key[0])
-    if len(key) == 1:
-      return unresolved_dict[key[0]]
-    current = key.pop(0)
-    return lookup_subdict(dictionary[current], key)
-
-  if not isinstance(skip_subtrees, list):
-    raise AttributeError('the subtrees to be skipped should be a list')
-  if mode == 'ietf':
-    tree = pybindIETFJSONEncoder.generate_element(obj, flt=filter,
-                                                  with_defaults=with_defaults)
-  else:
-    tree = obj.get(filter=filter)
-  for p in skip_subtrees:
-    pp = p.split("/")[1:]
-    # Iterate through the skip path and the object's own path to determine
-    # whether they match, then skip the relevant subtrees.
-    match = True
-    trimmed_path = copy.deepcopy(pp)
-    for i, j in zip(obj._path(), pp):
-      # paths may have attributes in them, but the skip dictionary does
-      # not, so we ensure that the object's absolute path is attribute
-      # free,
-      if "[" in i:
-        i = i.split("[")[0]
-      if not i == j:
-        match = False
-        break
-      trimmed_path.pop(0)
-
-    if match and len(trimmed_path):
-      tree = remove_path(tree, trimmed_path)
-
-  if select:
-    key_del = []
-    for t in tree:
-      keep = True
-      for k, v in six.iteritems(select):
-        v = six.text_type(v)
-        if mode == 'default' or isinstance(tree, dict):
-          if (keep and not six.text_type(lookup_subdict(tree[t], k.split("."))) == v):
-            keep = False
+        f = json.load(open(fn, "r"), object_pairs_hook=OrderedDict)
+    except IOError as m:
+        raise pybindJSONIOError("Could not open file to read: %s" % m)
+    return loads_ietf(f, parent_pymod, yang_module, path_helper, extmethods=extmethods, overwrite=overwrite)
+
+
+def dumps(obj, indent=4, filter=True, skip_subtrees=[], select=False, mode="default", with_defaults=None):
+
+    def lookup_subdict(dictionary, key):
+        if not isinstance(key, list):
+            raise AttributeError("keys should be a list")
+        unresolved_dict = {}
+        for k, v in six.iteritems(dictionary):
+            if ":" in k:
+                k = k.split(":")[1]
+            unresolved_dict[k] = v
+
+        if not key[0] in unresolved_dict:
+            raise KeyError("requested non-existent key (%s)" % key[0])
+        if len(key) == 1:
+            return unresolved_dict[key[0]]
+        current = key.pop(0)
+        return lookup_subdict(dictionary[current], key)
+
+    if not isinstance(skip_subtrees, list):
+        raise AttributeError("the subtrees to be skipped should be a list")
+    if mode == "ietf":
+        tree = pybindIETFJSONEncoder.generate_element(obj, flt=filter, with_defaults=with_defaults)
+    else:
+        tree = obj.get(filter=filter)
+    for p in skip_subtrees:
+        pp = p.split("/")[1:]
+        # Iterate through the skip path and the object's own path to determine
+        # whether they match, then skip the relevant subtrees.
+        match = True
+        trimmed_path = copy.deepcopy(pp)
+        for i, j in zip(obj._path(), pp):
+            # paths may have attributes in them, but the skip dictionary does
+            # not, so we ensure that the object's absolute path is attribute
+            # free,
+            if "[" in i:
+                i = i.split("[")[0]
+            if not i == j:
+                match = False
+                break
+            trimmed_path.pop(0)
+
+        if match and len(trimmed_path):
+            tree = remove_path(tree, trimmed_path)
+
+    if select:
+        key_del = []
+        for t in tree:
+            keep = True
+            for k, v in six.iteritems(select):
+                v = six.text_type(v)
+                if mode == "default" or isinstance(tree, dict):
+                    if keep and not six.text_type(lookup_subdict(tree[t], k.split("."))) == v:
+                        keep = False
+                else:
+                    # handle ietf case where we have a list and might have namespaces
+                    if keep and not six.text_type(lookup_subdict(t, k.split("."))) == v:
+                        keep = False
+            if not keep:
+                key_del.append(t)
+        if mode == "default" or isinstance(tree, dict):
+            for k in key_del:
+                if mode == "default":
+                    del tree[k]
         else:
-          # handle ietf case where we have a list and might have namespaces
-          if (keep and not six.text_type(lookup_subdict(t, k.split("."))) == v):
-            keep = False
-      if not keep:
-        key_del.append(t)
-    if mode == 'default' or isinstance(tree, dict):
-      for k in key_del:
-        if mode == 'default':
-          del tree[k]
+            for i in key_del:
+                tree.remove(i)
+
+    if mode == "ietf":
+        cls = pybindIETFJSONEncoder
     else:
-      for i in key_del:
-        tree.remove(i)
+        cls = pybindJSONEncoder
+
+    return json.dumps(tree, cls=cls, indent=indent)
 
-  if mode == "ietf":
-    cls = pybindIETFJSONEncoder
-  else:
-    cls = pybindJSONEncoder
-
-  return json.dumps(tree, cls=cls, indent=indent)
-
-
-def dump(obj, fn, indent=4, filter=True, skip_subtrees=[],
-         mode="default"):
-  try:
-    fh = open(fn, 'w')
-  except IOError as m:
-    raise pybindJSONIOError("could not open file for writing: %s" % m)
-  fh.write(dumps(obj, indent=indent, filter=filter,
-              skip_subtrees=skip_subtrees, mode=mode))
-  fh.close()
+
+def dump(obj, fn, indent=4, filter=True, skip_subtrees=[], mode="default"):
+    try:
+        fh = open(fn, "w")
+    except IOError as m:
+        raise pybindJSONIOError("could not open file for writing: %s" % m)
+    fh.write(dumps(obj, indent=indent, filter=filter, skip_subtrees=skip_subtrees, mode=mode))
+    fh.close()
```

### Comparing `pyangbind-0.8.1/pyangbind/lib/xpathhelper.py` & `pyangbind-0.8.2/pyangbind/lib/xpathhelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,28 +33,29 @@
 from lxml import etree
 
 from .base import PybindBase
 from .yangtypes import safe_name
 
 
 class YANGPathHelperException(Exception):
-  pass
+    pass
 
 
 class XPathError(Exception):
-  pass
+    pass
 
 
 class PybindImplementationError(Exception):
-  pass
+    pass
 
 
 class PybindXpathHelper(object):
-  def register(self, path, object_ptr, caller=False):
-    """
+
+    def register(self, path, object_ptr, caller=False):
+        """
       A PybindXpathHelper class should supply a register() method that
       takes two mandatory arguments, and one optional.
 
       * path - the path to which the object should be registered. This is
         supplied as a list of the names of the elements of the path. For
         example, /device/interfaces/interface[name='eth0'] is supplied as
         a ["device", "interfaces", "interface[@name='eth0']"].
@@ -62,283 +63,275 @@
       * object_ptr - a reference to the object that is to be stored at this
         location in the tree.
 
       * caller=False - this supplies the path of the object that is currently
         trying to perform a register. In general, it will not be used, but it
         is supplied to facilitate relative path lookups.
     """
-    raise PybindImplementationError("The path helper class specified does " +
-                                    "not implement register()")
+        raise PybindImplementationError("The path helper class specified does " + "not implement register()")
 
-  def unregister(self, path, caller=False):
-    """
+    def unregister(self, path, caller=False):
+        """
       A PybindXpathHelper class should supply an unregister() method that
       takes one mandatory argument, and one optional.
 
       * path - the path of the object to be unregistered. Supplied as a list()
         object of the elements of the path.
 
       * caller=False - the absolute path of the object calling the unregister()
         method.
     """
-    raise PybindImplementationError("The path helper class specified does " +
-                                    "not implement unregister()")
+        raise PybindImplementationError("The path helper class specified does " + "not implement unregister()")
 
-  def get(self, path, caller=False):
-    """
+    def get(self, path, caller=False):
+        """
       A PybindXpathHelper class should supply a get() method that takes one
       mandatory argument and one optional.
 
       * path - the path to the object to be retrieved. This may be specified as
         a list of parts, or an XPATH expression.
 
       * caller=False - the absolute path of the object calling the get method.
     """
-    raise PybindImplementationError("The path helper class specified does " +
-                                    "not implement get()")
+        raise PybindImplementationError("The path helper class specified does " + "not implement get()")
 
 
 # A class which acts as "/" within the hierarchy - it acts as per any other
 # PyangBind element for the purposes of get() calls - allowing "/" to be
 # serialised to
 class FakeRoot(PybindBase):
-  _pybind_generated_by = "FakeRoot"
+    _pybind_generated_by = "FakeRoot"
 
-  def __init__(self):
-    self._pyangbind_elements = OrderedDict()
+    def __init__(self):
+        self._pyangbind_elements = OrderedDict()
 
 
 class YANGPathHelper(PybindXpathHelper):
-  _attr_re = regex.compile("^(?P<tagname>[^\[]+)(?P<args>(\[[^\]]+\])+)$")
-  _arg_re = regex.compile("^((and|or) )?[@]?(?P<cmd>[a-zA-Z0-9\-\_:]+)([ ]+)?" +
-                       "=([ ]+)?[\'\"]?(?P<arg>[^ ^\'^\"]+)([\'\"])?([ ]+)?" +
-                       "(?P<remainder>.*)")
-  _relative_path_re = regex.compile("^(\.|\.\.)")
-
-  def __init__(self):
-    # Initialise an empty library and a new FakeRoot class to act as the
-    # data tree's root.
-    self._root = etree.Element("root")
-    self._library = {}
-    self._library["root"] = FakeRoot()
-    self._root.set("obj_ptr", "root")
-
-  def _path_parts(self, path):
-    c = 0
-    parts = []
-    buf = ""
-    in_qstr, in_attr = False, False
-    while c < len(path):
-      if path[c] == "/" and not in_qstr and not in_attr:
-        parts.append(buf)
+    _attr_re = regex.compile("^(?P<tagname>[^\[]+)(?P<args>(\[[^\]]+\])+)$")
+    _arg_re = regex.compile(
+        "^((and|or) )?[@]?(?P<cmd>[a-zA-Z0-9\-\_:]+)([ ]+)?"
+        + "=([ ]+)?['\"]?(?P<arg>[^ ^'^\"]+)(['\"])?([ ]+)?"
+        + "(?P<remainder>.*)"
+    )
+    _relative_path_re = regex.compile("^(\.|\.\.)")
+
+    def __init__(self):
+        # Initialise an empty library and a new FakeRoot class to act as the
+        # data tree's root.
+        self._root = etree.Element("root")
+        self._library = {}
+        self._library["root"] = FakeRoot()
+        self._root.set("obj_ptr", "root")
+
+    def _path_parts(self, path):
+        c = 0
+        parts = []
         buf = ""
-      elif path[c] == '"' and in_qstr:
-        in_qstr = False
-        buf += path[c]
-      elif path[c] == '"':
-        in_qstr = True
-        buf += path[c]
-      elif path[c] == '[':
-        in_attr = True
-        buf += path[c]
-      elif path[c] == ']':
-        in_attr = False
-        buf += path[c]
-      else:
-        buf += path[c]
-      c += 1
-    parts.append(buf)
-    return parts
-
-  def _encode_path(self, path, mode="search", find_parent=False,
-                   normalise_namespace=True, caller=False):
-    if mode not in ["search", "set"]:
-      raise XPathError("Path can only be encoded based on searching or " +
-                       "setting attributes")
-
-    parts = path
-    if len(parts) == 0:
-      return "/"
-    elif find_parent and len(parts) == 1:
-      return []
-
-    lastelem = len(parts) - 1 if find_parent else len(parts)
-    startelem = 1 if parts[0] == '' else 0
-    if self._relative_path_re.match(parts[0]):
-      epath = ""
-    else:
-      epath = "/"
-    for i in range(startelem, lastelem):
-      (tagname, attributes) = self._tagname_attributes(parts[i],
-                                    normalise_namespace=normalise_namespace)
-      if ":" in tagname and normalise_namespace:
-        tagname = tagname.split(":")[1]
-
-      if attributes is not None:
-        epath += tagname + "["
-        for k, v in six.iteritems(attributes):
-          # handling for rfc6020 current() specification
-          if "current()" in v:
-            remaining_path = regex.sub("current\(\)(?P<remaining>.*)",
-                                      '\g<remaining>', v).split("/")
-            # since the calling leaf may not exist, we need to do a
-            # lookup on a path that will do, which is the parent
-            if remaining_path[1] == "..":
-              lookup = caller[:-1] + remaining_path[2:]
+        in_qstr, in_attr = False, False
+        while c < len(path):
+            if path[c] == "/" and not in_qstr and not in_attr:
+                parts.append(buf)
+                buf = ""
+            elif path[c] == '"' and in_qstr:
+                in_qstr = False
+                buf += path[c]
+            elif path[c] == '"':
+                in_qstr = True
+                buf += path[c]
+            elif path[c] == "[":
+                in_attr = True
+                buf += path[c]
+            elif path[c] == "]":
+                in_attr = False
+                buf += path[c]
+            else:
+                buf += path[c]
+            c += 1
+        parts.append(buf)
+        return parts
+
+    def _encode_path(self, path, mode="search", find_parent=False, normalise_namespace=True, caller=False):
+        if mode not in ["search", "set"]:
+            raise XPathError("Path can only be encoded based on searching or " + "setting attributes")
+
+        parts = path
+        if len(parts) == 0:
+            return "/"
+        elif find_parent and len(parts) == 1:
+            return []
+
+        lastelem = len(parts) - 1 if find_parent else len(parts)
+        startelem = 1 if parts[0] == "" else 0
+        if self._relative_path_re.match(parts[0]):
+            epath = ""
+        else:
+            epath = "/"
+        for i in range(startelem, lastelem):
+            (tagname, attributes) = self._tagname_attributes(parts[i], normalise_namespace=normalise_namespace)
+            if ":" in tagname and normalise_namespace:
+                tagname = tagname.split(":")[1]
+
+            if attributes is not None:
+                epath += tagname + "["
+                for k, v in six.iteritems(attributes):
+                    # handling for rfc6020 current() specification
+                    if "current()" in v:
+                        remaining_path = regex.sub("current\(\)(?P<remaining>.*)", "\g<remaining>", v).split("/")
+                        # since the calling leaf may not exist, we need to do a
+                        # lookup on a path that will do, which is the parent
+                        if remaining_path[1] == "..":
+                            lookup = caller[:-1] + remaining_path[2:]
+                        else:
+                            lookup = caller + remaining_path[1:]
+                        resolved_current_attr = self.get(lookup)
+                        if not len(resolved_current_attr) == 1:
+                            raise XPathError(
+                                "XPATH specified a current() expression that " + "returned a non-unique list"
+                            )
+                        v = resolved_current_attr[0]
+                    epath += "@%s='%s' " % (k, v)
+                    if mode == "search":
+                        epath += "and "
+                if mode == "search":
+                    epath = epath.rstrip("and ")
+                epath = epath.rstrip(" ") + "]"
+                epath += "/"
+            else:
+                epath += tagname + "/"
+        epath = epath.rstrip("/")
+        return epath
+
+    def _tagname_attributes(self, tag, normalise_namespace=True):
+        tagname, attributes = tag, None
+        if self._attr_re.match(tag):
+            tagname, args = self._attr_re.sub("\g<tagname>||\g<args>", tag).split("||")
+            arg_parts = [i.strip("[") for i in args.split("]")]
+
+            attributes = {}
+            for arg in arg_parts:
+                tmp_arg = arg
+                while len(tmp_arg):
+                    if self._arg_re.match(tmp_arg):
+                        c, a, r = self._arg_re.sub("\g<cmd>||\g<arg>||\g<remainder>", tmp_arg).split("||")
+                        if ":" in c and normalise_namespace:
+                            c = c.split(":")[1]
+                        attributes[c] = a
+                        tmp_arg = r
+                    else:
+                        raise XPathError(
+                            "invalid attribute string specified"
+                            + "for %s" % tagname
+                            + "(err part: %s (%s))" % (arg, tmp_arg)
+                        )
+        return (tagname, attributes)
+
+    def register(self, object_path, object_ptr, caller=False):
+        if isinstance(object_path, str):
+            raise XPathError("not meant to receive strings as input to register()")
+
+        if regex.match("^\.\.", object_path[0]):
+            raise XPathError("unhandled relative path in register()")
+
+        # This is a hack to register anything that is a top-level object,
+        # it allows modules to register themselves against the FakeRoot
+        # class which acts as per other PyangBind objects.
+        if len(object_path) == 1:
+            setattr(self._library["root"], object_path[0], object_ptr)
+            setattr(self._library["root"], "_get_%s" % safe_name(object_path[0]), lambda: object_ptr)
+            self._library["root"]._pyangbind_elements[object_path[0]] = None
+
+        # check whether we're updating
+        this_obj_existing = self._get_etree(object_path)
+        if len(this_obj_existing) > 1:
+            raise XPathError("duplicate objects in tree - %s" % object_path)
+        if this_obj_existing is not None and not this_obj_existing == []:
+            this_obj_existing = this_obj_existing[0]
+            if self._library[this_obj_existing.get("obj_ptr")] == object_ptr:
+                return True
             else:
-              lookup = caller + remaining_path[1:]
-            resolved_current_attr = self.get(lookup)
-            if not len(resolved_current_attr) == 1:
-              raise XPathError('XPATH specified a current() expression that ' +
-                                'returned a non-unique list')
-            v = resolved_current_attr[0]
-          epath += "@%s='%s' " % (k, v)
-          if mode == "search":
-            epath += "and "
-        if mode == "search":
-          epath = epath.rstrip("and ")
-        epath = epath.rstrip(" ") + "]"
-        epath += "/"
-      else:
-        epath += tagname + "/"
-    epath = epath.rstrip("/")
-    return epath
-
-  def _tagname_attributes(self, tag, normalise_namespace=True):
-    tagname, attributes = tag, None
-    if self._attr_re.match(tag):
-      tagname, args = self._attr_re.sub('\g<tagname>||\g<args>',
-                                        tag).split("||")
-      arg_parts = [i.strip("[") for i in args.split("]")]
-
-      attributes = {}
-      for arg in arg_parts:
-        tmp_arg = arg
-        while len(tmp_arg):
-          if self._arg_re.match(tmp_arg):
-            c, a, r = self._arg_re.sub('\g<cmd>||\g<arg>||\g<remainder>',
-                                        tmp_arg).split("||")
-            if ":" in c and normalise_namespace:
-              c = c.split(":")[1]
-            attributes[c] = a
-            tmp_arg = r
-          else:
-            raise XPathError("invalid attribute string specified" +
-                             "for %s" % tagname +
-                             "(err part: %s (%s))" % (arg, tmp_arg))
-    return (tagname, attributes)
-
-  def register(self, object_path, object_ptr, caller=False):
-    if isinstance(object_path, str):
-      raise XPathError("not meant to receive strings as input to register()")
-
-    if regex.match('^\.\.', object_path[0]):
-      raise XPathError("unhandled relative path in register()")
-
-    # This is a hack to register anything that is a top-level object,
-    # it allows modules to register themselves against the FakeRoot
-    # class which acts as per other PyangBind objects.
-    if len(object_path) == 1:
-      setattr(self._library["root"], object_path[0], object_ptr)
-      setattr(self._library["root"], "_get_%s" % safe_name(object_path[0]), lambda: object_ptr)
-      self._library["root"]._pyangbind_elements[object_path[0]] = None
-
-    # check whether we're updating
-    this_obj_existing = self._get_etree(object_path)
-    if len(this_obj_existing) > 1:
-      raise XPathError("duplicate objects in tree - %s" % object_path)
-    if this_obj_existing is not None and not this_obj_existing == []:
-      this_obj_existing = this_obj_existing[0]
-      if self._library[this_obj_existing.get("obj_ptr")] == object_ptr:
-        return True
-      else:
-        del self._library[this_obj_existing.get("obj_ptr")]
-        new_uuid = str(uuid.uuid1())
-        self._library[new_uuid] = object_ptr
-        this_obj_existing.set("obj_ptr", new_uuid)
-        return True
-
-    this_obj_id = str(uuid.uuid1())
-    self._library[this_obj_id] = object_ptr
-    parent = object_path[:-1]
-    (tagname, attributes) = self._tagname_attributes(object_path[-1])
-
-    if parent == []:
-      parent_o = self._root
-    else:
-      parent_o = self._get_etree(parent)
-      if len(parent_o) > 1:
-        raise XPathError("multiple elements returned for parent %s, must be " +
-                          "exact path for registration" % "/" +
-                          "/".join(parent))
-      if parent_o == []:
-        raise XPathError("parent node did not exist for %s @ %s" % (tagname,
-                                    "/" + "/".join(parent)))
-      parent_o = parent_o[0]
-
-    added_item = etree.SubElement(parent_o, tagname, obj_ptr=this_obj_id)
-    if attributes is not None:
-      for k, v in six.iteritems(attributes):
-        added_item.set(k, v)
-
-  def unregister(self, object_path, caller=False):
-    if isinstance(object_path, str):
-      raise XPathError("should not receive paths as a str in unregister()")
-    if regex.match("^(\.|\.\.|\/)", object_path[0]):
-      raise XPathError("unhandled relative path in unregister()")
-
-    existing_objs = self._get_etree(object_path)
-    if len(existing_objs) == 0:
-      raise XPathError("object did not exist to unregister - %s" % object_path)
-
-    for obj in existing_objs:
-      ref = obj.get("obj_ptr")
-      del self._library[ref]
-      obj.getparent().remove(obj)
-
-  def _get_etree(self, object_path, caller=False):
-    fx_q = self._encode_path(object_path, caller=caller)
-    if self._relative_path_re.match(fx_q) and caller:
-      fx_q = "." + self._encode_path(caller)
-      fx_q += "/" + self._encode_path(object_path, caller=caller)
-    else:
-      if not fx_q == "/":
-        fx_q = "." + fx_q
-
-    retr_obj = self._root.xpath(fx_q)
-    return retr_obj
-
-  def get(self, object_path, caller=False):
-    if isinstance(object_path, six.string_types + (six.text_type,)):
-      object_path = self._path_parts(object_path)
-
-    return [self._library[i.get("obj_ptr")]
-              for i in self._get_etree(object_path, caller=caller)]
-
-  def get_unique(self, object_path, caller=False,
-                  exception_to_raise=YANGPathHelperException):
-    obj = self.get(object_path, caller=caller)
-    if len(obj) == 0:
-      raise exception_to_raise("Supplied path for %s found no results!"
-                                  % object_path)
-    if len(obj) != 1:
-      raise exception_to_raise("Supplied path for %s was not unique!"
-                                  % object_path)
-    return obj[0]
-
-  def get_list(self, object_path, caller=False,
-                exception_to_raise=YANGPathHelperException):
-    if isinstance(object_path, six.string_types + (six.text_type,)):
-      object_path = self._path_parts(object_path)
-
-    parent_obj = self.get_unique(object_path[:-1], caller=caller,
-                    exception_to_raise=exception_to_raise)
-
-    list_get_attr = getattr(parent_obj, "_get_%s" % safe_name(object_path[-1]), None)
-    if list_get_attr is None:
-      raise exception_to_raise("Element %s does not have an attribute named %s" %
-        ("/".join(object_path[:-1]), object_path[-1]))
+                del self._library[this_obj_existing.get("obj_ptr")]
+                new_uuid = str(uuid.uuid1())
+                self._library[new_uuid] = object_ptr
+                this_obj_existing.set("obj_ptr", new_uuid)
+                return True
+
+        this_obj_id = str(uuid.uuid1())
+        self._library[this_obj_id] = object_ptr
+        parent = object_path[:-1]
+        (tagname, attributes) = self._tagname_attributes(object_path[-1])
+
+        if parent == []:
+            parent_o = self._root
+        else:
+            parent_o = self._get_etree(parent)
+            if len(parent_o) > 1:
+                raise XPathError(
+                    "multiple elements returned for parent %s, must be "
+                    + "exact path for registration" % "/"
+                    + "/".join(parent)
+                )
+            if parent_o == []:
+                raise XPathError("parent node did not exist for %s @ %s" % (tagname, "/" + "/".join(parent)))
+            parent_o = parent_o[0]
+
+        added_item = etree.SubElement(parent_o, tagname, obj_ptr=this_obj_id)
+        if attributes is not None:
+            for k, v in six.iteritems(attributes):
+                added_item.set(k, v)
+
+    def unregister(self, object_path, caller=False):
+        if isinstance(object_path, str):
+            raise XPathError("should not receive paths as a str in unregister()")
+        if regex.match("^(\.|\.\.|\/)", object_path[0]):
+            raise XPathError("unhandled relative path in unregister()")
+
+        existing_objs = self._get_etree(object_path)
+        if len(existing_objs) == 0:
+            raise XPathError("object did not exist to unregister - %s" % object_path)
+
+        for obj in existing_objs:
+            ref = obj.get("obj_ptr")
+            del self._library[ref]
+            obj.getparent().remove(obj)
+
+    def _get_etree(self, object_path, caller=False):
+        fx_q = self._encode_path(object_path, caller=caller)
+        if self._relative_path_re.match(fx_q) and caller:
+            fx_q = "." + self._encode_path(caller)
+            fx_q += "/" + self._encode_path(object_path, caller=caller)
+        else:
+            if not fx_q == "/":
+                fx_q = "." + fx_q
+
+        retr_obj = self._root.xpath(fx_q)
+        return retr_obj
+
+    def get(self, object_path, caller=False):
+        if isinstance(object_path, six.string_types + (six.text_type,)):
+            object_path = self._path_parts(object_path)
+
+        return [self._library[i.get("obj_ptr")] for i in self._get_etree(object_path, caller=caller)]
+
+    def get_unique(self, object_path, caller=False, exception_to_raise=YANGPathHelperException):
+        obj = self.get(object_path, caller=caller)
+        if len(obj) == 0:
+            raise exception_to_raise("Supplied path for %s found no results!" % object_path)
+        if len(obj) != 1:
+            raise exception_to_raise("Supplied path for %s was not unique!" % object_path)
+        return obj[0]
+
+    def get_list(self, object_path, caller=False, exception_to_raise=YANGPathHelperException):
+        if isinstance(object_path, six.string_types + (six.text_type,)):
+            object_path = self._path_parts(object_path)
+
+        parent_obj = self.get_unique(object_path[:-1], caller=caller, exception_to_raise=exception_to_raise)
+
+        list_get_attr = getattr(parent_obj, "_get_%s" % safe_name(object_path[-1]), None)
+        if list_get_attr is None:
+            raise exception_to_raise(
+                "Element %s does not have an attribute named %s" % ("/".join(object_path[:-1]), object_path[-1])
+            )
 
-    return list_get_attr()
+        return list_get_attr()
 
-  def tostring(self, pretty_print=False):
-    return etree.tostring(self._root, pretty_print=pretty_print)
+    def tostring(self, pretty_print=False):
+        return etree.tostring(self._root, pretty_print=pretty_print)
```

### Comparing `pyangbind-0.8.1/pyangbind/lib/yangtypes.py` & `pyangbind-0.8.2/pyangbind/lib/yangtypes.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,846 +18,902 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from __future__ import unicode_literals
 
 import collections
+from collections import abc
 import copy
 import uuid
 from decimal import Decimal
 
 import regex
 import six
 from bitarray import bitarray
 
 # Words that could turn up in YANG definition files that are actually
 # reserved names in Python, such as being builtin types. This list is
 # not complete, but will probably continue to grow.
-reserved_name = ["list", "str", "int", "global", "decimal", "float",
-                  "as", "if", "else", "elif", "map", "set", "class",
-                  "from", "import", "pass", "return", "is", "exec",
-                  "pop", "insert", "remove", "add", "delete", "local",
-                  "get", "default", "yang_name", "def", "print", "del",
-                  "break", "continue", "raise", "in", "assert", "while",
-                  "for", "try", "finally", "with", "except", "lambda",
-                  "or", "and", "not", "yield", "property", "min", "max"]
+reserved_name = [
+    "list",
+    "str",
+    "int",
+    "global",
+    "decimal",
+    "float",
+    "as",
+    "if",
+    "else",
+    "elif",
+    "map",
+    "set",
+    "class",
+    "from",
+    "import",
+    "pass",
+    "return",
+    "is",
+    "exec",
+    "pop",
+    "insert",
+    "remove",
+    "add",
+    "delete",
+    "local",
+    "get",
+    "default",
+    "yang_name",
+    "def",
+    "print",
+    "del",
+    "break",
+    "continue",
+    "raise",
+    "in",
+    "assert",
+    "while",
+    "for",
+    "try",
+    "finally",
+    "with",
+    "except",
+    "lambda",
+    "or",
+    "and",
+    "not",
+    "yield",
+    "property",
+    "min",
+    "max",
+]
 
 
 def is_yang_list(arg):
-  if isinstance(arg, list):
-    return True
-  elif hasattr(arg, "_pybind_generated_by"):
-    pygen = getattr(arg, "_pybind_generated_by")
-    if pygen in ["TypedListType", "YANGListType"]:
-      return True
-  return False
+    if isinstance(arg, list):
+        return True
+    elif hasattr(arg, "_pybind_generated_by"):
+        pygen = getattr(arg, "_pybind_generated_by")
+        if pygen in ["TypedListType", "YANGListType"]:
+            return True
+    return False
 
 
 def is_yang_leaflist(arg):
-  pygen = getattr(arg, "_pybind_generated_by", None)
-  if pygen is None:
+    pygen = getattr(arg, "_pybind_generated_by", None)
+    if pygen is None:
+        return False
+    elif pygen == "TypedListType":
+        return True
     return False
-  elif pygen == "TypedListType":
-    return True
-  return False
 
 
 def remove_path_attributes(p):
-  new_path = []
-  for i in p:
-    if "[" in i:
-      new_path.append(i.split("[")[0])
-    else:
-      new_path.append(i)
-  return new_path
+    new_path = []
+    for i in p:
+        if "[" in i:
+            new_path.append(i.split("[")[0])
+        else:
+            new_path.append(i)
+    return new_path
 
 
 def safe_name(arg):
-  """
+    """
     Make a leaf or container name safe for use in Python.
   """
-  arg = arg.replace("-", "_")
-  arg = arg.replace(".", "_")
-  if arg in reserved_name:
-    arg += "_"
-  # store the unsafe->original version mapping
-  # so that we can retrieve it when get() is called.
-  return arg
+    arg = arg.replace("-", "_")
+    arg = arg.replace(".", "_")
+    if arg in reserved_name:
+        arg += "_"
+    # store the unsafe->original version mapping
+    # so that we can retrieve it when get() is called.
+    return arg
 
 
 def RestrictedPrecisionDecimalType(*args, **kwargs):
-  """
+    """
     Function to return a new type that is based on decimal.Decimal with
     an arbitrary restricted precision.
   """
-  precision = kwargs.pop("precision", False)
+    precision = kwargs.pop("precision", False)
 
-  class RestrictedPrecisionDecimal(Decimal):
-    """
+    class RestrictedPrecisionDecimal(Decimal):
+        """
       Class extending decimal.Decimal to restrict the precision that is
       stored, supporting the fraction-digits argument of the YANG decimal64
       type.
     """
-    _precision = 10.0**(-1.0 * int(precision))
-    _pybind_generated_by = 'RestrictedPrecisionDecimal'
+        _precision = 10.0 ** (-1.0 * int(precision))
+        _pybind_generated_by = "RestrictedPrecisionDecimal"
 
-    def __new__(self, *args, **kwargs):
-      """
+        def __new__(self, *args, **kwargs):
+            """
         Overloads the decimal __new__ function in order to round the input
         value to the new value.
       """
-      if self._precision is not None:
-        if len(args):
-          value = Decimal(args[0]).quantize(Decimal(str(self._precision)))
-        else:
-          value = Decimal(0)
-      elif len(args):
-        value = Decimal(args[0])
-      else:
-        value = Decimal(0)
-      obj = Decimal.__new__(self, value, **kwargs)
-      return obj
-  return type(RestrictedPrecisionDecimal(*args, **kwargs))
+            if self._precision is not None:
+                if len(args):
+                    value = Decimal(args[0]).quantize(Decimal(str(self._precision)))
+                else:
+                    value = Decimal(0)
+            elif len(args):
+                value = Decimal(args[0])
+            else:
+                value = Decimal(0)
+            obj = Decimal.__new__(self, value, **kwargs)
+            return obj
+
+    return type(RestrictedPrecisionDecimal(*args, **kwargs))
 
 
 def RestrictedClassType(*args, **kwargs):
-  """
+    """
     Function to return a new type that restricts an arbitrary base_type with
     a specified restriction. The restriction_type specified determines the
     type of restriction placed on the class, and the restriction_arg gives
     any input data that this function needs.
   """
-  base_type = kwargs.pop("base_type", six.text_type)
-  restriction_type = kwargs.pop("restriction_type", None)
-  restriction_arg = kwargs.pop("restriction_arg", None)
-  restriction_dict = kwargs.pop("restriction_dict", None)
-  int_size = kwargs.pop("int_size", None)
-
-  # this gives deserialisers some hints as to how to encode/decode this value
-  # it must be a list since a restricted class can encapsulate a restricted
-  # class
-  current_restricted_class_type = regex.sub("<(type|class) '(?P<class>.*)'>",
-                                          "\g<class>", six.text_type(base_type))
-  if hasattr(base_type, "_restricted_class_base"):
-    restricted_class_hint = getattr(base_type, "_restricted_class_base")
-    restricted_class_hint.append(current_restricted_class_type)
-  else:
-    restricted_class_hint = [current_restricted_class_type]
+    base_type = kwargs.pop("base_type", six.text_type)
+    restriction_type = kwargs.pop("restriction_type", None)
+    restriction_arg = kwargs.pop("restriction_arg", None)
+    restriction_dict = kwargs.pop("restriction_dict", None)
+    int_size = kwargs.pop("int_size", None)
+
+    # this gives deserialisers some hints as to how to encode/decode this value
+    # it must be a list since a restricted class can encapsulate a restricted
+    # class
+    current_restricted_class_type = regex.sub("<(type|class) '(?P<class>.*)'>", "\g<class>", six.text_type(base_type))
+    if hasattr(base_type, "_restricted_class_base"):
+        restricted_class_hint = getattr(base_type, "_restricted_class_base")
+        restricted_class_hint.append(current_restricted_class_type)
+    else:
+        restricted_class_hint = [current_restricted_class_type]
 
-  class RestrictedClass(base_type):
-    """
+    class RestrictedClass(base_type):
+        """
       A class that restricts the base_type class with a new function that the
       input value is validated against before being applied. The function is
       a static method which is assigned to _restricted_test.
     """
-    _pybind_generated_by = "RestrictedClassType"
+        _pybind_generated_by = "RestrictedClassType"
 
-    _restricted_class_base = restricted_class_hint
-    _restricted_int_size = int_size
+        _restricted_class_base = restricted_class_hint
+        _restricted_int_size = int_size
 
-    def __init__(self, *args, **kwargs):
-      """
+        def __init__(self, *args, **kwargs):
+            """
         Overloads the base_class __init__ method to check the input argument
         against the validation function - returns on instance of the base_type
         class, which can be manipulated as per a usual Python object.
       """
-      try:
-        self.__check(args[0])
-      except IndexError:
-        pass
-      try:
-        super(RestrictedClass, self).__init__(*args, **kwargs)
-      except TypeError:
-        super(RestrictedClass, self).__init__()
-
-    def __new__(self, *args, **kwargs):
-      self._restriction_dict = restriction_dict
-      self._restriction_tests = []
+            try:
+                self.__check(args[0])
+            except IndexError:
+                pass
+            try:
+                super(RestrictedClass, self).__init__(*args, **kwargs)
+            except TypeError:
+                super(RestrictedClass, self).__init__()
+
+        def __new__(self, *args, **kwargs):
+            self._restriction_dict = restriction_dict
+            self._restriction_tests = []
 
-      """
+            """
         Create a new class instance, and dynamically define the
         _restriction_test method so that it can be called by other functions.
       """
 
-      range_regex = regex.compile("(?P<low>\-?[0-9\.]+|min)([ ]+)?\.\.([ ]+)?" +
-                                "(?P<high>(\-?[0-9\.]+|max))")
-      range_single_value_regex = regex.compile("(?P<value>\-?[0-9\.]+)")
-
-      def convert_regexp(pattern):
-
-        # Some patterns include a $ character in them in some IANA modules, this
-        # is not escaped. Do some logic to escape them, whilst leaving one at the
-        # end of the string if it's there.
-        trimmed = False
-        if pattern[-1] == "$":
-          tmp_pattern = pattern[:-1]
-          trimmed = True
-        else:
-          tmp_pattern = pattern
-        tmp_pattern = tmp_pattern.replace("$", "\$")
-        pattern = tmp_pattern
-        if trimmed:
-          pattern += "$"
-
-        if not pattern[0] == "^":
-          pattern = "^%s" % pattern
-        if not pattern[len(pattern) - 1] == "$":
-          pattern = "%s$" % pattern
-
-        return pattern
-
-      def build_length_range_tuples(range, length=False, multiplier=1):
-        if range_regex.match(range_spec):
-          low, high = \
-              range_regex.sub("\g<low>,\g<high>", range_spec).split(",")
-          if not length:
-            high = base_type(high) if not high == "max" else None
-            low = base_type(low) if not low == "min" else None
-          else:
-            high = int(high) * multiplier if not high == "max" else None
-            low = int(low) * multiplier if not low == "min" else None
-          return (low, high)
-        elif range_single_value_regex.match(range_spec):
-          eqval = range_single_value_regex.sub('\g<value>', range_spec)
-          if not length:
-            eqval = base_type(eqval) if eqval not in ["max", "min"] else None
-          else:
-            eqval = int(eqval) * multiplier
-          return (eqval,)
-        else:
-          raise ValueError("Invalid range or length argument specified")
+            range_regex = regex.compile("(?P<low>\-?[0-9\.]+|min)([ ]+)?\.\.([ ]+)?" + "(?P<high>(\-?[0-9\.]+|max))")
+            range_single_value_regex = regex.compile("(?P<value>\-?[0-9\.]+)")
 
-      def in_range_check(low_high_tuples, length=False):
-        def range_check(value):
-          if length and isinstance(value, bitarray):
-            value = value.length()
-          elif length:
-            value = len(value)
-          range_results = []
-          for check_tuple in low_high_tuples:
-            chk = True
-            if len(check_tuple) == 2:
-              if check_tuple[0] is not None and value < check_tuple[0]:
-                chk = False
-              if check_tuple[1] is not None and value > check_tuple[1]:
-                chk = False
-            elif len(check_tuple) == 1:
-              if value != float(check_tuple[0]):
-                chk = False
-            else:
-              raise AttributeError("Invalid check tuple length specified")
-            range_results.append(chk)
-          return True in range_results
-        return range_check
-
-      def match_pattern_check(regexp):
-        def mp_check(value):
-          if not isinstance(value, six.string_types + (six.text_type,)):
-            return False
-          if regex.match(convert_regexp(regexp), value):
-            return True
-          return False
-        return mp_check
+            def convert_regexp(pattern):
 
-      def in_dictionary_check(dictionary):
-        return lambda i: six.text_type(i) in dictionary
+                # Some patterns include a $ character in them in some IANA modules, this
+                # is not escaped. Do some logic to escape them, whilst leaving one at the
+                # end of the string if it's there.
+                trimmed = False
+                if pattern[-1] == "$":
+                    tmp_pattern = pattern[:-1]
+                    trimmed = True
+                else:
+                    tmp_pattern = pattern
+                tmp_pattern = tmp_pattern.replace("$", "\$")
+                pattern = tmp_pattern
+                if trimmed:
+                    pattern += "$"
+
+                if not pattern[0] == "^":
+                    pattern = "^%s" % pattern
+                if not pattern[len(pattern) - 1] == "$":
+                    pattern = "%s$" % pattern
+
+                return pattern
+
+            def build_length_range_tuples(range, length=False, multiplier=1):
+                if range_regex.match(range_spec):
+                    low, high = range_regex.sub("\g<low>,\g<high>", range_spec).split(",")
+                    if not length:
+                        high = base_type(high) if not high == "max" else None
+                        low = base_type(low) if not low == "min" else None
+                    else:
+                        high = int(high) * multiplier if not high == "max" else None
+                        low = int(low) * multiplier if not low == "min" else None
+                    return (low, high)
+                elif range_single_value_regex.match(range_spec):
+                    eqval = range_single_value_regex.sub("\g<value>", range_spec)
+                    if not length:
+                        eqval = base_type(eqval) if eqval not in ["max", "min"] else None
+                    else:
+                        eqval = int(eqval) * multiplier
+                    return (eqval,)
+                else:
+                    raise ValueError("Invalid range or length argument specified")
+
+            def in_range_check(low_high_tuples, length=False):
+
+                def range_check(value):
+                    if length and isinstance(value, bitarray):
+                        value = value.length()
+                    elif length:
+                        value = len(value)
+                    range_results = []
+                    for check_tuple in low_high_tuples:
+                        chk = True
+                        if len(check_tuple) == 2:
+                            if check_tuple[0] is not None and value < check_tuple[0]:
+                                chk = False
+                            if check_tuple[1] is not None and value > check_tuple[1]:
+                                chk = False
+                        elif len(check_tuple) == 1:
+                            if value != float(check_tuple[0]):
+                                chk = False
+                        else:
+                            raise AttributeError("Invalid check tuple length specified")
+                        range_results.append(chk)
+                    return True in range_results
+
+                return range_check
+
+            def match_pattern_check(regexp):
+
+                def mp_check(value):
+                    if not isinstance(value, six.string_types + (six.text_type,)):
+                        return False
+                    if regex.match(convert_regexp(regexp), value):
+                        return True
+                    return False
 
-      val = False
-      try:
-        val = args[0]
-      except IndexError:
-        pass
-      if self._restriction_dict is None:
-        if restriction_type is not None and restriction_arg is not None:
-          self._restriction_dict = {restriction_type: restriction_arg}
-        else:
-          raise ValueError("must specify either a restriction dictionary or" +
-                            " a type and argument")
+                return mp_check
 
-      for rtype, rarg in self._restriction_dict.items():
-        if rtype == "pattern":
-          self._restriction_tests.append(match_pattern_check(rarg))
-        elif rtype == "range":
-          ranges = []
-          for range_spec in rarg:
-            ranges.append(build_length_range_tuples(range_spec))
-          self._restriction_tests.append(in_range_check(ranges))
-          if val:
+            def in_dictionary_check(dictionary):
+                return lambda i: six.text_type(i) in dictionary
+
+            val = False
             try:
-              val = base_type(val)
-            except Exception:
-              raise TypeError("must specify a numeric type for a range " +
-                                  "argument")
-        elif rtype == "length":
-          # When the type is a binary then the length is specified in
-          # octets rather than bits, so we must specify the length to
-          # be multiplied by 8.
-          multiplier = 1
-          if base_type == bitarray:
-            multiplier = 8
-          lengths = []
-          for range_spec in rarg:
-            lengths.append(build_length_range_tuples(range_spec, length=True,
-                                                    multiplier=multiplier))
-          self._restriction_tests.append(in_range_check(lengths, length=True))
-        elif rtype == "dict_key":
-          new_rarg = copy.deepcopy(rarg)
-          for k in rarg:
-            if k.startswith("@"):
-              new_rarg.pop(k, None)
-          # populate enum values
-          used_values = []
-          for k in new_rarg:
-            if "value" in new_rarg[k]:
-              used_values.append(int(new_rarg[k]["value"]))
-          c = 0
-          for k in new_rarg:
-            while c in used_values:
-              c += 1
-            if "value" not in new_rarg[k]:
-              new_rarg[k]["value"] = c
-            c += 1
-          self._restriction_tests.append(in_dictionary_check(new_rarg))
-          self._enumeration_dict = new_rarg
-        else:
-          raise TypeError("unsupported restriction type")
+                val = args[0]
+            except IndexError:
+                pass
+            if self._restriction_dict is None:
+                if restriction_type is not None and restriction_arg is not None:
+                    self._restriction_dict = {restriction_type: restriction_arg}
+                else:
+                    raise ValueError("must specify either a restriction dictionary or" + " a type and argument")
+
+            for rtype, rarg in self._restriction_dict.items():
+                if rtype == "pattern":
+                    self._restriction_tests.append(match_pattern_check(rarg))
+                elif rtype == "range":
+                    ranges = []
+                    for range_spec in rarg:
+                        ranges.append(build_length_range_tuples(range_spec))
+                    self._restriction_tests.append(in_range_check(ranges))
+                    if val:
+                        try:
+                            val = base_type(val)
+                        except Exception:
+                            raise TypeError("must specify a numeric type for a range " + "argument")
+                elif rtype == "length":
+                    # When the type is a binary then the length is specified in
+                    # octets rather than bits, so we must specify the length to
+                    # be multiplied by 8.
+                    multiplier = 1
+                    if base_type == bitarray:
+                        multiplier = 8
+                    lengths = []
+                    for range_spec in rarg:
+                        lengths.append(build_length_range_tuples(range_spec, length=True, multiplier=multiplier))
+                    self._restriction_tests.append(in_range_check(lengths, length=True))
+                elif rtype == "dict_key":
+                    new_rarg = copy.deepcopy(rarg)
+                    for k in rarg:
+                        if k.startswith("@"):
+                            new_rarg.pop(k, None)
+                    # populate enum values
+                    used_values = []
+                    for k in new_rarg:
+                        if "value" in new_rarg[k]:
+                            used_values.append(int(new_rarg[k]["value"]))
+                    c = 0
+                    for k in new_rarg:
+                        while c in used_values:
+                            c += 1
+                        if "value" not in new_rarg[k]:
+                            new_rarg[k]["value"] = c
+                        c += 1
+                    self._restriction_tests.append(in_dictionary_check(new_rarg))
+                    self._enumeration_dict = new_rarg
+                else:
+                    raise TypeError("unsupported restriction type")
+
+            if val is not False:
+                for test in self._restriction_tests:
+                    passed = False
+                    if test(val) is not False:
+                        passed = True
+                        break
+                if not passed:
+                    raise ValueError("%s does not match a restricted type" % val)
 
-      if val is not False:
-        for test in self._restriction_tests:
-          passed = False
-          if test(val) is not False:
-            passed = True
-            break
-        if not passed:
-          raise ValueError("%s does not match a restricted type" % val)
-
-      try:
-        obj = base_type.__new__(self, *args, **kwargs)
-      except TypeError:
-        obj = base_type.__new__(self)
-      return obj
+            try:
+                obj = base_type.__new__(self, *args, **kwargs)
+            except TypeError:
+                obj = base_type.__new__(self)
+            return obj
 
-    def __check(self, v):
-      """
+        def __check(self, v):
+            """
         Run the _restriction_test static method against the argument v,
         returning an error if the value does not validate.
       """
-      v = base_type(v)
-      for chkfn in self._restriction_tests:
-        if not chkfn(v):
-          raise ValueError("did not match restricted type")
-      return True
+            v = base_type(v)
+            for chkfn in self._restriction_tests:
+                if not chkfn(v):
+                    raise ValueError("did not match restricted type")
+            return True
 
-    def getValue(self, *args, **kwargs):
-      """
+        def getValue(self, *args, **kwargs):
+            """
         For types where there is a dict_key restriction (such as YANG
         enumeration), return the value of the dictionary key.
       """
-      if "dict_key" in self._restriction_dict:
-        value = kwargs.pop("mapped", False)
-        if value:
-          return self._enumeration_dict[self.__str__()]["value"]
-      return self
+            if "dict_key" in self._restriction_dict:
+                value = kwargs.pop("mapped", False)
+                if value:
+                    return self._enumeration_dict[self.__str__()]["value"]
+            return self
 
-  return type(RestrictedClass(*args, **kwargs))
+    return type(RestrictedClass(*args, **kwargs))
 
 
 def TypedListType(*args, **kwargs):
-  """
+    """
     Return a type that consists of a list object where only
     certain types (specified by allowed_type kwarg to the function)
     can be added to the list.
   """
-  allowed_type = kwargs.pop("allowed_type", six.text_type)
-  if not isinstance(allowed_type, list):
-    allowed_type = [allowed_type]
-
-  class TypedList(collections.MutableSequence):
-    _pybind_generated_by = "TypedListType"
-    _list = list()
-
-    def __init__(self, *args, **kwargs):
-      self._unique = kwargs.pop('unique', False)
-      self._allowed_type = allowed_type
-      self._list = list()
-      if len(args):
-        if isinstance(args[0], list):
-          tmp = []
-          for i in args[0]:
-            if not self._unique or i not in tmp:
-              tmp.append(self.check(i))
-          self._list.extend(tmp)
-        else:
-          tmp = self.check(args[0])
-          self._list.append(tmp)
+    allowed_type = kwargs.pop("allowed_type", six.text_type)
+    if not isinstance(allowed_type, list):
+        allowed_type = [allowed_type]
+
+    class TypedList(abc.MutableSequence):
+        _pybind_generated_by = "TypedListType"
+        _list = list()
+
+        def __init__(self, *args, **kwargs):
+            self._unique = kwargs.pop("unique", False)
+            self._allowed_type = allowed_type
+            self._list = list()
+            if len(args):
+                if isinstance(args[0], list):
+                    tmp = []
+                    for i in args[0]:
+                        if not self._unique or i not in tmp:
+                            tmp.append(self.check(i))
+                    self._list.extend(tmp)
+                else:
+                    tmp = self.check(args[0])
+                    self._list.append(tmp)
+
+        def check(self, v):
+            # Short circuit uniqueness check
+            if self._unique and v in self._list:
+                raise ValueError("Values in this list must be unique.")
+
+            passed = False
+            count = 0
+            for i in self._allowed_type:
+                if isinstance(v, i):
+                    tmp = v
+                    passed = True
+                    break
+                try:
+                    if hasattr(i, "_pybind_generated_by"):
+                        attr = getattr(i, "_pybind_generated_by")
+                        if attr == "RestrictedClassType":
+                            tmp = i(v)
+                            passed = True
+                            break
+                        elif attr == "ReferencePathType":
+                            tmp = i(v)
+                            passed = True
+                            break
+                        elif attr == "RestrictedPrecisionDecimal":
+                            tmp = i(v)
+                            passed = True
+                            break
+                    elif i == six.text_type and isinstance(v, six.string_types + (six.text_type,)):
+                        tmp = six.text_type(v)
+                        passed = True
+                        break
+                    elif i not in six.string_types + (six.text_type,):
+                        # for anything other than string we try
+                        # and cast. Using things for string or
+                        # unicode gives us strange results because we get
+                        # class name represetnations
+                        tmp = i(v)
+                        passed = True
+                        break
+                except Exception:
+                    # we catch all exceptions because we duck-type as
+                    # much as possible and some types - e.g., decimal do
+                    # not use builtins.
+                    pass
+                count += 1
+            if not passed:
+                raise ValueError("Cannot add %s to TypedList (accepts only %s)" % (v, self._allowed_type))
+            else:
+                return tmp
 
-    def check(self, v):
-      # Short circuit uniqueness check
-      if self._unique and v in self._list:
-        raise ValueError("Values in this list must be unique.")
-
-      passed = False
-      count = 0
-      for i in self._allowed_type:
-        if isinstance(v, i):
-          tmp = v
-          passed = True
-          break
-        try:
-          if hasattr(i, "_pybind_generated_by"):
-            attr = getattr(i, "_pybind_generated_by")
-            if attr == "RestrictedClassType":
-              tmp = i(v)
-              passed = True
-              break
-            elif attr == "ReferencePathType":
-              tmp = i(v)
-              passed = True
-              break
-            elif attr == "RestrictedPrecisionDecimal":
-              tmp = i(v)
-              passed = True
-              break
-          elif i == six.text_type and isinstance(v, six.string_types + (six.text_type,)):
-            tmp = six.text_type(v)
-            passed = True
-            break
-          elif i not in six.string_types + (six.text_type,):
-            # for anything other than string we try
-            # and cast. Using things for string or
-            # unicode gives us strange results because we get
-            # class name represetnations
-            tmp = i(v)
-            passed = True
-            break
-        except Exception:
-          # we catch all exceptions because we duck-type as
-          # much as possible and some types - e.g., decimal do
-          # not use builtins.
-          pass
-        count += 1
-      if not passed:
-        raise ValueError("Cannot add %s to TypedList (accepts only %s)" %
-          (v, self._allowed_type))
-      else:
-        return tmp
-
-    def __len__(self):
-      return len(self._list)
-
-    def __getitem__(self, i):
-      return self._list[i]
-
-    def __delitem__(self, i):
-      del self._list[i]
-
-    def __setitem__(self, i, v):
-      self.insert(i, v)
-
-    def insert(self, i, v):
-      val = self.check(v)
-      self._list.insert(i, val)
-
-    def append(self, v):
-      if not self._unique or v not in self._list:
-        val = self.check(v)
-        self._list.append(val)
+        def __len__(self):
+            return len(self._list)
 
-    def __str__(self):
-      return str(self._list)
+        def __getitem__(self, i):
+            return self._list[i]
 
-    def __iter__(self):
-      return iter(self._list)
+        def __delitem__(self, i):
+            del self._list[i]
 
-    def __eq__(self, other):
-      if self._list == other:
-        return True
-      return False
+        def __setitem__(self, i, v):
+            self.insert(i, v)
+
+        def insert(self, i, v):
+            val = self.check(v)
+            self._list.insert(i, val)
 
-    def get(self, filter=False):
-      return self._list
-  return type(TypedList(*args, **kwargs))
+        def append(self, v):
+            if not self._unique or v not in self._list:
+                val = self.check(v)
+                self._list.append(val)
+
+        def __str__(self):
+            return str(self._list)
+
+        def __iter__(self):
+            return iter(self._list)
+
+        def __eq__(self, other):
+            if self._list == other:
+                return True
+            return False
+
+        def get(self, filter=False):
+            return self._list
+
+    return type(TypedList(*args, **kwargs))
 
 
 def YANGListType(*args, **kwargs):
-  """
+    """
     Return a type representing a YANG list, with a contained class.
     An ordered dict is used to store the list, and the
     returned object behaves akin to a dictionary.
 
     Additional checks are performed to ensure that the keys of the
     list are valid before adding the value.
 
     .add(key) - initialises a new member of the list
     .delete(key) - removes it.
 
     Where a list exists that does not have a key - which can be the
     case for 'config false' lists - a uuid is generated and used
     as the key for the list.
   """
-  try:
-    keyname = args[0]
-    listclass = args[1]
-  except Exception:
-    raise TypeError("A YANGList must be specified with a key value and a " +
-                      "contained class")
-  is_container = kwargs.pop("is_container", False)
-  parent = kwargs.pop("parent", False)
-  yang_name = kwargs.pop("yang_name", False)
-  yang_keys = kwargs.pop("yang_keys", False)
-  user_ordered = kwargs.pop("user_ordered", False)
-  path_helper = kwargs.pop("path_helper", None)
-  extensions = kwargs.pop("extensions", None)
-
-  class YANGList(object):
-    __slots__ = ('_members', '_keyval',
-                  '_contained_class', '_path_helper', '_yang_keys',
-                  '_ordered',)
-    _pybind_generated_by = "YANGListType"
-
-    def __init__(self, *args, **kwargs):
-      self._ordered = True if user_ordered else False
-      self._members = collections.OrderedDict()
-
-      self._members._user_ordered = True if user_ordered else False
-
-      self._keyval = keyname
-      if not type(listclass) == type(int):
-        raise ValueError("contained class of a YANGList must be a class")
-      self._contained_class = listclass
-      self._path_helper = path_helper
-      self._yang_keys = yang_keys
-
-    def __str__(self):
-      return str(self._members)
+    try:
+        keyname = args[0]
+        listclass = args[1]
+    except Exception:
+        raise TypeError("A YANGList must be specified with a key value and a " + "contained class")
+    is_container = kwargs.pop("is_container", False)
+    parent = kwargs.pop("parent", False)
+    yang_name = kwargs.pop("yang_name", False)
+    yang_keys = kwargs.pop("yang_keys", False)
+    user_ordered = kwargs.pop("user_ordered", False)
+    path_helper = kwargs.pop("path_helper", None)
+    extensions = kwargs.pop("extensions", None)
+
+    class YANGList(object):
+        __slots__ = ("_members", "_keyval", "_contained_class", "_path_helper", "_yang_keys", "_ordered")
+        _pybind_generated_by = "YANGListType"
+
+        def __init__(self, *args, **kwargs):
+            self._ordered = True if user_ordered else False
+            self._members = collections.OrderedDict()
+
+            self._members._user_ordered = True if user_ordered else False
+
+            self._keyval = keyname
+            if not type(listclass) == type(int):
+                raise ValueError("contained class of a YANGList must be a class")
+            self._contained_class = listclass
+            self._path_helper = path_helper
+            self._yang_keys = yang_keys
+
+        def __str__(self):
+            return str(self._members)
+
+        def __repr__(self):
+            return repr(self._members)
+
+        def __check__(self, v):
+            if self._contained_class is None:
+                return False
+            try:
+                tmp = YANGDynClass(
+                    base=self._contained_class,
+                    parent=parent,
+                    yang_name=yang_name,
+                    is_container=is_container,
+                    path_helper=False,
+                )
+                valid = False
+                if not tmp.__slots__ == v.__slots__:
+                    valid = True
+                elif self._contained_class.__slots__ == v.__slots__:
+                    valid = True
+                if valid is False:
+                    return valid
+            except Exception:
+                return False
+            return True
 
-    def __repr__(self):
-      return repr(self._members)
+        def iteritems(self):
+            return six.iteritems(self._members)
 
-    def __check__(self, v):
-      if self._contained_class is None:
-        return False
-      try:
-        tmp = YANGDynClass(base=self._contained_class, parent=parent,
-                            yang_name=yang_name, is_container=is_container,
-                            path_helper=False)
-        valid = False
-        if not tmp.__slots__ == v.__slots__:
-          valid = True
-        elif self._contained_class.__slots__ == v.__slots__:
-          valid = True
-        if valid is False:
-          return valid
-      except Exception:
-        return False
-      return True
+        def itervalues(self):
+            return six.itervalues(self._members)
 
-    def iteritems(self):
-      return six.iteritems(self._members)
+        def _key_to_native_key_type(self, k):
+            if self._keyval is False:
+                raise AttributeError("List does not have a key")
+            elif " " in self._keyval:
+                raise AttributeError("Multiple key, string type should be used")
+            else:
+                member = self._members[k]
+                getfn = getattr(member, "_get_%s" % self._keyval)
+                return getfn()
+
+        def __iter__(self):
+            return iter(self._members)
+
+        def __contains__(self, k):
+            if k in self._members:
+                return True
+            return False
 
-    def itervalues(self):
-      return six.itervalues(self._members)
+        def __getitem__(self, k):
+            return self._members[k]
 
-    def _key_to_native_key_type(self, k):
-      if self._keyval is False:
-        raise AttributeError("List does not have a key")
-      elif " " in self._keyval:
-        raise AttributeError("Multiple key, string type should be used")
-      else:
-        member = self._members[k]
-        getfn = getattr(member, "_get_%s" % self._keyval)
-        return getfn()
+        def __setitem__(self, k, v):
+            self.__set(_k=k, _v=v)
 
-    def __iter__(self):
-      return iter(self._members)
+        def __set(self, *args, **kwargs):
+            k = kwargs.pop("_k", None)
+            v = kwargs.pop("_v", None)
+            named_set = kwargs.pop("_named_set", False)
+
+            if k is None and self._keyval and not named_set:
+                k = args[0]
+            elif k is None:
+                # this is a list that does not have a key specified, and hence
+                # we generate a uuid that is used as the key, the method then
+                # returns the uuid for the upstream process to use
+                k = six.text_type(uuid.uuid1())
+
+            update = False
+            if v is not None:
+                if not self.__check__(v):
+                    raise ValueError("value must be set to an instance of %s" % (self._contained_class))
+                else:
+                    update = True
+
+            if k in self._members:
+                update = True
+
+            if self._keyval:
+                try:
+                    tmp = YANGDynClass(
+                        base=self._contained_class,
+                        parent=parent,
+                        yang_name=yang_name,
+                        is_container="container",
+                        path_helper=False,
+                    )
+                    keydict = None
+
+                    if " " in self._keyval and not named_set:
+                        keys = self._keyval.split(" ")
+                        keyparts = k.split(" ")
+                        keydict = {}
+                        for kp, kv in zip(keys, keyparts):
+                            keydict[kp] = kv
+
+                        if not len(keyparts) == len(keys):
+                            raise KeyError(
+                                "YANGList key must contain all key elements (%s)" % (self._keyval.split(" "))
+                            )
+                    elif named_set:
+                        k = kwargs.pop("_python_key", None)
+                        keydict = copy.copy(kwargs)
+                    else:
+                        if k == "":
+                            raise KeyError("Cannot set a null key for a list entry!")
+                        keydict = {self._keyval: k}
+                        kv_obj = getattr(tmp, self._keyval)
+                        path_keystring = "[%s='%s']" % (kv_obj.yang_name(), k)
+
+                    if keydict is not None:
+                        keys = self._keyval.split(" ")
+                        path_keystring = "["
+                        for kv in keys:
+                            kv_obj = getattr(tmp, kv)
+                            path_keystring += "%s='%s' " % (kv_obj.yang_name(), keydict[kv])
+                        path_keystring = path_keystring[:-1]
+                        path_keystring += "]"
+
+                    if not update:
+                        tmp = YANGDynClass(
+                            base=self._contained_class,
+                            parent=parent,
+                            yang_name=yang_name,
+                            is_container="container",
+                            path_helper=path_helper,
+                            register_path=(self._parent._path() + [self._yang_name + path_keystring]),
+                            extmethods=self._parent._extmethods,
+                            extensions=extensions,
+                        )
+                    else:
+                        # hand the value to the init, rather than simply creating an empty
+                        # object.
+                        tmp = YANGDynClass(
+                            v,
+                            base=self._contained_class,
+                            parent=parent,
+                            yang_name=yang_name,
+                            is_container="container",
+                            path_helper=path_helper,
+                            register_path=(self._parent._path() + [self._yang_name + path_keystring]),
+                            extmethods=self._parent._extmethods,
+                            load=True,
+                            extensions=extensions,
+                        )
+
+                    if keydict is not None:
+                        for kn in keydict:
+                            key = getattr(tmp, "_set_%s" % safe_name(kn))
+                            key(keydict[kn], load=True)
 
-    def __contains__(self, k):
-      if k in self._members:
-        return True
-      return False
+                    if hasattr(k, "_referenced_object") and k._referenced_object is not None:
+                        k = k._referenced_object
 
-    def __getitem__(self, k):
-      return self._members[k]
+                    self._members[k] = tmp
 
-    def __setitem__(self, k, v):
-      self.__set(_k=k, _v=v)
+                except ValueError as m:
+                    raise KeyError("key value must be valid, %s" % m)
+            else:
+                self._members[k] = YANGDynClass(
+                    base=self._contained_class,
+                    parent=parent,
+                    yang_name=yang_name,
+                    is_container=is_container,
+                    path_helper=path_helper,
+                    extmethods=self._parent._extmethods,
+                    extensions=extensions,
+                )
+                return k
+
+        def __delitem__(self, k):
+            del self._members[k]
+
+        def __len__(self):
+            return len(self._members)
+
+        def keys(self):
+            return self._members.keys()
+
+        def items(self):
+            return self._members.items()
+
+        def values(self):
+            return self._members.values()
+
+        def _generate_key(self, *args, **kwargs):
+            keyargs = None
+            if len(args):
+                k = args[0]
+            elif len(kwargs):
+                keyargs = {}
+                k = ""
+                for kn in self._keyval.split(" "):
+                    try:
+                        keyargs[kn] = kwargs[kn]
+                    except KeyError as m:
+                        raise AttributeError(
+                            "Keyword list add function must have all " + "keys specified - cannot find %s" % m
+                        )
+                    k += "%s " % kwargs[kn]
+                k = k[:-1]
+            else:
+                k = None
+            return (k, keyargs)
 
-    def __set(self, *args, **kwargs):
-      k = kwargs.pop("_k", None)
-      v = kwargs.pop("_v", None)
-      named_set = kwargs.pop("_named_set", False)
-
-      if k is None and self._keyval and not named_set:
-        k = args[0]
-      elif k is None:
-        # this is a list that does not have a key specified, and hence
-        # we generate a uuid that is used as the key, the method then
-        # returns the uuid for the upstream process to use
-        k = six.text_type(uuid.uuid1())
-
-      update = False
-      if v is not None:
-        if not self.__check__(v):
-          raise ValueError("value must be set to an instance of %s" %
-            (self._contained_class))
-        else:
-          update = True
+        def _extract_key(self, obj):
+            kp = self._keyval.split(" ")
+            if len(kp) > 1:
+                ks = ""
+                for k in kp:
+                    kv = getattr(obj, "_get_%s" % safe_name(k), None)
+                    if kv is None:
+                        raise KeyError("Invalid key attribute specified for object")
+                    ks += "%s " % six.text_type(kv())
+                return ks.rstrip(" ")
+            else:
+                kv = getattr(obj, "_get_%s" % safe_name(self._keyval), None)
+                if kv is None:
+                    raise KeyError("Invalid key attribute specified for object: %s" % self._keyval)
+                return kv()
+
+        def append(self, obj):
+            self.__set(_k=self._extract_key(obj), _v=obj)
+
+        def _new_item(self):
+            return self._contained_class()
+
+        def add(self, *args, **kwargs):
+            if len(args) and len(kwargs):
+                raise AttributeError("Cannot add an entry to a list based on both " + " keywords and string args")
+
+            value = kwargs.pop("_v", None)
+
+            (k, keyargs) = self._generate_key(*args, **kwargs)
+
+            if k in self._members:
+                raise KeyError("%s is already defined as a list entry" % k)
+            if self._keyval and keyargs is None:
+                if k is None:
+                    raise KeyError("a list with a key value must have a key specified")
+                self.__set(_k=k)
+                return self._members[k]
+            elif self._keyval and keyargs is not None:
+                keyargs["_python_key"] = k
+                keyargs["_named_set"] = True
+                if value is not None:
+                    keyargs["_v"] = value
+                self.__set(**keyargs)
+                return self._members[k]
+            else:
+                k = self.__set()
+                return k
 
-      if k in self._members:
-        update = True
+        def delete(self, *args, **kwargs):
+            (k, _) = self._generate_key(*args, **kwargs)
 
-      if self._keyval:
-        try:
-          tmp = YANGDynClass(base=self._contained_class, parent=parent,
-                              yang_name=yang_name, is_container='container',
-                              path_helper=False)
-          keydict = None
-
-          if " " in self._keyval and not named_set:
-            keys = self._keyval.split(" ")
-            keyparts = k.split(" ")
-            keydict = {}
-            for kp, kv in zip(keys, keyparts):
-              keydict[kp] = kv
-
-            if not len(keyparts) == len(keys):
-              raise KeyError("YANGList key must contain all key elements (%s)"
-                                % (self._keyval.split(" ")))
-          elif named_set:
-            k = kwargs.pop("_python_key", None)
-            keydict = copy.copy(kwargs)
-          else:
-            if k == "":
-              raise KeyError("Cannot set a null key for a list entry!")
-            keydict = {self._keyval: k}
-            kv_obj = getattr(tmp, self._keyval)
-            path_keystring = "[%s='%s']" % (kv_obj.yang_name(), k)
-
-          if keydict is not None:
-            keys = self._keyval.split(" ")
-            path_keystring = "["
-            for kv in keys:
-              kv_obj = getattr(tmp, kv)
-              path_keystring += "%s='%s' " % (kv_obj.yang_name(), keydict[kv])
-            path_keystring = path_keystring[:-1]
-            path_keystring += "]"
-
-          if not update:
-            tmp = YANGDynClass(base=self._contained_class, parent=parent,
-                               yang_name=yang_name,
-                               is_container='container',
-                               path_helper=path_helper,
-                               register_path=(self._parent._path() +
-                                [self._yang_name + path_keystring]),
-                               extmethods=self._parent._extmethods,
-                               extensions=extensions)
-          else:
-            # hand the value to the init, rather than simply creating an empty
-            # object.
-            tmp = YANGDynClass(v, base=self._contained_class, parent=parent,
-                                yang_name=yang_name,
-                                is_container='container',
-                                path_helper=path_helper,
-                                register_path=(self._parent._path() +
-                                [self._yang_name + path_keystring]),
-                                extmethods=self._parent._extmethods,
-                                load=True,
-                                extensions=extensions)
-
-          if keydict is not None:
-            for kn in keydict:
-              key = getattr(tmp, "_set_%s" % safe_name(kn))
-              key(keydict[kn], load=True)
-
-          if hasattr(k, "_referenced_object") and \
-                k._referenced_object is not None:
-            k = k._referenced_object
-
-          self._members[k] = tmp
-
-        except ValueError as m:
-          raise KeyError("key value must be valid, %s" % m)
-      else:
-        self._members[k] = YANGDynClass(base=self._contained_class,
-                                          parent=parent, yang_name=yang_name,
-                                          is_container=is_container,
-                                          path_helper=path_helper,
-                                          extmethods=self._parent._extmethods,
-                                          extensions=extensions)
-        return k
-
-    def __delitem__(self, k):
-      del self._members[k]
-
-    def __len__(self):
-      return len(self._members)
-
-    def keys(self):
-      return self._members.keys()
-
-    def items(self):
-      return self._members.items()
-
-    def values(self):
-      return self._members.values()
-
-    def _generate_key(self, *args, **kwargs):
-      keyargs = None
-      if len(args):
-        k = args[0]
-      elif len(kwargs):
-        keyargs = {}
-        k = ""
-        for kn in self._keyval.split(" "):
-          try:
-            keyargs[kn] = kwargs[kn]
-          except KeyError as m:
-            raise AttributeError("Keyword list add function must have all " +
-                "keys specified - cannot find %s" % m)
-          k += "%s " % kwargs[kn]
-        k = k[:-1]
-      else:
-        k = None
-      return (k, keyargs)
-
-    def _extract_key(self, obj):
-      kp = self._keyval.split(" ")
-      if len(kp) > 1:
-        ks = ''
-        for k in kp:
-          kv = getattr(obj, "_get_%s" % safe_name(k), None)
-          if kv is None:
-            raise KeyError("Invalid key attribute specified for object")
-          ks += "%s " % six.text_type(kv())
-        return ks.rstrip(" ")
-      else:
-        kv = getattr(obj, "_get_%s" % safe_name(self._keyval), None)
-        if kv is None:
-          raise KeyError("Invalid key attribute specified for object: %s"
-                              % self._keyval)
-        return kv()
-
-    def append(self, obj):
-      self.__set(_k=self._extract_key(obj), _v=obj)
-
-    def _new_item(self):
-      return self._contained_class()
-
-    def add(self, *args, **kwargs):
-      if len(args) and len(kwargs):
-        raise AttributeError("Cannot add an entry to a list based on both " +
-                " keywords and string args")
-
-      value = kwargs.pop("_v", None)
-
-      (k, keyargs) = self._generate_key(*args, **kwargs)
-
-      if k in self._members:
-        raise KeyError("%s is already defined as a list entry" % k)
-      if self._keyval and keyargs is None:
-        if k is None:
-          raise KeyError("a list with a key value must have a key specified")
-        self.__set(_k=k)
-        return self._members[k]
-      elif self._keyval and keyargs is not None:
-        keyargs['_python_key'] = k
-        keyargs['_named_set'] = True
-        if value is not None:
-          keyargs['_v'] = value
-        self.__set(**keyargs)
-        return self._members[k]
-      else:
-        k = self.__set()
-        return k
-
-    def delete(self, *args, **kwargs):
-      (k, _) = self._generate_key(*args, **kwargs)
-
-      if self._path_helper:
-        current_item = self._members[k]
-        if " " in self._keyval:
-          keyparts = self._keyval.split(" ")
-          keyargs = k.split(" ")
-          key_string = "["
-          for key, val in zip(keyparts, keyargs):
-            kv_o = getattr(current_item, key)
-            key_string += "%s=%s " % (kv_o.yang_name(), val)
-          key_string = key_string.rstrip(" ")
-          key_string += "]"
-        else:
-          kv_o = getattr(current_item, self._keyval)
-          key_string = "[@%s=%s]" % (kv_o.yang_name(), k)
+            if self._path_helper:
+                current_item = self._members[k]
+                if " " in self._keyval:
+                    keyparts = self._keyval.split(" ")
+                    keyargs = k.split(" ")
+                    key_string = "["
+                    for key, val in zip(keyparts, keyargs):
+                        kv_o = getattr(current_item, key)
+                        key_string += "%s=%s " % (kv_o.yang_name(), val)
+                    key_string = key_string.rstrip(" ")
+                    key_string += "]"
+                else:
+                    kv_o = getattr(current_item, self._keyval)
+                    key_string = "[@%s=%s]" % (kv_o.yang_name(), k)
 
-        obj_path = self._parent._path() + [self._yang_name + key_string]
+                obj_path = self._parent._path() + [self._yang_name + key_string]
 
-      try:
-        del self._members[k]
-        if self._path_helper:
-          self._path_helper.unregister(obj_path)
-      except KeyError as m:
-        raise KeyError("key %s was not in list (%s)" % (k, m))
-
-    def _item(self, *args, **kwargs):
-      keystr = ""
-      if " " in self._keyval:
-        keyparts = self._keyval.split(" ")
-      else:
-        keyparts = [self._keyval]
-      for kn in keyparts:
-        try:
-          keystr += "%s " % kwargs[kn]
-        except KeyError:
-          raise KeyError("Must specify all keys to retrieve a list entry")
-      keystr = keystr[:-1]
-
-      return self._members[keystr]
-
-    def get(self, filter=False):
-      d = collections.OrderedDict()
-      d._user_ordered = self._members._user_ordered
-      for i in self._members:
-        if hasattr(self._members[i], "get"):
-          d[i] = self._members[i].get(filter=filter)
-        else:
-          d[i] = self._members[i]
-      return d
+            try:
+                del self._members[k]
+                if self._path_helper:
+                    self._path_helper.unregister(obj_path)
+            except KeyError as m:
+                raise KeyError("key %s was not in list (%s)" % (k, m))
+
+        def _item(self, *args, **kwargs):
+            keystr = ""
+            if " " in self._keyval:
+                keyparts = self._keyval.split(" ")
+            else:
+                keyparts = [self._keyval]
+            for kn in keyparts:
+                try:
+                    keystr += "%s " % kwargs[kn]
+                except KeyError:
+                    raise KeyError("Must specify all keys to retrieve a list entry")
+            keystr = keystr[:-1]
+
+            return self._members[keystr]
+
+        def get(self, filter=False):
+            d = collections.OrderedDict()
+            d._user_ordered = self._members._user_ordered
+            for i in self._members:
+                if hasattr(self._members[i], "get"):
+                    d[i] = self._members[i].get(filter=filter)
+                else:
+                    d[i] = self._members[i]
+            return d
 
-  return type(YANGList(*args, **kwargs))
+    return type(YANGList(*args, **kwargs))
 
 
 class YANGBool(int):
-  """
+    """
     A custom boolean class for using in YANG. Since bool has specific
     logic in python, it is not possible to extend the existing bool
     objects.
 
     This bool also accepts input matching strings to handle the
     forms that might be used in YANG modules.
   """
-  def __new__(self, *args, **kwargs):
-    false_args = ["false", "False", False, 0, "0"]
-    true_args = ["true", "True", True, 1, "1"]
-    if len(args):
-      if not args[0] in false_args + true_args:
-        raise ValueError("%s is an invalid value for a YANGBool" % args[0])
-      value = 0 if args[0] in false_args else 1
-    else:
-      value = 0
-    return int.__new__(self, bool(value))
 
-  def __repr__(self):
-    return str([False, True][self])
+    def __new__(self, *args, **kwargs):
+        false_args = ["false", "False", False, 0, "0"]
+        true_args = ["true", "True", True, 1, "1"]
+        if len(args):
+            if not args[0] in false_args + true_args:
+                raise ValueError("%s is an invalid value for a YANGBool" % args[0])
+            value = 0 if args[0] in false_args else 1
+        else:
+            value = 0
+        return int.__new__(self, bool(value))
+
+    def __repr__(self):
+        return str([False, True][self])
 
-  def __str__(self):
-    return str(self.__repr__())
+    def __str__(self):
+        return str(self.__repr__())
 
 
 def YANGDynClass(*args, **kwargs):
-  """
+    """
     Wrap an type - specified in the base_type arugment - with
     a set of custom attributes that YANG specifies (or are required
     for serialisation of that object). Particularly:
 
       - base_type:  the original type - for example, string, int.
       - default:    the YANG specified default value of the type.
       - yang_name:  the YANG name of the type (as opposed to a 'safe'
@@ -876,413 +932,425 @@
       - extensions:  The list of extensions that should be stored
                      with the type.
       - is_config:   Whether this is a configuration (editable)
                      node.
       - presence:    Whether the YANG container that is being
                      represented has the presence keyword
   """
-  base_type = kwargs.pop("base", False)
-  default = kwargs.pop("default", False)
-  yang_name = kwargs.pop("yang_name", False)
-  parent_instance = kwargs.pop("parent", False)
-  choice_member = kwargs.pop("choice", False)
-  is_container = kwargs.pop("is_container", False)
-  is_leaf = kwargs.pop("is_leaf", False)
-  path_helper = kwargs.pop("path_helper", None)
-  supplied_register_path = kwargs.pop("register_path", None)
-  extensions = kwargs.pop("extensions", None)
-  extmethods = kwargs.pop("extmethods", None)
-  is_keyval = kwargs.pop("is_keyval", False)
-  register_paths = kwargs.pop("register_paths", True)
-  yang_type = kwargs.pop("yang_type", None)
-  namespace = kwargs.pop("namespace", None)
-  defining_module = kwargs.pop("defining_module", None)
-  load = kwargs.pop("load", None)
-  is_config = kwargs.pop("is_config", True)
-  has_presence = kwargs.pop("presence", None)
-
-  if not base_type:
-    raise TypeError("must have a base type")
-
-  if isinstance(base_type, list):
-    # this is a union, we must infer type
-    if not len(args):
-      # there is no argument to infer the type from
-      # so use the first type (default)
-      base_type = base_type[0]
-    else:
-      type_test = False
-      for candidate_type in base_type:
-        try:
-          type_test = candidate_type(args[0])  # does the slipper fit?
-          break
-        except Exception:
-          pass  # don't worry, move on, plenty more fish (types) in the sea...
-      if type_test is False:
-        # we're left alone at midnight -- no types fit the arguments
-        raise TypeError("did not find a valid type using the argument as a" +
-                            " hint")
-      # otherwise, hop, skip and jump with the last candidate
-      base_type = candidate_type
-
-  clsslots = ['_default', '_mchanged', '_yang_name', '_choice', '_parent',
-                 '_supplied_register_path', '_path_helper', '_base_type',
-                 '_is_leaf', '_is_container', '_extensionsd',
-                 '_extmethods', '_is_keyval',
-                 '_register_paths', '_namespace', '_yang_type',
-                 '_defining_module', '_metadata', '_is_config', '_cpresent',
-                 '_presence']
-
-  if extmethods:
-    rpath = None
-    if supplied_register_path is not None:
-      rpath = supplied_register_path
-    if parent_instance is not None:
-      rpath = parent_instance._path() + [yang_name]
-    else:
-      rpath = []
-    chk_path = "/" + "/".join(remove_path_attributes(rpath))
-    if chk_path in extmethods:
-      for method in [i for i in dir(extmethods[chk_path])
-                                      if not i.startswith("_")]:
-        clsslots.append("_" + method)
-
-  class YANGBaseClass(base_type):
-    # we only create slots for things that are restricted
-    # in adding attributes to them - this means containing
-    # data nodes. This means that we can allow
-    # leaf._someattr to be used by consuming code - it
-    # also fixes an issue whereby we could set __slots__
-    # and try and inherit a variable-length inbuilt such
-    # as long, which is not allowed.
-    if yang_type in ["container", "list"] or is_container == "container":
-      __slots__ = tuple(clsslots)
+    base_type = kwargs.pop("base", False)
+    default = kwargs.pop("default", False)
+    yang_name = kwargs.pop("yang_name", False)
+    parent_instance = kwargs.pop("parent", False)
+    choice_member = kwargs.pop("choice", False)
+    is_container = kwargs.pop("is_container", False)
+    is_leaf = kwargs.pop("is_leaf", False)
+    path_helper = kwargs.pop("path_helper", None)
+    supplied_register_path = kwargs.pop("register_path", None)
+    extensions = kwargs.pop("extensions", None)
+    extmethods = kwargs.pop("extmethods", None)
+    is_keyval = kwargs.pop("is_keyval", False)
+    register_paths = kwargs.pop("register_paths", True)
+    yang_type = kwargs.pop("yang_type", None)
+    namespace = kwargs.pop("namespace", None)
+    defining_module = kwargs.pop("defining_module", None)
+    load = kwargs.pop("load", None)
+    is_config = kwargs.pop("is_config", True)
+    has_presence = kwargs.pop("presence", None)
+
+    if not base_type:
+        raise TypeError("must have a base type")
+
+    if isinstance(base_type, list):
+        # this is a union, we must infer type
+        if not len(args):
+            # there is no argument to infer the type from
+            # so use the first type (default)
+            base_type = base_type[0]
+        else:
+            type_test = False
+            for candidate_type in base_type:
+                try:
+                    type_test = candidate_type(args[0])  # does the slipper fit?
+                    break
+                except Exception:
+                    pass  # don't worry, move on, plenty more fish (types) in the sea...
+            if type_test is False:
+                # we're left alone at midnight -- no types fit the arguments
+                raise TypeError("did not find a valid type using the argument as a" + " hint")
+            # otherwise, hop, skip and jump with the last candidate
+            base_type = candidate_type
+
+    clsslots = [
+        "_default",
+        "_mchanged",
+        "_yang_name",
+        "_choice",
+        "_parent",
+        "_supplied_register_path",
+        "_path_helper",
+        "_base_type",
+        "_is_leaf",
+        "_is_container",
+        "_extensionsd",
+        "_extmethods",
+        "_is_keyval",
+        "_register_paths",
+        "_namespace",
+        "_yang_type",
+        "_defining_module",
+        "_metadata",
+        "_is_config",
+        "_cpresent",
+        "_presence",
+    ]
+
+    if extmethods:
+        rpath = None
+        if supplied_register_path is not None:
+            rpath = supplied_register_path
+        if parent_instance is not None:
+            rpath = parent_instance._path() + [yang_name]
+        else:
+            rpath = []
+        chk_path = "/" + "/".join(remove_path_attributes(rpath))
+        if chk_path in extmethods:
+            for method in [i for i in dir(extmethods[chk_path]) if not i.startswith("_")]:
+                clsslots.append("_" + method)
+
+    class YANGBaseClass(base_type):
+        # we only create slots for things that are restricted
+        # in adding attributes to them - this means containing
+        # data nodes. This means that we can allow
+        # leaf._someattr to be used by consuming code - it
+        # also fixes an issue whereby we could set __slots__
+        # and try and inherit a variable-length inbuilt such
+        # as long, which is not allowed.
+        if yang_type in ["container", "list"] or is_container == "container":
+            __slots__ = tuple(clsslots)
 
-    _pybind_base_class = regex.sub("<(type|class) '(?P<class>.*)'>", "\g<class>",
-                                  str(base_type))
+        _pybind_base_class = regex.sub("<(type|class) '(?P<class>.*)'>", "\g<class>", str(base_type))
 
-    def __new__(self, *args, **kwargs):
-      try:
-        obj = base_type.__new__(self, *args, **kwargs)
-      except TypeError:
-        obj = base_type.__new__(self)
-      return obj
-
-    def __init__(self, *args, **kwargs):
-      self._default = False
-      self._mchanged = False
-      self._yang_name = yang_name
-      self._parent = parent_instance
-      self._choice = choice_member
-      self._path_helper = path_helper
-      self._supplied_register_path = supplied_register_path
-      self._base_type = base_type
-      self._is_leaf = is_leaf
-      self._is_container = is_container
-      self._is_config = is_config
-      self._extensionsd = extensions
-      self._extmethods = extmethods
-      self._is_keyval = is_keyval
-      self._register_paths = register_paths
-      self._namespace = namespace
-      self._yang_type = yang_type
-      self._defining_module = defining_module
-      self._metadata = {}
-      self._presence = has_presence
-      self._cpresent = False
-
-      if self._extmethods:
-        chk_path = \
-            "/" + "/".join(remove_path_attributes(self._register_path()))
-        if chk_path in self._extmethods:
-          for method in [i for i in dir(self._extmethods[chk_path]) if
-                                  not i.startswith("_")]:
-            # Don't allow methods to be overwritten
-            if hasattr(self, "_" + method):
-              continue
-            member = getattr(self._extmethods[chk_path], method)
-            if hasattr(member, "__call__"):
-              if not hasattr(self, "_method"):
-                setattr(self, "_" + method, self.__generate_extmethod(member))
-
-      if default:
-        self._default = default
-      if len(args):
-        if self._default is not False:
-          if not args[0] == self._default:
+        def __new__(self, *args, **kwargs):
+            try:
+                obj = base_type.__new__(self, *args, **kwargs)
+            except TypeError:
+                obj = base_type.__new__(self)
+            return obj
+
+        def __init__(self, *args, **kwargs):
+            self._default = False
+            self._mchanged = False
+            self._yang_name = yang_name
+            self._parent = parent_instance
+            self._choice = choice_member
+            self._path_helper = path_helper
+            self._supplied_register_path = supplied_register_path
+            self._base_type = base_type
+            self._is_leaf = is_leaf
+            self._is_container = is_container
+            self._is_config = is_config
+            self._extensionsd = extensions
+            self._extmethods = extmethods
+            self._is_keyval = is_keyval
+            self._register_paths = register_paths
+            self._namespace = namespace
+            self._yang_type = yang_type
+            self._defining_module = defining_module
+            self._metadata = {}
+            self._presence = has_presence
+            self._cpresent = False
+
+            if self._extmethods:
+                chk_path = "/" + "/".join(remove_path_attributes(self._register_path()))
+                if chk_path in self._extmethods:
+                    for method in [i for i in dir(self._extmethods[chk_path]) if not i.startswith("_")]:
+                        # Don't allow methods to be overwritten
+                        if hasattr(self, "_" + method):
+                            continue
+                        member = getattr(self._extmethods[chk_path], method)
+                        if hasattr(member, "__call__"):
+                            if not hasattr(self, "_method"):
+                                setattr(self, "_" + method, self.__generate_extmethod(member))
+
+            if default:
+                self._default = default
+            if len(args):
+                self._set()
+
+            # lists themselves do not register, only elements within them
+            # are actually created in the tree.
+            if not self._is_container == "list":
+                if self._path_helper:
+                    if self._supplied_register_path is None:
+                        if self._register_paths:
+                            self._path_helper.register(self._register_path(), self)
+                    else:
+                        if self._register_paths:
+                            self._path_helper.register(self._supplied_register_path, self)
+
+            if self._is_container == "list" or self._is_container == "container":
+                kwargs["path_helper"] = self._path_helper
+                if load is not None:
+                    kwargs["load"] = load
+
+            try:
+                super(YANGBaseClass, self).__init__(*args, **kwargs)
+            except TypeError:
+                super(YANGBaseClass, self).__init__()
+            except Exception:
+                six.reraise()
+
+        def _changed(self):
+            return self._mchanged
+
+        def _extensions(self):
+            return self._extensionsd
+
+        def _path(self):
+            return self._register_path()
+
+        def _yang_path(self):
+            return "/" + "/".join(self._register_path())
+
+        def __str__(self):
+            return super(YANGBaseClass, self).__str__()
+
+        def __repr__(self):
+            return super(YANGBaseClass, self).__repr__()
+
+        def _set(self, choice=False):
+            if hasattr(self, "__choices__") and choice:
+                for ch in self.__choices__:
+                    if ch == choice[0]:
+                        for case in self.__choices__[ch]:
+                            if not case == choice[1]:
+                                for elem in self.__choices__[ch][case]:
+                                    method = "_unset_%s" % elem
+                                    if not hasattr(self, method):
+                                        raise AttributeError("unmapped choice!")
+                                    x = getattr(self, method)
+                                    x()
+
+            if self._choice and not choice:
+                choice = self._choice
+
+            self._mchanged = True
+
+            if self._presence:
+                self._cpresent = True
+
+            if self._parent and hasattr(self._parent, "_set"):
+                self._parent._set(choice=choice)
+
+        def _add_metadata(self, k, v):
+            self._metadata[k] = v
+
+        def yang_name(self):
+            return self._yang_name
+
+        def default(self):
+            return self._default
+
+        # we need to overload the set methods
+        def __setitem__(self, *args, **kwargs):
             self._set()
-        else:
-          self._set()
+            super(YANGBaseClass, self).__setitem__(*args, **kwargs)
 
-      # lists themselves do not register, only elements within them
-      # are actually created in the tree.
-      if not self._is_container == "list":
-        if self._path_helper:
-          if self._supplied_register_path is None:
-            if self._register_paths:
-              self._path_helper.register(self._register_path(), self)
-          else:
-            if self._register_paths:
-              self._path_helper.register(self._supplied_register_path, self)
-
-      if self._is_container == 'list' or self._is_container == 'container':
-        kwargs['path_helper'] = self._path_helper
-        if load is not None:
-          kwargs['load'] = load
-
-      try:
-        super(YANGBaseClass, self).__init__(*args, **kwargs)
-      except TypeError:
-        super(YANGBaseClass, self).__init__()
-      except Exception:
-        six.reraise()
-
-    def _changed(self):
-      return self._mchanged
+        def append(self, *args, **kwargs):
+            if not hasattr(super(YANGBaseClass, self), "append"):
+                raise AttributeError("%s object has no attribute append" % base_type)
+            self._set()
+            super(YANGBaseClass, self).append(*args, **kwargs)
 
-    def _extensions(self):
-      return self._extensionsd
+        def pop(self, *args, **kwargs):
+            if not hasattr(super(YANGBaseClass, self), "pop"):
+                raise AttributeError("%s object has no attribute pop" % base_type)
+            self._set()
+            item = super(YANGBaseClass, self).pop(*args, **kwargs)
+            return item
 
-    def _path(self):
-      return self._register_path()
+        def remove(self, *args, **kwargs):
+            if not hasattr(super(YANGBaseClass, self), "remove"):
+                raise AttributeError("%s object has no attribute remove" % base_type)
+            self._set()
+            if self._path_helper:
+                elem_index = super(YANGBaseClass, self).index(*args, **kwargs)
+                super(YANGBaseClass, self).__getitem__(elem_index)
+            super(YANGBaseClass, self).remove(*args, **kwargs)
+
+        def extend(self, *args, **kwargs):
+            if not hasattr(super(YANGBaseClass, self), "extend"):
+                raise AttributeError("%s object has no attribute extend" % base_type)
+            self._set()
+            super(YANGBaseClass, self).extend(*args, **kwargs)
 
-    def _yang_path(self):
-      return "/" + "/".join(self._register_path())
+        def insert(self, *args, **kwargs):
+            if not hasattr(super(YANGBaseClass, self), "insert"):
+                raise AttributeError("%s object has no attribute insert" % base_type)
+            self._set()
+            super(YANGBaseClass, self).insert(*args, **kwargs)
 
-    def __str__(self):
-      return super(YANGBaseClass, self).__str__()
+        def _register_path(self):
+            if self._supplied_register_path is not None:
+                return self._supplied_register_path
+            if self._parent is not None:
+                return self._parent._path() + [self._yang_name]
+            else:
+                return []
 
-    def __repr__(self):
-      return super(YANGBaseClass, self).__repr__()
+        def __generate_extmethod(self, methodfn):
 
-    def _set(self, choice=False):
-      if hasattr(self, '__choices__') and choice:
-        for ch in self.__choices__:
-          if ch == choice[0]:
-            for case in self.__choices__[ch]:
-              if not case == choice[1]:
-                for elem in self.__choices__[ch][case]:
-                  method = "_unset_%s" % elem
-                  if not hasattr(self, method):
-                    raise AttributeError("unmapped choice!")
-                  x = getattr(self, method)
-                  x()
-
-      if self._choice and not choice:
-        choice = self._choice
-
-      self._mchanged = True
-
-      if self._presence:
-        self._cpresent = True
-
-      if self._parent and hasattr(self._parent, "_set"):
-        self._parent._set(choice=choice)
-
-    def _add_metadata(self, k, v):
-      self._metadata[k] = v
-
-    def yang_name(self):
-      return self._yang_name
-
-    def default(self):
-      return self._default
-
-    # we need to overload the set methods
-    def __setitem__(self, *args, **kwargs):
-      self._set()
-      super(YANGBaseClass, self).__setitem__(*args, **kwargs)
-
-    def append(self, *args, **kwargs):
-      if not hasattr(super(YANGBaseClass, self), "append"):
-        raise AttributeError("%s object has no attribute append" % base_type)
-      self._set()
-      super(YANGBaseClass, self).append(*args, **kwargs)
-
-    def pop(self, *args, **kwargs):
-      if not hasattr(super(YANGBaseClass, self), "pop"):
-        raise AttributeError("%s object has no attribute pop" % base_type)
-      self._set()
-      item = super(YANGBaseClass, self).pop(*args, **kwargs)
-      return item
-
-    def remove(self, *args, **kwargs):
-      if not hasattr(super(YANGBaseClass, self), "remove"):
-        raise AttributeError("%s object has no attribute remove" % base_type)
-      self._set()
-      if self._path_helper:
-        elem_index = super(YANGBaseClass, self).index(*args, **kwargs)
-        super(YANGBaseClass, self).__getitem__(elem_index)
-      super(YANGBaseClass, self).remove(*args, **kwargs)
-
-    def extend(self, *args, **kwargs):
-      if not hasattr(super(YANGBaseClass, self), "extend"):
-        raise AttributeError("%s object has no attribute extend" % base_type)
-      self._set()
-      super(YANGBaseClass, self).extend(*args, **kwargs)
-
-    def insert(self, *args, **kwargs):
-      if not hasattr(super(YANGBaseClass, self), "insert"):
-        raise AttributeError("%s object has no attribute insert" % base_type)
-      self._set()
-      super(YANGBaseClass, self).insert(*args, **kwargs)
-
-    def _register_path(self):
-      if self._supplied_register_path is not None:
-        return self._supplied_register_path
-      if self._parent is not None:
-        return self._parent._path() + [self._yang_name]
-      else:
-        return []
-
-    def __generate_extmethod(self, methodfn):
-      def extmethodfn(*args, **kwargs):
-        kwargs['caller'] = self._register_path()
-        kwargs['path_helper'] = self._path_helper
-        return methodfn(*args, **kwargs)
-      return extmethodfn
-
-    def _set_present(self, present=True):
-      if not self._is_container == 'container':
-        raise AttributeError("Cannot set presence on a non-container")
-      self._cpresent = present
-      if present is True:
-        self._set()
-
-    def _present(self):
-      if not self._is_container == 'container':
-        return None
+            def extmethodfn(*args, **kwargs):
+                kwargs["caller"] = self._register_path()
+                kwargs["path_helper"] = self._path_helper
+                return methodfn(*args, **kwargs)
 
-      if self._presence is False:
-        return None
+            return extmethodfn
 
-      return self._cpresent
+        def _set_present(self, present=True):
+            if not self._is_container == "container":
+                raise AttributeError("Cannot set presence on a non-container")
+            self._cpresent = present
+            if present is True:
+                self._set()
 
-  return YANGBaseClass(*args, **kwargs)
+        def _present(self):
+            if not self._is_container == "container":
+                return None
+
+            if self._presence is False:
+                return None
+
+            return self._cpresent
+
+    return YANGBaseClass(*args, **kwargs)
 
 
 def ReferenceType(*args, **kwargs):
-  """
+    """
     A type which based on a path provided acts as a leafref.
     The caller argument is used to allow the path that is provided
     to be a relative (rather than absolute) path. The require_instance
     argument specifies whether errors should be thrown in the case
     that the referenced instance does not exist.
   """
-  ref_path = kwargs.pop("referenced_path", False)
-  path_helper = kwargs.pop("path_helper", None)
-  caller = kwargs.pop("caller", False)
-  require_instance = kwargs.pop("require_instance", False)
-
-  class ReferencePathType(object):
-
-    __slots__ = ('_referenced_path', '_path_helper', '_caller',
-                  '_referenced_object', '_ptr', '_require_instance', '_type',
-                  '_utype')
-
-    _pybind_generated_by = "ReferencePathType"
-
-    def __init__(self, *args, **kwargs):
-      self._referenced_path = ref_path
-      self._path_helper = path_helper
-      self._referenced_object = False
-      self._caller = caller
-      self._ptr = False
-      self._require_instance = require_instance
-      self._type = "unicode"
-      self._utype = six.text_type
-
-      if len(args):
-        value = args[0]
-        if hasattr(self, "_set"):
-          self._set()
-      else:
-        value = None
-
-      if self._path_helper and value is not None:
-        path_chk = self._path_helper.get(self._referenced_path,
-                                          caller=self._caller)
-
-        # if the lookup returns only one leaf, then this means that we have
-        # something that could potentially be a pointer. However, this is not
-        # sufficient to tell whether it is (it could be a single list entry)
-        # - thus perform two additional checks. 1) check whether this is the
-        # key value of a list (if it is then this is something that can be
-        # externally referenced) and 2) check that this is not
-        # a list itself (including a leaf-list)
-        if len(path_chk) == 1 and not path_chk[0]._is_keyval and \
-                      not is_yang_list(path_chk[0]):
-          # we are not checking whether this leaf exists, but rather
-          # this is a pointer to some other value.
-          path_parts = self._referenced_path.split("/")
-          leaf_name = path_parts[-1]
-          if ":" in leaf_name:
-            # normalise the namespace
-            leaf_name = leaf_name.split(":")[1]
-          set_method = getattr(path_chk[0]._parent, "_set_%s"
-                                % safe_name(leaf_name))
-          get_method = getattr(path_chk[0]._parent, "_get_%s"
-                                % safe_name(leaf_name))
-
-          if value is not None:
-            set_method(value)
-          self._type = regex.sub("<(type|class) '(?P<class>.*)'>", "\g<class>",
-                                  str(get_method()._base_type))
-
-          self._utype = get_method()._base_type
-          self._ptr = True
-        elif self._require_instance:
-          if value is None:
-            self._referenced_object = None
-          else:
-            found = False
-            path_chk = self._path_helper.get(self._referenced_path,
-                                              caller=self._caller)
-
-            if len(path_chk) == 1 and is_yang_leaflist(path_chk[0]):
-              index = 0
-              for i in path_chk[0]:
-                if six.text_type(i) == six.text_type(value):
-                  found = True
-                  self._referenced_object = path_chk[0][index]
-                  break
-                index += 1
+    ref_path = kwargs.pop("referenced_path", False)
+    path_helper = kwargs.pop("path_helper", None)
+    caller = kwargs.pop("caller", False)
+    require_instance = kwargs.pop("require_instance", False)
+
+    class ReferencePathType(object):
+
+        __slots__ = (
+            "_referenced_path",
+            "_path_helper",
+            "_caller",
+            "_referenced_object",
+            "_ptr",
+            "_require_instance",
+            "_type",
+            "_utype",
+        )
+
+        _pybind_generated_by = "ReferencePathType"
+
+        def __init__(self, *args, **kwargs):
+            self._referenced_path = ref_path
+            self._path_helper = path_helper
+            self._referenced_object = False
+            self._caller = caller
+            self._ptr = False
+            self._require_instance = require_instance
+            self._type = "unicode"
+            self._utype = six.text_type
+
+            if len(args):
+                value = args[0]
+                if hasattr(self, "_set"):
+                    self._set()
             else:
-              found = False
-              for i in path_chk:
-                if six.text_type(i) == six.text_type(value):
-                  found = True
-                  self._referenced_object = i
-
-            if not found:
-              raise ValueError("no such key (%s) existed in path (%s -> %s)"
-                                  % (value, self._referenced_path, path_chk))
-        else:
-          # require instance is not set, so act like the referenced type
-          self._referenced_object = value
-      elif value is not None:
-        # No path helper and a value is set, just act like the referenced type
-        self._referenced_object = value
-
-    def _get_ptr(self):
-      if self._ptr:
-        ptr = self._path_helper.get(self._referenced_path, caller=self._caller)
-        if len(ptr) == 1:
-          return ptr[0]
-      raise ValueError("Invalid pointer specified")
+                value = None
 
-    def __repr__(self):
-      if not self._ptr:
-        return repr(self._referenced_object)
-      return repr(self._get_ptr())
-
-    def _get(self):
-      if not self._ptr:
-        return self._referenced_object
-      return self._get_ptr()
+            if self._path_helper and value is not None:
+                path_chk = self._path_helper.get(self._referenced_path, caller=self._caller)
 
-    def __str__(self):
-      if not self._ptr:
-        return str(self._referenced_object)
-      return str(self._get_ptr())
+                # if the lookup returns only one leaf, then this means that we have
+                # something that could potentially be a pointer. However, this is not
+                # sufficient to tell whether it is (it could be a single list entry)
+                # - thus perform two additional checks. 1) check whether this is the
+                # key value of a list (if it is then this is something that can be
+                # externally referenced) and 2) check that this is not
+                # a list itself (including a leaf-list)
+                if len(path_chk) == 1 and not path_chk[0]._is_keyval and not is_yang_list(path_chk[0]):
+                    # we are not checking whether this leaf exists, but rather
+                    # this is a pointer to some other value.
+                    path_parts = self._referenced_path.split("/")
+                    leaf_name = path_parts[-1]
+                    if ":" in leaf_name:
+                        # normalise the namespace
+                        leaf_name = leaf_name.split(":")[1]
+                    set_method = getattr(path_chk[0]._parent, "_set_%s" % safe_name(leaf_name))
+                    get_method = getattr(path_chk[0]._parent, "_get_%s" % safe_name(leaf_name))
+
+                    if value is not None:
+                        set_method(value)
+                    self._type = regex.sub("<(type|class) '(?P<class>.*)'>", "\g<class>", str(get_method()._base_type))
+
+                    self._utype = get_method()._base_type
+                    self._ptr = True
+                elif self._require_instance:
+                    if value is None:
+                        self._referenced_object = None
+                    else:
+                        found = False
+                        path_chk = self._path_helper.get(self._referenced_path, caller=self._caller)
+
+                        if len(path_chk) == 1 and is_yang_leaflist(path_chk[0]):
+                            index = 0
+                            for i in path_chk[0]:
+                                if six.text_type(i) == six.text_type(value):
+                                    found = True
+                                    self._referenced_object = path_chk[0][index]
+                                    break
+                                index += 1
+                        else:
+                            found = False
+                            for i in path_chk:
+                                if six.text_type(i) == six.text_type(value):
+                                    found = True
+                                    self._referenced_object = i
+
+                        if not found:
+                            raise ValueError(
+                                "no such key (%s) existed in path (%s -> %s)"
+                                % (value, self._referenced_path, path_chk)
+                            )
+                else:
+                    # require instance is not set, so act like the referenced type
+                    self._referenced_object = value
+            elif value is not None:
+                # No path helper and a value is set, just act like the referenced type
+                self._referenced_object = value
+
+        def _get_ptr(self):
+            if self._ptr:
+                ptr = self._path_helper.get(self._referenced_path, caller=self._caller)
+                if len(ptr) == 1:
+                    return ptr[0]
+            raise ValueError("Invalid pointer specified")
+
+        def __repr__(self):
+            if not self._ptr:
+                return repr(self._referenced_object)
+            return repr(self._get_ptr())
+
+        def _get(self):
+            if not self._ptr:
+                return self._referenced_object
+            return self._get_ptr()
+
+        def __str__(self):
+            if not self._ptr:
+                return str(self._referenced_object)
+            return str(self._get_ptr())
 
-  return type(ReferencePathType(*args, **kwargs))
+    return type(ReferencePathType(*args, **kwargs))
```

### Comparing `pyangbind-0.8.1/pyangbind/plugin/pybind.py` & `pyangbind-0.8.2/pyangbind/plugin/pybind.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,32 +35,28 @@
 
 import pyangbind.helpers.misc as misc_help
 from pyangbind.helpers.identity import IdentityStore
 from pyangbind.lib.yangtypes import RestrictedClassType, YANGBool, safe_name
 
 # Python3 support
 if six.PY3:
-  long = int
+    long = int
 else:
-  import codecs
+    import codecs
 
 DEBUG = True
 if DEBUG:
-  import pprint
-  pp = pprint.PrettyPrinter(indent=2)
+    import pprint
+
+    pp = pprint.PrettyPrinter(indent=2)
 
 # YANG is quite flexible in terms of what it allows as input to a boolean
 # value, this map is used to provide a mapping of these values to the python
 # True and False boolean instances.
-class_bool_map = {
-    'false': False,
-    'False': False,
-    'true': True,
-    'True': True,
-}
+class_bool_map = {"false": False, "False": False, "true": True, "True": True}
 
 class_map = {
     # this map is dynamically built upon but defines how we take
     # a YANG type  and translate it into a native Python class
     # along with other attributes that are required for this mapping.
     #
     # key:                the name of the YANG type
@@ -93,933 +89,964 @@
     #                     we need to re-initialise an instance of the class,
     #                     such as in the setter methods of containers.
     # Other types may add their own types to this dictionary that have
     # meaning only for themselves. For example, a ReferenceType can add the
     # path it references, and whether the require-instance keyword was set
     # or not.
     #
-    'boolean': {
+    "boolean": {
         "native_type": "YANGBool",
         "map": class_bool_map,
         "base_type": True,
         "quote_arg": True,
-        "pytype": YANGBool
-    },
-    'binary': {
-        "native_type": "bitarray",
-        "base_type": True,
-        "quote_arg": True,
-        "pytype": bitarray
-    },
-    'uint8': {
-        "native_type": ("RestrictedClassType(base_type=int," +
-                       " restriction_dict={'range': ['0..255']}, int_size=8)"),
-        "base_type": True,
-        "pytype": RestrictedClassType(base_type=int,
-                    restriction_dict={'range': ['0..255']}, int_size=8)
-    },
-    'uint16': {
-        "native_type": ("RestrictedClassType(base_type=int," +
-                       " restriction_dict={'range': ['0..65535']}," +
-                       "int_size=16)"),
-        "base_type": True,
-        "pytype": RestrictedClassType(base_type=int,
-                    restriction_dict={'range': ['0..65535']}, int_size=16)
+        "pytype": YANGBool,
     },
-    'uint32': {
-        "native_type": ("RestrictedClassType(base_type=long," +
-                        " restriction_dict={'range': ['0..4294967295']}," +
-                        " int_size=32)"),
+    "binary": {"native_type": "bitarray", "base_type": True, "quote_arg": True, "pytype": bitarray},
+    "uint8": {
+        "native_type": ("RestrictedClassType(base_type=int," + " restriction_dict={'range': ['0..255']}, int_size=8)"),
         "base_type": True,
-        "pytype": RestrictedClassType(base_type=long,
-                    restriction_dict={'range': ['0..4294967295']}, int_size=32)
+        "pytype": RestrictedClassType(base_type=int, restriction_dict={"range": ["0..255"]}, int_size=8),
     },
-    'uint64': {
-        "native_type": ("RestrictedClassType(base_type=long, " +
-                       "restriction_dict={'range': " +
-                       " ['0..18446744073709551615']}, int_size=64)"),
+    "uint16": {
+        "native_type": (
+            "RestrictedClassType(base_type=int," + " restriction_dict={'range': ['0..65535']}," + "int_size=16)"
+        ),
         "base_type": True,
-        "pytype": RestrictedClassType(base_type=long,
-                    restriction_dict={'range': ['0..18446744073709551615']},
-                    int_size=64)
+        "pytype": RestrictedClassType(base_type=int, restriction_dict={"range": ["0..65535"]}, int_size=16),
     },
-    'string': {
-        "native_type": "six.text_type",
+    "uint32": {
+        "native_type": (
+            "RestrictedClassType(base_type=long," + " restriction_dict={'range': ['0..4294967295']}," + " int_size=32)"
+        ),
         "base_type": True,
-        "quote_arg": True,
-        "pytype": six.text_type
+        "pytype": RestrictedClassType(base_type=long, restriction_dict={"range": ["0..4294967295"]}, int_size=32),
     },
-    'decimal64': {
-        "native_type": "Decimal",
+    "uint64": {
+        "native_type": (
+            "RestrictedClassType(base_type=long, "
+            + "restriction_dict={'range': "
+            + " ['0..18446744073709551615']}, int_size=64)"
+        ),
         "base_type": True,
-        "pytype": decimal.Decimal
+        "pytype": RestrictedClassType(
+            base_type=long, restriction_dict={"range": ["0..18446744073709551615"]}, int_size=64
+        ),
     },
-    'empty': {
+    "string": {"native_type": "six.text_type", "base_type": True, "quote_arg": True, "pytype": six.text_type},
+    "decimal64": {"native_type": "Decimal", "base_type": True, "pytype": decimal.Decimal},
+    "empty": {
         "native_type": "YANGBool",
         "map": class_bool_map,
         "base_type": True,
         "quote_arg": True,
-        "pytype": YANGBool
+        "pytype": YANGBool,
     },
-    'int8': {
-        "native_type": "RestrictedClassType(base_type=int, " +
-                      "restriction_dict={'range': ['-128..127']}, int_size=8)",
+    "int8": {
+        "native_type": "RestrictedClassType(base_type=int, "
+        + "restriction_dict={'range': ['-128..127']}, int_size=8)",
         "base_type": True,
-        "pytype": RestrictedClassType(base_type=int,
-                    restriction_dict={'range': ['-128..127']}, int_size=8)
+        "pytype": RestrictedClassType(base_type=int, restriction_dict={"range": ["-128..127"]}, int_size=8),
     },
-    'int16': {
-        "native_type": ("RestrictedClassType(base_type=int,"
-                       "restriction_dict={'range': ['-32768..32767']}, " +
-                       "int_size=16)"),
+    "int16": {
+        "native_type": (
+            "RestrictedClassType(base_type=int," "restriction_dict={'range': ['-32768..32767']}, " + "int_size=16)"
+        ),
         "base_type": True,
-        "pytype": RestrictedClassType(base_type=int,
-                    restriction_dict={'range': ['-32768..32767']}, int_size=16)
+        "pytype": RestrictedClassType(base_type=int, restriction_dict={"range": ["-32768..32767"]}, int_size=16),
     },
-    'int32': {
-        "native_type": ("RestrictedClassType(base_type=long," +
-                        " restriction_dict={'range': " +
-                        "['-2147483648..2147483647']}, int_size=32)"),
+    "int32": {
+        "native_type": (
+            "RestrictedClassType(base_type=long,"
+            + " restriction_dict={'range': "
+            + "['-2147483648..2147483647']}, int_size=32)"
+        ),
         "base_type": True,
-        "pytype": RestrictedClassType(base_type=long,
-                    restriction_dict={'range': ['-2147483648..2147483647']},
-                    int_size=32)
+        "pytype": RestrictedClassType(
+            base_type=long, restriction_dict={"range": ["-2147483648..2147483647"]}, int_size=32
+        ),
     },
-    'int64': {
-        "native_type": ("RestrictedClassType(base_type=long, " +
-                       "restriction_dict={'range': " +
-                       "['-9223372036854775808..9223372036854775807']}, " +
-                       "int_size=64)"),
+    "int64": {
+        "native_type": (
+            "RestrictedClassType(base_type=long, "
+            + "restriction_dict={'range': "
+            + "['-9223372036854775808..9223372036854775807']}, "
+            + "int_size=64)"
+        ),
         "base_type": True,
-        "pytype": RestrictedClassType(base_type=long,
-                    restriction_dict={'range':
-                    ['-9223372036854775808..9223372036854775807']}, int_size=64)
+        "pytype": RestrictedClassType(
+            base_type=long, restriction_dict={"range": ["-9223372036854775808..9223372036854775807"]}, int_size=64
+        ),
     },
 }
 
 # We have a set of types which support "range" statements in RFC6020. This
 # list determins types that should be allowed to have a "range" argument.
-INT_RANGE_TYPES = ["uint8", "uint16", "uint32", "uint64",
-                    "int8", "int16", "int32", "int64"]
+INT_RANGE_TYPES = ["uint8", "uint16", "uint32", "uint64", "int8", "int16", "int32", "int64"]
 
 # The types that are built-in to YANG
-YANG_BUILTIN_TYPES = list(class_map.keys()) + \
-                      ["container", "list", "rpc", "notification", "leafref"]
+YANG_BUILTIN_TYPES = list(class_map.keys()) + ["container", "list", "rpc", "notification", "leafref"]
 
 
 # Base machinery to support operation as a plugin to pyang.
 def pyang_plugin_init():
     plugin.register_plugin(PyangBindClass())
 
 
 class PyangBindClass(plugin.PyangPlugin):
+
     def add_output_format(self, fmts):
-      # Add the 'pybind' output format to pyang.
-      self.multiple_modules = True
-      fmts['pybind'] = self
+        # Add the 'pybind' output format to pyang.
+        self.multiple_modules = True
+        fmts["pybind"] = self
 
     def emit(self, ctx, modules, fd):
-      # When called, call the build_pyangbind function.
-      build_pybind(ctx, modules, fd)
+        # When called, call the build_pyangbind function.
+        build_pybind(ctx, modules, fd)
 
     def add_opts(self, optparser):
-      # Add pyangbind specific operations to pyang. These are documented in the
-      # options, but are essentially divided into three sets.
-      #   * xpathhelper - How pyangbind should deal with xpath expressions.
-      #     This module is documented in lib/xpathhelper and describes how
-      #     to support registration, updates, and retrieval of xpaths.
-      #   * class output - whether a single file should be created, or whether
-      #     a hierarchy of python modules should be created. The latter is
-      #     preferable when one has large trees being compiled.
-      #   * extensions - support for YANG extensions that pyangbind should look
-      #     for, and add as a dictionary with each element.
-      option_group = optparse.OptionGroup(optparser, "pyangbind output specific options")
-      option_group.add_option("--use-xpathhelper",
-                           dest="use_xpathhelper",
-                           action="store_true",
-                           help="""Use the xpathhelper module to
-                                   resolve leafrefs"""),
-      option_group.add_option("--split-class-dir",
-                           metavar="DIR",
-                           dest="split_class_dir",
-                           help="""Split the code output into
-                                   multiple directories"""),
-      option_group.add_option("--interesting-extension",
-                          metavar="EXTENSION-MODULE",
-                          default=[],
-                          action="append",
-                          type=str,
-                          dest="pybind_interested_exts",
-                          help="""A set of extensions that
+        # Add pyangbind specific operations to pyang. These are documented in the
+        # options, but are essentially divided into three sets.
+        #   * xpathhelper - How pyangbind should deal with xpath expressions.
+        #     This module is documented in lib/xpathhelper and describes how
+        #     to support registration, updates, and retrieval of xpaths.
+        #   * class output - whether a single file should be created, or whether
+        #     a hierarchy of python modules should be created. The latter is
+        #     preferable when one has large trees being compiled.
+        #   * extensions - support for YANG extensions that pyangbind should look
+        #     for, and add as a dictionary with each element.
+        option_group = optparse.OptionGroup(optparser, "pyangbind output specific options")
+        option_group.add_option(
+            "--use-xpathhelper",
+            dest="use_xpathhelper",
+            action="store_true",
+            help="""Use the xpathhelper module to
+                                   resolve leafrefs""",
+        ),
+        option_group.add_option(
+            "--split-class-dir",
+            metavar="DIR",
+            dest="split_class_dir",
+            help="""Split the code output into
+                                   multiple directories""",
+        ),
+        option_group.add_option(
+            "--interesting-extension",
+            metavar="EXTENSION-MODULE",
+            default=[],
+            action="append",
+            type=str,
+            dest="pybind_interested_exts",
+            help="""A set of extensions that
                                   are interesting and should be
                                   stored with the class. They
                                   can be accessed through the
                                   "extension_dict()" argument.
                                   Multiple arguments can be
-                                  specified."""),
-      option_group.add_option("--use-extmethods",
-                          dest="use_extmethods",
-                          action="store_true",
-                          help="""Allow a path-keyed dictionary
+                                  specified.""",
+        ),
+        option_group.add_option(
+            "--use-extmethods",
+            dest="use_extmethods",
+            action="store_true",
+            help="""Allow a path-keyed dictionary
                                   to be used to specify methods
-                                  related to a particular class"""),
-      option_group.add_option("--build-rpcs",
-                          dest="build_rpcs",
-                          action="store_true",
-                          help="""Generate class bindings for
+                                  related to a particular class""",
+        ),
+        option_group.add_option(
+            "--build-rpcs",
+            dest="build_rpcs",
+            action="store_true",
+            help="""Generate class bindings for
                                   the input and output of RPCs
                                   defined in each module. These
                                   are placed at the root of
-                                  each module"""),
-      option_group.add_option("--presence",
-                            dest="generate_presence",
-                            action="store_true",
-                            help="""Capture whether the presence
+                                  each module""",
+        ),
+        option_group.add_option(
+            "--presence",
+            dest="generate_presence",
+            action="store_true",
+            help="""Capture whether the presence
                                     keyword is used in the generated
-                                    code."""),
-      option_group.add_option("--build-notifications",
-                          dest="build_notifications",
-                          action="store_true",
-                          help="""Generate class bindings for
+                                    code.""",
+        ),
+        option_group.add_option(
+            "--build-notifications",
+            dest="build_notifications",
+            action="store_true",
+            help="""Generate class bindings for
                                   notifications defined in each
                                   module. These are placed at
-                                  the root of each module"""),
-      optparser.add_option_group(option_group)
+                                  the root of each module""",
+        ),
+        optparser.add_option_group(option_group)
 
 
 # Core function to build the pyangbind output - starting with building the
 # dependencies - and then working through the instantiated tree that pyang has
 # already parsed.
 def build_pybind(ctx, modules, fd):
-  # Restrict the output of the plugin to only the modules that are supplied
-  # to pyang. More modules are parsed by pyangbind to resolve typedefs and
-  # identities.
-  module_d = {}
-  for mod in modules:
-    module_d[mod.arg] = mod
-  pyang_called_modules = module_d.keys()
-
-  # Bail if there are pyang errors, since this certainly means that the
-  # pyangbind output will fail - unless these are solely due to imports that
-  # we provided but then unused.
-  if len(ctx.errors):
-    for e in ctx.errors:
-      print("INFO: encountered %s" % str(e))
-      if not e[1] in ["UNUSED_IMPORT", "PATTERN_ERROR"]:
-        sys.stderr.write("FATAL: pyangbind cannot build module that pyang" +
-          " has found errors with.\n")
-        sys.exit(127)
-
-  # Build the common set of imports that all pyangbind files needs
-  ctx.pybind_common_hdr = "# -*- coding: utf-8 -*-"
-  ctx.pybind_common_hdr += "\n"
-  ctx.pybind_common_hdr += "from operator import attrgetter\n"
-  if ctx.opts.use_xpathhelper:
-    ctx.pybind_common_hdr += "import pyangbind.lib.xpathhelper as xpathhelper\n"
-
-  yangtypes_imports = ["RestrictedPrecisionDecimalType", "RestrictedClassType", "TypedListType",
-                       "YANGBool", "YANGListType", "YANGDynClass", "ReferenceType"]
-  for library in yangtypes_imports:
-    ctx.pybind_common_hdr += "from pyangbind.lib.yangtypes import {}\n".format(library)
-  ctx.pybind_common_hdr += "from pyangbind.lib.base import PybindBase\n"
-  ctx.pybind_common_hdr += "from collections import OrderedDict\n"
-  ctx.pybind_common_hdr += "from decimal import Decimal\n"
-  ctx.pybind_common_hdr += "from bitarray import bitarray\n"
-  ctx.pybind_common_hdr += "import six\n"
+    # Restrict the output of the plugin to only the modules that are supplied
+    # to pyang. More modules are parsed by pyangbind to resolve typedefs and
+    # identities.
+    module_d = {}
+    for mod in modules:
+        module_d[mod.arg] = mod
+    pyang_called_modules = module_d.keys()
+
+    # Bail if there are pyang errors, since this certainly means that the
+    # pyangbind output will fail - unless these are solely due to imports that
+    # we provided but then unused.
+    if len(ctx.errors):
+        for e in ctx.errors:
+            print("INFO: encountered %s" % str(e))
+            if not e[1] in ["UNUSED_IMPORT", "PATTERN_ERROR"]:
+                sys.stderr.write("FATAL: pyangbind cannot build module that pyang" + " has found errors with.\n")
+                sys.exit(127)
+
+    # Build the common set of imports that all pyangbind files needs
+    ctx.pybind_common_hdr = "# -*- coding: utf-8 -*-"
+    ctx.pybind_common_hdr += "\n"
+    ctx.pybind_common_hdr += "from operator import attrgetter\n"
+    if ctx.opts.use_xpathhelper:
+        ctx.pybind_common_hdr += "import pyangbind.lib.xpathhelper as xpathhelper\n"
+
+    yangtypes_imports = [
+        "RestrictedPrecisionDecimalType",
+        "RestrictedClassType",
+        "TypedListType",
+        "YANGBool",
+        "YANGListType",
+        "YANGDynClass",
+        "ReferenceType",
+    ]
+    for library in yangtypes_imports:
+        ctx.pybind_common_hdr += "from pyangbind.lib.yangtypes import {}\n".format(library)
+    ctx.pybind_common_hdr += "from pyangbind.lib.base import PybindBase\n"
+    ctx.pybind_common_hdr += "from collections import OrderedDict\n"
+    ctx.pybind_common_hdr += "from decimal import Decimal\n"
+    ctx.pybind_common_hdr += "from bitarray import bitarray\n"
+    ctx.pybind_common_hdr += "import six\n"
 
-  # Python3 support
-  ctx.pybind_common_hdr += """
+    # Python3 support
+    ctx.pybind_common_hdr += """
 # PY3 support of some PY2 keywords (needs improved)
 if six.PY3:
   import builtins as __builtin__
   long = int
 elif six.PY2:
   import __builtin__
 
 """
 
-  if not ctx.opts.split_class_dir:
-    fd.write(ctx.pybind_common_hdr)
-  else:
-    ctx.pybind_split_basepath = os.path.abspath(ctx.opts.split_class_dir)
-    if not os.path.exists(ctx.pybind_split_basepath):
-      os.makedirs(ctx.pybind_split_basepath)
-
-  # Determine all modules, and submodules that are needed, along with the
-  # prefix that is used for it. We need to ensure that we understand all of the
-  # prefixes that might be used to reference an identity or a typedef.
-  all_mods = []
-  for module in modules:
-    local_module_prefix = module.search_one('prefix')
-    if local_module_prefix is None:
-      local_module_prefix = \
-          module.search_one('belongs-to').search_one('prefix')
-      if local_module_prefix is None:
-        raise AttributeError("A module (%s) must have a prefix or parent " +
-          "module")
-      local_module_prefix = local_module_prefix.arg
+    if not ctx.opts.split_class_dir:
+        fd.write(ctx.pybind_common_hdr)
     else:
-      local_module_prefix = local_module_prefix.arg
-    mods = [(local_module_prefix, module)]
+        ctx.pybind_split_basepath = os.path.abspath(ctx.opts.split_class_dir)
+        if not os.path.exists(ctx.pybind_split_basepath):
+            os.makedirs(ctx.pybind_split_basepath)
+
+    # Determine all modules, and submodules that are needed, along with the
+    # prefix that is used for it. We need to ensure that we understand all of the
+    # prefixes that might be used to reference an identity or a typedef.
+    all_mods = []
+    for module in modules:
+        local_module_prefix = module.search_one("prefix")
+        if local_module_prefix is None:
+            local_module_prefix = module.search_one("belongs-to").search_one("prefix")
+            if local_module_prefix is None:
+                raise AttributeError("A module (%s) must have a prefix or parent " + "module")
+            local_module_prefix = local_module_prefix.arg
+        else:
+            local_module_prefix = local_module_prefix.arg
+        mods = [(local_module_prefix, module)]
 
-    imported_modules = module.search('import')
+        imported_modules = module.search("import")
 
-    # 'include' statements specify the submodules of the existing module -
-    # that also need to be parsed.
-    for i in module.search('include'):
-      subm = ctx.get_module(i.arg)
-      if subm is not None:
-        mods.append((local_module_prefix, subm))
-        # Handle the case that imports are within a submodule
-        if subm.search('import') is not None:
-          imported_modules.extend(subm.search('import'))
-
-    # 'import' statements specify the other modules that this module will
-    # reference.
-    for j in imported_modules:
-      mod = ctx.get_module(j.arg)
-      if mod is not None:
-        imported_module_prefix = j.search_one('prefix').arg
-        mods.append((imported_module_prefix, mod))
-        modules.append(mod)
-    all_mods.extend(mods)
-
-  # remove duplicates from the list (same module and prefix)
-  new_all_mods = []
-  for mod in all_mods:
-    if mod not in new_all_mods:
-      new_all_mods.append(mod)
-  all_mods = new_all_mods
-
-  # Build a list of the 'typedef' and 'identity' statements that are included
-  # in the modules supplied.
-  defn = OrderedDict()
-  for defnt in ['typedef', 'identity']:
-    defn[defnt] = OrderedDict()
-    for m in all_mods:
-      t = misc_help.find_definitions(defnt, ctx, m[1], m[0])
-      for k in t:
-        if k not in defn[defnt]:
-          defn[defnt][k] = t[k]
-
-  # Build the identities and typedefs (these are added to the class_map which
-  # is globally referenced).
-  build_identities(ctx, defn['identity'])
-  build_typedefs(ctx, defn['typedef'])
-
-  # Iterate through the tree which pyang has built, solely for the modules
-  # that pyang was asked to build
-  for modname in pyang_called_modules:
-    module = module_d[modname]
-    mods = [module]
-    for i in module.search('include'):
-      subm = ctx.get_module(i.arg)
-      if subm is not None:
-        mods.append(subm)
-    for m in mods:
-      children = [ch for ch in module.i_children
-            if ch.keyword in statements.data_definition_keywords]
-      get_children(ctx, fd, children, m, m)
-
-      if ctx.opts.build_rpcs:
-        rpcs = [ch for ch in module.i_children
-                  if ch.keyword == 'rpc']
-        # Build RPCs specifically under the module name, since this
-        # can be used as a proxy for the namespace.
-        if len(rpcs):
-          get_children(ctx, fd, rpcs, module, module, register_paths=False,
-                      path="/%s_rpc" % (safe_name(module.arg)))
-
-      if ctx.opts.build_notifications:
-        notifications = [ch for ch in module.i_children
-                  if ch.keyword == 'notification']
-        # Build notifications specifically under the module name,
-        # since this can be used as a proxy for the namespace.
-        if len(notifications):
-          get_children(ctx, fd, notifications, module, module, register_paths=False,
-                      path="/%s_notification" % (safe_name(module.arg)))
+        # 'include' statements specify the submodules of the existing module -
+        # that also need to be parsed.
+        for i in module.search("include"):
+            subm = ctx.get_module(i.arg)
+            if subm is not None:
+                mods.append((local_module_prefix, subm))
+                # Handle the case that imports are within a submodule
+                if subm.search("import") is not None:
+                    imported_modules.extend(subm.search("import"))
+
+        # 'import' statements specify the other modules that this module will
+        # reference.
+        for j in imported_modules:
+            mod = ctx.get_module(j.arg)
+            if mod is not None:
+                imported_module_prefix = j.search_one("prefix").arg
+                mods.append((imported_module_prefix, mod))
+                modules.append(mod)
+        all_mods.extend(mods)
+
+    # remove duplicates from the list (same module and prefix)
+    new_all_mods = []
+    for mod in all_mods:
+        if mod not in new_all_mods:
+            new_all_mods.append(mod)
+    all_mods = new_all_mods
+
+    # Build a list of the 'typedef' and 'identity' statements that are included
+    # in the modules supplied.
+    defn = OrderedDict()
+    for defnt in ["typedef", "identity"]:
+        defn[defnt] = OrderedDict()
+        for m in all_mods:
+            t = misc_help.find_definitions(defnt, ctx, m[1], m[0])
+            for k in t:
+                if k not in defn[defnt]:
+                    defn[defnt][k] = t[k]
+
+    # Build the identities and typedefs (these are added to the class_map which
+    # is globally referenced).
+    build_identities(ctx, defn["identity"])
+    build_typedefs(ctx, defn["typedef"])
+
+    # Iterate through the tree which pyang has built, solely for the modules
+    # that pyang was asked to build
+    for modname in pyang_called_modules:
+        module = module_d[modname]
+        mods = [module]
+        for i in module.search("include"):
+            subm = ctx.get_module(i.arg)
+            if subm is not None:
+                mods.append(subm)
+        for m in mods:
+            children = [ch for ch in module.i_children if ch.keyword in statements.data_definition_keywords]
+            get_children(ctx, fd, children, m, m)
+
+            if ctx.opts.build_rpcs:
+                rpcs = [ch for ch in module.i_children if ch.keyword == "rpc"]
+                # Build RPCs specifically under the module name, since this
+                # can be used as a proxy for the namespace.
+                if len(rpcs):
+                    get_children(
+                        ctx, fd, rpcs, module, module, register_paths=False, path="/%s_rpc" % (safe_name(module.arg))
+                    )
+
+            if ctx.opts.build_notifications:
+                notifications = [ch for ch in module.i_children if ch.keyword == "notification"]
+                # Build notifications specifically under the module name,
+                # since this can be used as a proxy for the namespace.
+                if len(notifications):
+                    get_children(
+                        ctx,
+                        fd,
+                        notifications,
+                        module,
+                        module,
+                        register_paths=False,
+                        path="/%s_notification" % (safe_name(module.arg)),
+                    )
 
 
 def build_identities(ctx, defnd):
-  # Build a storage object that has all the definitions that we
-  # require within it.
-  idstore = IdentityStore()
-  idstore.build_store_from_definitions(ctx, defnd)
-
-  identity_dict = {}
-  for identity in idstore:
-    for prefix in identity.prefixes():
-      ident = "%s:%s" % (prefix, identity.name)
-      identity_dict[ident] = {}
-      identity_dict["%s" % identity.name] = {}
-      for ch in identity.children:
-        d = {"@module": ch.source_module, "@namespace": ch.source_namespace}
-        for cpfx in ch.prefixes() + [None]:
-          if cpfx is not None:
-            spfx = "%s:" % cpfx
-          else:
-            spfx = ""
-          identity_dict[ident][ch.name] = d
-          identity_dict[identity.name][ch.name] = d
-          identity_dict[ident]["%s%s" % (spfx, ch.name)] = d
-          identity_dict[identity.name]["%s%s" % (spfx, ch.name)] = d
-
-    if identity.name not in identity_dict:
-      identity_dict[identity.name] = {}
-
-  # Add entries to the class_map such that this identity can be referenced by
-  # elements that use this identity ref.
-  for i in identity_dict:
-    id_type = {"native_type": """RestrictedClassType(base_type=six.text_type, """ +
-                              """restriction_type="dict_key", """ +
-                              """restriction_arg=%s,)""" % identity_dict[i],
-                "restriction_argument": identity_dict[i],
-                "restriction_type": "dict_key",
-                "parent_type": "string",
-                "base_type": False}
-    class_map[i] = id_type
+    # Build a storage object that has all the definitions that we
+    # require within it.
+    idstore = IdentityStore()
+    idstore.build_store_from_definitions(ctx, defnd)
+
+    identity_dict = {}
+    for identity in idstore:
+        for prefix in identity.prefixes():
+            ident = "%s:%s" % (prefix, identity.name)
+            identity_dict[ident] = {}
+            identity_dict["%s" % identity.name] = {}
+            for ch in identity.children:
+                d = {"@module": ch.source_module, "@namespace": ch.source_namespace}
+                for cpfx in ch.prefixes() + [None]:
+                    if cpfx is not None:
+                        spfx = "%s:" % cpfx
+                    else:
+                        spfx = ""
+                    identity_dict[ident][ch.name] = d
+                    identity_dict[identity.name][ch.name] = d
+                    identity_dict[ident]["%s%s" % (spfx, ch.name)] = d
+                    identity_dict[identity.name]["%s%s" % (spfx, ch.name)] = d
+
+        if identity.name not in identity_dict:
+            identity_dict[identity.name] = {}
+
+    # Add entries to the class_map such that this identity can be referenced by
+    # elements that use this identity ref.
+    for i in identity_dict:
+        id_type = {
+            "native_type": """RestrictedClassType(base_type=six.text_type, """
+            + """restriction_type="dict_key", """
+            + """restriction_arg=%s,)""" % identity_dict[i],
+            "restriction_argument": identity_dict[i],
+            "restriction_type": "dict_key",
+            "parent_type": "string",
+            "base_type": False,
+        }
+        class_map[i] = id_type
 
 
 def build_typedefs(ctx, defnd):
-  # Build the type definitions that are specified within a model. Since
-  # typedefs are essentially derived from existing types, order of processing
-  # is important - we need to go through and build the types in order where
-  # they have a known 'type'.
-  unresolved_tc = {}
-  for i in defnd:
-    unresolved_tc[i] = 0
-  unresolved_t = list(defnd.keys())
-  error_ids = []
-  known_types = list(class_map.keys())
-  known_types.append('enumeration')
-  known_types.append('leafref')
-  base_types = copy.deepcopy(known_types)
-  process_typedefs_ordered = []
-
-  while len(unresolved_t):
-    t = unresolved_t.pop(0)
-    base_t = defnd[t].search_one('type')
-    if base_t.arg == "union":
-      subtypes = []
-      for i in base_t.search('type'):
-        if i.arg == "identityref":
-          subtypes.append(i.search_one('base'))
-        else:
-          subtypes.append(i)
-    elif base_t.arg == "identityref":
-      subtypes = [base_t.search_one('base')]
-    else:
-      subtypes = [base_t]
-
-    any_unknown = False
-    for i in subtypes:
-      # Resolve this typedef to the module that it
-      # was defined by
-
-      if ":" in i.arg:
-        defining_module = util.prefix_to_module(defnd[t].i_module,
-                           i.arg.split(":")[0], defnd[t].pos, ctx.errors)
-      else:
-        defining_module = defnd[t].i_module
-
-      belongs_to = defining_module.search_one('belongs-to')
-      if belongs_to is not None:
-        for mod in ctx.modules:
-          if mod[0] == belongs_to.arg:
-            defining_module = ctx.modules[mod]
-
-      real_pfx = defining_module.search_one('prefix').arg
-
-      if ":" in i.arg:
-        tn = "%s:%s" % (real_pfx, i.arg.split(":")[1])
-      elif i.arg not in base_types:
-        # If this was not a base type (defined in YANG) then resolve it
-        # to the module it belongs to.
-        tn = "%s:%s" % (real_pfx, i.arg)
-      else:
-        tn = i.arg
-
-      if tn not in known_types:
-        any_unknown = True
-
-    if not any_unknown:
-      process_typedefs_ordered.append((t, defnd[t]))
-      known_types.append(t)
-    else:
-      unresolved_tc[t] += 1
-      if unresolved_tc[t] > 1000:
-        # Take a similar approach to the resolution of identities. If we have a
-        # typedef that has a type in it that is not found after many iterations
-        # then we should bail.
-        error_ids.append(t)
-        sys.stderr.write("could not find a match for %s type -> %s\n" %
-          (t, [i.arg for i in subtypes]))
-      else:
-        unresolved_t.append(t)
-
-  if error_ids:
-    raise TypeError("could not resolve typedefs %s" % error_ids)
-
-  # Process the types that we built above.
-  for i_tuple in process_typedefs_ordered:
-    item = i_tuple[1]
-    type_name = i_tuple[0]
-    # Copy the class_map entry - this is done so that we do not alter the
-    # existing instance in memory as we add to it.
-    cls, elemtype = copy.deepcopy(build_elemtype(ctx, item.search_one('type')))
+    # Build the type definitions that are specified within a model. Since
+    # typedefs are essentially derived from existing types, order of processing
+    # is important - we need to go through and build the types in order where
+    # they have a known 'type'.
+    unresolved_tc = {}
+    for i in defnd:
+        unresolved_tc[i] = 0
+    unresolved_t = list(defnd.keys())
+    error_ids = []
     known_types = list(class_map.keys())
-    # Enumeration is a native type, but is not natively supported
-    # in the class_map, and hence we append it here.
     known_types.append("enumeration")
     known_types.append("leafref")
+    base_types = copy.deepcopy(known_types)
+    process_typedefs_ordered = []
 
-    # Don't allow duplicate definitions of types
-    if type_name in known_types:
-      raise TypeError("Duplicate definition of %s" % type_name)
-    default_stmt = item.search_one('default')
-
-    # 'elemtype' is a list when the type includes a union, so we need to go
-    # through and build a type definition that supports multiple types.
-    if not isinstance(elemtype, list):
-      # Map the original type to the new type, parsing the additional arguments
-      # that may be specified, for example, a new default, a pattern that must
-      # be matched, or a length (stored in the restriction_argument, and
-      # restriction_type class_map variables).
-      class_map[type_name] = {"base_type": False}
-      class_map[type_name]["native_type"] = elemtype["native_type"]
-      if "parent_type" in elemtype:
-        class_map[type_name]["parent_type"] = elemtype["parent_type"]
-      else:
-        yang_type = item.search_one('type').arg
-        if yang_type not in known_types:
-          raise TypeError("typedef specified a native type that was not " +
-                            "supported")
-        class_map[type_name]["parent_type"] = yang_type
-      if default_stmt is not None:
-        class_map[type_name]["default"] = default_stmt.arg
-      if "referenced_path" in elemtype:
-        class_map[type_name]["referenced_path"] = elemtype["referenced_path"]
-        class_map[type_name]["class_override"] = "leafref"
-      if "require_instance" in elemtype:
-        class_map[type_name]["require_instance"] = elemtype["require_instance"]
-      if "restriction_type" in elemtype:
-        class_map[type_name]["restriction_type"] = \
-            elemtype["restriction_type"]
-        class_map[type_name]["restriction_argument"] = \
-                                              elemtype["restriction_argument"]
-      if "quote_arg" in elemtype:
-        class_map[type_name]["quote_arg"] = elemtype["quote_arg"]
-    else:
-      # Handle a typedef that is a union - extended the class_map arguments
-      # to be a list that is parsed by the relevant dynamic type generation
-      # function.
-      native_type = []
-      parent_type = []
-      default = False if default_stmt is None else default_stmt.arg
-      for i in elemtype:
+    while len(unresolved_t):
+        t = unresolved_t.pop(0)
+        base_t = defnd[t].search_one("type")
+        if base_t.arg == "union":
+            subtypes = []
+            for i in base_t.search("type"):
+                if i.arg == "identityref":
+                    subtypes.append(i.search_one("base"))
+                else:
+                    subtypes.append(i)
+        elif base_t.arg == "identityref":
+            subtypes = [base_t.search_one("base")]
+        else:
+            subtypes = [base_t]
 
-        if isinstance(i[1]["native_type"], list):
-          native_type.extend(i[1]["native_type"])
+        any_unknown = False
+        for i in subtypes:
+            # Resolve this typedef to the module that it
+            # was defined by
+
+            if ":" in i.arg:
+                defining_module = util.prefix_to_module(
+                    defnd[t].i_module, i.arg.split(":")[0], defnd[t].pos, ctx.errors
+                )
+            else:
+                defining_module = defnd[t].i_module
+
+            belongs_to = defining_module.search_one("belongs-to")
+            if belongs_to is not None:
+                for mod in ctx.modules:
+                    if mod[0] == belongs_to.arg:
+                        defining_module = ctx.modules[mod]
+
+            real_pfx = defining_module.search_one("prefix").arg
+
+            if ":" in i.arg:
+                tn = "%s:%s" % (real_pfx, i.arg.split(":")[1])
+            elif i.arg not in base_types:
+                # If this was not a base type (defined in YANG) then resolve it
+                # to the module it belongs to.
+                tn = "%s:%s" % (real_pfx, i.arg)
+            else:
+                tn = i.arg
+
+            if tn not in known_types:
+                any_unknown = True
+
+        if not any_unknown:
+            process_typedefs_ordered.append((t, defnd[t]))
+            known_types.append(t)
         else:
-          native_type.append(i[1]["native_type"])
+            unresolved_tc[t] += 1
+            if unresolved_tc[t] > 1000:
+                # Take a similar approach to the resolution of identities. If we have a
+                # typedef that has a type in it that is not found after many iterations
+                # then we should bail.
+                error_ids.append(t)
+                sys.stderr.write("could not find a match for %s type -> %s\n" % (t, [i.arg for i in subtypes]))
+            else:
+                unresolved_t.append(t)
+
+    if error_ids:
+        raise TypeError("could not resolve typedefs %s" % error_ids)
 
-        if i[1]["yang_type"] in known_types:
-          parent_type.append(i[1]["yang_type"])
-        elif i[1]["yang_type"] == "identityref":
-          parent_type.append(i[1]["parent_type"])
+    # Process the types that we built above.
+    for i_tuple in process_typedefs_ordered:
+        item = i_tuple[1]
+        type_name = i_tuple[0]
+        # Copy the class_map entry - this is done so that we do not alter the
+        # existing instance in memory as we add to it.
+        cls, elemtype = copy.deepcopy(build_elemtype(ctx, item.search_one("type")))
+        known_types = list(class_map.keys())
+        # Enumeration is a native type, but is not natively supported
+        # in the class_map, and hence we append it here.
+        known_types.append("enumeration")
+        known_types.append("leafref")
+
+        # Don't allow duplicate definitions of types
+        if type_name in known_types:
+            raise TypeError("Duplicate definition of %s" % type_name)
+        default_stmt = item.search_one("default")
+
+        # 'elemtype' is a list when the type includes a union, so we need to go
+        # through and build a type definition that supports multiple types.
+        if not isinstance(elemtype, list):
+            # Map the original type to the new type, parsing the additional arguments
+            # that may be specified, for example, a new default, a pattern that must
+            # be matched, or a length (stored in the restriction_argument, and
+            # restriction_type class_map variables).
+            class_map[type_name] = {"base_type": False}
+            class_map[type_name]["native_type"] = elemtype["native_type"]
+            if "parent_type" in elemtype:
+                class_map[type_name]["parent_type"] = elemtype["parent_type"]
+            else:
+                yang_type = item.search_one("type").arg
+                if yang_type not in known_types:
+                    raise TypeError("typedef specified a native type that was not " + "supported")
+                class_map[type_name]["parent_type"] = yang_type
+            if default_stmt is not None:
+                class_map[type_name]["default"] = default_stmt.arg
+            if "referenced_path" in elemtype:
+                class_map[type_name]["referenced_path"] = elemtype["referenced_path"]
+                class_map[type_name]["class_override"] = "leafref"
+            if "require_instance" in elemtype:
+                class_map[type_name]["require_instance"] = elemtype["require_instance"]
+            if "restriction_type" in elemtype:
+                class_map[type_name]["restriction_type"] = elemtype["restriction_type"]
+                class_map[type_name]["restriction_argument"] = elemtype["restriction_argument"]
+            if "quote_arg" in elemtype:
+                class_map[type_name]["quote_arg"] = elemtype["quote_arg"]
         else:
-          msg = "typedef in a union specified a native type that was not"
-          msg += " supported (%s in %s)" % (i[1]["yang_type"], item.arg)
-          raise TypeError(msg)
-
-        if "default" in i[1] and not default:
-          # When multiple 'default' values are specified within a union that
-          # is within a typedef, then pyangbind will choose the first one.
-          q = True if "quote_arg" in i[1] else False
-          default = (i[1]["default"], q)
-      class_map[type_name] = {"native_type": native_type, "base_type": False,
-                              "parent_type": parent_type}
-      if default:
-        class_map[type_name]["default"] = default[0]
-        class_map[type_name]["quote_default"] = default[1]
-
-    class_map[type_name.split(":")[1]] = class_map[type_name]
-
-
-def get_children(ctx, fd, i_children, module, parent, path=str(),
-                 parent_cfg=True, choice=False, register_paths=True):
-
-  # Iterative function that is called for all elements that have childen
-  # data nodes in the tree. This function resolves those nodes into the
-  # relevant leaf, or container/list configuration and outputs the python
-  # code that corresponds to it to the relevant file. parent_cfg is used to
-  # ensure that where a parent container was set to config false, this is
-  # inherited by all elements below it; and choice is used to store whether
-  # these leaves are within a choice or not.
-  elements = []
-  choices = False
-
-  # When pyangbind was asked to split classes, then we need to create the
-  # relevant directories for the modules to be created into. In this case
-  # even though fd might be a valid file handle, we ignore it.
-  if ctx.opts.split_class_dir:
-    if path == "":
-      fpath = ctx.pybind_split_basepath + "/__init__.py"
-    else:
-      pparts = path.split("/")
-      npath = "/"
+            # Handle a typedef that is a union - extended the class_map arguments
+            # to be a list that is parsed by the relevant dynamic type generation
+            # function.
+            native_type = []
+            parent_type = []
+            default = False if default_stmt is None else default_stmt.arg
+            for i in elemtype:
+
+                if isinstance(i[1]["native_type"], list):
+                    native_type.extend(i[1]["native_type"])
+                else:
+                    native_type.append(i[1]["native_type"])
 
-      # Check that we don't have the problem of containers that are nested
-      # with the same name
-      for i in range(1, len(pparts)):
-        if i > 0 and pparts[i] == pparts[i - 1]:
-          pname = safe_name(pparts[i]) + "_"
-        elif i == 1 and pparts[i] == module.arg:
-          pname = safe_name(pparts[i]) + "_"
+                if i[1]["yang_type"] in known_types:
+                    parent_type.append(i[1]["yang_type"])
+                elif i[1]["yang_type"] == "identityref":
+                    parent_type.append(i[1]["parent_type"])
+                else:
+                    msg = "typedef in a union specified a native type that was not"
+                    msg += " supported (%s in %s)" % (i[1]["yang_type"], item.arg)
+                    raise TypeError(msg)
+
+                if "default" in i[1] and not default:
+                    # When multiple 'default' values are specified within a union that
+                    # is within a typedef, then pyangbind will choose the first one.
+                    q = True if "quote_arg" in i[1] else False
+                    default = (i[1]["default"], q)
+            class_map[type_name] = {"native_type": native_type, "base_type": False, "parent_type": parent_type}
+            if default:
+                class_map[type_name]["default"] = default[0]
+                class_map[type_name]["quote_default"] = default[1]
+
+        class_map[type_name.split(":")[1]] = class_map[type_name]
+
+
+def get_children(ctx, fd, i_children, module, parent, path=str(), parent_cfg=True, choice=False, register_paths=True):
+
+    # Iterative function that is called for all elements that have childen
+    # data nodes in the tree. This function resolves those nodes into the
+    # relevant leaf, or container/list configuration and outputs the python
+    # code that corresponds to it to the relevant file. parent_cfg is used to
+    # ensure that where a parent container was set to config false, this is
+    # inherited by all elements below it; and choice is used to store whether
+    # these leaves are within a choice or not.
+    elements = []
+    choices = False
+
+    # When pyangbind was asked to split classes, then we need to create the
+    # relevant directories for the modules to be created into. In this case
+    # even though fd might be a valid file handle, we ignore it.
+    if ctx.opts.split_class_dir:
+        if path == "":
+            fpath = ctx.pybind_split_basepath + "/__init__.py"
         else:
-          pname = safe_name(pparts[i])
-        npath += pname + "/"
+            pparts = path.split("/")
+            npath = "/"
 
-      bpath = ctx.pybind_split_basepath + npath
-      if not os.path.exists(bpath):
-        os.makedirs(bpath)
-      fpath = bpath + "/__init__.py"
-    if not os.path.exists(fpath):
-      try:
-        if six.PY3:
-          nfd = open(fpath, 'w', encoding="utf-8")
+            # Check that we don't have the problem of containers that are nested
+            # with the same name
+            for i in range(1, len(pparts)):
+                if i > 0 and pparts[i] == pparts[i - 1]:
+                    pname = safe_name(pparts[i]) + "_"
+                elif i == 1 and pparts[i] == module.arg:
+                    pname = safe_name(pparts[i]) + "_"
+                else:
+                    pname = safe_name(pparts[i])
+                npath += pname + "/"
+
+            bpath = ctx.pybind_split_basepath + npath
+            if not os.path.exists(bpath):
+                os.makedirs(bpath)
+            fpath = bpath + "/__init__.py"
+        if not os.path.exists(fpath):
+            try:
+                if six.PY3:
+                    nfd = open(fpath, "w", encoding="utf-8")
+                else:
+                    nfd = codecs.open(fpath, "w", encoding="utf-8")
+            except IOError as m:
+                raise IOError("could not open pyangbind output file (%s)" % m)
+            nfd.write(ctx.pybind_common_hdr)
         else:
-          nfd = codecs.open(fpath, 'w', encoding="utf-8")
-      except IOError as m:
-        raise IOError("could not open pyangbind output file (%s)" % m)
-      nfd.write(ctx.pybind_common_hdr)
+            try:
+                if six.PY3:
+                    nfd = open(fpath, "a", encoding="utf-8")
+                else:
+                    nfd = codecs.open(fpath, "a", encoding="utf-8")
+            except IOError as w:
+                raise IOError("could not open pyangbind output file (%s)" % w)
     else:
-      try:
-        if six.PY3:
-          nfd = open(fpath, 'a', encoding="utf-8")
+        # If we weren't asked to split the files, then just use the file handle
+        # provided.
+        nfd = fd
+
+    if parent_cfg:
+        # The first time we find a container that has config false set on it
+        # then we need to hand this down the tree - we don't need to look if
+        # parent_cfg has already been set to False as we need to inherit.
+        parent_config = parent.search_one("config")
+        if parent_config is not None:
+            parent_config = parent_config.arg
+            if parent_config.upper() == "FALSE":
+                # this container is config false
+                parent_cfg = False
+
+    # When we are asked to split the classes into modules, then we need to find
+    # all elements that have their own class within this container, and make sure
+    # that they are imported. Additionally, we need to find the elements that are
+    # within a case, and ensure that these are built with the corresponding
+    # choice specified.
+    if ctx.opts.split_class_dir:
+        import_req = []
+
+    for ch in i_children:
+        children_tmp = getattr(ch, "i_children", None)
+        if children_tmp is not None:
+            children_tmp = [i.arg for i in children_tmp]
+        if ch.keyword == "choice":
+            for choice_ch in ch.i_children:
+                # these are case statements
+                for case_ch in choice_ch.i_children:
+                    elements += get_element(
+                        ctx,
+                        fd,
+                        case_ch,
+                        module,
+                        parent,
+                        path + "/" + case_ch.arg,
+                        parent_cfg=parent_cfg,
+                        choice=(ch.arg, choice_ch.arg),
+                        register_paths=register_paths,
+                    )
+                    if ctx.opts.split_class_dir:
+                        if hasattr(case_ch, "i_children") and len(case_ch.i_children):
+                            import_req.append(case_ch.arg)
         else:
-          nfd = codecs.open(fpath, 'a', encoding="utf-8")
-      except IOError as w:
-        raise IOError("could not open pyangbind output file (%s)" % w)
-  else:
-    # If we weren't asked to split the files, then just use the file handle
-    # provided.
-    nfd = fd
-
-  if parent_cfg:
-    # The first time we find a container that has config false set on it
-    # then we need to hand this down the tree - we don't need to look if
-    # parent_cfg has already been set to False as we need to inherit.
-    parent_config = parent.search_one('config')
-    if parent_config is not None:
-      parent_config = parent_config.arg
-      if parent_config.upper() == "FALSE":
-        # this container is config false
-        parent_cfg = False
-
-  # When we are asked to split the classes into modules, then we need to find
-  # all elements that have their own class within this container, and make sure
-  # that they are imported. Additionally, we need to find the elements that are
-  # within a case, and ensure that these are built with the corresponding
-  # choice specified.
-  if ctx.opts.split_class_dir:
-    import_req = []
-
-  for ch in i_children:
-    children_tmp = getattr(ch, "i_children", None)
-    if children_tmp is not None:
-      children_tmp = [i.arg for i in children_tmp]
-    if ch.keyword == "choice":
-      for choice_ch in ch.i_children:
-        # these are case statements
-        for case_ch in choice_ch.i_children:
-          elements += get_element(ctx, fd, case_ch, module, parent,
-            path + "/" + case_ch.arg, parent_cfg=parent_cfg,
-            choice=(ch.arg, choice_ch.arg), register_paths=register_paths)
-          if ctx.opts.split_class_dir:
-            if hasattr(case_ch, "i_children") and len(case_ch.i_children):
-              import_req.append(case_ch.arg)
-    else:
-      elements += get_element(ctx, fd, ch, module, parent, path + "/" + ch.arg,
-        parent_cfg=parent_cfg, choice=choice, register_paths=register_paths)
+            elements += get_element(
+                ctx,
+                fd,
+                ch,
+                module,
+                parent,
+                path + "/" + ch.arg,
+                parent_cfg=parent_cfg,
+                choice=choice,
+                register_paths=register_paths,
+            )
+
+            if ctx.opts.split_class_dir:
+                if hasattr(ch, "i_children") and len(ch.i_children):
+                    import_req.append(ch.arg)
 
-      if ctx.opts.split_class_dir:
-        if hasattr(ch, "i_children") and len(ch.i_children):
-          import_req.append(ch.arg)
-
-  # Write out the import statements if needed.
-  if ctx.opts.split_class_dir:
-    if len(import_req):
-      for im in import_req:
-        if im == parent.arg:
-          im += "_"
-        # Relative import in PY2/PY3 compatible style
-        nfd.write("from . import {}\n".format(safe_name(im)))
-
-  # 'container', 'module', 'list' and 'submodule' all have their own classes
-  # generated.
-  if parent.keyword in ["container", "module", "list", "submodule", "input",
-                         "output", "rpc", "notification"]:
+    # Write out the import statements if needed.
     if ctx.opts.split_class_dir:
-      nfd.write("class %s(PybindBase):\n" % safe_name(parent.arg))
-    else:
-      if not path == "":
-        nfd.write("class yc_%s_%s_%s(PybindBase):\n" % (safe_name(parent.arg),
-          safe_name(module.arg), safe_name(path.replace("/", "_"))))
-      else:
-        nfd.write("class %s(PybindBase):\n" % safe_name(parent.arg))
-
-    # If the container is actually a list, then determine what the key value
-    # is and store this such that we can give a hint.
-    keyval = False
-    if parent.keyword == "list":
-      keyval = parent.search_one('key').arg if parent.search_one('key') \
-          is not None else False
-      if keyval and " " in keyval:
-        keyval = keyval.split(" ")
-      else:
-        keyval = [keyval]
-
-    # Auto-generate a docstring based on the description that is provided in
-    # the YANG module. This aims to provide readability to someone perusing the
-    # code that is generated.
-    parent_descr = parent.search_one('description')
-    if parent_descr is not None:
-      parent_descr = "\n\n  YANG Description: %s" % parent_descr.arg
-    else:
-      parent_descr = ""
+        if len(import_req):
+            for im in import_req:
+                if im == parent.arg:
+                    im += "_"
+                # Relative import in PY2/PY3 compatible style
+                nfd.write("from . import {}\n".format(safe_name(im)))
+
+    # 'container', 'module', 'list' and 'submodule' all have their own classes
+    # generated.
+    if parent.keyword in ["container", "module", "list", "submodule", "input", "output", "rpc", "notification"]:
+        if ctx.opts.split_class_dir:
+            nfd.write("class %s(PybindBase):\n" % safe_name(parent.arg))
+        else:
+            if not path == "":
+                nfd.write(
+                    "class yc_%s_%s_%s(PybindBase):\n"
+                    % (safe_name(parent.arg), safe_name(module.arg), safe_name(path.replace("/", "_")))
+                )
+            else:
+                nfd.write("class %s(PybindBase):\n" % safe_name(parent.arg))
 
-    # Add more helper text.
-    nfd.write('''  """
+        # If the container is actually a list, then determine what the key value
+        # is and store this such that we can give a hint.
+        keyval = False
+        if parent.keyword == "list":
+            keyval = parent.search_one("key").arg if parent.search_one("key") is not None else False
+            if keyval and " " in keyval:
+                keyval = keyval.split(" ")
+            else:
+                keyval = [keyval]
+
+        # Auto-generate a docstring based on the description that is provided in
+        # the YANG module. This aims to provide readability to someone perusing the
+        # code that is generated.
+        parent_descr = parent.search_one("description")
+        if parent_descr is not None:
+            parent_descr = "\n\n  YANG Description: %s" % parent_descr.arg
+        else:
+            parent_descr = ""
+
+        # Add more helper text.
+        nfd.write(
+            '''  """
   This class was auto-generated by the PythonClass plugin for PYANG
   from YANG module %s - based on the path %s. Each member element of
   the container is represented as a class variable - with a specific
   YANG type.%s
-  """\n''' % (module.arg, (path if not path == "" else "/%s" % parent.arg),
-              parent_descr))
-  else:
-    raise TypeError("unhandled keyword with children %s at %s" %
-      (parent.keyword, parent.pos))
-
-  elements_str = ""
-  if len(elements) == 0:
-    nfd.write("  _pyangbind_elements = {}")
-  else:
-    # We want to prevent a user from creating new attributes on a class that
-    # are not allowed within the data model - this uses the __slots__ magic
-    # variable of the class to restrict anyone from adding to these classes.
-    # Doing so gives an AttributeError when a user tries to specify something
-    # that was not in the model.
-    elements_str = "_pyangbind_elements = OrderedDict(["
-    slots_str = "  __slots__ = ('_path_helper',"
-    slots_str += " '_extmethods', "
-    for i in elements:
-      slots_str += "'__%s'," % i["name"]
-      elements_str += "('%s', %s), " % (i["name"], i["name"])
-    slots_str += ")\n"
-    elements_str += "])\n"
-    nfd.write(slots_str + "\n")
-    # Store the real name of the element - since we often get values that are
-    # not allowed in python as identifiers, but we need the real-name when
-    # creating instance documents (e.g., peer-group is not valid due to '-').
-    nfd.write("  _yang_name = '%s'\n" % (parent.arg))
-
-    choices = {}
-    choice_attrs = []
-    classes = {}
-    for i in elements:
-      # Loop through the elements and build a string that corresponds to the
-      # class that is going to be created. In all cases (thus far) this uses
-      # the YANGDynClass helper function to generate a dynamic type. This
-      # can extend the base type that is provided, and does this to give us
-      # some attributes that base classes such as int(), or str() don't have -
-      # but YANG needs (such as a default value, the original YANG name, any
-      # extension that were provided with the leaf, etc.).
-      class_str = {}
-      if "default" in i and not i["default"] is None:
-        default_arg = "\"%s\"" % (i["default"]) if i["quote_arg"] else "%s" \
-            % i["default"]
-
-      if i["class"] == "leaf-list":
-        # Map a leaf-list to the type specified in the class map. This is a
-        # TypedList (see lib.yangtypes) with a particular set of types allowed.
-        class_str["name"] = "__%s" % (i["name"])
-        class_str["type"] = "YANGDynClass"
-        class_str["arg"] = "unique=True, base="
-        if isinstance(i["type"]["native_type"][1], list):
-          allowed_type = "["
-          for subtype in i["type"]["native_type"][1]:
-            allowed_type += "%s," % subtype
-          allowed_type += "]"
-        else:
-          allowed_type = "%s" % (i["type"]["native_type"][1])
-        class_str["arg"] += "%s(allowed_type=%s)" % \
-          (i["type"]["native_type"][0], allowed_type)
-        if "default" in i and not i["default"] is None:
-          class_str["arg"] += ", default=%s(%s)" % (i["defaulttype"],
-            default_arg)
-      elif i["class"] == "list":
-        # Map a list to YANGList class - this is dynamically derived by the
-        # YANGListType function to have the relevant characteristics, such as
-        # whether it is ordered by the user.
-        class_str["name"] = "__%s" % (i["name"])
-        class_str["type"] = "YANGDynClass"
-        class_str["arg"] = "base=YANGListType("
-        class_str["arg"] += "%s,%s" % ("\"%s\"" % i["key"] if i["key"]
-                                                  else False, i["type"])
-        class_str["arg"] += ", yang_name=\"%s\", parent=self" \
-            % (i["yang_name"])
-        class_str["arg"] += ", is_container='list', user_ordered=%s" \
-                                                  % i["user_ordered"]
-        class_str["arg"] += ", path_helper=self._path_helper"
-        class_str["arg"] += ", yang_keys='%s'" % i["yang_keys"]
-        class_str["arg"] += ", extensions=%s" % i["extensions"]
-        if i["choice"]:
-          class_str["arg"] += ", choice=%s" % repr(choice)
-        class_str["arg"] += ")"
-      elif i["class"] == "union" or i["class"] == "leaf-union":
-        # A special mapped type where there is a union that just includes
-        # leaves this is mapped to a particular Union type, and valid types
-        # within it. The dynamically generated class will determine whether
-        # the input can be mapped to the types included in the union.
-        class_str["name"] = "__%s" % (i["name"])
-        class_str["type"] = "YANGDynClass"
-        class_str["arg"] = "base=["
-        for u in i["type"][1]:
-          if isinstance(u[1]["native_type"], list):
-            for su_native_type in u[1]["native_type"]:
-              class_str["arg"] += "%s," % su_native_type
-          else:
-            class_str["arg"] += "%s," % u[1]["native_type"]
-        class_str["arg"] += "]"
-        if "default" in i and not i["default"] is None:
-          class_str["arg"] += ", default=%s(%s)" % (i["defaulttype"],
-            default_arg)
-      elif i["class"] == "leafref":
-        # A leafref, pyangbind uses the special ReferenceType which performs a
-        # lookup against the path_helper class provided.
-        class_str["name"] = "__%s" % (i["name"])
-        class_str["type"] = "YANGDynClass"
-        class_str["arg"] = "base=%s" % i["type"]
-        class_str["arg"] += "(referenced_path='%s'" % i["referenced_path"]
-        class_str["arg"] += ", caller=self._path() + ['%s'], " \
-                                % (i["yang_name"])
-        class_str["arg"] += "path_helper=self._path_helper, "
-        class_str["arg"] += "require_instance=%s)" % (i["require_instance"])
-      elif i["class"] == "leafref-list":
-        # Deal with the special case of a list of leafrefs, since the
-        # ReferenceType has different arguments that need to be provided to the
-        # class to properly initialise.
-        class_str["name"] = "__%s" % (i["name"])
-        class_str["type"] = "YANGDynClass"
-        class_str["arg"] = "base=%s" % i["type"]["native_type"][0]
-        class_str["arg"] += "(allowed_type=%s(referenced_path='%s'," \
-                              % (i["type"]["native_type"][1]["native_type"],
-                                i["type"]["native_type"][1]["referenced_path"])
-        class_str["arg"] += "caller=self._path() + ['%s'], " % i["yang_name"]
-        class_str["arg"] += "path_helper=self._path_helper, "
-        class_str["arg"] += "require_instance=%s))" % \
-                              (i["type"]["native_type"][1]["require_instance"])
-      else:
-        # Generically handle all other classes with the 'standard' mappings.
-        class_str["name"] = "__%s" % (i["name"])
-        class_str["type"] = "YANGDynClass"
-        if isinstance(i["type"], list):
-          class_str["arg"] = "base=["
-          for u in i["type"]:
-            class_str["arg"] += "%s," % u
-          class_str["arg"] += "]"
+  """\n'''
+            % (module.arg, (path if not path == "" else "/%s" % parent.arg), parent_descr)
+        )
+    else:
+        raise TypeError("unhandled keyword with children %s at %s" % (parent.keyword, parent.pos))
+
+    elements_str = ""
+    if len(elements) == 0:
+        nfd.write("  _pyangbind_elements = {}")
+    else:
+        # We want to prevent a user from creating new attributes on a class that
+        # are not allowed within the data model - this uses the __slots__ magic
+        # variable of the class to restrict anyone from adding to these classes.
+        # Doing so gives an AttributeError when a user tries to specify something
+        # that was not in the model.
+        elements_str = "_pyangbind_elements = OrderedDict(["
+        slots_str = "  __slots__ = ('_path_helper',"
+        slots_str += " '_extmethods', "
+        for i in elements:
+            slots_str += "'__%s'," % i["name"]
+            elements_str += "('%s', %s), " % (i["name"], i["name"])
+        slots_str += ")\n"
+        elements_str += "])\n"
+        nfd.write(slots_str + "\n")
+        # Store the real name of the element - since we often get values that are
+        # not allowed in python as identifiers, but we need the real-name when
+        # creating instance documents (e.g., peer-group is not valid due to '-').
+        nfd.write("  _yang_name = '%s'\n" % (parent.arg))
+
+        # Store the namespace URI for easier access during XML serialisation
+        if module.keyword == "submodule":
+            mod_location = next(v for k, v in ctx.modules.items() if k[0] == module.i_modulename)
         else:
-          class_str["arg"] = "base=%s" % i["type"]
-        if "default" in i and not i["default"] is None:
-          class_str["arg"] += ", default=%s(%s)" % (i["defaulttype"],
-                                                        default_arg)
-      if i["class"] == "container":
-        class_str["arg"] += ", is_container='container'"
-        if ctx.opts.generate_presence:
-          class_str["arg"] += ", presence=%s" % i["presence"]
-      elif i["class"] == "list":
-        class_str["arg"] += ", is_container='list'"
-      elif i["class"] == "leaf-list":
-        class_str["arg"] += ", is_leaf=False"
-      else:
-        class_str["arg"] += ", is_leaf=True"
-      if class_str["arg"]:
-        class_str["arg"] += ", yang_name=\"%s\"" % i["yang_name"]
-        class_str["arg"] += ", parent=self"
-        if i["choice"]:
-          class_str["arg"] += ", choice=%s" % repr(i["choice"])
-          choice_attrs.append(i["name"])
-          if not i["choice"][0] in choices:
-            choices[i["choice"][0]] = {}
-          if not i["choice"][1] in choices[i["choice"][0]]:
-            choices[i["choice"][0]][i["choice"][1]] = []
-          choices[i["choice"][0]][i["choice"][1]].append(i["name"])
-        class_str["arg"] += ", path_helper=self._path_helper"
-        class_str["arg"] += ", extmethods=self._extmethods"
-        class_str["arg"] += ", register_paths=%s" % i["register_paths"]
-        if "extensions" in i:
-          class_str["arg"] += ", extensions=%s" % i["extensions"]
-        if keyval and i["yang_name"] in keyval:
-          class_str["arg"] += ", is_keyval=True"
-        class_str["arg"] += ", namespace='%s'" % i["namespace"]
-        class_str["arg"] += ", defining_module='%s'" % i["defining_module"]
-        class_str["arg"] += ", yang_type='%s'" % i["origtype"]
-        class_str["arg"] += ", is_config=%s" % (i["config"] and parent_cfg)
-        classes[i["name"]] = class_str
-
-    # TODO: get and set methods currently have errors that are reported that
-    # are a bit ugly. The intention here is to act like an immutable type -
-    # such that new class instances are created each time that the value is
-    # set.
+            mod_location = module
+        nfd.write("  _yang_namespace = '%s'\n" % (mod_location.search("namespace")[0].arg))
 
-    # Generic class __init__, set up the path_helper if asked to.
-    nfd.write("""
+        choices = {}
+        choice_attrs = []
+        classes = {}
+        for i in elements:
+            # Loop through the elements and build a string that corresponds to the
+            # class that is going to be created. In all cases (thus far) this uses
+            # the YANGDynClass helper function to generate a dynamic type. This
+            # can extend the base type that is provided, and does this to give us
+            # some attributes that base classes such as int(), or str() don't have -
+            # but YANG needs (such as a default value, the original YANG name, any
+            # extension that were provided with the leaf, etc.).
+            class_str = {}
+            if "default" in i and not i["default"] is None:
+                default_arg = '"%s"' % (i["default"]) if i["quote_arg"] else "%s" % i["default"]
+
+            if i["class"] == "leaf-list":
+                # Map a leaf-list to the type specified in the class map. This is a
+                # TypedList (see lib.yangtypes) with a particular set of types allowed.
+                class_str["name"] = "__%s" % (i["name"])
+                class_str["type"] = "YANGDynClass"
+                class_str["arg"] = "unique=True, base="
+                if isinstance(i["type"]["native_type"][1], list):
+                    allowed_type = "["
+                    for subtype in i["type"]["native_type"][1]:
+                        allowed_type += "%s," % subtype
+                    allowed_type += "]"
+                else:
+                    allowed_type = "%s" % (i["type"]["native_type"][1])
+                class_str["arg"] += "%s(allowed_type=%s)" % (i["type"]["native_type"][0], allowed_type)
+                if "default" in i and not i["default"] is None:
+                    class_str["arg"] += ", default=%s(%s)" % (i["defaulttype"], default_arg)
+            elif i["class"] == "list":
+                # Map a list to YANGList class - this is dynamically derived by the
+                # YANGListType function to have the relevant characteristics, such as
+                # whether it is ordered by the user.
+                class_str["name"] = "__%s" % (i["name"])
+                class_str["type"] = "YANGDynClass"
+                class_str["arg"] = "base=YANGListType("
+                class_str["arg"] += "%s,%s" % ('"%s"' % i["key"] if i["key"] else False, i["type"])
+                class_str["arg"] += ', yang_name="%s", parent=self' % (i["yang_name"])
+                class_str["arg"] += ", is_container='list', user_ordered=%s" % i["user_ordered"]
+                class_str["arg"] += ", path_helper=self._path_helper"
+                class_str["arg"] += ", yang_keys='%s'" % i["yang_keys"]
+                class_str["arg"] += ", extensions=%s" % i["extensions"]
+                if i["choice"]:
+                    class_str["arg"] += ", choice=%s" % repr(choice)
+                class_str["arg"] += ")"
+            elif i["class"] == "union" or i["class"] == "leaf-union":
+                # A special mapped type where there is a union that just includes
+                # leaves this is mapped to a particular Union type, and valid types
+                # within it. The dynamically generated class will determine whether
+                # the input can be mapped to the types included in the union.
+                class_str["name"] = "__%s" % (i["name"])
+                class_str["type"] = "YANGDynClass"
+                class_str["arg"] = "base=["
+                for u in i["type"][1]:
+                    if isinstance(u[1]["native_type"], list):
+                        for su_native_type in u[1]["native_type"]:
+                            class_str["arg"] += "%s," % su_native_type
+                    else:
+                        class_str["arg"] += "%s," % u[1]["native_type"]
+                class_str["arg"] += "]"
+                if "default" in i and not i["default"] is None:
+                    class_str["arg"] += ", default=%s(%s)" % (i["defaulttype"], default_arg)
+            elif i["class"] == "leafref":
+                # A leafref, pyangbind uses the special ReferenceType which performs a
+                # lookup against the path_helper class provided.
+                class_str["name"] = "__%s" % (i["name"])
+                class_str["type"] = "YANGDynClass"
+                class_str["arg"] = "base=%s" % i["type"]
+                class_str["arg"] += "(referenced_path='%s'" % i["referenced_path"]
+                class_str["arg"] += ", caller=self._path() + ['%s'], " % (i["yang_name"])
+                class_str["arg"] += "path_helper=self._path_helper, "
+                class_str["arg"] += "require_instance=%s)" % (i["require_instance"])
+            elif i["class"] == "leafref-list":
+                # Deal with the special case of a list of leafrefs, since the
+                # ReferenceType has different arguments that need to be provided to the
+                # class to properly initialise.
+                class_str["name"] = "__%s" % (i["name"])
+                class_str["type"] = "YANGDynClass"
+                class_str["arg"] = "base=%s" % i["type"]["native_type"][0]
+                class_str["arg"] += "(allowed_type=%s(referenced_path='%s'," % (
+                    i["type"]["native_type"][1]["native_type"],
+                    i["type"]["native_type"][1]["referenced_path"],
+                )
+                class_str["arg"] += "caller=self._path() + ['%s'], " % i["yang_name"]
+                class_str["arg"] += "path_helper=self._path_helper, "
+                class_str["arg"] += "require_instance=%s))" % (i["type"]["native_type"][1]["require_instance"])
+            else:
+                # Generically handle all other classes with the 'standard' mappings.
+                class_str["name"] = "__%s" % (i["name"])
+                class_str["type"] = "YANGDynClass"
+                if isinstance(i["type"], list):
+                    class_str["arg"] = "base=["
+                    for u in i["type"]:
+                        class_str["arg"] += "%s," % u
+                    class_str["arg"] += "]"
+                else:
+                    class_str["arg"] = "base=%s" % i["type"]
+                if "default" in i and not i["default"] is None:
+                    class_str["arg"] += ", default=%s(%s)" % (i["defaulttype"], default_arg)
+            if i["class"] == "container":
+                class_str["arg"] += ", is_container='container'"
+                if ctx.opts.generate_presence:
+                    class_str["arg"] += ", presence=%s" % i["presence"]
+            elif i["class"] == "list":
+                class_str["arg"] += ", is_container='list'"
+            elif i["class"] == "leaf-list":
+                class_str["arg"] += ", is_leaf=False"
+            else:
+                class_str["arg"] += ", is_leaf=True"
+            if class_str["arg"]:
+                class_str["arg"] += ', yang_name="%s"' % i["yang_name"]
+                class_str["arg"] += ", parent=self"
+                if i["choice"]:
+                    class_str["arg"] += ", choice=%s" % repr(i["choice"])
+                    choice_attrs.append(i["name"])
+                    if not i["choice"][0] in choices:
+                        choices[i["choice"][0]] = {}
+                    if not i["choice"][1] in choices[i["choice"][0]]:
+                        choices[i["choice"][0]][i["choice"][1]] = []
+                    choices[i["choice"][0]][i["choice"][1]].append(i["name"])
+                class_str["arg"] += ", path_helper=self._path_helper"
+                class_str["arg"] += ", extmethods=self._extmethods"
+                class_str["arg"] += ", register_paths=%s" % i["register_paths"]
+                if "extensions" in i:
+                    class_str["arg"] += ", extensions=%s" % i["extensions"]
+                if keyval and i["yang_name"] in keyval:
+                    class_str["arg"] += ", is_keyval=True"
+                class_str["arg"] += ", namespace='%s'" % i["namespace"]
+                class_str["arg"] += ", defining_module='%s'" % i["defining_module"]
+                class_str["arg"] += ", yang_type='%s'" % i["origtype"]
+                class_str["arg"] += ", is_config=%s" % (i["config"] and parent_cfg)
+                classes[i["name"]] = class_str
+
+        # TODO: get and set methods currently have errors that are reported that
+        # are a bit ugly. The intention here is to act like an immutable type -
+        # such that new class instances are created each time that the value is
+        # set.
+
+        # Generic class __init__, set up the path_helper if asked to.
+        nfd.write(
+            """
   _pybind_generated_by = 'container'
 
-  def __init__(self, *args, **kwargs):\n""")
-    if ctx.opts.use_xpathhelper:
-      nfd.write("""
+  def __init__(self, *args, **kwargs):\n"""
+        )
+        if ctx.opts.use_xpathhelper:
+            nfd.write(
+                """
     helper = kwargs.pop("path_helper", None)
     if helper is False:
       self._path_helper = False
     elif helper is not None and isinstance(helper, xpathhelper.YANGPathHelper):
       self._path_helper = helper
     elif hasattr(self, "_parent"):
       helper = getattr(self._parent, "_path_helper", False)
       self._path_helper = helper
     else:
-      self._path_helper = False\n""")
-    else:
-      nfd.write("""
-    self._path_helper = False\n""")
-
-    if ctx.opts.use_extmethods:
-      nfd.write("""
+      self._path_helper = False\n"""
+            )
+        else:
+            nfd.write(
+                """
+    self._path_helper = False\n"""
+            )
+
+        if ctx.opts.use_extmethods:
+            nfd.write(
+                """
     extmethods = kwargs.pop("extmethods", None)
     if extmethods is False:
       self._extmethods = False
     elif extmethods is not None and isinstance(extmethods, dict):
       self._extmethods = extmethods
     elif hasattr(self, "_parent"):
       extmethods = getattr(self._parent, "_extmethods", None)
       self._extmethods = extmethods
     else:
-      self._extmethods = False\n""")
-    else:
-      nfd.write("""
-    self._extmethods = False\n""")
-
-    # Write out the classes that are stored locally as self.__foo where
-    # foo is the safe YANG name.
-    for c in classes:
-      nfd.write("    self.%s = %s(%s)\n" % (classes[c]["name"],
-                                  classes[c]["type"], classes[c]["arg"]))
-    # Don't accept arguments to a container/list/submodule class
-    nfd.write("""
+      self._extmethods = False\n"""
+            )
+        else:
+            nfd.write(
+                """
+    self._extmethods = False\n"""
+            )
+
+        # Write out the classes that are stored locally as self.__foo where
+        # foo is the safe YANG name.
+        for c in classes:
+            nfd.write("    self.%s = %s(%s)\n" % (classes[c]["name"], classes[c]["type"], classes[c]["arg"]))
+        # Don't accept arguments to a container/list/submodule class
+        nfd.write(
+            """
     load = kwargs.pop("load", None)
     if args:
       if len(args) > 1:
         raise TypeError("cannot create a YANG container with >1 argument")
       all_attr = True
       for e in self._pyangbind_elements:
         if not hasattr(args[0], e):
@@ -1031,612 +1058,644 @@
         nobj = getattr(args[0], e)
         if nobj._changed() is False:
           continue
         setmethod = getattr(self, "_set_%s" % e)
         if load is None:
           setmethod(getattr(args[0], e))
         else:
-          setmethod(getattr(args[0], e), load=load)\n""")
+          setmethod(getattr(args[0], e), load=load)\n"""
+        )
 
-    # A generic method to provide a path() method on each container, that gives
-    # a path in the form of a list that describes the nodes in the hierarchy.
-    nfd.write("""
+        # A generic method to provide a path() method on each container, that gives
+        # a path in the form of a list that describes the nodes in the hierarchy.
+        nfd.write(
+            """
   def _path(self):
     if hasattr(self, "_parent"):
       return self._parent._path()+[self._yang_name]
     else:
-      return %s\n""" % path.split("/")[1:])
-
-    # For each element, write out a getter and setter method - with the doc
-    # string of the element within the model.
-    for i in elements:
-      c_str = classes[i["name"]]
-      description_str = ""
-      if i["description"]:
-        description_str = "\n\n    YANG Description: %s" % i['description']
-      nfd.write('''
+      return %s\n"""
+            % path.split("/")[1:]
+        )
+
+        # For each element, write out a getter and setter method - with the doc
+        # string of the element within the model.
+        for i in elements:
+            c_str = classes[i["name"]]
+            description_str = ""
+            if i["description"]:
+                description_str = "\n\n    YANG Description: %s" % i["description"]
+            nfd.write(
+                '''
   def _get_%s(self):
     """
     Getter method for %s, mapped from YANG variable %s (%s)%s
     """
     return self.__%s
-      ''' % (i["name"], i["name"], i["path"], i["origtype"],
-             description_str, i["name"]))
+      '''
+                % (i["name"], i["name"], i["path"], i["origtype"], description_str, i["name"])
+            )
 
-      nfd.write('''
+            nfd.write(
+                '''
   def _set_%s(self, v, load=False):
     """
     Setter method for %s, mapped from YANG variable %s (%s)
     If this variable is read-only (config: false) in the
     source YANG file, then _set_%s is considered as a private
     method. Backends looking to populate this variable should
     do so via calling thisObj._set_%s() directly.%s
-    """''' % (i["name"], i["name"], i["path"],
-                          i["origtype"], i["name"], i["name"],
-                          description_str))
-      if keyval and i["yang_name"] in keyval:
-        nfd.write("""
+    """'''
+                % (i["name"], i["name"], i["path"], i["origtype"], i["name"], i["name"], description_str)
+            )
+            if keyval and i["yang_name"] in keyval:
+                nfd.write(
+                    """
     parent = getattr(self, "_parent", None)
     if parent is not None and load is False:
       raise AttributeError("Cannot set keys directly when" +
-                             " within an instantiated list")\n""")
-      nfd.write("""
+                             " within an instantiated list")\n"""
+                )
+            nfd.write(
+                """
     if hasattr(v, "_utype"):
-      v = v._utype(v)""")
-      nfd.write("""
+      v = v._utype(v)"""
+            )
+            nfd.write(
+                """
     try:
-      t = %s(v,%s)""" % (c_str["type"], c_str["arg"]))
-      nfd.write("""
-    except (TypeError, ValueError):\n""")
-      nfd.write("""      raise ValueError({
+      t = %s(v,%s)"""
+                % (c_str["type"], c_str["arg"])
+            )
+            nfd.write(
+                """
+    except (TypeError, ValueError):\n"""
+            )
+            nfd.write(
+                """      raise ValueError({
           'error-string': \"\"\"%s must be of a type compatible with %s\"\"\",
           'defined-type': "%s",
           'generated-type': \"\"\"%s(%s)\"\"\",
-        })\n\n""" % (i["name"], i["origtype"],
-                  "%s:%s" % (i["defining_module"], i["origtype"]) if ":"
-                  not in i["origtype"] and not i["origtype"] in
-                  YANG_BUILTIN_TYPES else i["origtype"], c_str["type"],
-                  c_str["arg"]))
-      nfd.write("    self.__%s = t\n" % (i["name"]))
-      nfd.write("    if hasattr(self, '_set'):\n")
-      nfd.write("      self._set()\n")
-
-      # When we want to return a value to its default, the unset method can
-      # be used. Generally, this is done in a choice where one branch needs to
-      # be set to the default, but may be used wherever re-initialiation of
-      # the object is required.
-      nfd.write("""
+        })\n\n"""
+                % (
+                    i["name"],
+                    i["origtype"],
+                    "%s:%s" % (i["defining_module"], i["origtype"])
+                    if ":" not in i["origtype"] and not i["origtype"] in YANG_BUILTIN_TYPES
+                    else i["origtype"],
+                    c_str["type"],
+                    c_str["arg"],
+                )
+            )
+            nfd.write("    self.__%s = t\n" % (i["name"]))
+            nfd.write("    if hasattr(self, '_set'):\n")
+            nfd.write("      self._set()\n")
+
+            # When we want to return a value to its default, the unset method can
+            # be used. Generally, this is done in a choice where one branch needs to
+            # be set to the default, but may be used wherever re-initialiation of
+            # the object is required.
+            nfd.write(
+                """
   def _unset_%s(self):
-    self.__%s = %s(%s)\n\n""" % (i["name"], i["name"],
-                                  c_str["type"], c_str["arg"],))
+    self.__%s = %s(%s)\n\n"""
+                % (i["name"], i["name"], c_str["type"], c_str["arg"])
+            )
+
+        # When an element is read-only, write out the _set and _get methods, but
+        # we don't actually make the property object accessible. This ensures that
+        # where backends are populating the model, then they can do so via the
+        # _set_X method - but a 'normal' user can't just do container.X = 10.
+        for i in elements:
+            rw = True
+            if not i["config"]:
+                rw = False
+            elif not parent_cfg:
+                rw = False
 
-    # When an element is read-only, write out the _set and _get methods, but
-    # we don't actually make the property object accessible. This ensures that
-    # where backends are populating the model, then they can do so via the
-    # _set_X method - but a 'normal' user can't just do container.X = 10.
-    for i in elements:
-      rw = True
-      if not i["config"]:
-        rw = False
-      elif not parent_cfg:
-        rw = False
-
-      if not rw:
-        nfd.write("""  %s = __builtin__.property(_get_%s)\n""" % (i["name"], i["name"]))
-      else:
-        nfd.write("""  %s = __builtin__.property(_get_%s, _set_%s)\n""" %
-                          (i["name"], i["name"], i["name"]))
-  nfd.write("\n")
-
-  # Store a list of the choices that are included within this module such that
-  # we can enforce each branch.
-  if choices:
-    nfd.write("  __choices__ = %s" % repr(choices))
-  nfd.write("""\n  %s\n""" % elements_str)
-  nfd.write("\n")
-
-  try:
-    nfd.flush()
-    os.fsync(nfd.fileno())
-  except OSError:
-    pass
+            if not rw:
+                nfd.write("""  %s = __builtin__.property(_get_%s)\n""" % (i["name"], i["name"]))
+            else:
+                nfd.write("""  %s = __builtin__.property(_get_%s, _set_%s)\n""" % (i["name"], i["name"], i["name"]))
+    nfd.write("\n")
 
-  if ctx.opts.split_class_dir:
-    nfd.close()
+    # Store a list of the choices that are included within this module such that
+    # we can enforce each branch.
+    if choices:
+        nfd.write("  __choices__ = %s" % repr(choices))
+    nfd.write("""\n  %s\n""" % elements_str)
+    nfd.write("\n")
 
-  return None
+    try:
+        nfd.flush()
+        os.fsync(nfd.fileno())
+    except OSError:
+        pass
+
+    if ctx.opts.split_class_dir:
+        nfd.close()
+
+    return None
 
 
 def build_elemtype(ctx, et, prefix=False):
-  # Build a dictionary which defines the type for the element. This is used
-  # both in the case that a typedef needs to be built, as well as on per-list
-  # basis.
-  cls = None
-  pattern_stmt = et.search_one('pattern') if not et.search_one('pattern') \
-                                              is None else False
-  range_stmt = et.search_one('range') if not et.search_one('range') \
-                                              is None else False
-  length_stmt = et.search_one('length') if not et.search_one('length') \
-                                              is None else False
-
-  # Determine whether there are any restrictions that are placed on this leaf,
-  # and build a dictionary of the different restrictions to be placed on the
-  # type.
-  restrictions = {}
-  if pattern_stmt:
-    restrictions['pattern'] = pattern_stmt.arg
-
-  if length_stmt:
-    if "|" in length_stmt.arg:
-      restrictions['length'] = [i.replace(' ', '') for i in
-                                  length_stmt.arg.split("|")]
-    else:
-      restrictions['length'] = [length_stmt.arg]
+    # Build a dictionary which defines the type for the element. This is used
+    # both in the case that a typedef needs to be built, as well as on per-list
+    # basis.
+    cls = None
+    pattern_stmt = et.search_one("pattern") if not et.search_one("pattern") is None else False
+    range_stmt = et.search_one("range") if not et.search_one("range") is None else False
+    length_stmt = et.search_one("length") if not et.search_one("length") is None else False
+
+    # Determine whether there are any restrictions that are placed on this leaf,
+    # and build a dictionary of the different restrictions to be placed on the
+    # type.
+    restrictions = {}
+    if pattern_stmt:
+        restrictions["pattern"] = pattern_stmt.arg
+
+    if length_stmt:
+        if "|" in length_stmt.arg:
+            restrictions["length"] = [i.replace(" ", "") for i in length_stmt.arg.split("|")]
+        else:
+            restrictions["length"] = [length_stmt.arg]
 
-  if range_stmt:
-    # Complex ranges are separated by pipes
-    if "|" in range_stmt.arg:
-      restrictions['range'] = [i.replace(' ', '') for i in
-                                  range_stmt.arg.split("|")]
-    else:
-      restrictions['range'] = [range_stmt.arg]
+    if range_stmt:
+        # Complex ranges are separated by pipes
+        if "|" in range_stmt.arg:
+            restrictions["range"] = [i.replace(" ", "") for i in range_stmt.arg.split("|")]
+        else:
+            restrictions["range"] = [range_stmt.arg]
 
-  # Build RestrictedClassTypes based on the compiled dictionary and the
-  # underlying base type.
-  if len(restrictions):
-    if 'length' in restrictions or 'pattern' in restrictions:
-      cls = "restricted-%s" % (et.arg)
-      elemtype = {
-          "native_type":
-              """RestrictedClassType(base_type=%s, restriction_dict=%s)"""
-              % (class_map[et.arg]["native_type"], repr(restrictions)),
-          "restriction_dict": restrictions,
-          "parent_type": et.arg,
-          "base_type": False,
-      }
-    elif 'range' in restrictions:
-      cls = "restricted-%s" % et.arg
-      elemtype = {
-          "native_type":
-              """RestrictedClassType(base_type=%s, restriction_dict=%s)"""
-              % (class_map[et.arg]["native_type"], repr(restrictions)),
-          "restriction_dict": restrictions,
-          "parent_type": et.arg,
-          "base_type": False,
-      }
-
-  # Handle all other types of leaves that are not restricted classes.
-  if cls is None:
-    cls = "leaf"
-    # Enumerations are built as RestrictedClasses where the value that is
-    # provided to the class is check against the keys of a dictionary.
-    if et.arg == "enumeration":
-      enumeration_dict = {}
-      for enum in et.search('enum'):
-        enumeration_dict[six.text_type(enum.arg)] = {}
-        val = enum.search_one('value')
-        if val is not None:
-          enumeration_dict[six.text_type(enum.arg)]["value"] = int(val.arg)
-      elemtype = {"native_type": """RestrictedClassType(base_type=six.text_type, \
+    # Build RestrictedClassTypes based on the compiled dictionary and the
+    # underlying base type.
+    if len(restrictions):
+        if "length" in restrictions or "pattern" in restrictions:
+            cls = "restricted-%s" % (et.arg)
+            elemtype = {
+                "native_type": """RestrictedClassType(base_type=%s, restriction_dict=%s)"""
+                % (class_map[et.arg]["native_type"], repr(restrictions)),
+                "restriction_dict": restrictions,
+                "parent_type": et.arg,
+                "base_type": False,
+            }
+        elif "range" in restrictions:
+            cls = "restricted-%s" % et.arg
+            elemtype = {
+                "native_type": """RestrictedClassType(base_type=%s, restriction_dict=%s)"""
+                % (class_map[et.arg]["native_type"], repr(restrictions)),
+                "restriction_dict": restrictions,
+                "parent_type": et.arg,
+                "base_type": False,
+            }
+
+    # Handle all other types of leaves that are not restricted classes.
+    if cls is None:
+        cls = "leaf"
+        # Enumerations are built as RestrictedClasses where the value that is
+        # provided to the class is check against the keys of a dictionary.
+        if et.arg == "enumeration":
+            enumeration_dict = {}
+            for enum in et.search("enum"):
+                enumeration_dict[six.text_type(enum.arg)] = {}
+                val = enum.search_one("value")
+                if val is not None:
+                    enumeration_dict[six.text_type(enum.arg)]["value"] = int(val.arg)
+            elemtype = {
+                "native_type": """RestrictedClassType(base_type=six.text_type, \
                                     restriction_type="dict_key", \
-                                    restriction_arg=%s,)""" %
-                                    (enumeration_dict),
-                  "restriction_argument": enumeration_dict,
-                  "restriction_type": "dict_key",
-                  "parent_type": "string",
-                  "base_type": False}
-    # Map decimal64 to a RestrictedPrecisionDecimalType - this is there to
-    # ensure that the fraction-digits argument can be implemented. Note that
-    # fraction-digits is a mandatory argument.
-    elif et.arg == "decimal64":
-      fd_stmt = et.search_one('fraction-digits')
-      if fd_stmt is not None:
-        cls = "restricted-decimal64"
-        elemtype = {"native_type":
-                      """RestrictedPrecisionDecimalType(precision=%s)""" %
-                      fd_stmt.arg, "base_type": False,
-                      "parent_type": "decimal64"}
-      else:
-        elemtype = class_map[et.arg]
-    # Handle unions - build a list of the supported types that are under the
-    # union.
-    elif et.arg == "union":
-      elemtype = []
-      for uniontype in et.search('type'):
-        elemtype_s = copy.deepcopy(build_elemtype(ctx, uniontype))
-        elemtype_s[1]["yang_type"] = uniontype.arg
-        elemtype.append(elemtype_s)
-      cls = "union"
-    # Map leafrefs to a ReferenceType, handling the referenced path, and
-    # whether require-instance is set. When xpathhelper is not specified, then
-    # no such mapping is done - at this point, we solely map to a string.
-    elif et.arg == "leafref":
-      path_stmt = et.search_one('path')
-      if path_stmt is None:
-        raise ValueError("leafref specified with no path statement")
-      require_instance = \
-                  class_bool_map[et.search_one('require-instance').arg] \
-                          if et.search_one('require-instance') \
-                            is not None else True
-      if ctx.opts.use_xpathhelper:
-        elemtype = {"native_type": "ReferenceType",
+                                    restriction_arg=%s,)"""
+                % (enumeration_dict),
+                "restriction_argument": enumeration_dict,
+                "restriction_type": "dict_key",
+                "parent_type": "string",
+                "base_type": False,
+            }
+        # Map decimal64 to a RestrictedPrecisionDecimalType - this is there to
+        # ensure that the fraction-digits argument can be implemented. Note that
+        # fraction-digits is a mandatory argument.
+        elif et.arg == "decimal64":
+            fd_stmt = et.search_one("fraction-digits")
+            if fd_stmt is not None:
+                cls = "restricted-decimal64"
+                elemtype = {
+                    "native_type": """RestrictedPrecisionDecimalType(precision=%s)""" % fd_stmt.arg,
+                    "base_type": False,
+                    "parent_type": "decimal64",
+                }
+            else:
+                elemtype = class_map[et.arg]
+        # Handle unions - build a list of the supported types that are under the
+        # union.
+        elif et.arg == "union":
+            elemtype = []
+            for uniontype in et.search("type"):
+                elemtype_s = copy.deepcopy(build_elemtype(ctx, uniontype))
+                elemtype_s[1]["yang_type"] = uniontype.arg
+                elemtype.append(elemtype_s)
+            cls = "union"
+        # Map leafrefs to a ReferenceType, handling the referenced path, and
+        # whether require-instance is set. When xpathhelper is not specified, then
+        # no such mapping is done - at this point, we solely map to a string.
+        elif et.arg == "leafref":
+            path_stmt = et.search_one("path")
+            if path_stmt is None:
+                raise ValueError("leafref specified with no path statement")
+            require_instance = (
+                class_bool_map[et.search_one("require-instance").arg]
+                if et.search_one("require-instance") is not None
+                else True
+            )
+            if ctx.opts.use_xpathhelper:
+                elemtype = {
+                    "native_type": "ReferenceType",
                     "referenced_path": path_stmt.arg,
                     "parent_type": "string",
                     "base_type": False,
-                    "require_instance": require_instance, }
-        cls = "leafref"
-      else:
-        elemtype = {
-            "native_type": "six.text_type",
-            "parent_type": "string",
-            "base_type": False,
-        }
-    # Handle identityrefs, but check whether there is a valid base where this
-    # has been specified.
-    elif et.arg == "identityref":
-      base_stmt = et.search_one('base')
-      if base_stmt is None:
-        raise ValueError("identityref specified with no base statement")
-      try:
-        elemtype = class_map[base_stmt.arg]
-      except KeyError:
-        sys.stderr.write("FATAL: identityref with an unknown base\n")
-        if DEBUG:
-          pp.pprint(class_map.keys())
-          pp.pprint(et.arg)
-          pp.pprint(base_stmt.arg)
-        sys.exit(127)
-    else:
-      # For all other cases, then we should be able to look up directly in the
-      # class_map for the defined type, since these are not 'derived' types
-      # at this point. In the case that we are referencing a type that is a
-      # typedef, then this has been added to the class_map.
-      try:
-        elemtype = class_map[et.arg]
-      except KeyError:
-        passed = False
-        if prefix:
-          try:
-            tmp_name = "%s:%s" % (prefix, et.arg)
-            elemtype = class_map[tmp_name]
-            passed = True
-          except Exception:
-            pass
-        if passed is False:
-          sys.stderr.write("FATAL: unmapped type (%s)\n" % (et.arg))
-          if DEBUG:
-            pp.pprint(class_map.keys())
-            pp.pprint(et.arg)
-            pp.pprint(prefix)
-          sys.exit(127)
-    if isinstance(elemtype, list):
-      cls = "leaf-union"
-    elif "class_override" in elemtype:
-      # this is used to propagate the fact that in some cases the
-      # native type needs to be dynamically built (e.g., leafref)
-      cls = elemtype["class_override"]
+                    "require_instance": require_instance,
+                }
+                cls = "leafref"
+            else:
+                elemtype = {"native_type": "six.text_type", "parent_type": "string", "base_type": False}
+        # Handle identityrefs, but check whether there is a valid base where this
+        # has been specified.
+        elif et.arg == "identityref":
+            base_stmt = et.search_one("base")
+            if base_stmt is None:
+                raise ValueError("identityref specified with no base statement")
+            try:
+                elemtype = class_map[base_stmt.arg]
+            except KeyError:
+                sys.stderr.write("FATAL: identityref with an unknown base\n")
+                if DEBUG:
+                    pp.pprint(class_map.keys())
+                    pp.pprint(et.arg)
+                    pp.pprint(base_stmt.arg)
+                sys.exit(127)
+        else:
+            # For all other cases, then we should be able to look up directly in the
+            # class_map for the defined type, since these are not 'derived' types
+            # at this point. In the case that we are referencing a type that is a
+            # typedef, then this has been added to the class_map.
+            try:
+                elemtype = class_map[et.arg]
+            except KeyError:
+                passed = False
+                if prefix:
+                    try:
+                        tmp_name = "%s:%s" % (prefix, et.arg)
+                        elemtype = class_map[tmp_name]
+                        passed = True
+                    except Exception:
+                        pass
+                if passed is False:
+                    sys.stderr.write("FATAL: unmapped type (%s)\n" % (et.arg))
+                    if DEBUG:
+                        pp.pprint(class_map.keys())
+                        pp.pprint(et.arg)
+                        pp.pprint(prefix)
+                    sys.exit(127)
+        if isinstance(elemtype, list):
+            cls = "leaf-union"
+        elif "class_override" in elemtype:
+            # this is used to propagate the fact that in some cases the
+            # native type needs to be dynamically built (e.g., leafref)
+            cls = elemtype["class_override"]
 
-  return (cls, elemtype)
+    return (cls, elemtype)
 
 
 def find_absolute_default_type(default_type, default_value, elemname):
-  if not isinstance(default_type, list):
-    return default_type
+    if not isinstance(default_type, list):
+        return default_type
 
-  for i in default_type:
-    if not i[1]["base_type"]:
-      test_type = class_map[i[1]["parent_type"]]
-    else:
-      test_type = i[1]
-    try:
-      test_type["pytype"](default_value)
-      default_type = test_type
-      break
-    except (ValueError, TypeError):
-      pass
-  return find_absolute_default_type(default_type, default_value, elemname)
-
-
-def get_element(ctx, fd, element, module, parent, path,
-                  parent_cfg=True, choice=False, register_paths=True):
-  # Handle mapping of an invidual element within the model. This function
-  # produces a dictionary that can then be mapped into the relevant code that
-  # dynamically generates a class.
-
-  # Find element's namespace and defining module
-  # If the element has the "main_module" attribute then it is part of a
-  # submodule and hence we should check the namespace and defining module
-  # of this, rather than the submodule
-  if hasattr(element, "main_module"):
-    element_module = element.main_module()
-  elif hasattr(element, "i_orig_module"):
-    element_module = element.i_orig_module
-  else:
-    element_module = None
-
-  namespace = element_module.search_one("namespace").arg if \
-                element_module.search_one("namespace") is not None else \
-                  None
-  defining_module = element_module.arg
-
-  this_object = []
-  has_children = False
-  create_list = False
-
-  elemdescr = element.search_one('description')
-  if elemdescr is None:
-    elemdescr = False
-  else:
-    elemdescr = elemdescr.arg
-
-    # In cases where there there are a set of interesting extensions specified
-    # then build a dictionary of these extension values to provide with the
-    # specific leaf for this element.
-  if element.substmts is not None and \
-        ctx.opts.pybind_interested_exts is not None:
-    extensions = {}
-    for ext in element.substmts:
-      if ext.keyword[0] in ctx.opts.pybind_interested_exts:
-        if not ext.keyword[0] in extensions:
-          extensions[ext.keyword[0]] = {}
-        extensions[ext.keyword[0]][ext.keyword[1]] = ext.arg
-
-  # If the element has an i_children attribute then this is a container, list
-  # leaf-list or choice. Alternatively, it can be the 'input' or 'output'
-  # substmts of an RPC or a notification
-  if hasattr(element, 'i_children'):
-    if element.keyword in ["container", "list", "input", "output", "notification"]:
-      has_children = True
-    elif element.keyword in ["leaf-list"]:
-      create_list = True
-
-    # Fixup the path when within a choice, because this iteration belives that
-    # we are under a new container, but this does not exist in the path.
-    if element.keyword in ["choice"]:
-      path_parts = path.split("/")
-      npath = ""
-      for i in range(0, len(path_parts) - 1):
-        npath += "%s/" % path_parts[i]
-      npath.rstrip("/")
+    for i in default_type:
+        if not i[1]["base_type"]:
+            test_type = class_map[i[1]["parent_type"]]
+        else:
+            test_type = i[1]
+        try:
+            test_type["pytype"](default_value)
+            default_type = test_type
+            break
+        except (ValueError, TypeError):
+            pass
+    return find_absolute_default_type(default_type, default_value, elemname)
+
+
+def get_element(ctx, fd, element, module, parent, path, parent_cfg=True, choice=False, register_paths=True):
+    # Handle mapping of an invidual element within the model. This function
+    # produces a dictionary that can then be mapped into the relevant code that
+    # dynamically generates a class.
+
+    # Find element's namespace and defining module
+    # If the element has the "main_module" attribute then it is part of a
+    # submodule and hence we should check the namespace and defining module
+    # of this, rather than the submodule
+    if hasattr(element, "main_module"):
+        element_module = element.main_module()
+    elif hasattr(element, "i_orig_module"):
+        element_module = element.i_orig_module
     else:
-      npath = path
+        element_module = None
 
-    # Create an element for a container.
-    if element.i_children or ctx.opts.generate_presence:
-      chs = element.i_children
-      has_presence = True if element.search_one('presence') is not None else False
-      if has_presence is False and len(chs) == 0:
-        return []
-
-      get_children(ctx, fd, chs, module, element, npath, parent_cfg=parent_cfg,
-                   choice=choice, register_paths=register_paths)
-
-      elemdict = {
-          "name": safe_name(element.arg), "origtype": element.keyword,
-          "class": element.keyword,
-          "path": safe_name(npath), "config": True,
-          "description": elemdescr,
-          "yang_name": element.arg,
-          "choice": choice,
-          "register_paths": register_paths,
-          "namespace": namespace,
-          "defining_module": defining_module,
-          "extensions": extensions if len(extensions) else None,
-          "presence": has_presence,
-      }
-
-      # Handle the different cases of class name, this depends on whether we
-      # were asked to split the bindings into a directory structure or not.
-      if ctx.opts.split_class_dir:
-        # If we were dealing with split classes, then rather than naming the
-        # class based on a unique intra-file name - and rather we must import
-        # the relative path to the module.class
-        if element.arg == parent.arg:
-          modname = safe_name(element.arg) + "_"
-        else:
-          modname = safe_name(element.arg)
-        elemdict["type"] = "%s.%s" % (modname, safe_name(element.arg))
+    namespace = (
+        element_module.search_one("namespace").arg if element_module.search_one("namespace") is not None else None
+    )
+    defining_module = element_module.arg
+
+    this_object = []
+    has_children = False
+    create_list = False
+
+    elemdescr = element.search_one("description")
+    if elemdescr is None:
+        elemdescr = False
+    else:
+        elemdescr = elemdescr.arg
 
-      else:
-        # Otherwise, give a unique name for the class within the dictionary.
-        elemdict["type"] = "yc_%s_%s_%s" % (safe_name(element.arg),
-                                            safe_name(module.arg),
-                                            safe_name(path.replace("/", "_")))
-
-      # Deal with specific cases for list - such as the key and how it is
-      # ordered.
-      if element.keyword == "list":
-        elemdict["key"] = safe_name(element.search_one("key").arg) \
-            if element.search_one("key") is not None else False
-        elemdict["yang_keys"] = element.search_one("key").arg \
-            if element.search_one("key") is not None else False
-        user_ordered = element.search_one('ordered-by')
-        elemdict["user_ordered"] = True if user_ordered is not None \
-          and user_ordered.arg.upper() == "USER" else False
-      this_object.append(elemdict)
-      has_children = True
-
-  # Deal with the cases that the attribute does not have children.
-  if not has_children:
-    if element.keyword in ["leaf-list"]:
-      create_list = True
-    cls, elemtype = copy.deepcopy(build_elemtype(ctx,
-                        element.search_one('type')))
-
-    # Determine what the default for the leaf should be where there are
-    # multiple available.
-    # Algorithm:
-    #   - build a tree that is rooted on this class.
-    #   - perform a breadth-first search - the first node found
-    #   - that has the "default" leaf set, then we take this
-    #     as the value for the default
-
-    # then starting at the selected default node, traverse
-    # until we find a node that is declared to be a base_type
-    elemdefault = element.search_one('default')
-    default_type = False
-    quote_arg = False
-    if elemdefault is not None:
-      elemdefault = elemdefault.arg
-      default_type = elemtype
-    if isinstance(elemtype, list):
-      # this is a union, we should check whether any of the types
-      # immediately has a default
-      for i in elemtype:
-        if "default" in i[1]:
-          elemdefault = i[1]["default"]
-          default_type = i[1]
-          # default_type = i[1]
-          # mapped_elemtype = i[1]
-    elif "default" in elemtype:
-      # if the actual type defines the default, then we need to maintain
-      # this
-      elemdefault = elemtype["default"]
-      default_type = elemtype
-
-    # we need to indicate that the default type for the class_map
-    # is str
-    tmp_class_map = copy.deepcopy(class_map)
-    tmp_class_map["enumeration"] = {"parent_type": "string"}
-
-    if not default_type:
-      if isinstance(elemtype, list):
-        # this type has multiple parents
-        for i in elemtype:
-          if "parent_type" in i[1]:
-            if isinstance(i[1]["parent_type"], list):
-              to_visit = [j for j in i[1]["parent_type"]]
-            else:
-              to_visit = [i[1]["parent_type"]]
-      elif "parent_type" in elemtype:
-        if isinstance(elemtype["parent_type"], list):
-          to_visit = [i for i in elemtype["parent_type"]]
+        # In cases where there there are a set of interesting extensions specified
+        # then build a dictionary of these extension values to provide with the
+        # specific leaf for this element.
+    if element.substmts is not None and ctx.opts.pybind_interested_exts is not None:
+        extensions = {}
+        for ext in element.substmts:
+            if ext.keyword[0] in ctx.opts.pybind_interested_exts:
+                if not ext.keyword[0] in extensions:
+                    extensions[ext.keyword[0]] = {}
+                extensions[ext.keyword[0]][ext.keyword[1]] = ext.arg
+
+    # If the element has an i_children attribute then this is a container, list
+    # leaf-list or choice. Alternatively, it can be the 'input' or 'output'
+    # substmts of an RPC or a notification
+    if hasattr(element, "i_children"):
+        if element.keyword in ["container", "list", "input", "output", "notification"]:
+            has_children = True
+        elif element.keyword in ["leaf-list"]:
+            create_list = True
+
+        # Fixup the path when within a choice, because this iteration belives that
+        # we are under a new container, but this does not exist in the path.
+        if element.keyword in ["choice"]:
+            path_parts = path.split("/")
+            npath = ""
+            for i in range(0, len(path_parts) - 1):
+                npath += "%s/" % path_parts[i]
+            npath.rstrip("/")
         else:
-          to_visit = [elemtype["parent_type"]]
+            npath = path
 
-        checked = list()
-        while to_visit:
-          check = to_visit.pop(0)
-          if check not in checked:
-            checked.append(check)
-            if "parent_type" in tmp_class_map[check]:
-              if isinstance(tmp_class_map[check]["parent_type"], list):
-                to_visit.extend(tmp_class_map[check]["parent_type"])
-              else:
-                to_visit.append(tmp_class_map[check]["parent_type"])
-
-        # checked now has the breadth-first search result
-        if elemdefault is None:
-          for option in checked:
-            if "default" in tmp_class_map[option]:
-              elemdefault = tmp_class_map[option]["default"]
-              default_type = tmp_class_map[option]
-              break
-
-    if elemdefault is not None:
-      # we now need to check whether there's a need to
-      # find out what the base type is for this type
-      # we really expect a linear chain here.
-
-      # if we have a tuple as the type here, this means that
-      # the default was set at a level where there was not
-      # a single option for the type. check the default
-      # against each option, to get a to a single default_type
-      if isinstance(default_type, list):
-        default_type = find_absolute_default_type(default_type, elemdefault,
-                          element.arg)
-
-      if not default_type["base_type"]:
-        if "parent_type" in default_type:
-          if isinstance(default_type["parent_type"], list):
-            to_visit = [i for i in default_type["parent_type"]]
-          else:
-            to_visit = [default_type["parent_type"]]
-        checked = list()
-        while to_visit:
-          check = to_visit.pop(0)  # remove from the top of stack - depth first
-          if check not in checked:
-            checked.append(check)
-            if "parent_type" in tmp_class_map[check]:
-              if isinstance(tmp_class_map[check]["parent_type"], list):
-                to_visit.extend(tmp_class_map[check]["parent_type"])
-              else:
-                to_visit.append(tmp_class_map[check]["parent_type"])
-        default_type = tmp_class_map[checked.pop()]
-        if not default_type["base_type"]:
-          raise TypeError("default type was not a base type")
-
-    # Set the default type based on what was determined above about the
-    # correct value to set.
-    if default_type:
-      quote_arg = default_type["quote_arg"] if "quote_arg" in \
-          default_type else False
-      default_type = default_type["native_type"]
-
-    elemconfig = class_bool_map[element.search_one('config').arg] if \
-                                  element.search_one('config') else True
-
-    elemname = safe_name(element.arg)
-
-    # Deal with the cases that there is a requirement to create a list - these
-    # are leaf lists. There is some special handling for leaf-lists to ensure
-    # that the references are correctly created.
-    if create_list:
-      if not cls == "leafref":
-        cls = "leaf-list"
+        # Create an element for a container.
+        if element.i_children or ctx.opts.generate_presence:
+            chs = element.i_children
+            has_presence = True if element.search_one("presence") is not None else False
+            if has_presence is False and len(chs) == 0:
+                return []
+
+            get_children(
+                ctx,
+                fd,
+                chs,
+                module,
+                element,
+                npath,
+                parent_cfg=parent_cfg,
+                choice=choice,
+                register_paths=register_paths,
+            )
+
+            elemdict = {
+                "name": safe_name(element.arg),
+                "origtype": element.keyword,
+                "class": element.keyword,
+                "path": safe_name(npath),
+                "config": True,
+                "description": elemdescr,
+                "yang_name": element.arg,
+                "choice": choice,
+                "register_paths": register_paths,
+                "namespace": namespace,
+                "defining_module": defining_module,
+                "extensions": extensions if len(extensions) else None,
+                "presence": has_presence,
+            }
+
+            # Handle the different cases of class name, this depends on whether we
+            # were asked to split the bindings into a directory structure or not.
+            if ctx.opts.split_class_dir:
+                # If we were dealing with split classes, then rather than naming the
+                # class based on a unique intra-file name - and rather we must import
+                # the relative path to the module.class
+                if element.arg == parent.arg:
+                    modname = safe_name(element.arg) + "_"
+                else:
+                    modname = safe_name(element.arg)
+                elemdict["type"] = "%s.%s" % (modname, safe_name(element.arg))
 
+            else:
+                # Otherwise, give a unique name for the class within the dictionary.
+                elemdict["type"] = "yc_%s_%s_%s" % (
+                    safe_name(element.arg),
+                    safe_name(module.arg),
+                    safe_name(path.replace("/", "_")),
+                )
+
+            # Deal with specific cases for list - such as the key and how it is
+            # ordered.
+            if element.keyword == "list":
+                elemdict["key"] = (
+                    safe_name(element.search_one("key").arg) if element.search_one("key") is not None else False
+                )
+                elemdict["yang_keys"] = (
+                    element.search_one("key").arg if element.search_one("key") is not None else False
+                )
+                user_ordered = element.search_one("ordered-by")
+                elemdict["user_ordered"] = (
+                    True if user_ordered is not None and user_ordered.arg.upper() == "USER" else False
+                )
+            this_object.append(elemdict)
+            has_children = True
+
+    # Deal with the cases that the attribute does not have children.
+    if not has_children:
+        if element.keyword in ["leaf-list"]:
+            create_list = True
+        cls, elemtype = copy.deepcopy(build_elemtype(ctx, element.search_one("type")))
+
+        # Determine what the default for the leaf should be where there are
+        # multiple available.
+        # Algorithm:
+        #   - build a tree that is rooted on this class.
+        #   - perform a breadth-first search - the first node found
+        #   - that has the "default" leaf set, then we take this
+        #     as the value for the default
+
+        # then starting at the selected default node, traverse
+        # until we find a node that is declared to be a base_type
+        elemdefault = element.search_one("default")
+        default_type = False
+        quote_arg = False
+        if elemdefault is not None:
+            elemdefault = elemdefault.arg
+            default_type = elemtype
         if isinstance(elemtype, list):
-          allowed_types = []
-          for subtype in elemtype:
-            # nested union within a leaf-list type
-            if isinstance(subtype, tuple):
-              if subtype[0] == "leaf-union":
-                for subelemtype in subtype[1]["native_type"]:
-                  allowed_types.append(subelemtype)
-              else:
-                if isinstance(subtype[1]["native_type"], list):
-                  allowed_types.extend(subtype[1]["native_type"])
+            # this is a union, we should check whether any of the types
+            # immediately has a default
+            for i in elemtype:
+                if "default" in i[1]:
+                    elemdefault = i[1]["default"]
+                    default_type = i[1]
+                    # default_type = i[1]
+                    # mapped_elemtype = i[1]
+        elif "default" in elemtype:
+            # if the actual type defines the default, then we need to maintain
+            # this
+            elemdefault = elemtype["default"]
+            default_type = elemtype
+
+        # we need to indicate that the default type for the class_map
+        # is str
+        tmp_class_map = copy.deepcopy(class_map)
+        tmp_class_map["enumeration"] = {"parent_type": "string"}
+
+        if not default_type:
+            if isinstance(elemtype, list):
+                # this type has multiple parents
+                for i in elemtype:
+                    if "parent_type" in i[1]:
+                        if isinstance(i[1]["parent_type"], list):
+                            to_visit = [j for j in i[1]["parent_type"]]
+                        else:
+                            to_visit = [i[1]["parent_type"]]
+            elif "parent_type" in elemtype:
+                if isinstance(elemtype["parent_type"], list):
+                    to_visit = [i for i in elemtype["parent_type"]]
+                else:
+                    to_visit = [elemtype["parent_type"]]
+
+                checked = list()
+                while to_visit:
+                    check = to_visit.pop(0)
+                    if check not in checked:
+                        checked.append(check)
+                        if "parent_type" in tmp_class_map[check]:
+                            if isinstance(tmp_class_map[check]["parent_type"], list):
+                                to_visit.extend(tmp_class_map[check]["parent_type"])
+                            else:
+                                to_visit.append(tmp_class_map[check]["parent_type"])
+
+                # checked now has the breadth-first search result
+                if elemdefault is None:
+                    for option in checked:
+                        if "default" in tmp_class_map[option]:
+                            elemdefault = tmp_class_map[option]["default"]
+                            default_type = tmp_class_map[option]
+                            break
+
+        if elemdefault is not None:
+            # we now need to check whether there's a need to
+            # find out what the base type is for this type
+            # we really expect a linear chain here.
+
+            # if we have a tuple as the type here, this means that
+            # the default was set at a level where there was not
+            # a single option for the type. check the default
+            # against each option, to get a to a single default_type
+            if isinstance(default_type, list):
+                default_type = find_absolute_default_type(default_type, elemdefault, element.arg)
+
+            if not default_type["base_type"]:
+                if "parent_type" in default_type:
+                    if isinstance(default_type["parent_type"], list):
+                        to_visit = [i for i in default_type["parent_type"]]
+                    else:
+                        to_visit = [default_type["parent_type"]]
+                checked = list()
+                while to_visit:
+                    check = to_visit.pop(0)  # remove from the top of stack - depth first
+                    if check not in checked:
+                        checked.append(check)
+                        if "parent_type" in tmp_class_map[check]:
+                            if isinstance(tmp_class_map[check]["parent_type"], list):
+                                to_visit.extend(tmp_class_map[check]["parent_type"])
+                            else:
+                                to_visit.append(tmp_class_map[check]["parent_type"])
+                default_type = tmp_class_map[checked.pop()]
+                if not default_type["base_type"]:
+                    raise TypeError("default type was not a base type")
+
+        # Set the default type based on what was determined above about the
+        # correct value to set.
+        if default_type:
+            quote_arg = default_type["quote_arg"] if "quote_arg" in default_type else False
+            default_type = default_type["native_type"]
+
+        elemconfig = class_bool_map[element.search_one("config").arg] if element.search_one("config") else True
+
+        elemname = safe_name(element.arg)
+
+        # Deal with the cases that there is a requirement to create a list - these
+        # are leaf lists. There is some special handling for leaf-lists to ensure
+        # that the references are correctly created.
+        if create_list:
+            if not cls == "leafref":
+                cls = "leaf-list"
+
+                if isinstance(elemtype, list):
+                    allowed_types = []
+                    for subtype in elemtype:
+                        # nested union within a leaf-list type
+                        if isinstance(subtype, tuple):
+                            if subtype[0] == "leaf-union":
+                                for subelemtype in subtype[1]["native_type"]:
+                                    allowed_types.append(subelemtype)
+                            else:
+                                if isinstance(subtype[1]["native_type"], list):
+                                    allowed_types.extend(subtype[1]["native_type"])
+                                else:
+                                    allowed_types.append(subtype[1]["native_type"])
+                        else:
+                            allowed_types.append(subtype["native_type"])
                 else:
-                  allowed_types.append(subtype[1]["native_type"])
+                    allowed_types = elemtype["native_type"]
             else:
-              allowed_types.append(subtype["native_type"])
+                cls = "leafref-list"
+                allowed_types = {
+                    "native_type": elemtype["native_type"],
+                    "referenced_path": elemtype["referenced_path"],
+                    "require_instance": elemtype["require_instance"],
+                }
+            elemntype = {"class": cls, "native_type": ("TypedListType", allowed_types)}
+
         else:
-          allowed_types = elemtype["native_type"]
-      else:
-        cls = "leafref-list"
-        allowed_types = {
-            "native_type": elemtype["native_type"],
-            "referenced_path": elemtype["referenced_path"],
-            "require_instance": elemtype["require_instance"],
+            if cls == "union" or cls == "leaf-union":
+                elemtype = {"class": cls, "native_type": ("UnionType", elemtype)}
+            elemntype = elemtype["native_type"]
+
+        # Build the dictionary for the element with the relevant meta-data
+        # specified within it.
+        elemdict = {
+            "name": elemname,
+            "type": elemntype,
+            "origtype": element.search_one("type").arg,
+            "path": safe_name(path),
+            "class": cls,
+            "default": elemdefault,
+            "config": elemconfig,
+            "defaulttype": default_type,
+            "quote_arg": quote_arg,
+            "description": elemdescr,
+            "yang_name": element.arg,
+            "choice": choice,
+            "register_paths": register_paths,
+            "namespace": namespace,
+            "defining_module": defining_module,
         }
-      elemntype = {"class": cls, "native_type": ("TypedListType",
-                  allowed_types)}
+        if len(extensions):
+            elemdict["extensions"] = extensions
 
-    else:
-      if cls == "union" or cls == "leaf-union":
-        elemtype = {"class": cls, "native_type": ("UnionType", elemtype)}
-      elemntype = elemtype["native_type"]
-
-    # Build the dictionary for the element with the relevant meta-data
-    # specified within it.
-    elemdict = {
-        "name": elemname, "type": elemntype,
-        "origtype": element.search_one('type').arg, "path":
-        safe_name(path),
-        "class": cls, "default": elemdefault,
-        "config": elemconfig, "defaulttype": default_type,
-        "quote_arg": quote_arg,
-        "description": elemdescr, "yang_name": element.arg,
-        "choice": choice,
-        "register_paths": register_paths,
-        "namespace": namespace,
-        "defining_module": defining_module
-    }
-    if len(extensions):
-      elemdict["extensions"] = extensions
-
-    if cls == "leafref":
-      elemdict["referenced_path"] = elemtype["referenced_path"]
-      elemdict["require_instance"] = elemtype["require_instance"]
+        if cls == "leafref":
+            elemdict["referenced_path"] = elemtype["referenced_path"]
+            elemdict["require_instance"] = elemtype["require_instance"]
 
-    this_object.append(elemdict)
-  return this_object
+        this_object.append(elemdict)
+    return this_object
```

### Comparing `pyangbind-0.8.1/pyangbind.egg-info/PKG-INFO` & `pyangbind-0.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,63 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyangbind
-Version: 0.8.1
-Summary: PyangBind is a plugin for pyang which converts YANG datamodels into a Python class hierarchy, such that Python can be used to manipulate data that conforms with a YANG model.
+Version: 0.8.2
+Summary: PyangBind is a plugin for pyang which converts YANG data models into a Python class hierarchy, such that Python can be used to manipulate data that conforms with a YANG model.
 Home-page: https://github.com/robshakir/pyangbind
 Author: Rob Shakir
 Author-email: rjs@rob.sh
-License: Apache
-Description: PyangBind
-        =========
-        
-        PyangBind is a plugin for pyang which converts YANG data models into a Python class hierarchy, such that Python can be used to manipulate data that conforms with a YANG model.
-        
-        This module provides the supporting classes and functions that PyangBind modules utilise, particularly:
-        
-        * pyangbind.base.PybindBase - which is the parent class inherited by all container or module YANG objects.
-        
-        * pyangbind.pybindJSON - which containers wrapper functions which can be used to help with serialisation of YANG to JSON.
-        
-        * pyangbind.serialise.pybindJSONEncoder - a class that can be used as a custom encoder for the JSON module to serialise PyangBind class hierarchies to JSON.
-        
-        * pyangbind.serialise.pybindJSONDecoder - a class that can be used as a custom decoder to load JSON-encoded instances of YANG models into a PyangBind class hierarchy.
-        
-        * pyangbind.xpathhelper.YANGPathHelper - a class which can have objects registered against it, and subsequently retrieved from it using XPATH expressions. This module also includes parent classes that can be used to implement other helper modules of this nature.
-        
-        * pyangbind.yangtypes: The various functions which generate python types that are used to represent YANG types, and some helper methods.
-        
-          - pyangbind.yangtypes.is_yang_list and is_yang_leaflist are self explainatory, but may be useful.
-        
-          - pyangbind.yangtypes.safe_name is used throughout PyangBind to determine how to map YANG element names into Python attribute names safely.
-        
-          - pyangbind.yangtypes.RestrictedPrecisionDecimalType - generates wrapped Decimal types that has a restricted set of decimal digits - i.e., can deal with fraction-digits arguments in YANG.
-        
-          - pyangbind.yangtypes.RestrictedClassType - generates types which wrap a 'base' type (e.g., integer) with particular restrictions. The restrictions are supplied as a dictionary, or with specific arguments if single restrictions are required. Currently, the restrictions supported are regexp matches, ranges, lengths, and restrictions to a set of values (provided as keys to a dict).
-        
-          - pyangbind.yangtypes.TypedListType - generates types which wrap a list to restrict the objects that it may contain.
-        
-          - pyangbind.yangtypes.YANGListType - generates types which wrap a class representing a container, such that it acts as a YANG list.
-        
-          - pyangbind.yangtypes.YANGBool - a boolean class.
-        
-          - pyangbind.yangtypes.YANGDynClass - generates types which consist of a wrapper (YANGDynClass) and a wrapped object which may be any other class. YANGDynClass is a meta-class that provides additional data on top of the attributes and functions of the wrapped class.
-        
-          - pyangbind.yangtypes.ReferenceType - generates types which can use a pyangbind.xpathhelper.PybindXpathHelper instance to look up values - particularly to support leafrefs in YANG.
-        
-        Usage documentation for PyangBind itself can be found on GitHub: https://github.com/robshakir/pyangbind
-Keywords: yang pyang
-Platform: UNKNOWN
+License: Apache License, Version 2.0
+Keywords: yang,pyang
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+PyangBind
+=========
+
+PyangBind is a plugin for pyang which converts YANG data models into a Python class hierarchy, such that Python can be used to manipulate data that conforms with a YANG model.
+
+This module provides the supporting classes and functions that PyangBind modules utilise, particularly:
+
+* pyangbind.base.PybindBase - which is the parent class inherited by all container or module YANG objects.
+
+* pyangbind.pybindJSON - which containers wrapper functions which can be used to help with serialisation of YANG to JSON.
+
+* pyangbind.serialise.pybindJSONEncoder - a class that can be used as a custom encoder for the JSON module to serialise PyangBind class hierarchies to JSON.
+
+* pyangbind.serialise.pybindJSONDecoder - a class that can be used as a custom decoder to load JSON-encoded instances of YANG models into a PyangBind class hierarchy.
+
+* pyangbind.xpathhelper.YANGPathHelper - a class which can have objects registered against it, and subsequently retrieved from it using XPATH expressions. This module also includes parent classes that can be used to implement other helper modules of this nature.
+
+* pyangbind.yangtypes: The various functions which generate python types that are used to represent YANG types, and some helper methods.
+
+  - pyangbind.yangtypes.is_yang_list and is_yang_leaflist are self explainatory, but may be useful.
+
+  - pyangbind.yangtypes.safe_name is used throughout PyangBind to determine how to map YANG element names into Python attribute names safely.
+
+  - pyangbind.yangtypes.RestrictedPrecisionDecimalType - generates wrapped Decimal types that has a restricted set of decimal digits - i.e., can deal with fraction-digits arguments in YANG.
+
+  - pyangbind.yangtypes.RestrictedClassType - generates types which wrap a 'base' type (e.g., integer) with particular restrictions. The restrictions are supplied as a dictionary, or with specific arguments if single restrictions are required. Currently, the restrictions supported are regexp matches, ranges, lengths, and restrictions to a set of values (provided as keys to a dict).
+
+  - pyangbind.yangtypes.TypedListType - generates types which wrap a list to restrict the objects that it may contain.
+
+  - pyangbind.yangtypes.YANGListType - generates types which wrap a class representing a container, such that it acts as a YANG list.
+
+  - pyangbind.yangtypes.YANGBool - a boolean class.
+
+  - pyangbind.yangtypes.YANGDynClass - generates types which consist of a wrapper (YANGDynClass) and a wrapped object which may be any other class. YANGDynClass is a meta-class that provides additional data on top of the attributes and functions of the wrapped class.
+
+  - pyangbind.yangtypes.ReferenceType - generates types which can use a pyangbind.xpathhelper.PybindXpathHelper instance to look up values - particularly to support leafrefs in YANG.
+
+Usage documentation for PyangBind itself can be found on GitHub: https://github.com/robshakir/pyangbind
```

### Comparing `pyangbind-0.8.1/pyangbind.egg-info/SOURCES.txt` & `pyangbind-0.8.2/pyangbind.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 README.rst
+pyproject.toml
 requirements.DEVELOPER.txt
 requirements.txt
 setup.cfg
-setup.py
 pyangbind/__init__.py
 pyangbind.egg-info/PKG-INFO
 pyangbind.egg-info/SOURCES.txt
 pyangbind.egg-info/dependency_links.txt
 pyangbind.egg-info/not-zip-safe
 pyangbind.egg-info/requires.txt
 pyangbind.egg-info/top_level.txt
```

### Comparing `pyangbind-0.8.1/LICENSE` & `pyangbind-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyangbind-0.8.1/README.md` & `pyangbind-0.8.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 [![#PyangBind][img-pyangbind]][pyangbind-docs]
 
-
-[![Travis][img-travis]][travis]
-[![Codecov][img-codecov]][codecov]
 [![PyPI][img-pypi]][pypi-project]
 [![PyPI - License][img-license]][license]
 [![PyPI - Python Version][img-pyversion]][pypi-project]
 
 
 **PyangBind** is a plugin for [Pyang][pyang] that generates a Python class hierarchy from a YANG data model. The resulting classes can be directly interacted with in Python. Particularly, **PyangBind** will allow you to:
 
@@ -161,23 +158,61 @@
   print("Cannot set tag: {}".format(m))
 ```
 
 ### Serialising a Data Instance <a name="serialising"></a>
 
 Clearly, populated PyangBind classes are not useful in and of themselves - the common use case is that they are sent to a external system (e.g., a router, or other NMS component). To achieve this the class hierarchy needs to be serialised into a format that can be sent to the remote entity. There are currently multiple ways to do this:
 
- * **XML** - the rules for this mapping are defined in [RFC 7950][rfc7950] - currently _NOT SUPPORTED_.
+ * **XML** - the rules for this mapping are defined in [RFC 7950][rfc7950] - supported.
  * **OpenConfig-suggested JSON** - the rules for this mapping are currently being written into a formal specification. This is the standard (`default`) format used by PyangBind. Some network equipment vendors utilise this serialisation format.
  * **IETF JSON** - the rules for this mapping are defined in [RFC 7951][rfc7951] - some network equipment vendors use this format.
 
 Any PyangBind class can be serialised into any of the supported formats. Using the static route example above, the entire `local-routing` module can be serialised into OC-JSON using the following code:
 
 ```python
+from pyangbind.lib.serialise import pybindIETFXMLEncoder
+# Dump the entire instance as RFC 7950 XML
+print(pybindIETFXMLEncoder.serialise(oclr))
+```
+
+This outputs the following XML fragment:
+
+```xml
+<openconfig-local-routing xmlns="http://openconfig.net/yang/local-routing">
+  <local-routes>
+    <static-routes>
+      <static>
+        <prefix>192.0.2.1/32</prefix>
+        <config>
+          <set-tag>42</set-tag>
+        </config>
+        <next-hops>
+          <next-hop>
+            <index>0</index>
+            <config>
+              <next-hop>192.168.0.1</next-hop>
+            </config>
+          </next-hop>
+          <next-hop>
+            <index>1</index>
+            <config>
+              <next-hop>10.0.0.1</next-hop>
+            </config>
+          </next-hop>
+        </next-hops>
+      </static>
+    </static-routes>
+  </local-routes>
+</openconfig-local-routing>
+```
+
+Or, similarly, using OpenConfig-suggested JSON:
+
+```python
 import pyangbind.lib.pybindJSON as pybindJSON
-# Dump the entire instance as JSON in PyangBind format
 print(pybindJSON.dumps(oclr))
 ```
 
 This outputs the following JSON structured text:
 
 ```json
 {
@@ -346,22 +381,22 @@
   * [GoDaddy][godaddy], particularly Joey Wilhelm's herculean efforts to refactor test code to use the `unittest` framework.
   * David Barroso, who initiated efforts to address Python 3 compatibility, and a number of other enhancements.
 * Design, debugging, example code, and ideas have been contributed by:
   * Members of the [OpenConfig][openconfig] working group.
   * The managability team at Juniper Networks.
 
 
-[img-pyangbind]: http://rob.sh/img/pyblogo_gh.png
+[img-pyangbind]: https://cdn.rob.sh/img/pyblogo_gh.png
 [img-travis]: https://img.shields.io/travis/robshakir/pyangbind.svg
 [img-codecov]: https://img.shields.io/codecov/c/github/robshakir/pyangbind.svg
 [img-pypi]: https://img.shields.io/pypi/v/pyangbind.svg
 [img-license]: https://img.shields.io/pypi/l/pyangbind.svg
 [img-pyversion]: https://img.shields.io/pypi/pyversions/pyangbind.svg
 
-[pyangbind-docs]: http://pynms.io/pyangbind/
+[pyangbind-docs]: https://github.com/robshakir/pyangbind/tree/master/docs
 [travis]: https://travis-ci.org/robshakir/pyangbind
 [codecov]: https://codecov.io/gh/robshakir/pyangbind
 [pypi-project]: https://pypi.org/project/pyangbind/
 [license]: http://www.apache.org/licenses/LICENSE-2.0
 [pyang]: https://github.com/mbj4668/pyang
 [openconfig]: http://www.openconfig.net
 [pypi]: https://pypi.org/
```

### Comparing `pyangbind-0.8.1/README.rst` & `pyangbind-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyangbind-0.8.1/PKG-INFO` & `pyangbind-0.8.2/pyangbind.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,63 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyangbind
-Version: 0.8.1
-Summary: PyangBind is a plugin for pyang which converts YANG datamodels into a Python class hierarchy, such that Python can be used to manipulate data that conforms with a YANG model.
+Version: 0.8.2
+Summary: PyangBind is a plugin for pyang which converts YANG data models into a Python class hierarchy, such that Python can be used to manipulate data that conforms with a YANG model.
 Home-page: https://github.com/robshakir/pyangbind
 Author: Rob Shakir
 Author-email: rjs@rob.sh
-License: Apache
-Description: PyangBind
-        =========
-        
-        PyangBind is a plugin for pyang which converts YANG data models into a Python class hierarchy, such that Python can be used to manipulate data that conforms with a YANG model.
-        
-        This module provides the supporting classes and functions that PyangBind modules utilise, particularly:
-        
-        * pyangbind.base.PybindBase - which is the parent class inherited by all container or module YANG objects.
-        
-        * pyangbind.pybindJSON - which containers wrapper functions which can be used to help with serialisation of YANG to JSON.
-        
-        * pyangbind.serialise.pybindJSONEncoder - a class that can be used as a custom encoder for the JSON module to serialise PyangBind class hierarchies to JSON.
-        
-        * pyangbind.serialise.pybindJSONDecoder - a class that can be used as a custom decoder to load JSON-encoded instances of YANG models into a PyangBind class hierarchy.
-        
-        * pyangbind.xpathhelper.YANGPathHelper - a class which can have objects registered against it, and subsequently retrieved from it using XPATH expressions. This module also includes parent classes that can be used to implement other helper modules of this nature.
-        
-        * pyangbind.yangtypes: The various functions which generate python types that are used to represent YANG types, and some helper methods.
-        
-          - pyangbind.yangtypes.is_yang_list and is_yang_leaflist are self explainatory, but may be useful.
-        
-          - pyangbind.yangtypes.safe_name is used throughout PyangBind to determine how to map YANG element names into Python attribute names safely.
-        
-          - pyangbind.yangtypes.RestrictedPrecisionDecimalType - generates wrapped Decimal types that has a restricted set of decimal digits - i.e., can deal with fraction-digits arguments in YANG.
-        
-          - pyangbind.yangtypes.RestrictedClassType - generates types which wrap a 'base' type (e.g., integer) with particular restrictions. The restrictions are supplied as a dictionary, or with specific arguments if single restrictions are required. Currently, the restrictions supported are regexp matches, ranges, lengths, and restrictions to a set of values (provided as keys to a dict).
-        
-          - pyangbind.yangtypes.TypedListType - generates types which wrap a list to restrict the objects that it may contain.
-        
-          - pyangbind.yangtypes.YANGListType - generates types which wrap a class representing a container, such that it acts as a YANG list.
-        
-          - pyangbind.yangtypes.YANGBool - a boolean class.
-        
-          - pyangbind.yangtypes.YANGDynClass - generates types which consist of a wrapper (YANGDynClass) and a wrapped object which may be any other class. YANGDynClass is a meta-class that provides additional data on top of the attributes and functions of the wrapped class.
-        
-          - pyangbind.yangtypes.ReferenceType - generates types which can use a pyangbind.xpathhelper.PybindXpathHelper instance to look up values - particularly to support leafrefs in YANG.
-        
-        Usage documentation for PyangBind itself can be found on GitHub: https://github.com/robshakir/pyangbind
-Keywords: yang pyang
-Platform: UNKNOWN
+License: Apache License, Version 2.0
+Keywords: yang,pyang
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+PyangBind
+=========
+
+PyangBind is a plugin for pyang which converts YANG data models into a Python class hierarchy, such that Python can be used to manipulate data that conforms with a YANG model.
+
+This module provides the supporting classes and functions that PyangBind modules utilise, particularly:
+
+* pyangbind.base.PybindBase - which is the parent class inherited by all container or module YANG objects.
+
+* pyangbind.pybindJSON - which containers wrapper functions which can be used to help with serialisation of YANG to JSON.
+
+* pyangbind.serialise.pybindJSONEncoder - a class that can be used as a custom encoder for the JSON module to serialise PyangBind class hierarchies to JSON.
+
+* pyangbind.serialise.pybindJSONDecoder - a class that can be used as a custom decoder to load JSON-encoded instances of YANG models into a PyangBind class hierarchy.
+
+* pyangbind.xpathhelper.YANGPathHelper - a class which can have objects registered against it, and subsequently retrieved from it using XPATH expressions. This module also includes parent classes that can be used to implement other helper modules of this nature.
+
+* pyangbind.yangtypes: The various functions which generate python types that are used to represent YANG types, and some helper methods.
+
+  - pyangbind.yangtypes.is_yang_list and is_yang_leaflist are self explainatory, but may be useful.
+
+  - pyangbind.yangtypes.safe_name is used throughout PyangBind to determine how to map YANG element names into Python attribute names safely.
+
+  - pyangbind.yangtypes.RestrictedPrecisionDecimalType - generates wrapped Decimal types that has a restricted set of decimal digits - i.e., can deal with fraction-digits arguments in YANG.
+
+  - pyangbind.yangtypes.RestrictedClassType - generates types which wrap a 'base' type (e.g., integer) with particular restrictions. The restrictions are supplied as a dictionary, or with specific arguments if single restrictions are required. Currently, the restrictions supported are regexp matches, ranges, lengths, and restrictions to a set of values (provided as keys to a dict).
+
+  - pyangbind.yangtypes.TypedListType - generates types which wrap a list to restrict the objects that it may contain.
+
+  - pyangbind.yangtypes.YANGListType - generates types which wrap a class representing a container, such that it acts as a YANG list.
+
+  - pyangbind.yangtypes.YANGBool - a boolean class.
+
+  - pyangbind.yangtypes.YANGDynClass - generates types which consist of a wrapper (YANGDynClass) and a wrapped object which may be any other class. YANGDynClass is a meta-class that provides additional data on top of the attributes and functions of the wrapped class.
+
+  - pyangbind.yangtypes.ReferenceType - generates types which can use a pyangbind.xpathhelper.PybindXpathHelper instance to look up values - particularly to support leafrefs in YANG.
+
+Usage documentation for PyangBind itself can be found on GitHub: https://github.com/robshakir/pyangbind
```

