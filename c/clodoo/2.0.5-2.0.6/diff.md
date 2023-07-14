# Comparing `tmp/clodoo-2.0.5.tar.gz` & `tmp/clodoo-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clodoo-2.0.5.tar", last modified: Tue May  9 17:25:22 2023, max compression
+gzip compressed data, was "dist/clodoo-2.0.6.tar", last modified: Fri Jul 14 15:46:13 2023, max compression
```

## Comparing `clodoo-2.0.5.tar` & `clodoo-2.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:22.000000 clodoo-2.0.5/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:22.000000 clodoo-2.0.5/clodoo/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 clodoo-2.0.5/clodoo/__main__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5934 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/update_coa.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    47741 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/clodoocore.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21644 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/odoo_install_repository
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    29780 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/transodoo.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    23877 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/clodoolib.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:22.000000 clodoo-2.0.5/clodoo/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2665 2023-05-09 17:25:01.000000 clodoo-2.0.5/clodoo/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6918 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 clodoo-2.0.5/clodoo/scripts/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)   232831 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/clodoo.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)    24448 2023-04-02 18:39:37.000000 clodoo-2.0.5/clodoo/transodoo.xlsx
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    14545 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/manage_odoo
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20723 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/manage_db
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3077 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/check_one2many.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8612 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/export_db_model.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8765 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/moduli_da_installare.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      701 2022-12-09 05:08:44.000000 clodoo-2.0.5/clodoo/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    97606 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/migrate_odoo_db.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    32167 2023-05-09 15:46:57.000000 clodoo-2.0.5/clodoo/odoorc
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-09 17:25:22.000000 clodoo-2.0.5/setup.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2665 2023-05-09 15:46:57.000000 clodoo-2.0.5/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1623 2023-05-09 17:25:22.000000 clodoo-2.0.5/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    17782 2023-05-09 17:25:22.000000 clodoo-2.0.5/README.rst
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:22.000000 clodoo-2.0.5/clodoo.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        7 2023-05-09 17:25:22.000000 clodoo-2.0.5/clodoo.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-09 17:25:22.000000 clodoo-2.0.5/clodoo.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:50:55.000000 clodoo-2.0.5/clodoo.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       58 2023-05-09 17:25:22.000000 clodoo-2.0.5/clodoo.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      654 2023-05-09 17:25:22.000000 clodoo-2.0.5/clodoo.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      100 2023-05-09 17:25:22.000000 clodoo-2.0.5/clodoo.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1623 2023-05-09 17:25:22.000000 clodoo-2.0.5/clodoo.egg-info/PKG-INFO
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 15:46:13.000000 clodoo-2.0.6/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 15:46:13.000000 clodoo-2.0.6/clodoo/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      164 2023-06-24 06:17:11.000000 clodoo-2.0.6/clodoo/__main__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5931 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/update_coa.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    50851 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/clodoocore.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21644 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/odoo_install_repository
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    29780 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/transodoo.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    24390 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/clodoolib.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 15:46:13.000000 clodoo-2.0.6/clodoo/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2717 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6918 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2023-05-14 13:22:41.000000 clodoo-2.0.6/clodoo/scripts/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)   233286 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/clodoo.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)    24448 2023-04-02 18:39:37.000000 clodoo-2.0.6/clodoo/transodoo.xlsx
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    14545 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/manage_odoo
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20723 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/manage_db
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3077 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/check_one2many.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8612 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/export_db_model.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8765 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/moduli_da_installare.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      759 2023-06-24 06:17:11.000000 clodoo-2.0.6/clodoo/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    93670 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/migrate_odoo_db.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    34327 2023-07-13 18:19:43.000000 clodoo-2.0.6/clodoo/odoorc
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-07-14 15:46:13.000000 clodoo-2.0.6/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2717 2023-07-13 18:19:43.000000 clodoo-2.0.6/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1623 2023-07-14 15:46:13.000000 clodoo-2.0.6/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4635 2023-07-13 18:19:43.000000 clodoo-2.0.6/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 15:46:13.000000 clodoo-2.0.6/clodoo.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        7 2023-07-14 15:46:13.000000 clodoo-2.0.6/clodoo.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-07-14 15:46:13.000000 clodoo-2.0.6/clodoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:50:55.000000 clodoo-2.0.6/clodoo.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       58 2023-07-14 15:46:13.000000 clodoo-2.0.6/clodoo.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      654 2023-07-14 15:46:13.000000 clodoo-2.0.6/clodoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      100 2023-07-14 15:46:13.000000 clodoo-2.0.6/clodoo.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1623 2023-07-14 15:46:13.000000 clodoo-2.0.6/clodoo.egg-info/PKG-INFO
```

### Comparing `clodoo-2.0.5/clodoo/update_coa.py` & `clodoo-2.0.6/clodoo/update_coa.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 # import pdb
 
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
@@ -128,21 +128,21 @@
 
 def update_coa(ctx):
     company_id = ctx["company_id"]
     model = "account.account"
     if len(clodoo.searchL8(ctx, model, [("company_id", "=", company_id)])) < 100:
         return
     company = clodoo.browseL8(ctx, "res.company", company_id)
-    print( "- Processing company %s" % company.name)
+    print("- Processing company %s" % company.name)
     for code in ("__", "A", "P", "R", "S"):
         ids = clodoo.searchL8(
             ctx, model, [("code", "=", code), ("company_id", "=", company_id)]
         )
         if len(ids) > 2:
-            print( "Warning: invalid account '%s'" % code)
+            print("Warning: invalid account '%s'" % code)
             sys.exit(1)
         elif ids:
             vals = get_code_values(ctx, code)
             try:
                 clodoo.writeL8(ctx, model, ids[0], vals)
             except BaseException:
                 pass
@@ -190,12 +190,12 @@
                 vals["parent_id"] = parent_id
                 clodoo.writeL8(ctx, model, account_id, vals)
 
 
 if __name__ == "__main__":
     # pdb.set_trace()
     oerp, uid, ctx = init_n_connect()
-    print( "Update Chart of Account on DB %s" % (ctx["db_name"]))
+    print("Update Chart of Account on DB %s" % (ctx["db_name"]))
     ids = clodoo.searchL8(ctx, "res.company", [])
     for company_id in ids:
         ctx["company_id"] = company_id
         update_coa(ctx)
```

### Comparing `clodoo-2.0.5/clodoo/clodoocore.py` & `clodoo-2.0.6/clodoo/clodoocore.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,32 @@
 from builtins import str
 
 # from builtins import *                                           # noqa: F403
 from past.utils import old_div
 import sys
 import re
 
-import odoorpc
-
 try:
-    import oerplib
+    import odoorpc
 except ImportError:
-    if sys.version_info[0] == 2:
-        raise ImportError("Package oerplib not found")
+    raise ImportError("Package odoorpc not found!")
+if sys.version_info[0] == 2:
+    try:
+        import oerplib
+    except ImportError:
+        raise ImportError("Package oerplib not found!")
+else:
+    try:
+        import oerplib3
+    except ImportError:
+        try:
+            import odoolib
+        except ImportError:
+            raise ImportError("Package oerplib3 / odoo-client-lib not found!")
+
 from os0 import os0
 
 try:
     from clodoolib import debug_msg_log, msg_log, decrypt
 except ImportError:
     from clodoo.clodoolib import debug_msg_log, msg_log, decrypt
 try:
@@ -53,15 +64,15 @@
 standard_library.install_aliases()  # noqa: E402
 
 
 STS_FAILED = 1
 STS_SUCCESS = 0
 
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 #############################################################################
 # Low level (driver) functions
 def psql_connect(ctx):
     cr = False
     if postgres_drive and ctx.get("psycopg2", False):
@@ -75,26 +86,48 @@
     return cr
 
 
 #############################################################################
 # Connection and database
 #
 def cnx(ctx):
+    port = ctx.get("http_port") or ctx.get("xmlrpc_port")
+    if "." in ctx["oe_version"] and int(ctx["oe_version"].split(".")[0]) < 10:
+        port = ctx.get("xmlrpc_port") or ctx.get("http_port")
     try:
         if ctx["svc_protocol"] == "jsonrpc":
-            odoo = odoorpc.ODOO(ctx["db_host"], ctx["svc_protocol"], ctx["xmlrpc_port"])
-        else:
+            odoo = odoorpc.ODOO(ctx["db_host"], ctx["svc_protocol"], port)
+            ctx["odoo_cnx"] = odoo
+            ctx["pypi"] = "odoorpc"
+        elif sys.version_info[0] == 2:
             odoo = oerplib.OERP(
                 server=ctx["db_host"],
                 protocol=ctx["svc_protocol"],
-                port=ctx["xmlrpc_port"],
+                port=port,
+            )
+            ctx["odoo_cnx"] = odoo
+            ctx["pypi"] = "oerplib"
+        elif "oerplib3" in globals():
+            odoo = oerplib3.OERP(
+                server=ctx["db_host"],
+                protocol=ctx["svc_protocol"],
+                port=port,
             )
-            # version=ctx['oe_version'])
+            ctx["odoo_cnx"] = odoo
+            ctx["pypi"] = "oerplib3"
+        else:
+            odoo = odoolib.get_connector(
+                hostname=ctx["db_host"], protocol=ctx["svc_protocol"], port=port
+            )
+            ctx["odoo_cnx"] = odoo
+            ctx["pypi"] = "odoo-client-lib"
     except BaseException:  # pragma: no cover
         odoo = False
+        ctx["odoo_cnx"] = odoo
+        ctx["pypi"] = ""
     return odoo
 
 
 def exec_sql(ctx, query, response=None):
     ctx["_cr"] = psql_connect(ctx)
     try:
         ctx["_cr"].execute(query)
@@ -127,21 +160,23 @@
         if ctx["oe_version"] != "*":
             return "!Odoo server %s is not running!" % ctx["oe_version"]
         if ctx["svc_protocol"] == "jsonrpc" and sys.version_info[0] == 2:
             ctx["svc_protocol"] = "xmlrpc"
         odoo = cnx(ctx)
         if not odoo:
             return "!Odoo server %s is not running!" % ctx["oe_version"]
-    if ctx["svc_protocol"] == "jsonrpc":
+    if ctx["pypi"] == "odoorpc":
         ctx["server_version"] = odoo.version
-    else:
+    elif ctx["pypi"].startswith("oerplib"):
         try:
             ctx["server_version"] = odoo.db.server_version()
         except BaseException:
-            ctx["server_version"] = odoo.version
+            ctx["server_version"] = ctx["oe_version"]
+    else:
+        ctx["server_version"] = odoo.get_service("db").server_version()
     x = re.match(r"[0-9]+\.[0-9]+", ctx["server_version"])
     if (
         ctx["oe_version"] != "*"
         and ctx["server_version"][0 : x.end()] != ctx["oe_version"]
     ):
         return "!Invalid Odoo Server version: expected %s, found %s!" % (
             ctx["oe_version"],
@@ -149,94 +184,136 @@
         )
     elif ctx["oe_version"] == "*":
         ctx["oe_version"] = ctx["server_version"][0 : x.end()]
     ctx["majver"] = eval(ctx["server_version"].split(".")[0])
     if ctx["majver"] < 10 and ctx["svc_protocol"] == "jsonrpc":
         ctx["svc_protocol"] = "xmlrpc"
         return connectL8(ctx)
-    ctx["odoo_session"] = odoo
+    ctx["cnx"] = ctx["odoo_session"] = odoo
     return True
 
 
 #############################################################################
 # Primitive version indipendent
 #
-def searchL8(ctx, model, where, order=None, context=None):
-    if ctx["svc_protocol"] == "jsonrpc":
+def create_model_object(ctx, resource, id, deep=3):
+    model = ctx["odoo_session"].get_model(resource)
+    values = model.read(id, [])
+    fields = model.fields_get()
+    for k, v in values.items():
+        if k == "id":
+            setattr(model, k, v)
+        elif fields[k]["type"] == "many2one":
+            if v and deep:
+                rel_model = fields[k]["relation"]
+                setattr(
+                    model, k, create_model_object(ctx, rel_model, v[0], deep=deep - 1)
+                )
+            else:
+                setattr(model, k, v)
+        elif fields[k]["type"] in ("one2many", "many2many"):
+            setattr(model, k, v)
+        else:
+            setattr(model, k, v)
+    return model
+
+
+def searchL8(ctx, model, domain, order=None, context=None):
+    if ctx["pypi"] == "odoorpc":
         return (
-            ctx["odoo_session"].env[model].search(where, order=order, context=context)
+            ctx["odoo_session"].env[model].search(domain, order=order, context=context)
         )
-    else:
-        return ctx["odoo_session"].search(model, where, order=order, context=context)
+    elif ctx["pypi"].startswith("oerplib"):
+        return ctx["odoo_session"].search(model, domain, order=order, context=context)
+    elif ctx["pypi"] == "odoo-client-lib":
+        if order:
+            return ctx["odoo_session"].get_model(model).search(domain, order=order)
+        return ctx["odoo_session"].get_model(model).search(domain)
 
 
 def browseL8(ctx, model, id, context=None):
-    if ctx["svc_protocol"] == "jsonrpc":
+    if ctx["pypi"] == "odoorpc":
         if context:
             return ctx["odoo_session"].env[model].browse(id).with_context(context)
         else:
             return ctx["odoo_session"].env[model].browse(id)
-    else:
+    elif ctx["pypi"].startswith("oerplib"):
         return ctx["odoo_session"].browse(model, id, context=context)
+    elif ctx["pypi"] == "odoo-client-lib":
+        if isinstance(id, (list, tuple)):
+            res = []
+            for ii in id:
+                res.append(create_model_object(ctx, model, ii))
+            return res
+        return create_model_object(ctx, model, id)
 
 
 def createL8(ctx, model, vals, context=None):
     vals = drop_invalid_fields(ctx, model, vals)
     vals = complete_fields(ctx, model, vals)
-    if ctx["svc_protocol"] == "jsonrpc":
+    if ctx["pypi"] == "odoorpc":
         if context:
             return ctx["odoo_session"].env[model].create(vals).with_context(context)
         else:
             return ctx["odoo_session"].env[model].create(vals)
-    else:
+    elif ctx["pypi"].startswith("oerplib"):
         return ctx["odoo_session"].create(model, vals)
-
-
-#
-#
-# def write_recordL8(ctx, record):
-#     # vals = drop_invalid_fields(ctx, model, vals)
-#     if ctx['svc_protocol'] == 'jsonrpc':
-#         model = record.__class__.__name__
-#         ctx['odoo_session'].env[model].write(record)
-#     else:
-#         ctx['odoo_session'].write_record(record)
+    elif ctx["pypi"] == "odoo-client-lib":
+        return ctx["odoo_session"].get_model(model).create(vals)
 
 
 def writeL8(ctx, model, ids, vals, context=None):
     vals = drop_invalid_fields(ctx, model, vals)
-    if ctx["svc_protocol"] == "jsonrpc":
+    if ctx["pypi"] == "odoorpc":
         if context:
             return (
                 ctx["odoo_session"]
                 .env[model]
                 .browse(ids)
                 .with_context(context)
                 .write(vals)
             )
         else:
             return ctx["odoo_session"].env[model].write(ids, vals)
-    else:
+    elif ctx["pypi"].startswith("oerplib"):
         return ctx["odoo_session"].write(model, ids, vals, context=context)
+    elif ctx["pypi"] == "odoo-client-lib":
+        return ctx["odoo_session"].get_model(model).write(ids, vals)
 
 
 def unlinkL8(ctx, model, ids):
-    if ctx["svc_protocol"] == "jsonrpc":
+    ids = ids if isinstance(ids, (list, tuple)) else [ids]
+    if ctx["pypi"] == "odoorpc":
         return ctx["odoo_session"].env[model].unlink(ids)
-    else:
+    elif ctx["pypi"].startswith("oerplib"):
         return ctx["odoo_session"].unlink(model, ids)
+    elif ctx["pypi"] == "odoo-client-lib":
+        return (
+            ctx["odoo_session"]
+            .get_model(model)
+            .unlink(ids if isinstance(ids, (list, tuple)) else [ids])
+        )
 
 
 def executeL8(ctx, model, action, *args):
     action = translate_from_to(
         ctx, model, action, "10.0", ctx["oe_version"], type="action"
     )
     if ctx["majver"] < 10 and action == "invoice_open":
         return ctx["odoo_session"].exec_workflow(model, action, *args)
-    return ctx["odoo_session"].execute(model, action, *args)
+    if ctx["pypi"] in ("odoorpc", "oerplib", "oerplib3"):
+        return ctx["odoo_session"].execute(model, action, *args)
+    elif ctx["pypi"] == "odoo-client-lib":
+        return (
+            ctx["odoo_session"]
+            .get_service('object')
+            .execute_kw(
+                ctx["db_name"], ctx["user_id"], ctx["_pwd"], model, action, *args
+            )
+        )
 
 
 def execute_action_L8(ctx, model, action, ids):
     sts = 0
     if model == "account.invoice":
         ids = [ids] if isinstance(ids, int) else ids
         try:
@@ -452,15 +529,14 @@
     ctx, model, vals, new_name, name, src_ver, tgt_ver, default=None
 ):
     vals = {}
     return vals
 
 
 def cvt_from_ver_2_ver(ctx, model, src_ver, tgt_ver, vals):
-
     APPLY = {
         "account.account.type": {"type": "acc_type()", "report_type": "acc_type()"},
         "account.account": {"child_id": "child_id()"},
         "account.tax": {"type": "group()", "type_tax_use": "type_tax_use()"},
         "res.partner": {"is_company": "true", "vat": "vat()", "state_id": "state_id()"},
         "ir.sequence": {"code": "seq_code()"},
     }
@@ -1337,15 +1413,15 @@
                 translate_from_to(
                     ctx, value[0], name, value[1], value[2], ctx["oe_version"]
                 )
                 != ""
             )
         else:
             return translate_from_sym(ctx, value[0], value[1], ctx["oe_version"]) != ""
-    if ctx["svc_protocol"] == "jsonrpc":
+    if ctx["pypi"] == "odoorpc":
         if (
             model
             and name
             and value
             and ctx["odoo_session"]
             .env[model]
             .search([(name[0], "=", value[0]), (name[1], "=", value[1])])
```

### Comparing `clodoo-2.0.5/clodoo/odoo_install_repository` & `clodoo-2.0.6/clodoo/odoo_install_repository`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.5
+__version__=2.0.6
 
 rmdir_if_exists() {
     #rmdir_if_exists (DSTPATH REPOS odoo_vid new_vid)
     local DSTPATH="$1" REPOS="$2" odoo_vid="$3" new_vid="$4"
     local b fn CWD
     local odoo_fver=$(build_odoo_param FULLVER "$odoo_vid")
     if [[ -d $DSTPATH ]]; then
```

### Comparing `clodoo-2.0.5/clodoo/transodoo.py` & `clodoo-2.0.6/clodoo/transodoo.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     from z0lib.z0lib import z0lib
 except ImportError:
     try:
         from z0lib import z0lib
     except ImportError:
         import z0lib
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 VERSIONS = [
     "6.1",
     "7.0",
     "8.0",
     "9.0",
     "10.0",
     "11.0",
```

### Comparing `clodoo-2.0.5/clodoo/clodoolib.py` & `clodoo-2.0.6/clodoo/clodoolib.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import unicode_literals
 
 from future import standard_library
 
 # from builtins import chr
 # from builtins import str
 # from builtins import *                                           # noqa: F403
-from past.builtins import unicode
+from past.builtins import unicode, basestring
 import argparse
 
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 import inspect
@@ -65,14 +65,15 @@
     "login_password",
     "crypt2_password",
     "login2_password",
     "admin_passwd",
     "db_host",
     "db_port",
     "data_dir",
+    "http_port",
     "xmlrpc_port",
     "oe_version",
     "zeroadm_mail",
     "zeroadm_login",
     "oneadm_mail",
     "oneadm_login",
     "oneadm_pwd",
@@ -173,15 +174,16 @@
     "lang",
     "with_demo",
     "no_fvalidation",
     "lgi_user",
     "lgi_pwd",
     "logfn",
     "quiet_mode",
-    "xmlrpc_port",
+    # "http_port",
+    # "xmlrpc_port",
     "odoo_vid",
     "exit_onerror",
     "data_selection",
 )
 # List of pure boolean parameters in line command; may be in LX_CFG_S list too
 LX_OPT_B = ("dry_run", "with_demo", "no_fvalidation", "exit_onerror")
 # List of numeric parameters in line command; may be in LX_CFG_S list too
@@ -194,15 +196,15 @@
 # switch values of options
 LX_OPT_ARGS = {}
 DEFDCT = {}
 
 msg_time = time.time()
 
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 #############################################################################
 # Message and output
 #
 def init_logger(ctx):
     if ctx["quiet_mode"]:
@@ -335,16 +337,16 @@
         "admin_passwd": "admin",
         "db_user": "postgres",
         "db_host": "localhost",
         "data_dir": "",
         "db_port": 5432,
         "oe_version": "*",
         "svc_protocol": "",
-        "xmlrpc_port": 8069,
-        "odoo_vid": "12.0",
+        # "http_port": 8069,
+        # "odoo_vid": "12.0",
         "db_name": "demo",
         "logfile": False,
         "dbfilter": ".*",
         "dbfilterd": "demo",
         "dbfiltert": "(openerp|odoo|test)",
         "dbfilterz": "zi[0-9]{8}",
         "dbtypefilter": "",
@@ -400,16 +402,27 @@
     }
 
 
 def get_versioned_option(conf_obj, sect, param, is_bool=None, defval=None):
     is_bool = is_bool or False
     found = False
     if conf_obj:
-        for sfx in ("6.1", "7.0", "8.0", "9.0", "10.0",
-                    "11.0", "12.0", "13.0", "14.0", "15.0", "16.0"):
+        for sfx in (
+            "6.1",
+            "7.0",
+            "8.0",
+            "9.0",
+            "10.0",
+            "11.0",
+            "12.0",
+            "13.0",
+            "14.0",
+            "15.0",
+            "16.0",
+        ):
             vparam = "%s_%s" % (param, sfx)
             if conf_obj.has_option(sect, vparam):
                 found = True
                 break
     if not found:
         vparam = param
         if conf_obj and conf_obj.has_option(sect, vparam):
@@ -502,19 +515,17 @@
                 "uninstall_modules",
                 "upgrade_modules",
                 "purge_modules",
             ):
                 ctx[opt_obj.do_sel_action] = opt_obj.modules_2_manage
         if hasattr(opt_obj, "data_path") and opt_obj.data_path != "":
             ctx["data_path"] = opt_obj.data_path
-    # if ctx['db_host'] == 'False':
-    #     ctx['db_host'] = 'localhost'
-    if "oe_version" in ctx and not ctx.get("odoo_vid"):
+    if ctx.get("oe_version") and ctx["oe_version"] != "*" and not ctx.get("odoo_vid"):
         ctx["odoo_vid"] = ctx["oe_version"]
-    else:
+    elif ctx.get("odoo_vid") and ctx["odoo_vid"] != "*":
         ctx["oe_version"] = build_odoo_param("FULLVER", ctx["odoo_vid"])
     if not ctx["svc_protocol"]:
         if ctx["oe_version"] in ("9.0", "8.0", "7.0", "6.1"):
             ctx["svc_protocol"] = "xmlrpc"
         else:
             ctx["svc_protocol"] = "jsonrpc"
     if ctx.get("do_sel_action", False):
@@ -524,14 +535,17 @@
         del ctx["actions_db"]
     elif ctx.get("actions_mc", None):
         ctx["actions"] = "per_company," + ctx["actions_mc"]
         del ctx["actions_mc"]
     elif ctx.get("actions_uu", None):
         ctx["actions"] = "per_users," + ctx["actions_uu"]
         del ctx["actions_uu"]
+    for p in ("http_port", "xmlrpc_port", "db_port"):
+        if isinstance(ctx.get(p), basestring) and ctx[p].isdigit():
+            ctx[p] = int(ctx[p])
     return ctx
 
 
 def docstring_summary(docstring):
     """Return summary of docstring."""
     for text in docstring.split("\n"):
         if text.strip():
@@ -558,15 +572,15 @@
 
 def read_config(ctx):
     """Read both user configuration and local configuration."""
 
     def set_confs(ctx):
         version_is_set = False
         for ver in ("odoo_vid", "oe_version"):
-            if ctx.get(ver):
+            if ctx.get(ver) and ctx[ver] != "*":
                 fnver = build_odoo_param("CONFN", ctx[ver], multi=True)
                 if os.path.isfile(fnver) and fnver not in ctx["conf_fns"]:
                     ctx["conf_fns"].insert(0, fnver)
                     version_is_set = True
                 else:
                     fnver = build_odoo_param("CONFN", ctx[ver])
                     if os.path.isfile(fnver) and fnver not in ctx["conf_fns"]:
@@ -582,16 +596,22 @@
     ctx["_conf_obj"] = ConfigParser.RawConfigParser(default_conf(ctx))
     ctx["conf_fns"] = ctx["_conf_obj"].read(ctx["conf_fns"])
     if not ctx["conf_fns"]:
         raise IOError("No configuration file found!")
     ctx = create_params_dict(ctx)
     if not version_is_set:
         ctx, version_is_set = set_confs(ctx)
-        ctx["conf_fns"] = ctx["_conf_obj"].read(ctx["conf_fns"])
-        ctx = create_params_dict(ctx)
+        if version_is_set:
+            ctx["conf_fns"] = ctx["_conf_obj"].read(ctx["conf_fns"])
+            ctx = create_params_dict(ctx)
+    if (not ctx.get("http_port") and not ctx.get("xmlrpc_port")):
+        if int(ctx.get("oe_version", "12.0").split(".")[0]) < 10:
+            ctx["xmlrpc_port"] = 8069
+        else:
+            ctx["http_port"] = 8069
     return ctx
 
 
 def create_parser(version, doc, ctx):
     """Return command-line parser.
     Some options are standard:
     -c --config     set configuration file (conf_fn)
@@ -701,17 +721,17 @@
         help="run silently",
         action="store_true",
         dest="quiet_mode",
         default=False,
     )
     parser.add_argument(
         "-r",
-        "--xmlrpc-port",
-        help="xmlrpc port",
-        dest="xmlrpc_port",
+        "--http-port",
+        help="http / xmlrpc port",
+        dest="http_port",
         metavar="port",
         default="",
     )
     parser.add_argument(
         "-S",
         "--data-selection",
         help="Select data to remove",
@@ -823,19 +843,17 @@
 
 
 def build_odoo_param(
     item, odoo_vid=None, debug=None, suppl=None, git_org=None, multi=None
 ):
     fct = "build_odoo_%s" % item
     if fct in globals():
-        return globals()[fct](odoo_vid=odoo_vid,
-                              debug=debug,
-                              suppl=suppl,
-                              git_org=git_org,
-                              multi=multi)
+        return globals()[fct](
+            odoo_vid=odoo_vid, debug=debug, suppl=suppl, git_org=git_org, multi=multi
+        )
     odoorc = os.path.join(os.path.dirname(__file__), "odoorc")
     if multi:
         cmd = 'opt_multi=1 %s %s "%s" "%s" "%s"' % (
             odoorc,
             item,
             odoo_vid,
             suppl or "",
```

### Comparing `clodoo-2.0.5/clodoo/scripts/setup.info` & `clodoo-2.0.6/clodoo/scripts/setup.info`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+# -*- coding: utf-8 -*-
 import sys
 
 from setuptools import find_packages, setup
 
 if sys.version_info >= (3, 0):
     install_requires = [
         "future",
         "jsonlib-python3",
         "openpyxl",
         "odoorpc",
-        "oerplib",
+        "oerplib3",
+        "odoo-client-lib",
         "os0",
         "psycopg2-binary",
         "python-plus",
         "unidecode",
         "z0lib",
     ]
 else:
@@ -27,15 +29,15 @@
         "python-plus",
         "unidecode==1.2.0",
         "z0lib",
     ]
 
 setup(
     name="clodoo",
-    version="2.0.5",
+    version="2.0.6",
     description="Do massive operations on Odoo Cloud",
     long_description="""
 Clodoo is a set of tools to manage to manage multiple Odoo installations with many DBs.
 
 With clodoo you can do massive operations on 1 or more Odoo databases based on
 different Odoo versions. Main operation are:
```

### Comparing `clodoo-2.0.5/clodoo/scripts/main.py` & `clodoo-2.0.6/clodoo/scripts/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
```

### Comparing `clodoo-2.0.5/clodoo/clodoo.py` & `clodoo-2.0.6/clodoo/clodoo.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,101 +148,155 @@
     'Z' for zeroincombenze production,
     'V' for VG7 customers
     'C' other customers
 oe_versions: select record if matches Odoo version
     i.e  +11.0+10.0 => select record if Odoo 11.0 or 10.0
     i.e  -6.1-7.0 => select record if Odoo is not 6.1 and not 7.0
 """
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
+from __future__ import absolute_import, division, print_function, unicode_literals
 
 import calendar
 import csv
 import inspect
 import os.path
 import platform
 import re
 import sys
 import time
+
 # from builtins import *                                           # noqa: F403
 from builtins import input, object
 from datetime import date, datetime, timedelta
 
 from future import standard_library
+
 # from builtins import str
 # from builtins import range
 from past.builtins import basestring
 
+if sys.version_info[0] == 3:
+    try:
+        import oerplib3         # noqa: F401
+    except ImportError:
+        try:
+            import odoolib
+        except ImportError:
+            raise ImportError("Package oerplib3 / odoo-client-lib not found!")
+
 # from passlib.context import CryptContext
 from os0 import os0
 from python_plus import _c
 
 try:
-    from clodoo.clodoocore import browseL8  # noqa: F401; noqa: F401
-    from clodoo.clodoocore import build_model_struct  # noqa: F401
-    from clodoo.clodoocore import connectL8  # noqa: F401
-    from clodoo.clodoocore import execute_action_L8  # noqa: F401
-    from clodoo.clodoocore import extr_table_generic  # noqa: F401
+    from clodoo.clodoocore import browseL8              # noqa: F401
+    from clodoo.clodoocore import build_model_struct    # noqa: F401
+    from clodoo.clodoocore import connectL8             # noqa: F401
+    from clodoo.clodoocore import execute_action_L8     # noqa: F401
+    from clodoo.clodoocore import extr_table_generic    # noqa: F401
     from clodoo.clodoocore import extract_vals_from_rec  # noqa: F401
-    from clodoo.clodoocore import get_val_from_field  # noqa: F401
-    from clodoo.clodoocore import import_file_get_hdr  # noqa: F401
-    from clodoo.clodoocore import model_has_company  # noqa: F401
-    from clodoo.clodoocore import put_model_alias  # noqa: F401
-    from clodoo.clodoocore import (createL8, cvt_from_ver_2_ver, eval_value,
-                                   exec_sql, executeL8, get_company_id,
-                                   get_model_model, get_model_name,
-                                   get_model_structure, get_query_id,
-                                   get_res_users, is_required_field,
-                                   is_valid_field, psql_connect, searchL8,
-                                   set_some_values, sql_reconnect, unlinkL8,
-                                   writeL8)
+    from clodoo.clodoocore import get_val_from_field    # noqa: F401
+    from clodoo.clodoocore import import_file_get_hdr   # noqa: F401
+    from clodoo.clodoocore import model_has_company     # noqa: F401
+    from clodoo.clodoocore import put_model_alias       # noqa: F401
+    from clodoo.clodoocore import (                     # noqa: F401
+        createL8,
+        cvt_from_ver_2_ver,
+        eval_value,
+        exec_sql,
+        executeL8,
+        get_company_id,
+        get_model_model,
+        get_model_name,
+        get_model_structure,
+        get_query_id,
+        get_res_users,
+        is_required_field,
+        is_valid_field,
+        psql_connect,
+        searchL8,
+        set_some_values,
+        sql_reconnect,
+        unlinkL8,
+        writeL8,
+        create_model_object,
+    )
 except ImportError:
-    from clodoocore import browseL8  # noqa: F401; noqa: F401
-    from clodoocore import build_model_struct  # noqa: F401
-    from clodoocore import connectL8  # noqa: F401
-    from clodoocore import execute_action_L8  # noqa: F401
-    from clodoocore import extr_table_generic  # noqa: F401
+    from clodoocore import browseL8             # noqa: F401
+    from clodoocore import build_model_struct   # noqa: F401
+    from clodoocore import connectL8            # noqa: F401
+    from clodoocore import execute_action_L8    # noqa: F401
+    from clodoocore import extr_table_generic   # noqa: F401
     from clodoocore import extract_vals_from_rec  # noqa: F401
-    from clodoocore import get_val_from_field  # noqa: F401
+    from clodoocore import get_val_from_field   # noqa: F401
     from clodoocore import import_file_get_hdr  # noqa: F401
-    from clodoocore import model_has_company  # noqa: F401
-    from clodoocore import put_model_alias  # noqa: F401
-    from clodoocore import (createL8, cvt_from_ver_2_ver, eval_value,  # noqa: F401
-                            exec_sql, executeL8, get_company_id,  # noqa: F401
-                            get_model_model, get_model_name,  # noqa: F401
-                            get_model_structure, get_query_id,  # noqa: F401
-                            get_res_users, is_required_field,  # noqa: F401
-                            is_valid_field, psql_connect, searchL8,  # noqa: F401
-                            set_some_values, sql_reconnect, unlinkL8,  # noqa: F401
-                            writeL8)  # noqa: F401
+    from clodoocore import model_has_company    # noqa: F401
+    from clodoocore import put_model_alias      # noqa: F401
+    from clodoocore import (   # noqa: F401
+        createL8,
+        cvt_from_ver_2_ver,
+        eval_value,
+        exec_sql,
+        executeL8,
+        get_company_id,
+        get_model_model,
+        get_model_name,
+        get_model_structure,
+        get_query_id,
+        get_res_users,
+        is_required_field,
+        is_valid_field,
+        psql_connect,
+        searchL8,
+        set_some_values,
+        sql_reconnect,
+        unlinkL8,
+        writeL8,
+        create_model_object,
+    )
 try:
-    from clodoo.clodoolib import init_logger  # noqa: F401; noqa: F401
-    from clodoo.clodoolib import msg_burst  # noqa: F401
-    from clodoo.clodoolib import tounicode  # noqa: F401
-    from clodoo.clodoolib import (build_odoo_param, crypt, debug_msg_log,
-                                  decrypt, default_conf, msg_log, parse_args,
-                                  read_config, set_base_ctx)
+    from clodoo.clodoolib import init_logger    # noqa: F401
+    from clodoo.clodoolib import msg_burst      # noqa: F401
+    from clodoo.clodoolib import tounicode      # noqa: F401
+    from clodoo.clodoolib import (
+        build_odoo_param,       # noqa: F401
+        crypt,
+        debug_msg_log,
+        decrypt,
+        default_conf,
+        msg_log,
+        parse_args,
+        read_config,
+        set_base_ctx,
+    )
 except ImportError:
-    from clodoolib import init_logger  # noqa: F401; noqa: F401
-    from clodoolib import msg_burst  # noqa: F401
-    from clodoolib import tounicode  # noqa: F401
-    from clodoolib import (build_odoo_param, crypt, debug_msg_log,  # noqa: F401
-                           decrypt, default_conf, msg_log, parse_args,  # noqa: F401
-                           read_config, set_base_ctx)  # noqa: F401
+    from clodoolib import init_logger   # noqa: F401
+    from clodoolib import msg_burst     # noqa: F401
+    from clodoolib import tounicode     # noqa: F401
+    from clodoolib import (             # noqa: F401
+        build_odoo_param,
+        crypt,
+        debug_msg_log,
+        decrypt,
+        default_conf,
+        msg_log,
+        parse_args,
+        read_config,
+        set_base_ctx,
+    )
 try:
     from transodoo import read_stored_dict, translate_from_to
 except ImportError:
     from clodoo.transodoo import read_stored_dict, translate_from_to
 
 # TMP
 from subprocess import PIPE, Popen
 
 standard_library.install_aliases()  # noqa: E402
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 # Apply for configuration file (True/False)
 APPLY_CONF = True
 STS_FAILED = 1
 STS_SUCCESS = 0
 
 PAY_MOVE_STS_2_DRAFT = ['posted']
@@ -311,22 +365,57 @@
 # Connection and database
 #
 def open_connection(ctx):
     """Open connection to Odoo service"""
     res = connectL8(ctx)
     if isinstance(res, basestring):
         raise RuntimeError(res)  # pragma: no cover
-    return ctx['odoo_session']
+    return ctx['odoo_cnx']
 
 
 def do_login(ctx):
     """Do a login into DB; try using more usernames and passwords"""
 
     def get_login_user(ctx):
-        return ctx['odoo_session'].env.user
+        return ctx['odoo_cnx'].env.user
+
+    def try_to_login(ctx, pwd):
+        if ctx["pypi"] == "odoorpc":
+            try:
+                ctx['odoo_cnx'].login(db=db_name, login=username, password=pwd)
+            except BaseException:
+                return False
+            user = get_login_user(ctx)
+            ctx['user_id'] = user.id
+            ctx["_pwd"] = pwd
+            return user
+        elif ctx["pypi"].startswith("oerplib"):
+            try:
+                user = ctx['odoo_cnx'].login(
+                    database=db_name, user=username, passwd=pwd
+                )
+                ctx['user_id'] = user.id
+                ctx["_pwd"] = pwd
+                return user
+            except BaseException:
+                return False
+        elif ctx["pypi"] == "odoo-client-lib":
+            connection = odoolib.Connection(ctx['odoo_cnx'], db_name, username, pwd)
+            if not connection:
+                return False
+            try:
+                connection.check_login(True)
+            except BaseException:
+                return False
+            ctx["odoo_session"] = connection
+            ctx['user_id'] = connection.user_id
+            ctx["_pwd"] = pwd
+            model = "res.users"
+            user = create_model_object(ctx, model, connection.user_id)
+            return user
 
     msg = "do_login()"
     debug_msg_log(ctx, ctx['level'] + 1, msg)
     userlist = ctx['login_user'].split(',')
     for u in ctx['login2_user'].split(','):
         if u and u not in userlist:
             userlist.append(u)
@@ -359,54 +448,30 @@
     user = False
     db_name = get_dbname(ctx, 'login')
     for username in userlist:
         for pwd in cryptlist:
             crypted = True
             msg = "do_login_%s(%s,$1$%s)" % (ctx['svc_protocol'], username, pwd)
             debug_msg_log(ctx, ctx['level'] + 2, msg)
-            if ctx['svc_protocol'] == 'jsonrpc':
-                try:
-                    ctx['odoo_session'].login(
-                        db=db_name, login=username, password=decrypt(pwd)
-                    )
-                except BaseException:
-                    continue
-                # Keep out of try / except to catch user error
-                user = get_login_user(ctx)
+            user = try_to_login(ctx, decrypt(pwd))
+            if user:
                 break
-            else:
-                try:
-                    user = ctx['odoo_session'].login(
-                        database=db_name, user=username, passwd=decrypt(pwd)
-                    )
-                    break
-                except BaseException:
-                    pass
+
         if not user:
             crypted = False
             for pwd in pwdlist:
-                try:
-                    msg = "do_login_%s(%s,$1$%s)" % (
-                        ctx['svc_protocol'],
-                        username,
-                        crypt(pwd),
-                    )
-                    debug_msg_log(ctx, ctx['level'] + 2, msg)
-                    if ctx['svc_protocol'] == 'jsonrpc':
-                        ctx['odoo_session'].login(
-                            db=db_name, login=username, password=pwd
-                        )
-                        user = get_login_user(ctx)
-                    else:
-                        user = ctx['odoo_session'].login(
-                            database=db_name, user=username, passwd=pwd
-                        )
+                msg = "do_login_%s(%s,$1$%s)" % (
+                    ctx['svc_protocol'],
+                    username,
+                    crypt(pwd),
+                )
+                debug_msg_log(ctx, ctx['level'] + 2, msg)
+                user = try_to_login(ctx, pwd)
+                if user:
                     break
-                except BaseException:
-                    pass
         if user:
             break
     if not user:
         if not ctx.get('no_warning_pwd', False):
             os0.wlog("!DB={}: invalid user/pwd".format(tounicode(ctx['db_name'])))
         return
     if not ctx['multi_user']:
@@ -471,14 +536,15 @@
     db=None,
     xmlrpc_port=None,
     oe_version=None,
     user=None,
     pwd=None,
     lang=None,
     ctx=None,
+    http_port=None,
 ):
     D_LIST = (
         'ena_inquire',
         'caller',
         'level',
         'dry_run',
         'multi_user',
@@ -496,48 +562,50 @@
         'login_password',
         'crypt_password',
         'login2_user',
         'login2_password',
         'crypt2_password',
         'svc_protocol',
         'oe_version',
-        'xmlrpc_port',
+        'http_port',
+        "xmlrpc_port",
         'lang',
         'psycopg2',
     )
     DEFLT = default_conf(ctx)
 
     def oerp_env_fill(
         db=None,
         xmlrpc_port=None,
         oe_version=None,
         user=None,
         pwd=None,
         lang=None,
         ctx=None,
         inquire=None,
+        http_port=None,
     ):
         ctx = ctx or {}
         for p in D_LIST + P_LIST:
             if p == 'db_name' and db:
                 ctx[p] = db
             elif p == 'login_user' and user:
                 ctx[p] = user
             elif p == 'login_password' and pwd:
                 ctx[p] = pwd
-            elif p == 'xmlrpc_port' and xmlrpc_port:
+            elif p == 'http_port' and http_port:
+                if isinstance(http_port, basestring):
+                    ctx[p] = int(http_port)
+                else:
+                    ctx[p] = http_port
+            elif p == 'xmlrpc_port' and xmlrpc_port and not http_port:
                 if isinstance(xmlrpc_port, basestring):
                     ctx[p] = int(xmlrpc_port)
                 else:
                     ctx[p] = xmlrpc_port
-            # elif p == 'db_port' and xmlrpc_port:
-            #     if isinstance(xmlrpc_port, basestring):
-            #         ctx[p] = int(xmlrpc_port)
-            #     else:
-            #         ctx[p] = xmlrpc_port
             elif p == 'oe_version' and oe_version and oe_version != '*':
                 ctx[p] = oe_version
                 if not ctx.get('odoo_vid'):
                     ctx['odoo_vid'] = ctx['oe_version']
             elif p == 'svc_protocol' and (p not in ctx or not ctx[p]):
                 if ctx.get('oe_version') in ('6.1', '7.0', '8.0'):
                     ctx[p] = 'xmlrpc'
@@ -565,14 +633,15 @@
         db=db,
         xmlrpc_port=xmlrpc_port,
         user=user,
         pwd=pwd,
         oe_version=oe_version or ctx.get('oe_version'),
         lang=lang,
         ctx=ctx,
+        http_port=http_port,
     )
     open_connection(ctx)
     if ctx['no_login']:
         return False, ctx
     lgiuser = do_login(ctx)
     if not lgiuser:
         raise RuntimeError('Invalid user or password!')  # pragma: no cover
@@ -647,15 +716,15 @@
     if ctx.get('company_country_id', 0) != 0:
         ctx['def_country_id'] = ctx['company_country_id']
         ctx['country_code'] = browseL8(ctx, 'res.country', ctx['def_country_id']).code
     return ctx
 
 
 def init_user_ctx(ctx, user):
-    ctx['user_id'] = user.id
+    # ctx['user_id'] = user.id
     if ctx['oe_version'] != "6.1":
         ctx['user_partner_id'] = user.partner_id.id
     ctx['user_name'] = get_res_users(ctx, user, 'name')
     ctx['def_email'] = '%s%s@example.com' % (
         user.login,
         ctx['oe_version'].split('.')[0],
     )
@@ -677,15 +746,15 @@
         for r in res.split('\n'):
             rs = r.split('|')
             if len(rs) > 2 and rs[1] == 'odoo12':
                 list.append(rs[0])
         return list
     elif ctx['oe_version'] == '7.0':  # FIX
         time.sleep(1)
-    return ctx['odoo_session'].db.list()
+    return ctx['odoo_cnx'].db.list()
 
 
 def get_companylist(ctx):
     return searchL8(ctx, 'res.company', [], order='id desc')
 
 
 def get_userlist(ctx):
@@ -1163,16 +1232,16 @@
         while sts == STS_FAILED and ctr > 0:
             try:
                 cmd = 'pg_db_active -wa %s' % db_name
                 os0.muteshell(cmd, simulate=False, keepout=False)
                 if ctx['oe_version'] == '12.0':  # FIX: odoorpc wont work 12.0
                     os0.muteshell("dropdb -Upostgres --if-exists " + db_name)
                 else:
-                    ctx['odoo_session'].db.drop(ctx['admin_passwd'], db_name)
-                # ctx['odoo_session'].db.drop(ctx['admin_passwd'],
+                    ctx['odoo_cnx'].db.drop(ctx['admin_passwd'], db_name)
+                # ctx['odoo_cnx'].db.drop(ctx['admin_passwd'],
                 #                             db_name)
                 sts = STS_SUCCESS
                 if db_name[0:11] != 'clodoo_test':
                     time.sleep(2)
             except BaseException:
                 ctr -= 1
                 if db_name[0:11] != 'clodoo_test':
@@ -1309,34 +1378,34 @@
         if ctx['db_name'] == 'auto':
             ctx['db_name'] = create_zero_db(ctx)
             msg = "Assigned name is %s" % (ctx['db_name'])
             msg_log(ctx, ctx['level'], msg)
         if ctx['db_name']:
             if ctx['crypt_password']:
                 pwd = decrypt(ctx['crypt_password'])
-                ctx['server_version'] = ctx['odoo_session'].version
+                ctx['server_version'] = ctx['odoo_cnx'].version
             else:
                 pwd = ctx['login_password']
                 try:
-                    ctx['server_version'] = ctx['odoo_session'].db.server_version()
+                    ctx['server_version'] = ctx['odoo_cnx'].db.server_version()
                 except BaseException:
-                    ctx['server_version'] = ctx['odoo_session'].version
+                    ctx['server_version'] = ctx['odoo_cnx'].version
             try:
                 if ctx['svc_protocol'] == 'jsonrpc':
-                    ctx['odoo_session'].db.create(
+                    ctx['odoo_cnx'].db.create(
                         ctx['admin_passwd'], ctx['db_name'], ctx['with_demo'], lang, pwd
                     )
                     time.sleep(3)
                     open_connection(ctx)  # Needed for 11.0
                 elif ctx['server_version'] == '7.0':
-                    ctx['odoo_session'].db.create_and_wait(
+                    ctx['odoo_cnx'].db.create_and_wait(
                         ctx['admin_passwd'], ctx['db_name'], ctx['with_demo'], lang, pwd
                     )
                 else:
-                    ctx['odoo_session'].db.create_database(
+                    ctx['odoo_cnx'].db.create_database(
                         ctx['admin_passwd'], ctx['db_name'], ctx['with_demo'], lang, pwd
                     )
                     time.sleep(3)
             except BaseException:
                 sts = STS_FAILED
             if sts == STS_SUCCESS:
                 ctx['no_warning_pwd'] = True
```

### Comparing `clodoo-2.0.5/clodoo/transodoo.xlsx` & `clodoo-2.0.6/clodoo/transodoo.xlsx`

 * *Files identical despite different names*

### Comparing `clodoo-2.0.5/clodoo/manage_odoo` & `clodoo-2.0.6/clodoo/manage_odoo`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.5
+__version__=2.0.6
 
 
 explore() {
 # explore(odoo_vid excl_list)
     local res=OCB
     local pkgdir=$(build_odoo_param HOME "$1" "" "$opt_org" "$opt_deploy")
     for fn in $pkgdir/*; do
```

### Comparing `clodoo-2.0.5/clodoo/manage_db` & `clodoo-2.0.6/clodoo/manage_db`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.5
+__version__=2.0.6
 
 
 up_oemod() {
 #up_oemod(DB branch)
     local DB=$1
     local oe_version=$2
     local passed_file=./upd_oemod_passed.log
```

### Comparing `clodoo-2.0.5/clodoo/check_one2many.py` & `clodoo-2.0.6/clodoo/check_one2many.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     try:
         from z0lib import z0lib
     except ImportError:
         import z0lib
 # import pdb
 
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
     t = time.time() - msg_time
     if t > 3:
```

### Comparing `clodoo-2.0.5/clodoo/export_db_model.py` & `clodoo-2.0.6/clodoo/export_db_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     try:
         from z0lib import z0lib
     except ImportError:
         import z0lib
 # import pdb
 
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 CACHE = {}
 
 
 def get_symbolic_value(ctx, model, name, value):
     name_model = "ir.model.data"
```

### Comparing `clodoo-2.0.5/clodoo/moduli_da_installare.py` & `clodoo-2.0.6/clodoo/moduli_da_installare.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     try:
         from z0lib import z0lib
     except ImportError:
         import z0lib
 # import transodoo
 # import pdb
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 VERSIONS = ["vg7", "61", "70", "80", "90", "100", "110", "120"]
 VERSIONS_PLUS = ["vg7", "61", "70", "80", "90", "100", "110", "120", "0"]
 ALIAS = {}
```

### Comparing `clodoo-2.0.5/clodoo/__init__.py` & `clodoo-2.0.6/clodoo/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,22 +9,24 @@
         extract_vals_from_rec,
         get_val_from_field,
         cvt_from_ver_2_ver,
         get_model_structure,
         is_valid_field,
         is_required_field,
         model_has_company,
+        create_model_object,
     )
 except:
     from clodoo.clodoocore import (
         extract_vals_from_rec,
         get_val_from_field,
         cvt_from_ver_2_ver,
         get_model_structure,
         is_valid_field,
         is_required_field,
         model_has_company,
+        create_model_object,
     )
 try:
     from clodoolib import build_odoo_param, crypt
 except:
     from clodoo.clodoolib import build_odoo_param, crypt
```

### Comparing `clodoo-2.0.5/clodoo/migrate_odoo_db.py` & `clodoo-2.0.6/clodoo/migrate_odoo_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,6085 +17,5839 @@
 00000100: 0a69 6d70 6f72 7420 7469 6d65 0a69 6d70  .import time.imp
 00000110: 6f72 7420 696e 7370 6563 740a 696d 706f  ort inspect.impo
 00000120: 7274 2067 6574 7061 7373 0a69 6d70 6f72  rt getpass.impor
 00000130: 7420 636f 6e74 6578 746c 6962 0a69 6d70  t contextlib.imp
 00000140: 6f72 7420 7368 7574 696c 0a69 6d70 6f72  ort shutil.impor
 00000150: 7420 7265 0a66 726f 6d20 7375 6270 726f  t re.from subpro
 00000160: 6365 7373 2069 6d70 6f72 7420 506f 7065  cess import Pope
-00000170: 6e0a 7472 793a 0a20 2020 2069 6d70 6f72  n.try:.    impor
-00000180: 7420 436f 6e66 6967 5061 7273 6572 0a65  t ConfigParser.e
-00000190: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
-000001a0: 723a 0a20 2020 2069 6d70 6f72 7420 636f  r:.    import co
-000001b0: 6e66 6967 7061 7273 6572 2061 7320 436f  nfigparser as Co
-000001c0: 6e66 6967 5061 7273 6572 0a66 726f 6d20  nfigParser.from 
-000001d0: 756e 6964 6563 6f64 6520 696d 706f 7274  unidecode import
-000001e0: 2075 6e69 6465 636f 6465 0a66 726f 6d20   unidecode.from 
-000001f0: 6f73 3020 696d 706f 7274 206f 7330 0a74  os0 import os0.t
-00000200: 7279 3a0a 2020 2020 6672 6f6d 2063 6c6f  ry:.    from clo
-00000210: 646f 6f20 696d 706f 7274 2063 6c6f 646f  doo import clodo
-00000220: 6f0a 6578 6365 7074 2049 6d70 6f72 7445  o.except ImportE
-00000230: 7272 6f72 3a0a 2020 2020 696d 706f 7274  rror:.    import
-00000240: 2063 6c6f 646f 6f0a 7472 793a 0a20 2020   clodoo.try:.   
-00000250: 2066 726f 6d20 7a30 6c69 622e 7a30 6c69   from z0lib.z0li
-00000260: 6220 696d 706f 7274 207a 306c 6962 0a65  b import z0lib.e
-00000270: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
-00000280: 723a 0a20 2020 2074 7279 3a0a 2020 2020  r:.    try:.    
-00000290: 2020 2020 6672 6f6d 207a 306c 6962 2069      from z0lib i
-000002a0: 6d70 6f72 7420 7a30 6c69 620a 2020 2020  mport z0lib.    
-000002b0: 6578 6365 7074 2049 6d70 6f72 7445 7272  except ImportErr
-000002c0: 6f72 3a0a 2020 2020 2020 2020 696d 706f  or:.        impo
-000002d0: 7274 207a 306c 6962 0a69 6d70 6f72 7420  rt z0lib.import 
-000002e0: 7472 616e 736f 646f 6f0a 2320 696d 706f  transodoo.# impo
-000002f0: 7274 2070 6462 0a0a 0a5f 5f76 6572 7369  rt pdb...__versi
-00000300: 6f6e 5f5f 203d 2022 322e 302e 3522 0a4d  on__ = "2.0.5".M
-00000310: 4158 5f44 4545 5020 3d20 3230 0a53 5953  AX_DEEP = 20.SYS
-00000320: 5445 4d5f 4d4f 4445 4c5f 524f 4f54 203d  TEM_MODEL_ROOT =
-00000330: 205b 0a20 2020 2027 6261 7365 2e63 6f6e   [.    'base.con
-00000340: 6669 672e 272c 0a20 2020 2027 6261 7365  fig.',.    'base
-00000350: 5f69 6d70 6f72 742e 272c 0a20 2020 2027  _import.',.    '
-00000360: 6261 7365 2e6c 616e 6775 6167 652e 272c  base.language.',
-00000370: 0a20 2020 2027 6261 7365 2e6d 6f64 756c  .    'base.modul
-00000380: 652e 272c 0a20 2020 2027 6261 7365 2e73  e.',.    'base.s
-00000390: 6574 7570 2e27 2c0a 2020 2020 2762 6173  etup.',.    'bas
-000003a0: 652e 7570 6461 7465 2e27 2c0a 2020 2020  e.update.',.    
-000003b0: 2769 722e 6163 7469 6f6e 732e 272c 0a20  'ir.actions.',. 
-000003c0: 2020 2027 6972 2e65 7870 6f72 7473 2e27     'ir.exports.'
-000003d0: 2c0a 2020 2020 2769 722e 6d6f 6465 6c2e  ,.    'ir.model.
-000003e0: 272c 0a20 2020 2027 6972 2e6d 6f64 756c  ',.    'ir.modul
-000003f0: 652e 272c 0a20 2020 2027 6972 2e71 7765  e.',.    'ir.qwe
-00000400: 622e 272c 0a20 2020 2027 7265 706f 7274  b.',.    'report
-00000410: 2e27 2c0a 2020 2020 2772 6573 2e63 6f6e  .',.    'res.con
-00000420: 6669 672e 272c 0a20 2020 2027 7765 625f  fig.',.    'web_
-00000430: 6564 6974 6f72 2e27 2c0a 2020 2020 2777  editor.',.    'w
-00000440: 6562 5f74 6f75 722e 272c 0a20 2020 2027  eb_tour.',.    '
-00000450: 776f 726b 666c 6f77 2e27 2c0a 5d0a 5359  workflow.',.].SY
-00000460: 5354 454d 5f4d 4f44 454c 5320 3d20 5b0a  STEM_MODELS = [.
-00000470: 2020 2020 275f 756e 6b6e 6f77 6e27 2c0a      '_unknown',.
-00000480: 2020 2020 2762 6173 6527 2c0a 2020 2020      'base',.    
-00000490: 2320 2762 6173 652e 636f 6e66 6967 2e73  # 'base.config.s
-000004a0: 6574 7469 6e67 7327 2c0a 2020 2020 2762  ettings',.    'b
-000004b0: 6173 655f 696d 706f 7274 272c 0a20 2020  ase_import',.   
-000004c0: 2027 6368 616e 6765 2e70 6173 7377 6f72   'change.passwor
-000004d0: 642e 7769 7a61 7264 272c 0a20 2020 2027  d.wizard',.    '
-000004e0: 6972 2e61 7574 6f76 6163 7575 6d27 2c0a  ir.autovacuum',.
-000004f0: 2020 2020 2769 722e 636f 6e66 6967 5f70      'ir.config_p
-00000500: 6172 616d 6574 6572 272c 0a20 2020 2027  arameter',.    '
-00000510: 6972 2e65 7870 6f72 7473 272c 0a20 2020  ir.exports',.   
-00000520: 2027 6972 2e66 6965 6c64 732e 636f 6e76   'ir.fields.conv
-00000530: 6572 7465 7227 2c0a 2020 2020 2769 722e  erter',.    'ir.
-00000540: 6669 6c74 6572 7327 2c0a 2020 2020 2769  filters',.    'i
-00000550: 722e 6874 7470 272c 0a20 2020 2027 6972  r.http',.    'ir
-00000560: 2e6c 6f67 6769 6e67 272c 0a20 2020 2027  .logging',.    '
-00000570: 6972 2e6d 6f64 656c 272c 0a20 2020 2027  ir.model',.    '
-00000580: 6972 2e6e 6565 6461 6374 696f 6e5f 6d69  ir.needaction_mi
-00000590: 7869 6e27 2c0a 2020 2020 2769 722e 7177  xin',.    'ir.qw
-000005a0: 6562 272c 0a20 2020 2027 6972 2e72 756c  eb',.    'ir.rul
-000005b0: 6527 2c0a 2020 2020 2769 722e 7472 616e  e',.    'ir.tran
-000005c0: 736c 6174 696f 6e27 2c0a 2020 2020 2769  slation',.    'i
-000005d0: 722e 7569 2e6d 656e 7527 2c0a 2020 2020  r.ui.menu',.    
-000005e0: 2769 722e 7569 2e76 6965 7727 2c0a 2020  'ir.ui.view',.  
-000005f0: 2020 2769 722e 7661 6c75 6573 272c 0a20    'ir.values',. 
-00000600: 2020 2027 7265 706f 7274 272c 0a20 2020     'report',.   
-00000610: 2027 7265 732e 636f 6e66 6967 272c 0a20   'res.config',. 
-00000620: 2020 2027 7265 732e 666f 6e74 272c 0a20     'res.font',. 
-00000630: 2020 2027 7265 732e 7265 7175 6573 742e     'res.request.
-00000640: 6c69 6e6b 272c 0a20 2020 2027 7265 732e  link',.    'res.
-00000650: 7573 6572 732e 6c6f 6727 2c0a 2020 2020  users.log',.    
-00000660: 2777 6562 5f74 6f75 7227 2c0a 2020 2020  'web_tour',.    
-00000670: 2777 6f72 6b66 6c6f 7727 2c0a 5d0a 4947  'workflow',.].IG
-00000680: 4e4f 5245 5f46 4945 4c44 5320 3d20 7b0a  NORE_FIELDS = {.
-00000690: 2020 2020 2772 6573 2e70 6172 746e 6572      'res.partner
-000006a0: 273a 205b 2772 6561 5f63 6f64 6527 2c0a  ': ['rea_code',.
-000006b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000170: 6e0a 0a74 7279 3a0a 2020 2020 696d 706f  n..try:.    impo
+00000180: 7274 2043 6f6e 6669 6750 6172 7365 720a  rt ConfigParser.
+00000190: 6578 6365 7074 2049 6d70 6f72 7445 7272  except ImportErr
+000001a0: 6f72 3a0a 2020 2020 696d 706f 7274 2063  or:.    import c
+000001b0: 6f6e 6669 6770 6172 7365 7220 6173 2043  onfigparser as C
+000001c0: 6f6e 6669 6750 6172 7365 720a 6672 6f6d  onfigParser.from
+000001d0: 2075 6e69 6465 636f 6465 2069 6d70 6f72   unidecode impor
+000001e0: 7420 756e 6964 6563 6f64 650a 6672 6f6d  t unidecode.from
+000001f0: 206f 7330 2069 6d70 6f72 7420 6f73 300a   os0 import os0.
+00000200: 0a74 7279 3a0a 2020 2020 6672 6f6d 2063  .try:.    from c
+00000210: 6c6f 646f 6f20 696d 706f 7274 2063 6c6f  lodoo import clo
+00000220: 646f 6f0a 6578 6365 7074 2049 6d70 6f72  doo.except Impor
+00000230: 7445 7272 6f72 3a0a 2020 2020 696d 706f  tError:.    impo
+00000240: 7274 2063 6c6f 646f 6f0a 7472 793a 0a20  rt clodoo.try:. 
+00000250: 2020 2066 726f 6d20 7a30 6c69 622e 7a30     from z0lib.z0
+00000260: 6c69 6220 696d 706f 7274 207a 306c 6962  lib import z0lib
+00000270: 0a65 7863 6570 7420 496d 706f 7274 4572  .except ImportEr
+00000280: 726f 723a 0a20 2020 2074 7279 3a0a 2020  ror:.    try:.  
+00000290: 2020 2020 2020 6672 6f6d 207a 306c 6962        from z0lib
+000002a0: 2069 6d70 6f72 7420 7a30 6c69 620a 2020   import z0lib.  
+000002b0: 2020 6578 6365 7074 2049 6d70 6f72 7445    except ImportE
+000002c0: 7272 6f72 3a0a 2020 2020 2020 2020 696d  rror:.        im
+000002d0: 706f 7274 207a 306c 6962 0a69 6d70 6f72  port z0lib.impor
+000002e0: 7420 7472 616e 736f 646f 6f0a 0a23 2069  t transodoo..# i
+000002f0: 6d70 6f72 7420 7064 620a 0a0a 5f5f 7665  mport pdb...__ve
+00000300: 7273 696f 6e5f 5f20 3d20 2232 2e30 2e36  rsion__ = "2.0.6
+00000310: 220a 4d41 585f 4445 4550 203d 2032 300a  ".MAX_DEEP = 20.
+00000320: 5359 5354 454d 5f4d 4f44 454c 5f52 4f4f  SYSTEM_MODEL_ROO
+00000330: 5420 3d20 5b0a 2020 2020 2762 6173 652e  T = [.    'base.
+00000340: 636f 6e66 6967 2e27 2c0a 2020 2020 2762  config.',.    'b
+00000350: 6173 655f 696d 706f 7274 2e27 2c0a 2020  ase_import.',.  
+00000360: 2020 2762 6173 652e 6c61 6e67 7561 6765    'base.language
+00000370: 2e27 2c0a 2020 2020 2762 6173 652e 6d6f  .',.    'base.mo
+00000380: 6475 6c65 2e27 2c0a 2020 2020 2762 6173  dule.',.    'bas
+00000390: 652e 7365 7475 702e 272c 0a20 2020 2027  e.setup.',.    '
+000003a0: 6261 7365 2e75 7064 6174 652e 272c 0a20  base.update.',. 
+000003b0: 2020 2027 6972 2e61 6374 696f 6e73 2e27     'ir.actions.'
+000003c0: 2c0a 2020 2020 2769 722e 6578 706f 7274  ,.    'ir.export
+000003d0: 732e 272c 0a20 2020 2027 6972 2e6d 6f64  s.',.    'ir.mod
+000003e0: 656c 2e27 2c0a 2020 2020 2769 722e 6d6f  el.',.    'ir.mo
+000003f0: 6475 6c65 2e27 2c0a 2020 2020 2769 722e  dule.',.    'ir.
+00000400: 7177 6562 2e27 2c0a 2020 2020 2772 6570  qweb.',.    'rep
+00000410: 6f72 742e 272c 0a20 2020 2027 7265 732e  ort.',.    'res.
+00000420: 636f 6e66 6967 2e27 2c0a 2020 2020 2777  config.',.    'w
+00000430: 6562 5f65 6469 746f 722e 272c 0a20 2020  eb_editor.',.   
+00000440: 2027 7765 625f 746f 7572 2e27 2c0a 2020   'web_tour.',.  
+00000450: 2020 2777 6f72 6b66 6c6f 772e 272c 0a5d    'workflow.',.]
+00000460: 0a53 5953 5445 4d5f 4d4f 4445 4c53 203d  .SYSTEM_MODELS =
+00000470: 205b 0a20 2020 2027 5f75 6e6b 6e6f 776e   [.    '_unknown
+00000480: 272c 0a20 2020 2027 6261 7365 272c 0a20  ',.    'base',. 
+00000490: 2020 2023 2027 6261 7365 2e63 6f6e 6669     # 'base.confi
+000004a0: 672e 7365 7474 696e 6773 272c 0a20 2020  g.settings',.   
+000004b0: 2027 6261 7365 5f69 6d70 6f72 7427 2c0a   'base_import',.
+000004c0: 2020 2020 2763 6861 6e67 652e 7061 7373      'change.pass
+000004d0: 776f 7264 2e77 697a 6172 6427 2c0a 2020  word.wizard',.  
+000004e0: 2020 2769 722e 6175 746f 7661 6375 756d    'ir.autovacuum
+000004f0: 272c 0a20 2020 2027 6972 2e63 6f6e 6669  ',.    'ir.confi
+00000500: 675f 7061 7261 6d65 7465 7227 2c0a 2020  g_parameter',.  
+00000510: 2020 2769 722e 6578 706f 7274 7327 2c0a    'ir.exports',.
+00000520: 2020 2020 2769 722e 6669 656c 6473 2e63      'ir.fields.c
+00000530: 6f6e 7665 7274 6572 272c 0a20 2020 2027  onverter',.    '
+00000540: 6972 2e66 696c 7465 7273 272c 0a20 2020  ir.filters',.   
+00000550: 2027 6972 2e68 7474 7027 2c0a 2020 2020   'ir.http',.    
+00000560: 2769 722e 6c6f 6767 696e 6727 2c0a 2020  'ir.logging',.  
+00000570: 2020 2769 722e 6d6f 6465 6c27 2c0a 2020    'ir.model',.  
+00000580: 2020 2769 722e 6e65 6564 6163 7469 6f6e    'ir.needaction
+00000590: 5f6d 6978 696e 272c 0a20 2020 2027 6972  _mixin',.    'ir
+000005a0: 2e71 7765 6227 2c0a 2020 2020 2769 722e  .qweb',.    'ir.
+000005b0: 7275 6c65 272c 0a20 2020 2027 6972 2e74  rule',.    'ir.t
+000005c0: 7261 6e73 6c61 7469 6f6e 272c 0a20 2020  ranslation',.   
+000005d0: 2027 6972 2e75 692e 6d65 6e75 272c 0a20   'ir.ui.menu',. 
+000005e0: 2020 2027 6972 2e75 692e 7669 6577 272c     'ir.ui.view',
+000005f0: 0a20 2020 2027 6972 2e76 616c 7565 7327  .    'ir.values'
+00000600: 2c0a 2020 2020 2772 6570 6f72 7427 2c0a  ,.    'report',.
+00000610: 2020 2020 2772 6573 2e63 6f6e 6669 6727      'res.config'
+00000620: 2c0a 2020 2020 2772 6573 2e66 6f6e 7427  ,.    'res.font'
+00000630: 2c0a 2020 2020 2772 6573 2e72 6571 7565  ,.    'res.reque
+00000640: 7374 2e6c 696e 6b27 2c0a 2020 2020 2772  st.link',.    'r
+00000650: 6573 2e75 7365 7273 2e6c 6f67 272c 0a20  es.users.log',. 
+00000660: 2020 2027 7765 625f 746f 7572 272c 0a20     'web_tour',. 
+00000670: 2020 2027 776f 726b 666c 6f77 272c 0a5d     'workflow',.]
+00000680: 0a49 474e 4f52 455f 4649 454c 4453 203d  .IGNORE_FIELDS =
+00000690: 207b 0a20 2020 2027 7265 732e 7061 7274   {.    'res.part
+000006a0: 6e65 7227 3a20 5b0a 2020 2020 2020 2020  ner': [.        
+000006b0: 2772 6561 5f63 6f64 6527 2c0a 2020 2020  'rea_code',.    
 000006c0: 2020 2020 2763 6869 6c64 5f69 6473 272c      'child_ids',
-000006d0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-000006e0: 2020 2020 2020 2023 2027 636f 6d6d 6572         # 'commer
-000006f0: 6369 616c 5f70 6172 746e 6572 5f69 6427  cial_partner_id'
-00000700: 5d2c 0a20 2020 2027 6163 636f 756e 742e  ],.    'account.
-00000710: 6163 636f 756e 7427 3a20 5b27 7061 7265  account': ['pare
-00000720: 6e74 5f69 6427 2c0a 2020 2020 2020 2020  nt_id',.        
-00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000740: 2770 6172 656e 745f 6c65 6674 272c 0a20  'parent_left',. 
-00000750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000760: 2020 2020 2020 2027 7061 7265 6e74 5f72         'parent_r
-00000770: 6967 6874 275d 2c0a 2020 2020 272a 273a  ight'],.    '*':
-00000780: 2020 5b27 6d65 7373 6167 655f 666f 6c6c    ['message_foll
-00000790: 6f77 6572 5f69 6473 272c 0a20 2020 2020  ower_ids',.     
-000007a0: 2020 2020 2020 276d 6573 7361 6765 5f69        'message_i
-000007b0: 6473 272c 5d2c 0a0a 7d0a 4d41 4e44 4154  ds',],..}.MANDAT
-000007c0: 4f52 595f 4649 454c 4453 203d 207b 0a20  ORY_FIELDS = {. 
-000007d0: 2020 2027 6163 636f 756e 742e 696e 766f     'account.invo
-000007e0: 6963 6527 3a20 5b27 636f 6d70 616e 795f  ice': ['company_
-000007f0: 6964 275d 2c0a 7d0a 504b 4559 5320 3d20  id'],.}.PKEYS = 
-00000800: 7b0a 2020 2020 2772 6573 2e63 6f75 6e74  {.    'res.count
-00000810: 7279 273a 2028 5b27 636f 6465 275d 2c20  ry': (['code'], 
-00000820: 5b27 6e61 6d65 275d 292c 0a20 2020 2027  ['name']),.    '
-00000830: 7265 732e 636f 756e 7472 792e 7374 6174  res.country.stat
-00000840: 6527 3a20 285b 276e 616d 6527 5d2c 0a20  e': (['name'],. 
-00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000860: 2020 2020 2020 2020 205b 2763 6f64 6527           ['code'
-00000870: 2c20 2763 6f75 6e74 7279 5f69 6427 5d2c  , 'country_id'],
-00000880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000890: 2020 2020 2020 2020 2020 205b 2764 696d             ['dim
-000008a0: 5f6e 616d 6527 5d2c 292c 0a20 2020 2027  _name'],),.    '
-000008b0: 7265 732e 7061 7274 6e65 7227 3a20 285b  res.partner': ([
-000008c0: 2776 6174 272c 2027 6669 7363 616c 636f  'vat', 'fiscalco
-000008d0: 6465 272c 2027 6973 5f63 6f6d 7061 6e79  de', 'is_company
-000008e0: 272c 2027 7479 7065 275d 2c0a 2020 2020  ', 'type'],.    
-000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000900: 5b27 7661 7427 2c20 2766 6973 6361 6c63  ['vat', 'fiscalc
-00000910: 6f64 6527 2c20 2769 735f 636f 6d70 616e  ode', 'is_compan
-00000920: 7927 5d2c 0a20 2020 2020 2020 2020 2020  y'],.           
-00000930: 2020 2020 2020 2020 205b 2772 6561 5f63           ['rea_c
-00000940: 6f64 6527 5d2c 0a20 2020 2020 2020 2020  ode'],.         
-00000950: 2020 2020 2020 2020 2020 205b 2776 6174             ['vat
-00000960: 272c 2027 6e61 6d65 272c 2027 6973 5f63  ', 'name', 'is_c
-00000970: 6f6d 7061 6e79 272c 2027 7479 7065 275d  ompany', 'type']
-00000980: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000990: 2020 2020 2020 5b27 6669 7363 616c 636f        ['fiscalco
-000009a0: 6465 272c 2027 7479 7065 275d 2c0a 2020  de', 'type'],.  
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2020 5b27 7661 7427 2c20 2769 735f 636f    ['vat', 'is_co
-000009d0: 6d70 616e 7927 5d2c 0a20 2020 2020 2020  mpany'],.       
-000009e0: 2020 2020 2020 2020 2020 2020 205b 276e               ['n
-000009f0: 616d 6527 2c20 2769 735f 636f 6d70 616e  ame', 'is_compan
-00000a00: 7927 5d2c 0a20 2020 2020 2020 2020 2020  y'],.           
-00000a10: 2020 2020 2020 2020 205b 2776 6174 275d           ['vat']
-00000a20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000a30: 2020 2020 2020 5b27 6e61 6d65 275d 2c0a        ['name'],.
-00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a50: 2020 2020 5b27 6469 6d5f 6e61 6d65 275d      ['dim_name']
-00000a60: 2c29 2c0a 2020 2020 2772 6573 2e63 6f6d  ,),.    'res.com
-00000a70: 7061 6e79 273a 2028 5b27 7661 7427 5d2c  pany': (['vat'],
-00000a80: 292c 0a20 2020 2027 6163 636f 756e 742e  ),.    'account.
-00000a90: 6163 636f 756e 742e 7479 7065 273a 2028  account.type': (
-00000aa0: 5b27 6e61 6d65 275d 2c29 2c0a 2020 2020  ['name'],),.    
-00000ab0: 2761 6363 6f75 6e74 2e61 6363 6f75 6e74  'account.account
-00000ac0: 273a 2028 5b27 636f 6465 272c 2027 636f  ': (['code', 'co
-00000ad0: 6d70 616e 795f 6964 275d 2c0a 2020 2020  mpany_id'],.    
-00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000af0: 2020 2020 5b27 6e61 6d65 272c 2027 636f      ['name', 'co
-00000b00: 6d70 616e 795f 6964 275d 2c0a 2020 2020  mpany_id'],.    
-00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b20: 2020 2020 5b27 6469 6d5f 6e61 6d65 272c      ['dim_name',
-00000b30: 2027 636f 6d70 616e 795f 6964 275d 2c29   'company_id'],)
-00000b40: 2c0a 2020 2020 2770 726f 6475 6374 2e74  ,.    'product.t
-00000b50: 656d 706c 6174 6527 3a20 285b 276e 616d  emplate': (['nam
-00000b60: 6527 2c20 2764 6566 6175 6c74 5f63 6f64  e', 'default_cod
-00000b70: 6527 5d29 2c0a 2020 2020 2770 726f 6475  e']),.    'produ
-00000b80: 6374 2e70 726f 6475 6374 273a 2028 5b27  ct.product': (['
-00000b90: 6e61 6d65 272c 2027 6465 6661 756c 745f  name', 'default_
-00000ba0: 636f 6465 275d 2c0a 2020 2020 2020 2020  code'],.        
-00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bc0: 5b27 6e61 6d65 272c 2027 6261 7263 6f64  ['name', 'barcod
-00000bd0: 6527 5d2c 0a20 2020 2020 2020 2020 2020  e'],.           
-00000be0: 2020 2020 2020 2020 2020 2020 205b 276e               ['n
-00000bf0: 616d 6527 5d2c 0a20 2020 2020 2020 2020  ame'],.         
-00000c00: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00000c10: 2764 6566 6175 6c74 5f63 6f64 6527 5d2c  'default_code'],
-00000c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c30: 2020 2020 2020 2020 205b 2762 6172 636f           ['barco
-00000c40: 6465 275d 2c0a 2020 2020 2020 2020 2020  de'],.          
-00000c50: 2020 2020 2020 2020 2020 2020 2020 5b27                ['
-00000c60: 6469 6d5f 6e61 6d65 275d 2c29 2c0a 7d0a  dim_name'],),.}.
-00000c70: 4445 545f 4649 454c 4420 3d20 7b0a 2020  DET_FIELD = {.  
-00000c80: 2020 2761 6363 6f75 6e74 2e69 6e76 6f69    'account.invoi
-00000c90: 6365 273a 2027 696e 766f 6963 655f 6c69  ce': 'invoice_li
-00000ca0: 6e65 272c 0a20 2020 2027 7361 6c65 2e6f  ne',.    'sale.o
-00000cb0: 7264 6572 273a 2027 6f72 6465 725f 6c69  rder': 'order_li
-00000cc0: 6e65 272c 0a7d 0a56 4552 5349 4f4e 5320  ne',.}.VERSIONS 
-00000cd0: 3d20 2827 362e 3127 2c20 2737 2e30 272c  = ('6.1', '7.0',
-00000ce0: 2027 382e 3027 2c20 2739 2e30 272c 2027   '8.0', '9.0', '
-00000cf0: 3130 2e30 272c 2027 3131 2e30 272c 2027  10.0', '11.0', '
-00000d00: 3132 2e30 2729 0a44 4546 5f43 4f4e 4620  12.0').DEF_CONF 
-00000d10: 3d20 7b7d 0a4d 4f44 554c 4553 5f32 5f4c  = {}.MODULES_2_L
-00000d20: 4541 5645 5f42 4548 494e 4420 3d20 5b0a  EAVE_BEHIND = [.
-00000d30: 2020 2020 2770 726f 6365 7373 272c 0a5d      'process',.]
-00000d40: 0a50 5245 5f4d 4947 5241 5449 4f4e 203d  .PRE_MIGRATION =
-00000d50: 2027 2727 0a23 202d 2a2d 2063 6f64 696e   '''.# -*- codin
-00000d60: 673a 2075 7466 2d38 202d 2a2d 0a66 726f  g: utf-8 -*-.fro
-00000d70: 6d20 6f70 656e 6572 702e 6f70 656e 7570  m openerp.openup
-00000d80: 6772 6164 6520 696d 706f 7274 206f 7065  grade import ope
-00000d90: 6e75 7067 7261 6465 0a66 726f 6d20 6f70  nupgrade.from op
-00000da0: 656e 6572 702e 6164 646f 6e73 2e6f 7065  enerp.addons.ope
-00000db0: 6e75 7067 7261 6465 5f72 6563 6f72 6473  nupgrade_records
-00000dc0: 2e6c 6962 2069 6d70 6f72 7420 6170 7269  .lib import apri
-00000dd0: 6f72 690a 0a23 2058 4d4c 5f49 4453 2066  ori..# XML_IDS f
-00000de0: 6f72 6d61 7420 6973 205b 286f 6c64 5f78  ormat is [(old_x
-00000df0: 6964 2c20 6e65 775f 7869 6429 2e2e 2e5d  id, new_xid)...]
-00000e00: 0a78 6d6c 5f69 6473 203d 205b 0a20 2020  .xml_ids = [.   
-00000e10: 2024 7b78 6d6c 5f69 6473 7d0a 5d0a 0a0a   ${xml_ids}.]...
-00000e20: 6465 6620 636c 6561 6e75 705f 6d6f 6475  def cleanup_modu
-00000e30: 6c65 7328 6372 293a 0a20 2020 2023 204d  les(cr):.    # M
-00000e40: 6f64 756c 6520 6d65 7267 6564 2066 6f72  odule merged for
-00000e50: 6d61 7420 6973 205b 286f 6c64 5f6d 6f64  mat is [(old_mod
-00000e60: 756c 652c 206e 6577 5f6d 6f64 756c 6529  ule, new_module)
-00000e70: 2e2e 2e5d 0a20 2020 206f 7065 6e75 7067  ...].    openupg
-00000e80: 7261 6465 2e75 7064 6174 655f 6d6f 6475  rade.update_modu
-00000e90: 6c65 5f6e 616d 6573 280a 2020 2020 2020  le_names(.      
-00000ea0: 2020 6372 2c20 5b0a 2020 2020 2020 2020    cr, [.        
-00000eb0: 2020 2020 247b 6d6f 6475 6c65 5f6d 6572      ${module_mer
-00000ec0: 6765 647d 0a20 2020 2020 2020 205d 2c20  ged}.        ], 
-00000ed0: 6d65 7267 655f 6d6f 6475 6c65 733d 5472  merge_modules=Tr
-00000ee0: 7565 2c0a 2020 2020 290a 0a0a 406f 7065  ue,.    )...@ope
-00000ef0: 6e75 7067 7261 6465 2e6d 6967 7261 7465  nupgrade.migrate
-00000f00: 2829 0a64 6566 206d 6967 7261 7465 2863  ().def migrate(c
-00000f10: 722c 2076 6572 7369 6f6e 293a 0a20 2020  r, version):.   
-00000f20: 2063 722e 6578 6563 7574 6528 2764 726f   cr.execute('dro
-00000f30: 7020 7669 6577 2069 6620 6578 6973 7473  p view if exists
-00000f40: 2072 6570 6f72 745f 646f 6375 6d65 6e74   report_document
-00000f50: 5f75 7365 7220 6361 7363 6164 6527 290a  _user cascade').
-00000f60: 2020 2020 6f70 656e 7570 6772 6164 652e      openupgrade.
-00000f70: 7570 6461 7465 5f6d 6f64 756c 655f 6e61  update_module_na
-00000f80: 6d65 7328 0a20 2020 2020 2020 2063 722c  mes(.        cr,
-00000f90: 2061 7072 696f 7269 2e72 656e 616d 6564   apriori.renamed
-00000fa0: 5f6d 6f64 756c 6573 2e69 7465 7269 7465  _modules.iterite
-00000fb0: 6d73 2829 0a20 2020 2029 0a20 2020 206f  ms().    ).    o
-00000fc0: 7065 6e75 7067 7261 6465 2e72 656e 616d  penupgrade.renam
-00000fd0: 655f 786d 6c69 6473 2863 722c 2078 6d6c  e_xmlids(cr, xml
-00000fe0: 5f69 6473 290a 2020 2020 6f70 656e 7570  _ids).    openup
-00000ff0: 6772 6164 652e 6368 6563 6b5f 7661 6c75  grade.check_valu
-00001000: 6573 5f73 656c 6563 7469 6f6e 5f66 6965  es_selection_fie
-00001010: 6c64 280a 2020 2020 2020 2020 6372 2c20  ld(.        cr, 
-00001020: 2769 725f 6163 745f 7265 706f 7274 5f78  'ir_act_report_x
-00001030: 6d6c 272c 2027 7265 706f 7274 5f74 7970  ml', 'report_typ
-00001040: 6527 2c0a 2020 2020 2020 2020 5b27 636f  e',.        ['co
-00001050: 6e74 726f 6c6c 6572 272c 2027 7064 6627  ntroller', 'pdf'
-00001060: 2c20 2771 7765 622d 6874 6d6c 272c 2027  , 'qweb-html', '
-00001070: 7177 6562 2d70 6466 272c 2027 7378 7727  qweb-pdf', 'sxw'
-00001080: 2c20 2777 6562 6b69 7427 5d29 0a20 2020  , 'webkit']).   
-00001090: 206f 7065 6e75 7067 7261 6465 2e63 6865   openupgrade.che
-000010a0: 636b 5f76 616c 7565 735f 7365 6c65 6374  ck_values_select
-000010b0: 696f 6e5f 6669 656c 6428 0a20 2020 2020  ion_field(.     
-000010c0: 2020 2063 722c 2027 6972 5f75 695f 7669     cr, 'ir_ui_vi
-000010d0: 6577 272c 2027 7479 7065 272c 205b 0a20  ew', 'type', [. 
-000010e0: 2020 2020 2020 2020 2020 2027 6361 6c65             'cale
-000010f0: 6e64 6172 272c 2027 6469 6167 7261 6d27  ndar', 'diagram'
-00001100: 2c20 2766 6f72 6d27 2c20 2767 616e 7474  , 'form', 'gantt
-00001110: 272c 2027 6772 6170 6827 2c20 276b 616e  ', 'graph', 'kan
-00001120: 6261 6e27 2c0a 2020 2020 2020 2020 2020  ban',.          
-00001130: 2020 2771 7765 6227 2c20 2773 6561 7263    'qweb', 'searc
-00001140: 6827 2c20 2774 7265 6527 5d29 0a20 2020  h', 'tree']).   
-00001150: 2063 6c65 616e 7570 5f6d 6f64 756c 6573   cleanup_modules
-00001160: 2863 7229 0a27 2727 0a6d 7367 5f74 696d  (cr).'''.msg_tim
-00001170: 6520 3d20 7469 6d65 2e74 696d 6528 290a  e = time.time().
-00001180: 0a0a 6465 6620 6d73 675f 6275 7273 7428  ..def msg_burst(
-00001190: 7465 7874 293a 0a20 2020 2067 6c6f 6261  text):.    globa
-000011a0: 6c20 6d73 675f 7469 6d65 0a20 2020 2074  l msg_time.    t
-000011b0: 203d 2074 696d 652e 7469 6d65 2829 202d   = time.time() -
-000011c0: 206d 7367 5f74 696d 650a 2020 2020 6966   msg_time.    if
-000011d0: 2028 7420 3e20 3329 3a0a 2020 2020 2020   (t > 3):.      
-000011e0: 2020 7072 696e 7428 7465 7874 290a 2020    print(text).  
-000011f0: 2020 2020 2020 6d73 675f 7469 6d65 203d        msg_time =
-00001200: 2074 696d 652e 7469 6d65 2829 0a0a 0a40   time.time()...@
-00001210: 636f 6e74 6578 746c 6962 2e63 6f6e 7465  contextlib.conte
-00001220: 7874 6d61 6e61 6765 720a 6465 6620 7075  xtmanager.def pu
-00001230: 7368 6428 6e65 775f 6469 7229 3a0a 2020  shd(new_dir):.  
-00001240: 2020 7072 6576 696f 7573 5f64 6972 203d    previous_dir =
-00001250: 206f 732e 6765 7463 7764 2829 0a20 2020   os.getcwd().   
-00001260: 206f 732e 6368 6469 7228 6e65 775f 6469   os.chdir(new_di
-00001270: 7229 0a20 2020 2079 6965 6c64 0a20 2020  r).    yield.   
-00001280: 206f 732e 6368 6469 7228 7072 6576 696f   os.chdir(previo
-00001290: 7573 5f64 6972 290a 0a0a 6465 6620 6d61  us_dir)...def ma
-000012a0: 6e61 6765 5f65 7272 6f72 2829 3a0a 2020  nage_error():.  
-000012b0: 2020 6475 6d6d 7920 3d20 2727 0a20 2020    dummy = ''.   
-000012c0: 2077 6869 6c65 2064 756d 6d79 206e 6f74   while dummy not
-000012d0: 2069 6e20 2827 4927 2c20 2769 272c 2027   in ('I', 'i', '
-000012e0: 5327 2c20 2773 272c 2027 4427 2c20 2764  S', 's', 'D', 'd
-000012f0: 2729 3a0a 2020 2020 2020 2020 6475 6d6d  '):.        dumm
-00001300: 7920 3d20 696e 7075 7428 2728 4967 6e6f  y = input('(Igno
-00001310: 7265 2c20 5374 6f70 2c20 4465 6275 6729  re, Stop, Debug)
-00001320: 3f20 2729 0a20 2020 2020 2020 2069 6620  ? ').        if 
-00001330: 6e6f 7420 6475 6d6d 793a 0a20 2020 2020  not dummy:.     
-00001340: 2020 2020 2020 2064 756d 6d79 203d 2027         dummy = '
-00001350: 4927 0a20 2020 2020 2020 2069 6620 6475  I'.        if du
-00001360: 6d6d 7920 3d3d 2027 5327 206f 7220 6475  mmy == 'S' or du
-00001370: 6d6d 7920 3d3d 2027 7327 3a0a 2020 2020  mmy == 's':.    
-00001380: 2020 2020 2020 2020 7379 732e 6578 6974          sys.exit
-00001390: 2831 290a 2020 2020 2020 2020 6966 2064  (1).        if d
-000013a0: 756d 6d79 203d 3d20 2744 2720 6f72 2064  ummy == 'D' or d
-000013b0: 756d 6d79 203d 3d20 2764 273a 0a20 2020  ummy == 'd':.   
-000013c0: 2020 2020 2020 2020 2069 6d70 6f72 7420           import 
-000013d0: 7064 6220 2020 2020 2020 2020 2023 2070  pdb          # p
-000013e0: 796c 696e 743a 2064 6973 6162 6c65 3d64  ylint: disable=d
-000013f0: 6570 7265 6361 7465 642d 6d6f 6475 6c65  eprecated-module
-00001400: 0a20 2020 2020 2020 2020 2020 2070 6462  .            pdb
-00001410: 2e73 6574 5f74 7261 6365 2829 0a0a 0a64  .set_trace()...d
-00001420: 6566 2065 7865 635f 7371 6c28 6374 782c  ef exec_sql(ctx,
-00001430: 2071 7565 7279 2c20 7265 7370 6f6e 7365   query, response
-00001440: 3d4e 6f6e 6529 3a0a 2020 2020 7265 7475  =None):.    retu
-00001450: 726e 2063 6c6f 646f 6f2e 6578 6563 5f73  rn clodoo.exec_s
-00001460: 716c 2863 7478 2c20 7175 6572 792c 2072  ql(ctx, query, r
-00001470: 6573 706f 6e73 653d 7265 7370 6f6e 7365  esponse=response
-00001480: 290a 0a0a 6465 6620 636f 7079 5f64 6228  )...def copy_db(
-00001490: 6374 782c 206f 6c64 5f64 622c 206e 6577  ctx, old_db, new
-000014a0: 5f64 6229 3a0a 2020 2020 7371 6c20 3d20  _db):.    sql = 
-000014b0: 2764 726f 7020 6461 7461 6261 7365 2069  'drop database i
-000014c0: 6620 6578 6973 7473 2022 2573 2227 2025  f exists "%s"' %
-000014d0: 206e 6577 5f64 620a 2020 2020 7275 6e5f   new_db.    run_
-000014e0: 7472 6163 6564 2827 7067 5f64 625f 6163  traced('pg_db_ac
-000014f0: 7469 7665 272c 2027 2d77 6127 2c20 2725  tive', '-wa', '%
-00001500: 7327 2025 206e 6577 5f64 6229 0a20 2020  s' % new_db).   
-00001510: 2065 7865 635f 7371 6c28 6374 782c 2073   exec_sql(ctx, s
-00001520: 716c 290a 2020 2020 7371 6c20 3d20 2763  ql).    sql = 'c
-00001530: 7265 6174 6520 6461 7461 6261 7365 2022  reate database "
-00001540: 2573 2220 7769 7468 2074 656d 706c 6174  %s" with templat
-00001550: 6520 2225 7322 2720 2520 286e 6577 5f64  e "%s"' % (new_d
-00001560: 622c 206f 6c64 5f64 6229 0a20 2020 2063  b, old_db).    c
-00001570: 6c6f 646f 6f2e 7371 6c5f 7265 636f 6e6e  lodoo.sql_reconn
-00001580: 6563 7428 6374 7829 0a20 2020 2072 756e  ect(ctx).    run
-00001590: 5f74 7261 6365 6428 2770 675f 6462 5f61  _traced('pg_db_a
-000015a0: 6374 6976 6527 2c20 272d 7761 272c 2027  ctive', '-wa', '
-000015b0: 2573 2720 2520 6f6c 645f 6462 290a 2020  %s' % old_db).  
-000015c0: 2020 6966 206e 6f74 2065 7865 635f 7371    if not exec_sq
-000015d0: 6c28 6374 782c 2073 716c 293a 0a20 2020  l(ctx, sql):.   
-000015e0: 2020 2020 2073 716c 203d 2027 6372 6561       sql = 'crea
-000015f0: 7465 2064 6174 6162 6173 6520 2225 7322  te database "%s"
-00001600: 2720 2520 6e65 775f 6462 0a20 2020 2020  ' % new_db.     
-00001610: 2020 2065 7865 635f 7371 6c28 6374 782c     exec_sql(ctx,
-00001620: 2073 716c 290a 2020 2020 2020 2020 6f73   sql).        os
-00001630: 2e65 6e76 6972 6f6e 5b27 5047 5553 4552  .environ['PGUSER
-00001640: 275d 203d 2063 7478 5b27 6462 5f75 7365  '] = ctx['db_use
-00001650: 7227 5d0a 2020 2020 2020 2020 6966 206e  r'].        if n
-00001660: 6f74 206f 732e 656e 7669 726f 6e2e 6765  ot os.environ.ge
-00001670: 7428 2750 4748 4f53 5427 293a 0a20 2020  t('PGHOST'):.   
-00001680: 2020 2020 2020 2020 206f 732e 656e 7669           os.envi
-00001690: 726f 6e5b 2750 4748 4f53 5427 5d20 3d20  ron['PGHOST'] = 
-000016a0: 6374 785b 2764 625f 686f 7374 275d 0a20  ctx['db_host']. 
-000016b0: 2020 2020 2020 2069 6620 6e6f 7420 6f73         if not os
-000016c0: 2e65 6e76 6972 6f6e 2e67 6574 2827 5047  .environ.get('PG
-000016d0: 504f 5254 2729 3a0a 2020 2020 2020 2020  PORT'):.        
-000016e0: 2020 2020 6f73 2e65 6e76 6972 6f6e 5b27      os.environ['
-000016f0: 5047 504f 5254 275d 203d 2073 7472 2863  PGPORT'] = str(c
-00001700: 7478 5b27 6462 5f70 6f72 7427 5d29 0a20  tx['db_port']). 
-00001710: 2020 2020 2020 2063 6d64 203d 2027 7067         cmd = 'pg
-00001720: 5f64 756d 7020 2d55 2573 202d 2d66 6f72  _dump -U%s --for
-00001730: 6d61 743d 6375 7374 6f6d 202d 2d6e 6f2d  mat=custom --no-
-00001740: 7061 7373 776f 7264 2025 7320 2720 5c0a  password %s ' \.
-00001750: 2020 2020 2020 2020 2020 2020 2020 277c                '|
-00001760: 2070 675f 7265 7374 6f72 6520 2d55 2573   pg_restore -U%s
-00001770: 202d 2d6e 6f2d 7061 7373 776f 7264 202d   --no-password -
-00001780: 2d64 626e 616d 653d 2573 2720 2520 280a  -dbname=%s' % (.
-00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017a0: 2020 6374 785b 2764 625f 7573 6572 275d    ctx['db_user']
-000017b0: 2c20 6f6c 645f 6462 2c20 6374 785b 2764  , old_db, ctx['d
-000017c0: 625f 7573 6572 275d 2c20 6e65 775f 6462  b_user'], new_db
-000017d0: 290a 2020 2020 2020 2020 6f73 302e 776c  ).        os0.wl
-000017e0: 6f67 2827 3e3e 3e20 2573 2720 2520 636d  og('>>> %s' % cm
-000017f0: 6429 0a20 2020 2020 2020 2073 7473 203d  d).        sts =
-00001800: 2030 0a20 2020 2020 2020 2069 6620 6e6f   0.        if no
-00001810: 7420 7372 635f 6374 785b 2764 7279 5f72  t src_ctx['dry_r
-00001820: 756e 275d 3a0a 2020 2020 2020 2020 2020  un']:.          
-00001830: 2020 7374 7320 3d20 6f73 2e73 7973 7465    sts = os.syste
-00001840: 6d28 636d 6429 0a20 2020 2020 2020 2072  m(cmd).        r
-00001850: 6574 7572 6e20 2873 7473 203d 3d20 3029  eturn (sts == 0)
-00001860: 0a20 2020 2072 6574 7572 6e20 5472 7565  .    return True
-00001870: 0a0a 0a64 6566 2065 6e76 5f72 6566 2863  ...def env_ref(c
-00001880: 7478 2c20 7872 6566 293a 0a20 2020 2078  tx, xref):.    x
-00001890: 7265 6673 203d 2078 7265 662e 7370 6c69  refs = xref.spli
-000018a0: 7428 272e 2729 0a20 2020 2069 6620 6c65  t('.').    if le
-000018b0: 6e28 7872 6566 7329 203d 3d20 323a 0a20  n(xrefs) == 2:. 
-000018c0: 2020 2020 2020 2069 6473 203d 2063 6c6f         ids = clo
-000018d0: 646f 6f2e 7365 6172 6368 4c38 2863 7478  doo.searchL8(ctx
-000018e0: 2c20 2769 722e 6d6f 6465 6c2e 6461 7461  , 'ir.model.data
-000018f0: 272c 205b 2827 6d6f 6475 6c65 272c 2027  ', [('module', '
-00001900: 3d27 2c20 7872 6566 735b 305d 292c 0a20  =', xrefs[0]),. 
-00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001940: 2020 2020 2827 6e61 6d65 272c 2027 3d27      ('name', '='
-00001950: 2c20 7872 6566 735b 315d 295d 290a 2020  , xrefs[1])]).  
-00001960: 2020 2020 2020 6966 2069 6473 3a0a 2020        if ids:.  
-00001970: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00001980: 2063 6c6f 646f 6f2e 6272 6f77 7365 4c38   clodoo.browseL8
-00001990: 2863 7478 2c20 2769 722e 6d6f 6465 6c2e  (ctx, 'ir.model.
-000019a0: 6461 7461 272c 2069 6473 5b30 5d29 2e72  data', ids[0]).r
-000019b0: 6573 5f69 640a 2020 2020 7265 7475 726e  es_id.    return
-000019c0: 2046 616c 7365 0a0a 0a64 6566 2070 795f   False...def py_
-000019d0: 7265 6173 7369 676e 5f64 625f 6f77 6e65  reassign_db_owne
-000019e0: 7228 6374 782c 2064 626e 616d 652c 206f  r(ctx, dbname, o
-000019f0: 6c64 5f75 7365 722c 206e 6577 5f75 7365  ld_user, new_use
-00001a00: 7229 3a0a 2020 2020 666f 7220 7371 6c20  r):.    for sql 
-00001a10: 696e 2028 0a20 2020 2020 2020 2020 2020  in (.           
-00001a20: 2022 4752 414e 5420 414c 4c20 5052 4956   "GRANT ALL PRIV
-00001a30: 494c 4547 4553 204f 4e20 4441 5441 4241  ILEGES ON DATABA
-00001a40: 5345 2025 7320 544f 2025 7322 2025 2028  SE %s TO %s" % (
-00001a50: 6462 6e61 6d65 2c20 6e65 775f 7573 6572  dbname, new_user
-00001a60: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
-00001a70: 414c 5445 5220 4441 5441 4241 5345 2025  ALTER DATABASE %
-00001a80: 7320 4f57 4e45 5220 544f 2025 7322 2025  s OWNER TO %s" %
-00001a90: 2028 6462 6e61 6d65 2c20 6e65 775f 7573   (dbname, new_us
-00001aa0: 6572 292c 0a20 2020 2020 2020 2020 2020  er),.           
-00001ab0: 2022 4752 414e 5420 414c 4c20 5052 4956   "GRANT ALL PRIV
-00001ac0: 494c 4547 4553 204f 4e20 414c 4c20 5441  ILEGES ON ALL TA
-00001ad0: 424c 4553 2049 4e20 5343 4845 4d41 2070  BLES IN SCHEMA p
-00001ae0: 7562 6c69 6320 544f 2025 7322 2025 0a20  ublic TO %s" %. 
-00001af0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00001b00: 6577 5f75 7365 722c 0a20 2020 2020 2020  ew_user,.       
-00001b10: 2020 2020 2022 4752 414e 5420 414c 4c20       "GRANT ALL 
-00001b20: 5052 4956 494c 4547 4553 204f 4e20 414c  PRIVILEGES ON AL
-00001b30: 4c20 5345 5155 454e 4345 5320 494e 2053  L SEQUENCES IN S
-00001b40: 4348 454d 4120 7075 626c 6963 2054 4f20  CHEMA public TO 
-00001b50: 2573 2220 250a 2020 2020 2020 2020 2020  %s" %.          
-00001b60: 2020 2020 2020 6e65 775f 7573 6572 2c0a        new_user,.
-00001b70: 2020 2020 2020 2020 2020 2020 2247 5241              "GRA
-00001b80: 4e54 2041 4c4c 2050 5249 5649 4c45 4745  NT ALL PRIVILEGE
-00001b90: 5320 4f4e 2041 4c4c 2046 554e 4354 494f  S ON ALL FUNCTIO
-00001ba0: 4e53 2049 4e20 5343 4845 4d41 2070 7562  NS IN SCHEMA pub
-00001bb0: 6c69 6320 544f 2025 7322 2025 0a20 2020  lic TO %s" %.   
-00001bc0: 2020 2020 2020 2020 2020 2020 206e 6577               new
-00001bd0: 5f75 7365 722c 0a20 2020 2020 2020 2020  _user,.         
-00001be0: 2020 2022 414c 5445 5220 4445 4641 554c     "ALTER DEFAUL
-00001bf0: 5420 5052 4956 494c 4547 4553 2047 5241  T PRIVILEGES GRA
-00001c00: 4e54 2041 4c4c 204f 4e20 5441 424c 4553  NT ALL ON TABLES
-00001c10: 2054 4f20 2573 2220 2520 6e65 775f 7573   TO %s" % new_us
-00001c20: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-00001c30: 2241 4c54 4552 2044 4546 4155 4c54 2050  "ALTER DEFAULT P
-00001c40: 5249 5649 4c45 4745 5320 4752 414e 5420  RIVILEGES GRANT 
-00001c50: 414c 4c20 4f4e 2053 4551 5545 4e43 4553  ALL ON SEQUENCES
-00001c60: 2054 4f20 2573 2220 2520 6e65 775f 7573   TO %s" % new_us
-00001c70: 6572 0a20 2020 2020 2020 2020 2020 2029  er.            )
-00001c80: 3a0a 2020 2020 2020 2020 7374 7320 3d20  :.        sts = 
-00001c90: 6578 6563 5f73 716c 2863 7478 2c20 7371  exec_sql(ctx, sq
-00001ca0: 6c29 0a20 2020 2020 2020 2069 6620 7374  l).        if st
-00001cb0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-00001cc0: 6574 7572 6e20 7374 730a 2020 2020 7371  eturn sts.    sq
-00001cd0: 6c20 3d20 2273 656c 6563 7420 7461 626c  l = "select tabl
-00001ce0: 656e 616d 6520 6672 6f6d 2070 675f 7461  ename from pg_ta
-00001cf0: 626c 6573 2077 6865 7265 2073 6368 656d  bles where schem
-00001d00: 616e 616d 6520 3d20 2770 7562 6c69 6327  aname = 'public'
-00001d10: 220a 2020 2020 7265 6373 203d 2065 7865  ".    recs = exe
-00001d20: 635f 7371 6c28 6374 782c 2073 716c 2c20  c_sql(ctx, sql, 
-00001d30: 7265 7370 6f6e 7365 3d54 7275 6529 0a20  response=True). 
-00001d40: 2020 2066 6f72 2072 6563 2069 6e20 7265     for rec in re
-00001d50: 6373 3a0a 2020 2020 2020 2020 7371 6c20  cs:.        sql 
-00001d60: 3d20 2741 4c54 4552 2054 4142 4c45 2022  = 'ALTER TABLE "
-00001d70: 2573 2220 4f57 4e45 5220 544f 2025 7327  %s" OWNER TO %s'
-00001d80: 2025 2028 7265 635b 305d 2c20 6e65 775f   % (rec[0], new_
-00001d90: 7573 6572 290a 2020 2020 2020 2020 7374  user).        st
-00001da0: 7320 3d20 6578 6563 5f73 716c 2863 7478  s = exec_sql(ctx
-00001db0: 2c20 7371 6c29 0a20 2020 2020 2020 2069  , sql).        i
-00001dc0: 6620 7374 733a 0a20 2020 2020 2020 2020  f sts:.         
-00001dd0: 2020 2072 6574 7572 6e20 7374 730a 2020     return sts.  
-00001de0: 2020 2020 2020 7371 6c20 3d20 2747 5241        sql = 'GRA
-00001df0: 4e54 2041 4c4c 2050 5249 5649 4c45 4745  NT ALL PRIVILEGE
-00001e00: 5320 4f4e 2054 4142 4c45 2022 2573 2220  S ON TABLE "%s" 
-00001e10: 544f 2025 7327 2025 2028 7265 635b 305d  TO %s' % (rec[0]
-00001e20: 2c20 6e65 775f 7573 6572 290a 2020 2020  , new_user).    
-00001e30: 2020 2020 6578 6563 5f73 716c 2863 7478      exec_sql(ctx
-00001e40: 2c20 7371 6c29 0a20 2020 2020 2020 2069  , sql).        i
-00001e50: 6620 7374 733a 0a20 2020 2020 2020 2020  f sts:.         
-00001e60: 2020 2072 6574 7572 6e20 7374 730a 2020     return sts.  
-00001e70: 2020 7371 6c20 3d20 2273 656c 6563 7420    sql = "select 
-00001e80: 7365 7175 656e 6365 5f6e 616d 6520 6672  sequence_name fr
-00001e90: 6f6d 2069 6e66 6f72 6d61 7469 6f6e 5f73  om information_s
-00001ea0: 6368 656d 612e 7365 7175 656e 6365 7320  chema.sequences 
-00001eb0: 2220 5c0a 2020 2020 2020 2020 2020 2277  " \.          "w
-00001ec0: 6865 7265 2073 6571 7565 6e63 655f 7363  here sequence_sc
-00001ed0: 6865 6d61 203d 2027 7075 626c 6963 2722  hema = 'public'"
-00001ee0: 0a20 2020 2072 6563 7320 3d20 6578 6563  .    recs = exec
-00001ef0: 5f73 716c 2863 7478 2c20 7371 6c2c 2072  _sql(ctx, sql, r
-00001f00: 6573 706f 6e73 653d 5472 7565 290a 2020  esponse=True).  
-00001f10: 2020 666f 7220 7265 6320 696e 2072 6563    for rec in rec
-00001f20: 733a 0a20 2020 2020 2020 2073 716c 203d  s:.        sql =
-00001f30: 2027 414c 5445 5220 5345 5155 454e 4345   'ALTER SEQUENCE
-00001f40: 2022 2573 2220 4f57 4e45 5220 544f 2025   "%s" OWNER TO %
-00001f50: 7327 2025 2028 7265 635b 305d 2c20 6e65  s' % (rec[0], ne
-00001f60: 775f 7573 6572 290a 2020 2020 2020 2020  w_user).        
-00001f70: 6578 6563 5f73 716c 2863 7478 2c20 7371  exec_sql(ctx, sq
-00001f80: 6c29 0a20 2020 2020 2020 2069 6620 7374  l).        if st
-00001f90: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-00001fa0: 6574 7572 6e20 7374 730a 2020 2020 2020  eturn sts.      
-00001fb0: 2020 7371 6c20 3d20 2747 5241 4e54 2041    sql = 'GRANT A
-00001fc0: 4c4c 2050 5249 5649 4c45 4745 5320 4f4e  LL PRIVILEGES ON
-00001fd0: 2053 4551 5545 4e43 4520 2225 7322 2054   SEQUENCE "%s" T
-00001fe0: 4f20 2573 2720 2520 2872 6563 5b30 5d2c  O %s' % (rec[0],
-00001ff0: 206e 6577 5f75 7365 7229 0a20 2020 2020   new_user).     
-00002000: 2020 2065 7865 635f 7371 6c28 6374 782c     exec_sql(ctx,
-00002010: 2073 716c 290a 2020 2020 2020 2020 6966   sql).        if
-00002020: 2073 7473 3a0a 2020 2020 2020 2020 2020   sts:.          
-00002030: 2020 7265 7475 726e 2073 7473 0a20 2020    return sts.   
-00002040: 2073 716c 203d 2022 7365 6c65 6374 2074   sql = "select t
-00002050: 6162 6c65 5f6e 616d 6520 6672 6f6d 2069  able_name from i
-00002060: 6e66 6f72 6d61 7469 6f6e 5f73 6368 656d  nformation_schem
-00002070: 612e 7669 6577 7320 2220 5c0a 2020 2020  a.views " \.    
-00002080: 2020 2020 2020 2022 7768 6572 6520 7461         "where ta
-00002090: 626c 655f 7363 6865 6d61 203d 2027 7075  ble_schema = 'pu
-000020a0: 626c 6963 2722 0a20 2020 2072 6563 7320  blic'".    recs 
-000020b0: 3d20 6578 6563 5f73 716c 2863 7478 2c20  = exec_sql(ctx, 
-000020c0: 7371 6c2c 2072 6573 706f 6e73 653d 5472  sql, response=Tr
-000020d0: 7565 290a 2020 2020 666f 7220 7265 6320  ue).    for rec 
-000020e0: 696e 2072 6563 733a 0a20 2020 2020 2020  in recs:.       
-000020f0: 2073 716c 203d 2027 414c 5445 5220 5649   sql = 'ALTER VI
-00002100: 4557 2022 2573 2220 4f57 4e45 5220 544f  EW "%s" OWNER TO
-00002110: 2025 7327 2025 2028 7265 635b 305d 2c20   %s' % (rec[0], 
-00002120: 6e65 775f 7573 6572 290a 2020 2020 2020  new_user).      
-00002130: 2020 6578 6563 5f73 716c 2863 7478 2c20    exec_sql(ctx, 
-00002140: 7371 6c29 0a20 2020 2020 2020 2069 6620  sql).        if 
-00002150: 7374 733a 0a20 2020 2020 2020 2020 2020  sts:.           
-00002160: 2072 6574 7572 6e20 7374 730a 2020 2020   return sts.    
-00002170: 2020 2020 7371 6c20 3d20 2747 5241 4e54      sql = 'GRANT
-00002180: 2041 4c4c 2050 5249 5649 4c45 4745 5320   ALL PRIVILEGES 
-00002190: 4f4e 2054 4142 4c45 2022 2573 2220 544f  ON TABLE "%s" TO
-000021a0: 2025 7327 2025 2028 7265 635b 305d 2c20   %s' % (rec[0], 
-000021b0: 6e65 775f 7573 6572 290a 2020 2020 2020  new_user).      
-000021c0: 2020 6578 6563 5f73 716c 2863 7478 2c20    exec_sql(ctx, 
-000021d0: 7371 6c29 0a20 2020 2020 2020 2069 6620  sql).        if 
-000021e0: 7374 733a 0a20 2020 2020 2020 2020 2020  sts:.           
-000021f0: 2072 6574 7572 6e20 7374 730a 2020 2020   return sts.    
-00002200: 7371 6c20 3d20 2747 5241 4e54 2025 7320  sql = 'GRANT %s 
-00002210: 544f 2025 7327 2025 2028 6f6c 645f 7573  TO %s' % (old_us
-00002220: 6572 2c20 6e65 775f 7573 6572 290a 2020  er, new_user).  
-00002230: 2020 7265 7475 726e 2065 7865 635f 7371    return exec_sq
-00002240: 6c28 6374 782c 2073 716c 290a 0a0a 6465  l(ctx, sql)...de
-00002250: 6620 7265 6173 7369 676e 5f64 625f 6f77  f reassign_db_ow
-00002260: 6e65 7228 6374 782c 2064 626e 616d 652c  ner(ctx, dbname,
-00002270: 206f 6c64 5f75 7365 722c 206e 6577 5f75   old_user, new_u
-00002280: 7365 7229 3a0a 2020 2020 7275 6e5f 7472  ser):.    run_tr
-00002290: 6163 6564 2827 7067 5f64 625f 6163 7469  aced('pg_db_acti
-000022a0: 7665 272c 2027 2d77 6127 2c20 2725 7327  ve', '-wa', '%s'
-000022b0: 2025 2074 6774 5f63 7478 5b27 6462 5f6e   % tgt_ctx['db_n
-000022c0: 616d 6527 5d29 0a20 2020 2073 7473 203d  ame']).    sts =
-000022d0: 2070 795f 7265 6173 7369 676e 5f64 625f   py_reassign_db_
-000022e0: 6f77 6e65 7228 7467 745f 6374 782c 0a20  owner(tgt_ctx,. 
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002300: 2020 2020 2020 2020 2020 2020 2020 7467                tg
-00002310: 745f 6374 785b 2764 625f 6e61 6d65 275d  t_ctx['db_name']
-00002320: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002340: 2073 7263 5f63 7478 5b27 6462 5f75 7365   src_ctx['db_use
-00002350: 7227 5d2c 0a20 2020 2020 2020 2020 2020  r'],.           
-00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002370: 2020 2020 7467 745f 6374 785b 2764 625f      tgt_ctx['db_
-00002380: 7573 6572 275d 290a 2020 2020 6966 2073  user']).    if s
-00002390: 7473 3a0a 2020 2020 2020 2020 7275 6e5f  ts:.        run_
-000023a0: 7472 6163 6564 2827 7067 5f64 625f 7265  traced('pg_db_re
-000023b0: 6173 7369 676e 5f6f 776e 6572 272c 0a20  assign_owner',. 
-000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023d0: 2020 272d 6427 2c20 7467 745f 6374 785b    '-d', tgt_ctx[
-000023e0: 2764 625f 6e61 6d65 275d 2c0a 2020 2020  'db_name'],.    
-000023f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00002400: 2d6f 272c 2073 7263 5f63 7478 5b27 6462  -o', src_ctx['db
-00002410: 5f75 7365 7227 5d2c 0a20 2020 2020 2020  _user'],.       
-00002420: 2020 2020 2020 2020 2020 2020 272d 5527              '-U'
-00002430: 2c20 7467 745f 6374 785b 2764 625f 7573  , tgt_ctx['db_us
-00002440: 6572 275d 290a 0a64 6566 2064 726f 705f  er'])..def drop_
-00002450: 7365 7373 696f 6e28 6374 782c 2064 626e  session(ctx, dbn
-00002460: 616d 652c 2064 6174 6164 6972 3d4e 6f6e  ame, datadir=Non
-00002470: 652c 206f 646f 6f5f 7669 643d 4e6f 6e65  e, odoo_vid=None
-00002480: 293a 0a20 2020 2069 6620 6e6f 7420 6f64  ):.    if not od
-00002490: 6f6f 5f76 6964 3a0a 2020 2020 2020 2020  oo_vid:.        
-000024a0: 6f64 6f6f 5f76 6964 203d 2063 7478 2e67  odoo_vid = ctx.g
-000024b0: 6574 2827 7467 745f 7669 6427 290a 2020  et('tgt_vid').  
-000024c0: 2020 6966 206e 6f74 206f 646f 6f5f 7669    if not odoo_vi
-000024d0: 643a 0a20 2020 2020 2020 206f 646f 6f5f  d:.        odoo_
-000024e0: 7669 6420 3d20 6374 782e 6765 7428 2773  vid = ctx.get('s
-000024f0: 7263 5f76 6964 2729 0a20 2020 2069 6620  rc_vid').    if 
-00002500: 6e6f 7420 6461 7461 6469 723a 0a20 2020  not datadir:.   
-00002510: 2020 2020 2064 6174 6164 6972 203d 2063       datadir = c
-00002520: 7478 2e67 6574 2827 6461 7461 5f64 6972  tx.get('data_dir
-00002530: 2729 0a20 2020 2069 6620 6e6f 7420 6461  ').    if not da
-00002540: 7461 6469 723a 0a20 2020 2020 2020 2064  tadir:.        d
-00002550: 6174 6164 6972 203d 2063 6c6f 646f 6f2e  atadir = clodoo.
-00002560: 6275 696c 645f 6f64 6f6f 5f70 6172 616d  build_odoo_param
-00002570: 280a 2020 2020 2020 2020 2020 2020 2744  (.            'D
-00002580: 4449 5227 2c20 6f64 6f6f 5f76 6964 3d6f  DIR', odoo_vid=o
-00002590: 646f 6f5f 7669 642c 206d 756c 7469 3d54  doo_vid, multi=T
-000025a0: 7275 6529 0a20 2020 206f 646f 6f5f 7665  rue).    odoo_ve
-000025b0: 7220 3d20 636c 6f64 6f6f 2e62 7569 6c64  r = clodoo.build
-000025c0: 5f6f 646f 6f5f 7061 7261 6d28 0a20 2020  _odoo_param(.   
-000025d0: 2020 2020 2027 4d41 4a56 4552 272c 206f       'MAJVER', o
-000025e0: 646f 6f5f 7669 643d 6f64 6f6f 5f76 6964  doo_vid=odoo_vid
-000025f0: 2c20 6d75 6c74 693d 5472 7565 290a 2020  , multi=True).  
-00002600: 2020 6966 206f 646f 6f5f 7665 7220 3c20    if odoo_ver < 
-00002610: 383a 0a20 2020 2020 2020 206f 732e 7379  8:.        os.sy
-00002620: 7374 656d 2827 2727 666f 7220 6620 696e  stem('''for f in
-00002630: 2024 2867 7265 7020 2d6c 2022 2573 2220   $(grep -l "%s" 
-00002640: 2f74 6d70 2f6f 652d 7365 7373 696f 6e73  /tmp/oe-sessions
-00002650: 2d6f 646f 6f2f 2a29 3b20 646f 0a20 2020  -odoo/*); do.   
-00002660: 2020 2020 2072 6d20 2d66 2024 663b 2064       rm -f $f; d
-00002670: 6f6e 6527 2727 2025 2028 6462 6e61 6d65  one''' % (dbname
-00002680: 2929 0a20 2020 2065 6c73 653a 0a20 2020  )).    else:.   
-00002690: 2020 2020 206f 732e 7379 7374 656d 2827       os.system('
-000026a0: 2727 666f 7220 6620 696e 2024 2867 7265  ''for f in $(gre
-000026b0: 7020 2d6c 2022 2573 2220 2573 2f73 6573  p -l "%s" %s/ses
-000026c0: 7369 6f6e 732f 2a29 3b20 646f 0a20 2020  sions/*); do.   
-000026d0: 2020 2020 2072 6d20 2d66 2024 663b 2064       rm -f $f; d
-000026e0: 6f6e 6527 2727 2025 2028 6462 6e61 6d65  one''' % (dbname
-000026f0: 2c20 6461 7461 6469 7229 290a 0a0a 6465  , datadir))...de
-00002700: 6620 6765 745f 6361 6368 6528 6374 7829  f get_cache(ctx)
-00002710: 3a0a 2020 2020 6374 785b 275f 4341 4348  :.    ctx['_CACH
-00002720: 4527 5d20 3d20 6374 782e 6765 7428 275f  E'] = ctx.get('_
-00002730: 4341 4348 4527 2c20 7b7d 290a 2020 2020  CACHE', {}).    
-00002740: 7265 7475 726e 2063 7478 5b27 5f43 4143  return ctx['_CAC
-00002750: 4845 275d 0a0a 0a64 6566 2063 6163 6865  HE']...def cache
-00002760: 5f69 735f 656e 7472 7928 6361 6368 652c  _is_entry(cache,
-00002770: 206d 6f64 656c 2c20 6964 293a 0a20 2020   model, id):.   
-00002780: 2063 6163 6865 5b6d 6f64 656c 5d20 3d20   cache[model] = 
-00002790: 6361 6368 652e 6765 7428 6d6f 6465 6c2c  cache.get(model,
-000027a0: 207b 7d29 0a20 2020 2072 6574 7572 6e20   {}).    return 
-000027b0: 2869 6420 696e 2063 6163 6865 5b6d 6f64  (id in cache[mod
-000027c0: 656c 5d29 0a0a 0a64 6566 2063 6163 6865  el])...def cache
-000027d0: 5f67 6574 5f65 6e74 7279 2863 6163 6865  _get_entry(cache
-000027e0: 2c20 6d6f 6465 6c2c 2069 6429 3a0a 2020  , model, id):.  
-000027f0: 2020 6361 6368 655b 6d6f 6465 6c5d 203d    cache[model] =
-00002800: 2063 6163 6865 2e67 6574 286d 6f64 656c   cache.get(model
-00002810: 2c20 7b7d 290a 2020 2020 7265 7475 726e  , {}).    return
-00002820: 2063 6163 6865 5b6d 6f64 656c 5d2e 6765   cache[model].ge
-00002830: 7428 2769 6427 2c20 4661 6c73 6529 0a0a  t('id', False)..
-00002840: 0a64 6566 2063 6163 6865 5f73 746f 7265  .def cache_store
-00002850: 5f65 6e74 7279 2863 6163 6865 2c20 6d6f  _entry(cache, mo
-00002860: 6465 6c2c 2069 642c 206b 6565 703d 4e6f  del, id, keep=No
-00002870: 6e65 293a 0a20 2020 2063 6163 6865 5b6d  ne):.    cache[m
-00002880: 6f64 656c 5d20 3d20 6361 6368 652e 6765  odel] = cache.ge
-00002890: 7428 6d6f 6465 6c2c 207b 7d29 0a20 2020  t(model, {}).   
-000028a0: 2069 6620 6964 206f 7220 6b65 6570 3a0a   if id or keep:.
-000028b0: 2020 2020 2020 2020 6361 6368 655b 6d6f          cache[mo
-000028c0: 6465 6c5d 5b27 6964 275d 203d 2069 640a  del]['id'] = id.
-000028d0: 2020 2020 656c 6966 2069 6420 696e 2063      elif id in c
-000028e0: 6163 6865 5b6d 6f64 656c 5d3a 0a20 2020  ache[model]:.   
-000028f0: 2020 2020 2064 656c 2063 6163 6865 5b6d       del cache[m
-00002900: 6f64 656c 5d5b 2769 6427 5d0a 2020 2020  odel]['id'].    
-00002910: 7265 7475 726e 2063 6163 6865 5b6d 6f64  return cache[mod
-00002920: 656c 5d0a 0a0a 6465 6620 7365 745f 746d  el]...def set_tm
-00002930: 705f 6b65 7973 2863 7478 2c20 6d6f 6465  p_keys(ctx, mode
-00002940: 6c2c 2069 642c 2076 616c 7329 3a0a 2020  l, id, vals):.  
-00002950: 2020 7472 795f 6167 6169 6e20 3d20 4661    try_again = Fa
-00002960: 6c73 650a 2020 2020 6966 2027 636f 6465  lse.    if 'code
-00002970: 2720 696e 2076 616c 733a 0a20 2020 2020  ' in vals:.     
-00002980: 2020 2076 616c 735b 2763 6f64 6527 5d20     vals['code'] 
-00002990: 3d20 7374 7228 6964 290a 2020 2020 2020  = str(id).      
-000029a0: 2020 7472 795f 6167 6169 6e20 3d20 5472    try_again = Tr
-000029b0: 7565 0a20 2020 2069 6620 276e 616d 6527  ue.    if 'name'
-000029c0: 2069 6e20 7661 6c73 3a0a 2020 2020 2020   in vals:.      
-000029d0: 2020 7661 6c73 5b27 6e61 6d65 275d 203d    vals['name'] =
-000029e0: 2027 4944 3d25 6420 2573 2720 2520 2869   'ID=%d %s' % (i
-000029f0: 642c 2076 616c 735b 276e 616d 6527 5d29  d, vals['name'])
-00002a00: 0a20 2020 2020 2020 2074 7279 5f61 6761  .        try_aga
-00002a10: 696e 203d 2054 7275 650a 2020 2020 7265  in = True.    re
-00002a20: 7475 726e 2074 7279 5f61 6761 696e 2c20  turn try_again, 
-00002a30: 7661 6c73 0a0a 0a64 6566 2072 756e 5f74  vals...def run_t
-00002a40: 7261 6365 6428 2a61 7267 7329 3a0a 2020  raced(*args):.  
-00002a50: 2020 6f73 302e 776c 6f67 2827 3e3e 3e20    os0.wlog('>>> 
-00002a60: 2573 2720 2520 2720 272e 6a6f 696e 2861  %s' % ' '.join(a
-00002a70: 7267 7329 290a 2020 2020 7265 7475 726e  rgs)).    return
-00002a80: 2050 6f70 656e 2861 7267 7329 2e77 6169   Popen(args).wai
-00002a90: 7428 290a 0a0a 6465 6620 7365 6428 2a61  t()...def sed(*a
-00002aa0: 7267 7329 3a0a 2020 2020 6669 6c65 6e61  rgs):.    filena
-00002ab0: 6d65 203d 2061 7267 735b 305d 0a20 2020  me = args[0].   
-00002ac0: 2077 6974 6820 6f70 656e 2866 696c 656e   with open(filen
-00002ad0: 616d 652c 2027 7227 2920 6173 2066 643a  ame, 'r') as fd:
-00002ae0: 0a20 2020 2020 2020 206c 696e 6573 203d  .        lines =
-00002af0: 2066 642e 7265 6164 2829 2e73 706c 6974   fd.read().split
-00002b00: 2827 5c6e 2729 0a20 2020 2066 6f72 2061  ('\n').    for a
-00002b10: 7267 2069 6e20 6172 6773 5b31 3a5d 3a0a  rg in args[1:]:.
-00002b20: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00002b30: 7369 6e73 7461 6e63 6528 6172 672c 2028  sinstance(arg, (
-00002b40: 7475 706c 652c 206c 6973 7429 293a 0a20  tuple, list)):. 
-00002b50: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00002b60: 204b 6579 4572 726f 7228 2749 6e76 616c   KeyError('Inval
-00002b70: 6964 2070 6172 616d 6574 6573 2729 0a20  id parametes'). 
-00002b80: 2020 2020 2020 2066 6f72 206c 696e 656e         for linen
-00002b90: 6f20 696e 2072 616e 6765 286c 656e 286c  o in range(len(l
-00002ba0: 696e 6573 2929 3a0a 2020 2020 2020 2020  ines)):.        
-00002bb0: 2020 2020 6c69 6e65 735b 6c69 6e65 6e6f      lines[lineno
-00002bc0: 5d20 3d20 7265 2e73 7562 2861 7267 5b30  ] = re.sub(arg[0
-00002bd0: 5d2c 2061 7267 5b31 5d2c 206c 696e 6573  ], arg[1], lines
-00002be0: 5b6c 696e 656e 6f5d 290a 2020 2020 7769  [lineno]).    wi
-00002bf0: 7468 206f 7065 6e28 6669 6c65 6e61 6d65  th open(filename
-00002c00: 2c20 2777 2729 2061 7320 6664 3a0a 2020  , 'w') as fd:.  
-00002c10: 2020 2020 2020 6664 2e77 7269 7465 285f        fd.write(_
-00002c20: 6228 275c 6e27 2e6a 6f69 6e28 6c69 6e65  b('\n'.join(line
-00002c30: 7329 2929 0a0a 0a64 6566 2073 6564 5f61  s)))...def sed_a
-00002c40: 7070 656e 6428 2a61 7267 7329 3a0a 2020  ppend(*args):.  
-00002c50: 2020 6669 6c65 6e61 6d65 203d 2061 7267    filename = arg
-00002c60: 735b 305d 0a20 2020 2077 6974 6820 6f70  s[0].    with op
-00002c70: 656e 2866 696c 656e 616d 652c 2027 7227  en(filename, 'r'
-00002c80: 2920 6173 2066 643a 0a20 2020 2020 2020  ) as fd:.       
-00002c90: 206c 696e 6573 203d 2066 642e 7265 6164   lines = fd.read
-00002ca0: 2829 2e73 706c 6974 2827 5c6e 2729 0a20  ().split('\n'). 
-00002cb0: 2020 2066 6f72 2061 7267 2069 6e20 6172     for arg in ar
-00002cc0: 6773 5b31 3a5d 3a0a 2020 2020 2020 2020  gs[1:]:.        
-00002cd0: 6c69 6e65 732e 6170 7065 6e64 2861 7267  lines.append(arg
-00002ce0: 290a 2020 2020 7769 7468 206f 7065 6e28  ).    with open(
-00002cf0: 6669 6c65 6e61 6d65 2c20 2777 2729 2061  filename, 'w') a
-00002d00: 7320 6664 3a0a 2020 2020 2020 2020 6664  s fd:.        fd
-00002d10: 2e77 7269 7465 285f 6228 275c 6e27 2e6a  .write(_b('\n'.j
-00002d20: 6f69 6e28 6c69 6e65 7329 2929 0a0a 0a64  oin(lines)))...d
-00002d30: 6566 2063 6f6e 6669 675f 6765 745f 6c69  ef config_get_li
-00002d40: 7374 2863 6f6e 6669 672c 2069 7465 6d29  st(config, item)
-00002d50: 3a0a 2020 2020 7265 7475 726e 2063 6f6e  :.    return con
-00002d60: 6669 672e 6765 7428 276f 7074 696f 6e73  fig.get('options
-00002d70: 272c 2069 7465 6d29 2e73 7472 6970 2829  ', item).strip()
-00002d80: 2e73 706c 6974 2827 2c27 290a 0a0a 6465  .split(',')...de
-00002d90: 6620 7275 6e5f 6f64 6f6f 5f61 6c6c 7465  f run_odoo_allte
-00002da0: 7374 286f 646f 6f5f 7669 642c 2063 6f6e  st(odoo_vid, con
-00002db0: 666e 2c20 6462 5f6e 616d 652c 206c 6f67  fn, db_name, log
-00002dc0: 6669 6c65 2c20 6d6f 6475 6c65 733d 4e6f  file, modules=No
-00002dd0: 6e65 293a 0a20 2020 2069 6620 6d6f 6475  ne):.    if modu
-00002de0: 6c65 733a 0a20 2020 2020 2020 206d 6f64  les:.        mod
-00002df0: 756c 6573 203d 2027 2c27 2e6a 6f69 6e28  ules = ','.join(
-00002e00: 6d6f 6475 6c65 7329 0a20 2020 2065 6c73  modules).    els
-00002e10: 653a 0a20 2020 2020 2020 206d 6f64 756c  e:.        modul
-00002e20: 6573 203d 2027 616c 6c27 0a20 2020 2073  es = 'all'.    s
-00002e30: 7263 5f6f 646f 6f5f 6269 6e20 3d20 636c  rc_odoo_bin = cl
-00002e40: 6f64 6f6f 2e62 7569 6c64 5f6f 646f 6f5f  odoo.build_odoo_
-00002e50: 7061 7261 6d28 0a20 2020 2020 2020 2020  param(.         
-00002e60: 2020 2027 4249 4e27 2c20 6f64 6f6f 5f76     'BIN', odoo_v
-00002e70: 6964 3d6f 646f 6f5f 7669 642c 206d 756c  id=odoo_vid, mul
-00002e80: 7469 3d54 7275 6529 0a20 2020 2072 756e  ti=True).    run
-00002e90: 5f74 7261 6365 6428 7372 635f 6f64 6f6f  _traced(src_odoo
-00002ea0: 5f62 696e 2c0a 2020 2020 2020 2020 2020  _bin,.          
-00002eb0: 2020 2020 2027 2d63 272c 2063 6f6e 666e       '-c', confn
-00002ec0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002ed0: 2027 2d64 272c 2064 625f 6e61 6d65 2c0a   '-d', db_name,.
-00002ee0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00002ef0: 2d75 272c 206d 6f64 756c 6573 2c0a 2020  -u', modules,.  
-00002f00: 2020 2020 2020 2020 2020 2020 2027 2d2d               '--
-00002f10: 7374 6f70 2d61 6674 6572 2d69 6e69 7427  stop-after-init'
-00002f20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002f30: 2027 2d2d 6e6f 2d78 6d6c 7270 6327 2c0a   '--no-xmlrpc',.
-00002f40: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00002f50: 2d2d 6c6f 6766 696c 653d 2573 2720 2520  --logfile=%s' % 
-00002f60: 6c6f 6766 696c 6529 0a0a 0a64 6566 2064  logfile)...def d
-00002f70: 625f 6578 6973 7428 6374 782c 2064 626e  b_exist(ctx, dbn
-00002f80: 616d 6529 3a0a 2020 2020 7365 7373 696f  ame):.    sessio
-00002f90: 6e20 3d20 636c 6f64 6f6f 2e63 6f6e 6e65  n = clodoo.conne
-00002fa0: 6374 4c38 2863 7478 290a 2020 2020 6966  ctL8(ctx).    if
-00002fb0: 2069 7369 6e73 7461 6e63 6528 7365 7373   isinstance(sess
-00002fc0: 696f 6e2c 2062 6173 6573 7472 696e 6729  ion, basestring)
-00002fd0: 3a0a 2020 2020 2020 2020 6f73 302e 776c  :.        os0.wl
-00002fe0: 6f67 2827 436f 6e6e 6563 7469 6f6e 2065  og('Connection e
-00002ff0: 7272 6f72 2025 7327 2025 2073 6573 7369  rror %s' % sessi
-00003000: 6f6e 290a 2020 2020 2020 2020 7261 6973  on).        rais
-00003010: 6520 494f 4572 726f 7228 7365 7373 696f  e IOError(sessio
-00003020: 6e29 0a20 2020 2069 6620 6462 6e61 6d65  n).    if dbname
-00003030: 2069 6e20 6374 785b 276f 646f 6f5f 7365   in ctx['odoo_se
-00003040: 7373 696f 6e27 5d2e 6462 2e6c 6973 7428  ssion'].db.list(
-00003050: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00003060: 6e20 5472 7565 0a20 2020 2072 6574 7572  n True.    retur
-00003070: 6e20 4661 6c73 650a 0a0a 6465 6620 7765  n False...def we
-00003080: 705f 6c6f 6773 2863 7478 293a 0a20 2020  p_logs(ctx):.   
-00003090: 2069 6620 6f73 2e70 6174 682e 6973 6469   if os.path.isdi
-000030a0: 7228 6374 785b 276f 7074 5f6f 756c 7061  r(ctx['opt_oulpa
-000030b0: 7468 275d 293a 0a20 2020 2020 2020 2073  th']):.        s
-000030c0: 6875 7469 6c2e 726d 7472 6565 2863 7478  hutil.rmtree(ctx
-000030d0: 5b27 6f70 745f 6f75 6c70 6174 6827 5d29  ['opt_oulpath'])
-000030e0: 0a20 2020 2066 6f72 2076 6572 2069 6e20  .    for ver in 
-000030f0: 5645 5253 494f 4e53 3a0a 2020 2020 2020  VERSIONS:.      
-00003100: 2020 746d 705f 6469 7220 3d20 6f73 2e70    tmp_dir = os.p
-00003110: 6174 682e 6a6f 696e 2863 7478 5b27 6f70  ath.join(ctx['op
-00003120: 745f 6f75 7061 7468 275d 2c20 276f 755f  t_oupath'], 'ou_
-00003130: 2573 2720 2520 7665 7229 0a20 2020 2020  %s' % ver).     
-00003140: 2020 2069 6620 6f73 2e70 6174 682e 6973     if os.path.is
-00003150: 6469 7228 746d 705f 6469 7229 3a0a 2020  dir(tmp_dir):.  
-00003160: 2020 2020 2020 2020 2020 7368 7574 696c            shutil
-00003170: 2e72 6d74 7265 6528 746d 705f 6469 7229  .rmtree(tmp_dir)
-00003180: 0a20 2020 2074 6d70 5f64 6972 203d 206f  .    tmp_dir = o
-00003190: 732e 7061 7468 2e6a 6f69 6e28 6374 785b  s.path.join(ctx[
-000031a0: 276f 7074 5f6f 7570 6174 6827 5d2c 2027  'opt_oupath'], '
-000031b0: 6f70 656e 7570 6772 6164 6527 290a 2020  openupgrade').  
-000031c0: 2020 6966 206f 732e 7061 7468 2e69 7364    if os.path.isd
-000031d0: 6972 2874 6d70 5f64 6972 293a 0a20 2020  ir(tmp_dir):.   
-000031e0: 2020 2020 2073 6875 7469 6c2e 726d 7472       shutil.rmtr
-000031f0: 6565 2874 6d70 5f64 6972 290a 2020 2020  ee(tmp_dir).    
-00003200: 666c 6f67 5f64 6972 203d 2020 6f73 2e70  flog_dir =  os.p
-00003210: 6174 682e 6469 726e 616d 6528 6374 785b  ath.dirname(ctx[
-00003220: 276c 6f67 666e 275d 290a 2020 2020 6966  'logfn']).    if
-00003230: 206e 6f74 206f 732e 7061 7468 2e69 7364   not os.path.isd
-00003240: 6972 2866 6c6f 675f 6469 7229 3a0a 2020  ir(flog_dir):.  
-00003250: 2020 2020 2020 6f73 2e6d 6b64 6972 2866        os.mkdir(f
-00003260: 6c6f 675f 6469 7229 0a20 2020 2069 6620  log_dir).    if 
-00003270: 6f73 2e70 6174 682e 6973 6669 6c65 2863  os.path.isfile(c
-00003280: 7478 5b27 6c6f 6766 6e27 5d29 3a0a 2020  tx['logfn']):.  
-00003290: 2020 2020 2020 6f73 2e72 656d 6f76 6528        os.remove(
-000032a0: 6374 785b 276c 6f67 666e 275d 290a 2020  ctx['logfn']).  
-000032b0: 2020 6966 206f 732e 7061 7468 2e69 7366    if os.path.isf
-000032c0: 696c 6528 6374 785b 276c 6f67 6669 6c65  ile(ctx['logfile
-000032d0: 275d 293a 0a20 2020 2020 2020 206f 732e  ']):.        os.
-000032e0: 7265 6d6f 7665 2863 7478 5b27 6c6f 6766  remove(ctx['logf
-000032f0: 696c 6527 5d29 0a20 2020 2069 6620 6374  ile']).    if ct
-00003300: 785b 276f 6361 5f6d 6967 7261 7465 275d  x['oca_migrate']
-00003310: 3a0a 2020 2020 2020 2020 6966 206f 732e  :.        if os.
-00003320: 7061 7468 2e69 7364 6972 286f 732e 7061  path.isdir(os.pa
-00003330: 7468 2e6a 6f69 6e28 6f73 2e70 6174 682e  th.join(os.path.
-00003340: 6578 7061 6e64 7573 6572 2827 7e27 292c  expanduser('~'),
-00003350: 2027 6f70 656e 7570 6772 6164 6527 2929   'openupgrade'))
-00003360: 3a0a 2020 2020 2020 2020 2020 2020 7368  :.            sh
-00003370: 7574 696c 2e72 6d74 7265 6528 6f73 2e70  util.rmtree(os.p
-00003380: 6174 682e 6a6f 696e 286f 732e 7061 7468  ath.join(os.path
-00003390: 2e65 7870 616e 6475 7365 7228 277e 2729  .expanduser('~')
-000033a0: 2c20 276f 7065 6e75 7067 7261 6465 2729  , 'openupgrade')
-000033b0: 290a 0a0a 6465 6620 6472 6f70 5f64 6228  )...def drop_db(
-000033c0: 7372 635f 6374 782c 2074 6774 5f63 7478  src_ctx, tgt_ctx
-000033d0: 2c20 6462 6e61 6d65 2c20 6462 6e61 6d65  , dbname, dbname
-000033e0: 3229 3a0a 2020 2020 666f 7220 6462 2069  2):.    for db i
-000033f0: 6e20 2864 626e 616d 652c 2064 626e 616d  n (dbname, dbnam
-00003400: 6532 293a 0a20 2020 2020 2020 2063 6d64  e2):.        cmd
-00003410: 203d 2027 7067 5f64 625f 6163 7469 7665   = 'pg_db_active
-00003420: 202d 7761 2025 737c 6472 6f70 6462 202d   -wa %s|dropdb -
-00003430: 5525 7320 2573 2720 2520 280a 2020 2020  U%s %s' % (.    
-00003440: 2020 2020 2020 2020 6462 2c20 7467 745f          db, tgt_
-00003450: 6374 785b 2764 625f 7573 6572 275d 2c20  ctx['db_user'], 
-00003460: 6462 290a 2020 2020 2020 2020 6f73 2e73  db).        os.s
-00003470: 7973 7465 6d28 636d 6429 0a20 2020 2020  ystem(cmd).     
-00003480: 2020 2063 6d64 203d 2027 7067 5f64 625f     cmd = 'pg_db_
-00003490: 6163 7469 7665 202d 7761 2025 737c 6472  active -wa %s|dr
-000034a0: 6f70 6462 202d 5525 7320 2573 2720 2520  opdb -U%s %s' % 
-000034b0: 280a 2020 2020 2020 2020 2020 2020 6462  (.            db
-000034c0: 2c20 7372 635f 6374 785b 2764 625f 7573  , src_ctx['db_us
-000034d0: 6572 275d 2c20 6462 290a 2020 2020 2020  er'], db).      
-000034e0: 2020 6f73 2e73 7973 7465 6d28 636d 6429    os.system(cmd)
-000034f0: 0a0a 0a64 6566 2073 6574 5f75 6e69 6e73  ...def set_unins
-00003500: 7461 6c6c 6564 5f62 795f 7371 6c28 7467  talled_by_sql(tg
-00003510: 745f 6374 782c 2062 6164 5f6d 6f64 756c  t_ctx, bad_modul
-00003520: 655f 6c69 7374 293a 0a20 2020 206f 7330  e_list):.    os0
-00003530: 2e77 6c6f 6728 2773 6574 5f75 6e69 6e73  .wlog('set_unins
-00003540: 7461 6c6c 6564 5f62 795f 7371 6c25 7327  talled_by_sql%s'
-00003550: 2025 2062 6164 5f6d 6f64 756c 655f 6c69   % bad_module_li
-00003560: 7374 290a 2020 2020 7175 6572 7920 3d20  st).    query = 
-00003570: 2275 7064 6174 6520 6972 5f6d 6f64 756c  "update ir_modul
-00003580: 655f 6d6f 6475 6c65 2073 6574 2073 7461  e_module set sta
-00003590: 7465 3d27 756e 696e 7374 616c 6c65 6427  te='uninstalled'
-000035a0: 2220 5c0a 2020 2020 2020 2020 2020 2020  " \.            
-000035b0: 2220 7768 6572 6520 6e61 6d65 2069 6e20  " where name in 
-000035c0: 2825 7329 2061 6e64 2073 7461 7465 3c3e  (%s) and state<>
-000035d0: 2769 6e73 7461 6c6c 6564 273b 2220 2520  'installed';" % 
-000035e0: 7374 7228 0a20 2020 2020 2020 2020 2020  str(.           
-000035f0: 2020 2020 2062 6164 5f6d 6f64 756c 655f       bad_module_
-00003600: 6c69 7374 295b 313a 2d31 5d0a 2020 2020  list)[1:-1].    
-00003610: 6578 6563 5f73 716c 2874 6774 5f63 7478  exec_sql(tgt_ctx
-00003620: 2c20 7175 6572 7929 0a0a 0a64 6566 2073  , query)...def s
-00003630: 6574 5f69 6e73 7461 6c6c 6564 5f62 795f  et_installed_by_
-00003640: 7371 6c28 7467 745f 6374 782c 2062 6164  sql(tgt_ctx, bad
-00003650: 5f6d 6f64 756c 655f 6c69 7374 293a 0a20  _module_list):. 
-00003660: 2020 206f 7330 2e77 6c6f 6728 2773 6574     os0.wlog('set
-00003670: 5f69 6e73 7461 6c6c 6564 5f62 795f 7371  _installed_by_sq
-00003680: 6c25 7327 2025 2062 6164 5f6d 6f64 756c  l%s' % bad_modul
-00003690: 655f 6c69 7374 290a 2020 2020 7175 6572  e_list).    quer
-000036a0: 7920 3d20 2275 7064 6174 6520 6972 5f6d  y = "update ir_m
-000036b0: 6f64 756c 655f 6d6f 6475 6c65 2073 6574  odule_module set
-000036c0: 2073 7461 7465 3d27 696e 7374 616c 6c65   state='installe
-000036d0: 6427 2220 5c0a 2020 2020 2020 2020 2020  d'" \.          
-000036e0: 2020 2220 7768 6572 6520 6e61 6d65 2069    " where name i
-000036f0: 6e20 2825 7329 3b22 2025 2073 7472 2862  n (%s);" % str(b
-00003700: 6164 5f6d 6f64 756c 655f 6c69 7374 295b  ad_module_list)[
-00003710: 313a 2d31 5d0a 2020 2020 6578 6563 5f73  1:-1].    exec_s
-00003720: 716c 2874 6774 5f63 7478 2c20 7175 6572  ql(tgt_ctx, quer
-00003730: 7929 0a0a 0a64 6566 2072 656e 5f64 6228  y)...def ren_db(
-00003740: 6f6c 645f 6462 6e61 6d65 2c20 6e65 775f  old_dbname, new_
-00003750: 6462 6e61 6d65 2c20 6462 5f75 7365 7229  dbname, db_user)
-00003760: 3a0a 2020 2020 636d 6420 3d20 2770 675f  :.    cmd = 'pg_
-00003770: 6462 5f61 6374 6976 6520 2d77 6120 2573  db_active -wa %s
-00003780: 7c27 205c 0a20 2020 2020 2020 2020 2027  |' \.          '
-00003790: 7073 716c 202d 5525 7320 2d63 2022 414c  psql -U%s -c "AL
-000037a0: 5445 5220 4441 5441 4241 5345 2025 7320  TER DATABASE %s 
-000037b0: 5245 4e41 4d45 2054 4f20 2573 3b22 2074  RENAME TO %s;" t
-000037c0: 656d 706c 6174 6531 2720 2520 280a 2020  emplate1' % (.  
-000037d0: 2020 2020 2020 2020 2020 2020 6f6c 645f              old_
-000037e0: 6462 6e61 6d65 2c20 6462 5f75 7365 722c  dbname, db_user,
-000037f0: 206f 6c64 5f64 626e 616d 652c 206e 6577   old_dbname, new
-00003800: 5f64 626e 616d 6529 0a20 2020 206f 732e  _dbname).    os.
-00003810: 7379 7374 656d 2863 6d64 290a 0a0a 6465  system(cmd)...de
-00003820: 6620 6e65 775f 6462 6e61 6d65 2864 622c  f new_dbname(db,
-00003830: 206f 646f 6f5f 7665 722c 206f 6361 5f6d   odoo_ver, oca_m
-00003840: 6967 7261 7465 6429 3a0a 2020 2020 6966  igrated):.    if
-00003850: 206f 6361 5f6d 6967 7261 7465 643a 0a20   oca_migrated:. 
-00003860: 2020 2020 2020 2072 6574 7572 6e20 2725         return '%
-00003870: 735f 6d69 6772 6174 6564 2720 2520 6462  s_migrated' % db
-00003880: 0a20 2020 2070 7269 6f72 203d 206f 646f  .    prior = odo
-00003890: 6f5f 7665 7220 2d20 310a 2020 2020 6966  o_ver - 1.    if
-000038a0: 2064 622e 656e 6473 7769 7468 2873 7472   db.endswith(str
-000038b0: 2870 7269 6f72 2929 3a0a 2020 2020 2020  (prior)):.      
-000038c0: 2020 7265 7475 726e 2027 2573 5f25 6427    return '%s_%d'
-000038d0: 2025 2028 6462 5b30 3a20 2d6c 656e 2873   % (db[0: -len(s
-000038e0: 7472 2870 7269 6f72 2929 5d2c 206f 646f  tr(prior))], odo
-000038f0: 6f5f 7665 7229 0a20 2020 2072 6574 7572  o_ver).    retur
-00003900: 6e20 2725 735f 2564 2720 2520 2864 622c  n '%s_%d' % (db,
-00003910: 206f 646f 6f5f 7665 7229 0a0a 0a64 6566   odoo_ver)...def
-00003920: 2064 726f 705f 6d6f 6475 6c65 2863 7478   drop_module(ctx
-00003930: 2c20 6d6f 6475 6c65 2c20 666f 7263 653d  , module, force=
-00003940: 4e6f 6e65 293a 0a20 2020 2069 6620 666f  None):.    if fo
-00003950: 7263 653a 0a20 2020 2020 2020 206f 7330  rce:.        os0
-00003960: 2e77 6c6f 6728 273e 3e3e 2075 6e69 6e73  .wlog('>>> unins
-00003970: 7461 6c6c 2025 7327 2025 206d 6f64 756c  tall %s' % modul
-00003980: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
-00003990: 6e20 636c 6f64 6f6f 2e61 6374 5f75 6e69  n clodoo.act_uni
-000039a0: 6e73 7461 6c6c 5f6d 6f64 756c 6573 2863  nstall_modules(c
-000039b0: 7478 2c20 6d6f 6475 6c65 5f6c 6973 743d  tx, module_list=
-000039c0: 5b6d 6f64 756c 655d 290a 2020 2020 656c  [module]).    el
-000039d0: 7365 3a0a 2020 2020 2020 2020 6d6f 6475  se:.        modu
-000039e0: 6c65 5f69 6420 3d20 636c 6f64 6f6f 2e73  le_id = clodoo.s
-000039f0: 6561 7263 684c 3828 6374 782c 2027 6972  earchL8(ctx, 'ir
-00003a00: 2e6d 6f64 756c 652e 6d6f 6475 6c65 272c  .module.module',
-00003a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a30: 2020 2020 205b 2827 6e61 6d65 272c 2027       [('name', '
-00003a40: 3d27 2c20 6d6f 6475 6c65 295d 290a 2020  =', module)]).  
-00003a50: 2020 2020 2020 6964 7320 3d20 636c 6f64        ids = clod
-00003a60: 6f6f 2e73 6561 7263 684c 3828 6374 782c  oo.searchL8(ctx,
-00003a70: 2027 6972 2e6d 6f64 756c 652e 6d6f 6475   'ir.module.modu
-00003a80: 6c65 2e64 6570 656e 6465 6e63 7927 2c0a  le.dependency',.
-00003a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003aa0: 2020 2020 2020 2020 2020 2020 2020 5b28                [(
-00003ab0: 276e 616d 6527 2c20 273d 272c 206d 6f64  'name', '=', mod
-00003ac0: 756c 6529 5d29 0a20 2020 2020 2020 2069  ule)]).        i
-00003ad0: 6620 6e6f 7420 6964 733a 0a20 2020 2020  f not ids:.     
-00003ae0: 2020 2020 2020 206f 7330 2e77 6c6f 6728         os0.wlog(
-00003af0: 273e 3e3e 2075 6e69 6e73 7461 6c6c 2025  '>>> uninstall %
-00003b00: 7327 2025 206d 6f64 756c 6529 0a20 2020  s' % module).   
-00003b10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00003b20: 636c 6f64 6f6f 2e61 6374 5f75 6e69 6e73  clodoo.act_unins
-00003b30: 7461 6c6c 5f6d 6f64 756c 6573 2863 7478  tall_modules(ctx
-00003b40: 2c20 6d6f 6475 6c65 5f6c 6973 743d 5b6d  , module_list=[m
-00003b50: 6f64 756c 655d 290a 2020 2020 7265 7475  odule]).    retu
-00003b60: 726e 2031 0a0a 0a64 6566 2072 656d 6f76  rn 1...def remov
-00003b70: 655f 756e 6d69 6772 6162 6c65 5f6d 6f64  e_unmigrable_mod
-00003b80: 756c 6573 2873 7263 5f63 7478 2c20 7467  ules(src_ctx, tg
-00003b90: 745f 6374 782c 2062 6164 5f6d 6f64 756c  t_ctx, bad_modul
-00003ba0: 655f 6c69 7374 293a 0a20 2020 204d 4f44  e_list):.    MOD
-00003bb0: 554c 4553 5f32 5f44 524f 5020 3d20 7b0a  ULES_2_DROP = {.
-00003bc0: 2020 2020 2020 2020 2731 322e 3027 3a20          '12.0': 
-00003bd0: 5b5d 2c0a 2020 2020 2020 2020 2731 312e  [],.        '11.
-00003be0: 3027 3a20 5b5d 2c0a 2020 2020 2020 2020  0': [],.        
-00003bf0: 2731 302e 3027 3a20 5b5d 2c0a 2020 2020  '10.0': [],.    
-00003c00: 2020 2020 2739 2e30 273a 205b 2761 6363      '9.0': ['acc
-00003c10: 6f75 6e74 5f66 696e 616e 6369 616c 5f72  ount_financial_r
-00003c20: 6570 6f72 745f 7765 626b 6974 5f78 6c73  eport_webkit_xls
-00003c30: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00003c40: 2020 2027 6261 7365 5f68 6561 6465 7273     'base_headers
-00003c50: 5f77 6562 6b69 7427 2c0a 2020 2020 2020  _webkit',.      
-00003c60: 2020 2020 2020 2020 2020 2765 6469 272c            'edi',
-00003c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003c80: 2027 6b6e 6f77 6c65 6467 6527 2c0a 2020   'knowledge',.  
-00003c90: 2020 2020 2020 2020 2020 2020 2020 276d                'm
-00003ca0: 756c 7469 5f63 6f6d 7061 6e79 272c 0a20  ulti_company',. 
-00003cb0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00003cc0: 7265 706f 7274 5f78 6c73 272c 0a20 2020  report_xls',.   
-00003cd0: 2020 2020 2020 2020 2020 2020 2027 7368               'sh
-00003ce0: 6172 6527 5d2c 0a20 2020 2020 2020 2027  are'],.        '
-00003cf0: 382e 3027 3a20 5b5d 2c0a 2020 2020 2020  8.0': [],.      
-00003d00: 2020 2737 2e30 273a 205b 5d2c 0a20 2020    '7.0': [],.   
-00003d10: 2020 2020 2027 362e 3127 3a20 5b5d 2c0a       '6.1': [],.
-00003d20: 2020 2020 7d0a 2020 2020 4d4f 4455 4c45      }.    MODULE
-00003d30: 535f 464f 5243 455f 325f 4452 4f50 203d  S_FORCE_2_DROP =
-00003d40: 207b 0a20 2020 2020 2020 2027 3132 2e30   {.        '12.0
-00003d50: 273a 205b 5d2c 0a20 2020 2020 2020 2027  ': [],.        '
-00003d60: 3131 2e30 273a 205b 5d2c 0a20 2020 2020  11.0': [],.     
-00003d70: 2020 2027 3130 2e30 273a 205b 5d2c 0a20     '10.0': [],. 
-00003d80: 2020 2020 2020 2027 392e 3027 3a20 5b27         '9.0': ['
-00003d90: 6174 7461 6368 6d65 6e74 5f70 7265 7669  attachment_previ
-00003da0: 6577 272c 0a20 2020 2020 2020 2020 2020  ew',.           
-00003db0: 2020 2020 2027 6c31 306e 5f69 745f 7370       'l10n_it_sp
-00003dc0: 6c69 745f 7061 796d 656e 7427 5d2c 0a20  lit_payment'],. 
-00003dd0: 2020 2020 2020 2027 382e 3027 3a20 5b5d         '8.0': []
-00003de0: 2c0a 2020 2020 2020 2020 2737 2e30 273a  ,.        '7.0':
-00003df0: 205b 5d2c 0a20 2020 2020 2020 2027 362e   [],.        '6.
-00003e00: 3127 3a20 5b5d 2c0a 2020 2020 7d0a 2020  1': [],.    }.  
-00003e10: 2020 6f64 6f6f 5f66 7665 7220 3d20 7467    odoo_fver = tg
-00003e20: 745f 6374 785b 2774 6774 5f6f 646f 6f5f  t_ctx['tgt_odoo_
-00003e30: 6676 6572 275d 0a20 2020 2075 6964 2c20  fver'].    uid, 
-00003e40: 6374 7820 3d20 636c 6f64 6f6f 2e6f 6572  ctx = clodoo.oer
-00003e50: 705f 7365 745f 656e 7628 6374 783d 7372  p_set_env(ctx=sr
-00003e60: 635f 6374 782c 2064 623d 7467 745f 6374  c_ctx, db=tgt_ct
-00003e70: 785b 2764 625f 6e61 6d65 275d 290a 2020  x['db_name']).  
-00003e80: 2020 2320 4649 5820 6f65 7270 5f73 6574    # FIX oerp_set
-00003e90: 5f65 6e76 2063 6861 6e67 6520 6472 795f  _env change dry_
-00003ea0: 7275 6e0a 2020 2020 7372 635f 6374 785b  run.    src_ctx[
-00003eb0: 2764 7279 5f72 756e 275d 203d 2074 6774  'dry_run'] = tgt
-00003ec0: 5f63 7478 5b27 6472 795f 7275 6e27 5d0a  _ctx['dry_run'].
-00003ed0: 2020 2020 666f 7220 6d6f 6475 6c65 2069      for module i
-00003ee0: 6e20 6261 645f 6d6f 6475 6c65 5f6c 6973  n bad_module_lis
-00003ef0: 743a 0a20 2020 2020 2020 2069 6620 6d6f  t:.        if mo
-00003f00: 6475 6c65 2069 6e20 4d4f 4455 4c45 535f  dule in MODULES_
-00003f10: 325f 4452 4f50 5b6f 646f 6f5f 6676 6572  2_DROP[odoo_fver
-00003f20: 5d3a 0a20 2020 2020 2020 2020 2020 2064  ]:.            d
-00003f30: 726f 705f 6d6f 6475 6c65 2863 7478 2c20  rop_module(ctx, 
-00003f40: 6d6f 6475 6c65 290a 2020 2020 2020 2020  module).        
-00003f50: 656c 6966 206d 6f64 756c 6520 696e 204d  elif module in M
-00003f60: 4f44 554c 4553 5f46 4f52 4345 5f32 5f44  ODULES_FORCE_2_D
-00003f70: 524f 505b 6f64 6f6f 5f66 7665 725d 3a0a  ROP[odoo_fver]:.
-00003f80: 2020 2020 2020 2020 2020 2020 6472 6f70              drop
-00003f90: 5f6d 6f64 756c 6528 6374 782c 206d 6f64  _module(ctx, mod
-00003fa0: 756c 652c 2066 6f72 6365 3d54 7275 6529  ule, force=True)
-00003fb0: 0a20 2020 2072 756e 5f74 7261 6365 6428  .    run_traced(
-00003fc0: 2770 675f 6462 5f61 6374 6976 6527 2c20  'pg_db_active', 
-00003fd0: 272d 7761 272c 2027 2573 2720 2520 7467  '-wa', '%s' % tg
-00003fe0: 745f 6374 785b 2764 625f 6e61 6d65 275d  t_ctx['db_name']
-00003ff0: 290a 0a0a 6465 6620 6472 6f70 5f6f 7574  )...def drop_out
-00004000: 5f6f 7269 6769 6e61 6c73 2863 7478 2c20  _originals(ctx, 
-00004010: 6d6f 6465 6c2c 2069 642c 2076 616c 7329  model, id, vals)
-00004020: 3a0a 2020 2020 6465 6620 6472 6f70 5f6f  :.    def drop_o
-00004030: 7574 5f6f 7269 6769 6e61 6c5f 6669 656c  ut_original_fiel
-00004040: 6428 6374 782c 206d 6f64 656c 2c20 6964  d(ctx, model, id
-00004050: 2c20 7661 6c73 2c20 6e61 6d65 293a 0a20  , vals, name):. 
-00004060: 2020 2020 2020 2064 6f5f 6964 7320 3d20         do_ids = 
-00004070: 636c 6f64 6f6f 2e73 6561 7263 684c 3828  clodoo.searchL8(
-00004080: 6374 782c 206d 6f64 656c 2c0a 2020 2020  ctx, model,.    
-00004090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040a0: 2020 2020 2020 2020 2020 2020 205b 286e               [(n
-000040b0: 616d 652c 2027 3d27 2c20 7661 6c73 5b6e  ame, '=', vals[n
-000040c0: 616d 655d 295d 290a 2020 2020 2020 2020  ame])]).        
-000040d0: 6966 2064 6f5f 6964 733a 0a20 2020 2020  if do_ids:.     
-000040e0: 2020 2020 2020 2066 6f72 2064 6f5f 6964         for do_id
-000040f0: 2069 6e20 646f 5f69 6473 3a0a 2020 2020   in do_ids:.    
-00004100: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00004110: 7478 5b27 5f63 7227 5d3a 0a20 2020 2020  tx['_cr']:.     
-00004120: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00004130: 6162 6c65 203d 206d 6f64 656c 2e72 6570  able = model.rep
-00004140: 6c61 6365 2827 2e27 2c20 275f 2729 0a20  lace('.', '_'). 
+000006d0: 0a20 2020 205d 2c0a 2020 2020 2320 2763  .    ],.    # 'c
+000006e0: 6f6d 6d65 7263 6961 6c5f 7061 7274 6e65  ommercial_partne
+000006f0: 725f 6964 275d 2c0a 2020 2020 2761 6363  r_id'],.    'acc
+00000700: 6f75 6e74 2e61 6363 6f75 6e74 273a 205b  ount.account': [
+00000710: 2770 6172 656e 745f 6964 272c 2027 7061  'parent_id', 'pa
+00000720: 7265 6e74 5f6c 6566 7427 2c20 2770 6172  rent_left', 'par
+00000730: 656e 745f 7269 6768 7427 5d2c 0a20 2020  ent_right'],.   
+00000740: 2027 2a27 3a20 5b0a 2020 2020 2020 2020   '*': [.        
+00000750: 276d 6573 7361 6765 5f66 6f6c 6c6f 7765  'message_followe
+00000760: 725f 6964 7327 2c0a 2020 2020 2020 2020  r_ids',.        
+00000770: 276d 6573 7361 6765 5f69 6473 272c 0a20  'message_ids',. 
+00000780: 2020 205d 2c0a 7d0a 4d41 4e44 4154 4f52     ],.}.MANDATOR
+00000790: 595f 4649 454c 4453 203d 207b 0a20 2020  Y_FIELDS = {.   
+000007a0: 2027 6163 636f 756e 742e 696e 766f 6963   'account.invoic
+000007b0: 6527 3a20 5b27 636f 6d70 616e 795f 6964  e': ['company_id
+000007c0: 275d 2c0a 7d0a 504b 4559 5320 3d20 7b0a  '],.}.PKEYS = {.
+000007d0: 2020 2020 2772 6573 2e63 6f75 6e74 7279      'res.country
+000007e0: 273a 2028 5b27 636f 6465 275d 2c20 5b27  ': (['code'], ['
+000007f0: 6e61 6d65 275d 292c 0a20 2020 2027 7265  name']),.    're
+00000800: 732e 636f 756e 7472 792e 7374 6174 6527  s.country.state'
+00000810: 3a20 280a 2020 2020 2020 2020 5b27 6e61  : (.        ['na
+00000820: 6d65 275d 2c0a 2020 2020 2020 2020 5b27  me'],.        ['
+00000830: 636f 6465 272c 2027 636f 756e 7472 795f  code', 'country_
+00000840: 6964 275d 2c0a 2020 2020 2020 2020 5b27  id'],.        ['
+00000850: 6469 6d5f 6e61 6d65 275d 2c0a 2020 2020  dim_name'],.    
+00000860: 292c 0a20 2020 2027 7265 732e 7061 7274  ),.    'res.part
+00000870: 6e65 7227 3a20 280a 2020 2020 2020 2020  ner': (.        
+00000880: 5b27 7661 7427 2c20 2766 6973 6361 6c63  ['vat', 'fiscalc
+00000890: 6f64 6527 2c20 2769 735f 636f 6d70 616e  ode', 'is_compan
+000008a0: 7927 2c20 2774 7970 6527 5d2c 0a20 2020  y', 'type'],.   
+000008b0: 2020 2020 205b 2776 6174 272c 2027 6669       ['vat', 'fi
+000008c0: 7363 616c 636f 6465 272c 2027 6973 5f63  scalcode', 'is_c
+000008d0: 6f6d 7061 6e79 275d 2c0a 2020 2020 2020  ompany'],.      
+000008e0: 2020 5b27 7265 615f 636f 6465 275d 2c0a    ['rea_code'],.
+000008f0: 2020 2020 2020 2020 5b27 7661 7427 2c20          ['vat', 
+00000900: 276e 616d 6527 2c20 2769 735f 636f 6d70  'name', 'is_comp
+00000910: 616e 7927 2c20 2774 7970 6527 5d2c 0a20  any', 'type'],. 
+00000920: 2020 2020 2020 205b 2766 6973 6361 6c63         ['fiscalc
+00000930: 6f64 6527 2c20 2774 7970 6527 5d2c 0a20  ode', 'type'],. 
+00000940: 2020 2020 2020 205b 2776 6174 272c 2027         ['vat', '
+00000950: 6973 5f63 6f6d 7061 6e79 275d 2c0a 2020  is_company'],.  
+00000960: 2020 2020 2020 5b27 6e61 6d65 272c 2027        ['name', '
+00000970: 6973 5f63 6f6d 7061 6e79 275d 2c0a 2020  is_company'],.  
+00000980: 2020 2020 2020 5b27 7661 7427 5d2c 0a20        ['vat'],. 
+00000990: 2020 2020 2020 205b 276e 616d 6527 5d2c         ['name'],
+000009a0: 0a20 2020 2020 2020 205b 2764 696d 5f6e  .        ['dim_n
+000009b0: 616d 6527 5d2c 0a20 2020 2029 2c0a 2020  ame'],.    ),.  
+000009c0: 2020 2772 6573 2e63 6f6d 7061 6e79 273a    'res.company':
+000009d0: 2028 5b27 7661 7427 5d2c 292c 0a20 2020   (['vat'],),.   
+000009e0: 2027 6163 636f 756e 742e 6163 636f 756e   'account.accoun
+000009f0: 742e 7479 7065 273a 2028 5b27 6e61 6d65  t.type': (['name
+00000a00: 275d 2c29 2c0a 2020 2020 2761 6363 6f75  '],),.    'accou
+00000a10: 6e74 2e61 6363 6f75 6e74 273a 2028 0a20  nt.account': (. 
+00000a20: 2020 2020 2020 205b 2763 6f64 6527 2c20         ['code', 
+00000a30: 2763 6f6d 7061 6e79 5f69 6427 5d2c 0a20  'company_id'],. 
+00000a40: 2020 2020 2020 205b 276e 616d 6527 2c20         ['name', 
+00000a50: 2763 6f6d 7061 6e79 5f69 6427 5d2c 0a20  'company_id'],. 
+00000a60: 2020 2020 2020 205b 2764 696d 5f6e 616d         ['dim_nam
+00000a70: 6527 2c20 2763 6f6d 7061 6e79 5f69 6427  e', 'company_id'
+00000a80: 5d2c 0a20 2020 2029 2c0a 2020 2020 2770  ],.    ),.    'p
+00000a90: 726f 6475 6374 2e74 656d 706c 6174 6527  roduct.template'
+00000aa0: 3a20 285b 276e 616d 6527 2c20 2764 6566  : (['name', 'def
+00000ab0: 6175 6c74 5f63 6f64 6527 5d29 2c0a 2020  ault_code']),.  
+00000ac0: 2020 2770 726f 6475 6374 2e70 726f 6475    'product.produ
+00000ad0: 6374 273a 2028 0a20 2020 2020 2020 205b  ct': (.        [
+00000ae0: 276e 616d 6527 2c20 2764 6566 6175 6c74  'name', 'default
+00000af0: 5f63 6f64 6527 5d2c 0a20 2020 2020 2020  _code'],.       
+00000b00: 205b 276e 616d 6527 2c20 2762 6172 636f   ['name', 'barco
+00000b10: 6465 275d 2c0a 2020 2020 2020 2020 5b27  de'],.        ['
+00000b20: 6e61 6d65 275d 2c0a 2020 2020 2020 2020  name'],.        
+00000b30: 5b27 6465 6661 756c 745f 636f 6465 275d  ['default_code']
+00000b40: 2c0a 2020 2020 2020 2020 5b27 6261 7263  ,.        ['barc
+00000b50: 6f64 6527 5d2c 0a20 2020 2020 2020 205b  ode'],.        [
+00000b60: 2764 696d 5f6e 616d 6527 5d2c 0a20 2020  'dim_name'],.   
+00000b70: 2029 2c0a 7d0a 4445 545f 4649 454c 4420   ),.}.DET_FIELD 
+00000b80: 3d20 7b0a 2020 2020 2761 6363 6f75 6e74  = {.    'account
+00000b90: 2e69 6e76 6f69 6365 273a 2027 696e 766f  .invoice': 'invo
+00000ba0: 6963 655f 6c69 6e65 272c 0a20 2020 2027  ice_line',.    '
+00000bb0: 7361 6c65 2e6f 7264 6572 273a 2027 6f72  sale.order': 'or
+00000bc0: 6465 725f 6c69 6e65 272c 0a7d 0a56 4552  der_line',.}.VER
+00000bd0: 5349 4f4e 5320 3d20 2827 362e 3127 2c20  SIONS = ('6.1', 
+00000be0: 2737 2e30 272c 2027 382e 3027 2c20 2739  '7.0', '8.0', '9
+00000bf0: 2e30 272c 2027 3130 2e30 272c 2027 3131  .0', '10.0', '11
+00000c00: 2e30 272c 2027 3132 2e30 2729 0a44 4546  .0', '12.0').DEF
+00000c10: 5f43 4f4e 4620 3d20 7b7d 0a4d 4f44 554c  _CONF = {}.MODUL
+00000c20: 4553 5f32 5f4c 4541 5645 5f42 4548 494e  ES_2_LEAVE_BEHIN
+00000c30: 4420 3d20 5b0a 2020 2020 2770 726f 6365  D = [.    'proce
+00000c40: 7373 272c 0a5d 0a50 5245 5f4d 4947 5241  ss',.].PRE_MIGRA
+00000c50: 5449 4f4e 203d 2027 2727 0a23 202d 2a2d  TION = '''.# -*-
+00000c60: 2063 6f64 696e 673a 2075 7466 2d38 202d   coding: utf-8 -
+00000c70: 2a2d 0a66 726f 6d20 6f70 656e 6572 702e  *-.from openerp.
+00000c80: 6f70 656e 7570 6772 6164 6520 696d 706f  openupgrade impo
+00000c90: 7274 206f 7065 6e75 7067 7261 6465 0a66  rt openupgrade.f
+00000ca0: 726f 6d20 6f70 656e 6572 702e 6164 646f  rom openerp.addo
+00000cb0: 6e73 2e6f 7065 6e75 7067 7261 6465 5f72  ns.openupgrade_r
+00000cc0: 6563 6f72 6473 2e6c 6962 2069 6d70 6f72  ecords.lib impor
+00000cd0: 7420 6170 7269 6f72 690a 0a23 2058 4d4c  t apriori..# XML
+00000ce0: 5f49 4453 2066 6f72 6d61 7420 6973 205b  _IDS format is [
+00000cf0: 286f 6c64 5f78 6964 2c20 6e65 775f 7869  (old_xid, new_xi
+00000d00: 6429 2e2e 2e5d 0a78 6d6c 5f69 6473 203d  d)...].xml_ids =
+00000d10: 205b 0a20 2020 2024 7b78 6d6c 5f69 6473   [.    ${xml_ids
+00000d20: 7d0a 5d0a 0a0a 6465 6620 636c 6561 6e75  }.]...def cleanu
+00000d30: 705f 6d6f 6475 6c65 7328 6372 293a 0a20  p_modules(cr):. 
+00000d40: 2020 2023 204d 6f64 756c 6520 6d65 7267     # Module merg
+00000d50: 6564 2066 6f72 6d61 7420 6973 205b 286f  ed format is [(o
+00000d60: 6c64 5f6d 6f64 756c 652c 206e 6577 5f6d  ld_module, new_m
+00000d70: 6f64 756c 6529 2e2e 2e5d 0a20 2020 206f  odule)...].    o
+00000d80: 7065 6e75 7067 7261 6465 2e75 7064 6174  penupgrade.updat
+00000d90: 655f 6d6f 6475 6c65 5f6e 616d 6573 280a  e_module_names(.
+00000da0: 2020 2020 2020 2020 6372 2c20 5b0a 2020          cr, [.  
+00000db0: 2020 2020 2020 2020 2020 247b 6d6f 6475            ${modu
+00000dc0: 6c65 5f6d 6572 6765 647d 0a20 2020 2020  le_merged}.     
+00000dd0: 2020 205d 2c20 6d65 7267 655f 6d6f 6475     ], merge_modu
+00000de0: 6c65 733d 5472 7565 2c0a 2020 2020 290a  les=True,.    ).
+00000df0: 0a0a 406f 7065 6e75 7067 7261 6465 2e6d  ..@openupgrade.m
+00000e00: 6967 7261 7465 2829 0a64 6566 206d 6967  igrate().def mig
+00000e10: 7261 7465 2863 722c 2076 6572 7369 6f6e  rate(cr, version
+00000e20: 293a 0a20 2020 2063 722e 6578 6563 7574  ):.    cr.execut
+00000e30: 6528 2764 726f 7020 7669 6577 2069 6620  e('drop view if 
+00000e40: 6578 6973 7473 2072 6570 6f72 745f 646f  exists report_do
+00000e50: 6375 6d65 6e74 5f75 7365 7220 6361 7363  cument_user casc
+00000e60: 6164 6527 290a 2020 2020 6f70 656e 7570  ade').    openup
+00000e70: 6772 6164 652e 7570 6461 7465 5f6d 6f64  grade.update_mod
+00000e80: 756c 655f 6e61 6d65 7328 0a20 2020 2020  ule_names(.     
+00000e90: 2020 2063 722c 2061 7072 696f 7269 2e72     cr, apriori.r
+00000ea0: 656e 616d 6564 5f6d 6f64 756c 6573 2e69  enamed_modules.i
+00000eb0: 7465 7269 7465 6d73 2829 0a20 2020 2029  teritems().    )
+00000ec0: 0a20 2020 206f 7065 6e75 7067 7261 6465  .    openupgrade
+00000ed0: 2e72 656e 616d 655f 786d 6c69 6473 2863  .rename_xmlids(c
+00000ee0: 722c 2078 6d6c 5f69 6473 290a 2020 2020  r, xml_ids).    
+00000ef0: 6f70 656e 7570 6772 6164 652e 6368 6563  openupgrade.chec
+00000f00: 6b5f 7661 6c75 6573 5f73 656c 6563 7469  k_values_selecti
+00000f10: 6f6e 5f66 6965 6c64 280a 2020 2020 2020  on_field(.      
+00000f20: 2020 6372 2c20 2769 725f 6163 745f 7265    cr, 'ir_act_re
+00000f30: 706f 7274 5f78 6d6c 272c 2027 7265 706f  port_xml', 'repo
+00000f40: 7274 5f74 7970 6527 2c0a 2020 2020 2020  rt_type',.      
+00000f50: 2020 5b27 636f 6e74 726f 6c6c 6572 272c    ['controller',
+00000f60: 2027 7064 6627 2c20 2771 7765 622d 6874   'pdf', 'qweb-ht
+00000f70: 6d6c 272c 2027 7177 6562 2d70 6466 272c  ml', 'qweb-pdf',
+00000f80: 2027 7378 7727 2c20 2777 6562 6b69 7427   'sxw', 'webkit'
+00000f90: 5d29 0a20 2020 206f 7065 6e75 7067 7261  ]).    openupgra
+00000fa0: 6465 2e63 6865 636b 5f76 616c 7565 735f  de.check_values_
+00000fb0: 7365 6c65 6374 696f 6e5f 6669 656c 6428  selection_field(
+00000fc0: 0a20 2020 2020 2020 2063 722c 2027 6972  .        cr, 'ir
+00000fd0: 5f75 695f 7669 6577 272c 2027 7479 7065  _ui_view', 'type
+00000fe0: 272c 205b 0a20 2020 2020 2020 2020 2020  ', [.           
+00000ff0: 2027 6361 6c65 6e64 6172 272c 2027 6469   'calendar', 'di
+00001000: 6167 7261 6d27 2c20 2766 6f72 6d27 2c20  agram', 'form', 
+00001010: 2767 616e 7474 272c 2027 6772 6170 6827  'gantt', 'graph'
+00001020: 2c20 276b 616e 6261 6e27 2c0a 2020 2020  , 'kanban',.    
+00001030: 2020 2020 2020 2020 2771 7765 6227 2c20          'qweb', 
+00001040: 2773 6561 7263 6827 2c20 2774 7265 6527  'search', 'tree'
+00001050: 5d29 0a20 2020 2063 6c65 616e 7570 5f6d  ]).    cleanup_m
+00001060: 6f64 756c 6573 2863 7229 0a27 2727 0a6d  odules(cr).'''.m
+00001070: 7367 5f74 696d 6520 3d20 7469 6d65 2e74  sg_time = time.t
+00001080: 696d 6528 290a 0a0a 6465 6620 6d73 675f  ime()...def msg_
+00001090: 6275 7273 7428 7465 7874 293a 0a20 2020  burst(text):.   
+000010a0: 2067 6c6f 6261 6c20 6d73 675f 7469 6d65   global msg_time
+000010b0: 0a20 2020 2074 203d 2074 696d 652e 7469  .    t = time.ti
+000010c0: 6d65 2829 202d 206d 7367 5f74 696d 650a  me() - msg_time.
+000010d0: 2020 2020 6966 2074 203e 2033 3a0a 2020      if t > 3:.  
+000010e0: 2020 2020 2020 7072 696e 7428 7465 7874        print(text
+000010f0: 290a 2020 2020 2020 2020 6d73 675f 7469  ).        msg_ti
+00001100: 6d65 203d 2074 696d 652e 7469 6d65 2829  me = time.time()
+00001110: 0a0a 0a40 636f 6e74 6578 746c 6962 2e63  ...@contextlib.c
+00001120: 6f6e 7465 7874 6d61 6e61 6765 720a 6465  ontextmanager.de
+00001130: 6620 7075 7368 6428 6e65 775f 6469 7229  f pushd(new_dir)
+00001140: 3a0a 2020 2020 7072 6576 696f 7573 5f64  :.    previous_d
+00001150: 6972 203d 206f 732e 6765 7463 7764 2829  ir = os.getcwd()
+00001160: 0a20 2020 206f 732e 6368 6469 7228 6e65  .    os.chdir(ne
+00001170: 775f 6469 7229 0a20 2020 2079 6965 6c64  w_dir).    yield
+00001180: 0a20 2020 206f 732e 6368 6469 7228 7072  .    os.chdir(pr
+00001190: 6576 696f 7573 5f64 6972 290a 0a0a 6465  evious_dir)...de
+000011a0: 6620 6d61 6e61 6765 5f65 7272 6f72 2829  f manage_error()
+000011b0: 3a0a 2020 2020 6475 6d6d 7920 3d20 2727  :.    dummy = ''
+000011c0: 0a20 2020 2077 6869 6c65 2064 756d 6d79  .    while dummy
+000011d0: 206e 6f74 2069 6e20 2827 4927 2c20 2769   not in ('I', 'i
+000011e0: 272c 2027 5327 2c20 2773 272c 2027 4427  ', 'S', 's', 'D'
+000011f0: 2c20 2764 2729 3a0a 2020 2020 2020 2020  , 'd'):.        
+00001200: 6475 6d6d 7920 3d20 696e 7075 7428 2728  dummy = input('(
+00001210: 4967 6e6f 7265 2c20 5374 6f70 2c20 4465  Ignore, Stop, De
+00001220: 6275 6729 3f20 2729 0a20 2020 2020 2020  bug)? ').       
+00001230: 2069 6620 6e6f 7420 6475 6d6d 793a 0a20   if not dummy:. 
+00001240: 2020 2020 2020 2020 2020 2064 756d 6d79             dummy
+00001250: 203d 2027 4927 0a20 2020 2020 2020 2069   = 'I'.        i
+00001260: 6620 6475 6d6d 7920 3d3d 2027 5327 206f  f dummy == 'S' o
+00001270: 7220 6475 6d6d 7920 3d3d 2027 7327 3a0a  r dummy == 's':.
+00001280: 2020 2020 2020 2020 2020 2020 7379 732e              sys.
+00001290: 6578 6974 2831 290a 2020 2020 2020 2020  exit(1).        
+000012a0: 6966 2064 756d 6d79 203d 3d20 2744 2720  if dummy == 'D' 
+000012b0: 6f72 2064 756d 6d79 203d 3d20 2764 273a  or dummy == 'd':
+000012c0: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
+000012d0: 6f72 7420 7064 6220 2023 2070 796c 696e  ort pdb  # pylin
+000012e0: 743a 2064 6973 6162 6c65 3d64 6570 7265  t: disable=depre
+000012f0: 6361 7465 642d 6d6f 6475 6c65 0a0a 2020  cated-module..  
+00001300: 2020 2020 2020 2020 2020 7064 622e 7365            pdb.se
+00001310: 745f 7472 6163 6528 290a 0a0a 6465 6620  t_trace()...def 
+00001320: 6578 6563 5f73 716c 2863 7478 2c20 7175  exec_sql(ctx, qu
+00001330: 6572 792c 2072 6573 706f 6e73 653d 4e6f  ery, response=No
+00001340: 6e65 293a 0a20 2020 2072 6574 7572 6e20  ne):.    return 
+00001350: 636c 6f64 6f6f 2e65 7865 635f 7371 6c28  clodoo.exec_sql(
+00001360: 6374 782c 2071 7565 7279 2c20 7265 7370  ctx, query, resp
+00001370: 6f6e 7365 3d72 6573 706f 6e73 6529 0a0a  onse=response)..
+00001380: 0a64 6566 2063 6f70 795f 6462 2863 7478  .def copy_db(ctx
+00001390: 2c20 6f6c 645f 6462 2c20 6e65 775f 6462  , old_db, new_db
+000013a0: 293a 0a20 2020 2073 716c 203d 2027 6472  ):.    sql = 'dr
+000013b0: 6f70 2064 6174 6162 6173 6520 6966 2065  op database if e
+000013c0: 7869 7374 7320 2225 7322 2720 2520 6e65  xists "%s"' % ne
+000013d0: 775f 6462 0a20 2020 2072 756e 5f74 7261  w_db.    run_tra
+000013e0: 6365 6428 2770 675f 6462 5f61 6374 6976  ced('pg_db_activ
+000013f0: 6527 2c20 272d 7761 272c 2027 2573 2720  e', '-wa', '%s' 
+00001400: 2520 6e65 775f 6462 290a 2020 2020 6578  % new_db).    ex
+00001410: 6563 5f73 716c 2863 7478 2c20 7371 6c29  ec_sql(ctx, sql)
+00001420: 0a20 2020 2073 716c 203d 2027 6372 6561  .    sql = 'crea
+00001430: 7465 2064 6174 6162 6173 6520 2225 7322  te database "%s"
+00001440: 2077 6974 6820 7465 6d70 6c61 7465 2022   with template "
+00001450: 2573 2227 2025 2028 6e65 775f 6462 2c20  %s"' % (new_db, 
+00001460: 6f6c 645f 6462 290a 2020 2020 636c 6f64  old_db).    clod
+00001470: 6f6f 2e73 716c 5f72 6563 6f6e 6e65 6374  oo.sql_reconnect
+00001480: 2863 7478 290a 2020 2020 7275 6e5f 7472  (ctx).    run_tr
+00001490: 6163 6564 2827 7067 5f64 625f 6163 7469  aced('pg_db_acti
+000014a0: 7665 272c 2027 2d77 6127 2c20 2725 7327  ve', '-wa', '%s'
+000014b0: 2025 206f 6c64 5f64 6229 0a20 2020 2069   % old_db).    i
+000014c0: 6620 6e6f 7420 6578 6563 5f73 716c 2863  f not exec_sql(c
+000014d0: 7478 2c20 7371 6c29 3a0a 2020 2020 2020  tx, sql):.      
+000014e0: 2020 7371 6c20 3d20 2763 7265 6174 6520    sql = 'create 
+000014f0: 6461 7461 6261 7365 2022 2573 2227 2025  database "%s"' %
+00001500: 206e 6577 5f64 620a 2020 2020 2020 2020   new_db.        
+00001510: 6578 6563 5f73 716c 2863 7478 2c20 7371  exec_sql(ctx, sq
+00001520: 6c29 0a20 2020 2020 2020 206f 732e 656e  l).        os.en
+00001530: 7669 726f 6e5b 2750 4755 5345 5227 5d20  viron['PGUSER'] 
+00001540: 3d20 6374 785b 2764 625f 7573 6572 275d  = ctx['db_user']
+00001550: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00001560: 6f73 2e65 6e76 6972 6f6e 2e67 6574 2827  os.environ.get('
+00001570: 5047 484f 5354 2729 3a0a 2020 2020 2020  PGHOST'):.      
+00001580: 2020 2020 2020 6f73 2e65 6e76 6972 6f6e        os.environ
+00001590: 5b27 5047 484f 5354 275d 203d 2063 7478  ['PGHOST'] = ctx
+000015a0: 5b27 6462 5f68 6f73 7427 5d0a 2020 2020  ['db_host'].    
+000015b0: 2020 2020 6966 206e 6f74 206f 732e 656e      if not os.en
+000015c0: 7669 726f 6e2e 6765 7428 2750 4750 4f52  viron.get('PGPOR
+000015d0: 5427 293a 0a20 2020 2020 2020 2020 2020  T'):.           
+000015e0: 206f 732e 656e 7669 726f 6e5b 2750 4750   os.environ['PGP
+000015f0: 4f52 5427 5d20 3d20 7374 7228 6374 785b  ORT'] = str(ctx[
+00001600: 2764 625f 706f 7274 275d 290a 2020 2020  'db_port']).    
+00001610: 2020 2020 636d 6420 3d20 280a 2020 2020      cmd = (.    
+00001620: 2020 2020 2020 2020 2770 675f 6475 6d70          'pg_dump
+00001630: 202d 5525 7320 2d2d 666f 726d 6174 3d63   -U%s --format=c
+00001640: 7573 746f 6d20 2d2d 6e6f 2d70 6173 7377  ustom --no-passw
+00001650: 6f72 6420 2573 2027 0a20 2020 2020 2020  ord %s '.       
+00001660: 2020 2020 2027 7c20 7067 5f72 6573 746f       '| pg_resto
+00001670: 7265 202d 5525 7320 2d2d 6e6f 2d70 6173  re -U%s --no-pas
+00001680: 7377 6f72 6420 2d2d 6462 6e61 6d65 3d25  sword --dbname=%
+00001690: 7327 0a20 2020 2020 2020 2020 2020 2025  s'.            %
+000016a0: 2028 6374 785b 2764 625f 7573 6572 275d   (ctx['db_user']
+000016b0: 2c20 6f6c 645f 6462 2c20 6374 785b 2764  , old_db, ctx['d
+000016c0: 625f 7573 6572 275d 2c20 6e65 775f 6462  b_user'], new_db
+000016d0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+000016e0: 2020 2020 6f73 302e 776c 6f67 2827 3e3e      os0.wlog('>>
+000016f0: 3e20 2573 2720 2520 636d 6429 0a20 2020  > %s' % cmd).   
+00001700: 2020 2020 2073 7473 203d 2030 0a20 2020       sts = 0.   
+00001710: 2020 2020 2069 6620 6e6f 7420 7372 635f       if not src_
+00001720: 6374 785b 2764 7279 5f72 756e 275d 3a0a  ctx['dry_run']:.
+00001730: 2020 2020 2020 2020 2020 2020 7374 7320              sts 
+00001740: 3d20 6f73 2e73 7973 7465 6d28 636d 6429  = os.system(cmd)
+00001750: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001760: 7374 7320 3d3d 2030 0a20 2020 2072 6574  sts == 0.    ret
+00001770: 7572 6e20 5472 7565 0a0a 0a64 6566 2065  urn True...def e
+00001780: 6e76 5f72 6566 2863 7478 2c20 7872 6566  nv_ref(ctx, xref
+00001790: 293a 0a20 2020 2078 7265 6673 203d 2078  ):.    xrefs = x
+000017a0: 7265 662e 7370 6c69 7428 272e 2729 0a20  ref.split('.'). 
+000017b0: 2020 2069 6620 6c65 6e28 7872 6566 7329     if len(xrefs)
+000017c0: 203d 3d20 323a 0a20 2020 2020 2020 2069   == 2:.        i
+000017d0: 6473 203d 2063 6c6f 646f 6f2e 7365 6172  ds = clodoo.sear
+000017e0: 6368 4c38 280a 2020 2020 2020 2020 2020  chL8(.          
+000017f0: 2020 6374 782c 2027 6972 2e6d 6f64 656c    ctx, 'ir.model
+00001800: 2e64 6174 6127 2c20 5b28 276d 6f64 756c  .data', [('modul
+00001810: 6527 2c20 273d 272c 2078 7265 6673 5b30  e', '=', xrefs[0
+00001820: 5d29 2c20 2827 6e61 6d65 272c 2027 3d27  ]), ('name', '='
+00001830: 2c20 7872 6566 735b 315d 295d 0a20 2020  , xrefs[1])].   
+00001840: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+00001850: 6620 6964 733a 0a20 2020 2020 2020 2020  f ids:.         
+00001860: 2020 2072 6574 7572 6e20 636c 6f64 6f6f     return clodoo
+00001870: 2e62 726f 7773 654c 3828 6374 782c 2027  .browseL8(ctx, '
+00001880: 6972 2e6d 6f64 656c 2e64 6174 6127 2c20  ir.model.data', 
+00001890: 6964 735b 305d 292e 7265 735f 6964 0a20  ids[0]).res_id. 
+000018a0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+000018b0: 0a0a 6465 6620 7079 5f72 6561 7373 6967  ..def py_reassig
+000018c0: 6e5f 6462 5f6f 776e 6572 2863 7478 2c20  n_db_owner(ctx, 
+000018d0: 6462 6e61 6d65 2c20 6f6c 645f 7573 6572  dbname, old_user
+000018e0: 2c20 6e65 775f 7573 6572 293a 0a20 2020  , new_user):.   
+000018f0: 2066 6f72 2073 716c 2069 6e20 280a 2020   for sql in (.  
+00001900: 2020 2020 2020 2247 5241 4e54 2041 4c4c        "GRANT ALL
+00001910: 2050 5249 5649 4c45 4745 5320 4f4e 2044   PRIVILEGES ON D
+00001920: 4154 4142 4153 4520 2573 2054 4f20 2573  ATABASE %s TO %s
+00001930: 2220 2520 2864 626e 616d 652c 206e 6577  " % (dbname, new
+00001940: 5f75 7365 7229 2c0a 2020 2020 2020 2020  _user),.        
+00001950: 2241 4c54 4552 2044 4154 4142 4153 4520  "ALTER DATABASE 
+00001960: 2573 204f 574e 4552 2054 4f20 2573 2220  %s OWNER TO %s" 
+00001970: 2520 2864 626e 616d 652c 206e 6577 5f75  % (dbname, new_u
+00001980: 7365 7229 2c0a 2020 2020 2020 2020 2247  ser),.        "G
+00001990: 5241 4e54 2041 4c4c 2050 5249 5649 4c45  RANT ALL PRIVILE
+000019a0: 4745 5320 4f4e 2041 4c4c 2054 4142 4c45  GES ON ALL TABLE
+000019b0: 5320 494e 2053 4348 454d 4120 7075 626c  S IN SCHEMA publ
+000019c0: 6963 2054 4f20 2573 2220 2520 6e65 775f  ic TO %s" % new_
+000019d0: 7573 6572 2c0a 2020 2020 2020 2020 2247  user,.        "G
+000019e0: 5241 4e54 2041 4c4c 2050 5249 5649 4c45  RANT ALL PRIVILE
+000019f0: 4745 5320 4f4e 2041 4c4c 2053 4551 5545  GES ON ALL SEQUE
+00001a00: 4e43 4553 2049 4e20 5343 4845 4d41 2070  NCES IN SCHEMA p
+00001a10: 7562 6c69 6320 544f 2025 7322 2025 206e  ublic TO %s" % n
+00001a20: 6577 5f75 7365 722c 0a20 2020 2020 2020  ew_user,.       
+00001a30: 2022 4752 414e 5420 414c 4c20 5052 4956   "GRANT ALL PRIV
+00001a40: 494c 4547 4553 204f 4e20 414c 4c20 4655  ILEGES ON ALL FU
+00001a50: 4e43 5449 4f4e 5320 494e 2053 4348 454d  NCTIONS IN SCHEM
+00001a60: 4120 7075 626c 6963 2054 4f20 2573 2220  A public TO %s" 
+00001a70: 2520 6e65 775f 7573 6572 2c0a 2020 2020  % new_user,.    
+00001a80: 2020 2020 2241 4c54 4552 2044 4546 4155      "ALTER DEFAU
+00001a90: 4c54 2050 5249 5649 4c45 4745 5320 4752  LT PRIVILEGES GR
+00001aa0: 414e 5420 414c 4c20 4f4e 2054 4142 4c45  ANT ALL ON TABLE
+00001ab0: 5320 544f 2025 7322 2025 206e 6577 5f75  S TO %s" % new_u
+00001ac0: 7365 722c 0a20 2020 2020 2020 2022 414c  ser,.        "AL
+00001ad0: 5445 5220 4445 4641 554c 5420 5052 4956  TER DEFAULT PRIV
+00001ae0: 494c 4547 4553 2047 5241 4e54 2041 4c4c  ILEGES GRANT ALL
+00001af0: 204f 4e20 5345 5155 454e 4345 5320 544f   ON SEQUENCES TO
+00001b00: 2025 7322 2025 206e 6577 5f75 7365 722c   %s" % new_user,
+00001b10: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00001b20: 7374 7320 3d20 6578 6563 5f73 716c 2863  sts = exec_sql(c
+00001b30: 7478 2c20 7371 6c29 0a20 2020 2020 2020  tx, sql).       
+00001b40: 2069 6620 7374 733a 0a20 2020 2020 2020   if sts:.       
+00001b50: 2020 2020 2072 6574 7572 6e20 7374 730a       return sts.
+00001b60: 2020 2020 7371 6c20 3d20 2273 656c 6563      sql = "selec
+00001b70: 7420 7461 626c 656e 616d 6520 6672 6f6d  t tablename from
+00001b80: 2070 675f 7461 626c 6573 2077 6865 7265   pg_tables where
+00001b90: 2073 6368 656d 616e 616d 6520 3d20 2770   schemaname = 'p
+00001ba0: 7562 6c69 6327 220a 2020 2020 7265 6373  ublic'".    recs
+00001bb0: 203d 2065 7865 635f 7371 6c28 6374 782c   = exec_sql(ctx,
+00001bc0: 2073 716c 2c20 7265 7370 6f6e 7365 3d54   sql, response=T
+00001bd0: 7275 6529 0a20 2020 2066 6f72 2072 6563  rue).    for rec
+00001be0: 2069 6e20 7265 6373 3a0a 2020 2020 2020   in recs:.      
+00001bf0: 2020 7371 6c20 3d20 2741 4c54 4552 2054    sql = 'ALTER T
+00001c00: 4142 4c45 2022 2573 2220 4f57 4e45 5220  ABLE "%s" OWNER 
+00001c10: 544f 2025 7327 2025 2028 7265 635b 305d  TO %s' % (rec[0]
+00001c20: 2c20 6e65 775f 7573 6572 290a 2020 2020  , new_user).    
+00001c30: 2020 2020 7374 7320 3d20 6578 6563 5f73      sts = exec_s
+00001c40: 716c 2863 7478 2c20 7371 6c29 0a20 2020  ql(ctx, sql).   
+00001c50: 2020 2020 2069 6620 7374 733a 0a20 2020       if sts:.   
+00001c60: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001c70: 7374 730a 2020 2020 2020 2020 7371 6c20  sts.        sql 
+00001c80: 3d20 2747 5241 4e54 2041 4c4c 2050 5249  = 'GRANT ALL PRI
+00001c90: 5649 4c45 4745 5320 4f4e 2054 4142 4c45  VILEGES ON TABLE
+00001ca0: 2022 2573 2220 544f 2025 7327 2025 2028   "%s" TO %s' % (
+00001cb0: 7265 635b 305d 2c20 6e65 775f 7573 6572  rec[0], new_user
+00001cc0: 290a 2020 2020 2020 2020 6578 6563 5f73  ).        exec_s
+00001cd0: 716c 2863 7478 2c20 7371 6c29 0a20 2020  ql(ctx, sql).   
+00001ce0: 2020 2020 2069 6620 7374 733a 0a20 2020       if sts:.   
+00001cf0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001d00: 7374 730a 2020 2020 7371 6c20 3d20 280a  sts.    sql = (.
+00001d10: 2020 2020 2020 2020 2273 656c 6563 7420          "select 
+00001d20: 7365 7175 656e 6365 5f6e 616d 6520 6672  sequence_name fr
+00001d30: 6f6d 2069 6e66 6f72 6d61 7469 6f6e 5f73  om information_s
+00001d40: 6368 656d 612e 7365 7175 656e 6365 7320  chema.sequences 
+00001d50: 220a 2020 2020 2020 2020 2277 6865 7265  ".        "where
+00001d60: 2073 6571 7565 6e63 655f 7363 6865 6d61   sequence_schema
+00001d70: 203d 2027 7075 626c 6963 2722 0a20 2020   = 'public'".   
+00001d80: 2029 0a20 2020 2072 6563 7320 3d20 6578   ).    recs = ex
+00001d90: 6563 5f73 716c 2863 7478 2c20 7371 6c2c  ec_sql(ctx, sql,
+00001da0: 2072 6573 706f 6e73 653d 5472 7565 290a   response=True).
+00001db0: 2020 2020 666f 7220 7265 6320 696e 2072      for rec in r
+00001dc0: 6563 733a 0a20 2020 2020 2020 2073 716c  ecs:.        sql
+00001dd0: 203d 2027 414c 5445 5220 5345 5155 454e   = 'ALTER SEQUEN
+00001de0: 4345 2022 2573 2220 4f57 4e45 5220 544f  CE "%s" OWNER TO
+00001df0: 2025 7327 2025 2028 7265 635b 305d 2c20   %s' % (rec[0], 
+00001e00: 6e65 775f 7573 6572 290a 2020 2020 2020  new_user).      
+00001e10: 2020 6578 6563 5f73 716c 2863 7478 2c20    exec_sql(ctx, 
+00001e20: 7371 6c29 0a20 2020 2020 2020 2069 6620  sql).        if 
+00001e30: 7374 733a 0a20 2020 2020 2020 2020 2020  sts:.           
+00001e40: 2072 6574 7572 6e20 7374 730a 2020 2020   return sts.    
+00001e50: 2020 2020 7371 6c20 3d20 2747 5241 4e54      sql = 'GRANT
+00001e60: 2041 4c4c 2050 5249 5649 4c45 4745 5320   ALL PRIVILEGES 
+00001e70: 4f4e 2053 4551 5545 4e43 4520 2225 7322  ON SEQUENCE "%s"
+00001e80: 2054 4f20 2573 2720 2520 2872 6563 5b30   TO %s' % (rec[0
+00001e90: 5d2c 206e 6577 5f75 7365 7229 0a20 2020  ], new_user).   
+00001ea0: 2020 2020 2065 7865 635f 7371 6c28 6374       exec_sql(ct
+00001eb0: 782c 2073 716c 290a 2020 2020 2020 2020  x, sql).        
+00001ec0: 6966 2073 7473 3a0a 2020 2020 2020 2020  if sts:.        
+00001ed0: 2020 2020 7265 7475 726e 2073 7473 0a20      return sts. 
+00001ee0: 2020 2073 716c 203d 2028 0a20 2020 2020     sql = (.     
+00001ef0: 2020 2022 7365 6c65 6374 2074 6162 6c65     "select table
+00001f00: 5f6e 616d 6520 6672 6f6d 2069 6e66 6f72  _name from infor
+00001f10: 6d61 7469 6f6e 5f73 6368 656d 612e 7669  mation_schema.vi
+00001f20: 6577 7320 220a 2020 2020 2020 2020 2277  ews ".        "w
+00001f30: 6865 7265 2074 6162 6c65 5f73 6368 656d  here table_schem
+00001f40: 6120 3d20 2770 7562 6c69 6327 220a 2020  a = 'public'".  
+00001f50: 2020 290a 2020 2020 7265 6373 203d 2065    ).    recs = e
+00001f60: 7865 635f 7371 6c28 6374 782c 2073 716c  xec_sql(ctx, sql
+00001f70: 2c20 7265 7370 6f6e 7365 3d54 7275 6529  , response=True)
+00001f80: 0a20 2020 2066 6f72 2072 6563 2069 6e20  .    for rec in 
+00001f90: 7265 6373 3a0a 2020 2020 2020 2020 7371  recs:.        sq
+00001fa0: 6c20 3d20 2741 4c54 4552 2056 4945 5720  l = 'ALTER VIEW 
+00001fb0: 2225 7322 204f 574e 4552 2054 4f20 2573  "%s" OWNER TO %s
+00001fc0: 2720 2520 2872 6563 5b30 5d2c 206e 6577  ' % (rec[0], new
+00001fd0: 5f75 7365 7229 0a20 2020 2020 2020 2065  _user).        e
+00001fe0: 7865 635f 7371 6c28 6374 782c 2073 716c  xec_sql(ctx, sql
+00001ff0: 290a 2020 2020 2020 2020 6966 2073 7473  ).        if sts
+00002000: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00002010: 7475 726e 2073 7473 0a20 2020 2020 2020  turn sts.       
+00002020: 2073 716c 203d 2027 4752 414e 5420 414c   sql = 'GRANT AL
+00002030: 4c20 5052 4956 494c 4547 4553 204f 4e20  L PRIVILEGES ON 
+00002040: 5441 424c 4520 2225 7322 2054 4f20 2573  TABLE "%s" TO %s
+00002050: 2720 2520 2872 6563 5b30 5d2c 206e 6577  ' % (rec[0], new
+00002060: 5f75 7365 7229 0a20 2020 2020 2020 2065  _user).        e
+00002070: 7865 635f 7371 6c28 6374 782c 2073 716c  xec_sql(ctx, sql
+00002080: 290a 2020 2020 2020 2020 6966 2073 7473  ).        if sts
+00002090: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000020a0: 7475 726e 2073 7473 0a20 2020 2073 716c  turn sts.    sql
+000020b0: 203d 2027 4752 414e 5420 2573 2054 4f20   = 'GRANT %s TO 
+000020c0: 2573 2720 2520 286f 6c64 5f75 7365 722c  %s' % (old_user,
+000020d0: 206e 6577 5f75 7365 7229 0a20 2020 2072   new_user).    r
+000020e0: 6574 7572 6e20 6578 6563 5f73 716c 2863  eturn exec_sql(c
+000020f0: 7478 2c20 7371 6c29 0a0a 0a64 6566 2072  tx, sql)...def r
+00002100: 6561 7373 6967 6e5f 6462 5f6f 776e 6572  eassign_db_owner
+00002110: 2863 7478 2c20 6462 6e61 6d65 2c20 6f6c  (ctx, dbname, ol
+00002120: 645f 7573 6572 2c20 6e65 775f 7573 6572  d_user, new_user
+00002130: 293a 0a20 2020 2072 756e 5f74 7261 6365  ):.    run_trace
+00002140: 6428 2770 675f 6462 5f61 6374 6976 6527  d('pg_db_active'
+00002150: 2c20 272d 7761 272c 2027 2573 2720 2520  , '-wa', '%s' % 
+00002160: 7467 745f 6374 785b 2764 625f 6e61 6d65  tgt_ctx['db_name
+00002170: 275d 290a 2020 2020 7374 7320 3d20 7079  ']).    sts = py
+00002180: 5f72 6561 7373 6967 6e5f 6462 5f6f 776e  _reassign_db_own
+00002190: 6572 280a 2020 2020 2020 2020 7467 745f  er(.        tgt_
+000021a0: 6374 782c 2074 6774 5f63 7478 5b27 6462  ctx, tgt_ctx['db
+000021b0: 5f6e 616d 6527 5d2c 2073 7263 5f63 7478  _name'], src_ctx
+000021c0: 5b27 6462 5f75 7365 7227 5d2c 2074 6774  ['db_user'], tgt
+000021d0: 5f63 7478 5b27 6462 5f75 7365 7227 5d0a  _ctx['db_user'].
+000021e0: 2020 2020 290a 2020 2020 6966 2073 7473      ).    if sts
+000021f0: 3a0a 2020 2020 2020 2020 7275 6e5f 7472  :.        run_tr
+00002200: 6163 6564 280a 2020 2020 2020 2020 2020  aced(.          
+00002210: 2020 2770 675f 6462 5f72 6561 7373 6967    'pg_db_reassig
+00002220: 6e5f 6f77 6e65 7227 2c0a 2020 2020 2020  n_owner',.      
+00002230: 2020 2020 2020 272d 6427 2c0a 2020 2020        '-d',.    
+00002240: 2020 2020 2020 2020 7467 745f 6374 785b          tgt_ctx[
+00002250: 2764 625f 6e61 6d65 275d 2c0a 2020 2020  'db_name'],.    
+00002260: 2020 2020 2020 2020 272d 6f27 2c0a 2020          '-o',.  
+00002270: 2020 2020 2020 2020 2020 7372 635f 6374            src_ct
+00002280: 785b 2764 625f 7573 6572 275d 2c0a 2020  x['db_user'],.  
+00002290: 2020 2020 2020 2020 2020 272d 5527 2c0a            '-U',.
+000022a0: 2020 2020 2020 2020 2020 2020 7467 745f              tgt_
+000022b0: 6374 785b 2764 625f 7573 6572 275d 2c0a  ctx['db_user'],.
+000022c0: 2020 2020 2020 2020 290a 0a0a 6465 6620          )...def 
+000022d0: 6472 6f70 5f73 6573 7369 6f6e 2863 7478  drop_session(ctx
+000022e0: 2c20 6462 6e61 6d65 2c20 6461 7461 6469  , dbname, datadi
+000022f0: 723d 4e6f 6e65 2c20 6f64 6f6f 5f76 6964  r=None, odoo_vid
+00002300: 3d4e 6f6e 6529 3a0a 2020 2020 6966 206e  =None):.    if n
+00002310: 6f74 206f 646f 6f5f 7669 643a 0a20 2020  ot odoo_vid:.   
+00002320: 2020 2020 206f 646f 6f5f 7669 6420 3d20       odoo_vid = 
+00002330: 6374 782e 6765 7428 2774 6774 5f76 6964  ctx.get('tgt_vid
+00002340: 2729 0a20 2020 2069 6620 6e6f 7420 6f64  ').    if not od
+00002350: 6f6f 5f76 6964 3a0a 2020 2020 2020 2020  oo_vid:.        
+00002360: 6f64 6f6f 5f76 6964 203d 2063 7478 2e67  odoo_vid = ctx.g
+00002370: 6574 2827 7372 635f 7669 6427 290a 2020  et('src_vid').  
+00002380: 2020 6966 206e 6f74 2064 6174 6164 6972    if not datadir
+00002390: 3a0a 2020 2020 2020 2020 6461 7461 6469  :.        datadi
+000023a0: 7220 3d20 6374 782e 6765 7428 2764 6174  r = ctx.get('dat
+000023b0: 615f 6469 7227 290a 2020 2020 6966 206e  a_dir').    if n
+000023c0: 6f74 2064 6174 6164 6972 3a0a 2020 2020  ot datadir:.    
+000023d0: 2020 2020 6461 7461 6469 7220 3d20 636c      datadir = cl
+000023e0: 6f64 6f6f 2e62 7569 6c64 5f6f 646f 6f5f  odoo.build_odoo_
+000023f0: 7061 7261 6d28 2744 4449 5227 2c20 6f64  param('DDIR', od
+00002400: 6f6f 5f76 6964 3d6f 646f 6f5f 7669 642c  oo_vid=odoo_vid,
+00002410: 206d 756c 7469 3d54 7275 6529 0a20 2020   multi=True).   
+00002420: 206f 646f 6f5f 7665 7220 3d20 636c 6f64   odoo_ver = clod
+00002430: 6f6f 2e62 7569 6c64 5f6f 646f 6f5f 7061  oo.build_odoo_pa
+00002440: 7261 6d28 274d 414a 5645 5227 2c20 6f64  ram('MAJVER', od
+00002450: 6f6f 5f76 6964 3d6f 646f 6f5f 7669 642c  oo_vid=odoo_vid,
+00002460: 206d 756c 7469 3d54 7275 6529 0a20 2020   multi=True).   
+00002470: 2069 6620 6f64 6f6f 5f76 6572 203c 2038   if odoo_ver < 8
+00002480: 3a0a 2020 2020 2020 2020 6f73 2e73 7973  :.        os.sys
+00002490: 7465 6d28 0a20 2020 2020 2020 2020 2020  tem(.           
+000024a0: 2027 2727 666f 7220 6620 696e 2024 2867   '''for f in $(g
+000024b0: 7265 7020 2d6c 2022 2573 2220 2f74 6d70  rep -l "%s" /tmp
+000024c0: 2f6f 652d 7365 7373 696f 6e73 2d6f 646f  /oe-sessions-odo
+000024d0: 6f2f 2a29 3b20 646f 0a20 2020 2020 2020  o/*); do.       
+000024e0: 2072 6d20 2d66 2024 663b 2064 6f6e 6527   rm -f $f; done'
+000024f0: 2727 0a20 2020 2020 2020 2020 2020 2025  ''.            %
+00002500: 2028 6462 6e61 6d65 290a 2020 2020 2020   (dbname).      
+00002510: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
+00002520: 2020 2020 2020 6f73 2e73 7973 7465 6d28        os.system(
+00002530: 0a20 2020 2020 2020 2020 2020 2027 2727  .            '''
+00002540: 666f 7220 6620 696e 2024 2867 7265 7020  for f in $(grep 
+00002550: 2d6c 2022 2573 2220 2573 2f73 6573 7369  -l "%s" %s/sessi
+00002560: 6f6e 732f 2a29 3b20 646f 0a20 2020 2020  ons/*); do.     
+00002570: 2020 2072 6d20 2d66 2024 663b 2064 6f6e     rm -f $f; don
+00002580: 6527 2727 0a20 2020 2020 2020 2020 2020  e'''.           
+00002590: 2025 2028 6462 6e61 6d65 2c20 6461 7461   % (dbname, data
+000025a0: 6469 7229 0a20 2020 2020 2020 2029 0a0a  dir).        )..
+000025b0: 0a64 6566 2067 6574 5f63 6163 6865 2863  .def get_cache(c
+000025c0: 7478 293a 0a20 2020 2063 7478 5b27 5f43  tx):.    ctx['_C
+000025d0: 4143 4845 275d 203d 2063 7478 2e67 6574  ACHE'] = ctx.get
+000025e0: 2827 5f43 4143 4845 272c 207b 7d29 0a20  ('_CACHE', {}). 
+000025f0: 2020 2072 6574 7572 6e20 6374 785b 275f     return ctx['_
+00002600: 4341 4348 4527 5d0a 0a0a 6465 6620 6361  CACHE']...def ca
+00002610: 6368 655f 6973 5f65 6e74 7279 2863 6163  che_is_entry(cac
+00002620: 6865 2c20 6d6f 6465 6c2c 2069 6429 3a0a  he, model, id):.
+00002630: 2020 2020 6361 6368 655b 6d6f 6465 6c5d      cache[model]
+00002640: 203d 2063 6163 6865 2e67 6574 286d 6f64   = cache.get(mod
+00002650: 656c 2c20 7b7d 290a 2020 2020 7265 7475  el, {}).    retu
+00002660: 726e 2069 6420 696e 2063 6163 6865 5b6d  rn id in cache[m
+00002670: 6f64 656c 5d0a 0a0a 6465 6620 6361 6368  odel]...def cach
+00002680: 655f 6765 745f 656e 7472 7928 6361 6368  e_get_entry(cach
+00002690: 652c 206d 6f64 656c 2c20 6964 293a 0a20  e, model, id):. 
+000026a0: 2020 2063 6163 6865 5b6d 6f64 656c 5d20     cache[model] 
+000026b0: 3d20 6361 6368 652e 6765 7428 6d6f 6465  = cache.get(mode
+000026c0: 6c2c 207b 7d29 0a20 2020 2072 6574 7572  l, {}).    retur
+000026d0: 6e20 6361 6368 655b 6d6f 6465 6c5d 2e67  n cache[model].g
+000026e0: 6574 2827 6964 272c 2046 616c 7365 290a  et('id', False).
+000026f0: 0a0a 6465 6620 6361 6368 655f 7374 6f72  ..def cache_stor
+00002700: 655f 656e 7472 7928 6361 6368 652c 206d  e_entry(cache, m
+00002710: 6f64 656c 2c20 6964 2c20 6b65 6570 3d4e  odel, id, keep=N
+00002720: 6f6e 6529 3a0a 2020 2020 6361 6368 655b  one):.    cache[
+00002730: 6d6f 6465 6c5d 203d 2063 6163 6865 2e67  model] = cache.g
+00002740: 6574 286d 6f64 656c 2c20 7b7d 290a 2020  et(model, {}).  
+00002750: 2020 6966 2069 6420 6f72 206b 6565 703a    if id or keep:
+00002760: 0a20 2020 2020 2020 2063 6163 6865 5b6d  .        cache[m
+00002770: 6f64 656c 5d5b 2769 6427 5d20 3d20 6964  odel]['id'] = id
+00002780: 0a20 2020 2065 6c69 6620 6964 2069 6e20  .    elif id in 
+00002790: 6361 6368 655b 6d6f 6465 6c5d 3a0a 2020  cache[model]:.  
+000027a0: 2020 2020 2020 6465 6c20 6361 6368 655b        del cache[
+000027b0: 6d6f 6465 6c5d 5b27 6964 275d 0a20 2020  model]['id'].   
+000027c0: 2072 6574 7572 6e20 6361 6368 655b 6d6f   return cache[mo
+000027d0: 6465 6c5d 0a0a 0a64 6566 2073 6574 5f74  del]...def set_t
+000027e0: 6d70 5f6b 6579 7328 6374 782c 206d 6f64  mp_keys(ctx, mod
+000027f0: 656c 2c20 6964 2c20 7661 6c73 293a 0a20  el, id, vals):. 
+00002800: 2020 2074 7279 5f61 6761 696e 203d 2046     try_again = F
+00002810: 616c 7365 0a20 2020 2069 6620 2763 6f64  alse.    if 'cod
+00002820: 6527 2069 6e20 7661 6c73 3a0a 2020 2020  e' in vals:.    
+00002830: 2020 2020 7661 6c73 5b27 636f 6465 275d      vals['code']
+00002840: 203d 2073 7472 2869 6429 0a20 2020 2020   = str(id).     
+00002850: 2020 2074 7279 5f61 6761 696e 203d 2054     try_again = T
+00002860: 7275 650a 2020 2020 6966 2027 6e61 6d65  rue.    if 'name
+00002870: 2720 696e 2076 616c 733a 0a20 2020 2020  ' in vals:.     
+00002880: 2020 2076 616c 735b 276e 616d 6527 5d20     vals['name'] 
+00002890: 3d20 2749 443d 2564 2025 7327 2025 2028  = 'ID=%d %s' % (
+000028a0: 6964 2c20 7661 6c73 5b27 6e61 6d65 275d  id, vals['name']
+000028b0: 290a 2020 2020 2020 2020 7472 795f 6167  ).        try_ag
+000028c0: 6169 6e20 3d20 5472 7565 0a20 2020 2072  ain = True.    r
+000028d0: 6574 7572 6e20 7472 795f 6167 6169 6e2c  eturn try_again,
+000028e0: 2076 616c 730a 0a0a 6465 6620 7275 6e5f   vals...def run_
+000028f0: 7472 6163 6564 282a 6172 6773 293a 0a20  traced(*args):. 
+00002900: 2020 206f 7330 2e77 6c6f 6728 273e 3e3e     os0.wlog('>>>
+00002910: 2025 7327 2025 2027 2027 2e6a 6f69 6e28   %s' % ' '.join(
+00002920: 6172 6773 2929 0a20 2020 2072 6574 7572  args)).    retur
+00002930: 6e20 506f 7065 6e28 6172 6773 292e 7761  n Popen(args).wa
+00002940: 6974 2829 0a0a 0a64 6566 2073 6564 282a  it()...def sed(*
+00002950: 6172 6773 293a 0a20 2020 2066 696c 656e  args):.    filen
+00002960: 616d 6520 3d20 6172 6773 5b30 5d0a 2020  ame = args[0].  
+00002970: 2020 7769 7468 206f 7065 6e28 6669 6c65    with open(file
+00002980: 6e61 6d65 2c20 2772 2729 2061 7320 6664  name, 'r') as fd
+00002990: 3a0a 2020 2020 2020 2020 6c69 6e65 7320  :.        lines 
+000029a0: 3d20 6664 2e72 6561 6428 292e 7370 6c69  = fd.read().spli
+000029b0: 7428 275c 6e27 290a 2020 2020 666f 7220  t('\n').    for 
+000029c0: 6172 6720 696e 2061 7267 735b 313a 5d3a  arg in args[1:]:
+000029d0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000029e0: 6973 696e 7374 616e 6365 2861 7267 2c20  isinstance(arg, 
+000029f0: 2874 7570 6c65 2c20 6c69 7374 2929 3a0a  (tuple, list)):.
+00002a00: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00002a10: 6520 4b65 7945 7272 6f72 2827 496e 7661  e KeyError('Inva
+00002a20: 6c69 6420 7061 7261 6d65 7465 7327 290a  lid parametes').
+00002a30: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
+00002a40: 6e6f 2069 6e20 7261 6e67 6528 6c65 6e28  no in range(len(
+00002a50: 6c69 6e65 7329 293a 0a20 2020 2020 2020  lines)):.       
+00002a60: 2020 2020 206c 696e 6573 5b6c 696e 656e       lines[linen
+00002a70: 6f5d 203d 2072 652e 7375 6228 6172 675b  o] = re.sub(arg[
+00002a80: 305d 2c20 6172 675b 315d 2c20 6c69 6e65  0], arg[1], line
+00002a90: 735b 6c69 6e65 6e6f 5d29 0a20 2020 2077  s[lineno]).    w
+00002aa0: 6974 6820 6f70 656e 2866 696c 656e 616d  ith open(filenam
+00002ab0: 652c 2027 7727 2920 6173 2066 643a 0a20  e, 'w') as fd:. 
+00002ac0: 2020 2020 2020 2066 642e 7772 6974 6528         fd.write(
+00002ad0: 5f62 2827 5c6e 272e 6a6f 696e 286c 696e  _b('\n'.join(lin
+00002ae0: 6573 2929 290a 0a0a 6465 6620 7365 645f  es)))...def sed_
+00002af0: 6170 7065 6e64 282a 6172 6773 293a 0a20  append(*args):. 
+00002b00: 2020 2066 696c 656e 616d 6520 3d20 6172     filename = ar
+00002b10: 6773 5b30 5d0a 2020 2020 7769 7468 206f  gs[0].    with o
+00002b20: 7065 6e28 6669 6c65 6e61 6d65 2c20 2772  pen(filename, 'r
+00002b30: 2729 2061 7320 6664 3a0a 2020 2020 2020  ') as fd:.      
+00002b40: 2020 6c69 6e65 7320 3d20 6664 2e72 6561    lines = fd.rea
+00002b50: 6428 292e 7370 6c69 7428 275c 6e27 290a  d().split('\n').
+00002b60: 2020 2020 666f 7220 6172 6720 696e 2061      for arg in a
+00002b70: 7267 735b 313a 5d3a 0a20 2020 2020 2020  rgs[1:]:.       
+00002b80: 206c 696e 6573 2e61 7070 656e 6428 6172   lines.append(ar
+00002b90: 6729 0a20 2020 2077 6974 6820 6f70 656e  g).    with open
+00002ba0: 2866 696c 656e 616d 652c 2027 7727 2920  (filename, 'w') 
+00002bb0: 6173 2066 643a 0a20 2020 2020 2020 2066  as fd:.        f
+00002bc0: 642e 7772 6974 6528 5f62 2827 5c6e 272e  d.write(_b('\n'.
+00002bd0: 6a6f 696e 286c 696e 6573 2929 290a 0a0a  join(lines)))...
+00002be0: 6465 6620 636f 6e66 6967 5f67 6574 5f6c  def config_get_l
+00002bf0: 6973 7428 636f 6e66 6967 2c20 6974 656d  ist(config, item
+00002c00: 293a 0a20 2020 2072 6574 7572 6e20 636f  ):.    return co
+00002c10: 6e66 6967 2e67 6574 2827 6f70 7469 6f6e  nfig.get('option
+00002c20: 7327 2c20 6974 656d 292e 7374 7269 7028  s', item).strip(
+00002c30: 292e 7370 6c69 7428 272c 2729 0a0a 0a64  ).split(',')...d
+00002c40: 6566 2072 756e 5f6f 646f 6f5f 616c 6c74  ef run_odoo_allt
+00002c50: 6573 7428 6f64 6f6f 5f76 6964 2c20 636f  est(odoo_vid, co
+00002c60: 6e66 6e2c 2064 625f 6e61 6d65 2c20 6c6f  nfn, db_name, lo
+00002c70: 6766 696c 652c 206d 6f64 756c 6573 3d4e  gfile, modules=N
+00002c80: 6f6e 6529 3a0a 2020 2020 6966 206d 6f64  one):.    if mod
+00002c90: 756c 6573 3a0a 2020 2020 2020 2020 6d6f  ules:.        mo
+00002ca0: 6475 6c65 7320 3d20 272c 272e 6a6f 696e  dules = ','.join
+00002cb0: 286d 6f64 756c 6573 290a 2020 2020 656c  (modules).    el
+00002cc0: 7365 3a0a 2020 2020 2020 2020 6d6f 6475  se:.        modu
+00002cd0: 6c65 7320 3d20 2761 6c6c 270a 2020 2020  les = 'all'.    
+00002ce0: 7372 635f 6f64 6f6f 5f62 696e 203d 2063  src_odoo_bin = c
+00002cf0: 6c6f 646f 6f2e 6275 696c 645f 6f64 6f6f  lodoo.build_odoo
+00002d00: 5f70 6172 616d 2827 4249 4e27 2c20 6f64  _param('BIN', od
+00002d10: 6f6f 5f76 6964 3d6f 646f 6f5f 7669 642c  oo_vid=odoo_vid,
+00002d20: 206d 756c 7469 3d54 7275 6529 0a20 2020   multi=True).   
+00002d30: 2072 756e 5f74 7261 6365 6428 0a20 2020   run_traced(.   
+00002d40: 2020 2020 2073 7263 5f6f 646f 6f5f 6269       src_odoo_bi
+00002d50: 6e2c 0a20 2020 2020 2020 2027 2d63 272c  n,.        '-c',
+00002d60: 0a20 2020 2020 2020 2063 6f6e 666e 2c0a  .        confn,.
+00002d70: 2020 2020 2020 2020 272d 6427 2c0a 2020          '-d',.  
+00002d80: 2020 2020 2020 6462 5f6e 616d 652c 0a20        db_name,. 
+00002d90: 2020 2020 2020 2027 2d75 272c 0a20 2020         '-u',.   
+00002da0: 2020 2020 206d 6f64 756c 6573 2c0a 2020       modules,.  
+00002db0: 2020 2020 2020 272d 2d73 746f 702d 6166        '--stop-af
+00002dc0: 7465 722d 696e 6974 272c 0a20 2020 2020  ter-init',.     
+00002dd0: 2020 2027 2d2d 6e6f 2d78 6d6c 7270 6327     '--no-xmlrpc'
+00002de0: 2c0a 2020 2020 2020 2020 272d 2d6c 6f67  ,.        '--log
+00002df0: 6669 6c65 3d25 7327 2025 206c 6f67 6669  file=%s' % logfi
+00002e00: 6c65 2c0a 2020 2020 290a 0a0a 6465 6620  le,.    )...def 
+00002e10: 6462 5f65 7869 7374 2863 7478 2c20 6462  db_exist(ctx, db
+00002e20: 6e61 6d65 293a 0a20 2020 2073 6573 7369  name):.    sessi
+00002e30: 6f6e 203d 2063 6c6f 646f 6f2e 636f 6e6e  on = clodoo.conn
+00002e40: 6563 744c 3828 6374 7829 0a20 2020 2069  ectL8(ctx).    i
+00002e50: 6620 6973 696e 7374 616e 6365 2873 6573  f isinstance(ses
+00002e60: 7369 6f6e 2c20 6261 7365 7374 7269 6e67  sion, basestring
+00002e70: 293a 0a20 2020 2020 2020 206f 7330 2e77  ):.        os0.w
+00002e80: 6c6f 6728 2743 6f6e 6e65 6374 696f 6e20  log('Connection 
+00002e90: 6572 726f 7220 2573 2720 2520 7365 7373  error %s' % sess
+00002ea0: 696f 6e29 0a20 2020 2020 2020 2072 6169  ion).        rai
+00002eb0: 7365 2049 4f45 7272 6f72 2873 6573 7369  se IOError(sessi
+00002ec0: 6f6e 290a 2020 2020 6966 2064 626e 616d  on).    if dbnam
+00002ed0: 6520 696e 2063 7478 5b27 6f64 6f6f 5f73  e in ctx['odoo_s
+00002ee0: 6573 7369 6f6e 275d 2e64 622e 6c69 7374  ession'].db.list
+00002ef0: 2829 3a0a 2020 2020 2020 2020 7265 7475  ():.        retu
+00002f00: 726e 2054 7275 650a 2020 2020 7265 7475  rn True.    retu
+00002f10: 726e 2046 616c 7365 0a0a 0a64 6566 2077  rn False...def w
+00002f20: 6570 5f6c 6f67 7328 6374 7829 3a0a 2020  ep_logs(ctx):.  
+00002f30: 2020 6966 206f 732e 7061 7468 2e69 7364    if os.path.isd
+00002f40: 6972 2863 7478 5b27 6f70 745f 6f75 6c70  ir(ctx['opt_oulp
+00002f50: 6174 6827 5d29 3a0a 2020 2020 2020 2020  ath']):.        
+00002f60: 7368 7574 696c 2e72 6d74 7265 6528 6374  shutil.rmtree(ct
+00002f70: 785b 276f 7074 5f6f 756c 7061 7468 275d  x['opt_oulpath']
+00002f80: 290a 2020 2020 666f 7220 7665 7220 696e  ).    for ver in
+00002f90: 2056 4552 5349 4f4e 533a 0a20 2020 2020   VERSIONS:.     
+00002fa0: 2020 2074 6d70 5f64 6972 203d 206f 732e     tmp_dir = os.
+00002fb0: 7061 7468 2e6a 6f69 6e28 6374 785b 276f  path.join(ctx['o
+00002fc0: 7074 5f6f 7570 6174 6827 5d2c 2027 6f75  pt_oupath'], 'ou
+00002fd0: 5f25 7327 2025 2076 6572 290a 2020 2020  _%s' % ver).    
+00002fe0: 2020 2020 6966 206f 732e 7061 7468 2e69      if os.path.i
+00002ff0: 7364 6972 2874 6d70 5f64 6972 293a 0a20  sdir(tmp_dir):. 
+00003000: 2020 2020 2020 2020 2020 2073 6875 7469             shuti
+00003010: 6c2e 726d 7472 6565 2874 6d70 5f64 6972  l.rmtree(tmp_dir
+00003020: 290a 2020 2020 746d 705f 6469 7220 3d20  ).    tmp_dir = 
+00003030: 6f73 2e70 6174 682e 6a6f 696e 2863 7478  os.path.join(ctx
+00003040: 5b27 6f70 745f 6f75 7061 7468 275d 2c20  ['opt_oupath'], 
+00003050: 276f 7065 6e75 7067 7261 6465 2729 0a20  'openupgrade'). 
+00003060: 2020 2069 6620 6f73 2e70 6174 682e 6973     if os.path.is
+00003070: 6469 7228 746d 705f 6469 7229 3a0a 2020  dir(tmp_dir):.  
+00003080: 2020 2020 2020 7368 7574 696c 2e72 6d74        shutil.rmt
+00003090: 7265 6528 746d 705f 6469 7229 0a20 2020  ree(tmp_dir).   
+000030a0: 2066 6c6f 675f 6469 7220 3d20 6f73 2e70   flog_dir = os.p
+000030b0: 6174 682e 6469 726e 616d 6528 6374 785b  ath.dirname(ctx[
+000030c0: 276c 6f67 666e 275d 290a 2020 2020 6966  'logfn']).    if
+000030d0: 206e 6f74 206f 732e 7061 7468 2e69 7364   not os.path.isd
+000030e0: 6972 2866 6c6f 675f 6469 7229 3a0a 2020  ir(flog_dir):.  
+000030f0: 2020 2020 2020 6f73 2e6d 6b64 6972 2866        os.mkdir(f
+00003100: 6c6f 675f 6469 7229 0a20 2020 2069 6620  log_dir).    if 
+00003110: 6f73 2e70 6174 682e 6973 6669 6c65 2863  os.path.isfile(c
+00003120: 7478 5b27 6c6f 6766 6e27 5d29 3a0a 2020  tx['logfn']):.  
+00003130: 2020 2020 2020 6f73 2e72 656d 6f76 6528        os.remove(
+00003140: 6374 785b 276c 6f67 666e 275d 290a 2020  ctx['logfn']).  
+00003150: 2020 6966 206f 732e 7061 7468 2e69 7366    if os.path.isf
+00003160: 696c 6528 6374 785b 276c 6f67 6669 6c65  ile(ctx['logfile
+00003170: 275d 293a 0a20 2020 2020 2020 206f 732e  ']):.        os.
+00003180: 7265 6d6f 7665 2863 7478 5b27 6c6f 6766  remove(ctx['logf
+00003190: 696c 6527 5d29 0a20 2020 2069 6620 6374  ile']).    if ct
+000031a0: 785b 276f 6361 5f6d 6967 7261 7465 275d  x['oca_migrate']
+000031b0: 3a0a 2020 2020 2020 2020 6966 206f 732e  :.        if os.
+000031c0: 7061 7468 2e69 7364 6972 286f 732e 7061  path.isdir(os.pa
+000031d0: 7468 2e6a 6f69 6e28 6f73 2e70 6174 682e  th.join(os.path.
+000031e0: 6578 7061 6e64 7573 6572 2827 7e27 292c  expanduser('~'),
+000031f0: 2027 6f70 656e 7570 6772 6164 6527 2929   'openupgrade'))
+00003200: 3a0a 2020 2020 2020 2020 2020 2020 7368  :.            sh
+00003210: 7574 696c 2e72 6d74 7265 6528 6f73 2e70  util.rmtree(os.p
+00003220: 6174 682e 6a6f 696e 286f 732e 7061 7468  ath.join(os.path
+00003230: 2e65 7870 616e 6475 7365 7228 277e 2729  .expanduser('~')
+00003240: 2c20 276f 7065 6e75 7067 7261 6465 2729  , 'openupgrade')
+00003250: 290a 0a0a 6465 6620 6472 6f70 5f64 6228  )...def drop_db(
+00003260: 7372 635f 6374 782c 2074 6774 5f63 7478  src_ctx, tgt_ctx
+00003270: 2c20 6462 6e61 6d65 2c20 6462 6e61 6d65  , dbname, dbname
+00003280: 3229 3a0a 2020 2020 666f 7220 6462 2069  2):.    for db i
+00003290: 6e20 2864 626e 616d 652c 2064 626e 616d  n (dbname, dbnam
+000032a0: 6532 293a 0a20 2020 2020 2020 2063 6d64  e2):.        cmd
+000032b0: 203d 2027 7067 5f64 625f 6163 7469 7665   = 'pg_db_active
+000032c0: 202d 7761 2025 737c 6472 6f70 6462 202d   -wa %s|dropdb -
+000032d0: 5525 7320 2573 2720 2520 2864 622c 2074  U%s %s' % (db, t
+000032e0: 6774 5f63 7478 5b27 6462 5f75 7365 7227  gt_ctx['db_user'
+000032f0: 5d2c 2064 6229 0a20 2020 2020 2020 206f  ], db).        o
+00003300: 732e 7379 7374 656d 2863 6d64 290a 2020  s.system(cmd).  
+00003310: 2020 2020 2020 636d 6420 3d20 2770 675f        cmd = 'pg_
+00003320: 6462 5f61 6374 6976 6520 2d77 6120 2573  db_active -wa %s
+00003330: 7c64 726f 7064 6220 2d55 2573 2025 7327  |dropdb -U%s %s'
+00003340: 2025 2028 6462 2c20 7372 635f 6374 785b   % (db, src_ctx[
+00003350: 2764 625f 7573 6572 275d 2c20 6462 290a  'db_user'], db).
+00003360: 2020 2020 2020 2020 6f73 2e73 7973 7465          os.syste
+00003370: 6d28 636d 6429 0a0a 0a64 6566 2073 6574  m(cmd)...def set
+00003380: 5f75 6e69 6e73 7461 6c6c 6564 5f62 795f  _uninstalled_by_
+00003390: 7371 6c28 7467 745f 6374 782c 2062 6164  sql(tgt_ctx, bad
+000033a0: 5f6d 6f64 756c 655f 6c69 7374 293a 0a20  _module_list):. 
+000033b0: 2020 206f 7330 2e77 6c6f 6728 2773 6574     os0.wlog('set
+000033c0: 5f75 6e69 6e73 7461 6c6c 6564 5f62 795f  _uninstalled_by_
+000033d0: 7371 6c25 7327 2025 2062 6164 5f6d 6f64  sql%s' % bad_mod
+000033e0: 756c 655f 6c69 7374 290a 2020 2020 7175  ule_list).    qu
+000033f0: 6572 7920 3d20 280a 2020 2020 2020 2020  ery = (.        
+00003400: 2275 7064 6174 6520 6972 5f6d 6f64 756c  "update ir_modul
+00003410: 655f 6d6f 6475 6c65 2073 6574 2073 7461  e_module set sta
+00003420: 7465 3d27 756e 696e 7374 616c 6c65 6427  te='uninstalled'
+00003430: 220a 2020 2020 2020 2020 2220 7768 6572  ".        " wher
+00003440: 6520 6e61 6d65 2069 6e20 2825 7329 2061  e name in (%s) a
+00003450: 6e64 2073 7461 7465 3c3e 2769 6e73 7461  nd state<>'insta
+00003460: 6c6c 6564 273b 2220 2520 7374 7228 6261  lled';" % str(ba
+00003470: 645f 6d6f 6475 6c65 5f6c 6973 7429 5b31  d_module_list)[1
+00003480: 3a2d 315d 0a20 2020 2029 0a20 2020 2065  :-1].    ).    e
+00003490: 7865 635f 7371 6c28 7467 745f 6374 782c  xec_sql(tgt_ctx,
+000034a0: 2071 7565 7279 290a 0a0a 6465 6620 7365   query)...def se
+000034b0: 745f 696e 7374 616c 6c65 645f 6279 5f73  t_installed_by_s
+000034c0: 716c 2874 6774 5f63 7478 2c20 6261 645f  ql(tgt_ctx, bad_
+000034d0: 6d6f 6475 6c65 5f6c 6973 7429 3a0a 2020  module_list):.  
+000034e0: 2020 6f73 302e 776c 6f67 2827 7365 745f    os0.wlog('set_
+000034f0: 696e 7374 616c 6c65 645f 6279 5f73 716c  installed_by_sql
+00003500: 2573 2720 2520 6261 645f 6d6f 6475 6c65  %s' % bad_module
+00003510: 5f6c 6973 7429 0a20 2020 2071 7565 7279  _list).    query
+00003520: 203d 2028 0a20 2020 2020 2020 2022 7570   = (.        "up
+00003530: 6461 7465 2069 725f 6d6f 6475 6c65 5f6d  date ir_module_m
+00003540: 6f64 756c 6520 7365 7420 7374 6174 653d  odule set state=
+00003550: 2769 6e73 7461 6c6c 6564 2722 0a20 2020  'installed'".   
+00003560: 2020 2020 2022 2077 6865 7265 206e 616d       " where nam
+00003570: 6520 696e 2028 2573 293b 2220 2520 7374  e in (%s);" % st
+00003580: 7228 6261 645f 6d6f 6475 6c65 5f6c 6973  r(bad_module_lis
+00003590: 7429 5b31 3a2d 315d 0a20 2020 2029 0a20  t)[1:-1].    ). 
+000035a0: 2020 2065 7865 635f 7371 6c28 7467 745f     exec_sql(tgt_
+000035b0: 6374 782c 2071 7565 7279 290a 0a0a 6465  ctx, query)...de
+000035c0: 6620 7265 6e5f 6462 286f 6c64 5f64 626e  f ren_db(old_dbn
+000035d0: 616d 652c 206e 6577 5f64 626e 616d 652c  ame, new_dbname,
+000035e0: 2064 625f 7573 6572 293a 0a20 2020 2063   db_user):.    c
+000035f0: 6d64 203d 2028 0a20 2020 2020 2020 2027  md = (.        '
+00003600: 7067 5f64 625f 6163 7469 7665 202d 7761  pg_db_active -wa
+00003610: 2025 737c 270a 2020 2020 2020 2020 2770   %s|'.        'p
+00003620: 7371 6c20 2d55 2573 202d 6320 2241 4c54  sql -U%s -c "ALT
+00003630: 4552 2044 4154 4142 4153 4520 2573 2052  ER DATABASE %s R
+00003640: 454e 414d 4520 544f 2025 733b 2220 7465  ENAME TO %s;" te
+00003650: 6d70 6c61 7465 3127 0a20 2020 2020 2020  mplate1'.       
+00003660: 2025 2028 6f6c 645f 6462 6e61 6d65 2c20   % (old_dbname, 
+00003670: 6462 5f75 7365 722c 206f 6c64 5f64 626e  db_user, old_dbn
+00003680: 616d 652c 206e 6577 5f64 626e 616d 6529  ame, new_dbname)
+00003690: 0a20 2020 2029 0a20 2020 206f 732e 7379  .    ).    os.sy
+000036a0: 7374 656d 2863 6d64 290a 0a0a 6465 6620  stem(cmd)...def 
+000036b0: 6e65 775f 6462 6e61 6d65 2864 622c 206f  new_dbname(db, o
+000036c0: 646f 6f5f 7665 722c 206f 6361 5f6d 6967  doo_ver, oca_mig
+000036d0: 7261 7465 6429 3a0a 2020 2020 6966 206f  rated):.    if o
+000036e0: 6361 5f6d 6967 7261 7465 643a 0a20 2020  ca_migrated:.   
+000036f0: 2020 2020 2072 6574 7572 6e20 2725 735f       return '%s_
+00003700: 6d69 6772 6174 6564 2720 2520 6462 0a20  migrated' % db. 
+00003710: 2020 2070 7269 6f72 203d 206f 646f 6f5f     prior = odoo_
+00003720: 7665 7220 2d20 310a 2020 2020 6966 2064  ver - 1.    if d
+00003730: 622e 656e 6473 7769 7468 2873 7472 2870  b.endswith(str(p
+00003740: 7269 6f72 2929 3a0a 2020 2020 2020 2020  rior)):.        
+00003750: 7265 7475 726e 2027 2573 5f25 6427 2025  return '%s_%d' %
+00003760: 2028 6462 5b30 203a 202d 6c65 6e28 7374   (db[0 : -len(st
+00003770: 7228 7072 696f 7229 295d 2c20 6f64 6f6f  r(prior))], odoo
+00003780: 5f76 6572 290a 2020 2020 7265 7475 726e  _ver).    return
+00003790: 2027 2573 5f25 6427 2025 2028 6462 2c20   '%s_%d' % (db, 
+000037a0: 6f64 6f6f 5f76 6572 290a 0a0a 6465 6620  odoo_ver)...def 
+000037b0: 6472 6f70 5f6d 6f64 756c 6528 6374 782c  drop_module(ctx,
+000037c0: 206d 6f64 756c 652c 2066 6f72 6365 3d4e   module, force=N
+000037d0: 6f6e 6529 3a0a 2020 2020 6966 2066 6f72  one):.    if for
+000037e0: 6365 3a0a 2020 2020 2020 2020 6f73 302e  ce:.        os0.
+000037f0: 776c 6f67 2827 3e3e 3e20 756e 696e 7374  wlog('>>> uninst
+00003800: 616c 6c20 2573 2720 2520 6d6f 6475 6c65  all %s' % module
+00003810: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00003820: 2063 6c6f 646f 6f2e 6163 745f 756e 696e   clodoo.act_unin
+00003830: 7374 616c 6c5f 6d6f 6475 6c65 7328 6374  stall_modules(ct
+00003840: 782c 206d 6f64 756c 655f 6c69 7374 3d5b  x, module_list=[
+00003850: 6d6f 6475 6c65 5d29 0a20 2020 2065 6c73  module]).    els
+00003860: 653a 0a20 2020 2020 2020 206d 6f64 756c  e:.        modul
+00003870: 655f 6964 203d 2063 6c6f 646f 6f2e 7365  e_id = clodoo.se
+00003880: 6172 6368 4c38 2863 7478 2c20 2769 722e  archL8(ctx, 'ir.
+00003890: 6d6f 6475 6c65 2e6d 6f64 756c 6527 2c20  module.module', 
+000038a0: 5b28 276e 616d 6527 2c20 273d 272c 206d  [('name', '=', m
+000038b0: 6f64 756c 6529 5d29 0a20 2020 2020 2020  odule)]).       
+000038c0: 2069 6473 203d 2063 6c6f 646f 6f2e 7365   ids = clodoo.se
+000038d0: 6172 6368 4c38 280a 2020 2020 2020 2020  archL8(.        
+000038e0: 2020 2020 6374 782c 2027 6972 2e6d 6f64      ctx, 'ir.mod
+000038f0: 756c 652e 6d6f 6475 6c65 2e64 6570 656e  ule.module.depen
+00003900: 6465 6e63 7927 2c20 5b28 276e 616d 6527  dency', [('name'
+00003910: 2c20 273d 272c 206d 6f64 756c 6529 5d0a  , '=', module)].
+00003920: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00003930: 2020 6966 206e 6f74 2069 6473 3a0a 2020    if not ids:.  
+00003940: 2020 2020 2020 2020 2020 6f73 302e 776c            os0.wl
+00003950: 6f67 2827 3e3e 3e20 756e 696e 7374 616c  og('>>> uninstal
+00003960: 6c20 2573 2720 2520 6d6f 6475 6c65 290a  l %s' % module).
+00003970: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00003980: 726e 2063 6c6f 646f 6f2e 6163 745f 756e  rn clodoo.act_un
+00003990: 696e 7374 616c 6c5f 6d6f 6475 6c65 7328  install_modules(
+000039a0: 6374 782c 206d 6f64 756c 655f 6c69 7374  ctx, module_list
+000039b0: 3d5b 6d6f 6475 6c65 5d29 0a20 2020 2072  =[module]).    r
+000039c0: 6574 7572 6e20 310a 0a0a 6465 6620 7265  eturn 1...def re
+000039d0: 6d6f 7665 5f75 6e6d 6967 7261 626c 655f  move_unmigrable_
+000039e0: 6d6f 6475 6c65 7328 7372 635f 6374 782c  modules(src_ctx,
+000039f0: 2074 6774 5f63 7478 2c20 6261 645f 6d6f   tgt_ctx, bad_mo
+00003a00: 6475 6c65 5f6c 6973 7429 3a0a 2020 2020  dule_list):.    
+00003a10: 4d4f 4455 4c45 535f 325f 4452 4f50 203d  MODULES_2_DROP =
+00003a20: 207b 0a20 2020 2020 2020 2027 3132 2e30   {.        '12.0
+00003a30: 273a 205b 5d2c 0a20 2020 2020 2020 2027  ': [],.        '
+00003a40: 3131 2e30 273a 205b 5d2c 0a20 2020 2020  11.0': [],.     
+00003a50: 2020 2027 3130 2e30 273a 205b 5d2c 0a20     '10.0': [],. 
+00003a60: 2020 2020 2020 2027 392e 3027 3a20 5b0a         '9.0': [.
+00003a70: 2020 2020 2020 2020 2020 2020 2761 6363              'acc
+00003a80: 6f75 6e74 5f66 696e 616e 6369 616c 5f72  ount_financial_r
+00003a90: 6570 6f72 745f 7765 626b 6974 5f78 6c73  eport_webkit_xls
+00003aa0: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+00003ab0: 6261 7365 5f68 6561 6465 7273 5f77 6562  base_headers_web
+00003ac0: 6b69 7427 2c0a 2020 2020 2020 2020 2020  kit',.          
+00003ad0: 2020 2765 6469 272c 0a20 2020 2020 2020    'edi',.       
+00003ae0: 2020 2020 2027 6b6e 6f77 6c65 6467 6527       'knowledge'
+00003af0: 2c0a 2020 2020 2020 2020 2020 2020 276d  ,.            'm
+00003b00: 756c 7469 5f63 6f6d 7061 6e79 272c 0a20  ulti_company',. 
+00003b10: 2020 2020 2020 2020 2020 2027 7265 706f             'repo
+00003b20: 7274 5f78 6c73 272c 0a20 2020 2020 2020  rt_xls',.       
+00003b30: 2020 2020 2027 7368 6172 6527 2c0a 2020       'share',.  
+00003b40: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00003b50: 2027 382e 3027 3a20 5b5d 2c0a 2020 2020   '8.0': [],.    
+00003b60: 2020 2020 2737 2e30 273a 205b 5d2c 0a20      '7.0': [],. 
+00003b70: 2020 2020 2020 2027 362e 3127 3a20 5b5d         '6.1': []
+00003b80: 2c0a 2020 2020 7d0a 2020 2020 4d4f 4455  ,.    }.    MODU
+00003b90: 4c45 535f 464f 5243 455f 325f 4452 4f50  LES_FORCE_2_DROP
+00003ba0: 203d 207b 0a20 2020 2020 2020 2027 3132   = {.        '12
+00003bb0: 2e30 273a 205b 5d2c 0a20 2020 2020 2020  .0': [],.       
+00003bc0: 2027 3131 2e30 273a 205b 5d2c 0a20 2020   '11.0': [],.   
+00003bd0: 2020 2020 2027 3130 2e30 273a 205b 5d2c       '10.0': [],
+00003be0: 0a20 2020 2020 2020 2027 392e 3027 3a20  .        '9.0': 
+00003bf0: 5b27 6174 7461 6368 6d65 6e74 5f70 7265  ['attachment_pre
+00003c00: 7669 6577 272c 2027 6c31 306e 5f69 745f  view', 'l10n_it_
+00003c10: 7370 6c69 745f 7061 796d 656e 7427 5d2c  split_payment'],
+00003c20: 0a20 2020 2020 2020 2027 382e 3027 3a20  .        '8.0': 
+00003c30: 5b5d 2c0a 2020 2020 2020 2020 2737 2e30  [],.        '7.0
+00003c40: 273a 205b 5d2c 0a20 2020 2020 2020 2027  ': [],.        '
+00003c50: 362e 3127 3a20 5b5d 2c0a 2020 2020 7d0a  6.1': [],.    }.
+00003c60: 2020 2020 6f64 6f6f 5f66 7665 7220 3d20      odoo_fver = 
+00003c70: 7467 745f 6374 785b 2774 6774 5f6f 646f  tgt_ctx['tgt_odo
+00003c80: 6f5f 6676 6572 275d 0a20 2020 2075 6964  o_fver'].    uid
+00003c90: 2c20 6374 7820 3d20 636c 6f64 6f6f 2e6f  , ctx = clodoo.o
+00003ca0: 6572 705f 7365 745f 656e 7628 6374 783d  erp_set_env(ctx=
+00003cb0: 7372 635f 6374 782c 2064 623d 7467 745f  src_ctx, db=tgt_
+00003cc0: 6374 785b 2764 625f 6e61 6d65 275d 290a  ctx['db_name']).
+00003cd0: 2020 2020 2320 4649 5820 6f65 7270 5f73      # FIX oerp_s
+00003ce0: 6574 5f65 6e76 2063 6861 6e67 6520 6472  et_env change dr
+00003cf0: 795f 7275 6e0a 2020 2020 7372 635f 6374  y_run.    src_ct
+00003d00: 785b 2764 7279 5f72 756e 275d 203d 2074  x['dry_run'] = t
+00003d10: 6774 5f63 7478 5b27 6472 795f 7275 6e27  gt_ctx['dry_run'
+00003d20: 5d0a 2020 2020 666f 7220 6d6f 6475 6c65  ].    for module
+00003d30: 2069 6e20 6261 645f 6d6f 6475 6c65 5f6c   in bad_module_l
+00003d40: 6973 743a 0a20 2020 2020 2020 2069 6620  ist:.        if 
+00003d50: 6d6f 6475 6c65 2069 6e20 4d4f 4455 4c45  module in MODULE
+00003d60: 535f 325f 4452 4f50 5b6f 646f 6f5f 6676  S_2_DROP[odoo_fv
+00003d70: 6572 5d3a 0a20 2020 2020 2020 2020 2020  er]:.           
+00003d80: 2064 726f 705f 6d6f 6475 6c65 2863 7478   drop_module(ctx
+00003d90: 2c20 6d6f 6475 6c65 290a 2020 2020 2020  , module).      
+00003da0: 2020 656c 6966 206d 6f64 756c 6520 696e    elif module in
+00003db0: 204d 4f44 554c 4553 5f46 4f52 4345 5f32   MODULES_FORCE_2
+00003dc0: 5f44 524f 505b 6f64 6f6f 5f66 7665 725d  _DROP[odoo_fver]
+00003dd0: 3a0a 2020 2020 2020 2020 2020 2020 6472  :.            dr
+00003de0: 6f70 5f6d 6f64 756c 6528 6374 782c 206d  op_module(ctx, m
+00003df0: 6f64 756c 652c 2066 6f72 6365 3d54 7275  odule, force=Tru
+00003e00: 6529 0a20 2020 2072 756e 5f74 7261 6365  e).    run_trace
+00003e10: 6428 2770 675f 6462 5f61 6374 6976 6527  d('pg_db_active'
+00003e20: 2c20 272d 7761 272c 2027 2573 2720 2520  , '-wa', '%s' % 
+00003e30: 7467 745f 6374 785b 2764 625f 6e61 6d65  tgt_ctx['db_name
+00003e40: 275d 290a 0a0a 6465 6620 6472 6f70 5f6f  '])...def drop_o
+00003e50: 7574 5f6f 7269 6769 6e61 6c73 2863 7478  ut_originals(ctx
+00003e60: 2c20 6d6f 6465 6c2c 2069 642c 2076 616c  , model, id, val
+00003e70: 7329 3a0a 2020 2020 6465 6620 6472 6f70  s):.    def drop
+00003e80: 5f6f 7574 5f6f 7269 6769 6e61 6c5f 6669  _out_original_fi
+00003e90: 656c 6428 6374 782c 206d 6f64 656c 2c20  eld(ctx, model, 
+00003ea0: 6964 2c20 7661 6c73 2c20 6e61 6d65 293a  id, vals, name):
+00003eb0: 0a20 2020 2020 2020 2064 6f5f 6964 7320  .        do_ids 
+00003ec0: 3d20 636c 6f64 6f6f 2e73 6561 7263 684c  = clodoo.searchL
+00003ed0: 3828 6374 782c 206d 6f64 656c 2c20 5b28  8(ctx, model, [(
+00003ee0: 6e61 6d65 2c20 273d 272c 2076 616c 735b  name, '=', vals[
+00003ef0: 6e61 6d65 5d29 5d29 0a20 2020 2020 2020  name])]).       
+00003f00: 2069 6620 646f 5f69 6473 3a0a 2020 2020   if do_ids:.    
+00003f10: 2020 2020 2020 2020 666f 7220 646f 5f69          for do_i
+00003f20: 6420 696e 2064 6f5f 6964 733a 0a20 2020  d in do_ids:.   
+00003f30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00003f40: 6374 785b 275f 6372 275d 3a0a 2020 2020  ctx['_cr']:.    
+00003f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f60: 7461 626c 6520 3d20 6d6f 6465 6c2e 7265  table = model.re
+00003f70: 706c 6163 6528 272e 272c 2027 5f27 290a  place('.', '_').
+00003f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f90: 2020 2020 7371 6c20 3d20 2275 7064 6174      sql = "updat
+00003fa0: 6520 2573 2073 6574 2025 733d 2728 6964  e %s set %s='(id
+00003fb0: 3d25 6429 203d 3e25 6427 2077 6865 7265  =%d) =>%d' where
+00003fc0: 2069 643d 2564 3b22 2025 2028 0a20 2020   id=%d;" % (.   
+00003fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fe0: 2020 2020 2074 6162 6c65 2c0a 2020 2020       table,.    
+00003ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004000: 2020 2020 6e61 6d65 2c0a 2020 2020 2020      name,.      
+00004010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004020: 2020 646f 5f69 642c 0a20 2020 2020 2020    do_id,.       
+00004030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004040: 2069 642c 0a20 2020 2020 2020 2020 2020   id,.           
+00004050: 2020 2020 2020 2020 2020 2020 2064 6f5f               do_
+00004060: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+00004070: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00004080: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00004090: 6563 5f73 716c 2863 7478 2c20 7371 6c29  ec_sql(ctx, sql)
+000040a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000040b0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000040c0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+000040d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040e0: 2020 2020 2020 2020 636c 6f64 6f6f 2e77          clodoo.w
+000040f0: 7269 7465 4c38 280a 2020 2020 2020 2020  riteL8(.        
+00004100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004110: 2020 2020 6374 782c 206d 6f64 656c 2c20      ctx, model, 
+00004120: 646f 5f69 6473 2c20 7b6e 616d 653a 2027  do_ids, {name: '
+00004130: 2869 643d 2564 2920 3d3e 2564 2720 2520  (id=%d) =>%d' % 
+00004140: 2864 6f5f 6964 2c20 6964 297d 0a20 2020  (do_id, id)}.   
 00004150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004160: 2020 2073 716c 203d 2022 7570 6461 7465     sql = "update
-00004170: 2025 7320 7365 7420 2573 3d27 2869 643d   %s set %s='(id=
-00004180: 2564 2920 3d3e 2564 2720 7768 6572 6520  %d) =>%d' where 
-00004190: 6964 3d25 643b 2220 2520 280a 2020 2020  id=%d;" % (.    
-000041a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041b0: 2020 2020 7461 626c 652c 206e 616d 652c      table, name,
-000041c0: 2064 6f5f 6964 2c20 6964 2c20 646f 5f69   do_id, id, do_i
-000041d0: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-000041e0: 2020 2020 2020 2065 7865 635f 7371 6c28         exec_sql(
-000041f0: 6374 782c 2073 716c 290a 2020 2020 2020  ctx, sql).      
-00004200: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00004210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004220: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00004230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004240: 2063 6c6f 646f 6f2e 7772 6974 654c 3828   clodoo.writeL8(
-00004250: 6374 782c 206d 6f64 656c 2c20 646f 5f69  ctx, model, do_i
-00004260: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
-00004270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004280: 2020 2020 2020 2020 2020 207b 6e61 6d65             {name
-00004290: 3a20 2728 6964 3d25 6429 203d 3e25 6427  : '(id=%d) =>%d'
-000042a0: 2025 2028 0a20 2020 2020 2020 2020 2020   % (.           
-000042b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042d0: 646f 5f69 642c 2069 6429 7d29 0a20 2020  do_id, id)}).   
-000042e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042f0: 2065 7863 6570 7420 4261 7365 4578 6365   except BaseExce
-00004300: 7074 696f 6e3a 0a20 2020 2020 2020 2020  ption:.         
-00004310: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00004320: 6173 730a 2020 2020 6966 2027 636f 6465  ass.    if 'code
-00004330: 2720 696e 2076 616c 733a 0a20 2020 2020  ' in vals:.     
-00004340: 2020 2064 726f 705f 6f75 745f 6f72 6967     drop_out_orig
-00004350: 696e 616c 5f66 6965 6c64 2863 7478 2c20  inal_field(ctx, 
-00004360: 6d6f 6465 6c2c 2069 642c 2076 616c 732c  model, id, vals,
-00004370: 2027 636f 6465 2729 0a20 2020 2069 6620   'code').    if 
-00004380: 276e 616d 6527 2069 6e20 7661 6c73 3a0a  'name' in vals:.
-00004390: 2020 2020 2020 2020 6472 6f70 5f6f 7574          drop_out
-000043a0: 5f6f 7269 6769 6e61 6c5f 6669 656c 6428  _original_field(
-000043b0: 6374 782c 206d 6f64 656c 2c20 6964 2c20  ctx, model, id, 
-000043c0: 7661 6c73 2c20 276e 616d 6527 290a 0a0a  vals, 'name')...
-000043d0: 6465 6620 7765 705f 6669 656c 6473 2863  def wep_fields(c
-000043e0: 7478 2c20 7661 6c73 293a 0a20 2020 2066  tx, vals):.    f
-000043f0: 6f72 206e 6d20 696e 2028 2763 7265 6174  or nm in ('creat
-00004400: 655f 6461 7465 272c 2027 6372 6561 7465  e_date', 'create
-00004410: 5f75 6964 272c 2027 6964 272c 0a20 2020  _uid', 'id',.   
-00004420: 2020 2020 2020 2020 2020 2020 276d 6573              'mes
-00004430: 7361 6765 5f63 6861 6e6e 656c 5f69 6473  sage_channel_ids
-00004440: 272c 2027 6d65 7373 6167 655f 666f 6c6c  ', 'message_foll
-00004450: 6f77 6572 5f69 6473 272c 0a20 2020 2020  ower_ids',.     
-00004460: 2020 2020 2020 2020 2020 276d 6573 7361            'messa
-00004470: 6765 5f69 6473 272c 2027 6d65 7373 6167  ge_ids', 'messag
-00004480: 655f 6973 5f66 6f6c 6c6f 7765 7227 2c0a  e_is_follower',.
-00004490: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000044a0: 6d65 7373 6167 655f 6c61 7374 5f70 6f73  message_last_pos
-000044b0: 7427 2c20 276d 6573 7361 6765 5f6e 6565  t', 'message_nee
-000044c0: 6461 6374 696f 6e27 2c0a 2020 2020 2020  daction',.      
-000044d0: 2020 2020 2020 2020 2027 6d65 7373 6167           'messag
-000044e0: 655f 6e65 6564 6163 7469 6f6e 5f63 6f75  e_needaction_cou
-000044f0: 6e74 6572 272c 2027 6d65 7373 6167 655f  nter', 'message_
-00004500: 756e 7265 6164 272c 0a20 2020 2020 2020  unread',.       
-00004510: 2020 2020 2020 2020 276d 6573 7361 6765          'message
-00004520: 5f75 6e72 6561 645f 636f 756e 7465 7227  _unread_counter'
-00004530: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004540: 2027 7772 6974 655f 6461 7465 272c 2027   'write_date', '
-00004550: 7772 6974 655f 7569 6427 293a 0a20 2020  write_uid'):.   
-00004560: 2020 2020 2069 6620 6e6d 2069 6e20 7661       if nm in va
-00004570: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
-00004580: 6465 6c20 7661 6c73 5b6e 6d5d 0a20 2020  del vals[nm].   
-00004590: 2072 6574 7572 6e20 7661 6c73 0a0a 0a64   return vals...d
-000045a0: 6566 2077 7269 7465 5f6e 6f5f 6475 7028  ef write_no_dup(
-000045b0: 6374 782c 206d 6f64 656c 2c20 6964 732c  ctx, model, ids,
-000045c0: 2076 616c 732c 2073 7263 5f69 6429 3a0a   vals, src_id):.
-000045d0: 2020 2020 7661 6c73 203d 2077 6570 5f66      vals = wep_f
-000045e0: 6965 6c64 7328 6374 782c 2076 616c 7329  ields(ctx, vals)
-000045f0: 0a20 2020 2074 7279 5f61 6761 696e 203d  .    try_again =
-00004600: 2046 616c 7365 0a20 2020 2074 7279 3a0a   False.    try:.
-00004610: 2020 2020 2020 2020 636c 6f64 6f6f 2e77          clodoo.w
-00004620: 7269 7465 4c38 2863 7478 2c20 6d6f 6465  riteL8(ctx, mode
-00004630: 6c2c 2069 6473 2c20 7661 6c73 290a 2020  l, ids, vals).  
-00004640: 2020 6578 6365 7074 2049 4f45 7272 6f72    except IOError
-00004650: 3a0a 2020 2020 2020 2020 7472 795f 6167  :.        try_ag
-00004660: 6169 6e20 3d20 5472 7565 0a20 2020 2020  ain = True.     
-00004670: 2020 2064 726f 705f 6f75 745f 6f72 6967     drop_out_orig
-00004680: 696e 616c 7328 6374 782c 206d 6f64 656c  inals(ctx, model
-00004690: 2c20 6964 735b 305d 2c20 7661 6c73 290a  , ids[0], vals).
-000046a0: 2020 2020 6966 2074 7279 5f61 6761 696e      if try_again
-000046b0: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
-000046c0: 2020 2020 2020 2020 2020 2074 7279 5f61             try_a
-000046d0: 6761 696e 203d 2046 616c 7365 0a20 2020  gain = False.   
-000046e0: 2020 2020 2020 2020 2063 6c6f 646f 6f2e           clodoo.
-000046f0: 7772 6974 654c 3828 6374 782c 206d 6f64  writeL8(ctx, mod
-00004700: 656c 2c20 6964 732c 2076 616c 7329 0a20  el, ids, vals). 
-00004710: 2020 2020 2020 2065 7863 6570 7420 494f         except IO
-00004720: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-00004730: 2020 2074 7279 5f61 6761 696e 2c20 7661     try_again, va
-00004740: 6c73 203d 2073 6574 5f74 6d70 5f6b 6579  ls = set_tmp_key
-00004750: 7328 6374 782c 206d 6f64 656c 2c20 6964  s(ctx, model, id
-00004760: 735b 305d 2c20 7661 6c73 290a 2020 2020  s[0], vals).    
-00004770: 6966 2074 7279 5f61 6761 696e 3a0a 2020  if try_again:.  
-00004780: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00004790: 2020 2020 2020 2074 7279 5f61 6761 696e         try_again
-000047a0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-000047b0: 2020 2020 2063 6c6f 646f 6f2e 7772 6974       clodoo.writ
-000047c0: 654c 3828 6374 782c 206d 6f64 656c 2c20  eL8(ctx, model, 
-000047d0: 6964 732c 2076 616c 7329 0a20 2020 2020  ids, vals).     
-000047e0: 2020 2065 7863 6570 7420 494f 4572 726f     except IOErro
-000047f0: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
-00004800: 2020 2020 6f73 302e 776c 6f67 2827 2573      os0.wlog('%s
-00004810: 2045 7272 6f72 2077 7269 7469 6e67 2072   Error writing r
-00004820: 6563 6f72 6420 2564 206f 6620 2573 2720  ecord %d of %s' 
-00004830: 2520 2865 2c20 7372 635f 6964 2c20 6d6f  % (e, src_id, mo
-00004840: 6465 6c29 290a 2020 2020 2020 2020 2020  del)).          
-00004850: 2020 6d61 6e61 6765 5f65 7272 6f72 2829    manage_error()
-00004860: 0a0a 0a64 6566 2063 7265 6174 655f 7769  ...def create_wi
-00004870: 7468 5f69 6428 6374 782c 206d 6f64 656c  th_id(ctx, model
-00004880: 2c20 6964 2c20 7661 6c73 293a 0a20 2020  , id, vals):.   
-00004890: 2076 616c 7320 3d20 7765 705f 6669 656c   vals = wep_fiel
-000048a0: 6473 2863 7478 2c20 7661 6c73 290a 2020  ds(ctx, vals).  
-000048b0: 2020 6c61 7374 5f69 6420 3d20 300a 2020    last_id = 0.  
-000048c0: 2020 7371 6c5f 6c61 7374 203d 2027 270a    sql_last = ''.
-000048d0: 2020 2020 7371 6c5f 7365 7120 3d20 2727      sql_seq = ''
-000048e0: 0a20 2020 2069 6620 6374 785b 275f 6372  .    if ctx['_cr
-000048f0: 275d 3a0a 2020 2020 2020 2020 7461 626c  ']:.        tabl
-00004900: 6520 3d20 2725 735f 6964 5f73 6571 2720  e = '%s_id_seq' 
-00004910: 2520 6d6f 6465 6c0a 2020 2020 2020 2020  % model.        
-00004920: 7461 626c 6520 3d20 7461 626c 652e 7265  table = table.re
-00004930: 706c 6163 6528 272e 272c 2027 5f27 290a  place('.', '_').
-00004940: 2020 2020 2020 2020 7371 6c5f 6c61 7374          sql_last
-00004950: 203d 2027 7365 6c65 6374 206c 6173 745f   = 'select last_
-00004960: 7661 6c75 6520 6672 6f6d 2025 733b 2720  value from %s;' 
-00004970: 2520 7461 626c 650a 2020 2020 2020 2020  % table.        
-00004980: 726f 7773 203d 2065 7865 635f 7371 6c28  rows = exec_sql(
-00004990: 6374 782c 2073 716c 5f6c 6173 742c 2072  ctx, sql_last, r
-000049a0: 6573 706f 6e73 653d 5472 7565 290a 2020  esponse=True).  
-000049b0: 2020 2020 2020 6c61 7374 5f69 6420 3d20        last_id = 
-000049c0: 726f 7773 5b30 5d5b 305d 0a20 2020 2020  rows[0][0].     
-000049d0: 2020 2069 6620 6964 203e 2030 3a0a 2020     if id > 0:.  
-000049e0: 2020 2020 2020 2020 2020 6966 206c 6173            if las
-000049f0: 745f 6964 2021 3d20 6964 3a0a 2020 2020  t_id != id:.    
-00004a00: 2020 2020 2020 2020 2020 2020 7371 6c5f              sql_
-00004a10: 7365 7120 3d20 2761 6c74 6572 2073 6571  seq = 'alter seq
-00004a20: 7565 6e63 6520 2573 2072 6573 7461 7274  uence %s restart
-00004a30: 2025 643b 2720 2520 2874 6162 6c65 2c20   %d;' % (table, 
-00004a40: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
-00004a50: 2020 2020 6578 6563 5f73 716c 2863 7478      exec_sql(ctx
-00004a60: 2c20 7371 6c5f 7365 7129 0a20 2020 2074  , sql_seq).    t
-00004a70: 7279 5f61 6761 696e 203d 2046 616c 7365  ry_again = False
-00004a80: 0a20 2020 206e 6577 5f69 6420 3d20 300a  .    new_id = 0.
-00004a90: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00004aa0: 206e 6577 5f69 6420 3d20 636c 6f64 6f6f   new_id = clodoo
-00004ab0: 2e63 7265 6174 654c 3828 6374 782c 206d  .createL8(ctx, m
-00004ac0: 6f64 656c 2c20 7661 6c73 290a 2020 2020  odel, vals).    
-00004ad0: 6578 6365 7074 2049 4f45 7272 6f72 3a0a  except IOError:.
-00004ae0: 2020 2020 2020 2020 7472 795f 6167 6169          try_agai
-00004af0: 6e20 3d20 5472 7565 0a20 2020 2020 2020  n = True.       
-00004b00: 2064 726f 705f 6f75 745f 6f72 6967 696e   drop_out_origin
-00004b10: 616c 7328 6374 782c 206d 6f64 656c 2c20  als(ctx, model, 
-00004b20: 6964 2c20 7661 6c73 290a 2020 2020 6966  id, vals).    if
-00004b30: 2074 7279 5f61 6761 696e 3a0a 2020 2020   try_again:.    
-00004b40: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00004b50: 2020 2020 2074 7279 5f61 6761 696e 203d       try_again =
-00004b60: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00004b70: 2020 2069 6620 7371 6c5f 7365 713a 0a20     if sql_seq:. 
-00004b80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00004b90: 7865 635f 7371 6c28 6374 782c 2073 716c  xec_sql(ctx, sql
-00004ba0: 5f73 6571 290a 2020 2020 2020 2020 2020  _seq).          
-00004bb0: 2020 6e65 775f 6964 203d 2063 6c6f 646f    new_id = clodo
-00004bc0: 6f2e 6372 6561 7465 4c38 2863 7478 2c20  o.createL8(ctx, 
-00004bd0: 6d6f 6465 6c2c 2076 616c 7329 0a20 2020  model, vals).   
-00004be0: 2020 2020 2065 7863 6570 7420 494f 4572       except IOEr
-00004bf0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
-00004c00: 2074 7279 5f61 6761 696e 2c20 7661 6c73   try_again, vals
-00004c10: 203d 2073 6574 5f74 6d70 5f6b 6579 7328   = set_tmp_keys(
-00004c20: 6374 782c 206d 6f64 656c 2c20 6964 2c20  ctx, model, id, 
-00004c30: 7661 6c73 290a 2020 2020 6966 2074 7279  vals).    if try
-00004c40: 5f61 6761 696e 3a0a 2020 2020 2020 2020  _again:.        
-00004c50: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00004c60: 2074 7279 5f61 6761 696e 203d 2046 616c   try_again = Fal
-00004c70: 7365 0a20 2020 2020 2020 2020 2020 2069  se.            i
-00004c80: 6620 7371 6c5f 7365 713a 0a20 2020 2020  f sql_seq:.     
-00004c90: 2020 2020 2020 2020 2020 2065 7865 635f             exec_
-00004ca0: 7371 6c28 6374 782c 2073 716c 5f73 6571  sql(ctx, sql_seq
-00004cb0: 290a 2020 2020 2020 2020 2020 2020 6e65  ).            ne
-00004cc0: 775f 6964 203d 2063 6c6f 646f 6f2e 6372  w_id = clodoo.cr
-00004cd0: 6561 7465 4c38 2863 7478 2c20 6d6f 6465  eateL8(ctx, mode
-00004ce0: 6c2c 2076 616c 7329 0a20 2020 2020 2020  l, vals).       
-00004cf0: 2065 7863 6570 7420 494f 4572 726f 723a   except IOError:
-00004d00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00004d10: 6374 785b 275f 6372 275d 3a0a 2020 2020  ctx['_cr']:.    
-00004d20: 2020 2020 2020 2020 2020 2020 7472 795f              try_
-00004d30: 6167 6169 6e20 3d20 5472 7565 0a20 2020  again = True.   
-00004d40: 2020 2020 2020 2020 2020 2020 2074 6162               tab
-00004d50: 6c65 203d 2027 2573 2720 2520 6d6f 6465  le = '%s' % mode
-00004d60: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
-00004d70: 2020 7461 626c 6520 3d20 7461 626c 652e    table = table.
-00004d80: 7265 706c 6163 6528 272e 272c 2027 5f27  replace('.', '_'
-00004d90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004da0: 2020 7371 6c5f 6465 6c20 3d20 2764 656c    sql_del = 'del
-00004db0: 6574 6520 6672 6f6d 2025 7320 7768 6572  ete from %s wher
-00004dc0: 6520 6964 3d25 733b 2720 2520 2874 6162  e id=%s;' % (tab
-00004dd0: 6c65 2c20 6964 290a 2020 2020 2020 2020  le, id).        
-00004de0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e00: 2063 7478 5b27 5f63 7227 5d2e 6578 6563   ctx['_cr'].exec
-00004e10: 7574 6528 7371 6c5f 6465 6c29 0a20 2020  ute(sql_del).   
-00004e20: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00004e30: 6570 7420 4261 7365 4578 6365 7074 696f  ept BaseExceptio
-00004e40: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
-00004e50: 2020 2020 2020 2074 7279 5f61 6761 696e         try_again
-00004e60: 203d 2046 616c 7365 0a20 2020 2069 6620   = False.    if 
-00004e70: 7472 795f 6167 6169 6e3a 0a20 2020 2020  try_again:.     
-00004e80: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00004e90: 2020 2020 6966 2073 716c 5f73 6571 3a0a      if sql_seq:.
-00004ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004eb0: 6578 6563 5f73 716c 2863 7478 2c20 7371  exec_sql(ctx, sq
-00004ec0: 6c5f 7365 7129 0a20 2020 2020 2020 2020  l_seq).         
-00004ed0: 2020 206e 6577 5f69 6420 3d20 636c 6f64     new_id = clod
-00004ee0: 6f6f 2e63 7265 6174 654c 3828 6374 782c  oo.createL8(ctx,
-00004ef0: 206d 6f64 656c 2c20 7661 6c73 290a 2020   model, vals).  
-00004f00: 2020 2020 2020 6578 6365 7074 2049 4f45        except IOE
-00004f10: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
-00004f20: 2020 6f73 302e 776c 6f67 2827 4572 726f    os0.wlog('Erro
-00004f30: 7220 6372 6561 7469 6e67 2072 6563 6f72  r creating recor
-00004f40: 6420 2564 206f 6620 2573 2720 2520 2869  d %d of %s' % (i
-00004f50: 642c 206d 6f64 656c 2929 0a20 2020 2020  d, model)).     
-00004f60: 2020 2020 2020 206d 616e 6167 655f 6572         manage_er
-00004f70: 726f 7228 290a 2020 2020 2020 2020 2020  ror().          
-00004f80: 2020 6e65 775f 6964 203d 2069 640a 2020    new_id = id.  
-00004f90: 2020 6966 206e 6577 5f69 6420 213d 2069    if new_id != i
-00004fa0: 643a 0a20 2020 2020 2020 206f 7330 2e77  d:.        os0.w
-00004fb0: 6c6f 6728 2243 616e 6e6f 7420 6372 6561  log("Cannot crea
-00004fc0: 7465 2072 6563 6f72 6420 2564 206f 6620  te record %d of 
-00004fd0: 2573 2220 2520 2869 642c 206d 6f64 656c  %s" % (id, model
-00004fe0: 2929 0a20 2020 2020 2020 2069 6620 6e6f  )).        if no
-00004ff0: 7420 6374 785b 2761 7373 756d 655f 7965  t ctx['assume_ye
-00005000: 7327 5d3a 0a20 2020 2020 2020 2020 2020  s']:.           
-00005010: 2069 6e70 7574 2827 5072 6573 7320 5245   input('Press RE
-00005020: 5420 746f 2063 6f6e 7469 6e75 6527 290a  T to continue').
-00005030: 2020 2020 6966 206c 6173 745f 6964 2061      if last_id a
-00005040: 6e64 206c 6173 745f 6964 203e 2031 2061  nd last_id > 1 a
-00005050: 6e64 206c 6173 745f 6964 203e 2069 643a  nd last_id > id:
-00005060: 0a20 2020 2020 2020 2073 716c 203d 2027  .        sql = '
-00005070: 616c 7465 7220 7365 7175 656e 6365 2025  alter sequence %
-00005080: 7320 7265 7374 6172 7420 2564 3b27 2025  s restart %d;' %
-00005090: 2028 7461 626c 652c 206c 6173 745f 6964   (table, last_id
-000050a0: 290a 2020 2020 2020 2020 6578 6563 5f73  ).        exec_s
-000050b0: 716c 2863 7478 2c20 7371 6c29 0a0a 0a64  ql(ctx, sql)...d
-000050c0: 6566 2069 6e73 7461 6c6c 5f6d 6f64 756c  ef install_modul
-000050d0: 6573 2874 6774 5f63 7478 2c20 7372 635f  es(tgt_ctx, src_
-000050e0: 6374 7829 3a0a 2020 2020 6173 7375 6d65  ctx):.    assume
-000050f0: 5f79 6573 203d 2074 6774 5f63 7478 5b27  _yes = tgt_ctx['
-00005100: 6173 7375 6d65 5f79 6573 275d 0a20 2020  assume_yes'].   
-00005110: 2075 7067 7261 6465 203d 2046 616c 7365   upgrade = False
-00005120: 0a20 2020 2069 6620 6e6f 7420 7467 745f  .    if not tgt_
-00005130: 6374 785b 2761 7373 756d 655f 7965 7327  ctx['assume_yes'
-00005140: 5d3a 0a20 2020 2020 2020 2064 756d 6d79  ]:.        dummy
-00005150: 203d 2069 6e70 7574 2827 496e 7374 616c   = input('Instal
-00005160: 6c20 6d6f 6475 6c65 7320 2859 6573 2c4e  l modules (Yes,N
-00005170: 6f2c 416c 6c29 3f20 2729 0a20 2020 2020  o,All)? ').     
-00005180: 2020 2069 6620 6475 6d6d 795b 305d 2069     if dummy[0] i
-00005190: 6e20 2827 6e27 2c20 274e 2729 3a0a 2020  n ('n', 'N'):.  
-000051a0: 2020 2020 2020 2020 2020 6173 7375 6d65            assume
-000051b0: 5f79 6573 203d 2027 4e27 0a20 2020 2020  _yes = 'N'.     
-000051c0: 2020 2069 6620 6475 6d6d 795b 305d 2069     if dummy[0] i
-000051d0: 6e20 2827 6127 2c20 2741 2729 3a0a 2020  n ('a', 'A'):.  
-000051e0: 2020 2020 2020 2020 2020 6173 7375 6d65            assume
-000051f0: 5f79 6573 203d 2027 5927 0a20 2020 2020  _yes = 'Y'.     
-00005200: 2020 2064 756d 6d79 203d 2069 6e70 7574     dummy = input
-00005210: 2827 5570 6772 6164 6520 696e 7374 616c  ('Upgrade instal
-00005220: 6c65 6420 6d6f 6475 6c65 7320 2859 6573  led modules (Yes
-00005230: 2c4e 6f29 3f20 2729 0a20 2020 2020 2020  ,No)? ').       
-00005240: 2069 6620 6475 6d6d 795b 305d 2069 6e20   if dummy[0] in 
-00005250: 2827 7927 2c20 2759 2729 3a0a 2020 2020  ('y', 'Y'):.    
-00005260: 2020 2020 2020 2020 7570 6772 6164 6520          upgrade 
-00005270: 3d20 5472 7565 0a20 2020 2020 2020 2069  = True.        i
-00005280: 6620 6173 7375 6d65 5f79 6573 203d 3d20  f assume_yes == 
-00005290: 274e 2720 616e 6420 6e6f 7420 7570 6772  'N' and not upgr
-000052a0: 6164 653a 0a20 2020 2020 2020 2020 2020  ade:.           
-000052b0: 2072 6574 7572 6e0a 2020 2020 6d6f 6465   return.    mode
-000052c0: 6c20 3d20 2769 722e 6d6f 6475 6c65 2e6d  l = 'ir.module.m
-000052d0: 6f64 756c 6527 0a20 2020 2066 6f72 206d  odule'.    for m
-000052e0: 6f64 756c 655f 7372 6320 696e 2063 6c6f  odule_src in clo
-000052f0: 646f 6f2e 6272 6f77 7365 4c38 2873 7263  doo.browseL8(src
-00005300: 5f63 7478 2c20 6d6f 6465 6c2c 0a20 2020  _ctx, model,.   
-00005310: 2020 2020 2020 2020 2063 6c6f 646f 6f2e           clodoo.
-00005320: 7365 6172 6368 4c38 2873 7263 5f63 7478  searchL8(src_ctx
-00005330: 2c20 6d6f 6465 6c2c 205b 2827 7374 6174  , model, [('stat
-00005340: 6527 2c20 273d 272c 2027 696e 7374 616c  e', '=', 'instal
-00005350: 6c65 6427 295d 2929 3a0a 2020 2020 2020  led')])):.      
-00005360: 2020 6f6c 645f 6d6f 6475 6c65 203d 206d    old_module = m
-00005370: 6f64 756c 655f 7372 632e 6e61 6d65 0a20  odule_src.name. 
-00005380: 2020 2020 2020 206d 6f64 756c 6520 3d20         module = 
-00005390: 7472 616e 736f 646f 6f2e 7472 616e 736c  transodoo.transl
-000053a0: 6174 655f 6672 6f6d 5f74 6f28 7372 635f  ate_from_to(src_
-000053b0: 6374 782c 0a20 2020 2020 2020 2020 2020  ctx,.           
-000053c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053e0: 2020 2769 722e 6d6f 6475 6c65 2e6d 6f64    'ir.module.mod
-000053f0: 756c 6527 2c0a 2020 2020 2020 2020 2020  ule',.          
-00005400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005420: 2020 206f 6c64 5f6d 6f64 756c 652c 0a20     old_module,. 
-00005430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005450: 2020 2020 2020 2020 2020 2020 7372 635f              src_
-00005460: 6374 785b 276f 655f 7665 7273 696f 6e27  ctx['oe_version'
-00005470: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00005480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054a0: 7467 745f 6374 785b 276f 655f 7665 7273  tgt_ctx['oe_vers
-000054b0: 696f 6e27 5d2c 0a20 2020 2020 2020 2020  ion'],.         
-000054c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054e0: 2020 2020 7479 7065 3d27 6d6f 6475 6c65      type='module
-000054f0: 2729 0a20 2020 2020 2020 2069 6620 6d6f  ').        if mo
-00005500: 6475 6c65 203d 3d20 6f6c 645f 6d6f 6475  dule == old_modu
-00005510: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-00005520: 6d6f 6475 6c65 203d 2074 7261 6e73 6f64  module = transod
-00005530: 6f6f 2e74 7261 6e73 6c61 7465 5f66 726f  oo.translate_fro
-00005540: 6d5f 746f 2873 7263 5f63 7478 2c0a 2020  m_to(src_ctx,.  
-00005550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005570: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00005580: 6972 2e6d 6f64 756c 652e 6d6f 6475 6c65  ir.module.module
-00005590: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00004160: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00004170: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00004180: 7420 4261 7365 4578 6365 7074 696f 6e3a  t BaseException:
+00004190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000041a0: 2020 2020 2020 2020 2070 6173 730a 0a20           pass.. 
+000041b0: 2020 2069 6620 2763 6f64 6527 2069 6e20     if 'code' in 
+000041c0: 7661 6c73 3a0a 2020 2020 2020 2020 6472  vals:.        dr
+000041d0: 6f70 5f6f 7574 5f6f 7269 6769 6e61 6c5f  op_out_original_
+000041e0: 6669 656c 6428 6374 782c 206d 6f64 656c  field(ctx, model
+000041f0: 2c20 6964 2c20 7661 6c73 2c20 2763 6f64  , id, vals, 'cod
+00004200: 6527 290a 2020 2020 6966 2027 6e61 6d65  e').    if 'name
+00004210: 2720 696e 2076 616c 733a 0a20 2020 2020  ' in vals:.     
+00004220: 2020 2064 726f 705f 6f75 745f 6f72 6967     drop_out_orig
+00004230: 696e 616c 5f66 6965 6c64 2863 7478 2c20  inal_field(ctx, 
+00004240: 6d6f 6465 6c2c 2069 642c 2076 616c 732c  model, id, vals,
+00004250: 2027 6e61 6d65 2729 0a0a 0a64 6566 2077   'name')...def w
+00004260: 6570 5f66 6965 6c64 7328 6374 782c 2076  ep_fields(ctx, v
+00004270: 616c 7329 3a0a 2020 2020 666f 7220 6e6d  als):.    for nm
+00004280: 2069 6e20 280a 2020 2020 2020 2020 2763   in (.        'c
+00004290: 7265 6174 655f 6461 7465 272c 0a20 2020  reate_date',.   
+000042a0: 2020 2020 2027 6372 6561 7465 5f75 6964       'create_uid
+000042b0: 272c 0a20 2020 2020 2020 2027 6964 272c  ',.        'id',
+000042c0: 0a20 2020 2020 2020 2027 6d65 7373 6167  .        'messag
+000042d0: 655f 6368 616e 6e65 6c5f 6964 7327 2c0a  e_channel_ids',.
+000042e0: 2020 2020 2020 2020 276d 6573 7361 6765          'message
+000042f0: 5f66 6f6c 6c6f 7765 725f 6964 7327 2c0a  _follower_ids',.
+00004300: 2020 2020 2020 2020 276d 6573 7361 6765          'message
+00004310: 5f69 6473 272c 0a20 2020 2020 2020 2027  _ids',.        '
+00004320: 6d65 7373 6167 655f 6973 5f66 6f6c 6c6f  message_is_follo
+00004330: 7765 7227 2c0a 2020 2020 2020 2020 276d  wer',.        'm
+00004340: 6573 7361 6765 5f6c 6173 745f 706f 7374  essage_last_post
+00004350: 272c 0a20 2020 2020 2020 2027 6d65 7373  ',.        'mess
+00004360: 6167 655f 6e65 6564 6163 7469 6f6e 272c  age_needaction',
+00004370: 0a20 2020 2020 2020 2027 6d65 7373 6167  .        'messag
+00004380: 655f 6e65 6564 6163 7469 6f6e 5f63 6f75  e_needaction_cou
+00004390: 6e74 6572 272c 0a20 2020 2020 2020 2027  nter',.        '
+000043a0: 6d65 7373 6167 655f 756e 7265 6164 272c  message_unread',
+000043b0: 0a20 2020 2020 2020 2027 6d65 7373 6167  .        'messag
+000043c0: 655f 756e 7265 6164 5f63 6f75 6e74 6572  e_unread_counter
+000043d0: 272c 0a20 2020 2020 2020 2027 7772 6974  ',.        'writ
+000043e0: 655f 6461 7465 272c 0a20 2020 2020 2020  e_date',.       
+000043f0: 2027 7772 6974 655f 7569 6427 2c0a 2020   'write_uid',.  
+00004400: 2020 293a 0a20 2020 2020 2020 2069 6620    ):.        if 
+00004410: 6e6d 2069 6e20 7661 6c73 3a0a 2020 2020  nm in vals:.    
+00004420: 2020 2020 2020 2020 6465 6c20 7661 6c73          del vals
+00004430: 5b6e 6d5d 0a20 2020 2072 6574 7572 6e20  [nm].    return 
+00004440: 7661 6c73 0a0a 0a64 6566 2077 7269 7465  vals...def write
+00004450: 5f6e 6f5f 6475 7028 6374 782c 206d 6f64  _no_dup(ctx, mod
+00004460: 656c 2c20 6964 732c 2076 616c 732c 2073  el, ids, vals, s
+00004470: 7263 5f69 6429 3a0a 2020 2020 7661 6c73  rc_id):.    vals
+00004480: 203d 2077 6570 5f66 6965 6c64 7328 6374   = wep_fields(ct
+00004490: 782c 2076 616c 7329 0a20 2020 2074 7279  x, vals).    try
+000044a0: 5f61 6761 696e 203d 2046 616c 7365 0a20  _again = False. 
+000044b0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+000044c0: 636c 6f64 6f6f 2e77 7269 7465 4c38 2863  clodoo.writeL8(c
+000044d0: 7478 2c20 6d6f 6465 6c2c 2069 6473 2c20  tx, model, ids, 
+000044e0: 7661 6c73 290a 2020 2020 6578 6365 7074  vals).    except
+000044f0: 2049 4f45 7272 6f72 3a0a 2020 2020 2020   IOError:.      
+00004500: 2020 7472 795f 6167 6169 6e20 3d20 5472    try_again = Tr
+00004510: 7565 0a20 2020 2020 2020 2064 726f 705f  ue.        drop_
+00004520: 6f75 745f 6f72 6967 696e 616c 7328 6374  out_originals(ct
+00004530: 782c 206d 6f64 656c 2c20 6964 735b 305d  x, model, ids[0]
+00004540: 2c20 7661 6c73 290a 2020 2020 6966 2074  , vals).    if t
+00004550: 7279 5f61 6761 696e 3a0a 2020 2020 2020  ry_again:.      
+00004560: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00004570: 2020 2074 7279 5f61 6761 696e 203d 2046     try_again = F
+00004580: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+00004590: 2063 6c6f 646f 6f2e 7772 6974 654c 3828   clodoo.writeL8(
+000045a0: 6374 782c 206d 6f64 656c 2c20 6964 732c  ctx, model, ids,
+000045b0: 2076 616c 7329 0a20 2020 2020 2020 2065   vals).        e
+000045c0: 7863 6570 7420 494f 4572 726f 723a 0a20  xcept IOError:. 
+000045d0: 2020 2020 2020 2020 2020 2074 7279 5f61             try_a
+000045e0: 6761 696e 2c20 7661 6c73 203d 2073 6574  gain, vals = set
+000045f0: 5f74 6d70 5f6b 6579 7328 6374 782c 206d  _tmp_keys(ctx, m
+00004600: 6f64 656c 2c20 6964 735b 305d 2c20 7661  odel, ids[0], va
+00004610: 6c73 290a 2020 2020 6966 2074 7279 5f61  ls).    if try_a
+00004620: 6761 696e 3a0a 2020 2020 2020 2020 7472  gain:.        tr
+00004630: 793a 0a20 2020 2020 2020 2020 2020 2074  y:.            t
+00004640: 7279 5f61 6761 696e 203d 2046 616c 7365  ry_again = False
+00004650: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
+00004660: 646f 6f2e 7772 6974 654c 3828 6374 782c  doo.writeL8(ctx,
+00004670: 206d 6f64 656c 2c20 6964 732c 2076 616c   model, ids, val
+00004680: 7329 0a20 2020 2020 2020 2065 7863 6570  s).        excep
+00004690: 7420 494f 4572 726f 7220 6173 2065 3a0a  t IOError as e:.
+000046a0: 2020 2020 2020 2020 2020 2020 6f73 302e              os0.
+000046b0: 776c 6f67 2827 2573 2045 7272 6f72 2077  wlog('%s Error w
+000046c0: 7269 7469 6e67 2072 6563 6f72 6420 2564  riting record %d
+000046d0: 206f 6620 2573 2720 2520 2865 2c20 7372   of %s' % (e, sr
+000046e0: 635f 6964 2c20 6d6f 6465 6c29 290a 2020  c_id, model)).  
+000046f0: 2020 2020 2020 2020 2020 6d61 6e61 6765            manage
+00004700: 5f65 7272 6f72 2829 0a0a 0a64 6566 2063  _error()...def c
+00004710: 7265 6174 655f 7769 7468 5f69 6428 6374  reate_with_id(ct
+00004720: 782c 206d 6f64 656c 2c20 6964 2c20 7661  x, model, id, va
+00004730: 6c73 293a 0a20 2020 2076 616c 7320 3d20  ls):.    vals = 
+00004740: 7765 705f 6669 656c 6473 2863 7478 2c20  wep_fields(ctx, 
+00004750: 7661 6c73 290a 2020 2020 6c61 7374 5f69  vals).    last_i
+00004760: 6420 3d20 300a 2020 2020 7371 6c5f 6c61  d = 0.    sql_la
+00004770: 7374 203d 2027 270a 2020 2020 7371 6c5f  st = ''.    sql_
+00004780: 7365 7120 3d20 2727 0a20 2020 2069 6620  seq = ''.    if 
+00004790: 6374 785b 275f 6372 275d 3a0a 2020 2020  ctx['_cr']:.    
+000047a0: 2020 2020 7461 626c 6520 3d20 2725 735f      table = '%s_
+000047b0: 6964 5f73 6571 2720 2520 6d6f 6465 6c0a  id_seq' % model.
+000047c0: 2020 2020 2020 2020 7461 626c 6520 3d20          table = 
+000047d0: 7461 626c 652e 7265 706c 6163 6528 272e  table.replace('.
+000047e0: 272c 2027 5f27 290a 2020 2020 2020 2020  ', '_').        
+000047f0: 7371 6c5f 6c61 7374 203d 2027 7365 6c65  sql_last = 'sele
+00004800: 6374 206c 6173 745f 7661 6c75 6520 6672  ct last_value fr
+00004810: 6f6d 2025 733b 2720 2520 7461 626c 650a  om %s;' % table.
+00004820: 2020 2020 2020 2020 726f 7773 203d 2065          rows = e
+00004830: 7865 635f 7371 6c28 6374 782c 2073 716c  xec_sql(ctx, sql
+00004840: 5f6c 6173 742c 2072 6573 706f 6e73 653d  _last, response=
+00004850: 5472 7565 290a 2020 2020 2020 2020 6c61  True).        la
+00004860: 7374 5f69 6420 3d20 726f 7773 5b30 5d5b  st_id = rows[0][
+00004870: 305d 0a20 2020 2020 2020 2069 6620 6964  0].        if id
+00004880: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+00004890: 2020 6966 206c 6173 745f 6964 2021 3d20    if last_id != 
+000048a0: 6964 3a0a 2020 2020 2020 2020 2020 2020  id:.            
+000048b0: 2020 2020 7371 6c5f 7365 7120 3d20 2761      sql_seq = 'a
+000048c0: 6c74 6572 2073 6571 7565 6e63 6520 2573  lter sequence %s
+000048d0: 2072 6573 7461 7274 2025 643b 2720 2520   restart %d;' % 
+000048e0: 2874 6162 6c65 2c20 6964 290a 2020 2020  (table, id).    
+000048f0: 2020 2020 2020 2020 2020 2020 6578 6563              exec
+00004900: 5f73 716c 2863 7478 2c20 7371 6c5f 7365  _sql(ctx, sql_se
+00004910: 7129 0a20 2020 2074 7279 5f61 6761 696e  q).    try_again
+00004920: 203d 2046 616c 7365 0a20 2020 206e 6577   = False.    new
+00004930: 5f69 6420 3d20 300a 2020 2020 7472 793a  _id = 0.    try:
+00004940: 0a20 2020 2020 2020 206e 6577 5f69 6420  .        new_id 
+00004950: 3d20 636c 6f64 6f6f 2e63 7265 6174 654c  = clodoo.createL
+00004960: 3828 6374 782c 206d 6f64 656c 2c20 7661  8(ctx, model, va
+00004970: 6c73 290a 2020 2020 6578 6365 7074 2049  ls).    except I
+00004980: 4f45 7272 6f72 3a0a 2020 2020 2020 2020  OError:.        
+00004990: 7472 795f 6167 6169 6e20 3d20 5472 7565  try_again = True
+000049a0: 0a20 2020 2020 2020 2064 726f 705f 6f75  .        drop_ou
+000049b0: 745f 6f72 6967 696e 616c 7328 6374 782c  t_originals(ctx,
+000049c0: 206d 6f64 656c 2c20 6964 2c20 7661 6c73   model, id, vals
+000049d0: 290a 2020 2020 6966 2074 7279 5f61 6761  ).    if try_aga
+000049e0: 696e 3a0a 2020 2020 2020 2020 7472 793a  in:.        try:
+000049f0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00004a00: 5f61 6761 696e 203d 2046 616c 7365 0a20  _again = False. 
+00004a10: 2020 2020 2020 2020 2020 2069 6620 7371             if sq
+00004a20: 6c5f 7365 713a 0a20 2020 2020 2020 2020  l_seq:.         
+00004a30: 2020 2020 2020 2065 7865 635f 7371 6c28         exec_sql(
+00004a40: 6374 782c 2073 716c 5f73 6571 290a 2020  ctx, sql_seq).  
+00004a50: 2020 2020 2020 2020 2020 6e65 775f 6964            new_id
+00004a60: 203d 2063 6c6f 646f 6f2e 6372 6561 7465   = clodoo.create
+00004a70: 4c38 2863 7478 2c20 6d6f 6465 6c2c 2076  L8(ctx, model, v
+00004a80: 616c 7329 0a20 2020 2020 2020 2065 7863  als).        exc
+00004a90: 6570 7420 494f 4572 726f 723a 0a20 2020  ept IOError:.   
+00004aa0: 2020 2020 2020 2020 2074 7279 5f61 6761           try_aga
+00004ab0: 696e 2c20 7661 6c73 203d 2073 6574 5f74  in, vals = set_t
+00004ac0: 6d70 5f6b 6579 7328 6374 782c 206d 6f64  mp_keys(ctx, mod
+00004ad0: 656c 2c20 6964 2c20 7661 6c73 290a 2020  el, id, vals).  
+00004ae0: 2020 6966 2074 7279 5f61 6761 696e 3a0a    if try_again:.
+00004af0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00004b00: 2020 2020 2020 2020 2074 7279 5f61 6761           try_aga
+00004b10: 696e 203d 2046 616c 7365 0a20 2020 2020  in = False.     
+00004b20: 2020 2020 2020 2069 6620 7371 6c5f 7365         if sql_se
+00004b30: 713a 0a20 2020 2020 2020 2020 2020 2020  q:.             
+00004b40: 2020 2065 7865 635f 7371 6c28 6374 782c     exec_sql(ctx,
+00004b50: 2073 716c 5f73 6571 290a 2020 2020 2020   sql_seq).      
+00004b60: 2020 2020 2020 6e65 775f 6964 203d 2063        new_id = c
+00004b70: 6c6f 646f 6f2e 6372 6561 7465 4c38 2863  lodoo.createL8(c
+00004b80: 7478 2c20 6d6f 6465 6c2c 2076 616c 7329  tx, model, vals)
+00004b90: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+00004ba0: 494f 4572 726f 723a 0a20 2020 2020 2020  IOError:.       
+00004bb0: 2020 2020 2069 6620 6374 785b 275f 6372       if ctx['_cr
+00004bc0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+00004bd0: 2020 2020 7472 795f 6167 6169 6e20 3d20      try_again = 
+00004be0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+00004bf0: 2020 2020 2074 6162 6c65 203d 2027 2573       table = '%s
+00004c00: 2720 2520 6d6f 6465 6c0a 2020 2020 2020  ' % model.      
+00004c10: 2020 2020 2020 2020 2020 7461 626c 6520            table 
+00004c20: 3d20 7461 626c 652e 7265 706c 6163 6528  = table.replace(
+00004c30: 272e 272c 2027 5f27 290a 2020 2020 2020  '.', '_').      
+00004c40: 2020 2020 2020 2020 2020 7371 6c5f 6465            sql_de
+00004c50: 6c20 3d20 2764 656c 6574 6520 6672 6f6d  l = 'delete from
+00004c60: 2025 7320 7768 6572 6520 6964 3d25 733b   %s where id=%s;
+00004c70: 2720 2520 2874 6162 6c65 2c20 6964 290a  ' % (table, id).
+00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c90: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00004ca0: 2020 2020 2020 2020 2063 7478 5b27 5f63           ctx['_c
+00004cb0: 7227 5d2e 6578 6563 7574 6528 7371 6c5f  r'].execute(sql_
+00004cc0: 6465 6c29 0a20 2020 2020 2020 2020 2020  del).           
+00004cd0: 2020 2020 2065 7863 6570 7420 4261 7365       except Base
+00004ce0: 4578 6365 7074 696f 6e3a 0a20 2020 2020  Exception:.     
+00004cf0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00004d00: 7279 5f61 6761 696e 203d 2046 616c 7365  ry_again = False
+00004d10: 0a20 2020 2069 6620 7472 795f 6167 6169  .    if try_agai
+00004d20: 6e3a 0a20 2020 2020 2020 2074 7279 3a0a  n:.        try:.
+00004d30: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00004d40: 716c 5f73 6571 3a0a 2020 2020 2020 2020  ql_seq:.        
+00004d50: 2020 2020 2020 2020 6578 6563 5f73 716c          exec_sql
+00004d60: 2863 7478 2c20 7371 6c5f 7365 7129 0a20  (ctx, sql_seq). 
+00004d70: 2020 2020 2020 2020 2020 206e 6577 5f69             new_i
+00004d80: 6420 3d20 636c 6f64 6f6f 2e63 7265 6174  d = clodoo.creat
+00004d90: 654c 3828 6374 782c 206d 6f64 656c 2c20  eL8(ctx, model, 
+00004da0: 7661 6c73 290a 2020 2020 2020 2020 6578  vals).        ex
+00004db0: 6365 7074 2049 4f45 7272 6f72 3a0a 2020  cept IOError:.  
+00004dc0: 2020 2020 2020 2020 2020 6f73 302e 776c            os0.wl
+00004dd0: 6f67 2827 4572 726f 7220 6372 6561 7469  og('Error creati
+00004de0: 6e67 2072 6563 6f72 6420 2564 206f 6620  ng record %d of 
+00004df0: 2573 2720 2520 2869 642c 206d 6f64 656c  %s' % (id, model
+00004e00: 2929 0a20 2020 2020 2020 2020 2020 206d  )).            m
+00004e10: 616e 6167 655f 6572 726f 7228 290a 2020  anage_error().  
+00004e20: 2020 2020 2020 2020 2020 6e65 775f 6964            new_id
+00004e30: 203d 2069 640a 2020 2020 6966 206e 6577   = id.    if new
+00004e40: 5f69 6420 213d 2069 643a 0a20 2020 2020  _id != id:.     
+00004e50: 2020 206f 7330 2e77 6c6f 6728 2243 616e     os0.wlog("Can
+00004e60: 6e6f 7420 6372 6561 7465 2072 6563 6f72  not create recor
+00004e70: 6420 2564 206f 6620 2573 2220 2520 2869  d %d of %s" % (i
+00004e80: 642c 206d 6f64 656c 2929 0a20 2020 2020  d, model)).     
+00004e90: 2020 2069 6620 6e6f 7420 6374 785b 2761     if not ctx['a
+00004ea0: 7373 756d 655f 7965 7327 5d3a 0a20 2020  ssume_yes']:.   
+00004eb0: 2020 2020 2020 2020 2069 6e70 7574 2827           input('
+00004ec0: 5072 6573 7320 5245 5420 746f 2063 6f6e  Press RET to con
+00004ed0: 7469 6e75 6527 290a 2020 2020 6966 206c  tinue').    if l
+00004ee0: 6173 745f 6964 2061 6e64 206c 6173 745f  ast_id and last_
+00004ef0: 6964 203e 2031 2061 6e64 206c 6173 745f  id > 1 and last_
+00004f00: 6964 203e 2069 643a 0a20 2020 2020 2020  id > id:.       
+00004f10: 2073 716c 203d 2027 616c 7465 7220 7365   sql = 'alter se
+00004f20: 7175 656e 6365 2025 7320 7265 7374 6172  quence %s restar
+00004f30: 7420 2564 3b27 2025 2028 7461 626c 652c  t %d;' % (table,
+00004f40: 206c 6173 745f 6964 290a 2020 2020 2020   last_id).      
+00004f50: 2020 6578 6563 5f73 716c 2863 7478 2c20    exec_sql(ctx, 
+00004f60: 7371 6c29 0a0a 0a64 6566 2069 6e73 7461  sql)...def insta
+00004f70: 6c6c 5f6d 6f64 756c 6573 2874 6774 5f63  ll_modules(tgt_c
+00004f80: 7478 2c20 7372 635f 6374 7829 3a0a 2020  tx, src_ctx):.  
+00004f90: 2020 6173 7375 6d65 5f79 6573 203d 2074    assume_yes = t
+00004fa0: 6774 5f63 7478 5b27 6173 7375 6d65 5f79  gt_ctx['assume_y
+00004fb0: 6573 275d 0a20 2020 2075 7067 7261 6465  es'].    upgrade
+00004fc0: 203d 2046 616c 7365 0a20 2020 2069 6620   = False.    if 
+00004fd0: 6e6f 7420 7467 745f 6374 785b 2761 7373  not tgt_ctx['ass
+00004fe0: 756d 655f 7965 7327 5d3a 0a20 2020 2020  ume_yes']:.     
+00004ff0: 2020 2064 756d 6d79 203d 2069 6e70 7574     dummy = input
+00005000: 2827 496e 7374 616c 6c20 6d6f 6475 6c65  ('Install module
+00005010: 7320 2859 6573 2c4e 6f2c 416c 6c29 3f20  s (Yes,No,All)? 
+00005020: 2729 0a20 2020 2020 2020 2069 6620 6475  ').        if du
+00005030: 6d6d 795b 305d 2069 6e20 2827 6e27 2c20  mmy[0] in ('n', 
+00005040: 274e 2729 3a0a 2020 2020 2020 2020 2020  'N'):.          
+00005050: 2020 6173 7375 6d65 5f79 6573 203d 2027    assume_yes = '
+00005060: 4e27 0a20 2020 2020 2020 2069 6620 6475  N'.        if du
+00005070: 6d6d 795b 305d 2069 6e20 2827 6127 2c20  mmy[0] in ('a', 
+00005080: 2741 2729 3a0a 2020 2020 2020 2020 2020  'A'):.          
+00005090: 2020 6173 7375 6d65 5f79 6573 203d 2027    assume_yes = '
+000050a0: 5927 0a20 2020 2020 2020 2064 756d 6d79  Y'.        dummy
+000050b0: 203d 2069 6e70 7574 2827 5570 6772 6164   = input('Upgrad
+000050c0: 6520 696e 7374 616c 6c65 6420 6d6f 6475  e installed modu
+000050d0: 6c65 7320 2859 6573 2c4e 6f29 3f20 2729  les (Yes,No)? ')
+000050e0: 0a20 2020 2020 2020 2069 6620 6475 6d6d  .        if dumm
+000050f0: 795b 305d 2069 6e20 2827 7927 2c20 2759  y[0] in ('y', 'Y
+00005100: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+00005110: 7570 6772 6164 6520 3d20 5472 7565 0a20  upgrade = True. 
+00005120: 2020 2020 2020 2069 6620 6173 7375 6d65         if assume
+00005130: 5f79 6573 203d 3d20 274e 2720 616e 6420  _yes == 'N' and 
+00005140: 6e6f 7420 7570 6772 6164 653a 0a20 2020  not upgrade:.   
+00005150: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00005160: 2020 2020 6d6f 6465 6c20 3d20 2769 722e      model = 'ir.
+00005170: 6d6f 6475 6c65 2e6d 6f64 756c 6527 0a20  module.module'. 
+00005180: 2020 2066 6f72 206d 6f64 756c 655f 7372     for module_sr
+00005190: 6320 696e 2063 6c6f 646f 6f2e 6272 6f77  c in clodoo.brow
+000051a0: 7365 4c38 280a 2020 2020 2020 2020 7372  seL8(.        sr
+000051b0: 635f 6374 782c 206d 6f64 656c 2c20 636c  c_ctx, model, cl
+000051c0: 6f64 6f6f 2e73 6561 7263 684c 3828 7372  odoo.searchL8(sr
+000051d0: 635f 6374 782c 206d 6f64 656c 2c20 5b28  c_ctx, model, [(
+000051e0: 2773 7461 7465 272c 2027 3d27 2c20 2769  'state', '=', 'i
+000051f0: 6e73 7461 6c6c 6564 2729 5d29 0a20 2020  nstalled')]).   
+00005200: 2029 3a0a 2020 2020 2020 2020 6f6c 645f   ):.        old_
+00005210: 6d6f 6475 6c65 203d 206d 6f64 756c 655f  module = module_
+00005220: 7372 632e 6e61 6d65 0a20 2020 2020 2020  src.name.       
+00005230: 206d 6f64 756c 6520 3d20 7472 616e 736f   module = transo
+00005240: 646f 6f2e 7472 616e 736c 6174 655f 6672  doo.translate_fr
+00005250: 6f6d 5f74 6f28 0a20 2020 2020 2020 2020  om_to(.         
+00005260: 2020 2073 7263 5f63 7478 2c0a 2020 2020     src_ctx,.    
+00005270: 2020 2020 2020 2020 2769 722e 6d6f 6475          'ir.modu
+00005280: 6c65 2e6d 6f64 756c 6527 2c0a 2020 2020  le.module',.    
+00005290: 2020 2020 2020 2020 6f6c 645f 6d6f 6475          old_modu
+000052a0: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
+000052b0: 7372 635f 6374 785b 276f 655f 7665 7273  src_ctx['oe_vers
+000052c0: 696f 6e27 5d2c 0a20 2020 2020 2020 2020  ion'],.         
+000052d0: 2020 2074 6774 5f63 7478 5b27 6f65 5f76     tgt_ctx['oe_v
+000052e0: 6572 7369 6f6e 275d 2c0a 2020 2020 2020  ersion'],.      
+000052f0: 2020 2020 2020 7479 7065 3d27 6d6f 6475        type='modu
+00005300: 6c65 272c 0a20 2020 2020 2020 2029 0a20  le',.        ). 
+00005310: 2020 2020 2020 2069 6620 6d6f 6475 6c65         if module
+00005320: 203d 3d20 6f6c 645f 6d6f 6475 6c65 3a0a   == old_module:.
+00005330: 2020 2020 2020 2020 2020 2020 6d6f 6475              modu
+00005340: 6c65 203d 2074 7261 6e73 6f64 6f6f 2e74  le = transodoo.t
+00005350: 7261 6e73 6c61 7465 5f66 726f 6d5f 746f  ranslate_from_to
+00005360: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00005370: 2020 7372 635f 6374 782c 0a20 2020 2020    src_ctx,.     
+00005380: 2020 2020 2020 2020 2020 2027 6972 2e6d             'ir.m
+00005390: 6f64 756c 652e 6d6f 6475 6c65 272c 0a20  odule.module',. 
+000053a0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+000053b0: 6c64 5f6d 6f64 756c 652c 0a20 2020 2020  ld_module,.     
+000053c0: 2020 2020 2020 2020 2020 2073 7263 5f63             src_c
+000053d0: 7478 5b27 6f65 5f76 6572 7369 6f6e 275d  tx['oe_version']
+000053e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000053f0: 2020 7467 745f 6374 785b 276f 655f 7665    tgt_ctx['oe_ve
+00005400: 7273 696f 6e27 5d2c 0a20 2020 2020 2020  rsion'],.       
+00005410: 2020 2020 2020 2020 2074 7970 653d 276d           type='m
+00005420: 6572 6765 272c 0a20 2020 2020 2020 2020  erge',.         
+00005430: 2020 2029 0a20 2020 2020 2020 206d 7367     ).        msg
+00005440: 5f62 7572 7374 2827 416e 616c 797a 696e  _burst('Analyzin
+00005450: 6720 6d6f 6475 6c65 2025 7320 2825 7329  g module %s (%s)
+00005460: 2720 2520 286d 6f64 756c 652c 206f 6c64  ' % (module, old
+00005470: 5f6d 6f64 756c 6529 290a 2020 2020 2020  _module)).      
+00005480: 2020 6966 206e 6f74 2063 6c6f 646f 6f2e    if not clodoo.
+00005490: 7365 6172 6368 4c38 280a 2020 2020 2020  searchL8(.      
+000054a0: 2020 2020 2020 7467 745f 6374 782c 206d        tgt_ctx, m
+000054b0: 6f64 656c 2c20 5b28 276e 616d 6527 2c20  odel, [('name', 
+000054c0: 273d 272c 206d 6f64 756c 6529 2c20 2827  '=', module), ('
+000054d0: 7374 6174 6527 2c20 273d 272c 2027 696e  state', '=', 'in
+000054e0: 7374 616c 6c65 6427 295d 0a20 2020 2020  stalled')].     
+000054f0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00005500: 2020 6966 2061 7373 756d 655f 7965 733a    if assume_yes:
+00005510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005520: 206f 7330 2e77 6c6f 6728 2749 6e73 7461   os0.wlog('Insta
+00005530: 6c6c 696e 6720 6d6f 6475 6c65 2025 7327  lling module %s'
+00005540: 2025 206d 6f64 756c 6529 0a20 2020 2020   % module).     
+00005550: 2020 2020 2020 2020 2020 2064 756d 6d79             dummy
+00005560: 203d 2027 5927 0a20 2020 2020 2020 2020   = 'Y'.         
+00005570: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00005580: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00005590: 6173 7375 6d65 5f79 6573 3a0a 2020 2020  assume_yes:.    
 000055a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055c0: 2020 2020 6f6c 645f 6d6f 6475 6c65 2c0a      old_module,.
-000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005600: 2073 7263 5f63 7478 5b27 6f65 5f76 6572   src_ctx['oe_ver
-00005610: 7369 6f6e 275d 2c0a 2020 2020 2020 2020  sion'],.        
-00005620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005640: 2020 2020 2020 2020 2074 6774 5f63 7478           tgt_ctx
-00005650: 5b27 6f65 5f76 6572 7369 6f6e 275d 2c0a  ['oe_version'],.
-00005660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005690: 2074 7970 653d 276d 6572 6765 2729 0a20   type='merge'). 
-000056a0: 2020 2020 2020 206d 7367 5f62 7572 7374         msg_burst
-000056b0: 2827 416e 616c 797a 696e 6720 6d6f 6475  ('Analyzing modu
-000056c0: 6c65 2025 7320 2825 7329 2720 2520 286d  le %s (%s)' % (m
-000056d0: 6f64 756c 652c 206f 6c64 5f6d 6f64 756c  odule, old_modul
-000056e0: 6529 290a 2020 2020 2020 2020 6966 206e  e)).        if n
-000056f0: 6f74 2063 6c6f 646f 6f2e 7365 6172 6368  ot clodoo.search
-00005700: 4c38 2874 6774 5f63 7478 2c20 6d6f 6465  L8(tgt_ctx, mode
-00005710: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
-00005720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005730: 2020 5b28 276e 616d 6527 2c20 273d 272c    [('name', '=',
-00005740: 206d 6f64 756c 6529 2c0a 2020 2020 2020   module),.      
-00005750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005760: 2020 2020 2020 2020 2020 2827 7374 6174            ('stat
-00005770: 6527 2c20 273d 272c 2027 696e 7374 616c  e', '=', 'instal
-00005780: 6c65 6427 295d 293a 0a20 2020 2020 2020  led')]):.       
-00005790: 2020 2020 2069 6620 6173 7375 6d65 5f79       if assume_y
-000057a0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-000057b0: 2020 2020 6f73 302e 776c 6f67 2827 496e      os0.wlog('In
-000057c0: 7374 616c 6c69 6e67 206d 6f64 756c 6520  stalling module 
-000057d0: 2573 2720 2520 6d6f 6475 6c65 290a 2020  %s' % module).  
-000057e0: 2020 2020 2020 2020 2020 2020 2020 6475                du
-000057f0: 6d6d 7920 3d20 2759 270a 2020 2020 2020  mmy = 'Y'.      
-00005800: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00005810: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00005820: 6f74 2061 7373 756d 655f 7965 733a 0a20  ot assume_yes:. 
+000055b0: 6475 6d6d 7920 3d20 696e 7075 7428 2749  dummy = input('I
+000055c0: 6e73 7461 6c6c 206d 6f64 756c 6520 2573  nstall module %s
+000055d0: 2028 5965 732c 4e6f 2c41 6c6c 2c51 7569   (Yes,No,All,Qui
+000055e0: 7429 3f20 2720 2520 6d6f 6475 6c65 290a  t)? ' % module).
+000055f0: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+00005600: 756d 6d79 5b30 5d20 696e 2028 276e 272c  ummy[0] in ('n',
+00005610: 2027 4e27 293a 0a20 2020 2020 2020 2020   'N'):.         
+00005620: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00005630: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+00005640: 756d 6d79 5b30 5d20 696e 2028 2771 272c  ummy[0] in ('q',
+00005650: 2027 5127 293a 0a20 2020 2020 2020 2020   'Q'):.         
+00005660: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00005670: 2020 2020 2020 2020 2020 6966 2064 756d            if dum
+00005680: 6d79 5b30 5d20 696e 2028 2761 272c 2027  my[0] in ('a', '
+00005690: 4127 293a 0a20 2020 2020 2020 2020 2020  A'):.           
+000056a0: 2020 2020 2061 7373 756d 655f 7965 7320       assume_yes 
+000056b0: 3d20 2759 270a 2020 2020 2020 2020 2020  = 'Y'.          
+000056c0: 2020 7374 7320 3d20 636c 6f64 6f6f 2e61    sts = clodoo.a
+000056d0: 6374 5f69 6e73 7461 6c6c 5f6d 6f64 756c  ct_install_modul
+000056e0: 6573 2874 6774 5f63 7478 2c20 6d6f 6475  es(tgt_ctx, modu
+000056f0: 6c65 5f6c 6973 743d 5b6d 6f64 756c 655d  le_list=[module]
+00005700: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00005710: 2073 7473 3a0a 2020 2020 2020 2020 2020   sts:.          
+00005720: 2020 2020 2020 6964 203d 2063 6c6f 646f        id = clodo
+00005730: 6f2e 7365 6172 6368 4c38 2874 6774 5f63  o.searchL8(tgt_c
+00005740: 7478 2c20 6d6f 6465 6c2c 205b 2827 6e61  tx, model, [('na
+00005750: 6d65 272c 2027 3d27 2c20 6d6f 6475 6c65  me', '=', module
+00005760: 295d 290a 2020 2020 2020 2020 2020 2020  )]).            
+00005770: 2020 2020 6966 2069 643a 0a20 2020 2020      if id:.     
+00005780: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00005790: 6c6f 646f 6f2e 7772 6974 654c 3828 7467  lodoo.writeL8(tg
+000057a0: 745f 6374 782c 206d 6f64 656c 2c20 6964  t_ctx, model, id
+000057b0: 2c20 7b27 7374 6174 6527 3a20 2774 6f20  , {'state': 'to 
+000057c0: 696e 7374 616c 6c27 7d29 0a20 2020 2020  install'}).     
+000057d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000057e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000057f0: 2020 2020 2076 616c 7320 3d20 7b0a 2020       vals = {.  
+00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005810: 2020 2020 2020 276e 616d 6527 3a20 6d6f        'name': mo
+00005820: 6475 6c65 5f73 7263 2e6e 616d 652c 0a20  dule_src.name,. 
 00005830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005840: 2020 2064 756d 6d79 203d 2069 6e70 7574     dummy = input
-00005850: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00005860: 2020 2020 2020 2020 2020 2749 6e73 7461            'Insta
-00005870: 6c6c 206d 6f64 756c 6520 2573 2028 5965  ll module %s (Ye
-00005880: 732c 4e6f 2c41 6c6c 2c51 7569 7429 3f20  s,No,All,Quit)? 
-00005890: 2720 2520 6d6f 6475 6c65 290a 2020 2020  ' % module).    
-000058a0: 2020 2020 2020 2020 6966 2064 756d 6d79          if dummy
-000058b0: 5b30 5d20 696e 2028 276e 272c 2027 4e27  [0] in ('n', 'N'
-000058c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000058d0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-000058e0: 2020 2020 2020 2020 6966 2064 756d 6d79          if dummy
-000058f0: 5b30 5d20 696e 2028 2771 272c 2027 5127  [0] in ('q', 'Q'
-00005900: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00005910: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00005920: 2020 2020 2020 6966 2064 756d 6d79 5b30        if dummy[0
-00005930: 5d20 696e 2028 2761 272c 2027 4127 293a  ] in ('a', 'A'):
-00005940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005950: 2061 7373 756d 655f 7965 7320 3d20 2759   assume_yes = 'Y
-00005960: 270a 2020 2020 2020 2020 2020 2020 7374  '.            st
-00005970: 7320 3d20 636c 6f64 6f6f 2e61 6374 5f69  s = clodoo.act_i
-00005980: 6e73 7461 6c6c 5f6d 6f64 756c 6573 2874  nstall_modules(t
-00005990: 6774 5f63 7478 2c20 6d6f 6475 6c65 5f6c  gt_ctx, module_l
-000059a0: 6973 743d 5b6d 6f64 756c 655d 290a 2020  ist=[module]).  
-000059b0: 2020 2020 2020 2020 2020 6966 2073 7473            if sts
-000059c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000059d0: 2020 6964 203d 2063 6c6f 646f 6f2e 7365    id = clodoo.se
-000059e0: 6172 6368 4c38 2874 6774 5f63 7478 2c20  archL8(tgt_ctx, 
-000059f0: 6d6f 6465 6c2c 0a20 2020 2020 2020 2020  model,.         
-00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a10: 2020 2020 2020 5b28 276e 616d 6527 2c20        [('name', 
-00005a20: 273d 272c 206d 6f64 756c 6529 5d29 0a20  '=', module)]). 
-00005a30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005a40: 6620 6964 3a0a 2020 2020 2020 2020 2020  f id:.          
-00005a50: 2020 2020 2020 2020 2020 636c 6f64 6f6f            clodoo
-00005a60: 2e77 7269 7465 4c38 2874 6774 5f63 7478  .writeL8(tgt_ctx
-00005a70: 2c20 6d6f 6465 6c2c 2069 642c 207b 2773  , model, id, {'s
-00005a80: 7461 7465 273a 2027 746f 2069 6e73 7461  tate': 'to insta
-00005a90: 6c6c 277d 290a 2020 2020 2020 2020 2020  ll'}).          
-00005aa0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ac0: 7661 6c73 203d 207b 0a20 2020 2020 2020  vals = {.       
-00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ae0: 2027 6e61 6d65 273a 206d 6f64 756c 655f   'name': module_
-00005af0: 7372 632e 6e61 6d65 2c0a 2020 2020 2020  src.name,.      
-00005b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b10: 2020 2761 7574 686f 7227 3a20 6d6f 6475    'author': modu
-00005b20: 6c65 5f73 7263 2e61 7574 686f 722c 0a20  le_src.author,. 
-00005b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b40: 2020 2020 2020 2027 6465 6d6f 273a 206d         'demo': m
-00005b50: 6f64 756c 655f 7372 632e 6465 6d6f 2c0a  odule_src.demo,.
-00005b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b70: 2020 2020 2020 2020 2764 6573 6372 6970          'descrip
-00005b80: 7469 6f6e 273a 206d 6f64 756c 655f 7372  tion': module_sr
-00005b90: 632e 6465 7363 7269 7074 696f 6e2c 0a20  c.description,. 
-00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bb0: 2020 2020 2020 2027 7375 6d6d 6172 7927         'summary'
-00005bc0: 3a20 6d6f 6475 6c65 5f73 7263 2e73 756d  : module_src.sum
-00005bd0: 6d61 7279 2c0a 2020 2020 2020 2020 2020  mary,.          
-00005be0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-00005bf0: 7461 7465 273a 2027 746f 2069 6e73 7461  tate': 'to insta
-00005c00: 6c6c 270a 2020 2020 2020 2020 2020 2020  ll'.            
-00005c10: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00005c20: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-00005c30: 6f64 6f6f 2e63 7265 6174 654c 3828 7467  odoo.createL8(tg
-00005c40: 745f 6374 782c 206d 6f64 656c 2c20 7661  t_ctx, model, va
-00005c50: 6c73 290a 2020 2020 2020 2020 656c 6966  ls).        elif
-00005c60: 2075 7067 7261 6465 3a0a 2020 2020 2020   upgrade:.      
-00005c70: 2020 2020 2020 6966 2063 6c6f 646f 6f2e        if clodoo.
-00005c80: 7365 6172 6368 4c38 2874 6774 5f63 7478  searchL8(tgt_ctx
-00005c90: 2c20 6d6f 6465 6c2c 0a20 2020 2020 2020  , model,.       
-00005ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cb0: 2020 2020 2020 2020 5b28 276e 616d 6527          [('name'
-00005cc0: 2c20 273d 272c 206d 6f64 756c 6529 2c0a  , '=', module),.
-00005cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cf0: 2827 7374 6174 6527 2c20 273d 272c 2027  ('state', '=', '
-00005d00: 696e 7374 616c 6c65 6427 295d 293a 0a20  installed')]):. 
-00005d10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005d20: 7473 203d 2063 6c6f 646f 6f2e 6163 745f  ts = clodoo.act_
-00005d30: 7570 6772 6164 655f 6d6f 6475 6c65 7328  upgrade_modules(
-00005d40: 7467 745f 6374 782c 206d 6f64 756c 655f  tgt_ctx, module_
-00005d50: 6c69 7374 3d5b 6d6f 6475 6c65 5d29 0a0a  list=[module])..
-00005d60: 0a64 6566 2067 6574 5f66 6f72 6569 676e  .def get_foreign
-00005d70: 5f76 616c 7565 2874 6774 5f63 7478 2c20  _value(tgt_ctx, 
-00005d80: 7372 635f 6374 782c 2072 656c 6174 696f  src_ctx, relatio
-00005d90: 6e2c 2076 616c 7565 2c0a 2020 2020 2020  n, value,.      
-00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005db0: 746f 6d61 6e79 3d4e 6f6e 652c 2066 6f72  tomany=None, for
-00005dc0: 6d61 743d 4661 6c73 6529 3a0a 0a20 2020  mat=False):..   
-00005dd0: 2064 6566 2062 696e 645f 666f 7265 6967   def bind_foreig
-00005de0: 6e5f 7265 6628 7467 745f 6374 782c 2073  n_ref(tgt_ctx, s
-00005df0: 7263 5f63 7478 2c20 6d6f 6465 6c2c 2069  rc_ctx, model, i
-00005e00: 642c 2072 656c 5f6d 6f64 6529 3a0a 2020  d, rel_mode):.  
-00005e10: 2020 2020 2020 6e65 775f 7661 6c75 6520        new_value 
-00005e20: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00005e30: 6361 6368 6520 3d20 6765 745f 6361 6368  cache = get_cach
-00005e40: 6528 7372 635f 6374 7829 0a20 2020 2020  e(src_ctx).     
-00005e50: 2020 2069 6620 7265 6c5f 6d6f 6465 203d     if rel_mode =
-00005e60: 3d20 2769 6d61 6765 273a 0a20 2020 2020  = 'image':.     
-00005e70: 2020 2020 2020 2069 6620 636c 6f64 6f6f         if clodoo
-00005e80: 2e73 6561 7263 684c 3828 7467 745f 6374  .searchL8(tgt_ct
-00005e90: 782c 2072 656c 6174 696f 6e2c 205b 2827  x, relation, [('
-00005ea0: 6964 272c 2027 3d27 2c20 6964 295d 293a  id', '=', id)]):
-00005eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005ec0: 206e 6577 5f76 616c 7565 203d 2069 640a   new_value = id.
-00005ed0: 2020 2020 2020 2020 656c 6966 2063 6163          elif cac
-00005ee0: 6865 5f69 735f 656e 7472 7928 6361 6368  he_is_entry(cach
-00005ef0: 652c 206d 6f64 656c 2c20 6964 293a 0a20  e, model, id):. 
-00005f00: 2020 2020 2020 2020 2020 206e 6577 5f76             new_v
-00005f10: 616c 7565 203d 2063 6163 6865 5f67 6574  alue = cache_get
-00005f20: 5f65 6e74 7279 2863 6163 6865 2c20 6d6f  _entry(cache, mo
-00005f30: 6465 6c2c 2069 6429 0a20 2020 2020 2020  del, id).       
-00005f40: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00005f50: 2020 2072 656c 5f72 6563 203d 2063 6c6f     rel_rec = clo
-00005f60: 646f 6f2e 6272 6f77 7365 4c38 2873 7263  doo.browseL8(src
-00005f70: 5f63 7478 2c20 7265 6c61 7469 6f6e 2c20  _ctx, relation, 
-00005f80: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
-00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fa0: 2020 2020 2020 2020 2020 636f 6e74 6578            contex
-00005fb0: 743d 7b27 6c61 6e67 273a 2027 656e 5f55  t={'lang': 'en_U
-00005fc0: 5327 7d29 0a20 2020 2020 2020 2020 2020  S'}).           
-00005fd0: 206b 6579 7661 6c20 3d20 636c 6f64 6f6f   keyval = clodoo
-00005fe0: 2e65 7874 7261 6374 5f76 616c 735f 6672  .extract_vals_fr
-00005ff0: 6f6d 5f72 6563 2873 7263 5f63 7478 2c0a  om_rec(src_ctx,.
-00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006030: 2020 6d6f 6465 6c2c 0a20 2020 2020 2020    model,.       
-00006040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006060: 2020 2020 2020 2020 2020 2072 656c 5f72             rel_r
-00006070: 6563 2c0a 2020 2020 2020 2020 2020 2020  ec,.            
-00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060a0: 2020 2020 2020 666f 726d 6174 3d27 7374        format='st
-000060b0: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
-000060c0: 6964 203d 2073 6561 7263 6834 7265 6328  id = search4rec(
-000060d0: 7467 745f 6374 782c 206d 6f64 656c 2c20  tgt_ctx, model, 
-000060e0: 6b65 7976 616c 290a 2020 2020 2020 2020  keyval).        
-000060f0: 2020 2020 6966 2069 6420 3e3d 2031 3a0a      if id >= 1:.
-00006100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006110: 6e65 775f 7661 6c75 6520 3d20 6964 0a20  new_value = id. 
-00006120: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00006130: 6163 6865 5f73 746f 7265 5f65 6e74 7279  ache_store_entry
-00006140: 2863 6163 6865 2c20 6d6f 6465 6c2c 2069  (cache, model, i
-00006150: 6429 0a20 2020 2020 2020 2020 2020 2065  d).            e
-00006160: 6c69 6620 6e6f 7420 7372 635f 6374 782e  lif not src_ctx.
-00006170: 6765 7428 276e 6f5f 7265 6375 7273 6527  get('no_recurse'
-00006180: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00006190: 2020 206e 6577 5f76 616c 7565 203d 2073     new_value = s
-000061a0: 796e 6368 726f 2874 6774 5f63 7478 2c20  ynchro(tgt_ctx, 
-000061b0: 7265 6c61 7469 6f6e 2c20 6b65 7976 616c  relation, keyval
-000061c0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000061d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000061e0: 2020 2020 6361 6368 655f 7374 6f72 655f      cache_store_
-000061f0: 656e 7472 7928 6361 6368 652c 206d 6f64  entry(cache, mod
-00006200: 656c 2c20 6e65 775f 7661 6c75 6529 0a20  el, new_value). 
-00006210: 2020 2020 2020 2072 6574 7572 6e20 6e65         return ne
-00006220: 775f 7661 6c75 650a 0a20 2020 2069 6620  w_value..    if 
-00006230: 6e6f 7420 7661 6c75 653a 0a20 2020 2020  not value:.     
-00006240: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00006250: 2020 2020 6966 206e 6f74 2072 656c 6174      if not relat
-00006260: 696f 6e3a 0a20 2020 2020 2020 2072 6169  ion:.        rai
-00006270: 7365 2052 756e 7469 6d65 4572 726f 7228  se RuntimeError(
-00006280: 274e 6f20 7265 6c61 7469 6f6e 2025 7320  'No relation %s 
-00006290: 666f 756e 6427 2025 2072 656c 6174 696f  found' % relatio
-000062a0: 6e29 0a20 2020 2072 656c 5f6d 6f64 6520  n).    rel_mode 
-000062b0: 3d20 6765 745f 6d6f 6465 6c5f 636f 7079  = get_model_copy
-000062c0: 5f6d 6f64 6528 7467 745f 6374 782c 2072  _mode(tgt_ctx, r
-000062d0: 656c 6174 696f 6e29 0a20 2020 2063 6c6f  elation).    clo
-000062e0: 646f 6f2e 6765 745f 6d6f 6465 6c5f 7374  doo.get_model_st
-000062f0: 7275 6374 7572 6528 0a20 2020 2020 2020  ructure(.       
-00006300: 2073 7263 5f63 7478 2c20 7265 6c61 7469   src_ctx, relati
-00006310: 6f6e 2c0a 2020 2020 2020 2020 6967 6e6f  on,.        igno
-00006320: 7265 3d49 474e 4f52 455f 4649 454c 4453  re=IGNORE_FIELDS
-00006330: 2e67 6574 2872 656c 6174 696f 6e2c 205b  .get(relation, [
-00006340: 5d29 202b 2049 474e 4f52 455f 4649 454c  ]) + IGNORE_FIEL
-00006350: 4453 5b27 2a27 5d29 0a20 2020 2063 6c6f  DS['*']).    clo
-00006360: 646f 6f2e 6765 745f 6d6f 6465 6c5f 7374  doo.get_model_st
-00006370: 7275 6374 7572 6528 0a20 2020 2020 2020  ructure(.       
-00006380: 2074 6774 5f63 7478 2c20 7265 6c61 7469   tgt_ctx, relati
-00006390: 6f6e 2c0a 2020 2020 2020 2020 6967 6e6f  on,.        igno
-000063a0: 7265 3d49 474e 4f52 455f 4649 454c 4453  re=IGNORE_FIELDS
-000063b0: 2e67 6574 2872 656c 6174 696f 6e2c 205b  .get(relation, [
-000063c0: 5d29 202b 2049 474e 4f52 455f 4649 454c  ]) + IGNORE_FIEL
-000063d0: 4453 5b27 2a27 5d29 0a20 2020 206e 6577  DS['*']).    new
-000063e0: 5f76 616c 7565 203d 2046 616c 7365 0a20  _value = False. 
-000063f0: 2020 2069 6620 7467 745f 6374 785b 275f     if tgt_ctx['_
-00006400: 6d6c 275d 2e67 6574 2872 656c 6174 696f  ml'].get(relatio
-00006410: 6e29 2021 3d20 276e 6f27 3a0a 2020 2020  n) != 'no':.    
-00006420: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00006430: 6528 7661 6c75 652c 2062 6173 6573 7472  e(value, basestr
-00006440: 696e 6729 3a0a 2020 2020 2020 2020 2020  ing):.          
-00006450: 2020 7061 7373 2020 2020 2320 544f 444f    pass    # TODO
-00006460: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00006470: 746f 6d61 6e79 3a0a 2020 2020 2020 2020  tomany:.        
-00006480: 2020 2020 2020 2020 6e65 775f 7661 6c75          new_valu
-00006490: 6520 3d20 5b6e 6577 5f76 616c 7565 5d0a  e = [new_value].
-000064a0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-000064b0: 6e73 7461 6e63 6528 7265 6c61 7469 6f6e  nstance(relation
-000064c0: 2c20 286c 6973 742c 2074 7570 6c65 2929  , (list, tuple))
-000064d0: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
-000064e0: 775f 7661 6c75 6520 3d20 5b5d 0a20 2020  w_value = [].   
-000064f0: 2020 2020 2020 2020 2066 6f72 2069 6420           for id 
-00006500: 696e 2076 616c 7565 3a0a 2020 2020 2020  in value:.      
-00006510: 2020 2020 2020 2020 2020 6e65 775f 7661            new_va
-00006520: 6c75 652e 6170 7065 6e64 280a 2020 2020  lue.append(.    
-00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006540: 6269 6e64 5f66 6f72 6569 676e 5f72 6566  bind_foreign_ref
-00006550: 2874 6774 5f63 7478 2c20 7372 635f 6374  (tgt_ctx, src_ct
-00006560: 782c 2072 656c 6174 696f 6e2c 2069 642c  x, relation, id,
-00006570: 2072 656c 5f6d 6f64 6529 290a 2020 2020   rel_mode)).    
-00006580: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00006590: 2020 2020 2020 6e65 775f 7661 6c75 6520        new_value 
-000065a0: 3d20 6269 6e64 5f66 6f72 6569 676e 5f72  = bind_foreign_r
-000065b0: 6566 280a 2020 2020 2020 2020 2020 2020  ef(.            
-000065c0: 2020 2020 7467 745f 6374 782c 2073 7263      tgt_ctx, src
-000065d0: 5f63 7478 2c20 7265 6c61 7469 6f6e 2c20  _ctx, relation, 
-000065e0: 7661 6c75 652c 2072 656c 5f6d 6f64 6529  value, rel_mode)
-000065f0: 0a20 2020 2069 6620 666f 726d 6174 203d  .    if format =
-00006600: 3d20 2763 6d64 2720 616e 6420 7661 6c75  = 'cmd' and valu
-00006610: 6520 616e 6420 746f 6d61 6e79 3a0a 2020  e and tomany:.  
-00006620: 2020 2020 2020 7661 6c75 6520 3d20 5b28        value = [(
-00006630: 362c 2030 2c20 7661 6c75 6529 5d0a 2020  6, 0, value)].  
-00006640: 2020 7265 7475 726e 206e 6577 5f76 616c    return new_val
-00006650: 7565 0a0a 0a64 6566 2063 7674 5f6f 326d  ue...def cvt_o2m
-00006660: 5f76 616c 7565 2874 6774 5f63 7478 2c20  _value(tgt_ctx, 
-00006670: 7372 635f 6374 782c 206d 6f64 656c 2c20  src_ctx, model, 
-00006680: 6e61 6d65 2c20 7661 6c75 652c 2066 6f72  name, value, for
-00006690: 6d61 743d 4661 6c73 6529 3a0a 2020 2020  mat=False):.    
-000066a0: 7265 6c61 7469 6f6e 203d 2073 7263 5f63  relation = src_c
-000066b0: 7478 5b27 5354 5255 4354 275d 5b6d 6f64  tx['STRUCT'][mod
-000066c0: 656c 5d5b 6e61 6d65 5d5b 2772 656c 6174  el][name]['relat
-000066d0: 696f 6e27 5d0a 2020 2020 7265 7475 726e  ion'].    return
-000066e0: 2067 6574 5f66 6f72 6569 676e 5f76 616c   get_foreign_val
-000066f0: 7565 2874 6774 5f63 7478 2c20 7372 635f  ue(tgt_ctx, src_
-00006700: 6374 782c 2072 656c 6174 696f 6e2c 2076  ctx, relation, v
-00006710: 616c 7565 2c20 746f 6d61 6e79 3d54 7275  alue, tomany=Tru
-00006720: 6529 0a0a 0a64 6566 2063 7674 5f6d 326d  e)...def cvt_m2m
-00006730: 5f76 616c 7565 2874 6774 5f63 7478 2c20  _value(tgt_ctx, 
-00006740: 7372 635f 6374 782c 206d 6f64 656c 2c20  src_ctx, model, 
-00006750: 6e61 6d65 2c20 7661 6c75 652c 2066 6f72  name, value, for
-00006760: 6d61 743d 4661 6c73 6529 3a0a 2020 2020  mat=False):.    
-00006770: 7265 6c61 7469 6f6e 203d 2073 7263 5f63  relation = src_c
-00006780: 7478 5b27 5354 5255 4354 275d 5b6d 6f64  tx['STRUCT'][mod
-00006790: 656c 5d5b 6e61 6d65 5d5b 2772 656c 6174  el][name]['relat
-000067a0: 696f 6e27 5d0a 2020 2020 7265 7475 726e  ion'].    return
-000067b0: 2067 6574 5f66 6f72 6569 676e 5f76 616c   get_foreign_val
-000067c0: 7565 2874 6774 5f63 7478 2c20 7372 635f  ue(tgt_ctx, src_
-000067d0: 6374 782c 2072 656c 6174 696f 6e2c 2076  ctx, relation, v
-000067e0: 616c 7565 2c20 746f 6d61 6e79 3d54 7275  alue, tomany=Tru
-000067f0: 6529 0a0a 0a64 6566 2063 7674 5f6d 326f  e)...def cvt_m2o
-00006800: 5f76 616c 7565 2874 6774 5f63 7478 2c20  _value(tgt_ctx, 
-00006810: 7372 635f 6374 782c 206d 6f64 656c 2c20  src_ctx, model, 
-00006820: 6e61 6d65 2c20 7661 6c75 652c 2066 6f72  name, value, for
-00006830: 6d61 743d 4661 6c73 6529 3a0a 2020 2020  mat=False):.    
-00006840: 7265 6c61 7469 6f6e 203d 2073 7263 5f63  relation = src_c
-00006850: 7478 5b27 5354 5255 4354 275d 5b6d 6f64  tx['STRUCT'][mod
-00006860: 656c 5d5b 6e61 6d65 5d5b 2772 656c 6174  el][name]['relat
-00006870: 696f 6e27 5d0a 2020 2020 7265 7475 726e  ion'].    return
-00006880: 2067 6574 5f66 6f72 6569 676e 5f76 616c   get_foreign_val
-00006890: 7565 2874 6774 5f63 7478 2c20 7372 635f  ue(tgt_ctx, src_
-000068a0: 6374 782c 2072 656c 6174 696f 6e2c 2076  ctx, relation, v
-000068b0: 616c 7565 290a 0a0a 6465 6620 6c6f 6164  alue)...def load
-000068c0: 5f72 6563 6f72 6428 7467 745f 6374 782c  _record(tgt_ctx,
-000068d0: 2073 7263 5f63 7478 2c20 6d6f 6465 6c2c   src_ctx, model,
-000068e0: 2072 6563 2c20 6d6f 6465 3d4e 6f6e 6529   rec, mode=None)
-000068f0: 3a0a 2020 2020 6d6f 6465 203d 206d 6f64  :.    mode = mod
-00006900: 6520 6f72 2067 6574 5f6d 6f64 656c 5f63  e or get_model_c
-00006910: 6f70 795f 6d6f 6465 2873 7263 5f63 7478  opy_mode(src_ctx
-00006920: 2c20 6d6f 6465 6c29 0a20 2020 2076 616c  , model).    val
-00006930: 7320 3d20 636c 6f64 6f6f 2e65 7874 7261  s = clodoo.extra
-00006940: 6374 5f76 616c 735f 6672 6f6d 5f72 6563  ct_vals_from_rec
-00006950: 2873 7263 5f63 7478 2c20 6d6f 6465 6c2c  (src_ctx, model,
-00006960: 2072 6563 2c20 666f 726d 6174 3d27 7374   rec, format='st
-00006970: 7227 290a 2020 2020 7661 6c73 203d 2063  r').    vals = c
-00006980: 6c6f 646f 6f2e 6376 745f 6672 6f6d 5f76  lodoo.cvt_from_v
-00006990: 6572 5f32 5f76 6572 2874 6774 5f63 7478  er_2_ver(tgt_ctx
-000069a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069c0: 2020 2020 2020 206d 6f64 656c 2c0a 2020         model,.  
-000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069f0: 2020 2073 7263 5f63 7478 5b27 6f65 5f76     src_ctx['oe_v
-00006a00: 6572 7369 6f6e 275d 2c0a 2020 2020 2020  ersion'],.      
-00006a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a20: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00006a30: 6774 5f63 7478 5b27 6f65 5f76 6572 7369  gt_ctx['oe_versi
-00006a40: 6f6e 275d 2c0a 2020 2020 2020 2020 2020  on'],.          
-00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a60: 2020 2020 2020 2020 2020 2076 616c 7329             vals)
-00006a70: 0a20 2020 2066 6f72 206e 616d 6520 696e  .    for name in
-00006a80: 2076 616c 732e 636f 7079 2829 3a0a 2020   vals.copy():.  
-00006a90: 2020 2020 2020 6966 206e 616d 6520 6e6f        if name no
-00006aa0: 7420 696e 2074 6774 5f63 7478 5b27 5354  t in tgt_ctx['ST
-00006ab0: 5255 4354 275d 5b6d 6f64 656c 5d3a 0a20  RUCT'][model]:. 
-00006ac0: 2020 2020 2020 2020 2020 2064 656c 2076             del v
-00006ad0: 616c 735b 6e61 6d65 5d0a 2020 2020 2020  als[name].      
-00006ae0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-00006af0: 2020 2020 2020 2065 6c69 6620 6e61 6d65         elif name
-00006b00: 203d 3d20 2763 6f6d 7061 6e79 5f69 6427   == 'company_id'
-00006b10: 2061 6e64 2073 7263 5f63 7478 5b27 6279   and src_ctx['by
-00006b20: 5f63 6f6d 7061 6e79 275d 3a0a 2020 2020  _company']:.    
-00006b30: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00006b40: 0a20 2020 2020 2020 2065 6c69 6620 7467  .        elif tg
-00006b50: 745f 6374 785b 2753 5452 5543 5427 5d5b  t_ctx['STRUCT'][
-00006b60: 6d6f 6465 6c5d 5b6e 616d 655d 5b27 7474  model][name]['tt
-00006b70: 7970 6527 5d20 696e 2028 276f 6e65 326d  ype'] in ('one2m
-00006b80: 616e 7927 293a 0a20 2020 2020 2020 2020  any'):.         
-00006b90: 2020 2076 616c 735b 6e61 6d65 5d20 3d20     vals[name] = 
-00006ba0: 6376 745f 6f32 6d5f 7661 6c75 6528 7467  cvt_o2m_value(tg
-00006bb0: 745f 6374 782c 2074 6774 5f63 7478 2c20  t_ctx, tgt_ctx, 
-00006bc0: 6d6f 6465 6c2c 206e 616d 652c 0a20 2020  model, name,.   
-00006bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bf0: 2020 2020 7661 6c73 5b6e 616d 655d 2c20      vals[name], 
-00006c00: 666f 726d 6174 3d27 636d 6427 290a 2020  format='cmd').  
-00006c10: 2020 2020 2020 656c 6966 2074 6774 5f63        elif tgt_c
-00006c20: 7478 5b27 5354 5255 4354 275d 5b6d 6f64  tx['STRUCT'][mod
-00006c30: 656c 5d5b 6e61 6d65 5d5b 2774 7479 7065  el][name]['ttype
-00006c40: 275d 2069 6e20 2827 6d61 6e79 326d 616e  '] in ('many2man
-00006c50: 7927 293a 0a20 2020 2020 2020 2020 2020  y'):.           
-00006c60: 2076 616c 735b 6e61 6d65 5d20 3d20 6376   vals[name] = cv
-00006c70: 745f 6d32 6d5f 7661 6c75 6528 7467 745f  t_m2m_value(tgt_
-00006c80: 6374 782c 2074 6774 5f63 7478 2c20 6d6f  ctx, tgt_ctx, mo
-00006c90: 6465 6c2c 206e 616d 652c 0a20 2020 2020  del, name,.     
-00006ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cc0: 2020 7661 6c73 5b6e 616d 655d 2c20 666f    vals[name], fo
-00006cd0: 726d 6174 3d27 636d 6427 290a 2020 2020  rmat='cmd').    
-00006ce0: 2020 2020 656c 6966 2074 6774 5f63 7478      elif tgt_ctx
-00006cf0: 5b27 5354 5255 4354 275d 5b6d 6f64 656c  ['STRUCT'][model
-00006d00: 5d5b 6e61 6d65 5d5b 2774 7479 7065 275d  ][name]['ttype']
-00006d10: 2069 6e20 2827 6d61 6e79 326f 6e65 2729   in ('many2one')
-00006d20: 3a0a 2020 2020 2020 2020 2020 2020 7661  :.            va
-00006d30: 6c73 5b6e 616d 655d 203d 2063 7674 5f6d  ls[name] = cvt_m
-00006d40: 326f 5f76 616c 7565 2874 6774 5f63 7478  2o_value(tgt_ctx
-00006d50: 2c20 7467 745f 6374 782c 206d 6f64 656c  , tgt_ctx, model
-00006d60: 2c20 6e61 6d65 2c0a 2020 2020 2020 2020  , name,.        
-00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d80: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00006d90: 616c 735b 6e61 6d65 5d2c 2066 6f72 6d61  als[name], forma
-00006da0: 743d 2763 6d64 2729 0a20 2020 2020 2020  t='cmd').       
-00006db0: 2069 6620 2876 616c 735b 6e61 6d65 5d20   if (vals[name] 
-00006dc0: 6973 2046 616c 7365 2061 6e64 0a20 2020  is False and.   
-00006dd0: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
-00006de0: 5f63 7478 5b27 5354 5255 4354 275d 5b6d  _ctx['STRUCT'][m
-00006df0: 6f64 656c 5d5b 6e61 6d65 5d5b 2774 7479  odel][name]['tty
-00006e00: 7065 275d 2021 3d20 2762 6f6f 6c65 616e  pe'] != 'boolean
-00006e10: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-00006e20: 6465 6c20 7661 6c73 5b6e 616d 655d 0a20  del vals[name]. 
-00006e30: 2020 2072 6574 7572 6e20 7661 6c73 0a0a     return vals..
-00006e40: 0a64 6566 2075 7365 5f73 796e 6368 726f  .def use_synchro
-00006e50: 2874 6774 5f63 7478 2c20 6d6f 6465 6c29  (tgt_ctx, model)
-00006e60: 3a0a 2020 2020 6966 2074 6774 5f63 7478  :.    if tgt_ctx
-00006e70: 5b27 7573 655f 7379 6e63 6872 6f27 5d20  ['use_synchro'] 
-00006e80: 616e 6420 6d6f 6465 6c20 696e 2028 2772  and model in ('r
-00006e90: 6573 2e63 6f75 6e74 7279 272c 0a20 2020  es.country',.   
-00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ec0: 2020 2020 2020 2020 2027 7265 732e 7061           'res.pa
-00006ed0: 7274 6e65 7227 2c0a 2020 2020 2020 2020  rtner',.        
-00006ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f00: 2020 2020 2761 6363 6f75 6e74 2e61 6363      'account.acc
-00006f10: 6f75 6e74 272c 0a20 2020 2020 2020 2020  ount',.         
-00006f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f40: 2020 2027 6163 636f 756e 742e 6163 636f     'account.acco
-00006f50: 756e 742e 7479 7065 272c 0a20 2020 2020  unt.type',.     
-00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f80: 2020 2020 2020 2027 6163 636f 756e 742e         'account.
-00006f90: 696e 766f 6963 6527 2c0a 2020 2020 2020  invoice',.      
-00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fc0: 2020 2020 2020 2761 6363 6f75 6e74 2e69        'account.i
-00006fd0: 6e76 6f69 6365 2e6c 696e 6527 2c0a 2020  nvoice.line',.  
-00006fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007000: 2020 2020 2020 2020 2020 2761 6363 6f75            'accou
-00007010: 6e74 2e74 6178 272c 0a20 2020 2020 2020  nt.tax',.       
-00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007040: 2020 2020 2027 7072 6f64 7563 742e 7465       'product.te
-00007050: 6d70 6c61 7465 272c 0a20 2020 2020 2020  mplate',.       
-00007060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007080: 2020 2020 2027 7072 6f64 7563 742e 7072       'product.pr
-00007090: 6f64 7563 7427 2c0a 2020 2020 2020 2020  oduct',.        
-000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070c0: 2020 2020 2773 616c 652e 6f72 6465 7227      'sale.order'
-000070d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070f0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-00007100: 616c 652e 6f72 6465 722e 6c69 6e65 2729  ale.order.line')
-00007110: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00007120: 2054 7275 650a 2020 2020 7265 7475 726e   True.    return
-00007130: 2046 616c 7365 0a0a 0a64 6566 2073 6574   False...def set
-00007140: 5f61 6374 7561 6c5f 7374 6174 6528 7467  _actual_state(tg
-00007150: 745f 6374 782c 206d 6f64 656c 2c20 6964  t_ctx, model, id
-00007160: 2c20 7374 6174 6529 3a0a 2020 2020 6966  , state):.    if
-00007170: 206d 6f64 656c 203d 3d20 2761 6363 6f75   model == 'accou
-00007180: 6e74 2e69 6e76 6f69 6365 273a 0a20 2020  nt.invoice':.   
-00007190: 2020 2020 2069 6620 6964 3a0a 2020 2020       if id:.    
-000071a0: 2020 2020 2020 2020 7265 6320 3d20 636c          rec = cl
-000071b0: 6f64 6f6f 2e62 726f 7773 654c 3828 7467  odoo.browseL8(tg
-000071c0: 745f 6374 782c 206d 6f64 656c 2c20 6964  t_ctx, model, id
-000071d0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-000071e0: 2073 7461 7465 203d 3d20 2764 7261 6674   state == 'draft
-000071f0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00007200: 2020 2061 6374 696f 6e20 3d20 2727 0a20     action = ''. 
-00007210: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00007220: 6574 7572 6e20 7265 632e 6964 0a20 2020  eturn rec.id.   
-00007230: 2020 2020 2020 2020 2065 6c69 6620 7265           elif re
-00007240: 632e 7374 6174 6520 213d 2027 6472 6166  c.state != 'draf
-00007250: 7427 3a0a 2020 2020 2020 2020 2020 2020  t':.            
-00007260: 2020 2020 7265 7475 726e 202d 340a 2020      return -4.  
-00007270: 2020 2020 2020 2020 2020 656c 6966 2072            elif r
-00007280: 6563 2e6f 7269 6769 6e61 6c5f 7374 6174  ec.original_stat
-00007290: 6520 3d3d 2027 6f70 656e 273a 0a20 2020  e == 'open':.   
-000072a0: 2020 2020 2020 2020 2020 2020 2072 6563               rec
-000072b0: 2e61 6374 696f 6e5f 696e 766f 6963 655f  .action_invoice_
-000072c0: 6f70 656e 2829 0a20 2020 2020 2020 2020  open().         
-000072d0: 2020 2065 6c69 6620 7265 632e 6f72 6967     elif rec.orig
-000072e0: 696e 616c 5f73 7461 7465 203d 3d20 2763  inal_state == 'c
-000072f0: 616e 6365 6c27 3a0a 2020 2020 2020 2020  ancel':.        
-00007300: 2020 2020 2020 2020 7265 632e 6163 7469          rec.acti
-00007310: 6f6e 5f69 6e76 6f69 6365 5f63 616e 6365  on_invoice_cance
-00007320: 6c28 290a 2020 2020 656c 6966 206d 6f64  l().    elif mod
-00007330: 656c 203d 3d20 2773 616c 652e 6f72 6465  el == 'sale.orde
-00007340: 7227 3a0a 2020 2020 2020 2020 6966 2069  r':.        if i
-00007350: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
-00007360: 6563 203d 2063 6c6f 646f 6f2e 6272 6f77  ec = clodoo.brow
-00007370: 7365 4c38 2874 6774 5f63 7478 2c20 6d6f  seL8(tgt_ctx, mo
-00007380: 6465 6c2c 2069 6429 0a20 2020 2020 2020  del, id).       
-00007390: 2020 2020 2072 6563 2e5f 636f 6d70 7574       rec._comput
-000073a0: 655f 7461 785f 6964 2829 0a20 2020 2020  e_tax_id().     
-000073b0: 2020 2020 2020 2069 6620 7265 632e 7374         if rec.st
-000073c0: 6174 6520 3d3d 2072 6563 2e6f 7269 6769  ate == rec.origi
-000073d0: 6e61 6c5f 7374 6174 653a 0a20 2020 2020  nal_state:.     
-000073e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000073f0: 6e20 7265 632e 6964 0a20 2020 2020 2020  n rec.id.       
-00007400: 2020 2020 2065 6c69 6620 7265 632e 7374       elif rec.st
-00007410: 6174 6520 213d 2027 6472 6166 7427 3a0a  ate != 'draft':.
-00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007430: 7265 7475 726e 202d 340a 2020 2020 2020  return -4.      
-00007440: 2020 2020 2020 656c 6966 2072 6563 2e6f        elif rec.o
-00007450: 7269 6769 6e61 6c5f 7374 6174 6520 3d3d  riginal_state ==
-00007460: 2027 7361 6c65 273a 0a20 2020 2020 2020   'sale':.       
-00007470: 2020 2020 2020 2020 2072 6563 2e61 6374           rec.act
-00007480: 696f 6e5f 636f 6e66 6972 6d28 290a 2020  ion_confirm().  
-00007490: 2020 2020 2020 2020 2020 656c 6966 2072            elif r
-000074a0: 6563 2e6f 7269 6769 6e61 6c5f 7374 6174  ec.original_stat
-000074b0: 6520 3d3d 2027 6361 6e63 656c 273a 0a20  e == 'cancel':. 
-000074c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000074d0: 6563 2e61 6374 696f 6e5f 6361 6e63 656c  ec.action_cancel
-000074e0: 2829 0a20 2020 2072 6574 7572 6e20 7265  ().    return re
-000074f0: 632e 6964 0a0a 0a64 6566 2073 6574 5f73  c.id...def set_s
-00007500: 7461 7465 5f74 6f5f 6472 6166 7428 7467  tate_to_draft(tg
-00007510: 745f 6374 782c 206d 6f64 656c 2c20 6964  t_ctx, model, id
-00007520: 732c 2076 616c 7329 3a0a 2020 2020 7265  s, vals):.    re
-00007530: 6320 3d20 4661 6c73 650a 2020 2020 6966  c = False.    if
-00007540: 206e 6f74 2069 6473 3a0a 2020 2020 2020   not ids:.      
-00007550: 2020 6964 203d 2046 616c 7365 0a20 2020    id = False.   
-00007560: 2065 6c73 653a 0a20 2020 2020 2020 2069   else:.        i
-00007570: 6420 3d20 6964 735b 305d 0a20 2020 2074  d = ids[0].    t
-00007580: 6774 5f63 7478 5b27 5f43 4f4d 4d49 5427  gt_ctx['_COMMIT'
-00007590: 5d5b 6d6f 6465 6c5d 203d 207b 2769 6427  ][model] = {'id'
-000075a0: 3a20 6964 7d0a 2020 2020 6966 2027 7374  : id}.    if 'st
-000075b0: 6174 6527 2069 6e20 7661 6c73 3a0a 2020  ate' in vals:.  
-000075c0: 2020 2020 2020 7467 745f 6374 785b 275f        tgt_ctx['_
-000075d0: 434f 4d4d 4954 275d 5b6d 6f64 656c 5d5b  COMMIT'][model][
-000075e0: 2773 7461 7465 275d 203d 2076 616c 735b  'state'] = vals[
-000075f0: 2773 7461 7465 275d 0a20 2020 2065 6c69  'state'].    eli
-00007600: 6620 6964 3a0a 2020 2020 2020 2020 7265  f id:.        re
-00007610: 6320 3d20 636c 6f64 6f6f 2e62 726f 7773  c = clodoo.brows
-00007620: 654c 3828 7467 745f 6374 782c 206d 6f64  eL8(tgt_ctx, mod
-00007630: 656c 2c20 6964 290a 2020 2020 2020 2020  el, id).        
-00007640: 6966 2027 7374 6174 6527 2069 6e20 7265  if 'state' in re
-00007650: 633a 0a20 2020 2020 2020 2020 2020 2074  c:.            t
-00007660: 6774 5f63 7478 5b27 5f43 4f4d 4d49 5427  gt_ctx['_COMMIT'
-00007670: 5d5b 6d6f 6465 6c5d 5b27 7374 6174 6527  ][model]['state'
-00007680: 5d20 3d20 7265 632e 7374 6174 650a 2020  ] = rec.state.  
-00007690: 2020 6966 206d 6f64 656c 203d 3d20 2761    if model == 'a
-000076a0: 6363 6f75 6e74 2e69 6e76 6f69 6365 273a  ccount.invoice':
-000076b0: 0a20 2020 2020 2020 2069 6620 7265 633a  .        if rec:
-000076c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000076d0: 7265 632e 7374 6174 6520 3d3d 2027 7061  rec.state == 'pa
-000076e0: 6964 273a 0a20 2020 2020 2020 2020 2020  id':.           
-000076f0: 2020 2020 2072 6574 7572 6e20 7661 6c73       return vals
-00007700: 2c20 2d34 0a20 2020 2020 2020 2020 2020  , -4.           
-00007710: 2065 6c69 6620 7265 632e 7374 6174 6520   elif rec.state 
-00007720: 3d3d 2027 6f70 656e 273a 0a20 2020 2020  == 'open':.     
-00007730: 2020 2020 2020 2020 2020 2069 6420 3d20             id = 
-00007740: 636c 6f64 6f6f 2e65 7865 6375 7465 4c38  clodoo.executeL8
-00007750: 2874 6774 5f63 7478 2c0a 2020 2020 2020  (tgt_ctx,.      
-00007760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007780: 6d6f 6465 6c2c 0a20 2020 2020 2020 2020  model,.         
-00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077a0: 2020 2020 2020 2020 2020 2020 2027 6163               'ac
-000077b0: 7469 6f6e 5f69 6e76 6f69 6365 5f63 616e  tion_invoice_can
-000077c0: 6365 6c27 2c0a 2020 2020 2020 2020 2020  cel',.          
-000077d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077e0: 2020 2020 2020 2020 2020 2020 6964 7329              ids)
-000077f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007800: 2069 6420 3d20 636c 6f64 6f6f 2e65 7865   id = clodoo.exe
-00007810: 6375 7465 4c38 2874 6774 5f63 7478 2c0a  cuteL8(tgt_ctx,.
-00007820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007840: 2020 2020 2020 6d6f 6465 6c2c 0a20 2020        model,.   
-00007850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007870: 2020 2027 6163 7469 6f6e 5f69 6e76 6f69     'action_invoi
-00007880: 6365 5f64 7261 6674 272c 0a20 2020 2020  ce_draft',.     
-00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078b0: 2069 6473 290a 2020 2020 2020 2020 2020   ids).          
-000078c0: 2020 656c 6966 2072 6563 2e73 7461 7465    elif rec.state
-000078d0: 203d 3d20 2763 616e 6365 6c27 3a0a 2020   == 'cancel':.  
-000078e0: 2020 2020 2020 2020 2020 2020 2020 6964                id
-000078f0: 203d 2063 6c6f 646f 6f2e 6578 6563 7574   = clodoo.execut
-00007900: 654c 3828 7467 745f 6374 782c 0a20 2020  eL8(tgt_ctx,.   
-00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007930: 2020 206d 6f64 656c 2c0a 2020 2020 2020     model,.      
-00007940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007960: 2761 6374 696f 6e5f 696e 766f 6963 655f  'action_invoice_
-00007970: 6472 6166 7427 2c0a 2020 2020 2020 2020  draft',.        
-00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007990: 2020 2020 2020 2020 2020 2020 2020 6964                id
-000079a0: 7329 0a20 2020 2020 2020 2076 616c 735b  s).        vals[
-000079b0: 2773 7461 7465 275d 203d 2027 6472 6166  'state'] = 'draf
-000079c0: 7427 0a20 2020 2065 6c69 6620 6d6f 6465  t'.    elif mode
-000079d0: 6c20 3d3d 2027 7361 6c65 2e6f 7264 6572  l == 'sale.order
-000079e0: 273a 0a20 2020 2020 2020 2069 6620 7265  ':.        if re
-000079f0: 633a 0a20 2020 2020 2020 2020 2020 2069  c:.            i
-00007a00: 6620 7265 632e 7374 6174 6520 3d3d 2027  f rec.state == '
-00007a10: 646f 6e65 273a 0a20 2020 2020 2020 2020  done':.         
-00007a20: 2020 2020 2020 2072 6574 7572 6e20 7661         return va
-00007a30: 6c73 2c20 2d34 0a20 2020 2020 2020 2020  ls, -4.         
-00007a40: 2020 2065 6c69 6620 7265 632e 7374 6174     elif rec.stat
-00007a50: 6520 3d3d 2027 7361 6c65 273a 0a20 2020  e == 'sale':.   
-00007a60: 2020 2020 2020 2020 2020 2020 2069 6420               id 
-00007a70: 3d20 636c 6f64 6f6f 2e65 7865 6375 7465  = clodoo.execute
-00007a80: 4c38 2874 6774 5f63 7478 2c0a 2020 2020  L8(tgt_ctx,.    
-00007a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ab0: 2020 6d6f 6465 6c2c 0a20 2020 2020 2020    model,.       
-00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ad0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00007ae0: 6163 7469 6f6e 5f63 616e 6365 6c27 2c0a  action_cancel',.
-00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b10: 2020 2020 2020 6964 7329 0a20 2020 2020        ids).     
-00007b20: 2020 2020 2020 2020 2020 2069 6420 3d20             id = 
-00007b30: 636c 6f64 6f6f 2e65 7865 6375 7465 4c38  clodoo.executeL8
-00007b40: 2874 6774 5f63 7478 2c0a 2020 2020 2020  (tgt_ctx,.      
-00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b70: 6d6f 6465 6c2c 0a20 2020 2020 2020 2020  model,.         
-00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b90: 2020 2020 2020 2020 2020 2020 2027 6163               'ac
-00007ba0: 7469 6f6e 5f64 7261 6674 272c 0a20 2020  tion_draft',.   
-00007bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bd0: 2020 2069 6473 290a 2020 2020 2020 2020     ids).        
-00007be0: 2020 2020 656c 6966 2072 6563 2e73 7461      elif rec.sta
-00007bf0: 7465 203d 3d20 2763 616e 6365 6c27 3a0a  te == 'cancel':.
-00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c10: 6964 203d 2063 6c6f 646f 6f2e 6578 6563  id = clodoo.exec
-00007c20: 7574 654c 3828 7467 745f 6374 782c 0a20  uteL8(tgt_ctx,. 
-00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c50: 2020 2020 206d 6f64 656c 2c0a 2020 2020       model,.    
-00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c80: 2020 2761 6374 696f 6e5f 6472 6166 7427    'action_draft'
-00007c90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cb0: 2020 2020 2020 2020 6964 7329 0a20 2020          ids).   
-00007cc0: 2020 2020 2076 616c 735b 2773 7461 7465       vals['state
-00007cd0: 275d 203d 2027 6472 6166 7427 0a20 2020  '] = 'draft'.   
-00007ce0: 2072 6574 7572 6e20 7661 6c73 2c20 300a   return vals, 0.
-00007cf0: 0a0a 6465 6620 636f 6d6d 6974 5f74 6162  ..def commit_tab
-00007d00: 6c65 2874 6774 5f63 7478 2c20 7372 635f  le(tgt_ctx, src_
-00007d10: 6374 782c 206d 6f64 656c 293a 0a20 2020  ctx, model):.   
-00007d20: 2069 6420 3d20 4661 6c73 650a 2020 2020   id = False.    
-00007d30: 6966 2074 6774 5f63 7478 5b27 5f43 4f4d  if tgt_ctx['_COM
-00007d40: 4d49 5427 5d2e 6765 7428 6d6f 6465 6c29  MIT'].get(model)
-00007d50: 3a0a 2020 2020 2020 2020 6964 203d 2074  :.        id = t
-00007d60: 6774 5f63 7478 5b27 5f43 4f4d 4d49 5427  gt_ctx['_COMMIT'
-00007d70: 5d5b 6d6f 6465 6c5d 5b27 6964 275d 0a20  ][model]['id']. 
-00007d80: 2020 2020 2020 2069 6620 7573 655f 7379         if use_sy
-00007d90: 6e63 6872 6f28 7467 745f 6374 782c 206d  nchro(tgt_ctx, m
-00007da0: 6f64 656c 293a 0a20 2020 2020 2020 2020  odel):.         
-00007db0: 2020 2069 6420 3d20 636c 6f64 6f6f 2e65     id = clodoo.e
-00007dc0: 7865 6375 7465 4c38 2874 6774 5f63 7478  xecuteL8(tgt_ctx
-00007dd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007df0: 2020 2020 6d6f 6465 6c2c 0a20 2020 2020      model,.     
-00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e10: 2020 2020 2020 2020 2020 2020 2027 636f               'co
-00007e20: 6d6d 6974 272c 0a20 2020 2020 2020 2020  mmit',.         
-00007e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e40: 2020 2020 2020 2020 2069 6429 0a20 2020           id).   
-00007e50: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00007e60: 2020 2020 2020 2073 6574 5f61 6374 7561         set_actua
-00007e70: 6c5f 7374 6174 6528 0a20 2020 2020 2020  l_state(.       
-00007e80: 2020 2020 2020 2020 2074 6774 5f63 7478           tgt_ctx
-00007e90: 2c20 6d6f 6465 6c2c 2069 642c 2074 6774  , model, id, tgt
-00007ea0: 5f63 7478 5b27 5f43 4f4d 4d49 5427 5d5b  _ctx['_COMMIT'][
-00007eb0: 6d6f 6465 6c5d 5b27 7374 6174 6527 5d29  model]['state'])
-00007ec0: 0a20 2020 2074 6774 5f63 7478 5b27 5f43  .    tgt_ctx['_C
-00007ed0: 4f4d 4d49 5427 5d5b 6d6f 6465 6c5d 203d  OMMIT'][model] =
-00007ee0: 2046 616c 7365 0a20 2020 2072 6574 7572   False.    retur
-00007ef0: 6e20 6964 0a0a 0a64 6566 2073 796e 6368  n id...def synch
-00007f00: 726f 2874 6774 5f63 7478 2c20 6d6f 6465  ro(tgt_ctx, mode
-00007f10: 6c2c 2076 616c 7329 3a0a 2020 2020 7467  l, vals):.    tg
-00007f20: 745f 6374 785b 275f 434f 4d4d 4954 275d  t_ctx['_COMMIT']
-00007f30: 5b6d 6f64 656c 5d20 3d20 4661 6c73 650a  [model] = False.
-00007f40: 2020 2020 6361 6368 6520 3d20 6765 745f      cache = get_
-00007f50: 6361 6368 6528 7372 635f 6374 7829 0a20  cache(src_ctx). 
-00007f60: 2020 2023 2069 6620 2763 6f6d 7061 6e79     # if 'company
-00007f70: 5f69 6427 2069 6e20 7661 6c73 2061 6e64  _id' in vals and
-00007f80: 2074 6774 5f63 7478 2e67 6574 2827 6279   tgt_ctx.get('by
-00007f90: 5f63 6f6d 7061 6e79 2729 3a0a 2020 2020  _company'):.    
-00007fa0: 2320 2020 2020 7661 6c73 5b27 636f 6d70  #     vals['comp
-00007fb0: 616e 795f 6964 275d 203d 2074 6774 5f63  any_id'] = tgt_c
-00007fc0: 7478 5b27 636f 6d70 616e 795f 6964 275d  tx['company_id']
-00007fd0: 0a20 2020 2069 6420 3d20 7365 6172 6368  .    id = search
-00007fe0: 3472 6563 2874 6774 5f63 7478 2c20 6d6f  4rec(tgt_ctx, mo
-00007ff0: 6465 6c2c 2076 616c 7329 0a20 2020 2069  del, vals).    i
-00008000: 6620 6964 203e 2030 3a0a 2020 2020 2020  f id > 0:.      
-00008010: 2020 7661 6c73 2c20 7374 7320 3d20 7365    vals, sts = se
-00008020: 745f 7374 6174 655f 746f 5f64 7261 6674  t_state_to_draft
-00008030: 2874 6774 5f63 7478 2c20 6d6f 6465 6c2c  (tgt_ctx, model,
-00008040: 205b 6964 5d2c 2076 616c 7329 0a20 2020   [id], vals).   
-00008050: 2020 2020 2077 7269 7465 5f6e 6f5f 6475       write_no_du
-00008060: 7028 7467 745f 6374 782c 206d 6f64 656c  p(tgt_ctx, model
-00008070: 2c20 5b69 645d 2c20 7661 6c73 2c20 6964  , [id], vals, id
-00008080: 290a 2020 2020 2020 2020 6361 6368 655f  ).        cache_
-00008090: 7374 6f72 655f 656e 7472 7928 6361 6368  store_entry(cach
-000080a0: 652c 206d 6f64 656c 2c20 6964 290a 2020  e, model, id).  
-000080b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000080c0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-000080d0: 2076 616c 732c 2073 7473 203d 2073 6574   vals, sts = set
-000080e0: 5f73 7461 7465 5f74 6f5f 6472 6166 7428  _state_to_draft(
-000080f0: 7467 745f 6374 782c 206d 6f64 656c 2c20  tgt_ctx, model, 
-00008100: 4661 6c73 652c 2076 616c 7329 0a20 2020  False, vals).   
-00008110: 2020 2020 2020 2020 2069 6420 3d20 636c           id = cl
-00008120: 6f64 6f6f 2e63 7265 6174 654c 3828 7467  odoo.createL8(tg
-00008130: 745f 6374 782c 206d 6f64 656c 2c20 7661  t_ctx, model, va
-00008140: 6c73 290a 2020 2020 2020 2020 2020 2020  ls).            
-00008150: 6361 6368 655f 7374 6f72 655f 656e 7472  cache_store_entr
-00008160: 7928 6361 6368 652c 206d 6f64 656c 2c20  y(cache, model, 
-00008170: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
-00008180: 7467 745f 6374 785b 275f 434f 4d4d 4954  tgt_ctx['_COMMIT
-00008190: 275d 5b6d 6f64 656c 5d5b 2769 6427 5d20  '][model]['id'] 
-000081a0: 3d20 6964 0a20 2020 2020 2020 2065 7863  = id.        exc
-000081b0: 6570 7420 494f 4572 726f 7220 6173 2065  ept IOError as e
-000081c0: 3a0a 2020 2020 2020 2020 2020 2020 6f73  :.            os
-000081d0: 302e 776c 6f67 2827 2573 2043 616e 6e6f  0.wlog('%s Canno
-000081e0: 7420 6372 6561 7465 2025 7320 7372 6320  t create %s src 
-000081f0: 6964 3d25 6427 2025 2028 652c 206d 6f64  id=%d' % (e, mod
-00008200: 656c 2c20 6964 2929 0a20 2020 2020 2020  el, id)).       
-00008210: 2020 2020 206d 616e 6167 655f 6572 726f       manage_erro
-00008220: 7228 290a 0a0a 0a64 6566 2073 6561 7263  r()....def searc
-00008230: 6834 7265 6328 7467 745f 6374 782c 206d  h4rec(tgt_ctx, m
-00008240: 6f64 656c 2c20 7661 6c73 293a 0a0a 2020  odel, vals):..  
-00008250: 2020 6465 6620 6469 6d5f 7465 7874 2874    def dim_text(t
-00008260: 6578 7429 3a0a 2020 2020 2020 2020 6966  ext):.        if
-00008270: 2074 6578 743a 0a20 2020 2020 2020 2020   text:.         
-00008280: 2020 2074 6578 7420 3d20 756e 6964 6563     text = unidec
-00008290: 6f64 6528 7465 7874 292e 7374 7269 7028  ode(text).strip(
-000082a0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-000082b0: 7320 3d20 2727 0a20 2020 2020 2020 2020  s = ''.         
-000082c0: 2020 2066 6f72 2063 6820 696e 2074 6578     for ch in tex
-000082d0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-000082e0: 2020 2069 6620 6368 2e69 7361 6c6e 756d     if ch.isalnum
-000082f0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00008300: 2020 2020 2020 2020 7265 7320 2b3d 2063          res += c
-00008310: 682e 6c6f 7765 7228 290a 2020 2020 2020  h.lower().      
-00008320: 2020 2020 2020 7465 7874 203d 2072 6573        text = res
-00008330: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008340: 7465 7874 0a0a 2020 2020 636f 6d70 616e  text..    compan
-00008350: 795f 6964 203d 2020 7467 745f 6374 782e  y_id =  tgt_ctx.
-00008360: 6765 7428 2763 6f6d 7061 6e79 5f69 6427  get('company_id'
-00008370: 2c20 4661 6c73 6529 0a20 2020 2069 6420  , False).    id 
-00008380: 3d20 2d31 0a20 2020 2066 6f72 206b 6579  = -1.    for key
-00008390: 7320 696e 2074 6774 5f63 7478 5b27 5f6b  s in tgt_ctx['_k
-000083a0: 6c27 5d5b 6d6f 6465 6c5d 3a0a 2020 2020  l'][model]:.    
-000083b0: 2020 2020 7768 6572 6520 3d20 5b5d 0a20      where = []. 
-000083c0: 2020 2020 2020 2066 6f72 206b 6579 2069         for key i
-000083d0: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
-000083e0: 2020 2020 6966 2028 6b65 7920 6e6f 7420      if (key not 
-000083f0: 696e 2076 616c 7320 616e 640a 2020 2020  in vals and.    
-00008400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008410: 6b65 7920 3d3d 2027 6469 6d5f 6e61 6d65  key == 'dim_name
-00008420: 2720 616e 640a 2020 2020 2020 2020 2020  ' and.          
-00008430: 2020 2020 2020 2020 2020 7661 6c73 2e67            vals.g
-00008440: 6574 2827 6e61 6d65 2729 293a 0a20 2020  et('name')):.   
-00008450: 2020 2020 2020 2020 2020 2020 2077 6865               whe
-00008460: 7265 2e61 7070 656e 6428 2827 6469 6d5f  re.append(('dim_
-00008470: 6e61 6d65 272c 0a20 2020 2020 2020 2020  name',.         
-00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008490: 2020 2020 2027 3d27 2c0a 2020 2020 2020       '=',.      
-000084a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084b0: 2020 2020 2020 2020 6469 6d5f 7465 7874          dim_text
-000084c0: 2876 616c 735b 276e 616d 6527 5d29 2929  (vals['name'])))
-000084d0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-000084e0: 6620 6b65 7920 6e6f 7420 696e 2076 616c  f key not in val
-000084f0: 7320 616e 6420 6b65 7920 3d3d 2027 636f  s and key == 'co
-00008500: 6d70 616e 795f 6964 273a 0a20 2020 2020  mpany_id':.     
-00008510: 2020 2020 2020 2020 2020 2077 6865 7265             where
-00008520: 2e61 7070 656e 6428 286b 6579 2c20 273d  .append((key, '=
-00008530: 272c 2063 6f6d 7061 6e79 5f69 6429 290a  ', company_id)).
-00008540: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00008550: 206b 6579 206e 6f74 2069 6e20 7661 6c73   key not in vals
-00008560: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008570: 2020 7768 6572 6520 3d20 5b5d 0a20 2020    where = [].   
-00008580: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-00008590: 616b 0a20 2020 2020 2020 2020 2020 2065  ak.            e
-000085a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000085b0: 2020 2020 2077 6865 7265 2e61 7070 656e       where.appen
-000085c0: 6428 286b 6579 2c20 273d 272c 2076 616c  d((key, '=', val
-000085d0: 735b 6b65 795d 2929 0a20 2020 2020 2020  s[key])).       
-000085e0: 2069 6620 7768 6572 653a 0a20 2020 2020   if where:.     
-000085f0: 2020 2020 2020 2069 6473 203d 2063 6c6f         ids = clo
-00008600: 646f 6f2e 7365 6172 6368 4c38 2874 6774  doo.searchL8(tgt
-00008610: 5f63 7478 2c20 6d6f 6465 6c2c 2077 6865  _ctx, model, whe
-00008620: 7265 290a 2020 2020 2020 2020 2020 2020  re).            
-00008630: 6966 206e 6f74 2069 6473 2061 6e64 2027  if not ids and '
-00008640: 6163 7469 7665 2720 696e 2074 6774 5f63  active' in tgt_c
-00008650: 7478 5b27 5354 5255 4354 275d 5b6d 6f64  tx['STRUCT'][mod
-00008660: 656c 5d3a 0a20 2020 2020 2020 2020 2020  el]:.           
-00008670: 2020 2020 2077 6865 7265 2e61 7070 656e       where.appen
-00008680: 6428 2827 6163 7469 7665 272c 2027 3d27  d(('active', '='
-00008690: 2c20 4661 6c73 6529 290a 2020 2020 2020  , False)).      
-000086a0: 2020 2020 2020 2020 2020 6964 7320 3d20            ids = 
-000086b0: 636c 6f64 6f6f 2e73 6561 7263 684c 3828  clodoo.searchL8(
-000086c0: 7467 745f 6374 782c 206d 6f64 656c 2c20  tgt_ctx, model, 
-000086d0: 7768 6572 6529 0a20 2020 2020 2020 2020  where).         
-000086e0: 2020 2069 6620 6964 733a 0a20 2020 2020     if ids:.     
-000086f0: 2020 2020 2020 2020 2020 2069 6420 3d20             id = 
-00008700: 6964 735b 305d 0a20 2020 2020 2020 2020  ids[0].         
-00008710: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-00008720: 2072 6574 7572 6e20 6964 0a0a 0a64 6566   return id...def
-00008730: 2063 6f70 795f 7265 636f 7264 2874 6774   copy_record(tgt
-00008740: 5f63 7478 2c20 7372 635f 6374 782c 206d  _ctx, src_ctx, m
-00008750: 6f64 656c 2c20 7265 632c 206d 6f64 653d  odel, rec, mode=
-00008760: 4e6f 6e65 293a 0a20 2020 206d 7367 5f62  None):.    msg_b
-00008770: 7572 7374 2827 2573 2025 6427 2025 2028  urst('%s %d' % (
-00008780: 6d6f 6465 6c2c 2072 6563 2e69 6429 290a  model, rec.id)).
-00008790: 2020 2020 6d6f 6465 203d 206d 6f64 6520      mode = mode 
-000087a0: 6f72 2067 6574 5f6d 6f64 656c 5f63 6f70  or get_model_cop
-000087b0: 795f 6d6f 6465 2873 7263 5f63 7478 2c20  y_mode(src_ctx, 
-000087c0: 6d6f 6465 6c29 0a20 2020 2023 2041 766f  model).    # Avo
-000087d0: 6964 206c 6f6f 7020 6e65 7374 696e 670a  id loop nesting.
-000087e0: 2020 2020 6361 6368 6520 3d20 6765 745f      cache = get_
-000087f0: 6361 6368 6528 7372 635f 6374 7829 0a20  cache(src_ctx). 
-00008800: 2020 2069 6620 6361 6368 655f 6973 5f65     if cache_is_e
-00008810: 6e74 7279 2863 6163 6865 2c20 6d6f 6465  ntry(cache, mode
-00008820: 6c2c 2072 6563 2e69 6429 3a0a 2020 2020  l, rec.id):.    
-00008830: 2020 2020 7265 7475 726e 0a20 2020 2063      return.    c
-00008840: 6163 6865 5f73 746f 7265 5f65 6e74 7279  ache_store_entry
-00008850: 2863 6163 6865 2c20 6d6f 6465 6c2c 2046  (cache, model, F
-00008860: 616c 7365 2c20 6b65 6570 3d54 7275 6529  alse, keep=True)
-00008870: 0a20 2020 2076 616c 7320 3d20 6c6f 6164  .    vals = load
-00008880: 5f72 6563 6f72 6428 7467 745f 6374 782c  _record(tgt_ctx,
-00008890: 2073 7263 5f63 7478 2c20 6d6f 6465 6c2c   src_ctx, model,
-000088a0: 2072 6563 2c20 6d6f 6465 3d6d 6f64 6529   rec, mode=mode)
-000088b0: 0a20 2020 2069 6620 6e6f 7420 7661 6c73  .    if not vals
-000088c0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000088d0: 0a20 2020 2069 6620 6d6f 6465 203d 3d20  .    if mode == 
-000088e0: 2769 6d61 6765 273a 0a20 2020 2020 2020  'image':.       
-000088f0: 2069 6473 203d 2063 6c6f 646f 6f2e 7365   ids = clodoo.se
-00008900: 6172 6368 4c38 2874 6774 5f63 7478 2c20  archL8(tgt_ctx, 
-00008910: 6d6f 6465 6c2c 0a20 2020 2020 2020 2020  model,.         
-00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008930: 2020 2020 205b 2827 6964 272c 2027 3d27       [('id', '='
-00008940: 2c20 7265 632e 6964 295d 290a 2020 2020  , rec.id)]).    
-00008950: 2020 2020 6966 2069 6473 3a0a 2020 2020      if ids:.    
-00008960: 2020 2020 2020 2020 7772 6974 655f 6e6f          write_no
-00008970: 5f64 7570 2874 6774 5f63 7478 2c20 6d6f  _dup(tgt_ctx, mo
-00008980: 6465 6c2c 2069 6473 2c20 7661 6c73 2c20  del, ids, vals, 
-00008990: 7265 632e 6964 290a 2020 2020 2020 2020  rec.id).        
-000089a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000089b0: 2020 6964 203d 2063 7265 6174 655f 7769    id = create_wi
-000089c0: 7468 5f69 6428 7467 745f 6374 782c 206d  th_id(tgt_ctx, m
-000089d0: 6f64 656c 2c20 7265 632e 6964 2c20 7661  odel, rec.id, va
-000089e0: 6c73 290a 2020 2020 656c 6966 2075 7365  ls).    elif use
-000089f0: 5f73 796e 6368 726f 2874 6774 5f63 7478  _synchro(tgt_ctx
-00008a00: 2c20 6d6f 6465 6c29 3a0a 2020 2020 2020  , model):.      
-00008a10: 2020 7661 6c73 5b27 6f65 375f 6964 275d    vals['oe7_id']
-00008a20: 203d 2072 6563 2e69 640a 2020 2020 2020   = rec.id.      
-00008a30: 2020 6964 203d 2063 6c6f 646f 6f2e 6578    id = clodoo.ex
-00008a40: 6563 7574 654c 3828 7467 745f 6374 782c  ecuteL8(tgt_ctx,
-00008a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008a60: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00008a70: 6f64 656c 2c0a 2020 2020 2020 2020 2020  odel,.          
-00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a90: 2020 2020 2773 796e 6368 726f 272c 0a20      'synchro',. 
-00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ab0: 2020 2020 2020 2020 2020 2020 2076 616c               val
-00008ac0: 7329 0a20 2020 2065 6c73 653a 0a20 2020  s).    else:.   
-00008ad0: 2020 2020 2073 796e 6368 726f 2874 6774       synchro(tgt
-00008ae0: 5f63 7478 2c20 6d6f 6465 6c2c 2076 616c  _ctx, model, val
-00008af0: 7329 0a0a 0a64 6566 2064 6574 6169 6c5f  s)...def detail_
-00008b00: 6d6f 6465 6c28 6d6f 6465 6c29 3a0a 2020  model(model):.  
-00008b10: 2020 6966 206d 6f64 656c 2069 6e20 2827    if model in ('
-00008b20: 6163 636f 756e 742e 696e 766f 6963 6527  account.invoice'
-00008b30: 2c20 2773 616c 652e 6f72 6465 7227 293a  , 'sale.order'):
-00008b40: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008b50: 2725 732e 6c69 6e65 2720 2520 6d6f 6465  '%s.line' % mode
-00008b60: 6c0a 2020 2020 7265 7475 726e 2046 616c  l.    return Fal
-00008b70: 7365 0a0a 0a64 6566 2073 6574 5f77 6865  se...def set_whe
-00008b80: 7265 5f66 726f 6d5f 7478 7469 6473 2876  re_from_txtids(v
-00008b90: 616c 7565 293a 0a20 2020 2077 6865 7265  alue):.    where
-00008ba0: 203d 205b 5d0a 2020 2020 6966 2076 616c   = [].    if val
-00008bb0: 7565 3a0a 2020 2020 2020 2020 6964 7320  ue:.        ids 
-00008bc0: 3d20 6576 616c 2876 616c 7565 290a 2020  = eval(value).  
-00008bd0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00008be0: 6e63 6528 6964 732c 2028 696e 742c 206c  nce(ids, (int, l
-00008bf0: 6f6e 6729 293a 0a20 2020 2020 2020 2020  ong)):.         
-00008c00: 2020 2077 6865 7265 2e61 7070 656e 6428     where.append(
-00008c10: 2827 6964 272c 2027 3d27 2c20 6964 7329  ('id', '=', ids)
-00008c20: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00008c30: 2020 2020 2020 2020 2020 2020 7768 6572              wher
-00008c40: 652e 6170 7065 6e64 2828 2769 6427 2c20  e.append(('id', 
-00008c50: 2769 6e27 2c20 6964 7329 290a 2020 2020  'in', ids)).    
-00008c60: 7265 7475 726e 2077 6865 7265 0a0a 0a64  return where...d
-00008c70: 6566 2063 6f70 795f 7461 626c 6528 7467  ef copy_table(tg
-00008c80: 745f 6374 782c 2073 7263 5f63 7478 2c20  t_ctx, src_ctx, 
-00008c90: 6d6f 6465 6c2c 206d 6f64 653d 4e6f 6e65  model, mode=None
-00008ca0: 293a 0a20 2020 2063 6c6f 646f 6f2e 6765  ):.    clodoo.ge
-00008cb0: 745f 6d6f 6465 6c5f 7374 7275 6374 7572  t_model_structur
-00008cc0: 6528 0a20 2020 2020 2020 2073 7263 5f63  e(.        src_c
-00008cd0: 7478 2c20 6d6f 6465 6c2c 0a20 2020 2020  tx, model,.     
-00008ce0: 2020 2069 676e 6f72 653d 4947 4e4f 5245     ignore=IGNORE
-00008cf0: 5f46 4945 4c44 532e 6765 7428 6d6f 6465  _FIELDS.get(mode
-00008d00: 6c2c 205b 5d29 202b 2049 474e 4f52 455f  l, []) + IGNORE_
-00008d10: 4649 454c 4453 5b27 2a27 5d29 0a20 2020  FIELDS['*']).   
-00008d20: 2063 6c6f 646f 6f2e 6765 745f 6d6f 6465   clodoo.get_mode
-00008d30: 6c5f 7374 7275 6374 7572 6528 0a20 2020  l_structure(.   
-00008d40: 2020 2020 2074 6774 5f63 7478 2c20 6d6f       tgt_ctx, mo
-00008d50: 6465 6c2c 0a20 2020 2020 2020 2069 676e  del,.        ign
-00008d60: 6f72 653d 4947 4e4f 5245 5f46 4945 4c44  ore=IGNORE_FIELD
-00008d70: 532e 6765 7428 6d6f 6465 6c2c 205b 5d29  S.get(model, [])
-00008d80: 202b 2049 474e 4f52 455f 4649 454c 4453   + IGNORE_FIELDS
-00008d90: 5b27 2a27 5d29 0a20 2020 2064 6574 5f6d  ['*']).    det_m
-00008da0: 6f64 656c 203d 2064 6574 6169 6c5f 6d6f  odel = detail_mo
-00008db0: 6465 6c28 6d6f 6465 6c29 0a20 2020 2069  del(model).    i
-00008dc0: 6620 6465 745f 6d6f 6465 6c3a 0a20 2020  f det_model:.   
-00008dd0: 2020 2020 2063 6c6f 646f 6f2e 6765 745f       clodoo.get_
-00008de0: 6d6f 6465 6c5f 7374 7275 6374 7572 6528  model_structure(
-00008df0: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
-00008e00: 5f63 7478 2c20 6465 745f 6d6f 6465 6c2c  _ctx, det_model,
-00008e10: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
-00008e20: 6f72 653d 4947 4e4f 5245 5f46 4945 4c44  ore=IGNORE_FIELD
-00008e30: 532e 6765 7428 6465 745f 6d6f 6465 6c2c  S.get(det_model,
-00008e40: 205b 5d29 202b 2049 474e 4f52 455f 4649   []) + IGNORE_FI
-00008e50: 454c 4453 5b27 2a27 5d29 0a20 2020 2020  ELDS['*']).     
-00008e60: 2020 2063 6c6f 646f 6f2e 6765 745f 6d6f     clodoo.get_mo
-00008e70: 6465 6c5f 7374 7275 6374 7572 6528 0a20  del_structure(. 
-00008e80: 2020 2020 2020 2020 2020 2074 6774 5f63             tgt_c
-00008e90: 7478 2c20 6465 745f 6d6f 6465 6c2c 0a20  tx, det_model,. 
-00008ea0: 2020 2020 2020 2020 2020 2069 676e 6f72             ignor
-00008eb0: 653d 4947 4e4f 5245 5f46 4945 4c44 532e  e=IGNORE_FIELDS.
-00008ec0: 6765 7428 6465 745f 6d6f 6465 6c2c 205b  get(det_model, [
-00008ed0: 5d29 202b 2049 474e 4f52 455f 4649 454c  ]) + IGNORE_FIEL
-00008ee0: 4453 5b27 2a27 5d29 0a20 2020 2074 6774  DS['*']).    tgt
-00008ef0: 5f63 7478 5b27 5f43 4f4d 4d49 5427 5d20  _ctx['_COMMIT'] 
-00008f00: 3d20 7b7d 0a0a 2020 2020 6d6f 6465 203d  = {}..    mode =
-00008f10: 206d 6f64 6520 6f72 2067 6574 5f6d 6f64   mode or get_mod
-00008f20: 656c 5f63 6f70 795f 6d6f 6465 2873 7263  el_copy_mode(src
-00008f30: 5f63 7478 2c20 6d6f 6465 6c29 0a20 2020  _ctx, model).   
-00008f40: 2069 6620 6d6f 6465 203d 3d20 2769 6d61   if mode == 'ima
-00008f50: 6765 2720 616e 6420 7372 635f 6374 785b  ge' and src_ctx[
-00008f60: 275f 6372 275d 3a0a 2020 2020 2020 2020  '_cr']:.        
-00008f70: 7461 626c 6520 3d20 6d6f 6465 6c2e 7265  table = model.re
-00008f80: 706c 6163 6528 272e 272c 2027 5f27 290a  place('.', '_').
-00008f90: 2020 2020 2020 2020 7371 6c20 3d20 2773          sql = 's
-00008fa0: 656c 6563 7420 6d61 7828 6964 2920 6672  elect max(id) fr
-00008fb0: 6f6d 2025 733b 2720 2520 7461 626c 650a  om %s;' % table.
-00008fc0: 2020 2020 2020 2020 726f 7773 203d 2065          rows = e
-00008fd0: 7865 635f 7371 6c28 7372 635f 6374 782c  xec_sql(src_ctx,
-00008fe0: 2073 716c 2c20 7265 7370 6f6e 7365 3d54   sql, response=T
-00008ff0: 7275 6529 0a20 2020 2020 2020 206c 6173  rue).        las
-00009000: 745f 6964 203d 2072 6f77 735b 305d 5b30  t_id = rows[0][0
-00009010: 5d0a 2020 2020 2020 2020 6966 206c 6173  ].        if las
-00009020: 745f 6964 203e 2030 3a0a 2020 2020 2020  t_id > 0:.      
-00009030: 2020 2020 2020 666f 7220 6964 2069 6e20        for id in 
-00009040: 636c 6f64 6f6f 2e73 6561 7263 684c 3828  clodoo.searchL8(
-00009050: 7467 745f 6374 782c 206d 6f64 656c 2c0a  tgt_ctx, model,.
-00009060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009080: 2020 2020 2020 5b28 2769 6427 2c20 273e        [('id', '>
-00009090: 272c 206c 6173 745f 6964 295d 293a 0a20  ', last_id)]):. 
-000090a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000090b0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-000090c0: 2020 2020 2020 2020 636c 6f64 6f6f 2e75          clodoo.u
-000090d0: 6e6c 696e 6b4c 3828 7467 745f 6374 782c  nlinkL8(tgt_ctx,
-000090e0: 206d 6f64 656c 2c20 6964 290a 2020 2020   model, id).    
-000090f0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00009100: 7074 2049 4f45 7272 6f72 3a0a 2020 2020  pt IOError:.    
-00009110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009120: 6f73 302e 776c 6f67 2822 4361 6e6e 6f74  os0.wlog("Cannot
-00009130: 2064 656c 6574 6520 7265 636f 7264 2025   delete record %
-00009140: 6420 6f66 2025 7322 2025 2028 6964 2c20  d of %s" % (id, 
-00009150: 6d6f 6465 6c29 290a 2020 2020 2020 2020  model)).        
-00009160: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00009170: 6f74 2074 6774 5f63 7478 5b27 6173 7375  ot tgt_ctx['assu
-00009180: 6d65 5f79 6573 275d 3a0a 2020 2020 2020  me_yes']:.      
-00009190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091a0: 2020 6475 6d6d 7920 3d20 696e 7075 7428    dummy = input(
-000091b0: 2750 7265 7373 2052 4554 2074 6f20 636f  'Press RET to co
-000091c0: 6e74 696e 7565 2729 0a20 2020 2077 6865  ntinue').    whe
-000091d0: 7265 203d 2073 6574 5f77 6865 7265 5f66  re = set_where_f
-000091e0: 726f 6d5f 7478 7469 6473 2873 7263 5f63  rom_txtids(src_c
-000091f0: 7478 5b27 7365 6c5f 6964 7327 5d29 0a20  tx['sel_ids']). 
-00009200: 2020 2069 6620 7372 635f 6374 785b 2762     if src_ctx['b
-00009210: 795f 636f 6d70 616e 7927 5d3a 0a20 2020  y_company']:.   
-00009220: 2020 2020 2063 6f6d 7061 6e79 5f69 6420       company_id 
-00009230: 3d20 656e 765f 7265 6628 7372 635f 6374  = env_ref(src_ct
-00009240: 782c 2027 7a30 6275 672e 6d79 636f 6d70  x, 'z0bug.mycomp
-00009250: 616e 7927 290a 2020 2020 2020 2020 6966  any').        if
-00009260: 206e 6f74 2063 6f6d 7061 6e79 5f69 643a   not company_id:
-00009270: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00009280: 6e74 2827 2121 496e 7465 726e 616c 2065  nt('!!Internal e
-00009290: 7272 6f72 3a20 6e6f 2063 6f6d 7061 6e79  rror: no company
-000092a0: 2066 6f75 6e64 2127 290a 2020 2020 2020   found!').      
-000092b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000092c0: 2020 2020 7768 6572 652e 6170 7065 6e64      where.append
-000092d0: 2828 2763 6f6d 7061 6e79 5f69 6427 2c20  (('company_id', 
-000092e0: 273d 272c 2063 6f6d 7061 6e79 5f69 6429  '=', company_id)
-000092f0: 290a 2020 2020 666f 7220 7265 6320 696e  ).    for rec in
-00009300: 2063 6c6f 646f 6f2e 6272 6f77 7365 4c38   clodoo.browseL8
-00009310: 280a 2020 2020 2020 2020 7372 635f 6374  (.        src_ct
-00009320: 782c 206d 6f64 656c 2c20 636c 6f64 6f6f  x, model, clodoo
-00009330: 2e73 6561 7263 684c 3828 0a20 2020 2020  .searchL8(.     
-00009340: 2020 2020 2020 2073 7263 5f63 7478 2c20         src_ctx, 
-00009350: 6d6f 6465 6c2c 2077 6865 7265 2c20 6f72  model, where, or
-00009360: 6465 723d 2769 6427 292c 2063 6f6e 7465  der='id'), conte
-00009370: 7874 3d7b 276c 616e 6727 3a20 2765 6e5f  xt={'lang': 'en_
-00009380: 5553 277d 293a 0a20 2020 2020 2020 2063  US'}):.        c
-00009390: 6f70 795f 7265 636f 7264 2874 6774 5f63  opy_record(tgt_c
-000093a0: 7478 2c20 7372 635f 6374 782c 206d 6f64  tx, src_ctx, mod
-000093b0: 656c 2c20 7265 632c 206d 6f64 653d 6d6f  el, rec, mode=mo
-000093c0: 6465 290a 2020 2020 2020 2020 6966 2064  de).        if d
-000093d0: 6574 5f6d 6f64 656c 3a0a 2020 2020 2020  et_model:.      
-000093e0: 2020 2020 2020 6465 745f 6669 656c 6420        det_field 
-000093f0: 3d20 7472 616e 736f 646f 6f2e 7472 616e  = transodoo.tran
-00009400: 736c 6174 655f 6672 6f6d 5f74 6f28 7372  slate_from_to(sr
-00009410: 635f 6374 782c 0a20 2020 2020 2020 2020  c_ctx,.         
-00009420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009440: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-00009450: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00009460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009480: 2020 2020 2020 4445 545f 4649 454c 445b        DET_FIELD[
-00009490: 6d6f 6465 6c5d 2c0a 2020 2020 2020 2020  model],.        
-000094a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094c0: 2020 2020 2020 2020 2020 2020 2737 2e30              '7.0
-000094d0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00005840: 2020 2020 2020 2027 6175 7468 6f72 273a         'author':
+00005850: 206d 6f64 756c 655f 7372 632e 6175 7468   module_src.auth
+00005860: 6f72 2c0a 2020 2020 2020 2020 2020 2020  or,.            
+00005870: 2020 2020 2020 2020 2020 2020 2764 656d              'dem
+00005880: 6f27 3a20 6d6f 6475 6c65 5f73 7263 2e64  o': module_src.d
+00005890: 656d 6f2c 0a20 2020 2020 2020 2020 2020  emo,.           
+000058a0: 2020 2020 2020 2020 2020 2020 2027 6465               'de
+000058b0: 7363 7269 7074 696f 6e27 3a20 6d6f 6475  scription': modu
+000058c0: 6c65 5f73 7263 2e64 6573 6372 6970 7469  le_src.descripti
+000058d0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+000058e0: 2020 2020 2020 2020 2020 2020 2773 756d              'sum
+000058f0: 6d61 7279 273a 206d 6f64 756c 655f 7372  mary': module_sr
+00005900: 632e 7375 6d6d 6172 792c 0a20 2020 2020  c.summary,.     
+00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005920: 2020 2027 7374 6174 6527 3a20 2774 6f20     'state': 'to 
+00005930: 696e 7374 616c 6c27 2c0a 2020 2020 2020  install',.      
+00005940: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005960: 2020 2020 636c 6f64 6f6f 2e63 7265 6174      clodoo.creat
+00005970: 654c 3828 7467 745f 6374 782c 206d 6f64  eL8(tgt_ctx, mod
+00005980: 656c 2c20 7661 6c73 290a 2020 2020 2020  el, vals).      
+00005990: 2020 656c 6966 2075 7067 7261 6465 3a0a    elif upgrade:.
+000059a0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+000059b0: 6c6f 646f 6f2e 7365 6172 6368 4c38 280a  lodoo.searchL8(.
+000059c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059d0: 7467 745f 6374 782c 206d 6f64 656c 2c20  tgt_ctx, model, 
+000059e0: 5b28 276e 616d 6527 2c20 273d 272c 206d  [('name', '=', m
+000059f0: 6f64 756c 6529 2c20 2827 7374 6174 6527  odule), ('state'
+00005a00: 2c20 273d 272c 2027 696e 7374 616c 6c65  , '=', 'installe
+00005a10: 6427 295d 0a20 2020 2020 2020 2020 2020  d')].           
+00005a20: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+00005a30: 2020 2020 7374 7320 3d20 636c 6f64 6f6f      sts = clodoo
+00005a40: 2e61 6374 5f75 7067 7261 6465 5f6d 6f64  .act_upgrade_mod
+00005a50: 756c 6573 2874 6774 5f63 7478 2c20 6d6f  ules(tgt_ctx, mo
+00005a60: 6475 6c65 5f6c 6973 743d 5b6d 6f64 756c  dule_list=[modul
+00005a70: 655d 290a 0a0a 6465 6620 6765 745f 666f  e])...def get_fo
+00005a80: 7265 6967 6e5f 7661 6c75 6528 7467 745f  reign_value(tgt_
+00005a90: 6374 782c 2073 7263 5f63 7478 2c20 7265  ctx, src_ctx, re
+00005aa0: 6c61 7469 6f6e 2c20 7661 6c75 652c 2074  lation, value, t
+00005ab0: 6f6d 616e 793d 4e6f 6e65 2c20 666f 726d  omany=None, form
+00005ac0: 6174 3d46 616c 7365 293a 0a20 2020 2064  at=False):.    d
+00005ad0: 6566 2062 696e 645f 666f 7265 6967 6e5f  ef bind_foreign_
+00005ae0: 7265 6628 7467 745f 6374 782c 2073 7263  ref(tgt_ctx, src
+00005af0: 5f63 7478 2c20 6d6f 6465 6c2c 2069 642c  _ctx, model, id,
+00005b00: 2072 656c 5f6d 6f64 6529 3a0a 2020 2020   rel_mode):.    
+00005b10: 2020 2020 6e65 775f 7661 6c75 6520 3d20      new_value = 
+00005b20: 4661 6c73 650a 2020 2020 2020 2020 6361  False.        ca
+00005b30: 6368 6520 3d20 6765 745f 6361 6368 6528  che = get_cache(
+00005b40: 7372 635f 6374 7829 0a20 2020 2020 2020  src_ctx).       
+00005b50: 2069 6620 7265 6c5f 6d6f 6465 203d 3d20   if rel_mode == 
+00005b60: 2769 6d61 6765 273a 0a20 2020 2020 2020  'image':.       
+00005b70: 2020 2020 2069 6620 636c 6f64 6f6f 2e73       if clodoo.s
+00005b80: 6561 7263 684c 3828 7467 745f 6374 782c  earchL8(tgt_ctx,
+00005b90: 2072 656c 6174 696f 6e2c 205b 2827 6964   relation, [('id
+00005ba0: 272c 2027 3d27 2c20 6964 295d 293a 0a20  ', '=', id)]):. 
+00005bb0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00005bc0: 6577 5f76 616c 7565 203d 2069 640a 2020  ew_value = id.  
+00005bd0: 2020 2020 2020 656c 6966 2063 6163 6865        elif cache
+00005be0: 5f69 735f 656e 7472 7928 6361 6368 652c  _is_entry(cache,
+00005bf0: 206d 6f64 656c 2c20 6964 293a 0a20 2020   model, id):.   
+00005c00: 2020 2020 2020 2020 206e 6577 5f76 616c           new_val
+00005c10: 7565 203d 2063 6163 6865 5f67 6574 5f65  ue = cache_get_e
+00005c20: 6e74 7279 2863 6163 6865 2c20 6d6f 6465  ntry(cache, mode
+00005c30: 6c2c 2069 6429 0a20 2020 2020 2020 2065  l, id).        e
+00005c40: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00005c50: 2072 656c 5f72 6563 203d 2063 6c6f 646f   rel_rec = clodo
+00005c60: 6f2e 6272 6f77 7365 4c38 2873 7263 5f63  o.browseL8(src_c
+00005c70: 7478 2c20 7265 6c61 7469 6f6e 2c20 6964  tx, relation, id
+00005c80: 2c20 636f 6e74 6578 743d 7b27 6c61 6e67  , context={'lang
+00005c90: 273a 2027 656e 5f55 5327 7d29 0a20 2020  ': 'en_US'}).   
+00005ca0: 2020 2020 2020 2020 206b 6579 7661 6c20           keyval 
+00005cb0: 3d20 636c 6f64 6f6f 2e65 7874 7261 6374  = clodoo.extract
+00005cc0: 5f76 616c 735f 6672 6f6d 5f72 6563 2873  _vals_from_rec(s
+00005cd0: 7263 5f63 7478 2c20 6d6f 6465 6c2c 2072  rc_ctx, model, r
+00005ce0: 656c 5f72 6563 2c20 666f 726d 6174 3d27  el_rec, format='
+00005cf0: 7374 7227 290a 2020 2020 2020 2020 2020  str').          
+00005d00: 2020 6964 203d 2073 6561 7263 6834 7265    id = search4re
+00005d10: 6328 7467 745f 6374 782c 206d 6f64 656c  c(tgt_ctx, model
+00005d20: 2c20 6b65 7976 616c 290a 2020 2020 2020  , keyval).      
+00005d30: 2020 2020 2020 6966 2069 6420 3e3d 2031        if id >= 1
+00005d40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005d50: 2020 6e65 775f 7661 6c75 6520 3d20 6964    new_value = id
+00005d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005d70: 2063 6163 6865 5f73 746f 7265 5f65 6e74   cache_store_ent
+00005d80: 7279 2863 6163 6865 2c20 6d6f 6465 6c2c  ry(cache, model,
+00005d90: 2069 6429 0a20 2020 2020 2020 2020 2020   id).           
+00005da0: 2065 6c69 6620 6e6f 7420 7372 635f 6374   elif not src_ct
+00005db0: 782e 6765 7428 276e 6f5f 7265 6375 7273  x.get('no_recurs
+00005dc0: 6527 293a 0a20 2020 2020 2020 2020 2020  e'):.           
+00005dd0: 2020 2020 206e 6577 5f76 616c 7565 203d       new_value =
+00005de0: 2073 796e 6368 726f 2874 6774 5f63 7478   synchro(tgt_ctx
+00005df0: 2c20 7265 6c61 7469 6f6e 2c20 6b65 7976  , relation, keyv
+00005e00: 616c 290a 2020 2020 2020 2020 2020 2020  al).            
+00005e10: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00005e20: 2020 2020 2020 6361 6368 655f 7374 6f72        cache_stor
+00005e30: 655f 656e 7472 7928 6361 6368 652c 206d  e_entry(cache, m
+00005e40: 6f64 656c 2c20 6e65 775f 7661 6c75 6529  odel, new_value)
+00005e50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00005e60: 6e65 775f 7661 6c75 650a 0a20 2020 2069  new_value..    i
+00005e70: 6620 6e6f 7420 7661 6c75 653a 0a20 2020  f not value:.   
+00005e80: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00005e90: 650a 2020 2020 6966 206e 6f74 2072 656c  e.    if not rel
+00005ea0: 6174 696f 6e3a 0a20 2020 2020 2020 2072  ation:.        r
+00005eb0: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
+00005ec0: 7228 274e 6f20 7265 6c61 7469 6f6e 2025  r('No relation %
+00005ed0: 7320 666f 756e 6427 2025 2072 656c 6174  s found' % relat
+00005ee0: 696f 6e29 0a20 2020 2072 656c 5f6d 6f64  ion).    rel_mod
+00005ef0: 6520 3d20 6765 745f 6d6f 6465 6c5f 636f  e = get_model_co
+00005f00: 7079 5f6d 6f64 6528 7467 745f 6374 782c  py_mode(tgt_ctx,
+00005f10: 2072 656c 6174 696f 6e29 0a20 2020 2063   relation).    c
+00005f20: 6c6f 646f 6f2e 6765 745f 6d6f 6465 6c5f  lodoo.get_model_
+00005f30: 7374 7275 6374 7572 6528 0a20 2020 2020  structure(.     
+00005f40: 2020 2073 7263 5f63 7478 2c20 7265 6c61     src_ctx, rela
+00005f50: 7469 6f6e 2c20 6967 6e6f 7265 3d49 474e  tion, ignore=IGN
+00005f60: 4f52 455f 4649 454c 4453 2e67 6574 2872  ORE_FIELDS.get(r
+00005f70: 656c 6174 696f 6e2c 205b 5d29 202b 2049  elation, []) + I
+00005f80: 474e 4f52 455f 4649 454c 4453 5b27 2a27  GNORE_FIELDS['*'
+00005f90: 5d0a 2020 2020 290a 2020 2020 636c 6f64  ].    ).    clod
+00005fa0: 6f6f 2e67 6574 5f6d 6f64 656c 5f73 7472  oo.get_model_str
+00005fb0: 7563 7475 7265 280a 2020 2020 2020 2020  ucture(.        
+00005fc0: 7467 745f 6374 782c 2072 656c 6174 696f  tgt_ctx, relatio
+00005fd0: 6e2c 2069 676e 6f72 653d 4947 4e4f 5245  n, ignore=IGNORE
+00005fe0: 5f46 4945 4c44 532e 6765 7428 7265 6c61  _FIELDS.get(rela
+00005ff0: 7469 6f6e 2c20 5b5d 2920 2b20 4947 4e4f  tion, []) + IGNO
+00006000: 5245 5f46 4945 4c44 535b 272a 275d 0a20  RE_FIELDS['*']. 
+00006010: 2020 2029 0a20 2020 206e 6577 5f76 616c     ).    new_val
+00006020: 7565 203d 2046 616c 7365 0a20 2020 2069  ue = False.    i
+00006030: 6620 7467 745f 6374 785b 275f 6d6c 275d  f tgt_ctx['_ml']
+00006040: 2e67 6574 2872 656c 6174 696f 6e29 2021  .get(relation) !
+00006050: 3d20 276e 6f27 3a0a 2020 2020 2020 2020  = 'no':.        
+00006060: 6966 2069 7369 6e73 7461 6e63 6528 7661  if isinstance(va
+00006070: 6c75 652c 2062 6173 6573 7472 696e 6729  lue, basestring)
+00006080: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+00006090: 7373 2020 2320 544f 444f 0a20 2020 2020  ss  # TODO.     
+000060a0: 2020 2020 2020 2069 6620 746f 6d61 6e79         if tomany
+000060b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000060c0: 2020 6e65 775f 7661 6c75 6520 3d20 5b6e    new_value = [n
+000060d0: 6577 5f76 616c 7565 5d0a 2020 2020 2020  ew_value].      
+000060e0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+000060f0: 6528 7265 6c61 7469 6f6e 2c20 286c 6973  e(relation, (lis
+00006100: 742c 2074 7570 6c65 2929 3a0a 2020 2020  t, tuple)):.    
+00006110: 2020 2020 2020 2020 6e65 775f 7661 6c75          new_valu
+00006120: 6520 3d20 5b5d 0a20 2020 2020 2020 2020  e = [].         
+00006130: 2020 2066 6f72 2069 6420 696e 2076 616c     for id in val
+00006140: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+00006150: 2020 2020 6e65 775f 7661 6c75 652e 6170      new_value.ap
+00006160: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
+00006170: 2020 2020 2020 2020 2020 6269 6e64 5f66            bind_f
+00006180: 6f72 6569 676e 5f72 6566 2874 6774 5f63  oreign_ref(tgt_c
+00006190: 7478 2c20 7372 635f 6374 782c 2072 656c  tx, src_ctx, rel
+000061a0: 6174 696f 6e2c 2069 642c 2072 656c 5f6d  ation, id, rel_m
+000061b0: 6f64 6529 0a20 2020 2020 2020 2020 2020  ode).           
+000061c0: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
+000061d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000061e0: 206e 6577 5f76 616c 7565 203d 2062 696e   new_value = bin
+000061f0: 645f 666f 7265 6967 6e5f 7265 6628 7467  d_foreign_ref(tg
+00006200: 745f 6374 782c 2073 7263 5f63 7478 2c20  t_ctx, src_ctx, 
+00006210: 7265 6c61 7469 6f6e 2c20 7661 6c75 652c  relation, value,
+00006220: 2072 656c 5f6d 6f64 6529 0a20 2020 2069   rel_mode).    i
+00006230: 6620 666f 726d 6174 203d 3d20 2763 6d64  f format == 'cmd
+00006240: 2720 616e 6420 7661 6c75 6520 616e 6420  ' and value and 
+00006250: 746f 6d61 6e79 3a0a 2020 2020 2020 2020  tomany:.        
+00006260: 7661 6c75 6520 3d20 5b28 362c 2030 2c20  value = [(6, 0, 
+00006270: 7661 6c75 6529 5d0a 2020 2020 7265 7475  value)].    retu
+00006280: 726e 206e 6577 5f76 616c 7565 0a0a 0a64  rn new_value...d
+00006290: 6566 2063 7674 5f6f 326d 5f76 616c 7565  ef cvt_o2m_value
+000062a0: 2874 6774 5f63 7478 2c20 7372 635f 6374  (tgt_ctx, src_ct
+000062b0: 782c 206d 6f64 656c 2c20 6e61 6d65 2c20  x, model, name, 
+000062c0: 7661 6c75 652c 2066 6f72 6d61 743d 4661  value, format=Fa
+000062d0: 6c73 6529 3a0a 2020 2020 7265 6c61 7469  lse):.    relati
+000062e0: 6f6e 203d 2073 7263 5f63 7478 5b27 5354  on = src_ctx['ST
+000062f0: 5255 4354 275d 5b6d 6f64 656c 5d5b 6e61  RUCT'][model][na
+00006300: 6d65 5d5b 2772 656c 6174 696f 6e27 5d0a  me]['relation'].
+00006310: 2020 2020 7265 7475 726e 2067 6574 5f66      return get_f
+00006320: 6f72 6569 676e 5f76 616c 7565 2874 6774  oreign_value(tgt
+00006330: 5f63 7478 2c20 7372 635f 6374 782c 2072  _ctx, src_ctx, r
+00006340: 656c 6174 696f 6e2c 2076 616c 7565 2c20  elation, value, 
+00006350: 746f 6d61 6e79 3d54 7275 6529 0a0a 0a64  tomany=True)...d
+00006360: 6566 2063 7674 5f6d 326d 5f76 616c 7565  ef cvt_m2m_value
+00006370: 2874 6774 5f63 7478 2c20 7372 635f 6374  (tgt_ctx, src_ct
+00006380: 782c 206d 6f64 656c 2c20 6e61 6d65 2c20  x, model, name, 
+00006390: 7661 6c75 652c 2066 6f72 6d61 743d 4661  value, format=Fa
+000063a0: 6c73 6529 3a0a 2020 2020 7265 6c61 7469  lse):.    relati
+000063b0: 6f6e 203d 2073 7263 5f63 7478 5b27 5354  on = src_ctx['ST
+000063c0: 5255 4354 275d 5b6d 6f64 656c 5d5b 6e61  RUCT'][model][na
+000063d0: 6d65 5d5b 2772 656c 6174 696f 6e27 5d0a  me]['relation'].
+000063e0: 2020 2020 7265 7475 726e 2067 6574 5f66      return get_f
+000063f0: 6f72 6569 676e 5f76 616c 7565 2874 6774  oreign_value(tgt
+00006400: 5f63 7478 2c20 7372 635f 6374 782c 2072  _ctx, src_ctx, r
+00006410: 656c 6174 696f 6e2c 2076 616c 7565 2c20  elation, value, 
+00006420: 746f 6d61 6e79 3d54 7275 6529 0a0a 0a64  tomany=True)...d
+00006430: 6566 2063 7674 5f6d 326f 5f76 616c 7565  ef cvt_m2o_value
+00006440: 2874 6774 5f63 7478 2c20 7372 635f 6374  (tgt_ctx, src_ct
+00006450: 782c 206d 6f64 656c 2c20 6e61 6d65 2c20  x, model, name, 
+00006460: 7661 6c75 652c 2066 6f72 6d61 743d 4661  value, format=Fa
+00006470: 6c73 6529 3a0a 2020 2020 7265 6c61 7469  lse):.    relati
+00006480: 6f6e 203d 2073 7263 5f63 7478 5b27 5354  on = src_ctx['ST
+00006490: 5255 4354 275d 5b6d 6f64 656c 5d5b 6e61  RUCT'][model][na
+000064a0: 6d65 5d5b 2772 656c 6174 696f 6e27 5d0a  me]['relation'].
+000064b0: 2020 2020 7265 7475 726e 2067 6574 5f66      return get_f
+000064c0: 6f72 6569 676e 5f76 616c 7565 2874 6774  oreign_value(tgt
+000064d0: 5f63 7478 2c20 7372 635f 6374 782c 2072  _ctx, src_ctx, r
+000064e0: 656c 6174 696f 6e2c 2076 616c 7565 290a  elation, value).
+000064f0: 0a0a 6465 6620 6c6f 6164 5f72 6563 6f72  ..def load_recor
+00006500: 6428 7467 745f 6374 782c 2073 7263 5f63  d(tgt_ctx, src_c
+00006510: 7478 2c20 6d6f 6465 6c2c 2072 6563 2c20  tx, model, rec, 
+00006520: 6d6f 6465 3d4e 6f6e 6529 3a0a 2020 2020  mode=None):.    
+00006530: 6d6f 6465 203d 206d 6f64 6520 6f72 2067  mode = mode or g
+00006540: 6574 5f6d 6f64 656c 5f63 6f70 795f 6d6f  et_model_copy_mo
+00006550: 6465 2873 7263 5f63 7478 2c20 6d6f 6465  de(src_ctx, mode
+00006560: 6c29 0a20 2020 2076 616c 7320 3d20 636c  l).    vals = cl
+00006570: 6f64 6f6f 2e65 7874 7261 6374 5f76 616c  odoo.extract_val
+00006580: 735f 6672 6f6d 5f72 6563 2873 7263 5f63  s_from_rec(src_c
+00006590: 7478 2c20 6d6f 6465 6c2c 2072 6563 2c20  tx, model, rec, 
+000065a0: 666f 726d 6174 3d27 7374 7227 290a 2020  format='str').  
+000065b0: 2020 7661 6c73 203d 2063 6c6f 646f 6f2e    vals = clodoo.
+000065c0: 6376 745f 6672 6f6d 5f76 6572 5f32 5f76  cvt_from_ver_2_v
+000065d0: 6572 280a 2020 2020 2020 2020 7467 745f  er(.        tgt_
+000065e0: 6374 782c 206d 6f64 656c 2c20 7372 635f  ctx, model, src_
+000065f0: 6374 785b 276f 655f 7665 7273 696f 6e27  ctx['oe_version'
+00006600: 5d2c 2074 6774 5f63 7478 5b27 6f65 5f76  ], tgt_ctx['oe_v
+00006610: 6572 7369 6f6e 275d 2c20 7661 6c73 0a20  ersion'], vals. 
+00006620: 2020 2029 0a20 2020 2066 6f72 206e 616d     ).    for nam
+00006630: 6520 696e 2076 616c 732e 636f 7079 2829  e in vals.copy()
+00006640: 3a0a 2020 2020 2020 2020 6966 206e 616d  :.        if nam
+00006650: 6520 6e6f 7420 696e 2074 6774 5f63 7478  e not in tgt_ctx
+00006660: 5b27 5354 5255 4354 275d 5b6d 6f64 656c  ['STRUCT'][model
+00006670: 5d3a 0a20 2020 2020 2020 2020 2020 2064  ]:.            d
+00006680: 656c 2076 616c 735b 6e61 6d65 5d0a 2020  el vals[name].  
+00006690: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+000066a0: 7565 0a20 2020 2020 2020 2065 6c69 6620  ue.        elif 
+000066b0: 6e61 6d65 203d 3d20 2763 6f6d 7061 6e79  name == 'company
+000066c0: 5f69 6427 2061 6e64 2073 7263 5f63 7478  _id' and src_ctx
+000066d0: 5b27 6279 5f63 6f6d 7061 6e79 275d 3a0a  ['by_company']:.
+000066e0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+000066f0: 696e 7565 0a20 2020 2020 2020 2065 6c69  inue.        eli
+00006700: 6620 7467 745f 6374 785b 2753 5452 5543  f tgt_ctx['STRUC
+00006710: 5427 5d5b 6d6f 6465 6c5d 5b6e 616d 655d  T'][model][name]
+00006720: 5b27 7474 7970 6527 5d20 696e 2028 276f  ['ttype'] in ('o
+00006730: 6e65 326d 616e 7927 293a 0a20 2020 2020  ne2many'):.     
+00006740: 2020 2020 2020 2076 616c 735b 6e61 6d65         vals[name
+00006750: 5d20 3d20 6376 745f 6f32 6d5f 7661 6c75  ] = cvt_o2m_valu
+00006760: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00006770: 2020 2074 6774 5f63 7478 2c20 7467 745f     tgt_ctx, tgt_
+00006780: 6374 782c 206d 6f64 656c 2c20 6e61 6d65  ctx, model, name
+00006790: 2c20 7661 6c73 5b6e 616d 655d 2c20 666f  , vals[name], fo
+000067a0: 726d 6174 3d27 636d 6427 0a20 2020 2020  rmat='cmd'.     
+000067b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000067c0: 2065 6c69 6620 7467 745f 6374 785b 2753   elif tgt_ctx['S
+000067d0: 5452 5543 5427 5d5b 6d6f 6465 6c5d 5b6e  TRUCT'][model][n
+000067e0: 616d 655d 5b27 7474 7970 6527 5d20 696e  ame]['ttype'] in
+000067f0: 2028 276d 616e 7932 6d61 6e79 2729 3a0a   ('many2many'):.
+00006800: 2020 2020 2020 2020 2020 2020 7661 6c73              vals
+00006810: 5b6e 616d 655d 203d 2063 7674 5f6d 326d  [name] = cvt_m2m
+00006820: 5f76 616c 7565 280a 2020 2020 2020 2020  _value(.        
+00006830: 2020 2020 2020 2020 7467 745f 6374 782c          tgt_ctx,
+00006840: 2074 6774 5f63 7478 2c20 6d6f 6465 6c2c   tgt_ctx, model,
+00006850: 206e 616d 652c 2076 616c 735b 6e61 6d65   name, vals[name
+00006860: 5d2c 2066 6f72 6d61 743d 2763 6d64 270a  ], format='cmd'.
+00006870: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00006880: 2020 2020 2020 656c 6966 2074 6774 5f63        elif tgt_c
+00006890: 7478 5b27 5354 5255 4354 275d 5b6d 6f64  tx['STRUCT'][mod
+000068a0: 656c 5d5b 6e61 6d65 5d5b 2774 7479 7065  el][name]['ttype
+000068b0: 275d 2069 6e20 2827 6d61 6e79 326f 6e65  '] in ('many2one
+000068c0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+000068d0: 7661 6c73 5b6e 616d 655d 203d 2063 7674  vals[name] = cvt
+000068e0: 5f6d 326f 5f76 616c 7565 280a 2020 2020  _m2o_value(.    
+000068f0: 2020 2020 2020 2020 2020 2020 7467 745f              tgt_
+00006900: 6374 782c 2074 6774 5f63 7478 2c20 6d6f  ctx, tgt_ctx, mo
+00006910: 6465 6c2c 206e 616d 652c 2076 616c 735b  del, name, vals[
+00006920: 6e61 6d65 5d2c 2066 6f72 6d61 743d 2763  name], format='c
+00006930: 6d64 270a 2020 2020 2020 2020 2020 2020  md'.            
+00006940: 290a 2020 2020 2020 2020 6966 2076 616c  ).        if val
+00006950: 735b 6e61 6d65 5d20 6973 2046 616c 7365  s[name] is False
+00006960: 2061 6e64 2074 6774 5f63 7478 5b27 5354   and tgt_ctx['ST
+00006970: 5255 4354 275d 5b6d 6f64 656c 5d5b 6e61  RUCT'][model][na
+00006980: 6d65 5d5b 2774 7479 7065 275d 2021 3d20  me]['ttype'] != 
+00006990: 2762 6f6f 6c65 616e 273a 0a20 2020 2020  'boolean':.     
+000069a0: 2020 2020 2020 2064 656c 2076 616c 735b         del vals[
+000069b0: 6e61 6d65 5d0a 2020 2020 7265 7475 726e  name].    return
+000069c0: 2076 616c 730a 0a0a 6465 6620 7573 655f   vals...def use_
+000069d0: 7379 6e63 6872 6f28 7467 745f 6374 782c  synchro(tgt_ctx,
+000069e0: 206d 6f64 656c 293a 0a20 2020 2069 6620   model):.    if 
+000069f0: 7467 745f 6374 785b 2775 7365 5f73 796e  tgt_ctx['use_syn
+00006a00: 6368 726f 275d 2061 6e64 206d 6f64 656c  chro'] and model
+00006a10: 2069 6e20 280a 2020 2020 2020 2020 2772   in (.        'r
+00006a20: 6573 2e63 6f75 6e74 7279 272c 0a20 2020  es.country',.   
+00006a30: 2020 2020 2027 7265 732e 7061 7274 6e65       'res.partne
+00006a40: 7227 2c0a 2020 2020 2020 2020 2761 6363  r',.        'acc
+00006a50: 6f75 6e74 2e61 6363 6f75 6e74 272c 0a20  ount.account',. 
+00006a60: 2020 2020 2020 2027 6163 636f 756e 742e         'account.
+00006a70: 6163 636f 756e 742e 7479 7065 272c 0a20  account.type',. 
+00006a80: 2020 2020 2020 2027 6163 636f 756e 742e         'account.
+00006a90: 696e 766f 6963 6527 2c0a 2020 2020 2020  invoice',.      
+00006aa0: 2020 2761 6363 6f75 6e74 2e69 6e76 6f69    'account.invoi
+00006ab0: 6365 2e6c 696e 6527 2c0a 2020 2020 2020  ce.line',.      
+00006ac0: 2020 2761 6363 6f75 6e74 2e74 6178 272c    'account.tax',
+00006ad0: 0a20 2020 2020 2020 2027 7072 6f64 7563  .        'produc
+00006ae0: 742e 7465 6d70 6c61 7465 272c 0a20 2020  t.template',.   
+00006af0: 2020 2020 2027 7072 6f64 7563 742e 7072       'product.pr
+00006b00: 6f64 7563 7427 2c0a 2020 2020 2020 2020  oduct',.        
+00006b10: 2773 616c 652e 6f72 6465 7227 2c0a 2020  'sale.order',.  
+00006b20: 2020 2020 2020 2773 616c 652e 6f72 6465        'sale.orde
+00006b30: 722e 6c69 6e65 272c 0a20 2020 2029 3a0a  r.line',.    ):.
+00006b40: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00006b50: 7275 650a 2020 2020 7265 7475 726e 2046  rue.    return F
+00006b60: 616c 7365 0a0a 0a64 6566 2073 6574 5f61  alse...def set_a
+00006b70: 6374 7561 6c5f 7374 6174 6528 7467 745f  ctual_state(tgt_
+00006b80: 6374 782c 206d 6f64 656c 2c20 6964 2c20  ctx, model, id, 
+00006b90: 7374 6174 6529 3a0a 2020 2020 6966 206d  state):.    if m
+00006ba0: 6f64 656c 203d 3d20 2761 6363 6f75 6e74  odel == 'account
+00006bb0: 2e69 6e76 6f69 6365 273a 0a20 2020 2020  .invoice':.     
+00006bc0: 2020 2069 6620 6964 3a0a 2020 2020 2020     if id:.      
+00006bd0: 2020 2020 2020 7265 6320 3d20 636c 6f64        rec = clod
+00006be0: 6f6f 2e62 726f 7773 654c 3828 7467 745f  oo.browseL8(tgt_
+00006bf0: 6374 782c 206d 6f64 656c 2c20 6964 290a  ctx, model, id).
+00006c00: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00006c10: 7461 7465 203d 3d20 2764 7261 6674 273a  tate == 'draft':
+00006c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006c30: 2061 6374 696f 6e20 3d20 2727 0a20 2020   action = ''.   
+00006c40: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00006c50: 7572 6e20 7265 632e 6964 0a20 2020 2020  urn rec.id.     
+00006c60: 2020 2020 2020 2065 6c69 6620 7265 632e         elif rec.
+00006c70: 7374 6174 6520 213d 2027 6472 6166 7427  state != 'draft'
+00006c80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006c90: 2020 7265 7475 726e 202d 340a 2020 2020    return -4.    
+00006ca0: 2020 2020 2020 2020 656c 6966 2072 6563          elif rec
+00006cb0: 2e6f 7269 6769 6e61 6c5f 7374 6174 6520  .original_state 
+00006cc0: 3d3d 2027 6f70 656e 273a 0a20 2020 2020  == 'open':.     
+00006cd0: 2020 2020 2020 2020 2020 2072 6563 2e61             rec.a
+00006ce0: 6374 696f 6e5f 696e 766f 6963 655f 6f70  ction_invoice_op
+00006cf0: 656e 2829 0a20 2020 2020 2020 2020 2020  en().           
+00006d00: 2065 6c69 6620 7265 632e 6f72 6967 696e   elif rec.origin
+00006d10: 616c 5f73 7461 7465 203d 3d20 2763 616e  al_state == 'can
+00006d20: 6365 6c27 3a0a 2020 2020 2020 2020 2020  cel':.          
+00006d30: 2020 2020 2020 7265 632e 6163 7469 6f6e        rec.action
+00006d40: 5f69 6e76 6f69 6365 5f63 616e 6365 6c28  _invoice_cancel(
+00006d50: 290a 2020 2020 656c 6966 206d 6f64 656c  ).    elif model
+00006d60: 203d 3d20 2773 616c 652e 6f72 6465 7227   == 'sale.order'
+00006d70: 3a0a 2020 2020 2020 2020 6966 2069 643a  :.        if id:
+00006d80: 0a20 2020 2020 2020 2020 2020 2072 6563  .            rec
+00006d90: 203d 2063 6c6f 646f 6f2e 6272 6f77 7365   = clodoo.browse
+00006da0: 4c38 2874 6774 5f63 7478 2c20 6d6f 6465  L8(tgt_ctx, mode
+00006db0: 6c2c 2069 6429 0a20 2020 2020 2020 2020  l, id).         
+00006dc0: 2020 2072 6563 2e5f 636f 6d70 7574 655f     rec._compute_
+00006dd0: 7461 785f 6964 2829 0a20 2020 2020 2020  tax_id().       
+00006de0: 2020 2020 2069 6620 7265 632e 7374 6174       if rec.stat
+00006df0: 6520 3d3d 2072 6563 2e6f 7269 6769 6e61  e == rec.origina
+00006e00: 6c5f 7374 6174 653a 0a20 2020 2020 2020  l_state:.       
+00006e10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00006e20: 7265 632e 6964 0a20 2020 2020 2020 2020  rec.id.         
+00006e30: 2020 2065 6c69 6620 7265 632e 7374 6174     elif rec.stat
+00006e40: 6520 213d 2027 6472 6166 7427 3a0a 2020  e != 'draft':.  
+00006e50: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00006e60: 7475 726e 202d 340a 2020 2020 2020 2020  turn -4.        
+00006e70: 2020 2020 656c 6966 2072 6563 2e6f 7269      elif rec.ori
+00006e80: 6769 6e61 6c5f 7374 6174 6520 3d3d 2027  ginal_state == '
+00006e90: 7361 6c65 273a 0a20 2020 2020 2020 2020  sale':.         
+00006ea0: 2020 2020 2020 2072 6563 2e61 6374 696f         rec.actio
+00006eb0: 6e5f 636f 6e66 6972 6d28 290a 2020 2020  n_confirm().    
+00006ec0: 2020 2020 2020 2020 656c 6966 2072 6563          elif rec
+00006ed0: 2e6f 7269 6769 6e61 6c5f 7374 6174 6520  .original_state 
+00006ee0: 3d3d 2027 6361 6e63 656c 273a 0a20 2020  == 'cancel':.   
+00006ef0: 2020 2020 2020 2020 2020 2020 2072 6563               rec
+00006f00: 2e61 6374 696f 6e5f 6361 6e63 656c 2829  .action_cancel()
+00006f10: 0a20 2020 2072 6574 7572 6e20 7265 632e  .    return rec.
+00006f20: 6964 0a0a 0a64 6566 2073 6574 5f73 7461  id...def set_sta
+00006f30: 7465 5f74 6f5f 6472 6166 7428 7467 745f  te_to_draft(tgt_
+00006f40: 6374 782c 206d 6f64 656c 2c20 6964 732c  ctx, model, ids,
+00006f50: 2076 616c 7329 3a0a 2020 2020 7265 6320   vals):.    rec 
+00006f60: 3d20 4661 6c73 650a 2020 2020 6966 206e  = False.    if n
+00006f70: 6f74 2069 6473 3a0a 2020 2020 2020 2020  ot ids:.        
+00006f80: 6964 203d 2046 616c 7365 0a20 2020 2065  id = False.    e
+00006f90: 6c73 653a 0a20 2020 2020 2020 2069 6420  lse:.        id 
+00006fa0: 3d20 6964 735b 305d 0a20 2020 2074 6774  = ids[0].    tgt
+00006fb0: 5f63 7478 5b27 5f43 4f4d 4d49 5427 5d5b  _ctx['_COMMIT'][
+00006fc0: 6d6f 6465 6c5d 203d 207b 2769 6427 3a20  model] = {'id': 
+00006fd0: 6964 7d0a 2020 2020 6966 2027 7374 6174  id}.    if 'stat
+00006fe0: 6527 2069 6e20 7661 6c73 3a0a 2020 2020  e' in vals:.    
+00006ff0: 2020 2020 7467 745f 6374 785b 275f 434f      tgt_ctx['_CO
+00007000: 4d4d 4954 275d 5b6d 6f64 656c 5d5b 2773  MMIT'][model]['s
+00007010: 7461 7465 275d 203d 2076 616c 735b 2773  tate'] = vals['s
+00007020: 7461 7465 275d 0a20 2020 2065 6c69 6620  tate'].    elif 
+00007030: 6964 3a0a 2020 2020 2020 2020 7265 6320  id:.        rec 
+00007040: 3d20 636c 6f64 6f6f 2e62 726f 7773 654c  = clodoo.browseL
+00007050: 3828 7467 745f 6374 782c 206d 6f64 656c  8(tgt_ctx, model
+00007060: 2c20 6964 290a 2020 2020 2020 2020 6966  , id).        if
+00007070: 2027 7374 6174 6527 2069 6e20 7265 633a   'state' in rec:
+00007080: 0a20 2020 2020 2020 2020 2020 2074 6774  .            tgt
+00007090: 5f63 7478 5b27 5f43 4f4d 4d49 5427 5d5b  _ctx['_COMMIT'][
+000070a0: 6d6f 6465 6c5d 5b27 7374 6174 6527 5d20  model]['state'] 
+000070b0: 3d20 7265 632e 7374 6174 650a 2020 2020  = rec.state.    
+000070c0: 6966 206d 6f64 656c 203d 3d20 2761 6363  if model == 'acc
+000070d0: 6f75 6e74 2e69 6e76 6f69 6365 273a 0a20  ount.invoice':. 
+000070e0: 2020 2020 2020 2069 6620 7265 633a 0a20         if rec:. 
+000070f0: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+00007100: 632e 7374 6174 6520 3d3d 2027 7061 6964  c.state == 'paid
+00007110: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
+00007120: 2020 2072 6574 7572 6e20 7661 6c73 2c20     return vals, 
+00007130: 2d34 0a20 2020 2020 2020 2020 2020 2065  -4.            e
+00007140: 6c69 6620 7265 632e 7374 6174 6520 3d3d  lif rec.state ==
+00007150: 2027 6f70 656e 273a 0a20 2020 2020 2020   'open':.       
+00007160: 2020 2020 2020 2020 2069 6420 3d20 636c           id = cl
+00007170: 6f64 6f6f 2e65 7865 6375 7465 4c38 2874  odoo.executeL8(t
+00007180: 6774 5f63 7478 2c20 6d6f 6465 6c2c 2027  gt_ctx, model, '
+00007190: 6163 7469 6f6e 5f69 6e76 6f69 6365 5f63  action_invoice_c
+000071a0: 616e 6365 6c27 2c20 6964 7329 0a20 2020  ancel', ids).   
+000071b0: 2020 2020 2020 2020 2020 2020 2069 6420               id 
+000071c0: 3d20 636c 6f64 6f6f 2e65 7865 6375 7465  = clodoo.execute
+000071d0: 4c38 2874 6774 5f63 7478 2c20 6d6f 6465  L8(tgt_ctx, mode
+000071e0: 6c2c 2027 6163 7469 6f6e 5f69 6e76 6f69  l, 'action_invoi
+000071f0: 6365 5f64 7261 6674 272c 2069 6473 290a  ce_draft', ids).
+00007200: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00007210: 2072 6563 2e73 7461 7465 203d 3d20 2763   rec.state == 'c
+00007220: 616e 6365 6c27 3a0a 2020 2020 2020 2020  ancel':.        
+00007230: 2020 2020 2020 2020 6964 203d 2063 6c6f          id = clo
+00007240: 646f 6f2e 6578 6563 7574 654c 3828 7467  doo.executeL8(tg
+00007250: 745f 6374 782c 206d 6f64 656c 2c20 2761  t_ctx, model, 'a
+00007260: 6374 696f 6e5f 696e 766f 6963 655f 6472  ction_invoice_dr
+00007270: 6166 7427 2c20 6964 7329 0a20 2020 2020  aft', ids).     
+00007280: 2020 2076 616c 735b 2773 7461 7465 275d     vals['state']
+00007290: 203d 2027 6472 6166 7427 0a20 2020 2065   = 'draft'.    e
+000072a0: 6c69 6620 6d6f 6465 6c20 3d3d 2027 7361  lif model == 'sa
+000072b0: 6c65 2e6f 7264 6572 273a 0a20 2020 2020  le.order':.     
+000072c0: 2020 2069 6620 7265 633a 0a20 2020 2020     if rec:.     
+000072d0: 2020 2020 2020 2069 6620 7265 632e 7374         if rec.st
+000072e0: 6174 6520 3d3d 2027 646f 6e65 273a 0a20  ate == 'done':. 
+000072f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00007300: 6574 7572 6e20 7661 6c73 2c20 2d34 0a20  eturn vals, -4. 
+00007310: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00007320: 7265 632e 7374 6174 6520 3d3d 2027 7361  rec.state == 'sa
+00007330: 6c65 273a 0a20 2020 2020 2020 2020 2020  le':.           
+00007340: 2020 2020 2069 6420 3d20 636c 6f64 6f6f       id = clodoo
+00007350: 2e65 7865 6375 7465 4c38 2874 6774 5f63  .executeL8(tgt_c
+00007360: 7478 2c20 6d6f 6465 6c2c 2027 6163 7469  tx, model, 'acti
+00007370: 6f6e 5f63 616e 6365 6c27 2c20 6964 7329  on_cancel', ids)
+00007380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007390: 2069 6420 3d20 636c 6f64 6f6f 2e65 7865   id = clodoo.exe
+000073a0: 6375 7465 4c38 2874 6774 5f63 7478 2c20  cuteL8(tgt_ctx, 
+000073b0: 6d6f 6465 6c2c 2027 6163 7469 6f6e 5f64  model, 'action_d
+000073c0: 7261 6674 272c 2069 6473 290a 2020 2020  raft', ids).    
+000073d0: 2020 2020 2020 2020 656c 6966 2072 6563          elif rec
+000073e0: 2e73 7461 7465 203d 3d20 2763 616e 6365  .state == 'cance
+000073f0: 6c27 3a0a 2020 2020 2020 2020 2020 2020  l':.            
+00007400: 2020 2020 6964 203d 2063 6c6f 646f 6f2e      id = clodoo.
+00007410: 6578 6563 7574 654c 3828 7467 745f 6374  executeL8(tgt_ct
+00007420: 782c 206d 6f64 656c 2c20 2761 6374 696f  x, model, 'actio
+00007430: 6e5f 6472 6166 7427 2c20 6964 7329 0a20  n_draft', ids). 
+00007440: 2020 2020 2020 2076 616c 735b 2773 7461         vals['sta
+00007450: 7465 275d 203d 2027 6472 6166 7427 0a20  te'] = 'draft'. 
+00007460: 2020 2072 6574 7572 6e20 7661 6c73 2c20     return vals, 
+00007470: 300a 0a0a 6465 6620 636f 6d6d 6974 5f74  0...def commit_t
+00007480: 6162 6c65 2874 6774 5f63 7478 2c20 7372  able(tgt_ctx, sr
+00007490: 635f 6374 782c 206d 6f64 656c 293a 0a20  c_ctx, model):. 
+000074a0: 2020 2069 6420 3d20 4661 6c73 650a 2020     id = False.  
+000074b0: 2020 6966 2074 6774 5f63 7478 5b27 5f43    if tgt_ctx['_C
+000074c0: 4f4d 4d49 5427 5d2e 6765 7428 6d6f 6465  OMMIT'].get(mode
+000074d0: 6c29 3a0a 2020 2020 2020 2020 6964 203d  l):.        id =
+000074e0: 2074 6774 5f63 7478 5b27 5f43 4f4d 4d49   tgt_ctx['_COMMI
+000074f0: 5427 5d5b 6d6f 6465 6c5d 5b27 6964 275d  T'][model]['id']
+00007500: 0a20 2020 2020 2020 2069 6620 7573 655f  .        if use_
+00007510: 7379 6e63 6872 6f28 7467 745f 6374 782c  synchro(tgt_ctx,
+00007520: 206d 6f64 656c 293a 0a20 2020 2020 2020   model):.       
+00007530: 2020 2020 2069 6420 3d20 636c 6f64 6f6f       id = clodoo
+00007540: 2e65 7865 6375 7465 4c38 2874 6774 5f63  .executeL8(tgt_c
+00007550: 7478 2c20 6d6f 6465 6c2c 2027 636f 6d6d  tx, model, 'comm
+00007560: 6974 272c 2069 6429 0a20 2020 2020 2020  it', id).       
+00007570: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00007580: 2020 2073 6574 5f61 6374 7561 6c5f 7374     set_actual_st
+00007590: 6174 6528 7467 745f 6374 782c 206d 6f64  ate(tgt_ctx, mod
+000075a0: 656c 2c20 6964 2c20 7467 745f 6374 785b  el, id, tgt_ctx[
+000075b0: 275f 434f 4d4d 4954 275d 5b6d 6f64 656c  '_COMMIT'][model
+000075c0: 5d5b 2773 7461 7465 275d 290a 2020 2020  ]['state']).    
+000075d0: 7467 745f 6374 785b 275f 434f 4d4d 4954  tgt_ctx['_COMMIT
+000075e0: 275d 5b6d 6f64 656c 5d20 3d20 4661 6c73  '][model] = Fals
+000075f0: 650a 2020 2020 7265 7475 726e 2069 640a  e.    return id.
+00007600: 0a0a 6465 6620 7379 6e63 6872 6f28 7467  ..def synchro(tg
+00007610: 745f 6374 782c 206d 6f64 656c 2c20 7661  t_ctx, model, va
+00007620: 6c73 293a 0a20 2020 2074 6774 5f63 7478  ls):.    tgt_ctx
+00007630: 5b27 5f43 4f4d 4d49 5427 5d5b 6d6f 6465  ['_COMMIT'][mode
+00007640: 6c5d 203d 2046 616c 7365 0a20 2020 2063  l] = False.    c
+00007650: 6163 6865 203d 2067 6574 5f63 6163 6865  ache = get_cache
+00007660: 2873 7263 5f63 7478 290a 2020 2020 2320  (src_ctx).    # 
+00007670: 6966 2027 636f 6d70 616e 795f 6964 2720  if 'company_id' 
+00007680: 696e 2076 616c 7320 616e 6420 7467 745f  in vals and tgt_
+00007690: 6374 782e 6765 7428 2762 795f 636f 6d70  ctx.get('by_comp
+000076a0: 616e 7927 293a 0a20 2020 2023 2020 2020  any'):.    #    
+000076b0: 2076 616c 735b 2763 6f6d 7061 6e79 5f69   vals['company_i
+000076c0: 6427 5d20 3d20 7467 745f 6374 785b 2763  d'] = tgt_ctx['c
+000076d0: 6f6d 7061 6e79 5f69 6427 5d0a 2020 2020  ompany_id'].    
+000076e0: 6964 203d 2073 6561 7263 6834 7265 6328  id = search4rec(
+000076f0: 7467 745f 6374 782c 206d 6f64 656c 2c20  tgt_ctx, model, 
+00007700: 7661 6c73 290a 2020 2020 6966 2069 6420  vals).    if id 
+00007710: 3e20 303a 0a20 2020 2020 2020 2076 616c  > 0:.        val
+00007720: 732c 2073 7473 203d 2073 6574 5f73 7461  s, sts = set_sta
+00007730: 7465 5f74 6f5f 6472 6166 7428 7467 745f  te_to_draft(tgt_
+00007740: 6374 782c 206d 6f64 656c 2c20 5b69 645d  ctx, model, [id]
+00007750: 2c20 7661 6c73 290a 2020 2020 2020 2020  , vals).        
+00007760: 7772 6974 655f 6e6f 5f64 7570 2874 6774  write_no_dup(tgt
+00007770: 5f63 7478 2c20 6d6f 6465 6c2c 205b 6964  _ctx, model, [id
+00007780: 5d2c 2076 616c 732c 2069 6429 0a20 2020  ], vals, id).   
+00007790: 2020 2020 2063 6163 6865 5f73 746f 7265       cache_store
+000077a0: 5f65 6e74 7279 2863 6163 6865 2c20 6d6f  _entry(cache, mo
+000077b0: 6465 6c2c 2069 6429 0a20 2020 2065 6c73  del, id).    els
+000077c0: 653a 0a20 2020 2020 2020 2074 7279 3a0a  e:.        try:.
+000077d0: 2020 2020 2020 2020 2020 2020 7661 6c73              vals
+000077e0: 2c20 7374 7320 3d20 7365 745f 7374 6174  , sts = set_stat
+000077f0: 655f 746f 5f64 7261 6674 2874 6774 5f63  e_to_draft(tgt_c
+00007800: 7478 2c20 6d6f 6465 6c2c 2046 616c 7365  tx, model, False
+00007810: 2c20 7661 6c73 290a 2020 2020 2020 2020  , vals).        
+00007820: 2020 2020 6964 203d 2063 6c6f 646f 6f2e      id = clodoo.
+00007830: 6372 6561 7465 4c38 2874 6774 5f63 7478  createL8(tgt_ctx
+00007840: 2c20 6d6f 6465 6c2c 2076 616c 7329 0a20  , model, vals). 
+00007850: 2020 2020 2020 2020 2020 2063 6163 6865             cache
+00007860: 5f73 746f 7265 5f65 6e74 7279 2863 6163  _store_entry(cac
+00007870: 6865 2c20 6d6f 6465 6c2c 2069 6429 0a20  he, model, id). 
+00007880: 2020 2020 2020 2020 2020 2074 6774 5f63             tgt_c
+00007890: 7478 5b27 5f43 4f4d 4d49 5427 5d5b 6d6f  tx['_COMMIT'][mo
+000078a0: 6465 6c5d 5b27 6964 275d 203d 2069 640a  del]['id'] = id.
+000078b0: 2020 2020 2020 2020 6578 6365 7074 2049          except I
+000078c0: 4f45 7272 6f72 2061 7320 653a 0a20 2020  OError as e:.   
+000078d0: 2020 2020 2020 2020 206f 7330 2e77 6c6f           os0.wlo
+000078e0: 6728 2725 7320 4361 6e6e 6f74 2063 7265  g('%s Cannot cre
+000078f0: 6174 6520 2573 2073 7263 2069 643d 2564  ate %s src id=%d
+00007900: 2720 2520 2865 2c20 6d6f 6465 6c2c 2069  ' % (e, model, i
+00007910: 6429 290a 2020 2020 2020 2020 2020 2020  d)).            
+00007920: 6d61 6e61 6765 5f65 7272 6f72 2829 0a0a  manage_error()..
+00007930: 0a64 6566 2073 6561 7263 6834 7265 6328  .def search4rec(
+00007940: 7467 745f 6374 782c 206d 6f64 656c 2c20  tgt_ctx, model, 
+00007950: 7661 6c73 293a 0a20 2020 2064 6566 2064  vals):.    def d
+00007960: 696d 5f74 6578 7428 7465 7874 293a 0a20  im_text(text):. 
+00007970: 2020 2020 2020 2069 6620 7465 7874 3a0a         if text:.
+00007980: 2020 2020 2020 2020 2020 2020 7465 7874              text
+00007990: 203d 2075 6e69 6465 636f 6465 2874 6578   = unidecode(tex
+000079a0: 7429 2e73 7472 6970 2829 0a20 2020 2020  t).strip().     
+000079b0: 2020 2020 2020 2072 6573 203d 2027 270a         res = ''.
+000079c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000079d0: 6368 2069 6e20 7465 7874 3a0a 2020 2020  ch in text:.    
+000079e0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+000079f0: 682e 6973 616c 6e75 6d28 293a 0a20 2020  h.isalnum():.   
+00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a10: 2072 6573 202b 3d20 6368 2e6c 6f77 6572   res += ch.lower
+00007a20: 2829 0a20 2020 2020 2020 2020 2020 2074  ().            t
+00007a30: 6578 7420 3d20 7265 730a 2020 2020 2020  ext = res.      
+00007a40: 2020 7265 7475 726e 2074 6578 740a 0a20    return text.. 
+00007a50: 2020 2063 6f6d 7061 6e79 5f69 6420 3d20     company_id = 
+00007a60: 7467 745f 6374 782e 6765 7428 2763 6f6d  tgt_ctx.get('com
+00007a70: 7061 6e79 5f69 6427 2c20 4661 6c73 6529  pany_id', False)
+00007a80: 0a20 2020 2069 6420 3d20 2d31 0a20 2020  .    id = -1.   
+00007a90: 2066 6f72 206b 6579 7320 696e 2074 6774   for keys in tgt
+00007aa0: 5f63 7478 5b27 5f6b 6c27 5d5b 6d6f 6465  _ctx['_kl'][mode
+00007ab0: 6c5d 3a0a 2020 2020 2020 2020 7768 6572  l]:.        wher
+00007ac0: 6520 3d20 5b5d 0a20 2020 2020 2020 2066  e = [].        f
+00007ad0: 6f72 206b 6579 2069 6e20 6b65 7973 3a0a  or key in keys:.
+00007ae0: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+00007af0: 6579 206e 6f74 2069 6e20 7661 6c73 2061  ey not in vals a
+00007b00: 6e64 206b 6579 203d 3d20 2764 696d 5f6e  nd key == 'dim_n
+00007b10: 616d 6527 2061 6e64 2076 616c 732e 6765  ame' and vals.ge
+00007b20: 7428 276e 616d 6527 293a 0a20 2020 2020  t('name'):.     
+00007b30: 2020 2020 2020 2020 2020 2077 6865 7265             where
+00007b40: 2e61 7070 656e 6428 2827 6469 6d5f 6e61  .append(('dim_na
+00007b50: 6d65 272c 2027 3d27 2c20 6469 6d5f 7465  me', '=', dim_te
+00007b60: 7874 2876 616c 735b 276e 616d 6527 5d29  xt(vals['name'])
+00007b70: 2929 0a20 2020 2020 2020 2020 2020 2065  )).            e
+00007b80: 6c69 6620 6b65 7920 6e6f 7420 696e 2076  lif key not in v
+00007b90: 616c 7320 616e 6420 6b65 7920 3d3d 2027  als and key == '
+00007ba0: 636f 6d70 616e 795f 6964 273a 0a20 2020  company_id':.   
+00007bb0: 2020 2020 2020 2020 2020 2020 2077 6865               whe
+00007bc0: 7265 2e61 7070 656e 6428 286b 6579 2c20  re.append((key, 
+00007bd0: 273d 272c 2063 6f6d 7061 6e79 5f69 6429  '=', company_id)
+00007be0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00007bf0: 6966 206b 6579 206e 6f74 2069 6e20 7661  if key not in va
+00007c00: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
+00007c10: 2020 2020 7768 6572 6520 3d20 5b5d 0a20      where = []. 
+00007c20: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00007c30: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
+00007c40: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00007c50: 2020 2020 2020 2077 6865 7265 2e61 7070         where.app
+00007c60: 656e 6428 286b 6579 2c20 273d 272c 2076  end((key, '=', v
+00007c70: 616c 735b 6b65 795d 2929 0a20 2020 2020  als[key])).     
+00007c80: 2020 2069 6620 7768 6572 653a 0a20 2020     if where:.   
+00007c90: 2020 2020 2020 2020 2069 6473 203d 2063           ids = c
+00007ca0: 6c6f 646f 6f2e 7365 6172 6368 4c38 2874  lodoo.searchL8(t
+00007cb0: 6774 5f63 7478 2c20 6d6f 6465 6c2c 2077  gt_ctx, model, w
+00007cc0: 6865 7265 290a 2020 2020 2020 2020 2020  here).          
+00007cd0: 2020 6966 206e 6f74 2069 6473 2061 6e64    if not ids and
+00007ce0: 2027 6163 7469 7665 2720 696e 2074 6774   'active' in tgt
+00007cf0: 5f63 7478 5b27 5354 5255 4354 275d 5b6d  _ctx['STRUCT'][m
+00007d00: 6f64 656c 5d3a 0a20 2020 2020 2020 2020  odel]:.         
+00007d10: 2020 2020 2020 2077 6865 7265 2e61 7070         where.app
+00007d20: 656e 6428 2827 6163 7469 7665 272c 2027  end(('active', '
+00007d30: 3d27 2c20 4661 6c73 6529 290a 2020 2020  =', False)).    
+00007d40: 2020 2020 2020 2020 2020 2020 6964 7320              ids 
+00007d50: 3d20 636c 6f64 6f6f 2e73 6561 7263 684c  = clodoo.searchL
+00007d60: 3828 7467 745f 6374 782c 206d 6f64 656c  8(tgt_ctx, model
+00007d70: 2c20 7768 6572 6529 0a20 2020 2020 2020  , where).       
+00007d80: 2020 2020 2069 6620 6964 733a 0a20 2020       if ids:.   
+00007d90: 2020 2020 2020 2020 2020 2020 2069 6420               id 
+00007da0: 3d20 6964 735b 305d 0a20 2020 2020 2020  = ids[0].       
+00007db0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+00007dc0: 2020 2072 6574 7572 6e20 6964 0a0a 0a64     return id...d
+00007dd0: 6566 2063 6f70 795f 7265 636f 7264 2874  ef copy_record(t
+00007de0: 6774 5f63 7478 2c20 7372 635f 6374 782c  gt_ctx, src_ctx,
+00007df0: 206d 6f64 656c 2c20 7265 632c 206d 6f64   model, rec, mod
+00007e00: 653d 4e6f 6e65 293a 0a20 2020 206d 7367  e=None):.    msg
+00007e10: 5f62 7572 7374 2827 2573 2025 6427 2025  _burst('%s %d' %
+00007e20: 2028 6d6f 6465 6c2c 2072 6563 2e69 6429   (model, rec.id)
+00007e30: 290a 2020 2020 6d6f 6465 203d 206d 6f64  ).    mode = mod
+00007e40: 6520 6f72 2067 6574 5f6d 6f64 656c 5f63  e or get_model_c
+00007e50: 6f70 795f 6d6f 6465 2873 7263 5f63 7478  opy_mode(src_ctx
+00007e60: 2c20 6d6f 6465 6c29 0a20 2020 2023 2041  , model).    # A
+00007e70: 766f 6964 206c 6f6f 7020 6e65 7374 696e  void loop nestin
+00007e80: 670a 2020 2020 6361 6368 6520 3d20 6765  g.    cache = ge
+00007e90: 745f 6361 6368 6528 7372 635f 6374 7829  t_cache(src_ctx)
+00007ea0: 0a20 2020 2069 6620 6361 6368 655f 6973  .    if cache_is
+00007eb0: 5f65 6e74 7279 2863 6163 6865 2c20 6d6f  _entry(cache, mo
+00007ec0: 6465 6c2c 2072 6563 2e69 6429 3a0a 2020  del, rec.id):.  
+00007ed0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00007ee0: 2063 6163 6865 5f73 746f 7265 5f65 6e74   cache_store_ent
+00007ef0: 7279 2863 6163 6865 2c20 6d6f 6465 6c2c  ry(cache, model,
+00007f00: 2046 616c 7365 2c20 6b65 6570 3d54 7275   False, keep=Tru
+00007f10: 6529 0a20 2020 2076 616c 7320 3d20 6c6f  e).    vals = lo
+00007f20: 6164 5f72 6563 6f72 6428 7467 745f 6374  ad_record(tgt_ct
+00007f30: 782c 2073 7263 5f63 7478 2c20 6d6f 6465  x, src_ctx, mode
+00007f40: 6c2c 2072 6563 2c20 6d6f 6465 3d6d 6f64  l, rec, mode=mod
+00007f50: 6529 0a20 2020 2069 6620 6e6f 7420 7661  e).    if not va
+00007f60: 6c73 3a0a 2020 2020 2020 2020 7265 7475  ls:.        retu
+00007f70: 726e 0a20 2020 2069 6620 6d6f 6465 203d  rn.    if mode =
+00007f80: 3d20 2769 6d61 6765 273a 0a20 2020 2020  = 'image':.     
+00007f90: 2020 2069 6473 203d 2063 6c6f 646f 6f2e     ids = clodoo.
+00007fa0: 7365 6172 6368 4c38 2874 6774 5f63 7478  searchL8(tgt_ctx
+00007fb0: 2c20 6d6f 6465 6c2c 205b 2827 6964 272c  , model, [('id',
+00007fc0: 2027 3d27 2c20 7265 632e 6964 295d 290a   '=', rec.id)]).
+00007fd0: 2020 2020 2020 2020 6966 2069 6473 3a0a          if ids:.
+00007fe0: 2020 2020 2020 2020 2020 2020 7772 6974              writ
+00007ff0: 655f 6e6f 5f64 7570 2874 6774 5f63 7478  e_no_dup(tgt_ctx
+00008000: 2c20 6d6f 6465 6c2c 2069 6473 2c20 7661  , model, ids, va
+00008010: 6c73 2c20 7265 632e 6964 290a 2020 2020  ls, rec.id).    
+00008020: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008030: 2020 2020 2020 6964 203d 2063 7265 6174        id = creat
+00008040: 655f 7769 7468 5f69 6428 7467 745f 6374  e_with_id(tgt_ct
+00008050: 782c 206d 6f64 656c 2c20 7265 632e 6964  x, model, rec.id
+00008060: 2c20 7661 6c73 290a 2020 2020 656c 6966  , vals).    elif
+00008070: 2075 7365 5f73 796e 6368 726f 2874 6774   use_synchro(tgt
+00008080: 5f63 7478 2c20 6d6f 6465 6c29 3a0a 2020  _ctx, model):.  
+00008090: 2020 2020 2020 7661 6c73 5b27 6f65 375f        vals['oe7_
+000080a0: 6964 275d 203d 2072 6563 2e69 640a 2020  id'] = rec.id.  
+000080b0: 2020 2020 2020 6964 203d 2063 6c6f 646f        id = clodo
+000080c0: 6f2e 6578 6563 7574 654c 3828 7467 745f  o.executeL8(tgt_
+000080d0: 6374 782c 206d 6f64 656c 2c20 2773 796e  ctx, model, 'syn
+000080e0: 6368 726f 272c 2076 616c 7329 0a20 2020  chro', vals).   
+000080f0: 2065 6c73 653a 0a20 2020 2020 2020 2073   else:.        s
+00008100: 796e 6368 726f 2874 6774 5f63 7478 2c20  ynchro(tgt_ctx, 
+00008110: 6d6f 6465 6c2c 2076 616c 7329 0a0a 0a64  model, vals)...d
+00008120: 6566 2064 6574 6169 6c5f 6d6f 6465 6c28  ef detail_model(
+00008130: 6d6f 6465 6c29 3a0a 2020 2020 6966 206d  model):.    if m
+00008140: 6f64 656c 2069 6e20 2827 6163 636f 756e  odel in ('accoun
+00008150: 742e 696e 766f 6963 6527 2c20 2773 616c  t.invoice', 'sal
+00008160: 652e 6f72 6465 7227 293a 0a20 2020 2020  e.order'):.     
+00008170: 2020 2072 6574 7572 6e20 2725 732e 6c69     return '%s.li
+00008180: 6e65 2720 2520 6d6f 6465 6c0a 2020 2020  ne' % model.    
+00008190: 7265 7475 726e 2046 616c 7365 0a0a 0a64  return False...d
+000081a0: 6566 2073 6574 5f77 6865 7265 5f66 726f  ef set_where_fro
+000081b0: 6d5f 7478 7469 6473 2876 616c 7565 293a  m_txtids(value):
+000081c0: 0a20 2020 2077 6865 7265 203d 205b 5d0a  .    where = [].
+000081d0: 2020 2020 6966 2076 616c 7565 3a0a 2020      if value:.  
+000081e0: 2020 2020 2020 6964 7320 3d20 6576 616c        ids = eval
+000081f0: 2876 616c 7565 290a 2020 2020 2020 2020  (value).        
+00008200: 6966 2069 7369 6e73 7461 6e63 6528 6964  if isinstance(id
+00008210: 732c 2028 696e 742c 206c 6f6e 6729 293a  s, (int, long)):
+00008220: 0a20 2020 2020 2020 2020 2020 2077 6865  .            whe
+00008230: 7265 2e61 7070 656e 6428 2827 6964 272c  re.append(('id',
+00008240: 2027 3d27 2c20 6964 7329 290a 2020 2020   '=', ids)).    
+00008250: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008260: 2020 2020 2020 7768 6572 652e 6170 7065        where.appe
+00008270: 6e64 2828 2769 6427 2c20 2769 6e27 2c20  nd(('id', 'in', 
+00008280: 6964 7329 290a 2020 2020 7265 7475 726e  ids)).    return
+00008290: 2077 6865 7265 0a0a 0a64 6566 2063 6f70   where...def cop
+000082a0: 795f 7461 626c 6528 7467 745f 6374 782c  y_table(tgt_ctx,
+000082b0: 2073 7263 5f63 7478 2c20 6d6f 6465 6c2c   src_ctx, model,
+000082c0: 206d 6f64 653d 4e6f 6e65 293a 0a20 2020   mode=None):.   
+000082d0: 2063 6c6f 646f 6f2e 6765 745f 6d6f 6465   clodoo.get_mode
+000082e0: 6c5f 7374 7275 6374 7572 6528 0a20 2020  l_structure(.   
+000082f0: 2020 2020 2073 7263 5f63 7478 2c20 6d6f       src_ctx, mo
+00008300: 6465 6c2c 2069 676e 6f72 653d 4947 4e4f  del, ignore=IGNO
+00008310: 5245 5f46 4945 4c44 532e 6765 7428 6d6f  RE_FIELDS.get(mo
+00008320: 6465 6c2c 205b 5d29 202b 2049 474e 4f52  del, []) + IGNOR
+00008330: 455f 4649 454c 4453 5b27 2a27 5d0a 2020  E_FIELDS['*'].  
+00008340: 2020 290a 2020 2020 636c 6f64 6f6f 2e67    ).    clodoo.g
+00008350: 6574 5f6d 6f64 656c 5f73 7472 7563 7475  et_model_structu
+00008360: 7265 280a 2020 2020 2020 2020 7467 745f  re(.        tgt_
+00008370: 6374 782c 206d 6f64 656c 2c20 6967 6e6f  ctx, model, igno
+00008380: 7265 3d49 474e 4f52 455f 4649 454c 4453  re=IGNORE_FIELDS
+00008390: 2e67 6574 286d 6f64 656c 2c20 5b5d 2920  .get(model, []) 
+000083a0: 2b20 4947 4e4f 5245 5f46 4945 4c44 535b  + IGNORE_FIELDS[
+000083b0: 272a 275d 0a20 2020 2029 0a20 2020 2064  '*'].    ).    d
+000083c0: 6574 5f6d 6f64 656c 203d 2064 6574 6169  et_model = detai
+000083d0: 6c5f 6d6f 6465 6c28 6d6f 6465 6c29 0a20  l_model(model). 
+000083e0: 2020 2069 6620 6465 745f 6d6f 6465 6c3a     if det_model:
+000083f0: 0a20 2020 2020 2020 2063 6c6f 646f 6f2e  .        clodoo.
+00008400: 6765 745f 6d6f 6465 6c5f 7374 7275 6374  get_model_struct
+00008410: 7572 6528 0a20 2020 2020 2020 2020 2020  ure(.           
+00008420: 2073 7263 5f63 7478 2c0a 2020 2020 2020   src_ctx,.      
+00008430: 2020 2020 2020 6465 745f 6d6f 6465 6c2c        det_model,
+00008440: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
+00008450: 6f72 653d 4947 4e4f 5245 5f46 4945 4c44  ore=IGNORE_FIELD
+00008460: 532e 6765 7428 6465 745f 6d6f 6465 6c2c  S.get(det_model,
+00008470: 205b 5d29 202b 2049 474e 4f52 455f 4649   []) + IGNORE_FI
+00008480: 454c 4453 5b27 2a27 5d2c 0a20 2020 2020  ELDS['*'],.     
+00008490: 2020 2029 0a20 2020 2020 2020 2063 6c6f     ).        clo
+000084a0: 646f 6f2e 6765 745f 6d6f 6465 6c5f 7374  doo.get_model_st
+000084b0: 7275 6374 7572 6528 0a20 2020 2020 2020  ructure(.       
+000084c0: 2020 2020 2074 6774 5f63 7478 2c0a 2020       tgt_ctx,.  
+000084d0: 2020 2020 2020 2020 2020 6465 745f 6d6f            det_mo
+000084e0: 6465 6c2c 0a20 2020 2020 2020 2020 2020  del,.           
+000084f0: 2069 676e 6f72 653d 4947 4e4f 5245 5f46   ignore=IGNORE_F
+00008500: 4945 4c44 532e 6765 7428 6465 745f 6d6f  IELDS.get(det_mo
+00008510: 6465 6c2c 205b 5d29 202b 2049 474e 4f52  del, []) + IGNOR
+00008520: 455f 4649 454c 4453 5b27 2a27 5d2c 0a20  E_FIELDS['*'],. 
+00008530: 2020 2020 2020 2029 0a20 2020 2074 6774         ).    tgt
+00008540: 5f63 7478 5b27 5f43 4f4d 4d49 5427 5d20  _ctx['_COMMIT'] 
+00008550: 3d20 7b7d 0a0a 2020 2020 6d6f 6465 203d  = {}..    mode =
+00008560: 206d 6f64 6520 6f72 2067 6574 5f6d 6f64   mode or get_mod
+00008570: 656c 5f63 6f70 795f 6d6f 6465 2873 7263  el_copy_mode(src
+00008580: 5f63 7478 2c20 6d6f 6465 6c29 0a20 2020  _ctx, model).   
+00008590: 2069 6620 6d6f 6465 203d 3d20 2769 6d61   if mode == 'ima
+000085a0: 6765 2720 616e 6420 7372 635f 6374 785b  ge' and src_ctx[
+000085b0: 275f 6372 275d 3a0a 2020 2020 2020 2020  '_cr']:.        
+000085c0: 7461 626c 6520 3d20 6d6f 6465 6c2e 7265  table = model.re
+000085d0: 706c 6163 6528 272e 272c 2027 5f27 290a  place('.', '_').
+000085e0: 2020 2020 2020 2020 7371 6c20 3d20 2773          sql = 's
+000085f0: 656c 6563 7420 6d61 7828 6964 2920 6672  elect max(id) fr
+00008600: 6f6d 2025 733b 2720 2520 7461 626c 650a  om %s;' % table.
+00008610: 2020 2020 2020 2020 726f 7773 203d 2065          rows = e
+00008620: 7865 635f 7371 6c28 7372 635f 6374 782c  xec_sql(src_ctx,
+00008630: 2073 716c 2c20 7265 7370 6f6e 7365 3d54   sql, response=T
+00008640: 7275 6529 0a20 2020 2020 2020 206c 6173  rue).        las
+00008650: 745f 6964 203d 2072 6f77 735b 305d 5b30  t_id = rows[0][0
+00008660: 5d0a 2020 2020 2020 2020 6966 206c 6173  ].        if las
+00008670: 745f 6964 203e 2030 3a0a 2020 2020 2020  t_id > 0:.      
+00008680: 2020 2020 2020 666f 7220 6964 2069 6e20        for id in 
+00008690: 636c 6f64 6f6f 2e73 6561 7263 684c 3828  clodoo.searchL8(
+000086a0: 7467 745f 6374 782c 206d 6f64 656c 2c20  tgt_ctx, model, 
+000086b0: 5b28 2769 6427 2c20 273e 272c 206c 6173  [('id', '>', las
+000086c0: 745f 6964 295d 293a 0a20 2020 2020 2020  t_id)]):.       
+000086d0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086f0: 2020 636c 6f64 6f6f 2e75 6e6c 696e 6b4c    clodoo.unlinkL
+00008700: 3828 7467 745f 6374 782c 206d 6f64 656c  8(tgt_ctx, model
+00008710: 2c20 6964 290a 2020 2020 2020 2020 2020  , id).          
+00008720: 2020 2020 2020 6578 6365 7074 2049 4f45        except IOE
+00008730: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+00008740: 2020 2020 2020 2020 2020 6f73 302e 776c            os0.wl
+00008750: 6f67 2822 4361 6e6e 6f74 2064 656c 6574  og("Cannot delet
+00008760: 6520 7265 636f 7264 2025 6420 6f66 2025  e record %d of %
+00008770: 7322 2025 2028 6964 2c20 6d6f 6465 6c29  s" % (id, model)
+00008780: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008790: 2020 2020 2020 6966 206e 6f74 2074 6774        if not tgt
+000087a0: 5f63 7478 5b27 6173 7375 6d65 5f79 6573  _ctx['assume_yes
+000087b0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+000087c0: 2020 2020 2020 2020 2020 2020 6475 6d6d              dumm
+000087d0: 7920 3d20 696e 7075 7428 2750 7265 7373  y = input('Press
+000087e0: 2052 4554 2074 6f20 636f 6e74 696e 7565   RET to continue
+000087f0: 2729 0a20 2020 2077 6865 7265 203d 2073  ').    where = s
+00008800: 6574 5f77 6865 7265 5f66 726f 6d5f 7478  et_where_from_tx
+00008810: 7469 6473 2873 7263 5f63 7478 5b27 7365  tids(src_ctx['se
+00008820: 6c5f 6964 7327 5d29 0a20 2020 2069 6620  l_ids']).    if 
+00008830: 7372 635f 6374 785b 2762 795f 636f 6d70  src_ctx['by_comp
+00008840: 616e 7927 5d3a 0a20 2020 2020 2020 2063  any']:.        c
+00008850: 6f6d 7061 6e79 5f69 6420 3d20 656e 765f  ompany_id = env_
+00008860: 7265 6628 7372 635f 6374 782c 2027 7a30  ref(src_ctx, 'z0
+00008870: 6275 672e 6d79 636f 6d70 616e 7927 290a  bug.mycompany').
+00008880: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
+00008890: 6f6d 7061 6e79 5f69 643a 0a20 2020 2020  ompany_id:.     
+000088a0: 2020 2020 2020 2070 7269 6e74 2827 2121         print('!!
+000088b0: 496e 7465 726e 616c 2065 7272 6f72 3a20  Internal error: 
+000088c0: 6e6f 2063 6f6d 7061 6e79 2066 6f75 6e64  no company found
+000088d0: 2127 290a 2020 2020 2020 2020 656c 7365  !').        else
+000088e0: 3a0a 2020 2020 2020 2020 2020 2020 7768  :.            wh
+000088f0: 6572 652e 6170 7065 6e64 2828 2763 6f6d  ere.append(('com
+00008900: 7061 6e79 5f69 6427 2c20 273d 272c 2063  pany_id', '=', c
+00008910: 6f6d 7061 6e79 5f69 6429 290a 2020 2020  ompany_id)).    
+00008920: 666f 7220 7265 6320 696e 2063 6c6f 646f  for rec in clodo
+00008930: 6f2e 6272 6f77 7365 4c38 280a 2020 2020  o.browseL8(.    
+00008940: 2020 2020 7372 635f 6374 782c 0a20 2020      src_ctx,.   
+00008950: 2020 2020 206d 6f64 656c 2c0a 2020 2020       model,.    
+00008960: 2020 2020 636c 6f64 6f6f 2e73 6561 7263      clodoo.searc
+00008970: 684c 3828 7372 635f 6374 782c 206d 6f64  hL8(src_ctx, mod
+00008980: 656c 2c20 7768 6572 652c 206f 7264 6572  el, where, order
+00008990: 3d27 6964 2729 2c0a 2020 2020 2020 2020  ='id'),.        
+000089a0: 636f 6e74 6578 743d 7b27 6c61 6e67 273a  context={'lang':
+000089b0: 2027 656e 5f55 5327 7d2c 0a20 2020 2029   'en_US'},.    )
+000089c0: 3a0a 2020 2020 2020 2020 636f 7079 5f72  :.        copy_r
+000089d0: 6563 6f72 6428 7467 745f 6374 782c 2073  ecord(tgt_ctx, s
+000089e0: 7263 5f63 7478 2c20 6d6f 6465 6c2c 2072  rc_ctx, model, r
+000089f0: 6563 2c20 6d6f 6465 3d6d 6f64 6529 0a20  ec, mode=mode). 
+00008a00: 2020 2020 2020 2069 6620 6465 745f 6d6f         if det_mo
+00008a10: 6465 6c3a 0a20 2020 2020 2020 2020 2020  del:.           
+00008a20: 2064 6574 5f66 6965 6c64 203d 2074 7261   det_field = tra
+00008a30: 6e73 6f64 6f6f 2e74 7261 6e73 6c61 7465  nsodoo.translate
+00008a40: 5f66 726f 6d5f 746f 280a 2020 2020 2020  _from_to(.      
+00008a50: 2020 2020 2020 2020 2020 7372 635f 6374            src_ct
+00008a60: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
+00008a70: 2020 206d 6f64 656c 2c0a 2020 2020 2020     model,.      
+00008a80: 2020 2020 2020 2020 2020 4445 545f 4649            DET_FI
+00008a90: 454c 445b 6d6f 6465 6c5d 2c0a 2020 2020  ELD[model],.    
+00008aa0: 2020 2020 2020 2020 2020 2020 2737 2e30              '7.0
+00008ab0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00008ac0: 2020 2073 7263 5f63 7478 5b27 6f65 5f76     src_ctx['oe_v
+00008ad0: 6572 7369 6f6e 275d 2c0a 2020 2020 2020  ersion'],.      
+00008ae0: 2020 2020 2020 2020 2020 7479 7065 3d27            type='
+00008af0: 6669 656c 6427 2c0a 2020 2020 2020 2020  field',.        
+00008b00: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00008b10: 2020 666f 7220 6465 745f 7265 6320 696e    for det_rec in
+00008b20: 2072 6563 5b64 6574 5f66 6965 6c64 5d3a   rec[det_field]:
+00008b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008b40: 2063 6f70 795f 7265 636f 7264 2874 6774   copy_record(tgt
+00008b50: 5f63 7478 2c20 7372 635f 6374 782c 2064  _ctx, src_ctx, d
+00008b60: 6574 5f6d 6f64 656c 2c20 6465 745f 7265  et_model, det_re
+00008b70: 632c 206d 6f64 653d 6d6f 6465 290a 2020  c, mode=mode).  
+00008b80: 2020 6966 2064 6574 5f6d 6f64 656c 3a0a    if det_model:.
+00008b90: 2020 2020 2020 2020 636f 6d6d 6974 5f74          commit_t
+00008ba0: 6162 6c65 2874 6774 5f63 7478 2c20 7372  able(tgt_ctx, sr
+00008bb0: 635f 6374 782c 206d 6f64 656c 290a 0a0a  c_ctx, model)...
+00008bc0: 6465 6620 6973 5f73 7973 7465 6d5f 6d6f  def is_system_mo
+00008bd0: 6465 6c28 6d6f 6465 6c29 3a0a 2020 2020  del(model):.    
+00008be0: 6973 5f73 7973 7465 6d20 3d20 4661 6c73  is_system = Fals
+00008bf0: 650a 2020 2020 666f 7220 726f 6f74 2069  e.    for root i
+00008c00: 6e20 5359 5354 454d 5f4d 4f44 454c 5f52  n SYSTEM_MODEL_R
+00008c10: 4f4f 543a 0a20 2020 2020 2020 2069 6620  OOT:.        if 
+00008c20: 6d6f 6465 6c2e 7374 6172 7473 7769 7468  model.startswith
+00008c30: 2872 6f6f 7429 3a0a 2020 2020 2020 2020  (root):.        
+00008c40: 2020 2020 6973 5f73 7973 7465 6d20 3d20      is_system = 
+00008c50: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+00008c60: 2062 7265 616b 0a20 2020 2069 6620 6d6f   break.    if mo
+00008c70: 6465 6c20 696e 2053 5953 5445 4d5f 4d4f  del in SYSTEM_MO
+00008c80: 4445 4c53 3a0a 2020 2020 2020 2020 6973  DELS:.        is
+00008c90: 5f73 7973 7465 6d20 3d20 5472 7565 0a20  _system = True. 
+00008ca0: 2020 2072 6574 7572 6e20 6973 5f73 7973     return is_sys
+00008cb0: 7465 6d0a 0a0a 6465 6620 6275 696c 645f  tem...def build_
+00008cc0: 7461 626c 655f 7472 6565 2863 7478 293a  table_tree(ctx):
+00008cd0: 0a20 2020 2064 6566 206e 6577 5f65 6d70  .    def new_emp
+00008ce0: 7479 5f6d 6f64 656c 286d 6f64 656c 732c  ty_model(models,
+00008cf0: 206d 6f64 656c 293a 0a20 2020 2020 2020   model):.       
+00008d00: 2069 6620 6d6f 6465 6c20 6e6f 7420 696e   if model not in
+00008d10: 206d 6f64 656c 733a 0a20 2020 2020 2020   models:.       
+00008d20: 2020 2020 206d 6f64 656c 735b 6d6f 6465       models[mode
+00008d30: 6c5d 203d 207b 7d0a 2020 2020 2020 2020  l] = {}.        
+00008d40: 2020 2020 6d6f 6465 6c73 5b6d 6f64 656c      models[model
+00008d50: 5d5b 2764 6570 656e 6473 275d 203d 205b  ]['depends'] = [
+00008d60: 5d0a 2020 2020 2020 2020 2020 2020 6d6f  ].            mo
+00008d70: 6465 6c73 5b6d 6f64 656c 5d5b 276d 6179  dels[model]['may
+00008d80: 6465 7065 6e64 7327 5d20 3d20 5b5d 0a20  depends'] = []. 
+00008d90: 2020 2020 2020 2020 2020 206d 6f64 656c             model
+00008da0: 735b 6d6f 6465 6c5d 5b27 6d32 6d27 5d20  s[model]['m2m'] 
+00008db0: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+00008dc0: 206d 6f64 656c 735b 6d6f 6465 6c5d 5b27   models[model]['
+00008dd0: 6372 6f73 7364 6570 275d 203d 205b 5d0a  crossdep'] = [].
+00008de0: 0a20 2020 206d 6f64 656c 5f6c 6973 7420  .    model_list 
+00008df0: 3d20 5b5d 0a20 2020 206d 6f64 656c 7320  = [].    models 
+00008e00: 3d20 7b7d 0a20 2020 2066 6f72 206d 6f64  = {}.    for mod
+00008e10: 656c 5f72 6563 2069 6e20 636c 6f64 6f6f  el_rec in clodoo
+00008e20: 2e62 726f 7773 654c 3828 0a20 2020 2020  .browseL8(.     
+00008e30: 2020 2063 7478 2c20 2769 722e 6d6f 6465     ctx, 'ir.mode
+00008e40: 6c27 2c20 636c 6f64 6f6f 2e73 6561 7263  l', clodoo.searc
+00008e50: 684c 3828 6374 782c 2027 6972 2e6d 6f64  hL8(ctx, 'ir.mod
+00008e60: 656c 272c 205b 5d29 0a20 2020 2029 3a0a  el', []).    ):.
+00008e70: 2020 2020 2020 2020 6d6f 6465 6c20 3d20          model = 
+00008e80: 6d6f 6465 6c5f 7265 632e 6d6f 6465 6c0a  model_rec.model.
+00008e90: 2020 2020 2020 2020 6966 2069 735f 7379          if is_sy
+00008ea0: 7374 656d 5f6d 6f64 656c 286d 6f64 656c  stem_model(model
+00008eb0: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+00008ec0: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+00008ed0: 6d73 675f 6275 7273 7428 2720 2020 2067  msg_burst('    g
+00008ee0: 6574 2025 7320 2e2e 2e27 2025 206d 6f64  et %s ...' % mod
+00008ef0: 656c 290a 2020 2020 2020 2020 6d6f 6465  el).        mode
+00008f00: 6c5f 6c69 7374 2e61 7070 656e 6428 6d6f  l_list.append(mo
+00008f10: 6465 6c29 0a20 2020 2020 2020 206e 6577  del).        new
+00008f20: 5f65 6d70 7479 5f6d 6f64 656c 286d 6f64  _empty_model(mod
+00008f30: 656c 732c 206d 6f64 656c 290a 2020 2020  els, model).    
+00008f40: 2020 2020 6c65 7665 6c20 3d20 300a 2020      level = 0.  
+00008f50: 2020 2020 2020 666f 7220 6669 656c 6420        for field 
+00008f60: 696e 2063 6c6f 646f 6f2e 6272 6f77 7365  in clodoo.browse
+00008f70: 4c38 280a 2020 2020 2020 2020 2020 2020  L8(.            
+00008f80: 6374 782c 0a20 2020 2020 2020 2020 2020  ctx,.           
+00008f90: 2027 6972 2e6d 6f64 656c 2e66 6965 6c64   'ir.model.field
+00008fa0: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
+00008fb0: 636c 6f64 6f6f 2e73 6561 7263 684c 3828  clodoo.searchL8(
+00008fc0: 6374 782c 2027 6972 2e6d 6f64 656c 2e66  ctx, 'ir.model.f
+00008fd0: 6965 6c64 7327 2c20 5b28 276d 6f64 656c  ields', [('model
+00008fe0: 272c 2027 3d27 2c20 6d6f 6465 6c29 5d29  ', '=', model)])
+00008ff0: 2c0a 2020 2020 2020 2020 293a 0a20 2020  ,.        ):.   
+00009000: 2020 2020 2020 2020 2069 6620 6669 656c           if fiel
+00009010: 642e 7474 7970 6520 3d3d 2027 6d61 6e79  d.ttype == 'many
+00009020: 326f 6e65 2720 616e 6420 6669 656c 642e  2one' and field.
+00009030: 7265 6c61 7469 6f6e 2021 3d20 6d6f 6465  relation != mode
+00009040: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+00009050: 2020 2069 6620 6669 656c 642e 7265 6c61     if field.rela
+00009060: 7469 6f6e 206e 6f74 2069 6e20 6d6f 6465  tion not in mode
+00009070: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
+00009080: 2020 2020 2020 2020 6e65 775f 656d 7074          new_empt
+00009090: 795f 6d6f 6465 6c28 6d6f 6465 6c73 2c20  y_model(models, 
+000090a0: 6669 656c 642e 7265 6c61 7469 6f6e 290a  field.relation).
+000090b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090c0: 6966 2066 6965 6c64 2e72 6571 7569 7265  if field.require
+000090d0: 6420 616e 6420 6669 656c 642e 7265 6c61  d and field.rela
+000090e0: 7469 6f6e 206e 6f74 2069 6e20 6d6f 6465  tion not in mode
+000090f0: 6c73 5b6d 6f64 656c 5d5b 2764 6570 656e  ls[model]['depen
+00009100: 6473 275d 3a0a 2020 2020 2020 2020 2020  ds']:.          
+00009110: 2020 2020 2020 2020 2020 6d6f 6465 6c73            models
+00009120: 5b6d 6f64 656c 5d5b 2764 6570 656e 6473  [model]['depends
+00009130: 275d 2e61 7070 656e 6428 6669 656c 642e  '].append(field.
+00009140: 7265 6c61 7469 6f6e 290a 2020 2020 2020  relation).      
+00009150: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+00009160: 7665 6c20 3d20 2d31 0a20 2020 2020 2020  vel = -1.       
+00009170: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
+00009180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009190: 2020 6e6f 7420 6669 656c 642e 7265 7175    not field.requ
+000091a0: 6972 6564 0a20 2020 2020 2020 2020 2020  ired.           
+000091b0: 2020 2020 2020 2020 2061 6e64 2066 6965           and fie
+000091c0: 6c64 2e72 656c 6174 696f 6e20 6e6f 7420  ld.relation not 
+000091d0: 696e 206d 6f64 656c 735b 6d6f 6465 6c5d  in models[model]
+000091e0: 5b27 6d61 7964 6570 656e 6473 275d 0a20  ['maydepends']. 
+000091f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00009200: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009210: 2020 2020 2020 6d6f 6465 6c73 5b6d 6f64        models[mod
+00009220: 656c 5d5b 276d 6179 6465 7065 6e64 7327  el]['maydepends'
+00009230: 5d2e 6170 7065 6e64 2866 6965 6c64 2e72  ].append(field.r
+00009240: 656c 6174 696f 6e29 0a20 2020 2020 2020  elation).       
+00009250: 2020 2020 2065 6c69 6620 6669 656c 642e       elif field.
+00009260: 7474 7970 6520 3d3d 2027 6f6e 6532 6d61  ttype == 'one2ma
+00009270: 6e79 2720 616e 6420 6669 656c 642e 7265  ny' and field.re
+00009280: 6c61 7469 6f6e 2021 3d20 6d6f 6465 6c3a  lation != model:
+00009290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000092a0: 2069 6620 6669 656c 642e 7265 6c61 7469   if field.relati
+000092b0: 6f6e 206e 6f74 2069 6e20 6d6f 6465 6c73  on not in models
+000092c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000092d0: 2020 2020 2020 6e65 775f 656d 7074 795f        new_empty_
+000092e0: 6d6f 6465 6c28 6d6f 6465 6c73 2c20 6669  model(models, fi
+000092f0: 656c 642e 7265 6c61 7469 6f6e 290a 2020  eld.relation).  
+00009300: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00009310: 2066 6965 6c64 2e72 6571 7569 7265 6420   field.required 
+00009320: 616e 6420 6d6f 6465 6c20 6e6f 7420 696e  and model not in
+00009330: 206d 6f64 656c 735b 6669 656c 642e 7265   models[field.re
+00009340: 6c61 7469 6f6e 5d5b 2764 6570 656e 6473  lation]['depends
+00009350: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+00009360: 2020 2020 2020 2020 6d6f 6465 6c73 5b66          models[f
+00009370: 6965 6c64 2e72 656c 6174 696f 6e5d 5b27  ield.relation]['
+00009380: 6465 7065 6e64 7327 5d2e 6170 7065 6e64  depends'].append
+00009390: 286d 6f64 656c 290a 2020 2020 2020 2020  (model).        
+000093a0: 2020 2020 2020 2020 2020 2020 6c65 7665              leve
+000093b0: 6c20 3d20 2d31 0a20 2020 2020 2020 2020  l = -1.         
+000093c0: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
+000093d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093e0: 6e6f 7420 6669 656c 642e 7265 7175 6972  not field.requir
+000093f0: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
+00009400: 2020 2020 2020 2061 6e64 206d 6f64 656c         and model
+00009410: 206e 6f74 2069 6e20 6d6f 6465 6c73 5b66   not in models[f
+00009420: 6965 6c64 2e72 656c 6174 696f 6e5d 5b27  ield.relation]['
+00009430: 6d61 7964 6570 656e 6473 275d 0a20 2020  maydepends'].   
+00009440: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
+00009450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009460: 2020 2020 6d6f 6465 6c73 5b66 6965 6c64      models[field
+00009470: 2e72 656c 6174 696f 6e5d 5b27 6d61 7964  .relation]['mayd
+00009480: 6570 656e 6473 275d 2e61 7070 656e 6428  epends'].append(
+00009490: 6d6f 6465 6c29 0a20 2020 2020 2020 2020  model).         
+000094a0: 2020 2065 6c69 6620 6669 656c 642e 7474     elif field.tt
+000094b0: 7970 6520 696e 2027 6d61 6e79 326d 616e  ype in 'many2man
+000094c0: 7927 2061 6e64 2066 6965 6c64 2e72 656c  y' and field.rel
+000094d0: 6174 696f 6e20 213d 206d 6f64 656c 3a0a  ation != model:.
 000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009500: 2020 2020 2020 2073 7263 5f63 7478 5b27         src_ctx['
-00009510: 6f65 5f76 6572 7369 6f6e 275d 2c0a 2020  oe_version'],.  
-00009520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009550: 2020 7479 7065 3d27 6669 656c 6427 290a    type='field').
-00009560: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00009570: 6465 745f 7265 6320 696e 2072 6563 5b64  det_rec in rec[d
-00009580: 6574 5f66 6965 6c64 5d3a 0a20 2020 2020  et_field]:.     
-00009590: 2020 2020 2020 2020 2020 2063 6f70 795f             copy_
-000095a0: 7265 636f 7264 2874 6774 5f63 7478 2c20  record(tgt_ctx, 
-000095b0: 7372 635f 6374 782c 2064 6574 5f6d 6f64  src_ctx, det_mod
-000095c0: 656c 2c20 6465 745f 7265 632c 206d 6f64  el, det_rec, mod
-000095d0: 653d 6d6f 6465 290a 2020 2020 6966 2064  e=mode).    if d
-000095e0: 6574 5f6d 6f64 656c 3a0a 2020 2020 2020  et_model:.      
-000095f0: 2020 636f 6d6d 6974 5f74 6162 6c65 2874    commit_table(t
-00009600: 6774 5f63 7478 2c20 7372 635f 6374 782c  gt_ctx, src_ctx,
-00009610: 206d 6f64 656c 290a 0a0a 6465 6620 6973   model)...def is
-00009620: 5f73 7973 7465 6d5f 6d6f 6465 6c28 6d6f  _system_model(mo
-00009630: 6465 6c29 3a0a 2020 2020 6973 5f73 7973  del):.    is_sys
-00009640: 7465 6d20 3d20 4661 6c73 650a 2020 2020  tem = False.    
-00009650: 666f 7220 726f 6f74 2069 6e20 5359 5354  for root in SYST
-00009660: 454d 5f4d 4f44 454c 5f52 4f4f 543a 0a20  EM_MODEL_ROOT:. 
-00009670: 2020 2020 2020 2069 6620 6d6f 6465 6c2e         if model.
-00009680: 7374 6172 7473 7769 7468 2872 6f6f 7429  startswith(root)
-00009690: 3a0a 2020 2020 2020 2020 2020 2020 6973  :.            is
-000096a0: 5f73 7973 7465 6d20 3d20 5472 7565 0a20  _system = True. 
-000096b0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-000096c0: 0a20 2020 2069 6620 6d6f 6465 6c20 696e  .    if model in
-000096d0: 2053 5953 5445 4d5f 4d4f 4445 4c53 3a0a   SYSTEM_MODELS:.
-000096e0: 2020 2020 2020 2020 6973 5f73 7973 7465          is_syste
-000096f0: 6d20 3d20 5472 7565 0a20 2020 2072 6574  m = True.    ret
-00009700: 7572 6e20 6973 5f73 7973 7465 6d0a 0a0a  urn is_system...
-00009710: 6465 6620 6275 696c 645f 7461 626c 655f  def build_table_
-00009720: 7472 6565 2863 7478 293a 0a20 2020 2064  tree(ctx):.    d
-00009730: 6566 206e 6577 5f65 6d70 7479 5f6d 6f64  ef new_empty_mod
-00009740: 656c 286d 6f64 656c 732c 206d 6f64 656c  el(models, model
-00009750: 293a 0a20 2020 2020 2020 2069 6620 6d6f  ):.        if mo
-00009760: 6465 6c20 6e6f 7420 696e 206d 6f64 656c  del not in model
-00009770: 733a 0a20 2020 2020 2020 2020 2020 206d  s:.            m
-00009780: 6f64 656c 735b 6d6f 6465 6c5d 203d 207b  odels[model] = {
-00009790: 7d0a 2020 2020 2020 2020 2020 2020 6d6f  }.            mo
-000097a0: 6465 6c73 5b6d 6f64 656c 5d5b 2764 6570  dels[model]['dep
-000097b0: 656e 6473 275d 203d 205b 5d0a 2020 2020  ends'] = [].    
-000097c0: 2020 2020 2020 2020 6d6f 6465 6c73 5b6d          models[m
-000097d0: 6f64 656c 5d5b 276d 6179 6465 7065 6e64  odel]['maydepend
-000097e0: 7327 5d20 3d20 5b5d 0a20 2020 2020 2020  s'] = [].       
-000097f0: 2020 2020 206d 6f64 656c 735b 6d6f 6465       models[mode
-00009800: 6c5d 5b27 6d32 6d27 5d20 3d20 5b5d 0a20  l]['m2m'] = []. 
-00009810: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-00009820: 735b 6d6f 6465 6c5d 5b27 6372 6f73 7364  s[model]['crossd
-00009830: 6570 275d 203d 205b 5d0a 0a20 2020 206d  ep'] = []..    m
-00009840: 6f64 656c 5f6c 6973 7420 3d20 5b5d 0a20  odel_list = []. 
-00009850: 2020 206d 6f64 656c 7320 3d20 7b7d 0a20     models = {}. 
-00009860: 2020 2066 6f72 206d 6f64 656c 5f72 6563     for model_rec
-00009870: 2069 6e20 636c 6f64 6f6f 2e62 726f 7773   in clodoo.brows
-00009880: 654c 3828 0a20 2020 2020 2020 2063 7478  eL8(.        ctx
-00009890: 2c20 2769 722e 6d6f 6465 6c27 2c20 636c  , 'ir.model', cl
-000098a0: 6f64 6f6f 2e73 6561 7263 684c 3828 0a20  odoo.searchL8(. 
-000098b0: 2020 2020 2020 2020 2020 2063 7478 2c20             ctx, 
-000098c0: 2769 722e 6d6f 6465 6c27 2c20 5b5d 2929  'ir.model', []))
-000098d0: 3a0a 2020 2020 2020 2020 6d6f 6465 6c20  :.        model 
-000098e0: 3d20 6d6f 6465 6c5f 7265 632e 6d6f 6465  = model_rec.mode
-000098f0: 6c0a 2020 2020 2020 2020 6966 2069 735f  l.        if is_
-00009900: 7379 7374 656d 5f6d 6f64 656c 286d 6f64  system_model(mod
-00009910: 656c 293a 0a20 2020 2020 2020 2020 2020  el):.           
-00009920: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-00009930: 2020 6d73 675f 6275 7273 7428 2720 2020    msg_burst('   
-00009940: 2067 6574 2025 7320 2e2e 2e27 2025 206d   get %s ...' % m
-00009950: 6f64 656c 290a 2020 2020 2020 2020 6d6f  odel).        mo
-00009960: 6465 6c5f 6c69 7374 2e61 7070 656e 6428  del_list.append(
-00009970: 6d6f 6465 6c29 0a20 2020 2020 2020 206e  model).        n
-00009980: 6577 5f65 6d70 7479 5f6d 6f64 656c 286d  ew_empty_model(m
-00009990: 6f64 656c 732c 206d 6f64 656c 290a 2020  odels, model).  
-000099a0: 2020 2020 2020 6c65 7665 6c20 3d20 300a        level = 0.
-000099b0: 2020 2020 2020 2020 666f 7220 6669 656c          for fiel
-000099c0: 6420 696e 2063 6c6f 646f 6f2e 6272 6f77  d in clodoo.brow
-000099d0: 7365 4c38 280a 2020 2020 2020 2020 2020  seL8(.          
-000099e0: 2020 6374 782c 2027 6972 2e6d 6f64 656c    ctx, 'ir.model
-000099f0: 2e66 6965 6c64 7327 2c20 636c 6f64 6f6f  .fields', clodoo
-00009a00: 2e73 6561 7263 684c 3828 0a20 2020 2020  .searchL8(.     
-00009a10: 2020 2020 2020 2020 2020 2063 7478 2c20             ctx, 
-00009a20: 2769 722e 6d6f 6465 6c2e 6669 656c 6473  'ir.model.fields
-00009a30: 272c 205b 2827 6d6f 6465 6c27 2c20 273d  ', [('model', '=
-00009a40: 272c 206d 6f64 656c 295d 2929 3a0a 2020  ', model)])):.  
-00009a50: 2020 2020 2020 2020 2020 6966 2066 6965            if fie
-00009a60: 6c64 2e74 7479 7065 203d 3d20 276d 616e  ld.ttype == 'man
-00009a70: 7932 6f6e 6527 2061 6e64 2066 6965 6c64  y2one' and field
-00009a80: 2e72 656c 6174 696f 6e20 213d 206d 6f64  .relation != mod
-00009a90: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
-00009aa0: 2020 2020 6966 2066 6965 6c64 2e72 656c      if field.rel
-00009ab0: 6174 696f 6e20 6e6f 7420 696e 206d 6f64  ation not in mod
-00009ac0: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
-00009ad0: 2020 2020 2020 2020 206e 6577 5f65 6d70           new_emp
-00009ae0: 7479 5f6d 6f64 656c 286d 6f64 656c 732c  ty_model(models,
-00009af0: 2066 6965 6c64 2e72 656c 6174 696f 6e29   field.relation)
-00009b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009b10: 2069 6620 2866 6965 6c64 2e72 6571 7569   if (field.requi
-00009b20: 7265 6420 616e 640a 2020 2020 2020 2020  red and.        
+000094f0: 6966 2066 6965 6c64 2e72 656c 6174 696f  if field.relatio
+00009500: 6e20 6e6f 7420 696e 206d 6f64 656c 733a  n not in models:
+00009510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009520: 2020 2020 206e 6577 5f65 6d70 7479 5f6d       new_empty_m
+00009530: 6f64 656c 286d 6f64 656c 732c 2066 6965  odel(models, fie
+00009540: 6c64 2e72 656c 6174 696f 6e29 0a20 2020  ld.relation).   
+00009550: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00009560: 6669 656c 642e 7265 6c61 7469 6f6e 206e  field.relation n
+00009570: 6f74 2069 6e20 6d6f 6465 6c73 5b6d 6f64  ot in models[mod
+00009580: 656c 5d5b 276d 326d 275d 3a0a 2020 2020  el]['m2m']:.    
+00009590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095a0: 6d6f 6465 6c73 5b6d 6f64 656c 5d5b 276d  models[model]['m
+000095b0: 326d 275d 2e61 7070 656e 6428 6669 656c  2m'].append(fiel
+000095c0: 642e 7265 6c61 7469 6f6e 290a 2020 2020  d.relation).    
+000095d0: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+000095e0: 6f64 656c 206e 6f74 2069 6e20 6d6f 6465  odel not in mode
+000095f0: 6c73 5b66 6965 6c64 2e72 656c 6174 696f  ls[field.relatio
+00009600: 6e5d 5b27 6d32 6d27 5d3a 0a20 2020 2020  n]['m2m']:.     
+00009610: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00009620: 6f64 656c 735b 6669 656c 642e 7265 6c61  odels[field.rela
+00009630: 7469 6f6e 5d5b 276d 326d 275d 2e61 7070  tion]['m2m'].app
+00009640: 656e 6428 6d6f 6465 6c29 0a20 2020 2020  end(model).     
+00009650: 2020 2069 6620 6c65 7665 6c20 3d3d 2030     if level == 0
+00009660: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
+00009670: 6465 6c73 5b6d 6f64 656c 5d5b 276c 6576  dels[model]['lev
+00009680: 656c 275d 203d 206c 6576 656c 0a20 2020  el'] = level.   
+00009690: 2066 6f72 206d 6f64 656c 2069 6e20 6d6f   for model in mo
+000096a0: 6465 6c5f 6c69 7374 3a0a 2020 2020 2020  del_list:.      
+000096b0: 2020 6d73 675f 6275 7273 7428 2720 2020    msg_burst('   
+000096c0: 2063 726f 7373 6465 7020 2573 202e 2e2e   crossdep %s ...
+000096d0: 2720 2520 6d6f 6465 6c29 0a20 2020 2020  ' % model).     
+000096e0: 2020 2066 6f72 2073 7562 2069 6e20 6d6f     for sub in mo
+000096f0: 6465 6c73 5b6d 6f64 656c 5d5b 2764 6570  dels[model]['dep
+00009700: 656e 6473 275d 3a0a 2020 2020 2020 2020  ends']:.        
+00009710: 2020 2020 6966 206d 6f64 656c 2069 6e20      if model in 
+00009720: 6d6f 6465 6c73 5b73 7562 5d5b 2764 6570  models[sub]['dep
+00009730: 656e 6473 275d 3a0a 2020 2020 2020 2020  ends']:.        
+00009740: 2020 2020 2020 2020 6d6f 6465 6c73 5b6d          models[m
+00009750: 6f64 656c 5d5b 2763 726f 7373 6465 7027  odel]['crossdep'
+00009760: 5d20 3d20 7375 620a 2020 2020 2020 2020  ] = sub.        
+00009770: 2020 2020 2020 2020 6d6f 6465 6c73 5b73          models[s
+00009780: 7562 5d5b 2763 726f 7373 6465 7027 5d20  ub]['crossdep'] 
+00009790: 3d20 6d6f 6465 6c0a 2020 2020 666f 7220  = model.    for 
+000097a0: 6d6f 6465 6c20 696e 206d 6f64 656c 5f6c  model in model_l
+000097b0: 6973 743a 0a20 2020 2020 2020 206d 7367  ist:.        msg
+000097c0: 5f62 7572 7374 2827 2020 2020 6465 7065  _burst('    depe
+000097d0: 6e64 656e 6369 6573 2025 7320 2e2e 2e27  ndencies %s ...'
+000097e0: 2025 206d 6f64 656c 290a 2020 2020 2020   % model).      
+000097f0: 2020 6d6f 6465 6c73 5b6d 6f64 656c 5d5b    models[model][
+00009800: 2764 6570 656e 6473 275d 203d 206c 6973  'depends'] = lis
+00009810: 7428 0a20 2020 2020 2020 2020 2020 2073  t(.            s
+00009820: 6574 286d 6f64 656c 735b 6d6f 6465 6c5d  et(models[model]
+00009830: 5b27 6465 7065 6e64 7327 5d29 202d 2073  ['depends']) - s
+00009840: 6574 286d 6f64 656c 735b 6d6f 6465 6c5d  et(models[model]
+00009850: 5b27 6372 6f73 7364 6570 275d 290a 2020  ['crossdep']).  
+00009860: 2020 2020 2020 290a 2020 2020 6d69 7373        ).    miss
+00009870: 6564 5f6d 6f64 656c 7320 3d20 7b7d 0a20  ed_models = {}. 
+00009880: 2020 206d 6178 5f69 7465 7220 3d20 3939     max_iter = 99
+00009890: 0a20 2020 2070 6172 7369 6e67 203d 2054  .    parsing = T
+000098a0: 7275 650a 2020 2020 7768 696c 6520 7061  rue.    while pa
+000098b0: 7273 696e 673a 0a20 2020 2020 2020 2070  rsing:.        p
+000098c0: 6172 7369 6e67 203d 2046 616c 7365 0a20  arsing = False. 
+000098d0: 2020 2020 2020 206d 6178 5f69 7465 7220         max_iter 
+000098e0: 2d3d 2031 0a20 2020 2020 2020 2069 6620  -= 1.        if 
+000098f0: 6d61 785f 6974 6572 203c 3d20 303a 0a20  max_iter <= 0:. 
+00009900: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00009910: 0a20 2020 2020 2020 2066 6f72 206d 6f64  .        for mod
+00009920: 656c 2069 6e20 6d6f 6465 6c5f 6c69 7374  el in model_list
+00009930: 3a0a 2020 2020 2020 2020 2020 2020 6d73  :.            ms
+00009940: 675f 6275 7273 7428 2720 2020 2073 6f72  g_burst('    sor
+00009950: 7469 6e67 2025 7320 2e2e 2e27 2025 206d  ting %s ...' % m
+00009960: 6f64 656c 290a 2020 2020 2020 2020 2020  odel).          
+00009970: 2020 6966 2027 6c65 7665 6c27 206e 6f74    if 'level' not
+00009980: 2069 6e20 6d6f 6465 6c73 5b6d 6f64 656c   in models[model
+00009990: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+000099a0: 2020 2070 6172 7369 6e67 203d 2054 7275     parsing = Tru
+000099b0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000099c0: 2020 6375 725f 6c65 7665 6c20 3d20 300a    cur_level = 0.
+000099d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099e0: 666f 7220 7375 6220 696e 206d 6f64 656c  for sub in model
+000099f0: 735b 6d6f 6465 6c5d 5b27 6465 7065 6e64  s[model]['depend
+00009a00: 7327 5d3a 0a20 2020 2020 2020 2020 2020  s']:.           
+00009a10: 2020 2020 2020 2020 2069 6620 276c 6576           if 'lev
+00009a20: 656c 2720 696e 206d 6f64 656c 735b 7375  el' in models[su
+00009a30: 625d 3a0a 2020 2020 2020 2020 2020 2020  b]:.            
+00009a40: 2020 2020 2020 2020 2020 2020 6375 725f              cur_
+00009a50: 6c65 7665 6c20 3d20 6d61 7828 6375 725f  level = max(cur_
+00009a60: 6c65 7665 6c2c 206d 6f64 656c 735b 7375  level, models[su
+00009a70: 625d 5b27 6c65 7665 6c27 5d20 2b20 3129  b]['level'] + 1)
+00009a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009a90: 2020 2020 2020 2020 2069 6620 6375 725f           if cur_
+00009aa0: 6c65 7665 6c20 3e20 4d41 585f 4445 4550  level > MAX_DEEP
+00009ab0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009ac0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00009ad0: 725f 6c65 7665 6c20 3d20 4d41 585f 4445  r_level = MAX_DE
+00009ae0: 4550 0a20 2020 2020 2020 2020 2020 2020  EP.             
+00009af0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00009b00: 6f64 656c 735b 6d6f 6465 6c5d 5b27 7374  odels[model]['st
+00009b10: 6174 7573 275d 203d 2027 746f 6f20 6465  atus'] = 'too de
+00009b20: 6570 270a 2020 2020 2020 2020 2020 2020  ep'.            
 00009b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b40: 6669 656c 642e 7265 6c61 7469 6f6e 206e  field.relation n
-00009b50: 6f74 2069 6e20 6d6f 6465 6c73 5b6d 6f64  ot in models[mod
-00009b60: 656c 5d5b 2764 6570 656e 6473 275d 293a  el]['depends']):
-00009b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009b80: 2020 2020 206d 6f64 656c 735b 6d6f 6465       models[mode
-00009b90: 6c5d 5b27 6465 7065 6e64 7327 5d2e 6170  l]['depends'].ap
-00009ba0: 7065 6e64 2866 6965 6c64 2e72 656c 6174  pend(field.relat
-00009bb0: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
-00009bc0: 2020 2020 2020 2020 206c 6576 656c 203d           level =
-00009bd0: 202d 310a 2020 2020 2020 2020 2020 2020   -1.            
-00009be0: 2020 2020 6966 2028 6e6f 7420 6669 656c      if (not fiel
-00009bf0: 642e 7265 7175 6972 6564 2061 6e64 0a20  d.required and. 
-00009c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c10: 2020 2020 2020 2066 6965 6c64 2e72 656c         field.rel
-00009c20: 6174 696f 6e20 6e6f 7420 696e 206d 6f64  ation not in mod
-00009c30: 656c 735b 6d6f 6465 6c5d 5b27 6d61 7964  els[model]['mayd
-00009c40: 6570 656e 6473 275d 293a 0a20 2020 2020  epends']):.     
-00009c50: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00009c60: 6f64 656c 735b 6d6f 6465 6c5d 5b27 6d61  odels[model]['ma
-00009c70: 7964 6570 656e 6473 275d 2e61 7070 656e  ydepends'].appen
-00009c80: 6428 6669 656c 642e 7265 6c61 7469 6f6e  d(field.relation
-00009c90: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00009ca0: 6966 2066 6965 6c64 2e74 7479 7065 203d  if field.ttype =
-00009cb0: 3d20 276f 6e65 326d 616e 7927 2061 6e64  = 'one2many' and
-00009cc0: 2066 6965 6c64 2e72 656c 6174 696f 6e20   field.relation 
-00009cd0: 213d 206d 6f64 656c 3a0a 2020 2020 2020  != model:.      
-00009ce0: 2020 2020 2020 2020 2020 6966 2066 6965            if fie
-00009cf0: 6c64 2e72 656c 6174 696f 6e20 6e6f 7420  ld.relation not 
-00009d00: 696e 206d 6f64 656c 733a 0a20 2020 2020  in models:.     
-00009d10: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00009d20: 6577 5f65 6d70 7479 5f6d 6f64 656c 286d  ew_empty_model(m
-00009d30: 6f64 656c 732c 2066 6965 6c64 2e72 656c  odels, field.rel
-00009d40: 6174 696f 6e29 0a20 2020 2020 2020 2020  ation).         
-00009d50: 2020 2020 2020 2069 6620 2866 6965 6c64         if (field
-00009d60: 2e72 6571 7569 7265 6420 616e 640a 2020  .required and.  
-00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d80: 2020 2020 2020 6d6f 6465 6c20 6e6f 7420        model not 
-00009d90: 696e 206d 6f64 656c 735b 6669 656c 642e  in models[field.
-00009da0: 7265 6c61 7469 6f6e 5d5b 2764 6570 656e  relation]['depen
-00009db0: 6473 275d 293a 0a20 2020 2020 2020 2020  ds']):.         
-00009dc0: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-00009dd0: 735b 6669 656c 642e 7265 6c61 7469 6f6e  s[field.relation
-00009de0: 5d5b 2764 6570 656e 6473 275d 2e61 7070  ]['depends'].app
-00009df0: 656e 6428 6d6f 6465 6c29 0a20 2020 2020  end(model).     
-00009e00: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00009e10: 6576 656c 203d 202d 310a 2020 2020 2020  evel = -1.      
-00009e20: 2020 2020 2020 2020 2020 6966 2028 6e6f            if (no
-00009e30: 7420 6669 656c 642e 7265 7175 6972 6564  t field.required
-00009e40: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-00009e50: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00009e60: 656c 206e 6f74 2069 6e20 6d6f 6465 6c73  el not in models
-00009e70: 5b66 6965 6c64 2e72 656c 6174 696f 6e5d  [field.relation]
-00009e80: 5b27 6d61 7964 6570 656e 6473 275d 293a  ['maydepends']):
-00009e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009ea0: 2020 2020 206d 6f64 656c 735b 6669 656c       models[fiel
-00009eb0: 642e 7265 6c61 7469 6f6e 5d5b 276d 6179  d.relation]['may
-00009ec0: 6465 7065 6e64 7327 5d2e 6170 7065 6e64  depends'].append
-00009ed0: 286d 6f64 656c 290a 2020 2020 2020 2020  (model).        
-00009ee0: 2020 2020 656c 6966 2066 6965 6c64 2e74      elif field.t
-00009ef0: 7479 7065 2069 6e20 276d 616e 7932 6d61  type in 'many2ma
-00009f00: 6e79 2720 616e 6420 6669 656c 642e 7265  ny' and field.re
-00009f10: 6c61 7469 6f6e 2021 3d20 6d6f 6465 6c3a  lation != model:
-00009f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009f30: 2069 6620 6669 656c 642e 7265 6c61 7469   if field.relati
-00009f40: 6f6e 206e 6f74 2069 6e20 6d6f 6465 6c73  on not in models
-00009f50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009f60: 2020 2020 2020 6e65 775f 656d 7074 795f        new_empty_
-00009f70: 6d6f 6465 6c28 6d6f 6465 6c73 2c20 6669  model(models, fi
-00009f80: 656c 642e 7265 6c61 7469 6f6e 290a 2020  eld.relation).  
-00009f90: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00009fa0: 2066 6965 6c64 2e72 656c 6174 696f 6e20   field.relation 
-00009fb0: 6e6f 7420 696e 206d 6f64 656c 735b 6d6f  not in models[mo
-00009fc0: 6465 6c5d 5b27 6d32 6d27 5d3a 0a20 2020  del]['m2m']:.   
-00009fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fe0: 206d 6f64 656c 735b 6d6f 6465 6c5d 5b27   models[model]['
-00009ff0: 6d32 6d27 5d2e 6170 7065 6e64 2866 6965  m2m'].append(fie
-0000a000: 6c64 2e72 656c 6174 696f 6e29 0a20 2020  ld.relation).   
-0000a010: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000a020: 6d6f 6465 6c20 6e6f 7420 696e 206d 6f64  model not in mod
-0000a030: 656c 735b 6669 656c 642e 7265 6c61 7469  els[field.relati
-0000a040: 6f6e 5d5b 276d 326d 275d 3a0a 2020 2020  on]['m2m']:.    
-0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a060: 6d6f 6465 6c73 5b66 6965 6c64 2e72 656c  models[field.rel
-0000a070: 6174 696f 6e5d 5b27 6d32 6d27 5d2e 6170  ation]['m2m'].ap
-0000a080: 7065 6e64 286d 6f64 656c 290a 2020 2020  pend(model).    
-0000a090: 2020 2020 6966 206c 6576 656c 203d 3d20      if level == 
-0000a0a0: 303a 0a20 2020 2020 2020 2020 2020 206d  0:.            m
-0000a0b0: 6f64 656c 735b 6d6f 6465 6c5d 5b27 6c65  odels[model]['le
-0000a0c0: 7665 6c27 5d20 3d20 6c65 7665 6c0a 2020  vel'] = level.  
-0000a0d0: 2020 666f 7220 6d6f 6465 6c20 696e 206d    for model in m
-0000a0e0: 6f64 656c 5f6c 6973 743a 0a20 2020 2020  odel_list:.     
-0000a0f0: 2020 206d 7367 5f62 7572 7374 2827 2020     msg_burst('  
-0000a100: 2020 6372 6f73 7364 6570 2025 7320 2e2e    crossdep %s ..
-0000a110: 2e27 2025 206d 6f64 656c 290a 2020 2020  .' % model).    
-0000a120: 2020 2020 666f 7220 7375 6220 696e 206d      for sub in m
-0000a130: 6f64 656c 735b 6d6f 6465 6c5d 5b27 6465  odels[model]['de
-0000a140: 7065 6e64 7327 5d3a 0a20 2020 2020 2020  pends']:.       
-0000a150: 2020 2020 2069 6620 6d6f 6465 6c20 696e       if model in
-0000a160: 206d 6f64 656c 735b 7375 625d 5b27 6465   models[sub]['de
-0000a170: 7065 6e64 7327 5d3a 0a20 2020 2020 2020  pends']:.       
-0000a180: 2020 2020 2020 2020 206d 6f64 656c 735b           models[
-0000a190: 6d6f 6465 6c5d 5b27 6372 6f73 7364 6570  model]['crossdep
-0000a1a0: 275d 203d 2073 7562 0a20 2020 2020 2020  '] = sub.       
-0000a1b0: 2020 2020 2020 2020 206d 6f64 656c 735b           models[
-0000a1c0: 7375 625d 5b27 6372 6f73 7364 6570 275d  sub]['crossdep']
-0000a1d0: 203d 206d 6f64 656c 0a20 2020 2066 6f72   = model.    for
-0000a1e0: 206d 6f64 656c 2069 6e20 6d6f 6465 6c5f   model in model_
-0000a1f0: 6c69 7374 3a0a 2020 2020 2020 2020 6d73  list:.        ms
-0000a200: 675f 6275 7273 7428 2720 2020 2064 6570  g_burst('    dep
-0000a210: 656e 6465 6e63 6965 7320 2573 202e 2e2e  endencies %s ...
-0000a220: 2720 2520 6d6f 6465 6c29 0a20 2020 2020  ' % model).     
-0000a230: 2020 206d 6f64 656c 735b 6d6f 6465 6c5d     models[model]
-0000a240: 5b27 6465 7065 6e64 7327 5d20 3d20 6c69  ['depends'] = li
-0000a250: 7374 2873 6574 286d 6f64 656c 735b 6d6f  st(set(models[mo
-0000a260: 6465 6c5d 5b27 6465 7065 6e64 7327 5d29  del]['depends'])
-0000a270: 202d 0a20 2020 2020 2020 2020 2020 2020   -.             
-0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 2020 2020 2020 2020 2020 2073 6574 286d             set(m
-0000a2a0: 6f64 656c 735b 6d6f 6465 6c5d 5b27 6372  odels[model]['cr
-0000a2b0: 6f73 7364 6570 275d 2920 290a 2020 2020  ossdep']) ).    
-0000a2c0: 6d69 7373 6564 5f6d 6f64 656c 7320 3d20  missed_models = 
-0000a2d0: 7b7d 0a20 2020 206d 6178 5f69 7465 7220  {}.    max_iter 
-0000a2e0: 3d20 3939 0a20 2020 2070 6172 7369 6e67  = 99.    parsing
-0000a2f0: 203d 2054 7275 650a 2020 2020 7768 696c   = True.    whil
-0000a300: 6520 7061 7273 696e 673a 0a20 2020 2020  e parsing:.     
-0000a310: 2020 2070 6172 7369 6e67 203d 2046 616c     parsing = Fal
-0000a320: 7365 0a20 2020 2020 2020 206d 6178 5f69  se.        max_i
-0000a330: 7465 7220 2d3d 2031 0a20 2020 2020 2020  ter -= 1.       
-0000a340: 2069 6620 6d61 785f 6974 6572 203c 3d20   if max_iter <= 
-0000a350: 303a 0a20 2020 2020 2020 2020 2020 2062  0:.            b
-0000a360: 7265 616b 0a20 2020 2020 2020 2066 6f72  reak.        for
-0000a370: 206d 6f64 656c 2069 6e20 6d6f 6465 6c5f   model in model_
-0000a380: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
-0000a390: 2020 6d73 675f 6275 7273 7428 2720 2020    msg_burst('   
-0000a3a0: 2073 6f72 7469 6e67 2025 7320 2e2e 2e27   sorting %s ...'
-0000a3b0: 2025 206d 6f64 656c 290a 2020 2020 2020   % model).      
-0000a3c0: 2020 2020 2020 6966 2027 6c65 7665 6c27        if 'level'
-0000a3d0: 206e 6f74 2069 6e20 6d6f 6465 6c73 5b6d   not in models[m
-0000a3e0: 6f64 656c 5d3a 0a20 2020 2020 2020 2020  odel]:.         
-0000a3f0: 2020 2020 2020 2070 6172 7369 6e67 203d         parsing =
-0000a400: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-0000a410: 2020 2020 2020 6375 725f 6c65 7665 6c20        cur_level 
-0000a420: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
-0000a430: 2020 2020 666f 7220 7375 6220 696e 206d      for sub in m
-0000a440: 6f64 656c 735b 6d6f 6465 6c5d 5b27 6465  odels[model]['de
-0000a450: 7065 6e64 7327 5d3a 0a20 2020 2020 2020  pends']:.       
-0000a460: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000a470: 276c 6576 656c 2720 696e 206d 6f64 656c  'level' in model
-0000a480: 735b 7375 625d 3a0a 2020 2020 2020 2020  s[sub]:.        
-0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4a0: 6375 725f 6c65 7665 6c20 3d20 6d61 7828  cur_level = max(
-0000a4b0: 6375 725f 6c65 7665 6c2c 206d 6f64 656c  cur_level, model
-0000a4c0: 735b 7375 625d 5b27 6c65 7665 6c27 5d20  s[sub]['level'] 
-0000a4d0: 2b20 3129 0a20 2020 2020 2020 2020 2020  + 1).           
-0000a4e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000a4f0: 6375 725f 6c65 7665 6c20 3e20 4d41 585f  cur_level > MAX_
-0000a500: 4445 4550 3a0a 2020 2020 2020 2020 2020  DEEP:.          
-0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a520: 2020 6375 725f 6c65 7665 6c20 3d20 4d41    cur_level = MA
-0000a530: 585f 4445 4550 0a20 2020 2020 2020 2020  X_DEEP.         
-0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a550: 2020 206d 6f64 656c 735b 6d6f 6465 6c5d     models[model]
-0000a560: 5b27 7374 6174 7573 275d 203d 2027 746f  ['status'] = 'to
-0000a570: 6f20 6465 6570 270a 2020 2020 2020 2020  o deep'.        
-0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a590: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
-0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5d0: 2020 2020 6d6f 6465 6c73 5b6d 6f64 656c      models[model
-0000a5e0: 5d5b 2773 7461 7475 7327 5d20 3d20 274f  ]['status'] = 'O
-0000a5f0: 4b27 0a20 2020 2020 2020 2020 2020 2020  K'.             
-0000a600: 2020 2020 2020 2065 6c69 6620 6d6f 6465         elif mode
-0000a610: 6c20 696e 206d 6f64 656c 735b 7375 625d  l in models[sub]
-0000a620: 5b27 6465 7065 6e64 7327 5d3a 0a20 2020  ['depends']:.   
-0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a640: 2020 2020 206d 6f64 656c 735b 6d6f 6465       models[mode
-0000a650: 6c5d 5b27 7374 6174 7573 275d 203d 2027  l]['status'] = '
-0000a660: 6372 6f73 7320 6465 702e 2077 6974 6820  cross dep. with 
-0000a670: 2573 2720 2520 7375 620a 2020 2020 2020  %s' % sub.      
-0000a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a690: 2020 6d6f 6465 6c73 5b73 7562 5d5b 2773    models[sub]['s
-0000a6a0: 7461 7475 7327 5d20 3d20 2763 726f 7373  tatus'] = 'cross
-0000a6b0: 2064 6570 2e20 7769 7468 2025 7327 2025   dep. with %s' %
-0000a6c0: 206d 6f64 656c 0a20 2020 2020 2020 2020   model.         
-0000a6d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000a6e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a6f0: 2020 2020 2020 2020 2063 7572 5f6c 6576           cur_lev
-0000a700: 656c 203d 202d 310a 2020 2020 2020 2020  el = -1.        
-0000a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a720: 6d6f 6465 6c73 5b6d 6f64 656c 5d5b 2773  models[model]['s
-0000a730: 7461 7475 7327 5d20 3d20 2762 726f 6b65  tatus'] = 'broke
-0000a740: 6e20 6279 2025 7327 2025 2073 7562 0a20  n by %s' % sub. 
-0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a760: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-0000a770: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000a780: 6375 725f 6c65 7665 6c20 3e3d 204d 4158  cur_level >= MAX
-0000a790: 5f44 4545 503a 0a20 2020 2020 2020 2020  _DEEP:.         
-0000a7a0: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-0000a7b0: 735b 6d6f 6465 6c5d 5b27 6c65 7665 6c27  s[model]['level'
-0000a7c0: 5d20 3d20 4d41 585f 4445 4550 0a20 2020  ] = MAX_DEEP.   
-0000a7d0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-0000a7e0: 6620 6375 725f 6c65 7665 6c20 3e3d 2030  f cur_level >= 0
-0000a7f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a800: 2020 2020 2020 6d6f 6465 6c73 5b6d 6f64        models[mod
-0000a810: 656c 5d5b 276c 6576 656c 275d 203d 2063  el]['level'] = c
-0000a820: 7572 5f6c 6576 656c 0a20 2020 2066 6f72  ur_level.    for
-0000a830: 206d 6f64 656c 2069 6e20 6d6f 6465 6c5f   model in model_
-0000a840: 6c69 7374 3a0a 2020 2020 2020 2020 6966  list:.        if
-0000a850: 2027 6c65 7665 6c27 206e 6f74 2069 6e20   'level' not in 
-0000a860: 6d6f 6465 6c73 5b6d 6f64 656c 5d3a 0a20  models[model]:. 
-0000a870: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-0000a880: 735b 6d6f 6465 6c5d 5b27 6c65 7665 6c27  s[model]['level'
-0000a890: 5d20 3d20 4d41 585f 4445 4550 202b 2031  ] = MAX_DEEP + 1
-0000a8a0: 0a20 2020 2072 6574 7572 6e20 6d6f 6465  .    return mode
-0000a8b0: 6c73 0a0a 0a64 6566 2070 7269 6d6b 6579  ls...def primkey
-0000a8c0: 5f74 6162 6c65 2863 7478 2c20 6d6f 6465  _table(ctx, mode
-0000a8d0: 6c29 3a0a 2020 2020 636c 6f64 6f6f 2e67  l):.    clodoo.g
-0000a8e0: 6574 5f6d 6f64 656c 5f73 7472 7563 7475  et_model_structu
-0000a8f0: 7265 280a 2020 2020 2020 2020 6374 782c  re(.        ctx,
-0000a900: 206d 6f64 656c 2c0a 2020 2020 2020 2020   model,.        
-0000a910: 6967 6e6f 7265 3d49 474e 4f52 455f 4649  ignore=IGNORE_FI
-0000a920: 454c 4453 2e67 6574 286d 6f64 656c 2c20  ELDS.get(model, 
-0000a930: 5b5d 2920 2b20 4947 4e4f 5245 5f46 4945  []) + IGNORE_FIE
-0000a940: 4c44 535b 272a 275d 290a 2020 2020 6972  LDS['*']).    ir
-0000a950: 5f6d 6f64 656c 203d 2027 6972 2e6d 6f64  _model = 'ir.mod
-0000a960: 656c 2e63 6f6e 7374 7261 696e 7427 0a20  el.constraint'. 
-0000a970: 2020 2069 6620 6d6f 6465 6c20 696e 2050     if model in P
-0000a980: 4b45 5953 3a0a 2020 2020 2020 2020 6e61  KEYS:.        na
-0000a990: 6d65 7320 3d20 504b 4559 535b 6d6f 6465  mes = PKEYS[mode
-0000a9a0: 6c5d 0a20 2020 2065 6c73 653a 0a20 2020  l].    else:.   
-0000a9b0: 2020 2020 206e 616d 6573 203d 205b 5d0a       names = [].
-0000a9c0: 2020 2020 2020 2020 7072 696f 725f 6e61          prior_na
-0000a9d0: 6d65 203d 2027 270a 2020 2020 2020 2020  me = ''.        
-0000a9e0: 666f 7220 7265 6320 696e 2063 6c6f 646f  for rec in clodo
-0000a9f0: 6f2e 6272 6f77 7365 4c38 2863 7478 2c20  o.browseL8(ctx, 
-0000aa00: 6972 5f6d 6f64 656c 2c0a 2020 2020 2020  ir_model,.      
-0000aa10: 2020 2020 2020 636c 6f64 6f6f 2e73 6561        clodoo.sea
-0000aa20: 7263 684c 3828 6374 782c 2069 725f 6d6f  rchL8(ctx, ir_mo
-0000aa30: 6465 6c2c 0a20 2020 2020 2020 2020 2020  del,.           
-0000aa40: 2020 2020 205b 2827 6d6f 6465 6c27 2c20       [('model', 
-0000aa50: 273d 272c 206d 6f64 656c 292c 2028 2774  '=', model), ('t
-0000aa60: 7970 6527 2c20 273d 272c 2027 7527 295d  ype', '=', 'u')]
-0000aa70: 2c20 6f72 6465 723d 276e 616d 6527 2929  , order='name'))
-0000aa80: 3a0a 2020 2020 2020 2020 2020 2020 6e61  :.            na
-0000aa90: 6d65 203d 2072 6563 2e6e 616d 650a 2020  me = rec.name.  
-0000aaa0: 2020 2020 2020 2020 2020 6966 206e 616d            if nam
-0000aab0: 6520 3d3d 2070 7269 6f72 5f6e 616d 653a  e == prior_name:
-0000aac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000aad0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-0000aae0: 2020 2020 2020 7072 696f 725f 6e61 6d65        prior_name
-0000aaf0: 203d 206e 616d 650a 2020 2020 2020 2020   = name.        
-0000ab00: 2020 2020 6966 2072 6563 2e6e 616d 652e      if rec.name.
-0000ab10: 7374 6172 7473 7769 7468 286d 6f64 656c  startswith(model
-0000ab20: 2e72 6570 6c61 6365 2827 2e27 2c20 275f  .replace('.', '_
-0000ab30: 2729 293a 0a20 2020 2020 2020 2020 2020  ')):.           
-0000ab40: 2020 2020 206e 616d 6520 3d20 7265 632e       name = rec.
-0000ab50: 6e61 6d65 5b6c 656e 286d 6f64 656c 2920  name[len(model) 
-0000ab60: 2b20 313a 5d0a 2020 2020 2020 2020 2020  + 1:].          
-0000ab70: 2020 2020 2020 746f 6b5f 6964 203d 2027        tok_id = '
-0000ab80: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-0000ab90: 2020 666f 7220 746f 6b20 696e 206e 616d    for tok in nam
-0000aba0: 652e 7370 6c69 7428 275f 2729 3a0a 2020  e.split('_'):.  
-0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abc0: 2020 6966 2074 6f6b 203d 3d20 2769 6427    if tok == 'id'
-0000abd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000abe0: 2020 2020 2020 2020 2020 746f 6b5f 6964            tok_id
-0000abf0: 202b 3d20 275f 6964 270a 2020 2020 2020   += '_id'.      
-0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac10: 2020 6966 2074 6f6b 5f69 6420 696e 2063    if tok_id in c
-0000ac20: 7478 5b27 5354 5255 4354 275d 5b6d 6f64  tx['STRUCT'][mod
-0000ac30: 656c 5d3a 0a20 2020 2020 2020 2020 2020  el]:.           
-0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac50: 206e 616d 6573 2e61 7070 656e 6428 746f   names.append(to
-0000ac60: 6b5f 6964 290a 2020 2020 2020 2020 2020  k_id).          
-0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac80: 2020 746f 6b5f 6964 203d 2027 270a 2020    tok_id = ''.  
-0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aca0: 2020 656c 6966 2074 6f6b 2069 6e20 6374    elif tok in ct
-0000acb0: 785b 2753 5452 5543 5427 5d5b 6d6f 6465  x['STRUCT'][mode
-0000acc0: 6c5d 3a0a 2020 2020 2020 2020 2020 2020  l]:.            
-0000acd0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-0000ace0: 732e 6170 7065 6e64 2874 6f6b 290a 2020  s.append(tok).  
-0000acf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad00: 2020 2020 2020 746f 6b5f 6964 203d 2027        tok_id = '
-0000ad10: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-0000ad20: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad40: 2020 2020 746f 6b5f 6964 203d 2074 6f6b      tok_id = tok
-0000ad50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ad60: 206e 616d 6573 203d 2028 6e61 6d65 7329   names = (names)
-0000ad70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ad80: 2062 7265 616b 0a20 2020 2069 6620 6e6f   break.    if no
-0000ad90: 7420 6e61 6d65 733a 0a20 2020 2020 2020  t names:.       
-0000ada0: 2069 6620 636c 6f64 6f6f 2e69 735f 7661   if clodoo.is_va
-0000adb0: 6c69 645f 6669 656c 6428 6374 782c 206d  lid_field(ctx, m
-0000adc0: 6f64 656c 2c20 2763 6f6d 7061 6e79 5f69  odel, 'company_i
-0000add0: 6427 293a 0a20 2020 2020 2020 2020 2020  d'):.           
-0000ade0: 206e 616d 6573 203d 205b 2763 6f6d 7061   names = ['compa
-0000adf0: 6e79 5f69 6427 5d0a 2020 2020 2020 2020  ny_id'].        
-0000ae00: 6966 2063 6c6f 646f 6f2e 6973 5f76 616c  if clodoo.is_val
-0000ae10: 6964 5f66 6965 6c64 2863 7478 2c20 6d6f  id_field(ctx, mo
-0000ae20: 6465 6c2c 2027 636f 6465 2729 3a0a 2020  del, 'code'):.  
-0000ae30: 2020 2020 2020 2020 2020 6e61 6d65 732e            names.
-0000ae40: 6170 7065 6e64 2827 636f 6465 2729 0a20  append('code'). 
-0000ae50: 2020 2020 2020 2065 6c69 6620 636c 6f64         elif clod
-0000ae60: 6f6f 2e69 735f 7661 6c69 645f 6669 656c  oo.is_valid_fiel
-0000ae70: 6428 6374 782c 206d 6f64 656c 2c20 276e  d(ctx, model, 'n
-0000ae80: 616d 6527 293a 0a20 2020 2020 2020 2020  ame'):.         
-0000ae90: 2020 206e 616d 6573 2e61 7070 656e 6428     names.append(
-0000aea0: 276e 616d 6527 290a 2020 2020 2020 2020  'name').        
-0000aeb0: 6e61 6d65 7320 3d20 286e 616d 6573 290a  names = (names).
-0000aec0: 2020 2020 7265 7475 726e 206e 616d 6573      return names
-0000aed0: 0a0a 0a64 6566 2077 7269 7465 5f74 7265  ...def write_tre
-0000aee0: 655f 636f 6e66 2863 7478 293a 0a20 2020  e_conf(ctx):.   
-0000aef0: 2070 7269 6e74 2827 416e 616c 697a 696e   print('Analizin
-0000af00: 6720 736f 7572 6365 206d 6f64 656c 7320  g source models 
-0000af10: 2e2e 2e27 290a 2020 2020 6d6f 6465 6c73  ...').    models
-0000af20: 203d 2062 7569 6c64 5f74 6162 6c65 5f74   = build_table_t
-0000af30: 7265 6528 6374 7829 0a20 2020 2077 6974  ree(ctx).    wit
-0000af40: 6820 6f70 656e 2863 7478 5b27 636f 6d6d  h open(ctx['comm
-0000af50: 616e 645f 6669 6c65 275d 2c20 2777 2729  and_file'], 'w')
-0000af60: 2061 7320 6664 3a0a 2020 2020 2020 2020   as fd:.        
-0000af70: 666f 7220 6c65 7665 6c20 696e 2072 616e  for level in ran
-0000af80: 6765 284d 4158 5f44 4545 5029 3a0a 2020  ge(MAX_DEEP):.  
-0000af90: 2020 2020 2020 2020 2020 666f 7220 6d6f            for mo
-0000afa0: 6465 6c20 696e 206d 6f64 656c 733a 0a20  del in models:. 
-0000afb0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000afc0: 7367 5f62 7572 7374 2827 2020 2020 6b65  sg_burst('    ke
-0000afd0: 7973 2025 7320 2e2e 2e27 2025 206d 6f64  ys %s ...' % mod
-0000afe0: 656c 290a 2020 2020 2020 2020 2020 2020  el).            
-0000aff0: 2020 2020 6e61 6d65 7320 3d20 7072 696d      names = prim
-0000b000: 6b65 795f 7461 626c 6528 6374 782c 206d  key_table(ctx, m
-0000b010: 6f64 656c 290a 2020 2020 2020 2020 2020  odel).          
-0000b020: 2020 2020 2020 6966 206d 6f64 656c 735b        if models[
-0000b030: 6d6f 6465 6c5d 2e67 6574 2827 6c65 7665  model].get('leve
-0000b040: 6c27 2c20 2d31 2920 3d3d 206c 6576 656c  l', -1) == level
-0000b050: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b060: 2020 2020 2020 6664 2e77 7269 7465 2827        fd.write('
-0000b070: 2564 5c74 2573 5c74 696e 7175 6972 655c  %d\t%s\tinquire\
-0000b080: 7425 735c 6e27 2025 2028 6c65 7665 6c2c  t%s\n' % (level,
-0000b090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0c0: 2020 2020 2020 2020 206d 6f64 656c 2c0a           model,.
-0000b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b100: 2020 2020 2020 2020 6e61 6d65 7329 290a          names)).
-0000b110: 2020 2020 2020 2020 666f 7220 6d6f 6465          for mode
-0000b120: 6c20 696e 206d 6f64 656c 733a 0a20 2020  l in models:.   
-0000b130: 2020 2020 2020 2020 206d 7367 5f62 7572           msg_bur
-0000b140: 7374 2827 2020 2020 6b65 7973 2025 7320  st('    keys %s 
-0000b150: 2e2e 2e27 2025 206d 6f64 656c 290a 2020  ...' % model).  
-0000b160: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-0000b170: 656c 735b 6d6f 6465 6c5d 2e67 6574 2827  els[model].get('
-0000b180: 6c65 7665 6c27 2c20 2d31 2920 3e3d 204d  level', -1) >= M
-0000b190: 4158 5f44 4545 503a 0a20 2020 2020 2020  AX_DEEP:.       
-0000b1a0: 2020 2020 2020 2020 206e 616d 6573 203d           names =
-0000b1b0: 2070 7269 6d6b 6579 5f74 6162 6c65 2863   primkey_table(c
-0000b1c0: 7478 2c20 6d6f 6465 6c29 0a20 2020 2020  tx, model).     
-0000b1d0: 2020 2020 2020 2020 2020 2066 642e 7772             fd.wr
-0000b1e0: 6974 6528 2725 645c 7425 735c 7469 6e71  ite('%d\t%s\tinq
-0000b1f0: 7569 7265 5c74 2573 5c6e 2720 2520 286c  uire\t%s\n' % (l
-0000b200: 6576 656c 2c0a 2020 2020 2020 2020 2020  evel,.          
-0000b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b230: 2020 2020 2020 2020 2020 6d6f 6465 6c2c            model,
-0000b240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b270: 2020 2020 206e 616d 6573 2929 0a0a 0a64       names))...d
-0000b280: 6566 2067 6574 5f6d 6f64 656c 5f63 6f70  ef get_model_cop
-0000b290: 795f 6d6f 6465 2863 7478 2c20 6d6f 6465  y_mode(ctx, mode
-0000b2a0: 6c29 3a0a 2020 2020 6966 2069 735f 7379  l):.    if is_sy
-0000b2b0: 7374 656d 5f6d 6f64 656c 286d 6f64 656c  stem_model(model
-0000b2c0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-0000b2d0: 6e20 274e 6f27 0a20 2020 206d 6f64 6520  n 'No'.    mode 
-0000b2e0: 3d20 6374 785b 275f 6d6c 275d 2e67 6574  = ctx['_ml'].get
-0000b2f0: 286d 6f64 656c 2920 6f72 2027 696e 7175  (model) or 'inqu
-0000b300: 6972 6527 0a20 2020 2069 6620 6374 785b  ire'.    if ctx[
-0000b310: 2769 6d61 6765 5f6d 6f64 6527 5d3a 0a20  'image_mode']:. 
-0000b320: 2020 2020 2020 206d 6f64 6520 3d20 2769         mode = 'i
-0000b330: 6d61 6765 270a 2020 2020 656c 6966 206d  mage'.    elif m
-0000b340: 6f64 656c 2069 6e20 2827 6163 636f 756e  odel in ('accoun
-0000b350: 742e 6163 636f 756e 7427 2c0a 2020 2020  t.account',.    
-0000b360: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000b370: 6163 636f 756e 742e 6163 636f 756e 742e  account.account.
-0000b380: 7479 7065 272c 0a20 2020 2020 2020 2020  type',.         
-0000b390: 2020 2020 2020 2020 2020 2761 6363 6f75            'accou
-0000b3a0: 6e74 2e74 6178 272c 0a20 2020 2020 2020  nt.tax',.       
-0000b3b0: 2020 2020 2020 2020 2020 2020 2770 726f              'pro
-0000b3c0: 6475 6374 2e70 726f 6475 6374 272c 0a20  duct.product',. 
-0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3e0: 2020 2770 726f 6475 6374 2e74 656d 706c    'product.templ
-0000b3f0: 6174 6527 2c0a 2020 2020 2020 2020 2020  ate',.          
-0000b400: 2020 2020 2020 2020 2027 7265 732e 7061           'res.pa
-0000b410: 7274 6e65 7227 293a 0a20 2020 2020 2020  rtner'):.       
-0000b420: 206d 6f64 6520 3d20 2773 716c 270a 2020   mode = 'sql'.  
-0000b430: 2020 6966 206d 6f64 6520 3d3d 2027 696e    if mode == 'in
-0000b440: 7175 6972 6527 3a0a 2020 2020 2020 2020  quire':.        
-0000b450: 6d6f 6465 5f73 656c 6563 7469 6f6e 203d  mode_selection =
-0000b460: 207b 2769 273a 2027 696d 6167 6527 2c20   {'i': 'image', 
-0000b470: 2773 273a 2027 7371 6c27 2c20 276e 273a  's': 'sql', 'n':
-0000b480: 2027 6e6f 277d 0a20 2020 2020 2020 2064   'no'}.        d
-0000b490: 756d 6d79 203d 2027 270a 2020 2020 2020  ummy = ''.      
-0000b4a0: 2020 7768 696c 6520 6e6f 7420 6475 6d6d    while not dumm
-0000b4b0: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
-0000b4c0: 6620 6374 785b 2773 656c 5f6d 6f64 656c  f ctx['sel_model
-0000b4d0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
-0000b4e0: 2020 2020 6966 206d 6f64 656c 2069 6e20      if model in 
-0000b4f0: 6374 785b 2773 656c 5f6d 6f64 656c 275d  ctx['sel_model']
-0000b500: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b510: 2020 2020 2020 6475 6d6d 7920 3d20 2753        dummy = 'S
-0000b520: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-0000b530: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000b540: 2020 2020 2020 2020 2020 2020 6475 6d6d              dumm
-0000b550: 7920 3d20 274e 270a 2020 2020 2020 2020  y = 'N'.        
-0000b560: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000b570: 2020 2020 2020 2020 2020 6475 6d6d 7920            dummy 
-0000b580: 3d20 696e 7075 7428 2743 6f70 7920 7461  = input('Copy ta
-0000b590: 626c 6520 2573 2028 496d 6167 652c 5371  ble %s (Image,Sq
-0000b5a0: 6c2c 4e6f 293f 2027 2025 206d 6f64 656c  l,No)? ' % model
-0000b5b0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000b5c0: 2064 756d 6d79 2061 6e64 2064 756d 6d79   dummy and dummy
-0000b5d0: 5b30 5d2e 6c6f 7765 7228 2920 696e 206d  [0].lower() in m
-0000b5e0: 6f64 655f 7365 6c65 6374 696f 6e3a 0a20  ode_selection:. 
-0000b5f0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000b600: 6f64 6520 3d20 6d6f 6465 5f73 656c 6563  ode = mode_selec
-0000b610: 7469 6f6e 5b64 756d 6d79 5b30 5d2e 6c6f  tion[dummy[0].lo
-0000b620: 7765 7228 295d 0a20 2020 2020 2020 2020  wer()].         
-0000b630: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000b640: 2020 2020 2020 2020 2064 756d 6d79 203d           dummy =
-0000b650: 2027 270a 2020 2020 2020 2020 6374 785b   ''.        ctx[
-0000b660: 275f 6d6c 275d 5b6d 6f64 656c 5d20 3d20  '_ml'][model] = 
-0000b670: 6d6f 6465 0a20 2020 2072 6574 7572 6e20  mode.    return 
-0000b680: 6d6f 6465 0a0a 0a64 6566 206d 6967 7261  mode...def migra
-0000b690: 7465 5f73 656c 5f74 6162 6c65 7328 7372  te_sel_tables(sr
-0000b6a0: 635f 6374 782c 2074 6774 5f63 7478 293a  c_ctx, tgt_ctx):
-0000b6b0: 0a20 2020 2073 7263 5f63 7478 203d 2069  .    src_ctx = i
-0000b6c0: 6e69 745f 6374 7828 7372 635f 6374 7829  nit_ctx(src_ctx)
-0000b6d0: 0a20 2020 2069 6d70 6f72 7420 7064 620a  .    import pdb.
-0000b6e0: 2020 2020 7064 622e 7365 745f 7472 6163      pdb.set_trac
-0000b6f0: 6528 290a 2020 2020 7372 635f 6374 782c  e().    src_ctx,
-0000b700: 2074 6774 5f63 7478 2c20 7372 635f 636f   tgt_ctx, src_co
-0000b710: 6e66 6967 2c20 7467 745f 636f 6e66 6967  nfig, tgt_config
-0000b720: 203d 2061 646a 7573 745f 6374 7828 7372   = adjust_ctx(sr
-0000b730: 635f 6374 782c 2074 6774 5f63 7478 290a  c_ctx, tgt_ctx).
-0000b740: 2020 2020 7569 642c 2073 7263 5f63 7478      uid, src_ctx
-0000b750: 203d 2063 6c6f 646f 6f2e 6f65 7270 5f73   = clodoo.oerp_s
-0000b760: 6574 5f65 6e76 2863 7478 3d73 7263 5f63  et_env(ctx=src_c
-0000b770: 7478 290a 2020 2020 2320 4649 5820 6f65  tx).    # FIX oe
-0000b780: 7270 5f73 6574 5f65 6e76 2063 6861 6e67  rp_set_env chang
-0000b790: 6520 6472 795f 7275 6e0a 2020 2020 7372  e dry_run.    sr
-0000b7a0: 635f 6374 785b 2764 7279 5f72 756e 275d  c_ctx['dry_run']
-0000b7b0: 203d 2074 6774 5f63 7478 5b27 6472 795f   = tgt_ctx['dry_
-0000b7c0: 7275 6e27 5d0a 2020 2020 7569 642c 2074  run'].    uid, t
-0000b7d0: 6774 5f63 7478 203d 2063 6c6f 646f 6f2e  gt_ctx = clodoo.
-0000b7e0: 6f65 7270 5f73 6574 5f65 6e76 2863 7478  oerp_set_env(ctx
-0000b7f0: 3d74 6774 5f63 7478 290a 2020 2020 2320  =tgt_ctx).    # 
-0000b800: 4649 5820 6f65 7270 5f73 6574 5f65 6e76  FIX oerp_set_env
-0000b810: 2063 6861 6e67 6520 6472 795f 7275 6e0a   change dry_run.
-0000b820: 2020 2020 7467 745f 6374 785b 2764 7279      tgt_ctx['dry
-0000b830: 5f72 756e 275d 203d 2073 7263 5f63 7478  _run'] = src_ctx
-0000b840: 5b27 6472 795f 7275 6e27 5d0a 2020 2020  ['dry_run'].    
-0000b850: 7472 616e 736f 646f 6f2e 7265 6164 5f73  transodoo.read_s
-0000b860: 746f 7265 645f 6469 6374 2873 7263 5f63  tored_dict(src_c
-0000b870: 7478 290a 2020 2020 7467 745f 6374 785b  tx).    tgt_ctx[
-0000b880: 276d 696e 6472 6f6f 7427 5d20 3d20 7372  'mindroot'] = sr
-0000b890: 635f 6374 785b 276d 696e 6472 6f6f 7427  c_ctx['mindroot'
-0000b8a0: 5d0a 2020 2020 6966 206e 6f74 2074 6774  ].    if not tgt
-0000b8b0: 5f63 7478 5b27 7365 6c5f 6d6f 6465 6c27  _ctx['sel_model'
-0000b8c0: 5d3a 0a20 2020 2020 2020 2069 6e73 7461  ]:.        insta
-0000b8d0: 6c6c 5f6d 6f64 756c 6573 2874 6774 5f63  ll_modules(tgt_c
-0000b8e0: 7478 2c20 7372 635f 6374 7829 0a0a 2020  tx, src_ctx)..  
-0000b8f0: 2020 6966 2028 7372 635f 6374 785b 2764    if (src_ctx['d
-0000b900: 6566 6175 6c74 5f62 6568 6176 696f 7227  efault_behavior'
-0000b910: 5d20 6f72 0a20 2020 2020 2020 2020 2020  ] or.           
-0000b920: 206e 6f74 206f 732e 7061 7468 2e69 7366   not os.path.isf
-0000b930: 696c 6528 7372 635f 6374 785b 2763 6f6d  ile(src_ctx['com
-0000b940: 6d61 6e64 5f66 696c 6527 5d29 293a 0a20  mand_file'])):. 
-0000b950: 2020 2020 2020 2077 7269 7465 5f74 7265         write_tre
-0000b960: 655f 636f 6e66 2873 7263 5f63 7478 290a  e_conf(src_ctx).
-0000b970: 0a20 2020 2077 6974 6820 6f70 656e 2874  .    with open(t
-0000b980: 6774 5f63 7478 5b27 636f 6d6d 616e 645f  gt_ctx['command_
-0000b990: 6669 6c65 275d 2c20 2772 2729 2061 7320  file'], 'r') as 
-0000b9a0: 6664 3a0a 2020 2020 2020 2020 7467 745f  fd:.        tgt_
-0000b9b0: 6374 785b 275f 6d6c 275d 203d 207b 7d0a  ctx['_ml'] = {}.
-0000b9c0: 2020 2020 2020 2020 7467 745f 6374 785b          tgt_ctx[
-0000b9d0: 275f 6b6c 275d 203d 207b 7d0a 2020 2020  '_kl'] = {}.    
-0000b9e0: 2020 2020 7467 745f 6374 785b 276d 6f64      tgt_ctx['mod
-0000b9f0: 656c 5f6c 6973 7427 5d20 3d20 5b5d 0a20  el_list'] = []. 
-0000ba00: 2020 2020 2020 2066 6f72 206c 696e 6520         for line 
-0000ba10: 696e 2066 642e 7265 6164 2829 2e73 706c  in fd.read().spl
-0000ba20: 6974 2827 5c6e 2729 3a0a 2020 2020 2020  it('\n'):.      
-0000ba30: 2020 2020 2020 6c69 6e65 203d 206c 696e        line = lin
-0000ba40: 652e 7374 7269 7028 290a 2020 2020 2020  e.strip().      
-0000ba50: 2020 2020 2020 6966 206c 696e 653a 0a20        if line:. 
-0000ba60: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000ba70: 696e 6573 203d 206c 696e 652e 7370 6c69  ines = line.spli
-0000ba80: 7428 275c 7427 290a 2020 2020 2020 2020  t('\t').        
-0000ba90: 2020 2020 2020 2020 6c65 7665 6c20 3d20          level = 
-0000baa0: 6c69 6e65 735b 305d 0a20 2020 2020 2020  lines[0].       
-0000bab0: 2020 2020 2020 2020 206d 6f64 656c 203d           model =
-0000bac0: 206c 696e 6573 5b31 5d0a 2020 2020 2020   lines[1].      
-0000bad0: 2020 2020 2020 2020 2020 6d6f 6465 203d            mode =
-0000bae0: 2027 696e 7175 6972 6527 2069 6620 6c65   'inquire' if le
-0000baf0: 6e28 6c69 6e65 735b 315d 2920 3c3d 2032  n(lines[1]) <= 2
-0000bb00: 2065 6c73 6520 6c69 6e65 735b 325d 0a20   else lines[2]. 
-0000bb10: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-0000bb20: 6579 7320 3d20 276e 616d 6527 2069 6620  eys = 'name' if 
-0000bb30: 6c65 6e28 6c69 6e65 7329 203c 3d20 3320  len(lines) <= 3 
-0000bb40: 656c 7365 2065 7661 6c28 6c69 6e65 735b  else eval(lines[
-0000bb50: 335d 290a 2020 2020 2020 2020 2020 2020  3]).            
-0000bb60: 2020 2020 7467 745f 6374 785b 276d 6f64      tgt_ctx['mod
-0000bb70: 656c 5f6c 6973 7427 5d2e 6170 7065 6e64  el_list'].append
-0000bb80: 286d 6f64 656c 290a 2020 2020 2020 2020  (model).        
-0000bb90: 2020 2020 2020 2020 7467 745f 6374 785b          tgt_ctx[
-0000bba0: 275f 6d6c 275d 5b6d 6f64 656c 5d20 3d20  '_ml'][model] = 
-0000bbb0: 6d6f 6465 0a20 2020 2020 2020 2020 2020  mode.           
-0000bbc0: 2020 2020 2069 6620 6d6f 6465 6c20 696e       if model in
-0000bbd0: 2050 4b45 5953 3a0a 2020 2020 2020 2020   PKEYS:.        
-0000bbe0: 2020 2020 2020 2020 2020 2020 7467 745f              tgt_
-0000bbf0: 6374 785b 275f 6b6c 275d 5b6d 6f64 656c  ctx['_kl'][model
-0000bc00: 5d20 3d20 504b 4559 535b 6d6f 6465 6c5d  ] = PKEYS[model]
-0000bc10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bc20: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000bc30: 2020 2020 2020 2020 2020 2074 6774 5f63             tgt_c
-0000bc40: 7478 5b27 5f6b 6c27 5d5b 6d6f 6465 6c5d  tx['_kl'][model]
-0000bc50: 203d 206b 6579 730a 2020 2020 2020 2020   = keys.        
-0000bc60: 6664 2e63 6c6f 7365 2829 0a20 2020 2061  fd.close().    a
-0000bc70: 7373 756d 655f 7965 7320 3d20 2759 2720  ssume_yes = 'Y' 
-0000bc80: 6966 2074 6774 5f63 7478 5b27 6173 7375  if tgt_ctx['assu
-0000bc90: 6d65 5f79 6573 275d 2065 6c73 6520 2751  me_yes'] else 'Q
-0000bca0: 270a 2020 2020 6966 2074 6774 5f63 7478  '.    if tgt_ctx
-0000bcb0: 5b27 7365 6c5f 6d6f 6465 6c27 5d3a 0a20  ['sel_model']:. 
-0000bcc0: 2020 2020 2020 2074 6774 5f63 7478 5b27         tgt_ctx['
-0000bcd0: 6d6f 6465 6c5f 6c69 7374 275d 203d 2074  model_list'] = t
-0000bce0: 6774 5f63 7478 5b27 7365 6c5f 6d6f 6465  gt_ctx['sel_mode
-0000bcf0: 6c27 5d2e 7370 6c69 7428 272c 2729 0a20  l'].split(','). 
-0000bd00: 2020 2066 6f72 206d 6f64 656c 2069 6e20     for model in 
-0000bd10: 7467 745f 6374 785b 276d 6f64 656c 5f6c  tgt_ctx['model_l
-0000bd20: 6973 7427 5d3a 0a20 2020 2020 2020 206d  ist']:.        m
-0000bd30: 6f64 6520 3d20 6765 745f 6d6f 6465 6c5f  ode = get_model_
-0000bd40: 636f 7079 5f6d 6f64 6528 7467 745f 6374  copy_mode(tgt_ct
-0000bd50: 782c 206d 6f64 656c 290a 2020 2020 2020  x, model).      
-0000bd60: 2020 6966 206d 6f64 6520 6e6f 7420 696e    if mode not in
-0000bd70: 2028 2773 716c 272c 2027 696d 6167 6527   ('sql', 'image'
-0000bd80: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
-0000bd90: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-0000bda0: 636f 7079 5f74 6162 6c65 2874 6774 5f63  copy_table(tgt_c
-0000bdb0: 7478 2c20 7372 635f 6374 782c 206d 6f64  tx, src_ctx, mod
-0000bdc0: 656c 2c20 6d6f 6465 3d6d 6f64 6529 0a0a  el, mode=mode)..
-0000bdd0: 0a64 6566 2069 6e69 745f 6374 7828 7372  .def init_ctx(sr
-0000bde0: 635f 6374 7829 3a0a 2020 2020 7372 635f  c_ctx):.    src_
-0000bdf0: 6374 785b 2773 7263 5f76 6964 275d 203d  ctx['src_vid'] =
-0000be00: 2073 7263 5f63 7478 5b27 6672 6f6d 5f62   src_ctx['from_b
-0000be10: 7261 6e63 6827 5d0a 2020 2020 7372 635f  ranch'].    src_
-0000be20: 6374 785b 2773 7263 5f6f 646f 6f5f 6676  ctx['src_odoo_fv
-0000be30: 6572 275d 203d 2063 6c6f 646f 6f2e 6275  er'] = clodoo.bu
-0000be40: 696c 645f 6f64 6f6f 5f70 6172 616d 280a  ild_odoo_param(.
-0000be50: 2020 2020 2020 2020 2020 2020 2746 554c              'FUL
-0000be60: 4c56 4552 272c 206f 646f 6f5f 7669 643d  LVER', odoo_vid=
-0000be70: 7372 635f 6374 785b 2766 726f 6d5f 6272  src_ctx['from_br
-0000be80: 616e 6368 275d 2c20 6d75 6c74 693d 5472  anch'], multi=Tr
-0000be90: 7565 290a 2020 2020 7372 635f 6374 785b  ue).    src_ctx[
-0000bea0: 2766 726f 6d5f 6f64 6f6f 5f66 7665 7227  'from_odoo_fver'
-0000beb0: 5d20 3d20 7372 635f 6374 785b 2773 7263  ] = src_ctx['src
-0000bec0: 5f6f 646f 6f5f 6676 6572 275d 0a20 2020  _odoo_fver'].   
-0000bed0: 2073 7263 5f63 7478 5b27 7372 635f 6f64   src_ctx['src_od
-0000bee0: 6f6f 5f76 6572 275d 203d 2063 6c6f 646f  oo_ver'] = clodo
-0000bef0: 6f2e 6275 696c 645f 6f64 6f6f 5f70 6172  o.build_odoo_par
-0000bf00: 616d 280a 2020 2020 2020 2020 2020 2020  am(.            
-0000bf10: 274d 414a 5645 5227 2c20 6f64 6f6f 5f76  'MAJVER', odoo_v
-0000bf20: 6964 3d73 7263 5f63 7478 5b27 6672 6f6d  id=src_ctx['from
-0000bf30: 5f62 7261 6e63 6827 5d2c 206d 756c 7469  _branch'], multi
-0000bf40: 3d54 7275 6529 0a20 2020 2073 7263 5f63  =True).    src_c
-0000bf50: 7478 5b27 7372 635f 636f 6e66 5f66 6e27  tx['src_conf_fn'
-0000bf60: 5d20 3d20 7372 635f 6374 785b 2766 726f  ] = src_ctx['fro
-0000bf70: 6d5f 636f 6e66 6e27 5d0a 2020 2020 7372  m_confn'].    sr
-0000bf80: 635f 6374 785b 2773 7263 5f64 625f 6e61  c_ctx['src_db_na
-0000bf90: 6d65 275d 203d 2073 7263 5f63 7478 5b27  me'] = src_ctx['
-0000bfa0: 6672 6f6d 5f64 626e 616d 6527 5d0a 2020  from_dbname'].  
-0000bfb0: 2020 7265 7475 726e 2073 7263 5f63 7478    return src_ctx
-0000bfc0: 0a0a 0a64 6566 2067 6574 5f63 6f6e 6669  ...def get_confi
-0000bfd0: 675f 666e 7328 6374 782c 2073 7263 5f74  g_fns(ctx, src_t
-0000bfe0: 6774 293a 0a20 2020 2069 6620 7372 635f  gt):.    if src_
-0000bff0: 7467 7420 6e6f 7420 696e 2028 2773 7263  tgt not in ('src
-0000c000: 272c 2027 7467 7427 293a 0a20 2020 2020  ', 'tgt'):.     
-0000c010: 2020 2072 6169 7365 2827 496e 7661 6c69     raise('Invali
-0000c020: 6420 7061 7261 6d65 7465 7220 7372 632f  d parameter src/
-0000c030: 7467 7427 290a 2020 2020 6974 656d 203d  tgt').    item =
-0000c040: 2027 636f 6e66 5f66 6e27 0a20 2020 206f   'conf_fn'.    o
-0000c050: 646f 6f5f 636f 6e66 6e20 3d20 636c 6f64  doo_confn = clod
-0000c060: 6f6f 2e62 7569 6c64 5f6f 646f 6f5f 7061  oo.build_odoo_pa
-0000c070: 7261 6d28 0a20 2020 2020 2020 2027 434f  ram(.        'CO
-0000c080: 4e46 4e27 2c20 6f64 6f6f 5f76 6964 3d63  NFN', odoo_vid=c
-0000c090: 7478 5b27 2573 5f76 6964 2720 2520 7372  tx['%s_vid' % sr
-0000c0a0: 635f 7467 745d 2c20 6d75 6c74 693d 5472  c_tgt], multi=Tr
-0000c0b0: 7565 290a 2020 2020 6966 2073 7263 5f74  ue).    if src_t
-0000c0c0: 6774 203d 3d20 2773 7263 2720 616e 6420  gt == 'src' and 
-0000c0d0: 6374 785b 2725 735f 7669 6427 2025 2073  ctx['%s_vid' % s
-0000c0e0: 7263 5f74 6774 5d20 3d3d 2063 7478 5b27  rc_tgt] == ctx['
-0000c0f0: 6672 6f6d 5f62 7261 6e63 6827 5d3a 0a20  from_branch']:. 
-0000c100: 2020 2020 2020 2063 7478 5b69 7465 6d5d         ctx[item]
-0000c110: 203d 2063 7478 5b27 7372 635f 2573 2720   = ctx['src_%s' 
-0000c120: 2520 6974 656d 5d0a 2020 2020 2020 2020  % item].        
-0000c130: 6966 206e 6f74 206f 732e 7061 7468 2e69  if not os.path.i
-0000c140: 7366 696c 6528 6f64 6f6f 5f63 6f6e 666e  sfile(odoo_confn
-0000c150: 293a 0a20 2020 2020 2020 2020 2020 206f  ):.            o
-0000c160: 646f 6f5f 636f 6e66 6e20 3d20 4661 6c73  doo_confn = Fals
-0000c170: 650a 2020 2020 656c 6966 2073 7263 5f74  e.    elif src_t
-0000c180: 6774 203d 3d20 2774 6774 2720 616e 6420  gt == 'tgt' and 
-0000c190: 6374 785b 2725 735f 6f64 6f6f 5f76 6572  ctx['%s_odoo_ver
-0000c1a0: 2720 2520 7372 635f 7467 745d 203d 3d20  ' % src_tgt] == 
-0000c1b0: 6374 785b 2766 696e 616c 5f76 6572 275d  ctx['final_ver']
-0000c1c0: 3a0a 2020 2020 2020 2020 6966 2063 7478  :.        if ctx
-0000c1d0: 2e67 6574 2827 6669 6e61 6c5f 636f 6e66  .get('final_conf
-0000c1e0: 6e27 293a 0a20 2020 2020 2020 2020 2020  n'):.           
-0000c1f0: 2063 7478 5b69 7465 6d5d 203d 2074 6774   ctx[item] = tgt
-0000c200: 5f63 7478 5b27 6669 6e61 6c5f 636f 6e66  _ctx['final_conf
-0000c210: 6e27 5d0a 2020 2020 2020 2020 2020 2020  n'].            
-0000c220: 6966 206e 6f74 206f 732e 7061 7468 2e69  if not os.path.i
-0000c230: 7366 696c 6528 6f64 6f6f 5f63 6f6e 666e  sfile(odoo_confn
-0000c240: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000c250: 2020 206f 646f 6f5f 636f 6e66 6e20 3d20     odoo_confn = 
-0000c260: 4661 6c73 650a 2020 2020 2020 2020 656c  False.        el
-0000c270: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000c280: 6374 785b 6974 656d 5d20 3d20 6f64 6f6f  ctx[item] = odoo
-0000c290: 5f63 6f6e 666e 0a20 2020 2020 2020 2020  _confn.         
-0000c2a0: 2020 206f 646f 6f5f 636f 6e66 6e20 3d20     odoo_confn = 
-0000c2b0: 4661 6c73 650a 2020 2020 656c 7365 3a0a  False.    else:.
-0000c2c0: 2020 2020 2020 2020 6374 785b 6974 656d          ctx[item
-0000c2d0: 5d20 3d20 6f64 6f6f 5f63 6f6e 666e 0a20  ] = odoo_confn. 
-0000c2e0: 2020 2020 2020 206f 646f 6f5f 636f 6e66         odoo_conf
-0000c2f0: 6e20 3d20 4661 6c73 650a 2020 2020 6966  n = False.    if
-0000c300: 206e 6f74 206f 732e 7061 7468 2e69 7366   not os.path.isf
-0000c310: 696c 6528 6374 785b 6974 656d 5d29 3a0a  ile(ctx[item]):.
-0000c320: 2020 2020 2020 2020 7261 6973 6520 494f          raise IO
-0000c330: 4572 726f 7228 2746 696c 6520 2573 206e  Error('File %s n
-0000c340: 6f74 2066 6f75 6e64 2720 2520 6374 785b  ot found' % ctx[
-0000c350: 6974 656d 5d29 0a20 2020 2063 6f6e 6669  item]).    confi
-0000c360: 6720 3d20 436f 6e66 6967 5061 7273 6572  g = ConfigParser
-0000c370: 2e53 6166 6543 6f6e 6669 6750 6172 7365  .SafeConfigParse
-0000c380: 7228 290a 2020 2020 6966 206f 646f 6f5f  r().    if odoo_
-0000c390: 636f 6e66 6e3a 0a20 2020 2020 2020 2063  confn:.        c
-0000c3a0: 6f6e 6669 672e 7265 6164 285b 6374 785b  onfig.read([ctx[
-0000c3b0: 6974 656d 5d2c 206f 646f 6f5f 636f 6e66  item], odoo_conf
-0000c3c0: 6e5d 290a 2020 2020 656c 7365 3a0a 2020  n]).    else:.  
-0000c3d0: 2020 2020 2020 636f 6e66 6967 2e72 6561        config.rea
-0000c3e0: 6428 6374 785b 6974 656d 5d29 0a20 2020  d(ctx[item]).   
-0000c3f0: 2072 6574 7572 6e20 636f 6e66 6967 0a0a   return config..
-0000c400: 0a64 6566 2063 6865 636b 5f63 6f6e 6628  .def check_conf(
-0000c410: 636f 6e66 6e2c 2070 6172 616d 293a 0a20  confn, param):. 
-0000c420: 2020 2066 6420 3d20 6f70 656e 2863 6f6e     fd = open(con
-0000c430: 666e 2c20 2772 5527 290a 2020 2020 6c69  fn, 'rU').    li
-0000c440: 6e65 7320 3d20 6664 2e72 6561 6428 292e  nes = fd.read().
-0000c450: 7370 6c69 7428 275c 6e27 290a 2020 2020  split('\n').    
-0000c460: 7661 6c75 6520 3d20 4661 6c73 650a 2020  value = False.  
-0000c470: 2020 666f 7220 6c69 6e65 2069 6e20 6c69    for line in li
-0000c480: 6e65 733a 0a20 2020 2020 2020 2074 6b6e  nes:.        tkn
-0000c490: 203d 206c 696e 652e 7370 6c69 7428 273d   = line.split('=
-0000c4a0: 2729 0a20 2020 2020 2020 2074 6b6e 203d  ').        tkn =
-0000c4b0: 206d 6170 286c 616d 6264 6120 783a 2078   map(lambda x: x
-0000c4c0: 2e73 7472 6970 2829 2c20 746b 6e29 0a20  .strip(), tkn). 
-0000c4d0: 2020 2020 2020 2069 6620 746b 6e5b 305d         if tkn[0]
-0000c4e0: 203d 3d20 7061 7261 6d3a 0a20 2020 2020   == param:.     
-0000c4f0: 2020 2020 2020 2076 616c 7565 203d 2074         value = t
-0000c500: 6b6e 5b31 5d0a 2020 2020 2020 2020 2020  kn[1].          
-0000c510: 2020 6272 6561 6b0a 2020 2020 6664 2e63    break.    fd.c
-0000c520: 6c6f 7365 2829 0a20 2020 2072 6574 7572  lose().    retur
-0000c530: 6e20 7661 6c75 650a 0a0a 6465 6620 6c6f  n value...def lo
-0000c540: 6164 5f6f 7065 6e75 7067 7261 6465 6c69  ad_openupgradeli
-0000c550: 6228 6374 782c 206f 646f 6f5f 6676 6572  b(ctx, odoo_fver
-0000c560: 293a 0a20 2020 206f 756c 7061 7468 5f70  ):.    oulpath_p
-0000c570: 6172 656e 7464 6972 203d 2020 6f73 2e70  arentdir =  os.p
-0000c580: 6174 682e 6469 726e 616d 6528 6374 785b  ath.dirname(ctx[
-0000c590: 276f 7074 5f6f 756c 7061 7468 275d 290a  'opt_oulpath']).
-0000c5a0: 2020 2020 6f75 6c6e 616d 6520 3d20 206f      oulname =  o
-0000c5b0: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
-0000c5c0: 6374 785b 276f 7074 5f6f 756c 7061 7468  ctx['opt_oulpath
-0000c5d0: 275d 290a 2020 2020 6f75 6c70 6174 685f  ']).    oulpath_
-0000c5e0: 6269 6e64 6972 203d 206f 732e 7061 7468  bindir = os.path
-0000c5f0: 2e6a 6f69 6e28 6374 785b 276f 7074 5f6f  .join(ctx['opt_o
-0000c600: 756c 7061 7468 275d 2c20 276f 7065 6e75  ulpath'], 'openu
-0000c610: 7067 7261 6465 6c69 6227 290a 2020 2020  pgradelib').    
-0000c620: 6f75 6c70 6174 685f 7363 7269 7074 203d  oulpath_script =
-0000c630: 206f 732e 7061 7468 2e6a 6f69 6e28 6f75   os.path.join(ou
-0000c640: 6c70 6174 685f 6269 6e64 6972 2c20 276f  lpath_bindir, 'o
-0000c650: 7065 6e75 7067 7261 6465 2e70 7927 290a  penupgrade.py').
-0000c660: 2020 2020 6f75 6c5f 6769 7420 3d20 2768      oul_git = 'h
-0000c670: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000c680: 6d2f 4f43 412f 6f70 656e 7570 6772 6164  m/OCA/openupgrad
-0000c690: 656c 6962 2e67 6974 270a 2020 2020 6f73  elib.git'.    os
-0000c6a0: 302e 776c 6f67 2827 3e3e 3e20 6c6f 6164  0.wlog('>>> load
-0000c6b0: 5f6f 7065 6e75 7067 7261 6465 6c69 6228  _openupgradelib(
-0000c6c0: 2573 2927 2025 206f 646f 6f5f 6676 6572  %s)' % odoo_fver
-0000c6d0: 290a 0a20 2020 2069 6620 6e6f 7420 6f73  )..    if not os
-0000c6e0: 2e70 6174 682e 6973 6469 7228 6f75 6c70  .path.isdir(oulp
-0000c6f0: 6174 685f 6269 6e64 6972 2920 6f72 206e  ath_bindir) or n
-0000c700: 6f74 206f 732e 7061 7468 2e69 7366 696c  ot os.path.isfil
-0000c710: 6528 6f75 6c70 6174 685f 7363 7269 7074  e(oulpath_script
-0000c720: 293a 0a20 2020 2020 2020 2077 6974 6820  ):.        with 
-0000c730: 7075 7368 6428 6f75 6c70 6174 685f 7061  pushd(oulpath_pa
-0000c740: 7265 6e74 6469 7229 3a0a 2020 2020 2020  rentdir):.      
-0000c750: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
-0000c760: 2e69 7364 6972 2863 7478 5b27 6f70 745f  .isdir(ctx['opt_
-0000c770: 6f75 6c70 6174 6827 5d29 3a0a 2020 2020  oulpath']):.    
-0000c780: 2020 2020 2020 2020 2020 2020 7368 7574              shut
-0000c790: 696c 2e72 6d74 7265 6528 6374 785b 276f  il.rmtree(ctx['o
-0000c7a0: 7074 5f6f 756c 7061 7468 275d 290a 2020  pt_oulpath']).  
-0000c7b0: 2020 2020 2020 2020 2020 7275 6e5f 7472            run_tr
-0000c7c0: 6163 6564 2827 6769 7427 2c20 2763 6c6f  aced('git', 'clo
-0000c7d0: 6e65 272c 206f 756c 5f67 6974 2c20 6f75  ne', oul_git, ou
-0000c7e0: 6c6e 616d 652c 0a20 2020 2020 2020 2020  lname,.         
-0000c7f0: 2020 2020 2020 2020 2020 2020 2020 272d                '-
-0000c800: 2d73 696e 676c 652d 6272 616e 6368 272c  -single-branch',
-0000c810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c820: 2020 2020 2020 2020 272d 2d64 6570 7468          '--depth
-0000c830: 272c 2027 3127 290a 2020 2020 656c 7365  ', '1').    else
-0000c840: 3a0a 2020 2020 2020 2020 6f73 302e 776c  :.        os0.wl
-0000c850: 6f67 2827 466f 756e 6420 7661 6c69 6420  og('Found valid 
-0000c860: 6469 7265 6374 6f72 7920 2573 2720 2520  directory %s' % 
-0000c870: 6f75 6c70 6174 685f 6269 6e64 6972 290a  oulpath_bindir).
-0000c880: 2020 2020 2320 7379 732e 7061 7468 2e61      # sys.path.a
-0000c890: 7070 656e 6428 6374 785b 276f 7074 5f6f  ppend(ctx['opt_o
-0000c8a0: 756c 7061 7468 275d 290a 2020 2020 6f73  ulpath']).    os
-0000c8b0: 2e65 6e76 6972 6f6e 5b27 5059 5448 4f4e  .environ['PYTHON
-0000c8c0: 5041 5448 275d 203d 2027 3a27 2e6a 6f69  PATH'] = ':'.joi
-0000c8d0: 6e28 6669 6c74 6572 284e 6f6e 652c 205b  n(filter(None, [
-0000c8e0: 0a20 2020 2020 2020 2063 7478 5b27 6f70  .        ctx['op
-0000c8f0: 745f 6f75 6c70 6174 6827 5d2c 206f 732e  t_oulpath'], os.
-0000c900: 656e 7669 726f 6e2e 6765 7428 2750 5954  environ.get('PYT
-0000c910: 484f 4e50 4154 4827 295d 2929 0a0a 0a64  HONPATH')]))...d
-0000c920: 6566 206c 6f61 645f 6f70 656e 7570 6772  ef load_openupgr
-0000c930: 6164 6528 6374 782c 206f 646f 6f5f 6676  ade(ctx, odoo_fv
-0000c940: 6572 293a 0a20 2020 2069 6620 6f64 6f6f  er):.    if odoo
-0000c950: 5f66 7665 723a 0a20 2020 2020 2020 206f  _fver:.        o
-0000c960: 7570 6174 685f 7061 7265 6e74 6469 7220  upath_parentdir 
-0000c970: 3d20 6f73 2e70 6174 682e 6469 726e 616d  = os.path.dirnam
-0000c980: 6528 6374 785b 276f 7074 5f6f 7570 6174  e(ctx['opt_oupat
-0000c990: 6827 5d29 0a20 2020 2020 2020 206f 7570  h']).        oup
-0000c9a0: 6174 685f 6469 7220 3d20 6374 785b 276f  ath_dir = ctx['o
-0000c9b0: 7074 5f6f 7570 6174 6827 5d0a 2020 2020  pt_oupath'].    
-0000c9c0: 2020 2020 6f75 5f76 6572 5f70 6174 6820      ou_ver_path 
-0000c9d0: 3d20 6f73 2e70 6174 682e 6a6f 696e 2863  = os.path.join(c
-0000c9e0: 7478 5b27 6f70 745f 6f75 7061 7468 275d  tx['opt_oupath']
-0000c9f0: 2c20 276f 755f 2573 2720 2520 6f64 6f6f  , 'ou_%s' % odoo
-0000ca00: 5f66 7665 7229 0a20 2020 2065 6c73 653a  _fver).    else:
-0000ca10: 0a20 2020 2020 2020 206f 7570 6174 685f  .        oupath_
-0000ca20: 7061 7265 6e74 6469 7220 3d20 6f73 2e70  parentdir = os.p
-0000ca30: 6174 682e 6578 7061 6e64 7573 6572 2827  ath.expanduser('
-0000ca40: 7e27 290a 2020 2020 2020 2020 6f75 7061  ~').        oupa
-0000ca50: 7468 5f64 6972 203d 206f 7570 6174 685f  th_dir = oupath_
-0000ca60: 7061 7265 6e74 6469 720a 2020 2020 2020  parentdir.      
-0000ca70: 2020 6f75 5f76 6572 5f70 6174 6820 3d20    ou_ver_path = 
-0000ca80: 6f73 2e70 6174 682e 6a6f 696e 286f 732e  os.path.join(os.
-0000ca90: 7061 7468 2e65 7870 616e 6475 7365 7228  path.expanduser(
-0000caa0: 277e 2729 2c20 276f 7065 6e75 7067 7261  '~'), 'openupgra
-0000cab0: 6465 2729 0a20 2020 206f 7570 6174 685f  de').    oupath_
-0000cac0: 6269 6e64 6972 3920 3d20 6f73 2e70 6174  bindir9 = os.pat
-0000cad0: 682e 6a6f 696e 286f 755f 7665 725f 7061  h.join(ou_ver_pa
-0000cae0: 7468 2c20 276f 7065 6e65 7270 2729 0a20  th, 'openerp'). 
-0000caf0: 2020 206f 7570 6174 685f 6269 6e64 6972     oupath_bindir
-0000cb00: 3130 203d 206f 732e 7061 7468 2e6a 6f69  10 = os.path.joi
-0000cb10: 6e28 6f75 5f76 6572 5f70 6174 682c 2027  n(ou_ver_path, '
-0000cb20: 6f64 6f6f 2729 0a20 2020 206f 755f 6769  odoo').    ou_gi
-0000cb30: 7420 3d20 2768 7474 7073 3a2f 2f67 6974  t = 'https://git
-0000cb40: 6875 622e 636f 6d2f 4f43 412f 6f70 656e  hub.com/OCA/open
-0000cb50: 7570 6772 6164 652e 6769 7427 0a20 2020  upgrade.git'.   
-0000cb60: 206f 7330 2e77 6c6f 6728 273e 3e3e 206c   os0.wlog('>>> l
-0000cb70: 6f61 645f 6f70 656e 7570 6772 6164 6528  oad_openupgrade(
-0000cb80: 2573 2927 2025 2063 7478 5b27 7467 745f  %s)' % ctx['tgt_
-0000cb90: 6f64 6f6f 5f66 7665 7227 5d29 0a0a 2020  odoo_fver'])..  
-0000cba0: 2020 6465 6620 6765 745f 6f75 5f72 656c    def get_ou_rel
-0000cbb0: 6561 7365 286f 7570 6174 685f 6269 6e64  ease(oupath_bind
-0000cbc0: 6972 293a 0a20 2020 2020 2020 2077 6974  ir):.        wit
-0000cbd0: 6820 7075 7368 6428 6f75 7061 7468 5f62  h pushd(oupath_b
-0000cbe0: 696e 6469 7229 3a0a 2020 2020 2020 2020  indir):.        
-0000cbf0: 2020 2020 7379 732e 7061 7468 2e69 6e73      sys.path.ins
-0000cc00: 6572 7428 302c 2027 2729 0a20 2020 2020  ert(0, '').     
-0000cc10: 2020 2020 2020 2069 6d70 6f72 7420 7265         import re
-0000cc20: 6c65 6173 650a 2020 2020 2020 2020 2020  lease.          
-0000cc30: 2020 7820 3d20 7265 2e6d 6174 6368 2872    x = re.match(r
-0000cc40: 275b 302d 395d 2b5c 2e5b 302d 395d 2b27  '[0-9]+\.[0-9]+'
-0000cc50: 2c20 7265 6c65 6173 652e 7665 7273 696f  , release.versio
-0000cc60: 6e29 0a20 2020 2020 2020 2020 2020 2069  n).            i
-0000cc70: 6620 783a 0a20 2020 2020 2020 2020 2020  f x:.           
-0000cc80: 2020 2020 206f 755f 7665 7220 3d20 7265       ou_ver = re
-0000cc90: 6c65 6173 652e 7665 7273 696f 6e5b 303a  lease.version[0:
-0000cca0: 782e 656e 6428 295d 0a20 2020 2020 2020  x.end()].       
-0000ccb0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000ccc0: 2020 2020 2020 2020 2020 206f 755f 7665             ou_ve
-0000ccd0: 7220 3d20 7265 6c65 6173 652e 7665 7273  r = release.vers
-0000cce0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-0000ccf0: 6465 6c20 7379 732e 7061 7468 5b30 5d0a  del sys.path[0].
-0000cd00: 2020 2020 2020 2020 7265 7475 726e 206f          return o
-0000cd10: 755f 7665 720a 0a20 2020 206f 755f 7665  u_ver..    ou_ve
-0000cd20: 7220 3d20 2727 0a20 2020 2069 6620 6e6f  r = ''.    if no
-0000cd30: 7420 6f73 2e70 6174 682e 6578 6973 7473  t os.path.exists
-0000cd40: 286f 755f 7665 725f 7061 7468 293a 0a20  (ou_ver_path):. 
-0000cd50: 2020 2020 2020 2069 6620 6e6f 7420 6f73         if not os
-0000cd60: 2e70 6174 682e 6578 6973 7473 286f 7570  .path.exists(oup
-0000cd70: 6174 685f 7061 7265 6e74 6469 7229 3a0a  ath_parentdir):.
-0000cd80: 2020 2020 2020 2020 2020 2020 6f73 2e6d              os.m
-0000cd90: 6b64 6972 286f 7570 6174 685f 7061 7265  kdir(oupath_pare
-0000cda0: 6e74 6469 7229 0a20 2020 2020 2020 2069  ntdir).        i
-0000cdb0: 6620 6f64 6f6f 5f66 7665 7220 616e 6420  f odoo_fver and 
-0000cdc0: 6e6f 7420 6f73 2e70 6174 682e 6578 6973  not os.path.exis
-0000cdd0: 7473 2863 7478 5b27 6f70 745f 6f75 7061  ts(ctx['opt_oupa
-0000cde0: 7468 275d 293a 0a20 2020 2020 2020 2020  th']):.         
-0000cdf0: 2020 206f 732e 6d6b 6469 7228 6374 785b     os.mkdir(ctx[
-0000ce00: 276f 7074 5f6f 7570 6174 6827 5d29 0a20  'opt_oupath']). 
-0000ce10: 2020 2020 2020 206f 732e 6d6b 6469 7228         os.mkdir(
-0000ce20: 6f75 5f76 6572 5f70 6174 6829 0a20 2020  ou_ver_path).   
-0000ce30: 2065 6c69 6620 6f73 2e70 6174 682e 6973   elif os.path.is
-0000ce40: 6469 7228 6f75 7061 7468 5f62 696e 6469  dir(oupath_bindi
-0000ce50: 7231 3029 3a0a 2020 2020 2020 2020 6f75  r10):.        ou
-0000ce60: 5f76 6572 203d 2067 6574 5f6f 755f 7265  _ver = get_ou_re
-0000ce70: 6c65 6173 6528 6f75 7061 7468 5f62 696e  lease(oupath_bin
-0000ce80: 6469 7231 3029 0a20 2020 2065 6c69 6620  dir10).    elif 
-0000ce90: 6f73 2e70 6174 682e 6973 6469 7228 6f75  os.path.isdir(ou
-0000cea0: 7061 7468 5f62 696e 6469 7239 293a 0a20  path_bindir9):. 
-0000ceb0: 2020 2020 2020 206f 755f 7665 7220 3d20         ou_ver = 
-0000cec0: 6765 745f 6f75 5f72 656c 6561 7365 286f  get_ou_release(o
-0000ced0: 7570 6174 685f 6269 6e64 6972 3929 0a20  upath_bindir9). 
-0000cee0: 2020 2069 6620 6f75 5f76 6572 2021 3d20     if ou_ver != 
-0000cef0: 6374 785b 2774 6774 5f6f 646f 6f5f 6676  ctx['tgt_odoo_fv
-0000cf00: 6572 275d 3a0a 2020 2020 2020 2020 7769  er']:.        wi
-0000cf10: 7468 2070 7573 6864 286f 7570 6174 685f  th pushd(oupath_
-0000cf20: 6469 7229 3a0a 2020 2020 2020 2020 2020  dir):.          
-0000cf30: 2020 6966 206f 646f 6f5f 6676 6572 2061    if odoo_fver a
-0000cf40: 6e64 206f 732e 7061 7468 2e69 7364 6972  nd os.path.isdir
-0000cf50: 286f 755f 7665 725f 7061 7468 293a 0a20  (ou_ver_path):. 
-0000cf60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000cf70: 6875 7469 6c2e 726d 7472 6565 286f 755f  hutil.rmtree(ou_
-0000cf80: 7665 725f 7061 7468 290a 2020 2020 2020  ver_path).      
-0000cf90: 2020 2020 2020 7275 6e5f 7472 6163 6564        run_traced
-0000cfa0: 2827 6769 7427 2c20 2763 6c6f 6e65 272c  ('git', 'clone',
-0000cfb0: 206f 755f 6769 742c 0a20 2020 2020 2020   ou_git,.       
-0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfd0: 6f73 2e70 6174 682e 6261 7365 6e61 6d65  os.path.basename
-0000cfe0: 286f 755f 7665 725f 7061 7468 292c 0a20  (ou_ver_path),. 
-0000cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d000: 2020 2020 2020 272d 6227 2c20 6374 785b        '-b', ctx[
-0000d010: 2774 6774 5f6f 646f 6f5f 6676 6572 275d  'tgt_odoo_fver']
-0000d020: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d030: 2020 2020 2020 2020 2027 2d2d 7369 6e67           '--sing
-0000d040: 6c65 2d62 7261 6e63 6827 2c0a 2020 2020  le-branch',.    
-0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d060: 2020 2027 2d2d 6465 7074 6827 2c20 2731     '--depth', '1
-0000d070: 2729 0a20 2020 2020 2020 2020 2020 2061  ').            a
-0000d080: 7070 6c79 5f70 6174 6368 286f 755f 7665  pply_patch(ou_ve
-0000d090: 725f 7061 7468 2c20 6374 785b 2774 6774  r_path, ctx['tgt
-0000d0a0: 5f6f 646f 6f5f 6676 6572 275d 290a 2020  _odoo_fver']).  
-0000d0b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000d0c0: 6f73 302e 776c 6f67 2827 466f 756e 6420  os0.wlog('Found 
-0000d0d0: 7661 6c69 6420 6469 7265 6374 6f72 7920  valid directory 
-0000d0e0: 2573 2720 2520 6374 785b 276f 7074 5f6f  %s' % ctx['opt_o
-0000d0f0: 7570 6174 6827 5d29 0a20 2020 2069 6620  upath']).    if 
-0000d100: 6e6f 7420 7372 635f 6374 785b 276e 6f5f  not src_ctx['no_
-0000d110: 7665 6e76 275d 2061 6e64 206e 6f74 2073  venv'] and not s
-0000d120: 7263 5f63 7478 5b27 6472 795f 7275 6e27  rc_ctx['dry_run'
-0000d130: 5d3a 0a20 2020 2020 2020 2076 656e 765f  ]:.        venv_
-0000d140: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-0000d150: 6f69 6e28 7467 745f 6374 785b 2776 656e  oin(tgt_ctx['ven
-0000d160: 765f 6f75 7061 7468 275d 2c20 276f 7065  v_oupath'], 'ope
-0000d170: 6e75 7067 7261 6465 2729 0a20 2020 2020  nupgrade').     
-0000d180: 2020 2069 6620 6e6f 7420 6f73 2e70 6174     if not os.pat
-0000d190: 682e 6973 6469 7228 7665 6e76 5f70 6174  h.isdir(venv_pat
-0000d1a0: 6829 3a0a 2020 2020 2020 2020 2020 2020  h):.            
-0000d1b0: 6f73 2e73 796d 6c69 6e6b 286f 755f 7665  os.symlink(ou_ve
-0000d1c0: 725f 7061 7468 2c20 7665 6e76 5f70 6174  r_path, venv_pat
-0000d1d0: 6829 0a20 2020 2072 6574 7572 6e20 6f75  h).    return ou
-0000d1e0: 5f76 6572 5f70 6174 680a 0a0a 6465 6620  _ver_path...def 
-0000d1f0: 6170 706c 795f 7061 7463 6828 6f75 5f76  apply_patch(ou_v
-0000d200: 6572 5f70 6174 682c 206f 646f 6f5f 6676  er_path, odoo_fv
-0000d210: 6572 293a 0a20 2020 2069 6620 6f64 6f6f  er):.    if odoo
-0000d220: 5f66 7665 7220 3d3d 2027 392e 3027 3a0a  _fver == '9.0':.
-0000d230: 2020 2020 2020 2020 6669 6c65 203d 206f          file = o
-0000d240: 732e 7061 7468 2e6a 6f69 6e28 6f75 5f76  s.path.join(ou_v
-0000d250: 6572 5f70 6174 682c 2027 6f70 656e 6572  er_path, 'opener
-0000d260: 7027 2c20 2761 6464 6f6e 7327 2c20 2762  p', 'addons', 'b
-0000d270: 6173 6527 2c0a 2020 2020 2020 2020 2020  ase',.          
-0000d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d290: 2020 276d 6967 7261 7469 6f6e 7327 2c20    'migrations', 
-0000d2a0: 2739 2e30 2e31 2e33 272c 2027 706f 7374  '9.0.1.3', 'post
-0000d2b0: 2d6d 6967 7261 7469 6f6e 2e70 7927 290a  -migration.py').
-0000d2c0: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
-0000d2d0: 7468 2e69 7366 696c 6528 6669 6c65 293a  th.isfile(file):
-0000d2e0: 0a20 2020 2020 2020 2020 2020 2073 6564  .            sed
-0000d2f0: 2866 696c 652c 0a20 2020 2020 2020 2020  (file,.         
-0000d300: 2020 2020 2020 205b 7222 5e20 2a27 6972         [r"^ *'ir
-0000d310: 5f61 6374 696f 6e73 273a 205c 5b22 2c20  _actions': \[", 
-0000d320: 2223 2020 2020 2027 6972 5f61 6374 696f  "#     'ir_actio
-0000d330: 6e73 273a 205b 225d 2c0a 2020 2020 2020  ns': ["],.      
-0000d340: 2020 2020 2020 2020 2020 5b72 225e 202a            [r"^ *
-0000d350: 5c28 2768 656c 7027 2c20 4e6f 6e65 2c20  \('help', None, 
-0000d360: 4e6f 6e65 5c29 2c22 2c0a 2020 2020 2020  None\),",.      
-0000d370: 2020 2020 2020 2020 2020 2022 2320 2020             "#   
-0000d380: 2020 2020 2020 2827 6865 6c70 272c 204e        ('help', N
-0000d390: 6f6e 652c 204e 6f6e 6529 2c22 5d2c 0a20  one, None),"],. 
-0000d3a0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-0000d3b0: 225e 202a 5d2c 222c 2022 2320 2020 2020  "^ *],", "#     
-0000d3c0: 5d2c 225d 2c0a 2020 2020 2020 2020 2020  ],"],.          
-0000d3d0: 2020 2020 2020 290a 0a0a 6465 6620 6164        )...def ad
-0000d3e0: 645f 746e 6c5f 6974 656d 2863 7478 2c20  d_tnl_item(ctx, 
-0000d3f0: 6d6f 6465 6c2c 206d 6f64 756c 652c 206e  model, module, n
-0000d400: 6577 5f6d 6f64 756c 652c 2073 7263 5f66  ew_module, src_f
-0000d410: 7665 722c 2074 6774 5f66 7665 722c 0a20  ver, tgt_fver,. 
-0000d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d430: 7479 7065 3d46 616c 7365 293a 0a20 2020  type=False):.   
-0000d440: 2074 6e6c 203d 2074 7261 6e73 6f64 6f6f   tnl = transodoo
-0000d450: 2e74 7261 6e73 6c61 7465 5f66 726f 6d5f  .translate_from_
-0000d460: 746f 2863 7478 2c20 6d6f 6465 6c2c 206d  to(ctx, model, m
-0000d470: 6f64 756c 652c 2073 7263 5f66 7665 722c  odule, src_fver,
-0000d480: 2074 6774 5f66 7665 722c 0a20 2020 2020   tgt_fver,.     
-0000d490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4b0: 2074 7970 653d 7479 7065 290a 2020 2020   type=type).    
-0000d4c0: 6966 2074 6e6c 2021 3d20 6e65 775f 6d6f  if tnl != new_mo
-0000d4d0: 6475 6c65 3a0a 2020 2020 2020 2020 6f73  dule:.        os
-0000d4e0: 302e 776c 6f67 2827 5472 616e 736c 6174  0.wlog('Translat
-0000d4f0: 6520 6d6f 6475 6c65 2025 7320 2d3e 2025  e module %s -> %
-0000d500: 7327 2025 2028 6d6f 6475 6c65 2c20 6e65  s' % (module, ne
-0000d510: 775f 6d6f 6475 6c65 2929 0a20 2020 2020  w_module)).     
-0000d520: 2020 2076 6572 5f6e 616d 6573 203d 207b     ver_names = {
-0000d530: 7d0a 2020 2020 2020 2020 6e61 6d65 203d  }.        name =
-0000d540: 206d 6f64 756c 650a 2020 2020 2020 2020   module.        
-0000d550: 666f 7220 7665 7220 696e 2056 4552 5349  for ver in VERSI
-0000d560: 4f4e 533a 0a20 2020 2020 2020 2020 2020  ONS:.           
-0000d570: 2069 6620 7665 7220 3d3d 2063 7478 5b27   if ver == ctx['
-0000d580: 7467 745f 6f64 6f6f 5f66 7665 7227 5d3a  tgt_odoo_fver']:
-0000d590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d5a0: 206e 616d 6520 3d20 6e65 775f 6d6f 6475   name = new_modu
-0000d5b0: 6c65 0a20 2020 2020 2020 2020 2020 2076  le.            v
-0000d5c0: 6572 5f6e 616d 6573 5b76 6572 5d20 3d20  er_names[ver] = 
-0000d5d0: 6e61 6d65 0a20 2020 2020 2020 2075 6e61  name.        una
-0000d5e0: 6d65 203d 2074 7261 6e73 6f64 6f6f 2e73  me = transodoo.s
-0000d5f0: 6574 5f75 6e61 6d65 2874 7970 652c 206e  et_uname(type, n
-0000d600: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-0000d610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d620: 2020 2020 2020 2020 205b 7665 725f 6e61           [ver_na
-0000d630: 6d65 735b 785d 2066 6f72 2078 2069 6e20  mes[x] for x in 
-0000d640: 5645 5253 494f 4e53 5d29 0a20 2020 2020  VERSIONS]).     
-0000d650: 2020 2066 6f72 2076 6572 2069 6e20 5645     for ver in VE
-0000d660: 5253 494f 4e53 3a0a 2020 2020 2020 2020  RSIONS:.        
-0000d670: 2020 2020 6374 785b 276d 696e 6472 6f6f      ctx['mindroo
-0000d680: 7427 5d20 203d 2074 7261 6e73 6f64 6f6f  t']  = transodoo
-0000d690: 2e6c 696e 6b5f 7665 7273 696f 6e65 645f  .link_versioned_
-0000d6a0: 6e61 6d65 280a 2020 2020 2020 2020 2020  name(.          
-0000d6b0: 2020 2020 2020 6374 785b 276d 696e 6472        ctx['mindr
-0000d6c0: 6f6f 7427 5d2c 0a20 2020 2020 2020 2020  oot'],.         
-0000d6d0: 2020 2020 2020 206d 6f64 656c 2c0a 2020         model,.  
-0000d6e0: 2020 2020 2020 2020 2020 2020 2020 756e                un
-0000d6f0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-0000d700: 2020 2020 2074 7970 652c 0a20 2020 2020       type,.     
-0000d710: 2020 2020 2020 2020 2020 2076 6572 5f6e             ver_n
-0000d720: 616d 6573 5b76 6572 5d2c 0a20 2020 2020  ames[ver],.     
-0000d730: 2020 2020 2020 2020 2020 2076 6572 290a             ver).
-0000d740: 2020 2020 7265 7475 726e 2063 7478 0a0a      return ctx..
-0000d750: 0a64 6566 2064 6f5f 746e 6c5f 6d6f 6475  .def do_tnl_modu
-0000d760: 6c65 5f6c 6973 7428 6374 782c 206d 6f64  le_list(ctx, mod
-0000d770: 756c 655f 6c69 7374 2c20 7372 635f 6676  ule_list, src_fv
-0000d780: 6572 2c20 7467 745f 6676 6572 2c20 7467  er, tgt_fver, tg
-0000d790: 745f 6d6f 6475 6c65 5f6c 6973 742c 0a20  t_module_list,. 
-0000d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7b0: 2020 2020 2020 7075 7265 3d4e 6f6e 6529        pure=None)
-0000d7c0: 3a0a 2020 2020 7379 732e 7061 7468 2e61  :.    sys.path.a
-0000d7d0: 7070 656e 6428 6f73 2e70 6174 682e 6469  ppend(os.path.di
-0000d7e0: 726e 616d 6528 5f5f 6669 6c65 5f5f 2929  rname(__file__))
-0000d7f0: 0a20 2020 2074 7261 6e73 6f64 6f6f 2e72  .    transodoo.r
-0000d800: 6561 645f 7374 6f72 6564 5f64 6963 7428  ead_stored_dict(
-0000d810: 6374 7829 0a20 2020 2074 6e6c 5f6d 6f64  ctx).    tnl_mod
-0000d820: 756c 655f 6c69 7374 203d 205b 5d0a 2020  ule_list = [].  
-0000d830: 2020 6261 645f 6d6f 6475 6c65 5f6c 6973    bad_module_lis
-0000d840: 7420 3d20 5b5d 0a20 2020 206d 6f64 656c  t = [].    model
-0000d850: 203d 2027 6972 2e6d 6f64 756c 652e 6d6f   = 'ir.module.mo
-0000d860: 6475 6c65 270a 2020 2020 666f 7220 6974  dule'.    for it
-0000d870: 656d 2069 6e20 6d6f 6475 6c65 5f6c 6973  em in module_lis
-0000d880: 743a 0a20 2020 2020 2020 2074 6e6c 203d  t:.        tnl =
-0000d890: 2074 7261 6e73 6f64 6f6f 2e74 7261 6e73   transodoo.trans
-0000d8a0: 6c61 7465 5f66 726f 6d5f 746f 280a 2020  late_from_to(.  
-0000d8b0: 2020 2020 2020 2020 2020 6374 782c 206d            ctx, m
-0000d8c0: 6f64 656c 2c20 6974 656d 2c20 7372 635f  odel, item, src_
-0000d8d0: 6676 6572 2c20 7467 745f 6676 6572 2c20  fver, tgt_fver, 
-0000d8e0: 7479 7065 3d27 6d6f 6475 6c65 2729 0a20  type='module'). 
-0000d8f0: 2020 2020 2020 2069 6620 746e 6c20 3d3d         if tnl ==
-0000d900: 2069 7465 6d3a 0a20 2020 2020 2020 2020   item:.         
-0000d910: 2020 2074 6e6c 203d 2074 7261 6e73 6f64     tnl = transod
-0000d920: 6f6f 2e74 7261 6e73 6c61 7465 5f66 726f  oo.translate_fro
-0000d930: 6d5f 746f 280a 2020 2020 2020 2020 2020  m_to(.          
-0000d940: 2020 2020 2020 6374 782c 206d 6f64 656c        ctx, model
-0000d950: 2c20 6974 656d 2c20 7372 635f 6676 6572  , item, src_fver
-0000d960: 2c20 7467 745f 6676 6572 2c20 7479 7065  , tgt_fver, type
-0000d970: 3d27 6d65 7267 6527 290a 2020 2020 2020  ='merge').      
-0000d980: 2020 6966 2074 6774 5f6d 6f64 756c 655f    if tgt_module_
-0000d990: 6c69 7374 2061 6e64 2074 6e6c 206e 6f74  list and tnl not
-0000d9a0: 2069 6e20 7467 745f 6d6f 6475 6c65 5f6c   in tgt_module_l
-0000d9b0: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
-0000d9c0: 2062 6164 5f6d 6f64 756c 655f 6c69 7374   bad_module_list
-0000d9d0: 2e61 7070 656e 6428 6974 656d 290a 2020  .append(item).  
-0000d9e0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000d9f0: 2070 7572 653a 0a20 2020 2020 2020 2020   pure:.         
-0000da00: 2020 2020 2020 2074 6e6c 5f6d 6f64 756c         tnl_modul
-0000da10: 655f 6c69 7374 2e61 7070 656e 6428 746e  e_list.append(tn
-0000da20: 6c29 0a20 2020 2020 2020 2065 6c73 653a  l).        else:
-0000da30: 0a20 2020 2020 2020 2020 2020 2074 6e6c  .            tnl
-0000da40: 5f6d 6f64 756c 655f 6c69 7374 2e61 7070  _module_list.app
-0000da50: 656e 6428 746e 6c29 0a20 2020 2072 6574  end(tnl).    ret
-0000da60: 7572 6e20 746e 6c5f 6d6f 6475 6c65 5f6c  urn tnl_module_l
-0000da70: 6973 742c 2062 6164 5f6d 6f64 756c 655f  ist, bad_module_
-0000da80: 6c69 7374 0a0a 0a64 6566 206f 646f 6f5f  list...def odoo_
-0000da90: 6465 7065 6e64 656e 6369 6573 2863 7478  dependencies(ctx
-0000daa0: 2c20 6163 7469 6f6e 2c20 6462 5f6e 616d  , action, db_nam
-0000dab0: 652c 206c 636f 6e66 2c20 7061 7468 732c  e, lconf, paths,
-0000dac0: 206f 646f 6f5f 6676 6572 2c0a 2020 2020   odoo_fver,.    
-0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dae0: 2020 6d61 7463 6865 733d 4e6f 6e65 2c20    matches=None, 
-0000daf0: 6465 7065 6e64 735f 6279 3d4e 6f6e 6529  depends_by=None)
-0000db00: 3a0a 2020 2020 7769 7468 2070 7573 6864  :.    with pushd
-0000db10: 2827 2f6f 7074 2f6f 646f 6f2f 6465 762f  ('/opt/odoo/dev/
-0000db20: 7079 7069 2f77 6f6b 5f63 6f64 652f 776f  pypi/wok_code/wo
-0000db30: 6b5f 636f 6465 2729 3a0a 2020 2020 2020  k_code'):.      
-0000db40: 2020 7379 732e 7061 7468 2e61 7070 656e    sys.path.appen
-0000db50: 6428 2727 290a 2020 2020 2020 2020 696d  d('').        im
-0000db60: 706f 7274 206f 646f 6f5f 6465 7065 6e64  port odoo_depend
-0000db70: 656e 6369 6573 0a20 2020 2020 2020 2063  encies.        c
-0000db80: 7478 5b27 6272 616e 6368 275d 203d 206f  tx['branch'] = o
-0000db90: 646f 6f5f 6676 6572 0a20 2020 2020 2020  doo_fver.       
-0000dba0: 2069 6620 6462 5f6e 616d 653a 0a20 2020   if db_name:.   
-0000dbb0: 2020 2020 2020 2020 2063 7478 5b27 636f           ctx['co
-0000dbc0: 6e66 5f66 6e27 5d20 3d20 6c63 6f6e 660a  nf_fn'] = lconf.
-0000dbd0: 2020 2020 2020 2020 2020 2020 6374 7820              ctx 
-0000dbe0: 3d20 6f64 6f6f 5f64 6570 656e 6465 6e63  = odoo_dependenc
-0000dbf0: 6965 732e 7265 7472 6965 7665 5f64 625f  ies.retrieve_db_
-0000dc00: 6d6f 6475 6c65 7328 6374 7829 0a20 2020  modules(ctx).   
-0000dc10: 2020 2020 2020 2020 206d 6174 6368 6573           matches
-0000dc20: 203d 2063 7478 5b27 6d6f 6475 6c65 735f   = ctx['modules_
-0000dc30: 746f 5f6d 6174 6368 275d 0a20 2020 2020  to_match'].     
-0000dc40: 2020 2069 6620 6163 7469 6f6e 203d 3d20     if action == 
-0000dc50: 2764 6570 273a 0a20 2020 2020 2020 2020  'dep':.         
-0000dc60: 2020 2072 6573 203d 206f 646f 6f5f 6465     res = odoo_de
-0000dc70: 7065 6e64 656e 6369 6573 2e67 6574 5f64  pendencies.get_d
-0000dc80: 6570 656e 6465 6e63 6965 735f 6c69 7374  ependencies_list
-0000dc90: 2870 6174 6873 2c0a 2020 2020 2020 2020  (paths,.        
-0000dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcd0: 2020 6d61 7463 6865 733d 6d61 7463 6865    matches=matche
-0000dce0: 7329 0a20 2020 2020 2020 2065 6c69 6620  s).        elif 
-0000dcf0: 6163 7469 6f6e 203d 3d20 276d 6f64 273a  action == 'mod':
-0000dd00: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000dd10: 203d 206f 646f 6f5f 6465 7065 6e64 656e   = odoo_dependen
-0000dd20: 6369 6573 2e67 6574 5f6d 6f64 756c 6573  cies.get_modules
-0000dd30: 5f6c 6973 7428 7061 7468 732c 206d 6174  _list(paths, mat
-0000dd40: 6368 6573 3d6d 6174 6368 6573 290a 2020  ches=matches).  
-0000dd50: 2020 2020 2020 656c 6966 2061 6374 696f        elif actio
-0000dd60: 6e20 3d3d 2027 7265 7627 3a0a 2020 2020  n == 'rev':.    
-0000dd70: 2020 2020 2020 2020 7265 7320 3d20 6f64          res = od
-0000dd80: 6f6f 5f64 6570 656e 6465 6e63 6965 732e  oo_dependencies.
-0000dd90: 6765 745f 6465 7065 6e64 656e 7473 5f6c  get_dependents_l
-0000dda0: 6973 7428 0a20 2020 2020 2020 2020 2020  ist(.           
-0000ddb0: 2020 2020 2070 6174 6873 2c20 6d61 7463       paths, matc
-0000ddc0: 6865 733d 6d61 7463 6865 732c 2064 6570  hes=matches, dep
-0000ddd0: 656e 6473 5f62 793d 6465 7065 6e64 735f  ends_by=depends_
-0000dde0: 6279 290a 2020 2020 6465 6c20 7379 732e  by).    del sys.
-0000ddf0: 7061 7468 5b2d 315d 0a20 2020 2072 6574  path[-1].    ret
-0000de00: 7572 6e20 7265 730a 0a0a 6465 6620 6164  urn res...def ad
-0000de10: 645f 7665 7273 696f 6e65 645f 746e 6c28  d_versioned_tnl(
-0000de20: 6374 782c 2073 7263 5f66 7665 722c 2074  ctx, src_fver, t
-0000de30: 6774 5f66 7665 7229 3a0a 2020 2020 6f73  gt_fver):.    os
-0000de40: 302e 776c 6f67 2827 5570 6772 6164 696e  0.wlog('Upgradin
-0000de50: 6720 7472 616e 736c 6174 696f 6e20 6e61  g translation na
-0000de60: 6d65 2066 726f 6d20 2573 2074 6f20 2573  me from %s to %s
-0000de70: 2720 2520 2873 7263 5f66 7665 722c 2074  ' % (src_fver, t
-0000de80: 6774 5f66 7665 7229 290a 2020 2020 6f75  gt_fver)).    ou
-0000de90: 5f76 6572 5f70 6174 6820 3d20 6f73 2e70  _ver_path = os.p
-0000dea0: 6174 682e 6a6f 696e 2863 7478 5b27 6f70  ath.join(ctx['op
-0000deb0: 745f 6f75 7061 7468 275d 2c20 276f 755f  t_oupath'], 'ou_
-0000dec0: 2573 2720 2520 7467 745f 6676 6572 290a  %s' % tgt_fver).
-0000ded0: 2020 2020 7769 7468 2070 7573 6864 286f      with pushd(o
-0000dee0: 755f 7665 725f 7061 7468 293a 0a20 2020  u_ver_path):.   
-0000def0: 2020 2020 2073 7973 2e70 6174 682e 6170       sys.path.ap
-0000df00: 7065 6e64 2827 2729 0a20 2020 2020 2020  pend('').       
-0000df10: 2073 7973 2e70 6174 682e 6170 7065 6e64   sys.path.append
-0000df20: 286f 732e 7061 7468 2e64 6972 6e61 6d65  (os.path.dirname
-0000df30: 285f 5f66 696c 655f 5f29 290a 2020 2020  (__file__)).    
-0000df40: 2020 2020 6966 2069 6e74 2874 6774 5f66      if int(tgt_f
-0000df50: 7665 722e 7370 6c69 7428 272e 2729 5b30  ver.split('.')[0
-0000df60: 5d29 203c 2031 303a 0a20 2020 2020 2020  ]) < 10:.       
-0000df70: 2020 2020 2069 6d70 6f72 7420 6f70 656e       import open
-0000df80: 6572 702e 6164 646f 6e73 2e6f 7065 6e75  erp.addons.openu
-0000df90: 7067 7261 6465 5f72 6563 6f72 6473 2e6c  pgrade_records.l
-0000dfa0: 6962 2e61 7072 696f 7269 2061 7320 6170  ib.apriori as ap
-0000dfb0: 7269 6f72 690a 2020 2020 2020 2020 656c  riori.        el
-0000dfc0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000dfd0: 696d 706f 7274 206f 646f 6f2e 6164 646f  import odoo.addo
-0000dfe0: 6e73 2e6f 7065 6e75 7067 7261 6465 5f72  ns.openupgrade_r
-0000dff0: 6563 6f72 6473 2e6c 6962 2e61 7072 696f  ecords.lib.aprio
-0000e000: 7269 2061 7320 6170 7269 6f72 690a 2020  ri as apriori.  
-0000e010: 2020 2020 2020 7472 616e 736f 646f 6f2e        transodoo.
-0000e020: 7265 6164 5f73 746f 7265 645f 6469 6374  read_stored_dict
-0000e030: 2863 7478 290a 2020 2020 2020 2020 6d6f  (ctx).        mo
-0000e040: 6465 6c20 3d20 2769 722e 6d6f 6475 6c65  del = 'ir.module
-0000e050: 2e6d 6f64 756c 6527 0a20 2020 2020 2020  .module'.       
-0000e060: 2069 6620 6861 7361 7474 7228 6170 7269   if hasattr(apri
-0000e070: 6f72 692c 2027 7265 6e61 6d65 645f 6d6f  ori, 'renamed_mo
-0000e080: 6475 6c65 7327 293a 0a20 2020 2020 2020  dules'):.       
-0000e090: 2020 2020 2074 7970 203d 2027 6d6f 6475       typ = 'modu
-0000e0a0: 6c65 270a 2020 2020 2020 2020 2020 2020  le'.            
-0000e0b0: 666f 7220 6d6f 6475 6c65 2069 6e20 6170  for module in ap
-0000e0c0: 7269 6f72 692e 7265 6e61 6d65 645f 6d6f  riori.renamed_mo
-0000e0d0: 6475 6c65 733a 0a20 2020 2020 2020 2020  dules:.         
-0000e0e0: 2020 2020 2020 206e 6577 5f6d 6f64 756c         new_modul
-0000e0f0: 6520 3d20 6170 7269 6f72 692e 7265 6e61  e = apriori.rena
-0000e100: 6d65 645f 6d6f 6475 6c65 735b 6d6f 6475  med_modules[modu
-0000e110: 6c65 5d0a 2020 2020 2020 2020 2020 2020  le].            
-0000e120: 2020 2020 6374 7820 3d20 6164 645f 746e      ctx = add_tn
-0000e130: 6c5f 6974 656d 2863 7478 2c20 6d6f 6465  l_item(ctx, mode
-0000e140: 6c2c 206d 6f64 756c 652c 206e 6577 5f6d  l, module, new_m
-0000e150: 6f64 756c 652c 0a20 2020 2020 2020 2020  odule,.         
-0000e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e170: 2020 2020 2020 2020 2020 7372 635f 6676            src_fv
-0000e180: 6572 2c20 7467 745f 6676 6572 2c20 7479  er, tgt_fver, ty
-0000e190: 7065 3d74 7970 290a 2020 2020 2020 2020  pe=typ).        
-0000e1a0: 6966 2068 6173 6174 7472 2861 7072 696f  if hasattr(aprio
-0000e1b0: 7269 2c20 276d 6572 6765 645f 6d6f 6475  ri, 'merged_modu
-0000e1c0: 6c65 7327 293a 0a20 2020 2020 2020 2020  les'):.         
-0000e1d0: 2020 2074 7970 203d 2027 6d65 7267 6527     typ = 'merge'
-0000e1e0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000e1f0: 2069 7465 6d20 696e 2061 7072 696f 7269   item in apriori
-0000e200: 2e6d 6572 6765 645f 6d6f 6475 6c65 733a  .merged_modules:
-0000e210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e220: 206d 6f64 756c 6520 3d20 6974 656d 5b30   module = item[0
-0000e230: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000e240: 2020 6e65 775f 6d6f 6475 6c65 203d 2069    new_module = i
-0000e250: 7465 6d5b 315d 0a20 2020 2020 2020 2020  tem[1].         
-0000e260: 2020 2020 2020 2063 7478 203d 2061 6464         ctx = add
-0000e270: 5f74 6e6c 5f69 7465 6d28 6374 782c 206d  _tnl_item(ctx, m
-0000e280: 6f64 656c 2c20 6d6f 6475 6c65 2c20 6e65  odel, module, ne
-0000e290: 775f 6d6f 6475 6c65 2c0a 2020 2020 2020  w_module,.      
-0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2b0: 2020 2020 2020 2020 2020 2020 2073 7263               src
-0000e2c0: 5f66 7665 722c 2074 6774 5f66 7665 722c  _fver, tgt_fver,
-0000e2d0: 2074 7970 653d 7479 7029 0a20 2020 2020   type=typ).     
-0000e2e0: 2020 2069 6620 6861 7361 7474 7228 6170     if hasattr(ap
-0000e2f0: 7269 6f72 692c 2027 7265 6e61 6d65 645f  riori, 'renamed_
-0000e300: 6d6f 6465 6c73 2729 3a0a 2020 2020 2020  models'):.      
-0000e310: 2020 2020 2020 6d6f 6465 6c20 3d20 2769        model = 'i
-0000e320: 722e 6d6f 6465 6c27 0a20 2020 2020 2020  r.model'.       
-0000e330: 2020 2020 2074 7970 203d 2027 6d6f 6465       typ = 'mode
-0000e340: 6c27 0a20 2020 2020 2020 2020 2020 2066  l'.            f
-0000e350: 6f72 2069 7465 6d20 696e 2061 7072 696f  or item in aprio
-0000e360: 7269 2e72 656e 616d 6564 5f6d 6f64 656c  ri.renamed_model
-0000e370: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000e380: 2020 206d 6f64 756c 6520 3d20 6974 656d     module = item
-0000e390: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-0000e3a0: 2020 2020 6e65 775f 6d6f 6475 6c65 203d      new_module =
-0000e3b0: 2069 7465 6d5b 315d 0a20 2020 2020 2020   item[1].       
-0000e3c0: 2020 2020 2020 2020 2063 7478 203d 2061           ctx = a
-0000e3d0: 6464 5f74 6e6c 5f69 7465 6d28 6374 782c  dd_tnl_item(ctx,
-0000e3e0: 206d 6f64 656c 2c20 6d6f 6475 6c65 2c20   model, module, 
-0000e3f0: 6e65 775f 6d6f 6475 6c65 2c0a 2020 2020  new_module,.    
-0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e410: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e420: 7263 5f66 7665 722c 2074 6774 5f66 7665  rc_fver, tgt_fve
-0000e430: 722c 2074 7970 653d 7479 7029 0a20 2020  r, type=typ).   
-0000e440: 2020 2020 2074 7261 6e73 6f64 6f6f 2e77       transodoo.w
-0000e450: 7269 7465 5f73 746f 7265 645f 6469 6374  rite_stored_dict
-0000e460: 2863 7478 290a 2020 2020 2020 2020 6465  (ctx).        de
-0000e470: 6c20 7379 732e 7061 7468 5b2d 315d 0a20  l sys.path[-1]. 
-0000e480: 2020 2020 2020 2064 656c 2073 7973 2e70         del sys.p
-0000e490: 6174 685b 2d31 5d0a 0a0a 6465 6620 6164  ath[-1]...def ad
-0000e4a0: 6a75 7374 5f63 7478 2873 7263 5f63 7478  just_ctx(src_ctx
-0000e4b0: 2c20 7467 745f 6374 7829 3a0a 2020 2020  , tgt_ctx):.    
-0000e4c0: 666f 7220 6974 656d 2069 6e20 2827 6f64  for item in ('od
-0000e4d0: 6f6f 5f76 6572 272c 2027 6f64 6f6f 5f66  oo_ver', 'odoo_f
-0000e4e0: 7665 7227 2c20 2776 6964 272c 2027 636f  ver', 'vid', 'co
-0000e4f0: 6e66 5f66 6e27 2c20 2773 7663 5f70 726f  nf_fn', 'svc_pro
-0000e500: 746f 636f 6c27 2c0a 2020 2020 2020 2020  tocol',.        
-0000e510: 2020 2020 2020 2020 2027 6462 5f68 6f73           'db_hos
-0000e520: 7427 2c20 2764 625f 6e61 6d65 272c 2027  t', 'db_name', '
-0000e530: 6462 5f75 7365 7227 2c20 2764 625f 706f  db_user', 'db_po
-0000e540: 7274 272c 2027 6462 5f70 6173 7377 6f72  rt', 'db_passwor
-0000e550: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
-0000e560: 2020 2020 2027 6c65 7665 6c27 2c20 2027       'level',  '
-0000e570: 786d 6c72 7063 5f70 6f72 7427 2c20 2770  xmlrpc_port', 'p
-0000e580: 7379 636f 7067 3227 2c0a 2020 2020 2020  sycopg2',.      
-0000e590: 2020 2020 2020 2020 2020 2027 6c6f 6769             'logi
-0000e5a0: 6e5f 7573 6572 272c 2027 6c6f 6769 6e5f  n_user', 'login_
-0000e5b0: 7061 7373 776f 7264 272c 2027 6c6f 6766  password', 'logf
-0000e5c0: 696c 6527 2c20 2777 6974 686f 7574 5f64  ile', 'without_d
-0000e5d0: 656d 6f27 293a 0a20 2020 2020 2020 2073  emo'):.        s
-0000e5e0: 7263 5f70 6172 616d 203d 2027 7372 635f  rc_param = 'src_
-0000e5f0: 2573 2720 2520 6974 656d 0a20 2020 2020  %s' % item.     
-0000e600: 2020 2074 6774 5f70 6172 616d 203d 2027     tgt_param = '
-0000e610: 7467 745f 2573 2720 2520 6974 656d 0a20  tgt_%s' % item. 
-0000e620: 2020 2020 2020 2069 6620 6974 656d 203d         if item =
-0000e630: 3d20 276f 646f 6f5f 7665 7227 3a0a 2020  = 'odoo_ver':.  
-0000e640: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000e650: 2073 7263 5f63 7478 5b27 7365 6c5f 6d6f   src_ctx['sel_mo
-0000e660: 6465 6c27 5d3a 0a20 2020 2020 2020 2020  del']:.         
-0000e670: 2020 2020 2020 2074 6774 5f63 7478 5b74         tgt_ctx[t
-0000e680: 6774 5f70 6172 616d 5d20 3d20 7372 635f  gt_param] = src_
-0000e690: 6374 785b 7372 635f 7061 7261 6d5d 202b  ctx[src_param] +
-0000e6a0: 2031 0a20 2020 2020 2020 2065 6c69 6620   1.        elif 
-0000e6b0: 6974 656d 203d 3d20 276f 646f 6f5f 6676  item == 'odoo_fv
-0000e6c0: 6572 273a 0a20 2020 2020 2020 2020 2020  er':.           
-0000e6d0: 2069 6620 6e6f 7420 7372 635f 6374 785b   if not src_ctx[
-0000e6e0: 2773 656c 5f6d 6f64 656c 275d 3a0a 2020  'sel_model']:.  
-0000e6f0: 2020 2020 2020 2020 2020 2020 2020 7467                tg
-0000e700: 745f 6374 785b 7467 745f 7061 7261 6d5d  t_ctx[tgt_param]
-0000e710: 203d 2073 7263 5f63 7478 5b73 7263 5f70   = src_ctx[src_p
-0000e720: 6172 616d 5d2e 7265 706c 6163 6528 0a20  aram].replace(. 
-0000e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e740: 2020 2073 7472 2873 7263 5f63 7478 5b27     str(src_ctx['
-0000e750: 7372 635f 6f64 6f6f 5f76 6572 275d 292c  src_odoo_ver']),
-0000e760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e770: 2020 2020 2073 7472 2874 6774 5f63 7478       str(tgt_ctx
-0000e780: 5b27 7467 745f 6f64 6f6f 5f76 6572 275d  ['tgt_odoo_ver']
-0000e790: 2929 0a20 2020 2020 2020 2065 6c69 6620  )).        elif 
-0000e7a0: 6974 656d 203d 3d20 2776 6964 273a 0a20  item == 'vid':. 
-0000e7b0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0000e7c0: 7420 7372 635f 6374 785b 2773 656c 5f6d  t src_ctx['sel_m
-0000e7d0: 6f64 656c 275d 3a0a 2020 2020 2020 2020  odel']:.        
-0000e7e0: 2020 2020 2020 2020 7467 745f 6374 785b          tgt_ctx[
-0000e7f0: 7467 745f 7061 7261 6d5d 203d 2073 7263  tgt_param] = src
-0000e800: 5f63 7478 5b73 7263 5f70 6172 616d 5d2e  _ctx[src_param].
-0000e810: 7265 706c 6163 6528 0a20 2020 2020 2020  replace(.       
-0000e820: 2020 2020 2020 2020 2020 2020 2073 7472               str
-0000e830: 2873 7263 5f63 7478 5b27 7372 635f 6f64  (src_ctx['src_od
-0000e840: 6f6f 5f76 6572 275d 292c 0a20 2020 2020  oo_ver']),.     
-0000e850: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e860: 7472 2874 6774 5f63 7478 5b27 7467 745f  tr(tgt_ctx['tgt_
-0000e870: 6f64 6f6f 5f76 6572 275d 2929 0a20 2020  odoo_ver'])).   
-0000e880: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000e890: 7467 745f 6374 785b 7467 745f 7061 7261  tgt_ctx[tgt_para
-0000e8a0: 6d5d 2e73 7461 7274 7377 6974 6828 2776  m].startswith('v
-0000e8b0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-0000e8c0: 2020 2020 2020 2020 7467 745f 6374 785b          tgt_ctx[
-0000e8d0: 7467 745f 7061 7261 6d5d 203d 2074 6774  tgt_param] = tgt
-0000e8e0: 5f63 7478 5b27 7467 745f 6f64 6f6f 5f66  _ctx['tgt_odoo_f
-0000e8f0: 7665 7227 5d0a 2020 2020 2020 2020 2020  ver'].          
-0000e900: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000e910: 2020 2020 2020 2020 7467 745f 6374 785b          tgt_ctx[
-0000e920: 7467 745f 7061 7261 6d5d 203d 2074 6774  tgt_param] = tgt
-0000e930: 5f63 7478 5b27 6669 6e61 6c5f 6272 616e  _ctx['final_bran
-0000e940: 6368 275d 0a20 2020 2020 2020 2020 2020  ch'].           
-0000e950: 2020 2020 2074 6774 5f63 7478 5b27 7467       tgt_ctx['tg
-0000e960: 745f 6f64 6f6f 5f66 7665 7227 5d20 3d20  t_odoo_fver'] = 
-0000e970: 636c 6f64 6f6f 2e62 7569 6c64 5f6f 646f  clodoo.build_odo
-0000e980: 6f5f 7061 7261 6d28 0a20 2020 2020 2020  o_param(.       
-0000e990: 2020 2020 2020 2020 2020 2020 2027 4655               'FU
-0000e9a0: 4c4c 5645 5227 2c20 6f64 6f6f 5f76 6964  LLVER', odoo_vid
-0000e9b0: 3d74 6774 5f63 7478 5b27 6669 6e61 6c5f  =tgt_ctx['final_
-0000e9c0: 6272 616e 6368 275d 2c20 6d75 6c74 693d  branch'], multi=
-0000e9d0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-0000e9e0: 2020 2020 2020 7467 745f 6374 785b 2774        tgt_ctx['t
-0000e9f0: 6774 5f6f 646f 6f5f 7665 7227 5d20 3d20  gt_odoo_ver'] = 
-0000ea00: 636c 6f64 6f6f 2e62 7569 6c64 5f6f 646f  clodoo.build_odo
-0000ea10: 6f5f 7061 7261 6d28 0a20 2020 2020 2020  o_param(.       
-0000ea20: 2020 2020 2020 2020 2020 2020 2027 4d41               'MA
-0000ea30: 4a56 4552 272c 206f 646f 6f5f 7669 643d  JVER', odoo_vid=
-0000ea40: 7467 745f 6374 785b 2766 696e 616c 5f62  tgt_ctx['final_b
-0000ea50: 7261 6e63 6827 5d2c 206d 756c 7469 3d54  ranch'], multi=T
-0000ea60: 7275 6529 0a20 2020 2020 2020 2065 6c69  rue).        eli
-0000ea70: 6620 6974 656d 203d 3d20 2763 6f6e 665f  f item == 'conf_
-0000ea80: 666e 273a 0a20 2020 2020 2020 2020 2020  fn':.           
-0000ea90: 2073 7263 5f63 6f6e 6669 6720 3d20 6765   src_config = ge
-0000eaa0: 745f 636f 6e66 6967 5f66 6e73 2873 7263  t_config_fns(src
-0000eab0: 5f63 7478 2c20 2773 7263 2729 0a20 2020  _ctx, 'src').   
-0000eac0: 2020 2020 2020 2020 2074 6774 5f63 6f6e           tgt_con
-0000ead0: 6669 6720 3d20 6765 745f 636f 6e66 6967  fig = get_config
-0000eae0: 5f66 6e73 2874 6774 5f63 7478 2c20 2774  _fns(tgt_ctx, 't
-0000eaf0: 6774 2729 0a20 2020 2020 2020 2065 6c69  gt').        eli
-0000eb00: 6620 6974 656d 203d 3d20 2773 7663 5f70  f item == 'svc_p
-0000eb10: 726f 746f 636f 6c27 3a0a 2020 2020 2020  rotocol':.      
-0000eb20: 2020 2020 2020 7372 635f 6374 785b 2762        src_ctx['b
-0000eb30: 7261 6e63 6827 5d20 3d20 7372 635f 6374  ranch'] = src_ct
-0000eb40: 785b 2773 7263 5f6f 646f 6f5f 6676 6572  x['src_odoo_fver
-0000eb50: 275d 0a20 2020 2020 2020 2020 2020 2073  '].            s
-0000eb60: 7263 5f63 7478 5b27 6f65 5f76 6572 7369  rc_ctx['oe_versi
-0000eb70: 6f6e 275d 203d 2073 7263 5f63 7478 5b27  on'] = src_ctx['
-0000eb80: 7372 635f 6f64 6f6f 5f66 7665 7227 5d0a  src_odoo_fver'].
-0000eb90: 2020 2020 2020 2020 2020 2020 7372 635f              src_
-0000eba0: 636f 6e66 6967 2e73 6574 2827 6f70 7469  config.set('opti
-0000ebb0: 6f6e 7327 2c20 276f 655f 7665 7273 696f  ons', 'oe_versio
-0000ebc0: 6e27 2c20 7372 635f 6374 785b 276f 655f  n', src_ctx['oe_
-0000ebd0: 7665 7273 696f 6e27 5d29 0a20 2020 2020  version']).     
-0000ebe0: 2020 2020 2020 2069 6620 6e6f 7420 7372         if not sr
-0000ebf0: 635f 6374 782e 6765 7428 6974 656d 293a  c_ctx.get(item):
-0000ec00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ec10: 2069 6620 7372 635f 6374 785b 276f 655f   if src_ctx['oe_
-0000ec20: 7665 7273 696f 6e27 5d20 696e 2028 2736  version'] in ('6
-0000ec30: 2e31 272c 2027 372e 3027 2c20 2738 2e30  .1', '7.0', '8.0
-0000ec40: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-0000ec50: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-0000ec60: 2773 7663 5f70 726f 746f 636f 6c27 5d20  'svc_protocol'] 
-0000ec70: 3d20 2778 6d6c 7270 6327 0a20 2020 2020  = 'xmlrpc'.     
-0000ec80: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000ec90: 7372 635f 6374 785b 276f 655f 7665 7273  src_ctx['oe_vers
-0000eca0: 696f 6e27 5d3a 0a20 2020 2020 2020 2020  ion']:.         
-0000ecb0: 2020 2020 2020 2020 2020 2073 7263 5f63             src_c
-0000ecc0: 7478 5b27 7376 635f 7072 6f74 6f63 6f6c  tx['svc_protocol
-0000ecd0: 275d 203d 2027 6a73 6f6e 7270 6327 0a20  '] = 'jsonrpc'. 
-0000ece0: 2020 2020 2020 2020 2020 2074 6774 5f63             tgt_c
-0000ecf0: 7478 5b27 6272 616e 6368 275d 203d 2074  tx['branch'] = t
-0000ed00: 6774 5f63 7478 5b27 7467 745f 6f64 6f6f  gt_ctx['tgt_odoo
-0000ed10: 5f66 7665 7227 5d0a 2020 2020 2020 2020  _fver'].        
-0000ed20: 2020 2020 7467 745f 6374 785b 276f 655f      tgt_ctx['oe_
-0000ed30: 7665 7273 696f 6e27 5d20 3d20 7467 745f  version'] = tgt_
-0000ed40: 6374 785b 2774 6774 5f6f 646f 6f5f 6676  ctx['tgt_odoo_fv
-0000ed50: 6572 275d 0a20 2020 2020 2020 2020 2020  er'].           
-0000ed60: 2074 6774 5f63 6f6e 6669 672e 7365 7428   tgt_config.set(
-0000ed70: 276f 7074 696f 6e73 272c 2027 6f65 5f76  'options', 'oe_v
-0000ed80: 6572 7369 6f6e 272c 2074 6774 5f63 7478  ersion', tgt_ctx
-0000ed90: 5b27 6f65 5f76 6572 7369 6f6e 275d 290a  ['oe_version']).
-0000eda0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-0000edb0: 6774 5f63 7478 5b27 6f65 5f76 6572 7369  gt_ctx['oe_versi
-0000edc0: 6f6e 275d 2069 6e20 2827 362e 3127 2c20  on'] in ('6.1', 
-0000edd0: 2737 2e30 272c 2027 382e 3027 293a 0a20  '7.0', '8.0'):. 
-0000ede0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000edf0: 6774 5f63 7478 5b27 7376 635f 7072 6f74  gt_ctx['svc_prot
-0000ee00: 6f63 6f6c 275d 203d 2027 786d 6c72 7063  ocol'] = 'xmlrpc
-0000ee10: 270a 2020 2020 2020 2020 2020 2020 656c  '.            el
-0000ee20: 6966 2074 6774 5f63 7478 5b27 6f65 5f76  if tgt_ctx['oe_v
-0000ee30: 6572 7369 6f6e 275d 3a0a 2020 2020 2020  ersion']:.      
-0000ee40: 2020 2020 2020 2020 2020 7467 745f 6374            tgt_ct
-0000ee50: 785b 2773 7663 5f70 726f 746f 636f 6c27  x['svc_protocol'
-0000ee60: 5d20 3d20 276a 736f 6e72 7063 270a 2020  ] = 'jsonrpc'.  
-0000ee70: 2020 2020 2020 656c 6966 2069 7465 6d20        elif item 
-0000ee80: 3d3d 2027 6462 5f6e 616d 6527 3a0a 2020  == 'db_name':.  
-0000ee90: 2020 2020 2020 2020 2020 6966 2073 7263            if src
-0000eea0: 5f63 7478 5b27 7372 635f 7669 6427 5d20  _ctx['src_vid'] 
-0000eeb0: 3d3d 2073 7263 5f63 7478 5b27 6672 6f6d  == src_ctx['from
-0000eec0: 5f62 7261 6e63 6827 5d3a 0a20 2020 2020  _branch']:.     
-0000eed0: 2020 2020 2020 2020 2020 2073 7263 5f63             src_c
-0000eee0: 7478 5b69 7465 6d5d 203d 2073 7263 5f63  tx[item] = src_c
-0000eef0: 7478 5b73 7263 5f70 6172 616d 5d0a 2020  tx[src_param].  
-0000ef00: 2020 2020 2020 2020 2020 6966 2074 6774            if tgt
-0000ef10: 5f63 7478 5b27 7467 745f 6f64 6f6f 5f76  _ctx['tgt_odoo_v
-0000ef20: 6572 275d 203d 3d20 7467 745f 6374 785b  er'] == tgt_ctx[
-0000ef30: 2766 696e 616c 5f76 6572 275d 3a0a 2020  'final_ver']:.  
-0000ef40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000ef50: 2074 6774 5f63 7478 5b27 6669 6e61 6c5f   tgt_ctx['final_
-0000ef60: 6462 6e61 6d65 275d 3a0a 2020 2020 2020  dbname']:.      
-0000ef70: 2020 2020 2020 2020 2020 2020 2020 7467                tg
-0000ef80: 745f 6374 785b 6974 656d 5d20 3d20 7467  t_ctx[item] = tg
-0000ef90: 745f 6374 785b 2766 696e 616c 5f64 626e  t_ctx['final_dbn
-0000efa0: 616d 6527 5d0a 2020 2020 2020 2020 2020  ame'].          
-0000efb0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000efc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000efd0: 7467 745f 6374 785b 6974 656d 5d20 3d20  tgt_ctx[item] = 
-0000efe0: 6e65 775f 6462 6e61 6d65 2873 7263 5f63  new_dbname(src_c
-0000eff0: 7478 5b69 7465 6d5d 2c0a 2020 2020 2020  tx[item],.      
-0000f000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f020: 2020 2020 2020 2020 2074 6774 5f63 7478           tgt_ctx
-0000f030: 5b27 7467 745f 6f64 6f6f 5f76 6572 275d  ['tgt_odoo_ver']
-0000f040: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f070: 2074 6774 5f63 7478 5b27 6f63 615f 6d69   tgt_ctx['oca_mi
-0000f080: 6772 6174 6527 5d29 0a20 2020 2020 2020  grate']).       
-0000f090: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000f0a0: 2020 2020 2020 2020 2020 2074 6774 5f63             tgt_c
-0000f0b0: 7478 5b69 7465 6d5d 203d 206e 6577 5f64  tx[item] = new_d
-0000f0c0: 626e 616d 6528 7372 635f 6374 785b 6974  bname(src_ctx[it
-0000f0d0: 656d 5d2c 0a20 2020 2020 2020 2020 2020  em],.           
+00009b40: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
+00009b50: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00009b60: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00009b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b80: 6d6f 6465 6c73 5b6d 6f64 656c 5d5b 2773  models[model]['s
+00009b90: 7461 7475 7327 5d20 3d20 274f 4b27 0a20  tatus'] = 'OK'. 
+00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bb0: 2020 2065 6c69 6620 6d6f 6465 6c20 696e     elif model in
+00009bc0: 206d 6f64 656c 735b 7375 625d 5b27 6465   models[sub]['de
+00009bd0: 7065 6e64 7327 5d3a 0a20 2020 2020 2020  pends']:.       
+00009be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bf0: 206d 6f64 656c 735b 6d6f 6465 6c5d 5b27   models[model]['
+00009c00: 7374 6174 7573 275d 203d 2027 6372 6f73  status'] = 'cros
+00009c10: 7320 6465 702e 2077 6974 6820 2573 2720  s dep. with %s' 
+00009c20: 2520 7375 620a 2020 2020 2020 2020 2020  % sub.          
+00009c30: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+00009c40: 6465 6c73 5b73 7562 5d5b 2773 7461 7475  dels[sub]['statu
+00009c50: 7327 5d20 3d20 2763 726f 7373 2064 6570  s'] = 'cross dep
+00009c60: 2e20 7769 7468 2025 7327 2025 206d 6f64  . with %s' % mod
+00009c70: 656c 0a20 2020 2020 2020 2020 2020 2020  el.             
+00009c80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00009c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ca0: 2020 2020 2063 7572 5f6c 6576 656c 203d       cur_level =
+00009cb0: 202d 310a 2020 2020 2020 2020 2020 2020   -1.            
+00009cc0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+00009cd0: 6c73 5b6d 6f64 656c 5d5b 2773 7461 7475  ls[model]['statu
+00009ce0: 7327 5d20 3d20 2762 726f 6b65 6e20 6279  s'] = 'broken by
+00009cf0: 2025 7327 2025 2073 7562 0a20 2020 2020   %s' % sub.     
+00009d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d10: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00009d20: 2020 2020 2020 2020 2069 6620 6375 725f           if cur_
+00009d30: 6c65 7665 6c20 3e3d 204d 4158 5f44 4545  level >= MAX_DEE
+00009d40: 503a 0a20 2020 2020 2020 2020 2020 2020  P:.             
+00009d50: 2020 2020 2020 206d 6f64 656c 735b 6d6f         models[mo
+00009d60: 6465 6c5d 5b27 6c65 7665 6c27 5d20 3d20  del]['level'] = 
+00009d70: 4d41 585f 4445 4550 0a20 2020 2020 2020  MAX_DEEP.       
+00009d80: 2020 2020 2020 2020 2065 6c69 6620 6375           elif cu
+00009d90: 725f 6c65 7665 6c20 3e3d 2030 3a0a 2020  r_level >= 0:.  
+00009da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009db0: 2020 6d6f 6465 6c73 5b6d 6f64 656c 5d5b    models[model][
+00009dc0: 276c 6576 656c 275d 203d 2063 7572 5f6c  'level'] = cur_l
+00009dd0: 6576 656c 0a20 2020 2066 6f72 206d 6f64  evel.    for mod
+00009de0: 656c 2069 6e20 6d6f 6465 6c5f 6c69 7374  el in model_list
+00009df0: 3a0a 2020 2020 2020 2020 6966 2027 6c65  :.        if 'le
+00009e00: 7665 6c27 206e 6f74 2069 6e20 6d6f 6465  vel' not in mode
+00009e10: 6c73 5b6d 6f64 656c 5d3a 0a20 2020 2020  ls[model]:.     
+00009e20: 2020 2020 2020 206d 6f64 656c 735b 6d6f         models[mo
+00009e30: 6465 6c5d 5b27 6c65 7665 6c27 5d20 3d20  del]['level'] = 
+00009e40: 4d41 585f 4445 4550 202b 2031 0a20 2020  MAX_DEEP + 1.   
+00009e50: 2072 6574 7572 6e20 6d6f 6465 6c73 0a0a   return models..
+00009e60: 0a64 6566 2070 7269 6d6b 6579 5f74 6162  .def primkey_tab
+00009e70: 6c65 2863 7478 2c20 6d6f 6465 6c29 3a0a  le(ctx, model):.
+00009e80: 2020 2020 636c 6f64 6f6f 2e67 6574 5f6d      clodoo.get_m
+00009e90: 6f64 656c 5f73 7472 7563 7475 7265 280a  odel_structure(.
+00009ea0: 2020 2020 2020 2020 6374 782c 206d 6f64          ctx, mod
+00009eb0: 656c 2c20 6967 6e6f 7265 3d49 474e 4f52  el, ignore=IGNOR
+00009ec0: 455f 4649 454c 4453 2e67 6574 286d 6f64  E_FIELDS.get(mod
+00009ed0: 656c 2c20 5b5d 2920 2b20 4947 4e4f 5245  el, []) + IGNORE
+00009ee0: 5f46 4945 4c44 535b 272a 275d 0a20 2020  _FIELDS['*'].   
+00009ef0: 2029 0a20 2020 2069 725f 6d6f 6465 6c20   ).    ir_model 
+00009f00: 3d20 2769 722e 6d6f 6465 6c2e 636f 6e73  = 'ir.model.cons
+00009f10: 7472 6169 6e74 270a 2020 2020 6966 206d  traint'.    if m
+00009f20: 6f64 656c 2069 6e20 504b 4559 533a 0a20  odel in PKEYS:. 
+00009f30: 2020 2020 2020 206e 616d 6573 203d 2050         names = P
+00009f40: 4b45 5953 5b6d 6f64 656c 5d0a 2020 2020  KEYS[model].    
+00009f50: 656c 7365 3a0a 2020 2020 2020 2020 6e61  else:.        na
+00009f60: 6d65 7320 3d20 5b5d 0a20 2020 2020 2020  mes = [].       
+00009f70: 2070 7269 6f72 5f6e 616d 6520 3d20 2727   prior_name = ''
+00009f80: 0a20 2020 2020 2020 2066 6f72 2072 6563  .        for rec
+00009f90: 2069 6e20 636c 6f64 6f6f 2e62 726f 7773   in clodoo.brows
+00009fa0: 654c 3828 0a20 2020 2020 2020 2020 2020  eL8(.           
+00009fb0: 2063 7478 2c0a 2020 2020 2020 2020 2020   ctx,.          
+00009fc0: 2020 6972 5f6d 6f64 656c 2c0a 2020 2020    ir_model,.    
+00009fd0: 2020 2020 2020 2020 636c 6f64 6f6f 2e73          clodoo.s
+00009fe0: 6561 7263 684c 3828 0a20 2020 2020 2020  earchL8(.       
+00009ff0: 2020 2020 2020 2020 2063 7478 2c20 6972           ctx, ir
+0000a000: 5f6d 6f64 656c 2c20 5b28 276d 6f64 656c  _model, [('model
+0000a010: 272c 2027 3d27 2c20 6d6f 6465 6c29 2c20  ', '=', model), 
+0000a020: 2827 7479 7065 272c 2027 3d27 2c20 2775  ('type', '=', 'u
+0000a030: 2729 5d2c 206f 7264 6572 3d27 6e61 6d65  ')], order='name
+0000a040: 270a 2020 2020 2020 2020 2020 2020 292c  '.            ),
+0000a050: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
+0000a060: 2020 2020 2020 2020 6e61 6d65 203d 2072          name = r
+0000a070: 6563 2e6e 616d 650a 2020 2020 2020 2020  ec.name.        
+0000a080: 2020 2020 6966 206e 616d 6520 3d3d 2070      if name == p
+0000a090: 7269 6f72 5f6e 616d 653a 0a20 2020 2020  rior_name:.     
+0000a0a0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0000a0b0: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+0000a0c0: 7072 696f 725f 6e61 6d65 203d 206e 616d  prior_name = nam
+0000a0d0: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+0000a0e0: 2072 6563 2e6e 616d 652e 7374 6172 7473   rec.name.starts
+0000a0f0: 7769 7468 286d 6f64 656c 2e72 6570 6c61  with(model.repla
+0000a100: 6365 2827 2e27 2c20 275f 2729 293a 0a20  ce('.', '_')):. 
+0000a110: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000a120: 616d 6520 3d20 7265 632e 6e61 6d65 5b6c  ame = rec.name[l
+0000a130: 656e 286d 6f64 656c 2920 2b20 3120 3a5d  en(model) + 1 :]
+0000a140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a150: 2074 6f6b 5f69 6420 3d20 2727 0a20 2020   tok_id = ''.   
+0000a160: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000a170: 2074 6f6b 2069 6e20 6e61 6d65 2e73 706c   tok in name.spl
+0000a180: 6974 2827 5f27 293a 0a20 2020 2020 2020  it('_'):.       
+0000a190: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000a1a0: 746f 6b20 3d3d 2027 6964 273a 0a20 2020  tok == 'id':.   
+0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1c0: 2020 2020 2074 6f6b 5f69 6420 2b3d 2027       tok_id += '
+0000a1d0: 5f69 6427 0a20 2020 2020 2020 2020 2020  _id'.           
+0000a1e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000a1f0: 746f 6b5f 6964 2069 6e20 6374 785b 2753  tok_id in ctx['S
+0000a200: 5452 5543 5427 5d5b 6d6f 6465 6c5d 3a0a  TRUCT'][model]:.
+0000a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a220: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0000a230: 732e 6170 7065 6e64 2874 6f6b 5f69 6429  s.append(tok_id)
+0000a240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a250: 2020 2020 2020 2020 2020 2020 2074 6f6b               tok
+0000a260: 5f69 6420 3d20 2727 0a20 2020 2020 2020  _id = ''.       
+0000a270: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+0000a280: 6620 746f 6b20 696e 2063 7478 5b27 5354  f tok in ctx['ST
+0000a290: 5255 4354 275d 5b6d 6f64 656c 5d3a 0a20  RUCT'][model]:. 
+0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2b0: 2020 2020 2020 206e 616d 6573 2e61 7070         names.app
+0000a2c0: 656e 6428 746f 6b29 0a20 2020 2020 2020  end(tok).       
+0000a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2e0: 2074 6f6b 5f69 6420 3d20 2727 0a20 2020   tok_id = ''.   
+0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a300: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000a310: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000a320: 6f6b 5f69 6420 3d20 746f 6b0a 2020 2020  ok_id = tok.    
+0000a330: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0000a340: 7320 3d20 6e61 6d65 730a 2020 2020 2020  s = names.      
+0000a350: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+0000a360: 2020 2020 6966 206e 6f74 206e 616d 6573      if not names
+0000a370: 3a0a 2020 2020 2020 2020 6966 2063 6c6f  :.        if clo
+0000a380: 646f 6f2e 6973 5f76 616c 6964 5f66 6965  doo.is_valid_fie
+0000a390: 6c64 2863 7478 2c20 6d6f 6465 6c2c 2027  ld(ctx, model, '
+0000a3a0: 636f 6d70 616e 795f 6964 2729 3a0a 2020  company_id'):.  
+0000a3b0: 2020 2020 2020 2020 2020 6e61 6d65 7320            names 
+0000a3c0: 3d20 5b27 636f 6d70 616e 795f 6964 275d  = ['company_id']
+0000a3d0: 0a20 2020 2020 2020 2069 6620 636c 6f64  .        if clod
+0000a3e0: 6f6f 2e69 735f 7661 6c69 645f 6669 656c  oo.is_valid_fiel
+0000a3f0: 6428 6374 782c 206d 6f64 656c 2c20 2763  d(ctx, model, 'c
+0000a400: 6f64 6527 293a 0a20 2020 2020 2020 2020  ode'):.         
+0000a410: 2020 206e 616d 6573 2e61 7070 656e 6428     names.append(
+0000a420: 2763 6f64 6527 290a 2020 2020 2020 2020  'code').        
+0000a430: 656c 6966 2063 6c6f 646f 6f2e 6973 5f76  elif clodoo.is_v
+0000a440: 616c 6964 5f66 6965 6c64 2863 7478 2c20  alid_field(ctx, 
+0000a450: 6d6f 6465 6c2c 2027 6e61 6d65 2729 3a0a  model, 'name'):.
+0000a460: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0000a470: 732e 6170 7065 6e64 2827 6e61 6d65 2729  s.append('name')
+0000a480: 0a20 2020 2020 2020 206e 616d 6573 203d  .        names =
+0000a490: 206e 616d 6573 0a20 2020 2072 6574 7572   names.    retur
+0000a4a0: 6e20 6e61 6d65 730a 0a0a 6465 6620 7772  n names...def wr
+0000a4b0: 6974 655f 7472 6565 5f63 6f6e 6628 6374  ite_tree_conf(ct
+0000a4c0: 7829 3a0a 2020 2020 7072 696e 7428 2741  x):.    print('A
+0000a4d0: 6e61 6c69 7a69 6e67 2073 6f75 7263 6520  nalizing source 
+0000a4e0: 6d6f 6465 6c73 202e 2e2e 2729 0a20 2020  models ...').   
+0000a4f0: 206d 6f64 656c 7320 3d20 6275 696c 645f   models = build_
+0000a500: 7461 626c 655f 7472 6565 2863 7478 290a  table_tree(ctx).
+0000a510: 2020 2020 7769 7468 206f 7065 6e28 6374      with open(ct
+0000a520: 785b 2763 6f6d 6d61 6e64 5f66 696c 6527  x['command_file'
+0000a530: 5d2c 2027 7727 2920 6173 2066 643a 0a20  ], 'w') as fd:. 
+0000a540: 2020 2020 2020 2066 6f72 206c 6576 656c         for level
+0000a550: 2069 6e20 7261 6e67 6528 4d41 585f 4445   in range(MAX_DE
+0000a560: 4550 293a 0a20 2020 2020 2020 2020 2020  EP):.           
+0000a570: 2066 6f72 206d 6f64 656c 2069 6e20 6d6f   for model in mo
+0000a580: 6465 6c73 3a0a 2020 2020 2020 2020 2020  dels:.          
+0000a590: 2020 2020 2020 6d73 675f 6275 7273 7428        msg_burst(
+0000a5a0: 2720 2020 206b 6579 7320 2573 202e 2e2e  '    keys %s ...
+0000a5b0: 2720 2520 6d6f 6465 6c29 0a20 2020 2020  ' % model).     
+0000a5c0: 2020 2020 2020 2020 2020 206e 616d 6573             names
+0000a5d0: 203d 2070 7269 6d6b 6579 5f74 6162 6c65   = primkey_table
+0000a5e0: 2863 7478 2c20 6d6f 6465 6c29 0a20 2020  (ctx, model).   
+0000a5f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000a600: 6d6f 6465 6c73 5b6d 6f64 656c 5d2e 6765  models[model].ge
+0000a610: 7428 276c 6576 656c 272c 202d 3129 203d  t('level', -1) =
+0000a620: 3d20 6c65 7665 6c3a 0a20 2020 2020 2020  = level:.       
+0000a630: 2020 2020 2020 2020 2020 2020 2066 642e               fd.
+0000a640: 7772 6974 6528 2725 645c 7425 735c 7469  write('%d\t%s\ti
+0000a650: 6e71 7569 7265 5c74 2573 5c6e 2720 2520  nquire\t%s\n' % 
+0000a660: 286c 6576 656c 2c20 6d6f 6465 6c2c 206e  (level, model, n
+0000a670: 616d 6573 2929 0a20 2020 2020 2020 2066  ames)).        f
+0000a680: 6f72 206d 6f64 656c 2069 6e20 6d6f 6465  or model in mode
+0000a690: 6c73 3a0a 2020 2020 2020 2020 2020 2020  ls:.            
+0000a6a0: 6d73 675f 6275 7273 7428 2720 2020 206b  msg_burst('    k
+0000a6b0: 6579 7320 2573 202e 2e2e 2720 2520 6d6f  eys %s ...' % mo
+0000a6c0: 6465 6c29 0a20 2020 2020 2020 2020 2020  del).           
+0000a6d0: 2069 6620 6d6f 6465 6c73 5b6d 6f64 656c   if models[model
+0000a6e0: 5d2e 6765 7428 276c 6576 656c 272c 202d  ].get('level', -
+0000a6f0: 3129 203e 3d20 4d41 585f 4445 4550 3a0a  1) >= MAX_DEEP:.
+0000a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a710: 6e61 6d65 7320 3d20 7072 696d 6b65 795f  names = primkey_
+0000a720: 7461 626c 6528 6374 782c 206d 6f64 656c  table(ctx, model
+0000a730: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a740: 2020 6664 2e77 7269 7465 2827 2564 5c74    fd.write('%d\t
+0000a750: 2573 5c74 696e 7175 6972 655c 7425 735c  %s\tinquire\t%s\
+0000a760: 6e27 2025 2028 6c65 7665 6c2c 206d 6f64  n' % (level, mod
+0000a770: 656c 2c20 6e61 6d65 7329 290a 0a0a 6465  el, names))...de
+0000a780: 6620 6765 745f 6d6f 6465 6c5f 636f 7079  f get_model_copy
+0000a790: 5f6d 6f64 6528 6374 782c 206d 6f64 656c  _mode(ctx, model
+0000a7a0: 293a 0a20 2020 2069 6620 6973 5f73 7973  ):.    if is_sys
+0000a7b0: 7465 6d5f 6d6f 6465 6c28 6d6f 6465 6c29  tem_model(model)
+0000a7c0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0000a7d0: 2027 4e6f 270a 2020 2020 6d6f 6465 203d   'No'.    mode =
+0000a7e0: 2063 7478 5b27 5f6d 6c27 5d2e 6765 7428   ctx['_ml'].get(
+0000a7f0: 6d6f 6465 6c29 206f 7220 2769 6e71 7569  model) or 'inqui
+0000a800: 7265 270a 2020 2020 6966 2063 7478 5b27  re'.    if ctx['
+0000a810: 696d 6167 655f 6d6f 6465 275d 3a0a 2020  image_mode']:.  
+0000a820: 2020 2020 2020 6d6f 6465 203d 2027 696d        mode = 'im
+0000a830: 6167 6527 0a20 2020 2065 6c69 6620 6d6f  age'.    elif mo
+0000a840: 6465 6c20 696e 2028 0a20 2020 2020 2020  del in (.       
+0000a850: 2027 6163 636f 756e 742e 6163 636f 756e   'account.accoun
+0000a860: 7427 2c0a 2020 2020 2020 2020 2761 6363  t',.        'acc
+0000a870: 6f75 6e74 2e61 6363 6f75 6e74 2e74 7970  ount.account.typ
+0000a880: 6527 2c0a 2020 2020 2020 2020 2761 6363  e',.        'acc
+0000a890: 6f75 6e74 2e74 6178 272c 0a20 2020 2020  ount.tax',.     
+0000a8a0: 2020 2027 7072 6f64 7563 742e 7072 6f64     'product.prod
+0000a8b0: 7563 7427 2c0a 2020 2020 2020 2020 2770  uct',.        'p
+0000a8c0: 726f 6475 6374 2e74 656d 706c 6174 6527  roduct.template'
+0000a8d0: 2c0a 2020 2020 2020 2020 2772 6573 2e70  ,.        'res.p
+0000a8e0: 6172 746e 6572 272c 0a20 2020 2029 3a0a  artner',.    ):.
+0000a8f0: 2020 2020 2020 2020 6d6f 6465 203d 2027          mode = '
+0000a900: 7371 6c27 0a20 2020 2069 6620 6d6f 6465  sql'.    if mode
+0000a910: 203d 3d20 2769 6e71 7569 7265 273a 0a20   == 'inquire':. 
+0000a920: 2020 2020 2020 206d 6f64 655f 7365 6c65         mode_sele
+0000a930: 6374 696f 6e20 3d20 7b27 6927 3a20 2769  ction = {'i': 'i
+0000a940: 6d61 6765 272c 2027 7327 3a20 2773 716c  mage', 's': 'sql
+0000a950: 272c 2027 6e27 3a20 276e 6f27 7d0a 2020  ', 'n': 'no'}.  
+0000a960: 2020 2020 2020 6475 6d6d 7920 3d20 2727        dummy = ''
+0000a970: 0a20 2020 2020 2020 2077 6869 6c65 206e  .        while n
+0000a980: 6f74 2064 756d 6d79 3a0a 2020 2020 2020  ot dummy:.      
+0000a990: 2020 2020 2020 6966 2063 7478 5b27 7365        if ctx['se
+0000a9a0: 6c5f 6d6f 6465 6c27 5d3a 0a20 2020 2020  l_model']:.     
+0000a9b0: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+0000a9c0: 6465 6c20 696e 2063 7478 5b27 7365 6c5f  del in ctx['sel_
+0000a9d0: 6d6f 6465 6c27 5d3a 0a20 2020 2020 2020  model']:.       
+0000a9e0: 2020 2020 2020 2020 2020 2020 2064 756d               dum
+0000a9f0: 6d79 203d 2027 5327 0a20 2020 2020 2020  my = 'S'.       
+0000aa00: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa20: 2020 2064 756d 6d79 203d 2027 4e27 0a20     dummy = 'N'. 
+0000aa30: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000aa40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aa50: 2064 756d 6d79 203d 2069 6e70 7574 2827   dummy = input('
+0000aa60: 436f 7079 2074 6162 6c65 2025 7320 2849  Copy table %s (I
+0000aa70: 6d61 6765 2c53 716c 2c4e 6f29 3f20 2720  mage,Sql,No)? ' 
+0000aa80: 2520 6d6f 6465 6c29 0a20 2020 2020 2020  % model).       
+0000aa90: 2020 2020 2069 6620 6475 6d6d 7920 616e       if dummy an
+0000aaa0: 6420 6475 6d6d 795b 305d 2e6c 6f77 6572  d dummy[0].lower
+0000aab0: 2829 2069 6e20 6d6f 6465 5f73 656c 6563  () in mode_selec
+0000aac0: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+0000aad0: 2020 2020 2020 6d6f 6465 203d 206d 6f64        mode = mod
+0000aae0: 655f 7365 6c65 6374 696f 6e5b 6475 6d6d  e_selection[dumm
+0000aaf0: 795b 305d 2e6c 6f77 6572 2829 5d0a 2020  y[0].lower()].  
+0000ab00: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab20: 6475 6d6d 7920 3d20 2727 0a20 2020 2020  dummy = ''.     
+0000ab30: 2020 2063 7478 5b27 5f6d 6c27 5d5b 6d6f     ctx['_ml'][mo
+0000ab40: 6465 6c5d 203d 206d 6f64 650a 2020 2020  del] = mode.    
+0000ab50: 7265 7475 726e 206d 6f64 650a 0a0a 6465  return mode...de
+0000ab60: 6620 6d69 6772 6174 655f 7365 6c5f 7461  f migrate_sel_ta
+0000ab70: 626c 6573 2873 7263 5f63 7478 2c20 7467  bles(src_ctx, tg
+0000ab80: 745f 6374 7829 3a0a 2020 2020 7372 635f  t_ctx):.    src_
+0000ab90: 6374 7820 3d20 696e 6974 5f63 7478 2873  ctx = init_ctx(s
+0000aba0: 7263 5f63 7478 290a 2020 2020 696d 706f  rc_ctx).    impo
+0000abb0: 7274 2070 6462 0a0a 2020 2020 7064 622e  rt pdb..    pdb.
+0000abc0: 7365 745f 7472 6163 6528 290a 2020 2020  set_trace().    
+0000abd0: 7372 635f 6374 782c 2074 6774 5f63 7478  src_ctx, tgt_ctx
+0000abe0: 2c20 7372 635f 636f 6e66 6967 2c20 7467  , src_config, tg
+0000abf0: 745f 636f 6e66 6967 203d 2061 646a 7573  t_config = adjus
+0000ac00: 745f 6374 7828 7372 635f 6374 782c 2074  t_ctx(src_ctx, t
+0000ac10: 6774 5f63 7478 290a 2020 2020 7569 642c  gt_ctx).    uid,
+0000ac20: 2073 7263 5f63 7478 203d 2063 6c6f 646f   src_ctx = clodo
+0000ac30: 6f2e 6f65 7270 5f73 6574 5f65 6e76 2863  o.oerp_set_env(c
+0000ac40: 7478 3d73 7263 5f63 7478 290a 2020 2020  tx=src_ctx).    
+0000ac50: 2320 4649 5820 6f65 7270 5f73 6574 5f65  # FIX oerp_set_e
+0000ac60: 6e76 2063 6861 6e67 6520 6472 795f 7275  nv change dry_ru
+0000ac70: 6e0a 2020 2020 7372 635f 6374 785b 2764  n.    src_ctx['d
+0000ac80: 7279 5f72 756e 275d 203d 2074 6774 5f63  ry_run'] = tgt_c
+0000ac90: 7478 5b27 6472 795f 7275 6e27 5d0a 2020  tx['dry_run'].  
+0000aca0: 2020 7569 642c 2074 6774 5f63 7478 203d    uid, tgt_ctx =
+0000acb0: 2063 6c6f 646f 6f2e 6f65 7270 5f73 6574   clodoo.oerp_set
+0000acc0: 5f65 6e76 2863 7478 3d74 6774 5f63 7478  _env(ctx=tgt_ctx
+0000acd0: 290a 2020 2020 2320 4649 5820 6f65 7270  ).    # FIX oerp
+0000ace0: 5f73 6574 5f65 6e76 2063 6861 6e67 6520  _set_env change 
+0000acf0: 6472 795f 7275 6e0a 2020 2020 7467 745f  dry_run.    tgt_
+0000ad00: 6374 785b 2764 7279 5f72 756e 275d 203d  ctx['dry_run'] =
+0000ad10: 2073 7263 5f63 7478 5b27 6472 795f 7275   src_ctx['dry_ru
+0000ad20: 6e27 5d0a 2020 2020 7472 616e 736f 646f  n'].    transodo
+0000ad30: 6f2e 7265 6164 5f73 746f 7265 645f 6469  o.read_stored_di
+0000ad40: 6374 2873 7263 5f63 7478 290a 2020 2020  ct(src_ctx).    
+0000ad50: 7467 745f 6374 785b 276d 696e 6472 6f6f  tgt_ctx['mindroo
+0000ad60: 7427 5d20 3d20 7372 635f 6374 785b 276d  t'] = src_ctx['m
+0000ad70: 696e 6472 6f6f 7427 5d0a 2020 2020 6966  indroot'].    if
+0000ad80: 206e 6f74 2074 6774 5f63 7478 5b27 7365   not tgt_ctx['se
+0000ad90: 6c5f 6d6f 6465 6c27 5d3a 0a20 2020 2020  l_model']:.     
+0000ada0: 2020 2069 6e73 7461 6c6c 5f6d 6f64 756c     install_modul
+0000adb0: 6573 2874 6774 5f63 7478 2c20 7372 635f  es(tgt_ctx, src_
+0000adc0: 6374 7829 0a0a 2020 2020 6966 2073 7263  ctx)..    if src
+0000add0: 5f63 7478 5b27 6465 6661 756c 745f 6265  _ctx['default_be
+0000ade0: 6861 7669 6f72 275d 206f 7220 6e6f 7420  havior'] or not 
+0000adf0: 6f73 2e70 6174 682e 6973 6669 6c65 2873  os.path.isfile(s
+0000ae00: 7263 5f63 7478 5b27 636f 6d6d 616e 645f  rc_ctx['command_
+0000ae10: 6669 6c65 275d 293a 0a20 2020 2020 2020  file']):.       
+0000ae20: 2077 7269 7465 5f74 7265 655f 636f 6e66   write_tree_conf
+0000ae30: 2873 7263 5f63 7478 290a 0a20 2020 2077  (src_ctx)..    w
+0000ae40: 6974 6820 6f70 656e 2874 6774 5f63 7478  ith open(tgt_ctx
+0000ae50: 5b27 636f 6d6d 616e 645f 6669 6c65 275d  ['command_file']
+0000ae60: 2c20 2772 2729 2061 7320 6664 3a0a 2020  , 'r') as fd:.  
+0000ae70: 2020 2020 2020 7467 745f 6374 785b 275f        tgt_ctx['_
+0000ae80: 6d6c 275d 203d 207b 7d0a 2020 2020 2020  ml'] = {}.      
+0000ae90: 2020 7467 745f 6374 785b 275f 6b6c 275d    tgt_ctx['_kl']
+0000aea0: 203d 207b 7d0a 2020 2020 2020 2020 7467   = {}.        tg
+0000aeb0: 745f 6374 785b 276d 6f64 656c 5f6c 6973  t_ctx['model_lis
+0000aec0: 7427 5d20 3d20 5b5d 0a20 2020 2020 2020  t'] = [].       
+0000aed0: 2066 6f72 206c 696e 6520 696e 2066 642e   for line in fd.
+0000aee0: 7265 6164 2829 2e73 706c 6974 2827 5c6e  read().split('\n
+0000aef0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+0000af00: 6c69 6e65 203d 206c 696e 652e 7374 7269  line = line.stri
+0000af10: 7028 290a 2020 2020 2020 2020 2020 2020  p().            
+0000af20: 6966 206c 696e 653a 0a20 2020 2020 2020  if line:.       
+0000af30: 2020 2020 2020 2020 206c 696e 6573 203d           lines =
+0000af40: 206c 696e 652e 7370 6c69 7428 275c 7427   line.split('\t'
+0000af50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000af60: 2020 6c65 7665 6c20 3d20 6c69 6e65 735b    level = lines[
+0000af70: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+0000af80: 2020 206d 6f64 656c 203d 206c 696e 6573     model = lines
+0000af90: 5b31 5d0a 2020 2020 2020 2020 2020 2020  [1].            
+0000afa0: 2020 2020 6d6f 6465 203d 2027 696e 7175      mode = 'inqu
+0000afb0: 6972 6527 2069 6620 6c65 6e28 6c69 6e65  ire' if len(line
+0000afc0: 735b 315d 2920 3c3d 2032 2065 6c73 6520  s[1]) <= 2 else 
+0000afd0: 6c69 6e65 735b 325d 0a20 2020 2020 2020  lines[2].       
+0000afe0: 2020 2020 2020 2020 206b 6579 7320 3d20           keys = 
+0000aff0: 276e 616d 6527 2069 6620 6c65 6e28 6c69  'name' if len(li
+0000b000: 6e65 7329 203c 3d20 3320 656c 7365 2065  nes) <= 3 else e
+0000b010: 7661 6c28 6c69 6e65 735b 335d 290a 2020  val(lines[3]).  
+0000b020: 2020 2020 2020 2020 2020 2020 2020 7467                tg
+0000b030: 745f 6374 785b 276d 6f64 656c 5f6c 6973  t_ctx['model_lis
+0000b040: 7427 5d2e 6170 7065 6e64 286d 6f64 656c  t'].append(model
+0000b050: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000b060: 2020 7467 745f 6374 785b 275f 6d6c 275d    tgt_ctx['_ml']
+0000b070: 5b6d 6f64 656c 5d20 3d20 6d6f 6465 0a20  [model] = mode. 
+0000b080: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000b090: 6620 6d6f 6465 6c20 696e 2050 4b45 5953  f model in PKEYS
+0000b0a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b0b0: 2020 2020 2020 7467 745f 6374 785b 275f        tgt_ctx['_
+0000b0c0: 6b6c 275d 5b6d 6f64 656c 5d20 3d20 504b  kl'][model] = PK
+0000b0d0: 4559 535b 6d6f 6465 6c5d 0a20 2020 2020  EYS[model].     
+0000b0e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000b0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b100: 2020 2020 2074 6774 5f63 7478 5b27 5f6b       tgt_ctx['_k
+0000b110: 6c27 5d5b 6d6f 6465 6c5d 203d 206b 6579  l'][model] = key
+0000b120: 730a 2020 2020 2020 2020 6664 2e63 6c6f  s.        fd.clo
+0000b130: 7365 2829 0a20 2020 2061 7373 756d 655f  se().    assume_
+0000b140: 7965 7320 3d20 2759 2720 6966 2074 6774  yes = 'Y' if tgt
+0000b150: 5f63 7478 5b27 6173 7375 6d65 5f79 6573  _ctx['assume_yes
+0000b160: 275d 2065 6c73 6520 2751 270a 2020 2020  '] else 'Q'.    
+0000b170: 6966 2074 6774 5f63 7478 5b27 7365 6c5f  if tgt_ctx['sel_
+0000b180: 6d6f 6465 6c27 5d3a 0a20 2020 2020 2020  model']:.       
+0000b190: 2074 6774 5f63 7478 5b27 6d6f 6465 6c5f   tgt_ctx['model_
+0000b1a0: 6c69 7374 275d 203d 2074 6774 5f63 7478  list'] = tgt_ctx
+0000b1b0: 5b27 7365 6c5f 6d6f 6465 6c27 5d2e 7370  ['sel_model'].sp
+0000b1c0: 6c69 7428 272c 2729 0a20 2020 2066 6f72  lit(',').    for
+0000b1d0: 206d 6f64 656c 2069 6e20 7467 745f 6374   model in tgt_ct
+0000b1e0: 785b 276d 6f64 656c 5f6c 6973 7427 5d3a  x['model_list']:
+0000b1f0: 0a20 2020 2020 2020 206d 6f64 6520 3d20  .        mode = 
+0000b200: 6765 745f 6d6f 6465 6c5f 636f 7079 5f6d  get_model_copy_m
+0000b210: 6f64 6528 7467 745f 6374 782c 206d 6f64  ode(tgt_ctx, mod
+0000b220: 656c 290a 2020 2020 2020 2020 6966 206d  el).        if m
+0000b230: 6f64 6520 6e6f 7420 696e 2028 2773 716c  ode not in ('sql
+0000b240: 272c 2027 696d 6167 6527 293a 0a20 2020  ', 'image'):.   
+0000b250: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+0000b260: 650a 2020 2020 2020 2020 636f 7079 5f74  e.        copy_t
+0000b270: 6162 6c65 2874 6774 5f63 7478 2c20 7372  able(tgt_ctx, sr
+0000b280: 635f 6374 782c 206d 6f64 656c 2c20 6d6f  c_ctx, model, mo
+0000b290: 6465 3d6d 6f64 6529 0a0a 0a64 6566 2069  de=mode)...def i
+0000b2a0: 6e69 745f 6374 7828 7372 635f 6374 7829  nit_ctx(src_ctx)
+0000b2b0: 3a0a 2020 2020 7372 635f 6374 785b 2773  :.    src_ctx['s
+0000b2c0: 7263 5f76 6964 275d 203d 2073 7263 5f63  rc_vid'] = src_c
+0000b2d0: 7478 5b27 6672 6f6d 5f62 7261 6e63 6827  tx['from_branch'
+0000b2e0: 5d0a 2020 2020 7372 635f 6374 785b 2773  ].    src_ctx['s
+0000b2f0: 7263 5f6f 646f 6f5f 6676 6572 275d 203d  rc_odoo_fver'] =
+0000b300: 2063 6c6f 646f 6f2e 6275 696c 645f 6f64   clodoo.build_od
+0000b310: 6f6f 5f70 6172 616d 280a 2020 2020 2020  oo_param(.      
+0000b320: 2020 2746 554c 4c56 4552 272c 206f 646f    'FULLVER', odo
+0000b330: 6f5f 7669 643d 7372 635f 6374 785b 2766  o_vid=src_ctx['f
+0000b340: 726f 6d5f 6272 616e 6368 275d 2c20 6d75  rom_branch'], mu
+0000b350: 6c74 693d 5472 7565 0a20 2020 2029 0a20  lti=True.    ). 
+0000b360: 2020 2073 7263 5f63 7478 5b27 6672 6f6d     src_ctx['from
+0000b370: 5f6f 646f 6f5f 6676 6572 275d 203d 2073  _odoo_fver'] = s
+0000b380: 7263 5f63 7478 5b27 7372 635f 6f64 6f6f  rc_ctx['src_odoo
+0000b390: 5f66 7665 7227 5d0a 2020 2020 7372 635f  _fver'].    src_
+0000b3a0: 6374 785b 2773 7263 5f6f 646f 6f5f 7665  ctx['src_odoo_ve
+0000b3b0: 7227 5d20 3d20 636c 6f64 6f6f 2e62 7569  r'] = clodoo.bui
+0000b3c0: 6c64 5f6f 646f 6f5f 7061 7261 6d28 0a20  ld_odoo_param(. 
+0000b3d0: 2020 2020 2020 2027 4d41 4a56 4552 272c         'MAJVER',
+0000b3e0: 206f 646f 6f5f 7669 643d 7372 635f 6374   odoo_vid=src_ct
+0000b3f0: 785b 2766 726f 6d5f 6272 616e 6368 275d  x['from_branch']
+0000b400: 2c20 6d75 6c74 693d 5472 7565 0a20 2020  , multi=True.   
+0000b410: 2029 0a20 2020 2073 7263 5f63 7478 5b27   ).    src_ctx['
+0000b420: 7372 635f 636f 6e66 5f66 6e27 5d20 3d20  src_conf_fn'] = 
+0000b430: 7372 635f 6374 785b 2766 726f 6d5f 636f  src_ctx['from_co
+0000b440: 6e66 6e27 5d0a 2020 2020 7372 635f 6374  nfn'].    src_ct
+0000b450: 785b 2773 7263 5f64 625f 6e61 6d65 275d  x['src_db_name']
+0000b460: 203d 2073 7263 5f63 7478 5b27 6672 6f6d   = src_ctx['from
+0000b470: 5f64 626e 616d 6527 5d0a 2020 2020 7265  _dbname'].    re
+0000b480: 7475 726e 2073 7263 5f63 7478 0a0a 0a64  turn src_ctx...d
+0000b490: 6566 2067 6574 5f63 6f6e 6669 675f 666e  ef get_config_fn
+0000b4a0: 7328 6374 782c 2073 7263 5f74 6774 293a  s(ctx, src_tgt):
+0000b4b0: 0a20 2020 2069 6620 7372 635f 7467 7420  .    if src_tgt 
+0000b4c0: 6e6f 7420 696e 2028 2773 7263 272c 2027  not in ('src', '
+0000b4d0: 7467 7427 293a 0a20 2020 2020 2020 2072  tgt'):.        r
+0000b4e0: 6169 7365 2028 2749 6e76 616c 6964 2070  aise ('Invalid p
+0000b4f0: 6172 616d 6574 6572 2073 7263 2f74 6774  arameter src/tgt
+0000b500: 2729 0a20 2020 2069 7465 6d20 3d20 2763  ').    item = 'c
+0000b510: 6f6e 665f 666e 270a 2020 2020 6f64 6f6f  onf_fn'.    odoo
+0000b520: 5f63 6f6e 666e 203d 2063 6c6f 646f 6f2e  _confn = clodoo.
+0000b530: 6275 696c 645f 6f64 6f6f 5f70 6172 616d  build_odoo_param
+0000b540: 280a 2020 2020 2020 2020 2743 4f4e 464e  (.        'CONFN
+0000b550: 272c 206f 646f 6f5f 7669 643d 6374 785b  ', odoo_vid=ctx[
+0000b560: 2725 735f 7669 6427 2025 2073 7263 5f74  '%s_vid' % src_t
+0000b570: 6774 5d2c 206d 756c 7469 3d54 7275 650a  gt], multi=True.
+0000b580: 2020 2020 290a 2020 2020 6966 2073 7263      ).    if src
+0000b590: 5f74 6774 203d 3d20 2773 7263 2720 616e  _tgt == 'src' an
+0000b5a0: 6420 6374 785b 2725 735f 7669 6427 2025  d ctx['%s_vid' %
+0000b5b0: 2073 7263 5f74 6774 5d20 3d3d 2063 7478   src_tgt] == ctx
+0000b5c0: 5b27 6672 6f6d 5f62 7261 6e63 6827 5d3a  ['from_branch']:
+0000b5d0: 0a20 2020 2020 2020 2063 7478 5b69 7465  .        ctx[ite
+0000b5e0: 6d5d 203d 2063 7478 5b27 7372 635f 2573  m] = ctx['src_%s
+0000b5f0: 2720 2520 6974 656d 5d0a 2020 2020 2020  ' % item].      
+0000b600: 2020 6966 206e 6f74 206f 732e 7061 7468    if not os.path
+0000b610: 2e69 7366 696c 6528 6f64 6f6f 5f63 6f6e  .isfile(odoo_con
+0000b620: 666e 293a 0a20 2020 2020 2020 2020 2020  fn):.           
+0000b630: 206f 646f 6f5f 636f 6e66 6e20 3d20 4661   odoo_confn = Fa
+0000b640: 6c73 650a 2020 2020 656c 6966 2073 7263  lse.    elif src
+0000b650: 5f74 6774 203d 3d20 2774 6774 2720 616e  _tgt == 'tgt' an
+0000b660: 6420 6374 785b 2725 735f 6f64 6f6f 5f76  d ctx['%s_odoo_v
+0000b670: 6572 2720 2520 7372 635f 7467 745d 203d  er' % src_tgt] =
+0000b680: 3d20 6374 785b 2766 696e 616c 5f76 6572  = ctx['final_ver
+0000b690: 275d 3a0a 2020 2020 2020 2020 6966 2063  ']:.        if c
+0000b6a0: 7478 2e67 6574 2827 6669 6e61 6c5f 636f  tx.get('final_co
+0000b6b0: 6e66 6e27 293a 0a20 2020 2020 2020 2020  nfn'):.         
+0000b6c0: 2020 2063 7478 5b69 7465 6d5d 203d 2074     ctx[item] = t
+0000b6d0: 6774 5f63 7478 5b27 6669 6e61 6c5f 636f  gt_ctx['final_co
+0000b6e0: 6e66 6e27 5d0a 2020 2020 2020 2020 2020  nfn'].          
+0000b6f0: 2020 6966 206e 6f74 206f 732e 7061 7468    if not os.path
+0000b700: 2e69 7366 696c 6528 6f64 6f6f 5f63 6f6e  .isfile(odoo_con
+0000b710: 666e 293a 0a20 2020 2020 2020 2020 2020  fn):.           
+0000b720: 2020 2020 206f 646f 6f5f 636f 6e66 6e20       odoo_confn 
+0000b730: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+0000b740: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000b750: 2020 6374 785b 6974 656d 5d20 3d20 6f64    ctx[item] = od
+0000b760: 6f6f 5f63 6f6e 666e 0a20 2020 2020 2020  oo_confn.       
+0000b770: 2020 2020 206f 646f 6f5f 636f 6e66 6e20       odoo_confn 
+0000b780: 3d20 4661 6c73 650a 2020 2020 656c 7365  = False.    else
+0000b790: 3a0a 2020 2020 2020 2020 6374 785b 6974  :.        ctx[it
+0000b7a0: 656d 5d20 3d20 6f64 6f6f 5f63 6f6e 666e  em] = odoo_confn
+0000b7b0: 0a20 2020 2020 2020 206f 646f 6f5f 636f  .        odoo_co
+0000b7c0: 6e66 6e20 3d20 4661 6c73 650a 2020 2020  nfn = False.    
+0000b7d0: 6966 206e 6f74 206f 732e 7061 7468 2e69  if not os.path.i
+0000b7e0: 7366 696c 6528 6374 785b 6974 656d 5d29  sfile(ctx[item])
+0000b7f0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+0000b800: 494f 4572 726f 7228 2746 696c 6520 2573  IOError('File %s
+0000b810: 206e 6f74 2066 6f75 6e64 2720 2520 6374   not found' % ct
+0000b820: 785b 6974 656d 5d29 0a20 2020 2063 6f6e  x[item]).    con
+0000b830: 6669 6720 3d20 436f 6e66 6967 5061 7273  fig = ConfigPars
+0000b840: 6572 2e53 6166 6543 6f6e 6669 6750 6172  er.SafeConfigPar
+0000b850: 7365 7228 290a 2020 2020 6966 206f 646f  ser().    if odo
+0000b860: 6f5f 636f 6e66 6e3a 0a20 2020 2020 2020  o_confn:.       
+0000b870: 2063 6f6e 6669 672e 7265 6164 285b 6374   config.read([ct
+0000b880: 785b 6974 656d 5d2c 206f 646f 6f5f 636f  x[item], odoo_co
+0000b890: 6e66 6e5d 290a 2020 2020 656c 7365 3a0a  nfn]).    else:.
+0000b8a0: 2020 2020 2020 2020 636f 6e66 6967 2e72          config.r
+0000b8b0: 6561 6428 6374 785b 6974 656d 5d29 0a20  ead(ctx[item]). 
+0000b8c0: 2020 2072 6574 7572 6e20 636f 6e66 6967     return config
+0000b8d0: 0a0a 0a64 6566 2063 6865 636b 5f63 6f6e  ...def check_con
+0000b8e0: 6628 636f 6e66 6e2c 2070 6172 616d 293a  f(confn, param):
+0000b8f0: 0a20 2020 2066 6420 3d20 6f70 656e 2863  .    fd = open(c
+0000b900: 6f6e 666e 2c20 2772 5527 290a 2020 2020  onfn, 'rU').    
+0000b910: 6c69 6e65 7320 3d20 6664 2e72 6561 6428  lines = fd.read(
+0000b920: 292e 7370 6c69 7428 275c 6e27 290a 2020  ).split('\n').  
+0000b930: 2020 7661 6c75 6520 3d20 4661 6c73 650a    value = False.
+0000b940: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
+0000b950: 6c69 6e65 733a 0a20 2020 2020 2020 2074  lines:.        t
+0000b960: 6b6e 203d 206c 696e 652e 7370 6c69 7428  kn = line.split(
+0000b970: 273d 2729 0a20 2020 2020 2020 2074 6b6e  '=').        tkn
+0000b980: 203d 206d 6170 286c 616d 6264 6120 783a   = map(lambda x:
+0000b990: 2078 2e73 7472 6970 2829 2c20 746b 6e29   x.strip(), tkn)
+0000b9a0: 0a20 2020 2020 2020 2069 6620 746b 6e5b  .        if tkn[
+0000b9b0: 305d 203d 3d20 7061 7261 6d3a 0a20 2020  0] == param:.   
+0000b9c0: 2020 2020 2020 2020 2076 616c 7565 203d           value =
+0000b9d0: 2074 6b6e 5b31 5d0a 2020 2020 2020 2020   tkn[1].        
+0000b9e0: 2020 2020 6272 6561 6b0a 2020 2020 6664      break.    fd
+0000b9f0: 2e63 6c6f 7365 2829 0a20 2020 2072 6574  .close().    ret
+0000ba00: 7572 6e20 7661 6c75 650a 0a0a 6465 6620  urn value...def 
+0000ba10: 6c6f 6164 5f6f 7065 6e75 7067 7261 6465  load_openupgrade
+0000ba20: 6c69 6228 6374 782c 206f 646f 6f5f 6676  lib(ctx, odoo_fv
+0000ba30: 6572 293a 0a20 2020 206f 756c 7061 7468  er):.    oulpath
+0000ba40: 5f70 6172 656e 7464 6972 203d 206f 732e  _parentdir = os.
+0000ba50: 7061 7468 2e64 6972 6e61 6d65 2863 7478  path.dirname(ctx
+0000ba60: 5b27 6f70 745f 6f75 6c70 6174 6827 5d29  ['opt_oulpath'])
+0000ba70: 0a20 2020 206f 756c 6e61 6d65 203d 206f  .    oulname = o
+0000ba80: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
+0000ba90: 6374 785b 276f 7074 5f6f 756c 7061 7468  ctx['opt_oulpath
+0000baa0: 275d 290a 2020 2020 6f75 6c70 6174 685f  ']).    oulpath_
+0000bab0: 6269 6e64 6972 203d 206f 732e 7061 7468  bindir = os.path
+0000bac0: 2e6a 6f69 6e28 6374 785b 276f 7074 5f6f  .join(ctx['opt_o
+0000bad0: 756c 7061 7468 275d 2c20 276f 7065 6e75  ulpath'], 'openu
+0000bae0: 7067 7261 6465 6c69 6227 290a 2020 2020  pgradelib').    
+0000baf0: 6f75 6c70 6174 685f 7363 7269 7074 203d  oulpath_script =
+0000bb00: 206f 732e 7061 7468 2e6a 6f69 6e28 6f75   os.path.join(ou
+0000bb10: 6c70 6174 685f 6269 6e64 6972 2c20 276f  lpath_bindir, 'o
+0000bb20: 7065 6e75 7067 7261 6465 2e70 7927 290a  penupgrade.py').
+0000bb30: 2020 2020 6f75 6c5f 6769 7420 3d20 2768      oul_git = 'h
+0000bb40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000bb50: 6d2f 4f43 412f 6f70 656e 7570 6772 6164  m/OCA/openupgrad
+0000bb60: 656c 6962 2e67 6974 270a 2020 2020 6f73  elib.git'.    os
+0000bb70: 302e 776c 6f67 2827 3e3e 3e20 6c6f 6164  0.wlog('>>> load
+0000bb80: 5f6f 7065 6e75 7067 7261 6465 6c69 6228  _openupgradelib(
+0000bb90: 2573 2927 2025 206f 646f 6f5f 6676 6572  %s)' % odoo_fver
+0000bba0: 290a 0a20 2020 2069 6620 6e6f 7420 6f73  )..    if not os
+0000bbb0: 2e70 6174 682e 6973 6469 7228 6f75 6c70  .path.isdir(oulp
+0000bbc0: 6174 685f 6269 6e64 6972 2920 6f72 206e  ath_bindir) or n
+0000bbd0: 6f74 206f 732e 7061 7468 2e69 7366 696c  ot os.path.isfil
+0000bbe0: 6528 6f75 6c70 6174 685f 7363 7269 7074  e(oulpath_script
+0000bbf0: 293a 0a20 2020 2020 2020 2077 6974 6820  ):.        with 
+0000bc00: 7075 7368 6428 6f75 6c70 6174 685f 7061  pushd(oulpath_pa
+0000bc10: 7265 6e74 6469 7229 3a0a 2020 2020 2020  rentdir):.      
+0000bc20: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
+0000bc30: 2e69 7364 6972 2863 7478 5b27 6f70 745f  .isdir(ctx['opt_
+0000bc40: 6f75 6c70 6174 6827 5d29 3a0a 2020 2020  oulpath']):.    
+0000bc50: 2020 2020 2020 2020 2020 2020 7368 7574              shut
+0000bc60: 696c 2e72 6d74 7265 6528 6374 785b 276f  il.rmtree(ctx['o
+0000bc70: 7074 5f6f 756c 7061 7468 275d 290a 2020  pt_oulpath']).  
+0000bc80: 2020 2020 2020 2020 2020 7275 6e5f 7472            run_tr
+0000bc90: 6163 6564 280a 2020 2020 2020 2020 2020  aced(.          
+0000bca0: 2020 2020 2020 2767 6974 272c 2027 636c        'git', 'cl
+0000bcb0: 6f6e 6527 2c20 6f75 6c5f 6769 742c 206f  one', oul_git, o
+0000bcc0: 756c 6e61 6d65 2c20 272d 2d73 696e 676c  ulname, '--singl
+0000bcd0: 652d 6272 616e 6368 272c 2027 2d2d 6465  e-branch', '--de
+0000bce0: 7074 6827 2c20 2731 270a 2020 2020 2020  pth', '1'.      
+0000bcf0: 2020 2020 2020 290a 2020 2020 656c 7365        ).    else
+0000bd00: 3a0a 2020 2020 2020 2020 6f73 302e 776c  :.        os0.wl
+0000bd10: 6f67 2827 466f 756e 6420 7661 6c69 6420  og('Found valid 
+0000bd20: 6469 7265 6374 6f72 7920 2573 2720 2520  directory %s' % 
+0000bd30: 6f75 6c70 6174 685f 6269 6e64 6972 290a  oulpath_bindir).
+0000bd40: 2020 2020 2320 7379 732e 7061 7468 2e61      # sys.path.a
+0000bd50: 7070 656e 6428 6374 785b 276f 7074 5f6f  ppend(ctx['opt_o
+0000bd60: 756c 7061 7468 275d 290a 2020 2020 6f73  ulpath']).    os
+0000bd70: 2e65 6e76 6972 6f6e 5b27 5059 5448 4f4e  .environ['PYTHON
+0000bd80: 5041 5448 275d 203d 2027 3a27 2e6a 6f69  PATH'] = ':'.joi
+0000bd90: 6e28 0a20 2020 2020 2020 2066 696c 7465  n(.        filte
+0000bda0: 7228 4e6f 6e65 2c20 5b63 7478 5b27 6f70  r(None, [ctx['op
+0000bdb0: 745f 6f75 6c70 6174 6827 5d2c 206f 732e  t_oulpath'], os.
+0000bdc0: 656e 7669 726f 6e2e 6765 7428 2750 5954  environ.get('PYT
+0000bdd0: 484f 4e50 4154 4827 295d 290a 2020 2020  HONPATH')]).    
+0000bde0: 290a 0a0a 6465 6620 6c6f 6164 5f6f 7065  )...def load_ope
+0000bdf0: 6e75 7067 7261 6465 2863 7478 2c20 6f64  nupgrade(ctx, od
+0000be00: 6f6f 5f66 7665 7229 3a0a 2020 2020 6966  oo_fver):.    if
+0000be10: 206f 646f 6f5f 6676 6572 3a0a 2020 2020   odoo_fver:.    
+0000be20: 2020 2020 6f75 7061 7468 5f70 6172 656e      oupath_paren
+0000be30: 7464 6972 203d 206f 732e 7061 7468 2e64  tdir = os.path.d
+0000be40: 6972 6e61 6d65 2863 7478 5b27 6f70 745f  irname(ctx['opt_
+0000be50: 6f75 7061 7468 275d 290a 2020 2020 2020  oupath']).      
+0000be60: 2020 6f75 7061 7468 5f64 6972 203d 2063    oupath_dir = c
+0000be70: 7478 5b27 6f70 745f 6f75 7061 7468 275d  tx['opt_oupath']
+0000be80: 0a20 2020 2020 2020 206f 755f 7665 725f  .        ou_ver_
+0000be90: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+0000bea0: 6f69 6e28 6374 785b 276f 7074 5f6f 7570  oin(ctx['opt_oup
+0000beb0: 6174 6827 5d2c 2027 6f75 5f25 7327 2025  ath'], 'ou_%s' %
+0000bec0: 206f 646f 6f5f 6676 6572 290a 2020 2020   odoo_fver).    
+0000bed0: 656c 7365 3a0a 2020 2020 2020 2020 6f75  else:.        ou
+0000bee0: 7061 7468 5f70 6172 656e 7464 6972 203d  path_parentdir =
+0000bef0: 206f 732e 7061 7468 2e65 7870 616e 6475   os.path.expandu
+0000bf00: 7365 7228 277e 2729 0a20 2020 2020 2020  ser('~').       
+0000bf10: 206f 7570 6174 685f 6469 7220 3d20 6f75   oupath_dir = ou
+0000bf20: 7061 7468 5f70 6172 656e 7464 6972 0a20  path_parentdir. 
+0000bf30: 2020 2020 2020 206f 755f 7665 725f 7061         ou_ver_pa
+0000bf40: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
+0000bf50: 6e28 6f73 2e70 6174 682e 6578 7061 6e64  n(os.path.expand
+0000bf60: 7573 6572 2827 7e27 292c 2027 6f70 656e  user('~'), 'open
+0000bf70: 7570 6772 6164 6527 290a 2020 2020 6f75  upgrade').    ou
+0000bf80: 7061 7468 5f62 696e 6469 7239 203d 206f  path_bindir9 = o
+0000bf90: 732e 7061 7468 2e6a 6f69 6e28 6f75 5f76  s.path.join(ou_v
+0000bfa0: 6572 5f70 6174 682c 2027 6f70 656e 6572  er_path, 'opener
+0000bfb0: 7027 290a 2020 2020 6f75 7061 7468 5f62  p').    oupath_b
+0000bfc0: 696e 6469 7231 3020 3d20 6f73 2e70 6174  indir10 = os.pat
+0000bfd0: 682e 6a6f 696e 286f 755f 7665 725f 7061  h.join(ou_ver_pa
+0000bfe0: 7468 2c20 276f 646f 6f27 290a 2020 2020  th, 'odoo').    
+0000bff0: 6f75 5f67 6974 203d 2027 6874 7470 733a  ou_git = 'https:
+0000c000: 2f2f 6769 7468 7562 2e63 6f6d 2f4f 4341  //github.com/OCA
+0000c010: 2f6f 7065 6e75 7067 7261 6465 2e67 6974  /openupgrade.git
+0000c020: 270a 2020 2020 6f73 302e 776c 6f67 2827  '.    os0.wlog('
+0000c030: 3e3e 3e20 6c6f 6164 5f6f 7065 6e75 7067  >>> load_openupg
+0000c040: 7261 6465 2825 7329 2720 2520 6374 785b  rade(%s)' % ctx[
+0000c050: 2774 6774 5f6f 646f 6f5f 6676 6572 275d  'tgt_odoo_fver']
+0000c060: 290a 0a20 2020 2064 6566 2067 6574 5f6f  )..    def get_o
+0000c070: 755f 7265 6c65 6173 6528 6f75 7061 7468  u_release(oupath
+0000c080: 5f62 696e 6469 7229 3a0a 2020 2020 2020  _bindir):.      
+0000c090: 2020 7769 7468 2070 7573 6864 286f 7570    with pushd(oup
+0000c0a0: 6174 685f 6269 6e64 6972 293a 0a20 2020  ath_bindir):.   
+0000c0b0: 2020 2020 2020 2020 2073 7973 2e70 6174           sys.pat
+0000c0c0: 682e 696e 7365 7274 2830 2c20 2727 290a  h.insert(0, '').
+0000c0d0: 2020 2020 2020 2020 2020 2020 696d 706f              impo
+0000c0e0: 7274 2072 656c 6561 7365 0a0a 2020 2020  rt release..    
+0000c0f0: 2020 2020 2020 2020 7820 3d20 7265 2e6d          x = re.m
+0000c100: 6174 6368 2872 275b 302d 395d 2b5c 2e5b  atch(r'[0-9]+\.[
+0000c110: 302d 395d 2b27 2c20 7265 6c65 6173 652e  0-9]+', release.
+0000c120: 7665 7273 696f 6e29 0a20 2020 2020 2020  version).       
+0000c130: 2020 2020 2069 6620 783a 0a20 2020 2020       if x:.     
+0000c140: 2020 2020 2020 2020 2020 206f 755f 7665             ou_ve
+0000c150: 7220 3d20 7265 6c65 6173 652e 7665 7273  r = release.vers
+0000c160: 696f 6e5b 3020 3a20 782e 656e 6428 295d  ion[0 : x.end()]
+0000c170: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000c180: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000c190: 2020 206f 755f 7665 7220 3d20 7265 6c65     ou_ver = rele
+0000c1a0: 6173 652e 7665 7273 696f 6e0a 2020 2020  ase.version.    
+0000c1b0: 2020 2020 2020 2020 6465 6c20 7379 732e          del sys.
+0000c1c0: 7061 7468 5b30 5d0a 2020 2020 2020 2020  path[0].        
+0000c1d0: 7265 7475 726e 206f 755f 7665 720a 0a20  return ou_ver.. 
+0000c1e0: 2020 206f 755f 7665 7220 3d20 2727 0a20     ou_ver = ''. 
+0000c1f0: 2020 2069 6620 6e6f 7420 6f73 2e70 6174     if not os.pat
+0000c200: 682e 6578 6973 7473 286f 755f 7665 725f  h.exists(ou_ver_
+0000c210: 7061 7468 293a 0a20 2020 2020 2020 2069  path):.        i
+0000c220: 6620 6e6f 7420 6f73 2e70 6174 682e 6578  f not os.path.ex
+0000c230: 6973 7473 286f 7570 6174 685f 7061 7265  ists(oupath_pare
+0000c240: 6e74 6469 7229 3a0a 2020 2020 2020 2020  ntdir):.        
+0000c250: 2020 2020 6f73 2e6d 6b64 6972 286f 7570      os.mkdir(oup
+0000c260: 6174 685f 7061 7265 6e74 6469 7229 0a20  ath_parentdir). 
+0000c270: 2020 2020 2020 2069 6620 6f64 6f6f 5f66         if odoo_f
+0000c280: 7665 7220 616e 6420 6e6f 7420 6f73 2e70  ver and not os.p
+0000c290: 6174 682e 6578 6973 7473 2863 7478 5b27  ath.exists(ctx['
+0000c2a0: 6f70 745f 6f75 7061 7468 275d 293a 0a20  opt_oupath']):. 
+0000c2b0: 2020 2020 2020 2020 2020 206f 732e 6d6b             os.mk
+0000c2c0: 6469 7228 6374 785b 276f 7074 5f6f 7570  dir(ctx['opt_oup
+0000c2d0: 6174 6827 5d29 0a20 2020 2020 2020 206f  ath']).        o
+0000c2e0: 732e 6d6b 6469 7228 6f75 5f76 6572 5f70  s.mkdir(ou_ver_p
+0000c2f0: 6174 6829 0a20 2020 2065 6c69 6620 6f73  ath).    elif os
+0000c300: 2e70 6174 682e 6973 6469 7228 6f75 7061  .path.isdir(oupa
+0000c310: 7468 5f62 696e 6469 7231 3029 3a0a 2020  th_bindir10):.  
+0000c320: 2020 2020 2020 6f75 5f76 6572 203d 2067        ou_ver = g
+0000c330: 6574 5f6f 755f 7265 6c65 6173 6528 6f75  et_ou_release(ou
+0000c340: 7061 7468 5f62 696e 6469 7231 3029 0a20  path_bindir10). 
+0000c350: 2020 2065 6c69 6620 6f73 2e70 6174 682e     elif os.path.
+0000c360: 6973 6469 7228 6f75 7061 7468 5f62 696e  isdir(oupath_bin
+0000c370: 6469 7239 293a 0a20 2020 2020 2020 206f  dir9):.        o
+0000c380: 755f 7665 7220 3d20 6765 745f 6f75 5f72  u_ver = get_ou_r
+0000c390: 656c 6561 7365 286f 7570 6174 685f 6269  elease(oupath_bi
+0000c3a0: 6e64 6972 3929 0a20 2020 2069 6620 6f75  ndir9).    if ou
+0000c3b0: 5f76 6572 2021 3d20 6374 785b 2774 6774  _ver != ctx['tgt
+0000c3c0: 5f6f 646f 6f5f 6676 6572 275d 3a0a 2020  _odoo_fver']:.  
+0000c3d0: 2020 2020 2020 7769 7468 2070 7573 6864        with pushd
+0000c3e0: 286f 7570 6174 685f 6469 7229 3a0a 2020  (oupath_dir):.  
+0000c3f0: 2020 2020 2020 2020 2020 6966 206f 646f            if odo
+0000c400: 6f5f 6676 6572 2061 6e64 206f 732e 7061  o_fver and os.pa
+0000c410: 7468 2e69 7364 6972 286f 755f 7665 725f  th.isdir(ou_ver_
+0000c420: 7061 7468 293a 0a20 2020 2020 2020 2020  path):.         
+0000c430: 2020 2020 2020 2073 6875 7469 6c2e 726d         shutil.rm
+0000c440: 7472 6565 286f 755f 7665 725f 7061 7468  tree(ou_ver_path
+0000c450: 290a 2020 2020 2020 2020 2020 2020 7275  ).            ru
+0000c460: 6e5f 7472 6163 6564 280a 2020 2020 2020  n_traced(.      
+0000c470: 2020 2020 2020 2020 2020 2767 6974 272c            'git',
+0000c480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c490: 2027 636c 6f6e 6527 2c0a 2020 2020 2020   'clone',.      
+0000c4a0: 2020 2020 2020 2020 2020 6f75 5f67 6974            ou_git
+0000c4b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c4c0: 2020 6f73 2e70 6174 682e 6261 7365 6e61    os.path.basena
+0000c4d0: 6d65 286f 755f 7665 725f 7061 7468 292c  me(ou_ver_path),
+0000c4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c4f0: 2027 2d62 272c 0a20 2020 2020 2020 2020   '-b',.         
+0000c500: 2020 2020 2020 2063 7478 5b27 7467 745f         ctx['tgt_
+0000c510: 6f64 6f6f 5f66 7665 7227 5d2c 0a20 2020  odoo_fver'],.   
+0000c520: 2020 2020 2020 2020 2020 2020 2027 2d2d               '--
+0000c530: 7369 6e67 6c65 2d62 7261 6e63 6827 2c0a  single-branch',.
+0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c550: 272d 2d64 6570 7468 272c 0a20 2020 2020  '--depth',.     
+0000c560: 2020 2020 2020 2020 2020 2027 3127 2c0a             '1',.
+0000c570: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000c580: 2020 2020 2020 2020 2020 6170 706c 795f            apply_
+0000c590: 7061 7463 6828 6f75 5f76 6572 5f70 6174  patch(ou_ver_pat
+0000c5a0: 682c 2063 7478 5b27 7467 745f 6f64 6f6f  h, ctx['tgt_odoo
+0000c5b0: 5f66 7665 7227 5d29 0a20 2020 2065 6c73  _fver']).    els
+0000c5c0: 653a 0a20 2020 2020 2020 206f 7330 2e77  e:.        os0.w
+0000c5d0: 6c6f 6728 2746 6f75 6e64 2076 616c 6964  log('Found valid
+0000c5e0: 2064 6972 6563 746f 7279 2025 7327 2025   directory %s' %
+0000c5f0: 2063 7478 5b27 6f70 745f 6f75 7061 7468   ctx['opt_oupath
+0000c600: 275d 290a 2020 2020 6966 206e 6f74 2073  ']).    if not s
+0000c610: 7263 5f63 7478 5b27 6e6f 5f76 656e 7627  rc_ctx['no_venv'
+0000c620: 5d20 616e 6420 6e6f 7420 7372 635f 6374  ] and not src_ct
+0000c630: 785b 2764 7279 5f72 756e 275d 3a0a 2020  x['dry_run']:.  
+0000c640: 2020 2020 2020 7665 6e76 5f70 6174 6820        venv_path 
+0000c650: 3d20 6f73 2e70 6174 682e 6a6f 696e 2874  = os.path.join(t
+0000c660: 6774 5f63 7478 5b27 7665 6e76 5f6f 7570  gt_ctx['venv_oup
+0000c670: 6174 6827 5d2c 2027 6f70 656e 7570 6772  ath'], 'openupgr
+0000c680: 6164 6527 290a 2020 2020 2020 2020 6966  ade').        if
+0000c690: 206e 6f74 206f 732e 7061 7468 2e69 7364   not os.path.isd
+0000c6a0: 6972 2876 656e 765f 7061 7468 293a 0a20  ir(venv_path):. 
+0000c6b0: 2020 2020 2020 2020 2020 206f 732e 7379             os.sy
+0000c6c0: 6d6c 696e 6b28 6f75 5f76 6572 5f70 6174  mlink(ou_ver_pat
+0000c6d0: 682c 2076 656e 765f 7061 7468 290a 2020  h, venv_path).  
+0000c6e0: 2020 7265 7475 726e 206f 755f 7665 725f    return ou_ver_
+0000c6f0: 7061 7468 0a0a 0a64 6566 2061 7070 6c79  path...def apply
+0000c700: 5f70 6174 6368 286f 755f 7665 725f 7061  _patch(ou_ver_pa
+0000c710: 7468 2c20 6f64 6f6f 5f66 7665 7229 3a0a  th, odoo_fver):.
+0000c720: 2020 2020 6966 206f 646f 6f5f 6676 6572      if odoo_fver
+0000c730: 203d 3d20 2739 2e30 273a 0a20 2020 2020   == '9.0':.     
+0000c740: 2020 2066 696c 6520 3d20 6f73 2e70 6174     file = os.pat
+0000c750: 682e 6a6f 696e 280a 2020 2020 2020 2020  h.join(.        
+0000c760: 2020 2020 6f75 5f76 6572 5f70 6174 682c      ou_ver_path,
+0000c770: 0a20 2020 2020 2020 2020 2020 2027 6f70  .            'op
+0000c780: 656e 6572 7027 2c0a 2020 2020 2020 2020  enerp',.        
+0000c790: 2020 2020 2761 6464 6f6e 7327 2c0a 2020      'addons',.  
+0000c7a0: 2020 2020 2020 2020 2020 2762 6173 6527            'base'
+0000c7b0: 2c0a 2020 2020 2020 2020 2020 2020 276d  ,.            'm
+0000c7c0: 6967 7261 7469 6f6e 7327 2c0a 2020 2020  igrations',.    
+0000c7d0: 2020 2020 2020 2020 2739 2e30 2e31 2e33          '9.0.1.3
+0000c7e0: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+0000c7f0: 706f 7374 2d6d 6967 7261 7469 6f6e 2e70  post-migration.p
+0000c800: 7927 2c0a 2020 2020 2020 2020 290a 2020  y',.        ).  
+0000c810: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
+0000c820: 2e69 7366 696c 6528 6669 6c65 293a 0a20  .isfile(file):. 
+0000c830: 2020 2020 2020 2020 2020 2073 6564 280a             sed(.
+0000c840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c850: 6669 6c65 2c0a 2020 2020 2020 2020 2020  file,.          
+0000c860: 2020 2020 2020 5b72 225e 202a 2769 725f        [r"^ *'ir_
+0000c870: 6163 7469 6f6e 7327 3a20 5c5b 222c 2022  actions': \[", "
+0000c880: 2320 2020 2020 2769 725f 6163 7469 6f6e  #     'ir_action
+0000c890: 7327 3a20 5b22 5d2c 0a20 2020 2020 2020  s': ["],.       
+0000c8a0: 2020 2020 2020 2020 205b 7222 5e20 2a5c           [r"^ *\
+0000c8b0: 2827 6865 6c70 272c 204e 6f6e 652c 204e  ('help', None, N
+0000c8c0: 6f6e 655c 292c 222c 2022 2320 2020 2020  one\),", "#     
+0000c8d0: 2020 2020 2827 6865 6c70 272c 204e 6f6e      ('help', Non
+0000c8e0: 652c 204e 6f6e 6529 2c22 5d2c 0a20 2020  e, None),"],.   
+0000c8f0: 2020 2020 2020 2020 2020 2020 205b 225e               ["^
+0000c900: 202a 5d2c 222c 2022 2320 2020 2020 5d2c   *],", "#     ],
+0000c910: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+0000c920: 290a 0a0a 6465 6620 6164 645f 746e 6c5f  )...def add_tnl_
+0000c930: 6974 656d 2863 7478 2c20 6d6f 6465 6c2c  item(ctx, model,
+0000c940: 206d 6f64 756c 652c 206e 6577 5f6d 6f64   module, new_mod
+0000c950: 756c 652c 2073 7263 5f66 7665 722c 2074  ule, src_fver, t
+0000c960: 6774 5f66 7665 722c 2074 7970 653d 4661  gt_fver, type=Fa
+0000c970: 6c73 6529 3a0a 2020 2020 746e 6c20 3d20  lse):.    tnl = 
+0000c980: 7472 616e 736f 646f 6f2e 7472 616e 736c  transodoo.transl
+0000c990: 6174 655f 6672 6f6d 5f74 6f28 6374 782c  ate_from_to(ctx,
+0000c9a0: 206d 6f64 656c 2c20 6d6f 6475 6c65 2c20   model, module, 
+0000c9b0: 7372 635f 6676 6572 2c20 7467 745f 6676  src_fver, tgt_fv
+0000c9c0: 6572 2c20 7479 7065 3d74 7970 6529 0a20  er, type=type). 
+0000c9d0: 2020 2069 6620 746e 6c20 213d 206e 6577     if tnl != new
+0000c9e0: 5f6d 6f64 756c 653a 0a20 2020 2020 2020  _module:.       
+0000c9f0: 206f 7330 2e77 6c6f 6728 2754 7261 6e73   os0.wlog('Trans
+0000ca00: 6c61 7465 206d 6f64 756c 6520 2573 202d  late module %s -
+0000ca10: 3e20 2573 2720 2520 286d 6f64 756c 652c  > %s' % (module,
+0000ca20: 206e 6577 5f6d 6f64 756c 6529 290a 2020   new_module)).  
+0000ca30: 2020 2020 2020 7665 725f 6e61 6d65 7320        ver_names 
+0000ca40: 3d20 7b7d 0a20 2020 2020 2020 206e 616d  = {}.        nam
+0000ca50: 6520 3d20 6d6f 6475 6c65 0a20 2020 2020  e = module.     
+0000ca60: 2020 2066 6f72 2076 6572 2069 6e20 5645     for ver in VE
+0000ca70: 5253 494f 4e53 3a0a 2020 2020 2020 2020  RSIONS:.        
+0000ca80: 2020 2020 6966 2076 6572 203d 3d20 6374      if ver == ct
+0000ca90: 785b 2774 6774 5f6f 646f 6f5f 6676 6572  x['tgt_odoo_fver
+0000caa0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
+0000cab0: 2020 2020 6e61 6d65 203d 206e 6577 5f6d      name = new_m
+0000cac0: 6f64 756c 650a 2020 2020 2020 2020 2020  odule.          
+0000cad0: 2020 7665 725f 6e61 6d65 735b 7665 725d    ver_names[ver]
+0000cae0: 203d 206e 616d 650a 2020 2020 2020 2020   = name.        
+0000caf0: 756e 616d 6520 3d20 7472 616e 736f 646f  uname = transodo
+0000cb00: 6f2e 7365 745f 756e 616d 6528 7479 7065  o.set_uname(type
+0000cb10: 2c20 6e61 6d65 2c20 5b76 6572 5f6e 616d  , name, [ver_nam
+0000cb20: 6573 5b78 5d20 666f 7220 7820 696e 2056  es[x] for x in V
+0000cb30: 4552 5349 4f4e 535d 290a 2020 2020 2020  ERSIONS]).      
+0000cb40: 2020 666f 7220 7665 7220 696e 2056 4552    for ver in VER
+0000cb50: 5349 4f4e 533a 0a20 2020 2020 2020 2020  SIONS:.         
+0000cb60: 2020 2063 7478 5b27 6d69 6e64 726f 6f74     ctx['mindroot
+0000cb70: 275d 203d 2074 7261 6e73 6f64 6f6f 2e6c  '] = transodoo.l
+0000cb80: 696e 6b5f 7665 7273 696f 6e65 645f 6e61  ink_versioned_na
+0000cb90: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
+0000cba0: 2020 2020 6374 785b 276d 696e 6472 6f6f      ctx['mindroo
+0000cbb0: 7427 5d2c 206d 6f64 656c 2c20 756e 616d  t'], model, unam
+0000cbc0: 652c 2074 7970 652c 2076 6572 5f6e 616d  e, type, ver_nam
+0000cbd0: 6573 5b76 6572 5d2c 2076 6572 0a20 2020  es[ver], ver.   
+0000cbe0: 2020 2020 2020 2020 2029 0a20 2020 2072           ).    r
+0000cbf0: 6574 7572 6e20 6374 780a 0a0a 6465 6620  eturn ctx...def 
+0000cc00: 646f 5f74 6e6c 5f6d 6f64 756c 655f 6c69  do_tnl_module_li
+0000cc10: 7374 280a 2020 2020 6374 782c 206d 6f64  st(.    ctx, mod
+0000cc20: 756c 655f 6c69 7374 2c20 7372 635f 6676  ule_list, src_fv
+0000cc30: 6572 2c20 7467 745f 6676 6572 2c20 7467  er, tgt_fver, tg
+0000cc40: 745f 6d6f 6475 6c65 5f6c 6973 742c 2070  t_module_list, p
+0000cc50: 7572 653d 4e6f 6e65 0a29 3a0a 2020 2020  ure=None.):.    
+0000cc60: 7379 732e 7061 7468 2e61 7070 656e 6428  sys.path.append(
+0000cc70: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
+0000cc80: 5f5f 6669 6c65 5f5f 2929 0a20 2020 2074  __file__)).    t
+0000cc90: 7261 6e73 6f64 6f6f 2e72 6561 645f 7374  ransodoo.read_st
+0000cca0: 6f72 6564 5f64 6963 7428 6374 7829 0a20  ored_dict(ctx). 
+0000ccb0: 2020 2074 6e6c 5f6d 6f64 756c 655f 6c69     tnl_module_li
+0000ccc0: 7374 203d 205b 5d0a 2020 2020 6261 645f  st = [].    bad_
+0000ccd0: 6d6f 6475 6c65 5f6c 6973 7420 3d20 5b5d  module_list = []
+0000cce0: 0a20 2020 206d 6f64 656c 203d 2027 6972  .    model = 'ir
+0000ccf0: 2e6d 6f64 756c 652e 6d6f 6475 6c65 270a  .module.module'.
+0000cd00: 2020 2020 666f 7220 6974 656d 2069 6e20      for item in 
+0000cd10: 6d6f 6475 6c65 5f6c 6973 743a 0a20 2020  module_list:.   
+0000cd20: 2020 2020 2074 6e6c 203d 2074 7261 6e73       tnl = trans
+0000cd30: 6f64 6f6f 2e74 7261 6e73 6c61 7465 5f66  odoo.translate_f
+0000cd40: 726f 6d5f 746f 280a 2020 2020 2020 2020  rom_to(.        
+0000cd50: 2020 2020 6374 782c 206d 6f64 656c 2c20      ctx, model, 
+0000cd60: 6974 656d 2c20 7372 635f 6676 6572 2c20  item, src_fver, 
+0000cd70: 7467 745f 6676 6572 2c20 7479 7065 3d27  tgt_fver, type='
+0000cd80: 6d6f 6475 6c65 270a 2020 2020 2020 2020  module'.        
+0000cd90: 290a 2020 2020 2020 2020 6966 2074 6e6c  ).        if tnl
+0000cda0: 203d 3d20 6974 656d 3a0a 2020 2020 2020   == item:.      
+0000cdb0: 2020 2020 2020 746e 6c20 3d20 7472 616e        tnl = tran
+0000cdc0: 736f 646f 6f2e 7472 616e 736c 6174 655f  sodoo.translate_
+0000cdd0: 6672 6f6d 5f74 6f28 0a20 2020 2020 2020  from_to(.       
+0000cde0: 2020 2020 2020 2020 2063 7478 2c20 6d6f           ctx, mo
+0000cdf0: 6465 6c2c 2069 7465 6d2c 2073 7263 5f66  del, item, src_f
+0000ce00: 7665 722c 2074 6774 5f66 7665 722c 2074  ver, tgt_fver, t
+0000ce10: 7970 653d 276d 6572 6765 270a 2020 2020  ype='merge'.    
+0000ce20: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000ce30: 2020 6966 2074 6774 5f6d 6f64 756c 655f    if tgt_module_
+0000ce40: 6c69 7374 2061 6e64 2074 6e6c 206e 6f74  list and tnl not
+0000ce50: 2069 6e20 7467 745f 6d6f 6475 6c65 5f6c   in tgt_module_l
+0000ce60: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
+0000ce70: 2062 6164 5f6d 6f64 756c 655f 6c69 7374   bad_module_list
+0000ce80: 2e61 7070 656e 6428 6974 656d 290a 2020  .append(item).  
+0000ce90: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0000cea0: 2070 7572 653a 0a20 2020 2020 2020 2020   pure:.         
+0000ceb0: 2020 2020 2020 2074 6e6c 5f6d 6f64 756c         tnl_modul
+0000cec0: 655f 6c69 7374 2e61 7070 656e 6428 746e  e_list.append(tn
+0000ced0: 6c29 0a20 2020 2020 2020 2065 6c73 653a  l).        else:
+0000cee0: 0a20 2020 2020 2020 2020 2020 2074 6e6c  .            tnl
+0000cef0: 5f6d 6f64 756c 655f 6c69 7374 2e61 7070  _module_list.app
+0000cf00: 656e 6428 746e 6c29 0a20 2020 2072 6574  end(tnl).    ret
+0000cf10: 7572 6e20 746e 6c5f 6d6f 6475 6c65 5f6c  urn tnl_module_l
+0000cf20: 6973 742c 2062 6164 5f6d 6f64 756c 655f  ist, bad_module_
+0000cf30: 6c69 7374 0a0a 0a64 6566 206f 646f 6f5f  list...def odoo_
+0000cf40: 6465 7065 6e64 656e 6369 6573 280a 2020  dependencies(.  
+0000cf50: 2020 6374 782c 2061 6374 696f 6e2c 2064    ctx, action, d
+0000cf60: 625f 6e61 6d65 2c20 6c63 6f6e 662c 2070  b_name, lconf, p
+0000cf70: 6174 6873 2c20 6f64 6f6f 5f66 7665 722c  aths, odoo_fver,
+0000cf80: 206d 6174 6368 6573 3d4e 6f6e 652c 2064   matches=None, d
+0000cf90: 6570 656e 6473 5f62 793d 4e6f 6e65 0a29  epends_by=None.)
+0000cfa0: 3a0a 2020 2020 7769 7468 2070 7573 6864  :.    with pushd
+0000cfb0: 2827 2f6f 7074 2f6f 646f 6f2f 6465 762f  ('/opt/odoo/dev/
+0000cfc0: 7079 7069 2f77 6f6b 5f63 6f64 652f 776f  pypi/wok_code/wo
+0000cfd0: 6b5f 636f 6465 2729 3a0a 2020 2020 2020  k_code'):.      
+0000cfe0: 2020 7379 732e 7061 7468 2e61 7070 656e    sys.path.appen
+0000cff0: 6428 2727 290a 2020 2020 2020 2020 696d  d('').        im
+0000d000: 706f 7274 206f 646f 6f5f 6465 7065 6e64  port odoo_depend
+0000d010: 656e 6369 6573 0a0a 2020 2020 2020 2020  encies..        
+0000d020: 6374 785b 2762 7261 6e63 6827 5d20 3d20  ctx['branch'] = 
+0000d030: 6f64 6f6f 5f66 7665 720a 2020 2020 2020  odoo_fver.      
+0000d040: 2020 6966 2064 625f 6e61 6d65 3a0a 2020    if db_name:.  
+0000d050: 2020 2020 2020 2020 2020 6374 785b 2763            ctx['c
+0000d060: 6f6e 665f 666e 275d 203d 206c 636f 6e66  onf_fn'] = lconf
+0000d070: 0a20 2020 2020 2020 2020 2020 2063 7478  .            ctx
+0000d080: 203d 206f 646f 6f5f 6465 7065 6e64 656e   = odoo_dependen
+0000d090: 6369 6573 2e72 6574 7269 6576 655f 6462  cies.retrieve_db
+0000d0a0: 5f6d 6f64 756c 6573 2863 7478 290a 2020  _modules(ctx).  
+0000d0b0: 2020 2020 2020 2020 2020 6d61 7463 6865            matche
+0000d0c0: 7320 3d20 6374 785b 276d 6f64 756c 6573  s = ctx['modules
+0000d0d0: 5f74 6f5f 6d61 7463 6827 5d0a 2020 2020  _to_match'].    
+0000d0e0: 2020 2020 6966 2061 6374 696f 6e20 3d3d      if action ==
+0000d0f0: 2027 6465 7027 3a0a 2020 2020 2020 2020   'dep':.        
+0000d100: 2020 2020 7265 7320 3d20 6f64 6f6f 5f64      res = odoo_d
+0000d110: 6570 656e 6465 6e63 6965 732e 6765 745f  ependencies.get_
+0000d120: 6465 7065 6e64 656e 6369 6573 5f6c 6973  dependencies_lis
+0000d130: 7428 7061 7468 732c 206d 6174 6368 6573  t(paths, matches
+0000d140: 3d6d 6174 6368 6573 290a 2020 2020 2020  =matches).      
+0000d150: 2020 656c 6966 2061 6374 696f 6e20 3d3d    elif action ==
+0000d160: 2027 6d6f 6427 3a0a 2020 2020 2020 2020   'mod':.        
+0000d170: 2020 2020 7265 7320 3d20 6f64 6f6f 5f64      res = odoo_d
+0000d180: 6570 656e 6465 6e63 6965 732e 6765 745f  ependencies.get_
+0000d190: 6d6f 6475 6c65 735f 6c69 7374 2870 6174  modules_list(pat
+0000d1a0: 6873 2c20 6d61 7463 6865 733d 6d61 7463  hs, matches=matc
+0000d1b0: 6865 7329 0a20 2020 2020 2020 2065 6c69  hes).        eli
+0000d1c0: 6620 6163 7469 6f6e 203d 3d20 2772 6576  f action == 'rev
+0000d1d0: 273a 0a20 2020 2020 2020 2020 2020 2072  ':.            r
+0000d1e0: 6573 203d 206f 646f 6f5f 6465 7065 6e64  es = odoo_depend
+0000d1f0: 656e 6369 6573 2e67 6574 5f64 6570 656e  encies.get_depen
+0000d200: 6465 6e74 735f 6c69 7374 280a 2020 2020  dents_list(.    
+0000d210: 2020 2020 2020 2020 2020 2020 7061 7468              path
+0000d220: 732c 206d 6174 6368 6573 3d6d 6174 6368  s, matches=match
+0000d230: 6573 2c20 6465 7065 6e64 735f 6279 3d64  es, depends_by=d
+0000d240: 6570 656e 6473 5f62 790a 2020 2020 2020  epends_by.      
+0000d250: 2020 2020 2020 290a 2020 2020 6465 6c20        ).    del 
+0000d260: 7379 732e 7061 7468 5b2d 315d 0a20 2020  sys.path[-1].   
+0000d270: 2072 6574 7572 6e20 7265 730a 0a0a 6465   return res...de
+0000d280: 6620 6164 645f 7665 7273 696f 6e65 645f  f add_versioned_
+0000d290: 746e 6c28 6374 782c 2073 7263 5f66 7665  tnl(ctx, src_fve
+0000d2a0: 722c 2074 6774 5f66 7665 7229 3a0a 2020  r, tgt_fver):.  
+0000d2b0: 2020 6f73 302e 776c 6f67 2827 5570 6772    os0.wlog('Upgr
+0000d2c0: 6164 696e 6720 7472 616e 736c 6174 696f  ading translatio
+0000d2d0: 6e20 6e61 6d65 2066 726f 6d20 2573 2074  n name from %s t
+0000d2e0: 6f20 2573 2720 2520 2873 7263 5f66 7665  o %s' % (src_fve
+0000d2f0: 722c 2074 6774 5f66 7665 7229 290a 2020  r, tgt_fver)).  
+0000d300: 2020 6f75 5f76 6572 5f70 6174 6820 3d20    ou_ver_path = 
+0000d310: 6f73 2e70 6174 682e 6a6f 696e 2863 7478  os.path.join(ctx
+0000d320: 5b27 6f70 745f 6f75 7061 7468 275d 2c20  ['opt_oupath'], 
+0000d330: 276f 755f 2573 2720 2520 7467 745f 6676  'ou_%s' % tgt_fv
+0000d340: 6572 290a 2020 2020 7769 7468 2070 7573  er).    with pus
+0000d350: 6864 286f 755f 7665 725f 7061 7468 293a  hd(ou_ver_path):
+0000d360: 0a20 2020 2020 2020 2073 7973 2e70 6174  .        sys.pat
+0000d370: 682e 6170 7065 6e64 2827 2729 0a20 2020  h.append('').   
+0000d380: 2020 2020 2073 7973 2e70 6174 682e 6170       sys.path.ap
+0000d390: 7065 6e64 286f 732e 7061 7468 2e64 6972  pend(os.path.dir
+0000d3a0: 6e61 6d65 285f 5f66 696c 655f 5f29 290a  name(__file__)).
+0000d3b0: 2020 2020 2020 2020 6966 2069 6e74 2874          if int(t
+0000d3c0: 6774 5f66 7665 722e 7370 6c69 7428 272e  gt_fver.split('.
+0000d3d0: 2729 5b30 5d29 203c 2031 303a 0a20 2020  ')[0]) < 10:.   
+0000d3e0: 2020 2020 2020 2020 2069 6d70 6f72 7420           import 
+0000d3f0: 6f70 656e 6572 702e 6164 646f 6e73 2e6f  openerp.addons.o
+0000d400: 7065 6e75 7067 7261 6465 5f72 6563 6f72  penupgrade_recor
+0000d410: 6473 2e6c 6962 2e61 7072 696f 7269 2061  ds.lib.apriori a
+0000d420: 7320 6170 7269 6f72 690a 2020 2020 2020  s apriori.      
+0000d430: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000d440: 2020 2020 696d 706f 7274 206f 646f 6f2e      import odoo.
+0000d450: 6164 646f 6e73 2e6f 7065 6e75 7067 7261  addons.openupgra
+0000d460: 6465 5f72 6563 6f72 6473 2e6c 6962 2e61  de_records.lib.a
+0000d470: 7072 696f 7269 2061 7320 6170 7269 6f72  priori as aprior
+0000d480: 690a 2020 2020 2020 2020 7472 616e 736f  i.        transo
+0000d490: 646f 6f2e 7265 6164 5f73 746f 7265 645f  doo.read_stored_
+0000d4a0: 6469 6374 2863 7478 290a 2020 2020 2020  dict(ctx).      
+0000d4b0: 2020 6d6f 6465 6c20 3d20 2769 722e 6d6f    model = 'ir.mo
+0000d4c0: 6475 6c65 2e6d 6f64 756c 6527 0a20 2020  dule.module'.   
+0000d4d0: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
+0000d4e0: 6170 7269 6f72 692c 2027 7265 6e61 6d65  apriori, 'rename
+0000d4f0: 645f 6d6f 6475 6c65 7327 293a 0a20 2020  d_modules'):.   
+0000d500: 2020 2020 2020 2020 2074 7970 203d 2027           typ = '
+0000d510: 6d6f 6475 6c65 270a 2020 2020 2020 2020  module'.        
+0000d520: 2020 2020 666f 7220 6d6f 6475 6c65 2069      for module i
+0000d530: 6e20 6170 7269 6f72 692e 7265 6e61 6d65  n apriori.rename
+0000d540: 645f 6d6f 6475 6c65 733a 0a20 2020 2020  d_modules:.     
+0000d550: 2020 2020 2020 2020 2020 206e 6577 5f6d             new_m
+0000d560: 6f64 756c 6520 3d20 6170 7269 6f72 692e  odule = apriori.
+0000d570: 7265 6e61 6d65 645f 6d6f 6475 6c65 735b  renamed_modules[
+0000d580: 6d6f 6475 6c65 5d0a 2020 2020 2020 2020  module].        
+0000d590: 2020 2020 2020 2020 6374 7820 3d20 6164          ctx = ad
+0000d5a0: 645f 746e 6c5f 6974 656d 280a 2020 2020  d_tnl_item(.    
+0000d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5c0: 6374 782c 206d 6f64 656c 2c20 6d6f 6475  ctx, model, modu
+0000d5d0: 6c65 2c20 6e65 775f 6d6f 6475 6c65 2c20  le, new_module, 
+0000d5e0: 7372 635f 6676 6572 2c20 7467 745f 6676  src_fver, tgt_fv
+0000d5f0: 6572 2c20 7479 7065 3d74 7970 0a20 2020  er, type=typ.   
+0000d600: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000d610: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
+0000d620: 7228 6170 7269 6f72 692c 2027 6d65 7267  r(apriori, 'merg
+0000d630: 6564 5f6d 6f64 756c 6573 2729 3a0a 2020  ed_modules'):.  
+0000d640: 2020 2020 2020 2020 2020 7479 7020 3d20            typ = 
+0000d650: 276d 6572 6765 270a 2020 2020 2020 2020  'merge'.        
+0000d660: 2020 2020 666f 7220 6974 656d 2069 6e20      for item in 
+0000d670: 6170 7269 6f72 692e 6d65 7267 6564 5f6d  apriori.merged_m
+0000d680: 6f64 756c 6573 3a0a 2020 2020 2020 2020  odules:.        
+0000d690: 2020 2020 2020 2020 6d6f 6475 6c65 203d          module =
+0000d6a0: 2069 7465 6d5b 305d 0a20 2020 2020 2020   item[0].       
+0000d6b0: 2020 2020 2020 2020 206e 6577 5f6d 6f64           new_mod
+0000d6c0: 756c 6520 3d20 6974 656d 5b31 5d0a 2020  ule = item[1].  
+0000d6d0: 2020 2020 2020 2020 2020 2020 2020 6374                ct
+0000d6e0: 7820 3d20 6164 645f 746e 6c5f 6974 656d  x = add_tnl_item
+0000d6f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000d700: 2020 2020 2020 6374 782c 206d 6f64 656c        ctx, model
+0000d710: 2c20 6d6f 6475 6c65 2c20 6e65 775f 6d6f  , module, new_mo
+0000d720: 6475 6c65 2c20 7372 635f 6676 6572 2c20  dule, src_fver, 
+0000d730: 7467 745f 6676 6572 2c20 7479 7065 3d74  tgt_fver, type=t
+0000d740: 7970 0a20 2020 2020 2020 2020 2020 2020  yp.             
+0000d750: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+0000d760: 6861 7361 7474 7228 6170 7269 6f72 692c  hasattr(apriori,
+0000d770: 2027 7265 6e61 6d65 645f 6d6f 6465 6c73   'renamed_models
+0000d780: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+0000d790: 6d6f 6465 6c20 3d20 2769 722e 6d6f 6465  model = 'ir.mode
+0000d7a0: 6c27 0a20 2020 2020 2020 2020 2020 2074  l'.            t
+0000d7b0: 7970 203d 2027 6d6f 6465 6c27 0a20 2020  yp = 'model'.   
+0000d7c0: 2020 2020 2020 2020 2066 6f72 2069 7465           for ite
+0000d7d0: 6d20 696e 2061 7072 696f 7269 2e72 656e  m in apriori.ren
+0000d7e0: 616d 6564 5f6d 6f64 656c 733a 0a20 2020  amed_models:.   
+0000d7f0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+0000d800: 756c 6520 3d20 6974 656d 5b30 5d0a 2020  ule = item[0].  
+0000d810: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+0000d820: 775f 6d6f 6475 6c65 203d 2069 7465 6d5b  w_module = item[
+0000d830: 315d 0a20 2020 2020 2020 2020 2020 2020  1].             
+0000d840: 2020 2063 7478 203d 2061 6464 5f74 6e6c     ctx = add_tnl
+0000d850: 5f69 7465 6d28 0a20 2020 2020 2020 2020  _item(.         
+0000d860: 2020 2020 2020 2020 2020 2063 7478 2c20             ctx, 
+0000d870: 6d6f 6465 6c2c 206d 6f64 756c 652c 206e  model, module, n
+0000d880: 6577 5f6d 6f64 756c 652c 2073 7263 5f66  ew_module, src_f
+0000d890: 7665 722c 2074 6774 5f66 7665 722c 2074  ver, tgt_fver, t
+0000d8a0: 7970 653d 7479 700a 2020 2020 2020 2020  ype=typ.        
+0000d8b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000d8c0: 2020 7472 616e 736f 646f 6f2e 7772 6974    transodoo.writ
+0000d8d0: 655f 7374 6f72 6564 5f64 6963 7428 6374  e_stored_dict(ct
+0000d8e0: 7829 0a20 2020 2020 2020 2064 656c 2073  x).        del s
+0000d8f0: 7973 2e70 6174 685b 2d31 5d0a 2020 2020  ys.path[-1].    
+0000d900: 2020 2020 6465 6c20 7379 732e 7061 7468      del sys.path
+0000d910: 5b2d 315d 0a0a 0a64 6566 2061 646a 7573  [-1]...def adjus
+0000d920: 745f 6374 7828 7372 635f 6374 782c 2074  t_ctx(src_ctx, t
+0000d930: 6774 5f63 7478 293a 0a20 2020 2066 6f72  gt_ctx):.    for
+0000d940: 2069 7465 6d20 696e 2028 0a20 2020 2020   item in (.     
+0000d950: 2020 2027 6f64 6f6f 5f76 6572 272c 0a20     'odoo_ver',. 
+0000d960: 2020 2020 2020 2027 6f64 6f6f 5f66 7665         'odoo_fve
+0000d970: 7227 2c0a 2020 2020 2020 2020 2776 6964  r',.        'vid
+0000d980: 272c 0a20 2020 2020 2020 2027 636f 6e66  ',.        'conf
+0000d990: 5f66 6e27 2c0a 2020 2020 2020 2020 2773  _fn',.        's
+0000d9a0: 7663 5f70 726f 746f 636f 6c27 2c0a 2020  vc_protocol',.  
+0000d9b0: 2020 2020 2020 2764 625f 686f 7374 272c        'db_host',
+0000d9c0: 0a20 2020 2020 2020 2027 6462 5f6e 616d  .        'db_nam
+0000d9d0: 6527 2c0a 2020 2020 2020 2020 2764 625f  e',.        'db_
+0000d9e0: 7573 6572 272c 0a20 2020 2020 2020 2027  user',.        '
+0000d9f0: 6462 5f70 6f72 7427 2c0a 2020 2020 2020  db_port',.      
+0000da00: 2020 2764 625f 7061 7373 776f 7264 272c    'db_password',
+0000da10: 0a20 2020 2020 2020 2027 6c65 7665 6c27  .        'level'
+0000da20: 2c0a 2020 2020 2020 2020 2778 6d6c 7270  ,.        'xmlrp
+0000da30: 635f 706f 7274 272c 0a20 2020 2020 2020  c_port',.       
+0000da40: 2027 7073 7963 6f70 6732 272c 0a20 2020   'psycopg2',.   
+0000da50: 2020 2020 2027 6c6f 6769 6e5f 7573 6572       'login_user
+0000da60: 272c 0a20 2020 2020 2020 2027 6c6f 6769  ',.        'logi
+0000da70: 6e5f 7061 7373 776f 7264 272c 0a20 2020  n_password',.   
+0000da80: 2020 2020 2027 6c6f 6766 696c 6527 2c0a       'logfile',.
+0000da90: 2020 2020 2020 2020 2777 6974 686f 7574          'without
+0000daa0: 5f64 656d 6f27 2c0a 2020 2020 293a 0a20  _demo',.    ):. 
+0000dab0: 2020 2020 2020 2073 7263 5f70 6172 616d         src_param
+0000dac0: 203d 2027 7372 635f 2573 2720 2520 6974   = 'src_%s' % it
+0000dad0: 656d 0a20 2020 2020 2020 2074 6774 5f70  em.        tgt_p
+0000dae0: 6172 616d 203d 2027 7467 745f 2573 2720  aram = 'tgt_%s' 
+0000daf0: 2520 6974 656d 0a20 2020 2020 2020 2069  % item.        i
+0000db00: 6620 6974 656d 203d 3d20 276f 646f 6f5f  f item == 'odoo_
+0000db10: 7665 7227 3a0a 2020 2020 2020 2020 2020  ver':.          
+0000db20: 2020 6966 206e 6f74 2073 7263 5f63 7478    if not src_ctx
+0000db30: 5b27 7365 6c5f 6d6f 6465 6c27 5d3a 0a20  ['sel_model']:. 
+0000db40: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000db50: 6774 5f63 7478 5b74 6774 5f70 6172 616d  gt_ctx[tgt_param
+0000db60: 5d20 3d20 7372 635f 6374 785b 7372 635f  ] = src_ctx[src_
+0000db70: 7061 7261 6d5d 202b 2031 0a20 2020 2020  param] + 1.     
+0000db80: 2020 2065 6c69 6620 6974 656d 203d 3d20     elif item == 
+0000db90: 276f 646f 6f5f 6676 6572 273a 0a20 2020  'odoo_fver':.   
+0000dba0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0000dbb0: 7372 635f 6374 785b 2773 656c 5f6d 6f64  src_ctx['sel_mod
+0000dbc0: 656c 275d 3a0a 2020 2020 2020 2020 2020  el']:.          
+0000dbd0: 2020 2020 2020 7467 745f 6374 785b 7467        tgt_ctx[tg
+0000dbe0: 745f 7061 7261 6d5d 203d 2073 7263 5f63  t_param] = src_c
+0000dbf0: 7478 5b73 7263 5f70 6172 616d 5d2e 7265  tx[src_param].re
+0000dc00: 706c 6163 6528 0a20 2020 2020 2020 2020  place(.         
+0000dc10: 2020 2020 2020 2020 2020 2073 7472 2873             str(s
+0000dc20: 7263 5f63 7478 5b27 7372 635f 6f64 6f6f  rc_ctx['src_odoo
+0000dc30: 5f76 6572 275d 292c 2073 7472 2874 6774  _ver']), str(tgt
+0000dc40: 5f63 7478 5b27 7467 745f 6f64 6f6f 5f76  _ctx['tgt_odoo_v
+0000dc50: 6572 275d 290a 2020 2020 2020 2020 2020  er']).          
+0000dc60: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000dc70: 656c 6966 2069 7465 6d20 3d3d 2027 7669  elif item == 'vi
+0000dc80: 6427 3a0a 2020 2020 2020 2020 2020 2020  d':.            
+0000dc90: 6966 206e 6f74 2073 7263 5f63 7478 5b27  if not src_ctx['
+0000dca0: 7365 6c5f 6d6f 6465 6c27 5d3a 0a20 2020  sel_model']:.   
+0000dcb0: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
+0000dcc0: 5f63 7478 5b74 6774 5f70 6172 616d 5d20  _ctx[tgt_param] 
+0000dcd0: 3d20 7372 635f 6374 785b 7372 635f 7061  = src_ctx[src_pa
+0000dce0: 7261 6d5d 2e72 6570 6c61 6365 280a 2020  ram].replace(.  
+0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd00: 2020 7374 7228 7372 635f 6374 785b 2773    str(src_ctx['s
+0000dd10: 7263 5f6f 646f 6f5f 7665 7227 5d29 2c20  rc_odoo_ver']), 
+0000dd20: 7374 7228 7467 745f 6374 785b 2774 6774  str(tgt_ctx['tgt
+0000dd30: 5f6f 646f 6f5f 7665 7227 5d29 0a20 2020  _odoo_ver']).   
+0000dd40: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000dd50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000dd60: 6620 7467 745f 6374 785b 7467 745f 7061  f tgt_ctx[tgt_pa
+0000dd70: 7261 6d5d 2e73 7461 7274 7377 6974 6828  ram].startswith(
+0000dd80: 2776 2729 3a0a 2020 2020 2020 2020 2020  'v'):.          
+0000dd90: 2020 2020 2020 2020 2020 7467 745f 6374            tgt_ct
+0000dda0: 785b 7467 745f 7061 7261 6d5d 203d 2074  x[tgt_param] = t
+0000ddb0: 6774 5f63 7478 5b27 7467 745f 6f64 6f6f  gt_ctx['tgt_odoo
+0000ddc0: 5f66 7665 7227 5d0a 2020 2020 2020 2020  _fver'].        
+0000ddd0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000dde0: 2020 2020 2020 2020 2020 7467 745f 6374            tgt_ct
+0000ddf0: 785b 7467 745f 7061 7261 6d5d 203d 2074  x[tgt_param] = t
+0000de00: 6774 5f63 7478 5b27 6669 6e61 6c5f 6272  gt_ctx['final_br
+0000de10: 616e 6368 275d 0a20 2020 2020 2020 2020  anch'].         
+0000de20: 2020 2020 2020 2074 6774 5f63 7478 5b27         tgt_ctx['
+0000de30: 7467 745f 6f64 6f6f 5f66 7665 7227 5d20  tgt_odoo_fver'] 
+0000de40: 3d20 636c 6f64 6f6f 2e62 7569 6c64 5f6f  = clodoo.build_o
+0000de50: 646f 6f5f 7061 7261 6d28 0a20 2020 2020  doo_param(.     
+0000de60: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000de70: 4655 4c4c 5645 5227 2c20 6f64 6f6f 5f76  FULLVER', odoo_v
+0000de80: 6964 3d74 6774 5f63 7478 5b27 6669 6e61  id=tgt_ctx['fina
+0000de90: 6c5f 6272 616e 6368 275d 2c20 6d75 6c74  l_branch'], mult
+0000dea0: 693d 5472 7565 0a20 2020 2020 2020 2020  i=True.         
+0000deb0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000dec0: 2020 2020 2020 2020 2074 6774 5f63 7478           tgt_ctx
+0000ded0: 5b27 7467 745f 6f64 6f6f 5f76 6572 275d  ['tgt_odoo_ver']
+0000dee0: 203d 2063 6c6f 646f 6f2e 6275 696c 645f   = clodoo.build_
+0000def0: 6f64 6f6f 5f70 6172 616d 280a 2020 2020  odoo_param(.    
+0000df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df10: 274d 414a 5645 5227 2c20 6f64 6f6f 5f76  'MAJVER', odoo_v
+0000df20: 6964 3d74 6774 5f63 7478 5b27 6669 6e61  id=tgt_ctx['fina
+0000df30: 6c5f 6272 616e 6368 275d 2c20 6d75 6c74  l_branch'], mult
+0000df40: 693d 5472 7565 0a20 2020 2020 2020 2020  i=True.         
+0000df50: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000df60: 2065 6c69 6620 6974 656d 203d 3d20 2763   elif item == 'c
+0000df70: 6f6e 665f 666e 273a 0a20 2020 2020 2020  onf_fn':.       
+0000df80: 2020 2020 2073 7263 5f63 6f6e 6669 6720       src_config 
+0000df90: 3d20 6765 745f 636f 6e66 6967 5f66 6e73  = get_config_fns
+0000dfa0: 2873 7263 5f63 7478 2c20 2773 7263 2729  (src_ctx, 'src')
+0000dfb0: 0a20 2020 2020 2020 2020 2020 2074 6774  .            tgt
+0000dfc0: 5f63 6f6e 6669 6720 3d20 6765 745f 636f  _config = get_co
+0000dfd0: 6e66 6967 5f66 6e73 2874 6774 5f63 7478  nfig_fns(tgt_ctx
+0000dfe0: 2c20 2774 6774 2729 0a20 2020 2020 2020  , 'tgt').       
+0000dff0: 2065 6c69 6620 6974 656d 203d 3d20 2773   elif item == 's
+0000e000: 7663 5f70 726f 746f 636f 6c27 3a0a 2020  vc_protocol':.  
+0000e010: 2020 2020 2020 2020 2020 7372 635f 6374            src_ct
+0000e020: 785b 2762 7261 6e63 6827 5d20 3d20 7372  x['branch'] = sr
+0000e030: 635f 6374 785b 2773 7263 5f6f 646f 6f5f  c_ctx['src_odoo_
+0000e040: 6676 6572 275d 0a20 2020 2020 2020 2020  fver'].         
+0000e050: 2020 2073 7263 5f63 7478 5b27 6f65 5f76     src_ctx['oe_v
+0000e060: 6572 7369 6f6e 275d 203d 2073 7263 5f63  ersion'] = src_c
+0000e070: 7478 5b27 7372 635f 6f64 6f6f 5f66 7665  tx['src_odoo_fve
+0000e080: 7227 5d0a 2020 2020 2020 2020 2020 2020  r'].            
+0000e090: 7372 635f 636f 6e66 6967 2e73 6574 2827  src_config.set('
+0000e0a0: 6f70 7469 6f6e 7327 2c20 276f 655f 7665  options', 'oe_ve
+0000e0b0: 7273 696f 6e27 2c20 7372 635f 6374 785b  rsion', src_ctx[
+0000e0c0: 276f 655f 7665 7273 696f 6e27 5d29 0a20  'oe_version']). 
+0000e0d0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0000e0e0: 7420 7372 635f 6374 782e 6765 7428 6974  t src_ctx.get(it
+0000e0f0: 656d 293a 0a20 2020 2020 2020 2020 2020  em):.           
+0000e100: 2020 2020 2069 6620 7372 635f 6374 785b       if src_ctx[
+0000e110: 276f 655f 7665 7273 696f 6e27 5d20 696e  'oe_version'] in
+0000e120: 2028 2736 2e31 272c 2027 372e 3027 2c20   ('6.1', '7.0', 
+0000e130: 2738 2e30 2729 3a0a 2020 2020 2020 2020  '8.0'):.        
+0000e140: 2020 2020 2020 2020 2020 2020 7372 635f              src_
+0000e150: 6374 785b 2773 7663 5f70 726f 746f 636f  ctx['svc_protoco
+0000e160: 6c27 5d20 3d20 2778 6d6c 7270 6327 0a20  l'] = 'xmlrpc'. 
+0000e170: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000e180: 6c69 6620 7372 635f 6374 785b 276f 655f  lif src_ctx['oe_
+0000e190: 7665 7273 696f 6e27 5d3a 0a20 2020 2020  version']:.     
+0000e1a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e1b0: 7263 5f63 7478 5b27 7376 635f 7072 6f74  rc_ctx['svc_prot
+0000e1c0: 6f63 6f6c 275d 203d 2027 6a73 6f6e 7270  ocol'] = 'jsonrp
+0000e1d0: 6327 0a20 2020 2020 2020 2020 2020 2074  c'.            t
+0000e1e0: 6774 5f63 7478 5b27 6272 616e 6368 275d  gt_ctx['branch']
+0000e1f0: 203d 2074 6774 5f63 7478 5b27 7467 745f   = tgt_ctx['tgt_
+0000e200: 6f64 6f6f 5f66 7665 7227 5d0a 2020 2020  odoo_fver'].    
+0000e210: 2020 2020 2020 2020 7467 745f 6374 785b          tgt_ctx[
+0000e220: 276f 655f 7665 7273 696f 6e27 5d20 3d20  'oe_version'] = 
+0000e230: 7467 745f 6374 785b 2774 6774 5f6f 646f  tgt_ctx['tgt_odo
+0000e240: 6f5f 6676 6572 275d 0a20 2020 2020 2020  o_fver'].       
+0000e250: 2020 2020 2074 6774 5f63 6f6e 6669 672e       tgt_config.
+0000e260: 7365 7428 276f 7074 696f 6e73 272c 2027  set('options', '
+0000e270: 6f65 5f76 6572 7369 6f6e 272c 2074 6774  oe_version', tgt
+0000e280: 5f63 7478 5b27 6f65 5f76 6572 7369 6f6e  _ctx['oe_version
+0000e290: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
+0000e2a0: 6966 2074 6774 5f63 7478 5b27 6f65 5f76  if tgt_ctx['oe_v
+0000e2b0: 6572 7369 6f6e 275d 2069 6e20 2827 362e  ersion'] in ('6.
+0000e2c0: 3127 2c20 2737 2e30 272c 2027 382e 3027  1', '7.0', '8.0'
+0000e2d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000e2e0: 2020 2074 6774 5f63 7478 5b27 7376 635f     tgt_ctx['svc_
+0000e2f0: 7072 6f74 6f63 6f6c 275d 203d 2027 786d  protocol'] = 'xm
+0000e300: 6c72 7063 270a 2020 2020 2020 2020 2020  lrpc'.          
+0000e310: 2020 656c 6966 2074 6774 5f63 7478 5b27    elif tgt_ctx['
+0000e320: 6f65 5f76 6572 7369 6f6e 275d 3a0a 2020  oe_version']:.  
+0000e330: 2020 2020 2020 2020 2020 2020 2020 7467                tg
+0000e340: 745f 6374 785b 2773 7663 5f70 726f 746f  t_ctx['svc_proto
+0000e350: 636f 6c27 5d20 3d20 276a 736f 6e72 7063  col'] = 'jsonrpc
+0000e360: 270a 2020 2020 2020 2020 656c 6966 2069  '.        elif i
+0000e370: 7465 6d20 3d3d 2027 6462 5f6e 616d 6527  tem == 'db_name'
+0000e380: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000e390: 2073 7263 5f63 7478 5b27 7372 635f 7669   src_ctx['src_vi
+0000e3a0: 6427 5d20 3d3d 2073 7263 5f63 7478 5b27  d'] == src_ctx['
+0000e3b0: 6672 6f6d 5f62 7261 6e63 6827 5d3a 0a20  from_branch']:. 
+0000e3c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e3d0: 7263 5f63 7478 5b69 7465 6d5d 203d 2073  rc_ctx[item] = s
+0000e3e0: 7263 5f63 7478 5b73 7263 5f70 6172 616d  rc_ctx[src_param
+0000e3f0: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
+0000e400: 2074 6774 5f63 7478 5b27 7467 745f 6f64   tgt_ctx['tgt_od
+0000e410: 6f6f 5f76 6572 275d 203d 3d20 7467 745f  oo_ver'] == tgt_
+0000e420: 6374 785b 2766 696e 616c 5f76 6572 275d  ctx['final_ver']
+0000e430: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e440: 2020 6966 2074 6774 5f63 7478 5b27 6669    if tgt_ctx['fi
+0000e450: 6e61 6c5f 6462 6e61 6d65 275d 3a0a 2020  nal_dbname']:.  
+0000e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e470: 2020 7467 745f 6374 785b 6974 656d 5d20    tgt_ctx[item] 
+0000e480: 3d20 7467 745f 6374 785b 2766 696e 616c  = tgt_ctx['final
+0000e490: 5f64 626e 616d 6527 5d0a 2020 2020 2020  _dbname'].      
+0000e4a0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4c0: 2020 2020 7467 745f 6374 785b 6974 656d      tgt_ctx[item
+0000e4d0: 5d20 3d20 6e65 775f 6462 6e61 6d65 280a  ] = new_dbname(.
+0000e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4f0: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
+0000e500: 6974 656d 5d2c 2074 6774 5f63 7478 5b27  item], tgt_ctx['
+0000e510: 7467 745f 6f64 6f6f 5f76 6572 275d 2c20  tgt_odoo_ver'], 
+0000e520: 7467 745f 6374 785b 276f 6361 5f6d 6967  tgt_ctx['oca_mig
+0000e530: 7261 7465 275d 0a20 2020 2020 2020 2020  rate'].         
+0000e540: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000e550: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000e560: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000e570: 6774 5f63 7478 5b69 7465 6d5d 203d 206e  gt_ctx[item] = n
+0000e580: 6577 5f64 626e 616d 6528 0a20 2020 2020  ew_dbname(.     
+0000e590: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000e5a0: 7263 5f63 7478 5b69 7465 6d5d 2c20 7467  rc_ctx[item], tg
+0000e5b0: 745f 6374 785b 2774 6774 5f6f 646f 6f5f  t_ctx['tgt_odoo_
+0000e5c0: 7665 7227 5d2c 2074 6774 5f63 7478 5b27  ver'], tgt_ctx['
+0000e5d0: 6f63 615f 6d69 6772 6174 6527 5d0a 2020  oca_migrate'].  
+0000e5e0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000e5f0: 2020 2020 2020 2020 656c 6966 2069 7465          elif ite
+0000e600: 6d20 3d3d 2027 6c65 7665 6c27 3a0a 2020  m == 'level':.  
+0000e610: 2020 2020 2020 2020 2020 7372 635f 6374            src_ct
+0000e620: 785b 6974 656d 5d20 3d20 4445 465f 434f  x[item] = DEF_CO
+0000e630: 4e46 5b69 7465 6d5d 0a20 2020 2020 2020  NF[item].       
+0000e640: 2020 2020 2074 6774 5f63 7478 5b69 7465       tgt_ctx[ite
+0000e650: 6d5d 203d 2044 4546 5f43 4f4e 465b 6974  m] = DEF_CONF[it
+0000e660: 656d 5d0a 2020 2020 2020 2020 656c 6966  em].        elif
+0000e670: 2069 7465 6d20 696e 2028 2764 625f 686f   item in ('db_ho
+0000e680: 7374 272c 2027 6462 5f75 7365 7227 2c20  st', 'db_user', 
+0000e690: 2764 625f 706f 7274 272c 2027 6462 5f70  'db_port', 'db_p
+0000e6a0: 6173 7377 6f72 6427 2c20 2778 6d6c 7270  assword', 'xmlrp
+0000e6b0: 635f 706f 7274 2729 3a0a 2020 2020 2020  c_port'):.      
+0000e6c0: 2020 2020 2020 6966 2073 7263 5f63 6f6e        if src_con
+0000e6d0: 6669 672e 6861 735f 6f70 7469 6f6e 2827  fig.has_option('
+0000e6e0: 6f70 7469 6f6e 7327 2c20 6974 656d 293a  options', item):
+0000e6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e700: 2073 7263 5f63 7478 5b69 7465 6d5d 203d   src_ctx[item] =
+0000e710: 2073 7263 5f63 6f6e 6669 672e 6765 7428   src_config.get(
+0000e720: 276f 7074 696f 6e73 272c 2069 7465 6d29  'options', item)
+0000e730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e740: 2069 6620 7372 635f 6374 785b 6974 656d   if src_ctx[item
+0000e750: 5d20 3d3d 2027 4661 6c73 6527 3a0a 2020  ] == 'False':.  
+0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e770: 2020 7372 635f 6374 785b 6974 656d 5d20    src_ctx[item] 
+0000e780: 3d20 4445 465f 434f 4e46 5b69 7465 6d5d  = DEF_CONF[item]
+0000e790: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000e7a0: 6620 6974 656d 203d 3d20 2764 625f 7573  f item == 'db_us
+0000e7b0: 6572 273a 0a20 2020 2020 2020 2020 2020  er':.           
+0000e7c0: 2020 2020 2073 7263 5f63 7478 5b69 7465       src_ctx[ite
+0000e7d0: 6d5d 203d 2027 6f64 6f6f 270a 2020 2020  m] = 'odoo'.    
+0000e7e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000e7f0: 2020 2020 2020 2020 2020 2020 2020 7372                sr
+0000e800: 635f 6374 785b 6974 656d 5d20 3d20 4445  c_ctx[item] = DE
+0000e810: 465f 434f 4e46 5b69 7465 6d5d 0a20 2020  F_CONF[item].   
+0000e820: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+0000e830: 7374 616e 6365 2873 7263 5f63 7478 5b69  stance(src_ctx[i
+0000e840: 7465 6d5d 2c20 6261 7365 7374 7269 6e67  tem], basestring
+0000e850: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000e860: 2020 2073 7263 5f63 6f6e 6669 672e 7365     src_config.se
+0000e870: 7428 276f 7074 696f 6e73 272c 2069 7465  t('options', ite
+0000e880: 6d2c 2073 7263 5f63 7478 5b69 7465 6d5d  m, src_ctx[item]
+0000e890: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000e8a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000e8b0: 2020 2020 7372 635f 636f 6e66 6967 2e73      src_config.s
+0000e8c0: 6574 2827 6f70 7469 6f6e 7327 2c20 6974  et('options', it
+0000e8d0: 656d 2c20 7374 7228 7372 635f 6374 785b  em, str(src_ctx[
+0000e8e0: 6974 656d 5d29 290a 2020 2020 2020 2020  item])).        
+0000e8f0: 2020 2020 6966 2074 6774 5f63 6f6e 6669      if tgt_confi
+0000e900: 672e 6861 735f 6f70 7469 6f6e 2827 6f70  g.has_option('op
+0000e910: 7469 6f6e 7327 2c20 6974 656d 293a 0a20  tions', item):. 
+0000e920: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000e930: 6774 5f63 7478 5b69 7465 6d5d 203d 2074  gt_ctx[item] = t
+0000e940: 6774 5f63 6f6e 6669 672e 6765 7428 276f  gt_config.get('o
+0000e950: 7074 696f 6e73 272c 2069 7465 6d29 0a20  ptions', item). 
+0000e960: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000e970: 6620 7467 745f 6374 785b 6974 656d 5d20  f tgt_ctx[item] 
+0000e980: 3d3d 2027 4661 6c73 6527 3a0a 2020 2020  == 'False':.    
+0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9a0: 7467 745f 6374 785b 6974 656d 5d20 3d20  tgt_ctx[item] = 
+0000e9b0: 4445 465f 434f 4e46 5b69 7465 6d5d 0a20  DEF_CONF[item]. 
+0000e9c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000e9d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e9e0: 2074 6774 5f63 7478 5b69 7465 6d5d 203d   tgt_ctx[item] =
+0000e9f0: 2044 4546 5f43 4f4e 465b 6974 656d 5d0a   DEF_CONF[item].
+0000ea00: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0000ea10: 7369 6e73 7461 6e63 6528 7467 745f 6374  sinstance(tgt_ct
+0000ea20: 785b 6974 656d 5d2c 2062 6173 6573 7472  x[item], basestr
+0000ea30: 696e 6729 3a0a 2020 2020 2020 2020 2020  ing):.          
+0000ea40: 2020 2020 2020 7467 745f 636f 6e66 6967        tgt_config
+0000ea50: 2e73 6574 2827 6f70 7469 6f6e 7327 2c20  .set('options', 
+0000ea60: 6974 656d 2c20 7467 745f 6374 785b 6974  item, tgt_ctx[it
+0000ea70: 656d 5d29 0a20 2020 2020 2020 2020 2020  em]).           
+0000ea80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000ea90: 2020 2020 2020 2074 6774 5f63 6f6e 6669         tgt_confi
+0000eaa0: 672e 7365 7428 276f 7074 696f 6e73 272c  g.set('options',
+0000eab0: 2069 7465 6d2c 2073 7472 2874 6774 5f63   item, str(tgt_c
+0000eac0: 7478 5b69 7465 6d5d 2929 0a20 2020 2020  tx[item])).     
+0000ead0: 2020 2065 6c69 6620 6974 656d 203d 3d20     elif item == 
+0000eae0: 2770 7379 636f 7067 3227 3a0a 2020 2020  'psycopg2':.    
+0000eaf0: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
+0000eb00: 6974 656d 5d20 3d20 2754 7275 6527 0a20  item] = 'True'. 
+0000eb10: 2020 2020 2020 2020 2020 2073 7263 5f63             src_c
+0000eb20: 6f6e 6669 672e 7365 7428 276f 7074 696f  onfig.set('optio
+0000eb30: 6e73 272c 2069 7465 6d2c 2073 7472 2873  ns', item, str(s
+0000eb40: 7263 5f63 7478 5b69 7465 6d5d 2929 0a20  rc_ctx[item])). 
+0000eb50: 2020 2020 2020 2020 2020 2074 6774 5f63             tgt_c
+0000eb60: 7478 5b69 7465 6d5d 203d 2027 5472 7565  tx[item] = 'True
+0000eb70: 270a 2020 2020 2020 2020 2020 2020 7467  '.            tg
+0000eb80: 745f 636f 6e66 6967 2e73 6574 2827 6f70  t_config.set('op
+0000eb90: 7469 6f6e 7327 2c20 6974 656d 2c20 7374  tions', item, st
+0000eba0: 7228 7467 745f 6374 785b 6974 656d 5d29  r(tgt_ctx[item])
+0000ebb0: 290a 2020 2020 2020 2020 656c 6966 2069  ).        elif i
+0000ebc0: 7465 6d20 3d3d 2027 6c6f 6766 696c 6527  tem == 'logfile'
+0000ebd0: 3a0a 2020 2020 2020 2020 2020 2020 7372  :.            sr
+0000ebe0: 635f 636f 6e66 6967 2e73 6574 2827 6f70  c_config.set('op
+0000ebf0: 7469 6f6e 7327 2c20 6974 656d 2c20 7374  tions', item, st
+0000ec00: 7228 7372 635f 6374 785b 6974 656d 5d29  r(src_ctx[item])
+0000ec10: 290a 2020 2020 2020 2020 2020 2020 7467  ).            tg
+0000ec20: 745f 636f 6e66 6967 2e73 6574 2827 6f70  t_config.set('op
+0000ec30: 7469 6f6e 7327 2c20 6974 656d 2c20 7374  tions', item, st
+0000ec40: 7228 7467 745f 6374 785b 6974 656d 5d29  r(tgt_ctx[item])
+0000ec50: 290a 2020 2020 2020 2020 656c 6966 2069  ).        elif i
+0000ec60: 7465 6d20 3d3d 2027 6c6f 6769 6e5f 7573  tem == 'login_us
+0000ec70: 6572 273a 0a20 2020 2020 2020 2020 2020  er':.           
+0000ec80: 2069 6620 7372 635f 636f 6e66 6967 2e68   if src_config.h
+0000ec90: 6173 5f6f 7074 696f 6e28 276f 7074 696f  as_option('optio
+0000eca0: 6e73 272c 2069 7465 6d29 3a0a 2020 2020  ns', item):.    
+0000ecb0: 2020 2020 2020 2020 2020 2020 7372 635f              src_
+0000ecc0: 6374 785b 6974 656d 5d20 3d20 7372 635f  ctx[item] = src_
+0000ecd0: 636f 6e66 6967 2e67 6574 2827 6f70 7469  config.get('opti
+0000ece0: 6f6e 7327 2c20 6974 656d 290a 2020 2020  ons', item).    
+0000ecf0: 2020 2020 2020 2020 656c 6966 2073 7263          elif src
+0000ed00: 5f63 7478 2e67 6574 2869 7465 6d29 3a0a  _ctx.get(item):.
+0000ed10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed20: 7372 635f 636f 6e66 6967 2e73 6574 2827  src_config.set('
+0000ed30: 6f70 7469 6f6e 7327 2c20 6974 656d 2c20  options', item, 
+0000ed40: 7372 635f 6374 785b 6974 656d 5d29 0a20  src_ctx[item]). 
+0000ed50: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0000ed60: 7372 635f 6374 782e 6765 7428 276c 6769  src_ctx.get('lgi
+0000ed70: 5f75 7365 7227 293a 0a20 2020 2020 2020  _user'):.       
+0000ed80: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
+0000ed90: 5b69 7465 6d5d 203d 2073 7263 5f63 7478  [item] = src_ctx
+0000eda0: 5b27 6c67 695f 7573 6572 275d 0a20 2020  ['lgi_user'].   
+0000edb0: 2020 2020 2020 2020 2020 2020 2073 7263               src
+0000edc0: 5f63 6f6e 6669 672e 7365 7428 276f 7074  _config.set('opt
+0000edd0: 696f 6e73 272c 2069 7465 6d2c 2073 7263  ions', item, src
+0000ede0: 5f63 7478 5b69 7465 6d5d 290a 2020 2020  _ctx[item]).    
+0000edf0: 2020 2020 2020 2020 6966 2074 6774 5f63          if tgt_c
+0000ee00: 6f6e 6669 672e 6861 735f 6f70 7469 6f6e  onfig.has_option
+0000ee10: 2827 6f70 7469 6f6e 7327 2c20 6974 656d  ('options', item
+0000ee20: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000ee30: 2020 2074 6774 5f63 7478 5b69 7465 6d5d     tgt_ctx[item]
+0000ee40: 203d 2074 6774 5f63 6f6e 6669 672e 6765   = tgt_config.ge
+0000ee50: 7428 276f 7074 696f 6e73 272c 2069 7465  t('options', ite
+0000ee60: 6d29 0a20 2020 2020 2020 2020 2020 2065  m).            e
+0000ee70: 6c69 6620 7467 745f 6374 782e 6765 7428  lif tgt_ctx.get(
+0000ee80: 6974 656d 2920 616e 6420 7467 745f 6374  item) and tgt_ct
+0000ee90: 785b 6974 656d 5d20 213d 2027 6164 6d69  x[item] != 'admi
+0000eea0: 6e27 3a0a 2020 2020 2020 2020 2020 2020  n':.            
+0000eeb0: 2020 2020 7467 745f 636f 6e66 6967 2e73      tgt_config.s
+0000eec0: 6574 2827 6f70 7469 6f6e 7327 2c20 6974  et('options', it
+0000eed0: 656d 2c20 7467 745f 6374 785b 6974 656d  em, tgt_ctx[item
+0000eee0: 5d29 0a20 2020 2020 2020 2020 2020 2065  ]).            e
+0000eef0: 6c69 6620 7467 745f 6374 782e 6765 7428  lif tgt_ctx.get(
+0000ef00: 276c 6769 5f75 7365 7227 2920 616e 6420  'lgi_user') and 
+0000ef10: 7467 745f 6374 785b 276c 6769 5f75 7365  tgt_ctx['lgi_use
+0000ef20: 7227 5d20 213d 2027 6164 6d69 6e27 3a0a  r'] != 'admin':.
+0000ef30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef40: 7467 745f 6374 785b 6974 656d 5d20 3d20  tgt_ctx[item] = 
+0000ef50: 7467 745f 6374 785b 276c 6769 5f75 7365  tgt_ctx['lgi_use
+0000ef60: 7227 5d0a 2020 2020 2020 2020 2020 2020  r'].            
+0000ef70: 2020 2020 7467 745f 636f 6e66 6967 2e73      tgt_config.s
+0000ef80: 6574 2827 6f70 7469 6f6e 7327 2c20 6974  et('options', it
+0000ef90: 656d 2c20 7467 745f 6374 785b 6974 656d  em, tgt_ctx[item
+0000efa0: 5d29 0a20 2020 2020 2020 2020 2020 2065  ]).            e
+0000efb0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000efc0: 2020 2020 2074 6774 5f63 7478 5b69 7465       tgt_ctx[ite
+0000efd0: 6d5d 203d 2073 7263 5f63 7478 5b69 7465  m] = src_ctx[ite
+0000efe0: 6d5d 0a20 2020 2020 2020 2020 2020 2020  m].             
+0000eff0: 2020 2074 6774 5f63 6f6e 6669 672e 7365     tgt_config.se
+0000f000: 7428 276f 7074 696f 6e73 272c 2069 7465  t('options', ite
+0000f010: 6d2c 2074 6774 5f63 7478 5b69 7465 6d5d  m, tgt_ctx[item]
+0000f020: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0000f030: 756e 645f 7077 6420 3d20 4661 6c73 650a  und_pwd = False.
+0000f040: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000f050: 6e6d 2069 6e20 2827 6372 7970 745f 7061  nm in ('crypt_pa
+0000f060: 7373 776f 7264 272c 2027 6c6f 6769 6e5f  ssword', 'login_
+0000f070: 7061 7373 776f 7264 2729 3a0a 2020 2020  password'):.    
+0000f080: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000f090: 7263 5f63 7478 2e67 6574 286e 6d29 3a0a  rc_ctx.get(nm):.
+0000f0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0b0: 2020 2020 7372 635f 636f 6e66 6967 2e73      src_config.s
+0000f0c0: 6574 2827 6f70 7469 6f6e 7327 2c20 6e6d  et('options', nm
+0000f0d0: 2c20 7372 635f 6374 785b 6e6d 5d29 0a20  , src_ctx[nm]). 
 0000f0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f100: 7467 745f 6374 785b 2774 6774 5f6f 646f  tgt_ctx['tgt_odo
-0000f110: 6f5f 7665 7227 5d2c 0a20 2020 2020 2020  o_ver'],.       
-0000f120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f140: 2020 2020 7467 745f 6374 785b 276f 6361      tgt_ctx['oca
-0000f150: 5f6d 6967 7261 7465 275d 290a 2020 2020  _migrate']).    
-0000f160: 2020 2020 656c 6966 2069 7465 6d20 3d3d      elif item ==
-0000f170: 2027 6c65 7665 6c27 3a0a 2020 2020 2020   'level':.      
-0000f180: 2020 2020 2020 7372 635f 6374 785b 6974        src_ctx[it
-0000f190: 656d 5d20 3d20 4445 465f 434f 4e46 5b69  em] = DEF_CONF[i
-0000f1a0: 7465 6d5d 0a20 2020 2020 2020 2020 2020  tem].           
-0000f1b0: 2074 6774 5f63 7478 5b69 7465 6d5d 203d   tgt_ctx[item] =
-0000f1c0: 2044 4546 5f43 4f4e 465b 6974 656d 5d0a   DEF_CONF[item].
-0000f1d0: 2020 2020 2020 2020 656c 6966 2069 7465          elif ite
-0000f1e0: 6d20 696e 2028 2764 625f 686f 7374 272c  m in ('db_host',
-0000f1f0: 2027 6462 5f75 7365 7227 2c20 2764 625f   'db_user', 'db_
-0000f200: 706f 7274 272c 2027 6462 5f70 6173 7377  port', 'db_passw
-0000f210: 6f72 6427 2c0a 2020 2020 2020 2020 2020  ord',.          
-0000f220: 2020 2020 2020 2020 2020 2020 2778 6d6c              'xml
-0000f230: 7270 635f 706f 7274 2729 3a0a 2020 2020  rpc_port'):.    
-0000f240: 2020 2020 2020 2020 6966 2073 7263 5f63          if src_c
-0000f250: 6f6e 6669 672e 6861 735f 6f70 7469 6f6e  onfig.has_option
-0000f260: 2827 6f70 7469 6f6e 7327 2c20 6974 656d  ('options', item
-0000f270: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000f280: 2020 2073 7263 5f63 7478 5b69 7465 6d5d     src_ctx[item]
-0000f290: 203d 2073 7263 5f63 6f6e 6669 672e 6765   = src_config.ge
-0000f2a0: 7428 276f 7074 696f 6e73 272c 2069 7465  t('options', ite
-0000f2b0: 6d29 0a20 2020 2020 2020 2020 2020 2020  m).             
-0000f2c0: 2020 2069 6620 7372 635f 6374 785b 6974     if src_ctx[it
-0000f2d0: 656d 5d20 3d3d 2027 4661 6c73 6527 3a0a  em] == 'False':.
+0000f0f0: 2020 2066 6f75 6e64 5f70 7764 203d 2054     found_pwd = T
+0000f100: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0000f110: 2020 2020 656c 6966 2073 7263 5f63 6f6e      elif src_con
+0000f120: 6669 672e 6861 735f 6f70 7469 6f6e 2827  fig.has_option('
+0000f130: 6f70 7469 6f6e 7327 2c20 6e6d 293a 0a20  options', nm):. 
+0000f140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f150: 2020 2073 7263 5f63 7478 5b6e 6d5d 203d     src_ctx[nm] =
+0000f160: 2073 7263 5f63 6f6e 6669 672e 6765 7428   src_config.get(
+0000f170: 276f 7074 696f 6e73 272c 206e 6d29 0a20  'options', nm). 
+0000f180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f190: 2020 2066 6f75 6e64 5f70 7764 203d 2054     found_pwd = T
+0000f1a0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0000f1b0: 2020 2020 656c 6966 206e 6f74 2066 6f75      elif not fou
+0000f1c0: 6e64 5f70 7764 3a0a 2020 2020 2020 2020  nd_pwd:.        
+0000f1d0: 2020 2020 2020 2020 2020 2020 7372 635f              src_
+0000f1e0: 6374 785b 276c 6f67 696e 5f70 6173 7377  ctx['login_passw
+0000f1f0: 6f72 6427 5d20 3d20 6765 7470 6173 732e  ord'] = getpass.
+0000f200: 6765 7470 6173 7328 0a20 2020 2020 2020  getpass(.       
+0000f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f220: 2027 5061 7373 776f 7264 2066 6f72 206c   'Password for l
+0000f230: 6f67 696e 2075 7365 7220 2573 3a20 2720  ogin user %s: ' 
+0000f240: 2520 7372 635f 6374 785b 276c 6769 5f75  % src_ctx['lgi_u
+0000f250: 7365 7227 5d0a 2020 2020 2020 2020 2020  ser'].          
+0000f260: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000f270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f280: 7372 635f 636f 6e66 6967 2e73 6574 280a  src_config.set(.
+0000f290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2a0: 2020 2020 2020 2020 276f 7074 696f 6e73          'options
+0000f2b0: 272c 2027 6c6f 6769 6e5f 7061 7373 776f  ', 'login_passwo
+0000f2c0: 7264 272c 2073 7263 5f63 7478 5b27 6c6f  rd', src_ctx['lo
+0000f2d0: 6769 6e5f 7061 7373 776f 7264 275d 0a20  gin_password']. 
 0000f2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2f0: 2020 2020 7372 635f 6374 785b 6974 656d      src_ctx[item
-0000f300: 5d20 3d20 4445 465f 434f 4e46 5b69 7465  ] = DEF_CONF[ite
-0000f310: 6d5d 0a20 2020 2020 2020 2020 2020 2065  m].            e
-0000f320: 6c69 6620 6974 656d 203d 3d20 2764 625f  lif item == 'db_
-0000f330: 7573 6572 273a 0a20 2020 2020 2020 2020  user':.         
-0000f340: 2020 2020 2020 2073 7263 5f63 7478 5b69         src_ctx[i
-0000f350: 7465 6d5d 203d 2027 6f64 6f6f 270a 2020  tem] = 'odoo'.  
-0000f360: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f380: 7372 635f 6374 785b 6974 656d 5d20 3d20  src_ctx[item] = 
-0000f390: 4445 465f 434f 4e46 5b69 7465 6d5d 0a20  DEF_CONF[item]. 
-0000f3a0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-0000f3b0: 696e 7374 616e 6365 2873 7263 5f63 7478  instance(src_ctx
-0000f3c0: 5b69 7465 6d5d 2c20 6261 7365 7374 7269  [item], basestri
-0000f3d0: 6e67 293a 0a20 2020 2020 2020 2020 2020  ng):.           
-0000f3e0: 2020 2020 2073 7263 5f63 6f6e 6669 672e       src_config.
-0000f3f0: 7365 7428 276f 7074 696f 6e73 272c 2069  set('options', i
-0000f400: 7465 6d2c 2073 7263 5f63 7478 5b69 7465  tem, src_ctx[ite
-0000f410: 6d5d 290a 2020 2020 2020 2020 2020 2020  m]).            
-0000f420: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000f430: 2020 2020 2020 7372 635f 636f 6e66 6967        src_config
-0000f440: 2e73 6574 2827 6f70 7469 6f6e 7327 2c20  .set('options', 
-0000f450: 6974 656d 2c20 7374 7228 7372 635f 6374  item, str(src_ct
-0000f460: 785b 6974 656d 5d29 290a 2020 2020 2020  x[item])).      
-0000f470: 2020 2020 2020 6966 2074 6774 5f63 6f6e        if tgt_con
-0000f480: 6669 672e 6861 735f 6f70 7469 6f6e 2827  fig.has_option('
-0000f490: 6f70 7469 6f6e 7327 2c20 6974 656d 293a  options', item):
-0000f4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f4b0: 2074 6774 5f63 7478 5b69 7465 6d5d 203d   tgt_ctx[item] =
-0000f4c0: 2074 6774 5f63 6f6e 6669 672e 6765 7428   tgt_config.get(
-0000f4d0: 276f 7074 696f 6e73 272c 2069 7465 6d29  'options', item)
-0000f4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f4f0: 2069 6620 7467 745f 6374 785b 6974 656d   if tgt_ctx[item
-0000f500: 5d20 3d3d 2027 4661 6c73 6527 3a0a 2020  ] == 'False':.  
-0000f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f520: 2020 7467 745f 6374 785b 6974 656d 5d20    tgt_ctx[item] 
-0000f530: 3d20 4445 465f 434f 4e46 5b69 7465 6d5d  = DEF_CONF[item]
-0000f540: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000f550: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000f560: 2020 2074 6774 5f63 7478 5b69 7465 6d5d     tgt_ctx[item]
-0000f570: 203d 2044 4546 5f43 4f4e 465b 6974 656d   = DEF_CONF[item
-0000f580: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
-0000f590: 2069 7369 6e73 7461 6e63 6528 7467 745f   isinstance(tgt_
-0000f5a0: 6374 785b 6974 656d 5d2c 2062 6173 6573  ctx[item], bases
-0000f5b0: 7472 696e 6729 3a0a 2020 2020 2020 2020  tring):.        
-0000f5c0: 2020 2020 2020 2020 7467 745f 636f 6e66          tgt_conf
-0000f5d0: 6967 2e73 6574 2827 6f70 7469 6f6e 7327  ig.set('options'
-0000f5e0: 2c20 6974 656d 2c20 7467 745f 6374 785b  , item, tgt_ctx[
-0000f5f0: 6974 656d 5d29 0a20 2020 2020 2020 2020  item]).         
-0000f600: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000f610: 2020 2020 2020 2020 2074 6774 5f63 6f6e           tgt_con
-0000f620: 6669 672e 7365 7428 276f 7074 696f 6e73  fig.set('options
-0000f630: 272c 2069 7465 6d2c 2073 7472 2874 6774  ', item, str(tgt
-0000f640: 5f63 7478 5b69 7465 6d5d 2929 0a20 2020  _ctx[item])).   
-0000f650: 2020 2020 2065 6c69 6620 6974 656d 203d       elif item =
-0000f660: 3d20 2770 7379 636f 7067 3227 3a0a 2020  = 'psycopg2':.  
-0000f670: 2020 2020 2020 2020 2020 7372 635f 6374            src_ct
-0000f680: 785b 6974 656d 5d20 3d20 2754 7275 6527  x[item] = 'True'
-0000f690: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
-0000f6a0: 5f63 6f6e 6669 672e 7365 7428 276f 7074  _config.set('opt
-0000f6b0: 696f 6e73 272c 2069 7465 6d2c 2073 7472  ions', item, str
-0000f6c0: 2873 7263 5f63 7478 5b69 7465 6d5d 2929  (src_ctx[item]))
-0000f6d0: 0a20 2020 2020 2020 2020 2020 2074 6774  .            tgt
-0000f6e0: 5f63 7478 5b69 7465 6d5d 203d 2027 5472  _ctx[item] = 'Tr
-0000f6f0: 7565 270a 2020 2020 2020 2020 2020 2020  ue'.            
-0000f700: 7467 745f 636f 6e66 6967 2e73 6574 2827  tgt_config.set('
-0000f710: 6f70 7469 6f6e 7327 2c20 6974 656d 2c20  options', item, 
-0000f720: 7374 7228 7467 745f 6374 785b 6974 656d  str(tgt_ctx[item
-0000f730: 5d29 290a 2020 2020 2020 2020 656c 6966  ])).        elif
-0000f740: 2069 7465 6d20 3d3d 2027 6c6f 6766 696c   item == 'logfil
-0000f750: 6527 3a0a 2020 2020 2020 2020 2020 2020  e':.            
-0000f760: 7372 635f 636f 6e66 6967 2e73 6574 2827  src_config.set('
-0000f770: 6f70 7469 6f6e 7327 2c20 6974 656d 2c20  options', item, 
-0000f780: 7374 7228 7372 635f 6374 785b 6974 656d  str(src_ctx[item
-0000f790: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
-0000f7a0: 7467 745f 636f 6e66 6967 2e73 6574 2827  tgt_config.set('
-0000f7b0: 6f70 7469 6f6e 7327 2c20 6974 656d 2c20  options', item, 
-0000f7c0: 7374 7228 7467 745f 6374 785b 6974 656d  str(tgt_ctx[item
-0000f7d0: 5d29 290a 2020 2020 2020 2020 656c 6966  ])).        elif
-0000f7e0: 2069 7465 6d20 3d3d 2027 6c6f 6769 6e5f   item == 'login_
-0000f7f0: 7573 6572 273a 0a20 2020 2020 2020 2020  user':.         
-0000f800: 2020 2069 6620 7372 635f 636f 6e66 6967     if src_config
-0000f810: 2e68 6173 5f6f 7074 696f 6e28 276f 7074  .has_option('opt
-0000f820: 696f 6e73 272c 2069 7465 6d29 3a0a 2020  ions', item):.  
-0000f830: 2020 2020 2020 2020 2020 2020 2020 7372                sr
-0000f840: 635f 6374 785b 6974 656d 5d20 3d20 7372  c_ctx[item] = sr
-0000f850: 635f 636f 6e66 6967 2e67 6574 2827 6f70  c_config.get('op
-0000f860: 7469 6f6e 7327 2c20 6974 656d 290a 2020  tions', item).  
-0000f870: 2020 2020 2020 2020 2020 656c 6966 2073            elif s
-0000f880: 7263 5f63 7478 2e67 6574 2869 7465 6d29  rc_ctx.get(item)
-0000f890: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f8a0: 2020 7372 635f 636f 6e66 6967 2e73 6574    src_config.set
-0000f8b0: 2827 6f70 7469 6f6e 7327 2c20 6974 656d  ('options', item
-0000f8c0: 2c20 7372 635f 6374 785b 6974 656d 5d29  , src_ctx[item])
-0000f8d0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-0000f8e0: 6620 7372 635f 6374 782e 6765 7428 276c  f src_ctx.get('l
-0000f8f0: 6769 5f75 7365 7227 293a 0a20 2020 2020  gi_user'):.     
-0000f900: 2020 2020 2020 2020 2020 2073 7263 5f63             src_c
-0000f910: 7478 5b69 7465 6d5d 203d 2073 7263 5f63  tx[item] = src_c
-0000f920: 7478 5b27 6c67 695f 7573 6572 275d 0a20  tx['lgi_user']. 
-0000f930: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f940: 7263 5f63 6f6e 6669 672e 7365 7428 276f  rc_config.set('o
-0000f950: 7074 696f 6e73 272c 2069 7465 6d2c 2073  ptions', item, s
-0000f960: 7263 5f63 7478 5b69 7465 6d5d 290a 2020  rc_ctx[item]).  
-0000f970: 2020 2020 2020 2020 2020 6966 2074 6774            if tgt
-0000f980: 5f63 6f6e 6669 672e 6861 735f 6f70 7469  _config.has_opti
-0000f990: 6f6e 2827 6f70 7469 6f6e 7327 2c20 6974  on('options', it
-0000f9a0: 656d 293a 0a20 2020 2020 2020 2020 2020  em):.           
-0000f9b0: 2020 2020 2074 6774 5f63 7478 5b69 7465       tgt_ctx[ite
-0000f9c0: 6d5d 203d 2074 6774 5f63 6f6e 6669 672e  m] = tgt_config.
-0000f9d0: 6765 7428 276f 7074 696f 6e73 272c 2069  get('options', i
-0000f9e0: 7465 6d29 0a20 2020 2020 2020 2020 2020  tem).           
-0000f9f0: 2065 6c69 6620 7467 745f 6374 782e 6765   elif tgt_ctx.ge
-0000fa00: 7428 6974 656d 2920 616e 6420 7467 745f  t(item) and tgt_
-0000fa10: 6374 785b 6974 656d 5d20 213d 2027 6164  ctx[item] != 'ad
-0000fa20: 6d69 6e27 3a0a 2020 2020 2020 2020 2020  min':.          
-0000fa30: 2020 2020 2020 7467 745f 636f 6e66 6967        tgt_config
-0000fa40: 2e73 6574 2827 6f70 7469 6f6e 7327 2c20  .set('options', 
-0000fa50: 6974 656d 2c20 7467 745f 6374 785b 6974  item, tgt_ctx[it
-0000fa60: 656d 5d29 0a20 2020 2020 2020 2020 2020  em]).           
-0000fa70: 2065 6c69 6620 7467 745f 6374 782e 6765   elif tgt_ctx.ge
-0000fa80: 7428 276c 6769 5f75 7365 7227 2920 616e  t('lgi_user') an
-0000fa90: 6420 7467 745f 6374 785b 276c 6769 5f75  d tgt_ctx['lgi_u
-0000faa0: 7365 7227 5d20 213d 2027 6164 6d69 6e27  ser'] != 'admin'
-0000fab0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000fac0: 2020 7467 745f 6374 785b 6974 656d 5d20    tgt_ctx[item] 
-0000fad0: 3d20 7467 745f 6374 785b 276c 6769 5f75  = tgt_ctx['lgi_u
-0000fae0: 7365 7227 5d0a 2020 2020 2020 2020 2020  ser'].          
-0000faf0: 2020 2020 2020 7467 745f 636f 6e66 6967        tgt_config
-0000fb00: 2e73 6574 2827 6f70 7469 6f6e 7327 2c20  .set('options', 
-0000fb10: 6974 656d 2c20 7467 745f 6374 785b 6974  item, tgt_ctx[it
-0000fb20: 656d 5d29 0a20 2020 2020 2020 2020 2020  em]).           
-0000fb30: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000fb40: 2020 2020 2020 2074 6774 5f63 7478 5b69         tgt_ctx[i
-0000fb50: 7465 6d5d 203d 2073 7263 5f63 7478 5b69  tem] = src_ctx[i
-0000fb60: 7465 6d5d 0a20 2020 2020 2020 2020 2020  tem].           
-0000fb70: 2020 2020 2074 6774 5f63 6f6e 6669 672e       tgt_config.
-0000fb80: 7365 7428 276f 7074 696f 6e73 272c 2069  set('options', i
-0000fb90: 7465 6d2c 2074 6774 5f63 7478 5b69 7465  tem, tgt_ctx[ite
-0000fba0: 6d5d 290a 2020 2020 2020 2020 2020 2020  m]).            
-0000fbb0: 666f 756e 645f 7077 6420 3d20 4661 6c73  found_pwd = Fals
-0000fbc0: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
-0000fbd0: 7220 6e6d 2069 6e20 2827 6372 7970 745f  r nm in ('crypt_
-0000fbe0: 7061 7373 776f 7264 272c 2027 6c6f 6769  password', 'logi
-0000fbf0: 6e5f 7061 7373 776f 7264 2729 3a0a 2020  n_password'):.  
-0000fc00: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000fc10: 2073 7263 5f63 7478 2e67 6574 286e 6d29   src_ctx.get(nm)
-0000fc20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000fc30: 2020 2020 2020 7372 635f 636f 6e66 6967        src_config
-0000fc40: 2e73 6574 2827 6f70 7469 6f6e 7327 2c20  .set('options', 
-0000fc50: 6e6d 2c20 7372 635f 6374 785b 6e6d 5d29  nm, src_ctx[nm])
-0000fc60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fc70: 2020 2020 2066 6f75 6e64 5f70 7764 203d       found_pwd =
-0000fc80: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-0000fc90: 2020 2020 2020 656c 6966 2073 7263 5f63        elif src_c
-0000fca0: 6f6e 6669 672e 6861 735f 6f70 7469 6f6e  onfig.has_option
-0000fcb0: 2827 6f70 7469 6f6e 7327 2c20 6e6d 293a  ('options', nm):
-0000fcc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fcd0: 2020 2020 2073 7263 5f63 7478 5b6e 6d5d       src_ctx[nm]
-0000fce0: 203d 2073 7263 5f63 6f6e 6669 672e 6765   = src_config.ge
-0000fcf0: 7428 276f 7074 696f 6e73 272c 206e 6d29  t('options', nm)
-0000fd00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fd10: 2020 2020 2066 6f75 6e64 5f70 7764 203d       found_pwd =
-0000fd20: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-0000fd30: 2020 2020 2020 656c 6966 206e 6f74 2066        elif not f
-0000fd40: 6f75 6e64 5f70 7764 3a0a 2020 2020 2020  ound_pwd:.      
-0000fd50: 2020 2020 2020 2020 2020 2020 2020 7372                sr
-0000fd60: 635f 6374 785b 276c 6f67 696e 5f70 6173  c_ctx['login_pas
-0000fd70: 7377 6f72 6427 5d20 3d20 6765 7470 6173  sword'] = getpas
-0000fd80: 732e 6765 7470 6173 7328 0a20 2020 2020  s.getpass(.     
-0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fda0: 2020 2020 2020 2027 5061 7373 776f 7264         'Password
-0000fdb0: 2066 6f72 206c 6f67 696e 2075 7365 7220   for login user 
-0000fdc0: 2573 3a20 2720 250a 2020 2020 2020 2020  %s: ' %.        
-0000fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fde0: 2020 2020 7372 635f 6374 785b 276c 6769      src_ctx['lgi
-0000fdf0: 5f75 7365 7227 5d29 0a20 2020 2020 2020  _user']).       
-0000fe00: 2020 2020 2020 2020 2020 2020 2073 7263               src
-0000fe10: 5f63 6f6e 6669 672e 7365 7428 276f 7074  _config.set('opt
-0000fe20: 696f 6e73 272c 2027 6c6f 6769 6e5f 7061  ions', 'login_pa
-0000fe30: 7373 776f 7264 272c 0a20 2020 2020 2020  ssword',.       
-0000fe40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe50: 2020 2020 2020 2020 2020 2020 7372 635f              src_
-0000fe60: 6374 785b 276c 6f67 696e 5f70 6173 7377  ctx['login_passw
-0000fe70: 6f72 6427 5d29 0a20 2020 2020 2020 2020  ord']).         
-0000fe80: 2020 2020 2020 2069 6620 7467 745f 6374         if tgt_ct
-0000fe90: 782e 6765 7428 6e6d 293a 0a20 2020 2020  x.get(nm):.     
-0000fea0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000feb0: 6774 5f63 6f6e 6669 672e 7365 7428 276f  gt_config.set('o
-0000fec0: 7074 696f 6e73 272c 206e 6d2c 2074 6774  ptions', nm, tgt
-0000fed0: 5f63 7478 5b6e 6d5d 290a 2020 2020 2020  _ctx[nm]).      
-0000fee0: 2020 2020 2020 2020 2020 656c 6966 2074            elif t
-0000fef0: 6774 5f63 6f6e 6669 672e 6861 735f 6f70  gt_config.has_op
-0000ff00: 7469 6f6e 2827 6f70 7469 6f6e 7327 2c20  tion('options', 
-0000ff10: 6e6d 293a 0a20 2020 2020 2020 2020 2020  nm):.           
-0000ff20: 2020 2020 2020 2020 2074 6774 5f63 7478           tgt_ctx
-0000ff30: 5b6e 6d5d 203d 2074 6774 5f63 6f6e 6669  [nm] = tgt_confi
-0000ff40: 672e 6765 7428 276f 7074 696f 6e73 272c  g.get('options',
-0000ff50: 206e 6d29 0a20 2020 2020 2020 2020 2020   nm).           
-0000ff60: 2020 2020 2065 6c69 6620 7372 635f 6374       elif src_ct
-0000ff70: 782e 6765 7428 6e6d 293a 0a20 2020 2020  x.get(nm):.     
-0000ff80: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000ff90: 6774 5f63 7478 5b6e 6d5d 203d 2073 7263  gt_ctx[nm] = src
-0000ffa0: 5f63 7478 5b6e 6d5d 0a20 2020 2020 2020  _ctx[nm].       
-0000ffb0: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
-0000ffc0: 5f63 6f6e 6669 672e 7365 7428 276f 7074  _config.set('opt
-0000ffd0: 696f 6e73 272c 206e 6d2c 2074 6774 5f63  ions', nm, tgt_c
-0000ffe0: 7478 5b6e 6d5d 290a 2020 2020 2020 2020  tx[nm]).        
-0000fff0: 656c 6966 2069 7465 6d20 3d3d 2027 7769  elif item == 'wi
-00010000: 7468 6f75 745f 6465 6d6f 273a 0a20 2020  thout_demo':.   
-00010010: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
-00010020: 5b69 7465 6d5d 203d 2027 5472 7565 270a  [item] = 'True'.
-00010030: 2020 2020 2020 2020 2020 2020 7372 635f              src_
-00010040: 636f 6e66 6967 2e73 6574 2827 6f70 7469  config.set('opti
-00010050: 6f6e 7327 2c20 6974 656d 2c20 7372 635f  ons', item, src_
-00010060: 6374 785b 6974 656d 5d29 0a20 2020 2020  ctx[item]).     
-00010070: 2020 2020 2020 2074 6774 5f63 7478 5b69         tgt_ctx[i
-00010080: 7465 6d5d 203d 2027 5472 7565 270a 2020  tem] = 'True'.  
-00010090: 2020 2020 2020 2020 2020 7467 745f 636f            tgt_co
-000100a0: 6e66 6967 2e73 6574 2827 6f70 7469 6f6e  nfig.set('option
-000100b0: 7327 2c20 6974 656d 2c20 7467 745f 6374  s', item, tgt_ct
-000100c0: 785b 6974 656d 5d29 0a20 2020 2069 6620  x[item]).    if 
-000100d0: 7372 635f 6374 785b 276e 6f5f 7665 6e76  src_ctx['no_venv
-000100e0: 275d 3a0a 2020 2020 2020 2020 7372 635f  ']:.        src_
-000100f0: 6374 785b 2776 656e 765f 6f75 7061 7468  ctx['venv_oupath
-00010100: 275d 203d 2073 7263 5f63 7478 5b27 6f70  '] = src_ctx['op
-00010110: 745f 6f75 7061 7468 275d 0a20 2020 2065  t_oupath'].    e
-00010120: 6c73 653a 0a20 2020 2020 2020 2073 7263  lse:.        src
-00010130: 5f63 7478 5b27 7665 6e76 5f6f 7570 6174  _ctx['venv_oupat
-00010140: 6827 5d20 3d20 6f73 2e70 6174 682e 6a6f  h'] = os.path.jo
-00010150: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
-00010160: 6f73 2e70 6174 682e 6578 7061 6e64 7573  os.path.expandus
-00010170: 6572 2827 7e27 292c 2027 5645 4e56 2d25  er('~'), 'VENV-%
-00010180: 7327 2025 2074 6774 5f63 7478 5b27 7467  s' % tgt_ctx['tg
-00010190: 745f 6f64 6f6f 5f66 7665 7227 5d29 0a20  t_odoo_fver']). 
-000101a0: 2020 2074 6774 5f63 7478 5b27 7665 6e76     tgt_ctx['venv
-000101b0: 5f6f 7570 6174 6827 5d20 3d20 7372 635f  _oupath'] = src_
-000101c0: 6374 785b 2776 656e 765f 6f75 7061 7468  ctx['venv_oupath
-000101d0: 275d 0a20 2020 2072 6574 7572 6e20 7372  '].    return sr
-000101e0: 635f 6374 782c 2074 6774 5f63 7478 2c20  c_ctx, tgt_ctx, 
-000101f0: 7372 635f 636f 6e66 6967 2c20 7467 745f  src_config, tgt_
-00010200: 636f 6e66 6967 0a0a 0a64 6566 2073 6869  config...def shi
-00010210: 6674 5f63 7478 2873 7263 5f63 7478 2c20  ft_ctx(src_ctx, 
-00010220: 7467 745f 6374 782c 2070 6861 7365 3d4e  tgt_ctx, phase=N
-00010230: 6f6e 6529 3a0a 2020 2020 7068 6173 6520  one):.    phase 
-00010240: 3d20 7068 6173 6520 6f72 2031 0a20 2020  = phase or 1.   
-00010250: 2066 6f72 2069 7465 6d20 696e 2028 2776   for item in ('v
-00010260: 6964 272c 2027 6f64 6f6f 5f66 7665 7227  id', 'odoo_fver'
-00010270: 2c20 276f 646f 6f5f 7665 7227 293a 0a20  , 'odoo_ver'):. 
-00010280: 2020 2020 2020 2073 7263 5f63 7478 5b27         src_ctx['
-00010290: 7372 635f 2573 2720 2520 6974 656d 5d2c  src_%s' % item],
-000102a0: 2074 6774 5f63 7478 5b0a 2020 2020 2020   tgt_ctx[.      
-000102b0: 2020 2020 2020 2774 6774 5f25 7327 2025        'tgt_%s' %
-000102c0: 2069 7465 6d5d 203d 2074 6774 5f63 7478   item] = tgt_ctx
-000102d0: 5b27 7467 745f 2573 2720 2520 6974 656d  ['tgt_%s' % item
-000102e0: 5d2c 2046 616c 7365 0a20 2020 2066 6f72  ], False.    for
-000102f0: 2069 7465 6d20 696e 2028 2764 625f 6e61   item in ('db_na
-00010300: 6d65 272c 2027 636f 6e66 5f66 6e27 2c20  me', 'conf_fn', 
-00010310: 2778 6d6c 7270 635f 706f 7274 272c 2027  'xmlrpc_port', '
-00010320: 6462 5f75 7365 7227 293a 0a20 2020 2020  db_user'):.     
-00010330: 2020 2073 7263 5f63 7478 5b69 7465 6d5d     src_ctx[item]
-00010340: 2c20 7467 745f 6374 785b 6974 656d 5d20  , tgt_ctx[item] 
-00010350: 3d20 7467 745f 6374 785b 6974 656d 5d2c  = tgt_ctx[item],
-00010360: 2046 616c 7365 0a20 2020 2066 6f72 2069   False.    for i
-00010370: 7465 6d20 696e 2028 2764 625f 686f 7374  tem in ('db_host
-00010380: 272c 2027 6c6f 6769 6e5f 7573 6572 272c  ', 'login_user',
-00010390: 2027 6c6f 6769 6e5f 7061 7373 776f 7264   'login_password
-000103a0: 272c 2027 6372 7970 745f 7061 7373 776f  ', 'crypt_passwo
-000103b0: 7264 2729 3a0a 2020 2020 2020 2020 6966  rd'):.        if
-000103c0: 2074 6774 5f63 7478 2e67 6574 2869 7465   tgt_ctx.get(ite
-000103d0: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
-000103e0: 7372 635f 6374 785b 6974 656d 5d20 3d20  src_ctx[item] = 
-000103f0: 7467 745f 6374 785b 6974 656d 5d0a 2020  tgt_ctx[item].  
-00010400: 2020 7265 7475 726e 2073 7263 5f63 7478    return src_ctx
-00010410: 2c20 7467 745f 6374 780a 0a0a 6465 6620  , tgt_ctx...def 
-00010420: 7072 6570 6172 655f 636f 6e66 6967 5f66  prepare_config_f
-00010430: 696c 6528 6374 782c 2073 7263 5f63 6f6e  ile(ctx, src_con
-00010440: 6669 672c 206f 755f 7665 725f 7061 7468  fig, ou_ver_path
-00010450: 3d4e 6f6e 652c 2070 6174 6873 3d4e 6f6e  =None, paths=Non
-00010460: 6529 3a0a 2020 2020 6966 206f 755f 7665  e):.    if ou_ve
-00010470: 725f 7061 7468 3a0a 2020 2020 2020 2020  r_path:.        
-00010480: 7372 635f 6c63 6f6e 6620 3d20 276f 7065  src_lconf = 'ope
-00010490: 6e75 7067 7261 6465 2e63 6f6e 6627 0a20  nupgrade.conf'. 
-000104a0: 2020 2020 2020 2066 756c 6c5f 6c63 6f6e         full_lcon
-000104b0: 6620 3d20 6f73 2e70 6174 682e 6a6f 696e  f = os.path.join
-000104c0: 286f 755f 7665 725f 7061 7468 2c20 7372  (ou_ver_path, sr
-000104d0: 635f 6c63 6f6e 6629 0a20 2020 2065 6c73  c_lconf).    els
-000104e0: 653a 0a20 2020 2020 2020 2073 7263 5f6c  e:.        src_l
-000104f0: 636f 6e66 203d 2063 6c6f 646f 6f2e 6275  conf = clodoo.bu
-00010500: 696c 645f 6f64 6f6f 5f70 6172 616d 280a  ild_odoo_param(.
-00010510: 2020 2020 2020 2020 2020 2020 274c 434f              'LCO
-00010520: 4e46 4e27 2c20 6f64 6f6f 5f76 6964 3d63  NFN', odoo_vid=c
-00010530: 7478 5b27 7372 635f 7669 6427 5d2c 206d  tx['src_vid'], m
-00010540: 756c 7469 3d54 7275 6529 0a20 2020 2020  ulti=True).     
-00010550: 2020 2066 756c 6c5f 6c63 6f6e 6620 3d20     full_lconf = 
-00010560: 6f73 2e70 6174 682e 6a6f 696e 286f 732e  os.path.join(os.
-00010570: 7061 7468 2e65 7870 616e 6475 7365 7228  path.expanduser(
-00010580: 277e 2729 2c0a 2020 2020 2020 2020 2020  '~'),.          
-00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105a0: 2020 2020 2020 2020 7372 635f 6c63 6f6e          src_lcon
-000105b0: 6629 0a20 2020 2020 2020 2066 6f72 2066  f).        for f
-000105c0: 6e20 696e 2028 272e 6f70 656e 6572 705f  n in ('.openerp_
-000105d0: 7365 7276 6572 7263 272c 2027 2e6f 646f  serverrc', '.odo
-000105e0: 6f72 6327 293a 0a20 2020 2020 2020 2020  orc'):.         
-000105f0: 2020 2074 6d70 5f6c 636f 6e66 203d 206f     tmp_lconf = o
-00010600: 732e 7061 7468 2e6a 6f69 6e28 6f73 2e70  s.path.join(os.p
-00010610: 6174 682e 6578 7061 6e64 7573 6572 2827  ath.expanduser('
-00010620: 7e27 292c 2066 6e29 0a20 2020 2020 2020  ~'), fn).       
-00010630: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
-00010640: 6973 6669 6c65 2874 6d70 5f6c 636f 6e66  isfile(tmp_lconf
-00010650: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00010660: 2020 206f 732e 7265 6d6f 7665 2874 6d70     os.remove(tmp
-00010670: 5f6c 636f 6e66 290a 2020 2020 6966 2070  _lconf).    if p
-00010680: 6174 6873 3a0a 2020 2020 2020 2020 7372  aths:.        sr
-00010690: 635f 636f 6e66 6967 2e73 6574 2827 6f70  c_config.set('op
-000106a0: 7469 6f6e 7327 2c20 2761 6464 6f6e 735f  tions', 'addons_
-000106b0: 7061 7468 272c 2027 2c27 2e6a 6f69 6e28  path', ','.join(
-000106c0: 7061 7468 7329 290a 2020 2020 6966 206f  paths)).    if o
-000106d0: 755f 7665 725f 7061 7468 3a0a 2020 2020  u_ver_path:.    
-000106e0: 2020 2020 7372 635f 636f 6e66 6967 2e73      src_config.s
-000106f0: 6574 2827 6f70 7469 6f6e 7327 2c20 2772  et('options', 'r
-00010700: 6f6f 745f 7061 7468 272c 206f 755f 7665  oot_path', ou_ve
-00010710: 725f 7061 7468 290a 2020 2020 7372 635f  r_path).    src_
-00010720: 636f 6e66 6967 2e77 7269 7465 286f 7065  config.write(ope
-00010730: 6e28 6675 6c6c 5f6c 636f 6e66 2c20 2777  n(full_lconf, 'w
-00010740: 2b27 2929 0a20 2020 2073 7263 5f63 6f6e  +')).    src_con
-00010750: 6669 672e 7265 6164 2866 756c 6c5f 6c63  fig.read(full_lc
-00010760: 6f6e 6629 0a20 2020 2072 6574 7572 6e20  onf).    return 
-00010770: 6675 6c6c 5f6c 636f 6e66 0a0a 0a64 6566  full_lconf...def
-00010780: 2068 6172 645f 636c 6561 6e5f 6d6f 6475   hard_clean_modu
-00010790: 6c65 2863 7478 2c20 6d6f 6475 6c65 5f6e  le(ctx, module_n
-000107a0: 616d 6529 3a0a 2020 2020 6465 6620 6472  ame):.    def dr
-000107b0: 6f70 5f64 6174 615f 7461 626c 6528 6374  op_data_table(ct
-000107c0: 782c 206d 6f64 656c 2c20 6d6f 6475 6c65  x, model, module
-000107d0: 5f6e 616d 652c 2063 6f6c 6e3d 4e6f 6e65  _name, coln=None
-000107e0: 2c20 6964 3d4e 6f6e 6529 3a0a 2020 2020  , id=None):.    
-000107f0: 2020 2020 636f 6c6e 203d 2063 6f6c 6e20      coln = coln 
-00010800: 6f72 2027 6d6f 6475 6c65 270a 2020 2020  or 'module'.    
-00010810: 2020 2020 6966 2069 643a 0a20 2020 2020      if id:.     
-00010820: 2020 2020 2020 2071 7565 7279 203d 2022         query = "
-00010830: 6465 6c65 7465 2066 726f 6d20 2573 2077  delete from %s w
-00010840: 6865 7265 2025 733d 2564 2220 2520 286d  here %s=%d" % (m
-00010850: 6f64 656c 2c20 636f 6c6e 2c20 6964 290a  odel, coln, id).
-00010860: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00010870: 2020 2020 2020 2020 2020 7175 6572 7920            query 
-00010880: 3d20 2264 656c 6574 6520 6672 6f6d 2025  = "delete from %
-00010890: 7320 7768 6572 6520 2573 3d27 2573 2722  s where %s='%s'"
-000108a0: 2025 2028 6d6f 6465 6c2c 2063 6f6c 6e2c   % (model, coln,
-000108b0: 206d 6f64 756c 655f 6e61 6d65 290a 2020   module_name).  
-000108c0: 2020 2020 2020 7265 6373 203d 2065 7865        recs = exe
-000108d0: 635f 7371 6c28 6374 782c 2071 7565 7279  c_sql(ctx, query
-000108e0: 290a 0a20 2020 2071 7565 7279 203d 2022  )..    query = "
-000108f0: 7365 6c65 6374 2069 642c 6e61 6d65 2c73  select id,name,s
-00010900: 7461 7465 2066 726f 6d20 6972 5f6d 6f64  tate from ir_mod
-00010910: 756c 655f 6d6f 6475 6c65 2077 6865 7265  ule_module where
-00010920: 206e 616d 653d 2725 7327 2220 2520 5c0a   name='%s'" % \.
-00010930: 2020 2020 2020 2020 2020 2020 6d6f 6475              modu
-00010940: 6c65 5f6e 616d 650a 2020 2020 7265 6373  le_name.    recs
-00010950: 203d 2065 7865 635f 7371 6c28 6374 782c   = exec_sql(ctx,
-00010960: 2071 7565 7279 2c20 7265 7370 6f6e 7365   query, response
-00010970: 3d54 7275 6529 0a20 2020 2069 6620 6e6f  =True).    if no
-00010980: 7420 6c65 6e28 7265 6373 293a 0a20 2020  t len(recs):.   
-00010990: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-000109a0: 7374 6174 6520 3d20 7265 6373 5b30 5d5b  state = recs[0][
-000109b0: 325d 0a20 2020 2069 6420 3d20 7265 6373  2].    id = recs
-000109c0: 5b30 5d5b 305d 0a20 2020 2069 6620 7374  [0][0].    if st
-000109d0: 6174 6520 3d3d 2027 696e 7374 616c 6c65  ate == 'installe
-000109e0: 6427 3a0a 2020 2020 2020 2020 7265 7475  d':.        retu
-000109f0: 726e 0a20 2020 2064 726f 705f 6461 7461  rn.    drop_data
-00010a00: 5f74 6162 6c65 2863 7478 2c20 2769 725f  _table(ctx, 'ir_
-00010a10: 6d6f 6465 6c5f 6461 7461 272c 206d 6f64  model_data', mod
-00010a20: 756c 655f 6e61 6d65 290a 2020 2020 6472  ule_name).    dr
-00010a30: 6f70 5f64 6174 615f 7461 626c 6528 6374  op_data_table(ct
-00010a40: 782c 2027 6972 5f6d 6f64 756c 655f 6d6f  x, 'ir_module_mo
-00010a50: 6475 6c65 5f64 6570 656e 6465 6e63 7927  dule_dependency'
-00010a60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010a70: 2020 2020 2020 6d6f 6475 6c65 5f6e 616d        module_nam
-00010a80: 652c 2063 6f6c 6e3d 276d 6f64 756c 655f  e, coln='module_
-00010a90: 6964 272c 2069 643d 6964 290a 2020 2020  id', id=id).    
-00010aa0: 6472 6f70 5f64 6174 615f 7461 626c 6528  drop_data_table(
-00010ab0: 6374 782c 2027 6972 5f74 7261 6e73 6c61  ctx, 'ir_transla
-00010ac0: 7469 6f6e 272c 206d 6f64 756c 655f 6e61  tion', module_na
-00010ad0: 6d65 290a 2020 2020 7365 745f 756e 696e  me).    set_unin
-00010ae0: 7374 616c 6c65 645f 6279 5f73 716c 2863  stalled_by_sql(c
-00010af0: 7478 2c20 5b5f 6228 6d6f 6475 6c65 5f6e  tx, [_b(module_n
-00010b00: 616d 6529 5d29 0a0a 0a64 6566 2066 6978  ame)])...def fix
-00010b10: 5f62 7567 5f70 7265 2873 7263 5f63 7478  _bug_pre(src_ctx
-00010b20: 2c20 7467 745f 6374 782c 2073 7263 5f66  , tgt_ctx, src_f
-00010b30: 756c 6c5f 6c63 6f6e 662c 2073 7263 5f70  ull_lconf, src_p
-00010b40: 6174 6873 293a 0a20 2020 2073 6176 6564  aths):.    saved
-00010b50: 5f64 622c 2073 7263 5f63 7478 5b27 6462  _db, src_ctx['db
-00010b60: 5f6e 616d 6527 5d20 3d20 7372 635f 6374  _name'] = src_ct
-00010b70: 785b 2764 625f 6e61 6d65 275d 2c20 7467  x['db_name'], tg
-00010b80: 745f 6374 785b 2764 625f 6e61 6d65 275d  t_ctx['db_name']
-00010b90: 0a20 2020 2069 6620 2873 7263 5f63 7478  .    if (src_ctx
-00010ba0: 5b27 7372 635f 6f64 6f6f 5f66 7665 7227  ['src_odoo_fver'
-00010bb0: 5d20 3d3d 2027 372e 3027 2061 6e64 0a20  ] == '7.0' and. 
-00010bc0: 2020 2020 2020 2020 2020 2074 6774 5f63             tgt_c
-00010bd0: 7478 5b27 7467 745f 6f64 6f6f 5f66 7665  tx['tgt_odoo_fve
-00010be0: 7227 5d20 3d3d 2027 382e 3027 293a 0a20  r'] == '8.0'):. 
-00010bf0: 2020 2020 2020 2071 7565 7279 203d 2027         query = '
-00010c00: 2727 7570 6461 7465 2069 725f 7569 5f76  ''update ir_ui_v
-00010c10: 6965 770a 2020 2020 2020 2020 2020 2020  iew.            
-00010c20: 2020 2020 7365 7420 6172 6368 3d52 4547      set arch=REG
-00010c30: 4558 505f 5245 504c 4143 4528 6172 6368  EXP_REPLACE(arch
-00010c40: 2c20 273c 6669 656c 6420 6e61 6d65 3d22  , '<field name="
-00010c50: 6d65 6e75 5f69 6422 2e2a 2f3e 272c 2027  menu_id".*/>', '
-00010c60: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00010c70: 2020 2077 6865 7265 206d 6f64 656c 3d27     where model='
-00010c80: 7265 732e 7573 6572 7327 2061 6e64 0a20  res.users' and. 
-00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ca0: 2020 2020 2061 7263 6820 6c69 6b65 2027       arch like '
-00010cb0: 253c 6669 656c 6420 6e61 6d65 3d5f 6d65  %<field name=_me
-00010cc0: 6e75 5f69 645f 2527 3b27 2727 0a20 2020  nu_id_%';'''.   
-00010cd0: 2020 2020 2065 7865 635f 7371 6c28 7372       exec_sql(sr
-00010ce0: 635f 6374 782c 2071 7565 7279 290a 2020  c_ctx, query).  
-00010cf0: 2020 656c 6966 2028 7372 635f 6374 785b    elif (src_ctx[
-00010d00: 2773 7263 5f6f 646f 6f5f 6676 6572 275d  'src_odoo_fver']
-00010d10: 203d 3d20 2738 2e30 2720 616e 640a 2020   == '8.0' and.  
-00010d20: 2020 2020 2020 2020 2020 7467 745f 6374            tgt_ct
-00010d30: 785b 2774 6774 5f6f 646f 6f5f 6676 6572  x['tgt_odoo_fver
-00010d40: 275d 203d 3d20 2739 2e30 2729 3a0a 2020  '] == '9.0'):.  
-00010d50: 2020 2020 2020 6966 2027 6163 636f 756e        if 'accoun
-00010d60: 745f 7061 796d 656e 7427 2069 6e20 7372  t_payment' in sr
-00010d70: 635f 6374 785b 2773 7263 5f6d 6f64 756c  c_ctx['src_modul
-00010d80: 655f 6c69 7374 275d 3a0a 2020 2020 2020  e_list']:.      
-00010d90: 2020 2020 2020 7374 7320 3d20 636c 6f64        sts = clod
-00010da0: 6f6f 2e61 6374 5f69 6e73 7461 6c6c 5f6d  oo.act_install_m
-00010db0: 6f64 756c 6573 280a 2020 2020 2020 2020  odules(.        
-00010dc0: 2020 2020 2020 2020 7372 635f 6374 782c          src_ctx,
-00010dd0: 206d 6f64 756c 655f 6c69 7374 3d5b 2761   module_list=['a
-00010de0: 6363 6f75 6e74 5f62 616e 6b69 6e67 5f70  ccount_banking_p
-00010df0: 6179 6d65 6e74 5f65 7870 6f72 7427 5d29  ayment_export'])
-00010e00: 0a20 2020 2073 7263 5f63 7478 5b27 6462  .    src_ctx['db
-00010e10: 5f6e 616d 6527 5d20 3d20 7361 7665 645f  _name'] = saved_
-00010e20: 6462 0a0a 0a64 6566 2066 6978 5f62 7567  db...def fix_bug
-00010e30: 5f70 6f73 7428 7372 635f 6374 782c 2074  _post(src_ctx, t
-00010e40: 6774 5f63 7478 2c20 7467 745f 6675 6c6c  gt_ctx, tgt_full
-00010e50: 5f6c 636f 6e66 2c20 7467 745f 7061 7468  _lconf, tgt_path
-00010e60: 7329 3a0a 2020 2020 6966 2028 7372 635f  s):.    if (src_
-00010e70: 6374 785b 2773 7263 5f6f 646f 6f5f 6676  ctx['src_odoo_fv
-00010e80: 6572 275d 203d 3d20 2737 2e30 2720 616e  er'] == '7.0' an
-00010e90: 640a 2020 2020 2020 2020 2020 2020 7467  d.            tg
-00010ea0: 745f 6374 785b 2774 6774 5f6f 646f 6f5f  t_ctx['tgt_odoo_
-00010eb0: 6676 6572 275d 203d 3d20 2738 2e30 2729  fver'] == '8.0')
-00010ec0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-00010ed0: 0a64 6566 206d 6967 7261 7465 5f6f 646f  .def migrate_odo
-00010ee0: 6f28 7372 635f 6374 782c 2074 6774 5f63  o(src_ctx, tgt_c
-00010ef0: 7478 2c20 7372 635f 636f 6e66 6967 2c20  tx, src_config, 
-00010f00: 7467 745f 636f 6e66 6967 2c20 7068 6173  tgt_config, phas
-00010f10: 653d 4e6f 6e65 293a 0a0a 2020 2020 6465  e=None):..    de
-00010f20: 6620 6765 745f 7772 6f6e 675f 6d6f 6475  f get_wrong_modu
-00010f30: 6c65 7328 6374 782c 2062 6164 5f6d 6f64  les(ctx, bad_mod
-00010f40: 756c 655f 6c69 7374 3d4e 6f6e 6529 3a0a  ule_list=None):.
-00010f50: 2020 2020 2020 2020 6966 2073 7263 5f63          if src_c
-00010f60: 7478 5b27 6472 795f 7275 6e27 5d3a 0a20  tx['dry_run']:. 
-00010f70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00010f80: 6e20 5b5d 0a20 2020 2020 2020 2069 6620  n [].        if 
-00010f90: 6261 645f 6d6f 6475 6c65 5f6c 6973 743a  bad_module_list:
-00010fa0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00010fb0: 6c65 6e28 6261 645f 6d6f 6475 6c65 5f6c  len(bad_module_l
-00010fc0: 6973 7429 203d 3d20 313a 0a20 2020 2020  ist) == 1:.     
-00010fd0: 2020 2020 2020 2020 2020 2071 7565 7279             query
-00010fe0: 203d 2027 2727 7365 6c65 6374 2069 642c   = '''select id,
-00010ff0: 6e61 6d65 2c73 7461 7465 2066 726f 6d20  name,state from 
-00011000: 6972 5f6d 6f64 756c 655f 6d6f 6475 6c65  ir_module_module
-00011010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011020: 2020 2020 2020 2020 2020 2020 7768 6572              wher
-00011030: 6520 7374 6174 6520 6e6f 7420 696e 0a20  e state not in. 
-00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011050: 2020 2020 2020 2020 2020 2827 696e 7374            ('inst
-00011060: 616c 6c65 6427 2c20 2775 6e69 6e73 7461  alled', 'uninsta
-00011070: 6c6c 6564 272c 2027 756e 696e 7374 616c  lled', 'uninstal
-00011080: 6c61 626c 6527 2920 616e 640a 2020 2020  lable') and.    
-00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110a0: 2020 2020 2020 206e 616d 6520 3d20 2725         name = '%
-000110b0: 7327 3b27 2727 2025 2062 6164 5f6d 6f64  s';''' % bad_mod
-000110c0: 756c 655f 6c69 7374 5b30 5d0a 2020 2020  ule_list[0].    
-000110d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000110e0: 2020 2020 2020 2020 2020 2020 2020 7175                qu
-000110f0: 6572 7920 3d20 2727 2773 656c 6563 7420  ery = '''select 
-00011100: 6964 2c6e 616d 652c 7374 6174 6520 6672  id,name,state fr
-00011110: 6f6d 2069 725f 6d6f 6475 6c65 5f6d 6f64  om ir_module_mod
-00011120: 756c 650a 2020 2020 2020 2020 2020 2020  ule.            
-00011130: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00011140: 6865 7265 2073 7461 7465 206e 6f74 2069  here state not i
-00011150: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00011160: 2020 2020 2020 2020 2020 2020 2028 2769               ('i
-00011170: 6e73 7461 6c6c 6564 272c 2027 756e 696e  nstalled', 'unin
-00011180: 7374 616c 6c65 6427 2c20 2775 6e69 6e73  stalled', 'unins
-00011190: 7461 6c6c 6162 6c65 2729 2061 6e64 0a20  tallable') and. 
-000111a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111b0: 2020 2020 2020 2020 2020 6e61 6d65 2069            name i
-000111c0: 6e20 2825 7329 3b27 2727 2025 2028 0a20  n (%s);''' % (. 
-000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111e0: 2020 2020 2020 2020 2020 2020 2020 2227                "'
-000111f0: 2573 2722 2025 2022 272c 2722 2e6a 6f69  %s'" % "','".joi
-00011200: 6e28 6261 645f 6d6f 6475 6c65 5f6c 6973  n(bad_module_lis
-00011210: 7429 290a 0a20 2020 2020 2020 2065 6c73  t))..        els
-00011220: 653a 0a20 2020 2020 2020 2020 2020 2071  e:.            q
-00011230: 7565 7279 203d 2027 2727 7365 6c65 6374  uery = '''select
-00011240: 2069 642c 6e61 6d65 2c73 7461 7465 2066   id,name,state f
-00011250: 726f 6d20 6972 5f6d 6f64 756c 655f 6d6f  rom ir_module_mo
-00011260: 6475 6c65 0a20 2020 2020 2020 2020 2020  dule.           
-00011270: 2020 2020 2020 2020 2020 2020 7768 6572              wher
-00011280: 6520 7374 6174 6520 6e6f 7420 696e 0a20  e state not in. 
-00011290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112a0: 2020 2020 2020 2827 696e 7374 616c 6c65        ('installe
-000112b0: 6427 2c20 2775 6e69 6e73 7461 6c6c 6564  d', 'uninstalled
-000112c0: 272c 2027 756e 696e 7374 616c 6c61 626c  ', 'uninstallabl
-000112d0: 6527 293b 2727 270a 2020 2020 2020 2020  e');'''.        
-000112e0: 726f 7773 203d 2065 7865 635f 7371 6c28  rows = exec_sql(
-000112f0: 6374 782c 2071 7565 7279 2c20 7265 7370  ctx, query, resp
-00011300: 6f6e 7365 3d54 7275 6529 0a20 2020 2020  onse=True).     
-00011310: 2020 2077 726f 6e67 5f6c 6973 7420 3d20     wrong_list = 
-00011320: 5b5d 0a20 2020 2020 2020 2066 6f72 2072  [].        for r
-00011330: 6f77 2069 6e20 726f 7773 3a0a 2020 2020  ow in rows:.    
-00011340: 2020 2020 2020 2020 6966 206e 6f74 2062          if not b
-00011350: 6164 5f6d 6f64 756c 655f 6c69 7374 206f  ad_module_list o
-00011360: 7220 726f 775b 315d 206e 6f74 2069 6e20  r row[1] not in 
-00011370: 6261 645f 6d6f 6475 6c65 5f6c 6973 743a  bad_module_list:
-00011380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011390: 2077 726f 6e67 5f6c 6973 742e 6170 7065   wrong_list.appe
-000113a0: 6e64 2872 6f77 5b31 5d29 0a20 2020 2020  nd(row[1]).     
-000113b0: 2020 2072 6574 7572 6e20 7772 6f6e 675f     return wrong_
-000113c0: 6c69 7374 0a0a 2020 2020 6465 6620 7275  list..    def ru
-000113d0: 6e5f 6f70 656e 7570 6772 6164 6528 7467  n_openupgrade(tg
-000113e0: 745f 6374 782c 206f 755f 7665 725f 7061  t_ctx, ou_ver_pa
-000113f0: 7468 2c20 7467 745f 6675 6c6c 5f6c 636f  th, tgt_full_lco
-00011400: 6e66 293a 0a20 2020 2020 2020 206f 7570  nf):.        oup
-00011410: 6174 685f 7363 7269 7074 203d 2046 616c  ath_script = Fal
-00011420: 7365 0a20 2020 2020 2020 2066 6f72 2070  se.        for p
-00011430: 2069 6e20 2827 272c 2027 6f64 6f6f 272c   in ('', 'odoo',
-00011440: 2027 6f70 656e 6572 7027 2c20 2773 6572   'openerp', 'ser
-00011450: 7665 7227 293a 0a20 2020 2020 2020 2020  ver'):.         
-00011460: 2020 2069 6620 6f75 7061 7468 5f73 6372     if oupath_scr
-00011470: 6970 743a 0a20 2020 2020 2020 2020 2020  ipt:.           
-00011480: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-00011490: 2020 2020 2020 2066 6f72 206e 2069 6e20         for n in 
-000114a0: 2827 6f64 6f6f 2d62 696e 272c 2027 6f70  ('odoo-bin', 'op
-000114b0: 656e 6572 702d 7365 7276 6572 2729 3a0a  enerp-server'):.
-000114c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114d0: 6966 2070 3a0a 2020 2020 2020 2020 2020  if p:.          
-000114e0: 2020 2020 2020 2020 2020 7363 7269 7074            script
-000114f0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-00011500: 6f75 5f76 6572 5f70 6174 682c 2070 2c20  ou_ver_path, p, 
-00011510: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-00011520: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00011530: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-00011540: 6970 7420 3d20 6f73 2e70 6174 682e 6a6f  ipt = os.path.jo
-00011550: 696e 286f 755f 7665 725f 7061 7468 2c20  in(ou_ver_path, 
-00011560: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
-00011570: 2020 2069 6620 6f73 2e70 6174 682e 6973     if os.path.is
-00011580: 6669 6c65 2873 6372 6970 7429 3a0a 2020  file(script):.  
-00011590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115a0: 2020 6f75 7061 7468 5f73 6372 6970 7420    oupath_script 
-000115b0: 3d20 7363 7269 7074 0a20 2020 2020 2020  = script.       
-000115c0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-000115d0: 616b 0a20 2020 2020 2020 2069 6620 7372  ak.        if sr
-000115e0: 635f 6374 785b 276e 6f5f 7665 6e76 275d  c_ctx['no_venv']
-000115f0: 3a0a 2020 2020 2020 2020 2020 2020 7374  :.            st
-00011600: 7320 3d20 7275 6e5f 7472 6163 6564 286f  s = run_traced(o
-00011610: 7570 6174 685f 7363 7269 7074 2c0a 2020  upath_script,.  
-00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011630: 2020 2020 2020 2020 2020 2027 2d63 272c             '-c',
-00011640: 2074 6774 5f66 756c 6c5f 6c63 6f6e 662c   tgt_full_lconf,
-00011650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011660: 2020 2020 2020 2020 2020 2020 2020 272d                '-
-00011670: 6427 2c20 7467 745f 6374 785b 2764 625f  d', tgt_ctx['db_
-00011680: 6e61 6d65 275d 2c0a 2020 2020 2020 2020  name'],.        
-00011690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116a0: 2020 2020 2027 2d75 272c 2027 616c 6c27       '-u', 'all'
-000116b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000116c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000116d0: 2d2d 7374 6f70 2d61 6674 6572 2d69 6e69  --stop-after-ini
-000116e0: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
-000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011700: 2027 2d2d 6e6f 2d78 6d6c 7270 6327 2c0a   '--no-xmlrpc',.
-00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011720: 2020 2020 2020 2020 2020 2020 2027 2d2d               '--
-00011730: 6c6f 6766 696c 653d 2573 2720 2520 7467  logfile=%s' % tg
-00011740: 745f 6374 785b 276c 6f67 6669 6c65 275d  t_ctx['logfile']
-00011750: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00011760: 2020 2020 2020 2020 2020 2020 7363 7269              scri
-00011770: 7074 203d 206f 732e 7061 7468 2e6a 6f69  pt = os.path.joi
-00011780: 6e28 6f75 5f76 6572 5f70 6174 682c 2027  n(ou_ver_path, '
-00011790: 6d69 6772 6174 652e 7368 2729 0a20 2020  migrate.sh').   
-000117a0: 2020 2020 2020 2020 2066 6420 3d20 6f70           fd = op
-000117b0: 656e 2873 6372 6970 742c 2027 7727 290a  en(script, 'w').
-000117c0: 2020 2020 2020 2020 2020 2020 6664 2e77              fd.w
-000117d0: 7269 7465 2827 6364 2025 735c 6e27 2025  rite('cd %s\n' %
-000117e0: 2074 6774 5f63 7478 5b27 7665 6e76 5f6f   tgt_ctx['venv_o
-000117f0: 7570 6174 6827 5d29 0a20 2020 2020 2020  upath']).       
-00011800: 2020 2020 2066 642e 7772 6974 6528 6227       fd.write(b'
-00011810: 736f 7572 6365 202e 2f62 696e 2f61 6374  source ./bin/act
-00011820: 6976 6174 655c 6e27 290a 2020 2020 2020  ivate\n').      
-00011830: 2020 2020 2020 6664 2e77 7269 7465 2862        fd.write(b
-00011840: 2725 7320 2d63 2025 7320 2d64 2025 7320  '%s -c %s -d %s 
-00011850: 2d75 2061 6c6c 202d 2d73 746f 702d 6166  -u all --stop-af
-00011860: 7465 722d 696e 6974 202d 2d6e 6f2d 786d  ter-init --no-xm
-00011870: 6c72 7063 270a 2020 2020 2020 2020 2020  lrpc'.          
-00011880: 2020 2020 2020 2020 2020 2062 2720 2d2d             b' --
-00011890: 6c6f 6766 696c 653d 2573 5c6e 2720 2520  logfile=%s\n' % 
-000118a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000118b0: 2020 2020 2020 2020 2020 206f 7570 6174             oupat
-000118c0: 685f 7363 7269 7074 2c20 7467 745f 6675  h_script, tgt_fu
-000118d0: 6c6c 5f6c 636f 6e66 2c0a 2020 2020 2020  ll_lconf,.      
-000118e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118f0: 2020 2074 6774 5f63 7478 5b27 6462 5f6e     tgt_ctx['db_n
-00011900: 616d 6527 5d2c 0a20 2020 2020 2020 2020  ame'],.         
-00011910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011920: 7467 745f 6374 785b 276c 6f67 6669 6c65  tgt_ctx['logfile
-00011930: 275d 2929 0a20 2020 2020 2020 2020 2020  '])).           
-00011940: 2066 642e 7772 6974 6528 6227 7374 733d   fd.write(b'sts=
-00011950: 243f 5c6e 2729 0a20 2020 2020 2020 2020  $?\n').         
-00011960: 2020 2066 642e 7772 6974 6528 6227 6465     fd.write(b'de
-00011970: 6163 7469 7661 7465 5c6e 2729 0a20 2020  activate\n').   
-00011980: 2020 2020 2020 2020 2066 642e 7772 6974           fd.writ
-00011990: 6528 6227 6578 6974 2024 7374 735c 6e27  e(b'exit $sts\n'
-000119a0: 290a 2020 2020 2020 2020 2020 2020 6664  ).            fd
-000119b0: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
-000119c0: 2020 2020 206f 732e 6368 6d6f 6428 7363       os.chmod(sc
-000119d0: 7269 7074 2c20 306f 3734 3429 0a20 2020  ript, 0o744).   
-000119e0: 2020 2020 2020 2020 2073 7473 203d 2030           sts = 0
-000119f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011a00: 6e6f 7420 7372 635f 6374 785b 2764 7279  not src_ctx['dry
-00011a10: 5f72 756e 275d 3a0a 2020 2020 2020 2020  _run']:.        
-00011a20: 2020 2020 2020 2020 7374 7320 3d20 6f73          sts = os
-00011a30: 2e73 7973 7465 6d28 7363 7269 7074 290a  .system(script).
-00011a40: 2020 2020 2020 2020 6966 2073 7473 3a0a          if sts:.
-00011a50: 2020 2020 2020 2020 2020 2020 6f73 302e              os0.
-00011a60: 776c 6f67 2827 2a2a 2a20 5265 7475 726e  wlog('*** Return
-00011a70: 2063 6f64 6520 2564 202a 2a2a 2729 0a20   code %d ***'). 
-00011a80: 2020 2020 2020 2065 6c69 6620 6e6f 7420         elif not 
-00011a90: 7372 635f 6374 785b 2764 7279 5f72 756e  src_ctx['dry_run
-00011aa0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
-00011ab0: 7469 6d65 2e73 6c65 6570 2835 290a 0a20  time.sleep(5).. 
-00011ac0: 2020 2070 6861 7365 203d 2070 6861 7365     phase = phase
-00011ad0: 206f 7220 320a 2020 2020 7467 745f 7361   or 2.    tgt_sa
-00011ae0: 7665 645f 6663 6f6e 6620 3d20 7467 745f  ved_fconf = tgt_
-00011af0: 6374 785b 2763 6f6e 665f 666e 275d 0a20  ctx['conf_fn']. 
-00011b00: 2020 2073 7263 5f66 756c 6c5f 6c63 6f6e     src_full_lcon
-00011b10: 6620 3d20 7072 6570 6172 655f 636f 6e66  f = prepare_conf
-00011b20: 6967 5f66 696c 6528 7372 635f 6374 782c  ig_file(src_ctx,
-00011b30: 2073 7263 5f63 6f6e 6669 6729 0a20 2020   src_config).   
-00011b40: 2069 6620 2873 7263 5f63 7478 5b27 7372   if (src_ctx['sr
-00011b50: 635f 7669 6427 5d20 3d3d 2073 7263 5f63  c_vid'] == src_c
-00011b60: 7478 5b27 6672 6f6d 5f62 7261 6e63 6827  tx['from_branch'
-00011b70: 5d20 616e 640a 2020 2020 2020 2020 2020  ] and.          
-00011b80: 2020 6765 745f 7772 6f6e 675f 6d6f 6475    get_wrong_modu
-00011b90: 6c65 7328 7372 635f 6374 7829 293a 0a20  les(src_ctx)):. 
-00011ba0: 2020 2020 2020 2069 6620 7068 6173 6520         if phase 
-00011bb0: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
-00011bc0: 2020 6f73 302e 776c 6f67 2827 2a2a 2a20    os0.wlog('*** 
-00011bd0: 556e 7374 6162 6c65 2069 6e73 7461 6c6c  Unstable install
-00011be0: 6174 696f 6e20 2a2a 2a27 290a 2020 2020  ation ***').    
-00011bf0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00011c00: 2020 2020 2020 6f73 302e 776c 6f67 2827        os0.wlog('
-00011c10: 2a2a 2a20 556e 7374 6162 6c65 2069 6e73  *** Unstable ins
-00011c20: 7461 6c6c 6174 696f 6e3a 2074 7279 2074  tallation: try t
-00011c30: 6f20 636f 7272 6563 7420 6572 726f 7273  o correct errors
-00011c40: 202a 2a2a 2729 0a20 2020 2020 2020 2020   ***').         
-00011c50: 2020 2072 756e 5f6f 646f 6f5f 616c 6c74     run_odoo_allt
-00011c60: 6573 7428 7372 635f 6374 785b 2774 6774  est(src_ctx['tgt
-00011c70: 5f76 6964 275d 2c20 7372 635f 6675 6c6c  _vid'], src_full
-00011c80: 5f6c 636f 6e66 2c0a 2020 2020 2020 2020  _lconf,.        
-00011c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ca0: 2020 2020 2073 7263 5f63 7478 5b27 6462       src_ctx['db
-00011cb0: 5f6e 616d 6527 5d2c 2073 7263 5f63 7478  _name'], src_ctx
-00011cc0: 5b27 6c6f 6766 696c 6527 5d29 0a20 2020  ['logfile']).   
-00011cd0: 2020 2020 2020 2020 2062 6164 5f6d 6f64           bad_mod
-00011ce0: 756c 6573 203d 2067 6574 5f77 726f 6e67  ules = get_wrong
-00011cf0: 5f6d 6f64 756c 6573 2873 7263 5f63 7478  _modules(src_ctx
-00011d00: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00011d10: 2062 6164 5f6d 6f64 756c 6573 3a0a 2020   bad_modules:.  
-00011d20: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00011d30: 302e 776c 6f67 2827 2a2a 2a20 556e 7374  0.wlog('*** Unst
-00011d40: 6162 6c65 2069 6e73 7461 6c6c 6174 696f  able installatio
-00011d50: 6e20 6475 6520 746f 2025 7320 2a2a 2a27  n due to %s ***'
-00011d60: 2025 2062 6164 5f6d 6f64 756c 6573 290a   % bad_modules).
-00011d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d80: 6f73 302e 776c 6f67 2827 2a2a 2a20 4d49  os0.wlog('*** MI
-00011d90: 4752 4154 494f 4e20 5354 4f50 5045 4420  GRATION STOPPED 
-00011da0: 2a2a 2a27 290a 2020 2020 2020 2020 2020  ***').          
-00011db0: 2020 2020 2020 7379 732e 6578 6974 2831        sys.exit(1
-00011dc0: 290a 0a20 2020 2073 7263 5f70 6174 6873  )..    src_paths
-00011dd0: 203d 2063 6f6e 6669 675f 6765 745f 6c69   = config_get_li
-00011de0: 7374 2873 7263 5f63 6f6e 6669 672c 2027  st(src_config, '
-00011df0: 6164 646f 6e73 5f70 6174 6827 290a 2020  addons_path').  
-00011e00: 2020 7467 745f 7061 7468 7320 3d20 636f    tgt_paths = co
-00011e10: 6e66 6967 5f67 6574 5f6c 6973 7428 7467  nfig_get_list(tg
-00011e20: 745f 636f 6e66 6967 2c20 2761 6464 6f6e  t_config, 'addon
-00011e30: 735f 7061 7468 2729 0a20 2020 206f 7330  s_path').    os0
-00011e40: 2e77 6c6f 6728 2761 6464 6f6e 735f 7061  .wlog('addons_pa
-00011e50: 7468 3d25 7327 2025 2073 7263 5f70 6174  th=%s' % src_pat
-00011e60: 6873 290a 2020 2020 6966 2070 6861 7365  hs).    if phase
-00011e70: 203e 2031 206f 7220 7372 635f 6374 785b   > 1 or src_ctx[
-00011e80: 2773 7263 5f76 6964 275d 203d 3d20 7372  'src_vid'] == sr
-00011e90: 635f 6374 785b 2766 726f 6d5f 6272 616e  c_ctx['from_bran
-00011ea0: 6368 275d 3a0a 2020 2020 2020 2020 6f73  ch']:.        os
-00011eb0: 302e 776c 6f67 2827 5465 7374 2063 6f6e  0.wlog('Test con
-00011ec0: 6e65 6374 696f 6e20 746f 2073 6f75 7263  nection to sourc
-00011ed0: 6520 6462 2025 7327 2025 2073 7263 5f63  e db %s' % src_c
-00011ee0: 7478 5b27 6462 5f6e 616d 6527 5d29 0a20  tx['db_name']). 
-00011ef0: 2020 2020 2020 2075 6964 2c20 7372 635f         uid, src_
-00011f00: 6374 7820 3d20 636c 6f64 6f6f 2e6f 6572  ctx = clodoo.oer
-00011f10: 705f 7365 745f 656e 7628 0a20 2020 2020  p_set_env(.     
-00011f20: 2020 2020 2020 2063 7478 3d73 7263 5f63         ctx=src_c
-00011f30: 7478 2c20 636f 6e66 6e3d 7372 635f 6675  tx, confn=src_fu
-00011f40: 6c6c 5f6c 636f 6e66 2c20 6462 3d73 7263  ll_lconf, db=src
-00011f50: 5f63 7478 5b27 6462 5f6e 616d 6527 5d29  _ctx['db_name'])
-00011f60: 0a20 2020 2020 2020 2023 2046 4958 206f  .        # FIX o
-00011f70: 6572 705f 7365 745f 656e 7620 6368 616e  erp_set_env chan
-00011f80: 6765 2064 7279 5f72 756e 0a20 2020 2020  ge dry_run.     
-00011f90: 2020 2073 7263 5f63 7478 5b27 6472 795f     src_ctx['dry_
-00011fa0: 7275 6e27 5d20 3d20 7467 745f 6374 785b  run'] = tgt_ctx[
-00011fb0: 2764 7279 5f72 756e 275d 0a20 2020 2020  'dry_run'].     
-00011fc0: 2020 2069 6620 7068 6173 6520 3e20 313a     if phase > 1:
-00011fd0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011fe0: 2873 7263 5f63 7478 5b27 6f70 745f 7361  (src_ctx['opt_sa
-00011ff0: 6665 275d 2061 6e64 0a20 2020 2020 2020  fe'] and.       
-00012000: 2020 2020 2020 2020 2020 2020 2073 7263               src
-00012010: 5f63 7478 5b27 7372 635f 7669 6427 5d20  _ctx['src_vid'] 
-00012020: 3d3d 2073 7263 5f63 7478 5b27 6672 6f6d  == src_ctx['from
-00012030: 5f62 7261 6e63 6827 5d29 3a0a 2020 2020  _branch']):.    
-00012040: 2020 2020 2020 2020 2020 2020 636c 6f64              clod
-00012050: 6f6f 2e61 6374 5f63 6865 636b 5f63 6f6e  oo.act_check_con
-00012060: 6669 6728 7372 635f 6374 7829 0a20 2020  fig(src_ctx).   
-00012070: 2020 2020 2020 2020 2069 6620 2873 7263           if (src
-00012080: 5f63 7478 5b27 756e 696e 7374 616c 6c5f  _ctx['uninstall_
-00012090: 6d6f 6475 6c65 7327 5d20 616e 640a 2020  modules'] and.  
-000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120b0: 2020 7372 635f 6374 785b 2773 7263 5f76    src_ctx['src_v
-000120c0: 6964 275d 203d 3d20 7372 635f 6374 785b  id'] == src_ctx[
-000120d0: 2766 726f 6d5f 6272 616e 6368 275d 293a  'from_branch']):
-000120e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000120f0: 2066 6f72 206d 6f64 756c 6520 696e 2073   for module in s
-00012100: 7263 5f63 7478 5b27 756e 696e 7374 616c  rc_ctx['uninstal
-00012110: 6c5f 6d6f 6475 6c65 7327 5d2e 7370 6c69  l_modules'].spli
-00012120: 7428 272c 2729 3a0a 2020 2020 2020 2020  t(','):.        
-00012130: 2020 2020 2020 2020 2020 2020 6472 6f70              drop
-00012140: 5f6d 6f64 756c 6528 7372 635f 6374 782c  _module(src_ctx,
-00012150: 206d 6f64 756c 652c 2066 6f72 6365 3d54   module, force=T
-00012160: 7275 6529 0a20 2020 2020 2020 2073 7263  rue).        src
-00012170: 5f63 7478 5b27 7372 635f 6d6f 6475 6c65  _ctx['src_module
-00012180: 5f6c 6973 7427 5d20 3d20 6f64 6f6f 5f64  _list'] = odoo_d
-00012190: 6570 656e 6465 6e63 6965 7328 0a20 2020  ependencies(.   
-000121a0: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
-000121b0: 2c20 276d 6f64 272c 2073 7263 5f63 7478  , 'mod', src_ctx
-000121c0: 5b27 6462 5f6e 616d 6527 5d2c 2073 7263  ['db_name'], src
-000121d0: 5f66 756c 6c5f 6c63 6f6e 662c 2073 7263  _full_lconf, src
-000121e0: 5f70 6174 6873 2c0a 2020 2020 2020 2020  _paths,.        
-000121f0: 2020 2020 7372 635f 6374 785b 2773 7263      src_ctx['src
-00012200: 5f6f 646f 6f5f 6676 6572 275d 290a 2020  _odoo_fver']).  
-00012210: 2020 2020 2020 6f73 302e 776c 6f67 2827        os0.wlog('
-00012220: 4d6f 6475 6c65 206c 6973 7420 746f 206d  Module list to m
-00012230: 6967 7261 7465 3d25 7327 2025 2073 7263  igrate=%s' % src
-00012240: 5f63 7478 5b27 7372 635f 6d6f 6475 6c65  _ctx['src_module
-00012250: 5f6c 6973 7427 5d29 0a20 2020 2069 6620  _list']).    if 
-00012260: 6e6f 7420 7372 635f 6374 782e 6765 7428  not src_ctx.get(
-00012270: 276f 7269 6769 6e61 6c5f 6d6f 6475 6c65  'original_module
-00012280: 5f6c 6973 7427 293a 0a20 2020 2020 2020  _list'):.       
-00012290: 2073 7263 5f63 7478 5b27 6f72 6967 696e   src_ctx['origin
-000122a0: 616c 5f6d 6f64 756c 655f 6c69 7374 275d  al_module_list']
-000122b0: 203d 2073 7263 5f63 7478 5b27 7372 635f   = src_ctx['src_
-000122c0: 6d6f 6475 6c65 5f6c 6973 7427 5d0a 2020  module_list'].  
-000122d0: 2020 7372 635f 616c 6c5f 6d6f 6475 6c65    src_all_module
-000122e0: 5f6c 6973 7420 3d20 6f64 6f6f 5f64 6570  _list = odoo_dep
-000122f0: 656e 6465 6e63 6965 7328 0a20 2020 2020  endencies(.     
-00012300: 2020 2073 7263 5f63 7478 2c20 276d 6f64     src_ctx, 'mod
-00012310: 272c 2046 616c 7365 2c20 4661 6c73 652c  ', False, False,
-00012320: 2073 7263 5f70 6174 6873 2c0a 2020 2020   src_paths,.    
-00012330: 2020 2020 7372 635f 6374 785b 2773 7263      src_ctx['src
-00012340: 5f6f 646f 6f5f 6676 6572 275d 290a 2020  _odoo_fver']).  
-00012350: 2020 7467 745f 616c 6c5f 6d6f 6475 6c65    tgt_all_module
-00012360: 5f6c 6973 7420 3d20 6f64 6f6f 5f64 6570  _list = odoo_dep
-00012370: 656e 6465 6e63 6965 7328 0a20 2020 2020  endencies(.     
-00012380: 2020 2074 6774 5f63 7478 2c20 276d 6f64     tgt_ctx, 'mod
-00012390: 272c 2046 616c 7365 2c20 4661 6c73 652c  ', False, False,
-000123a0: 2074 6774 5f70 6174 6873 2c0a 2020 2020   tgt_paths,.    
-000123b0: 2020 2020 7467 745f 6374 785b 2774 6774      tgt_ctx['tgt
-000123c0: 5f6f 646f 6f5f 6676 6572 275d 290a 2020  _odoo_fver']).  
-000123d0: 2020 7372 635f 6374 785b 2774 6e6c 5f6d    src_ctx['tnl_m
-000123e0: 6f64 756c 655f 6c69 7374 275d 2c20 6261  odule_list'], ba
-000123f0: 645f 6d6f 6475 6c65 5f6c 6973 7420 3d20  d_module_list = 
-00012400: 5c0a 2020 2020 2020 2020 646f 5f74 6e6c  \.        do_tnl
-00012410: 5f6d 6f64 756c 655f 6c69 7374 2873 7263  _module_list(src
-00012420: 5f63 7478 2c0a 2020 2020 2020 2020 2020  _ctx,.          
-00012430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012440: 2073 7263 5f63 7478 5b27 7372 635f 6d6f   src_ctx['src_mo
-00012450: 6475 6c65 5f6c 6973 7427 5d2c 0a20 2020  dule_list'],.   
-00012460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012470: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-00012480: 2773 7263 5f6f 646f 6f5f 6676 6572 275d  'src_odoo_fver']
-00012490: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000124a0: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
-000124b0: 5f63 7478 5b27 7467 745f 6f64 6f6f 5f66  _ctx['tgt_odoo_f
-000124c0: 7665 7227 5d2c 0a20 2020 2020 2020 2020  ver'],.         
-000124d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124e0: 2020 7467 745f 616c 6c5f 6d6f 6475 6c65    tgt_all_module
-000124f0: 5f6c 6973 742c 0a20 2020 2020 2020 2020  _list,.         
-00012500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012510: 2020 7075 7265 3d54 7275 6529 0a20 2020    pure=True).   
-00012520: 206f 7330 2e77 6c6f 6728 0a20 2020 2020   os0.wlog(.     
-00012530: 2020 2027 5472 616e 736c 6174 6564 206c     'Translated l
-00012540: 6973 7420 6166 7465 7220 6d69 6772 6174  ist after migrat
-00012550: 696f 6e3d 2573 2720 2520 7372 635f 6374  ion=%s' % src_ct
-00012560: 785b 2774 6e6c 5f6d 6f64 756c 655f 6c69  x['tnl_module_li
-00012570: 7374 275d 290a 2020 2020 6675 6c6c 5f74  st']).    full_t
-00012580: 6e6c 5f6d 6f64 756c 655f 6c69 7374 203d  nl_module_list =
-00012590: 206f 646f 6f5f 6465 7065 6e64 656e 6369   odoo_dependenci
-000125a0: 6573 280a 2020 2020 2020 2020 7467 745f  es(.        tgt_
-000125b0: 6374 782c 2027 6465 7027 2c20 4661 6c73  ctx, 'dep', Fals
-000125c0: 652c 2046 616c 7365 2c20 7467 745f 7061  e, False, tgt_pa
-000125d0: 7468 732c 0a20 2020 2020 2020 2074 6774  ths,.        tgt
-000125e0: 5f63 7478 5b27 7372 635f 6f64 6f6f 5f66  _ctx['src_odoo_f
-000125f0: 7665 7227 5d2c 206d 6174 6368 6573 3d73  ver'], matches=s
-00012600: 7263 5f63 7478 5b27 746e 6c5f 6d6f 6475  rc_ctx['tnl_modu
-00012610: 6c65 5f6c 6973 7427 5d29 0a20 2020 206f  le_list']).    o
-00012620: 7330 2e77 6c6f 6728 0a20 2020 2020 2020  s0.wlog(.       
-00012630: 2027 5461 7267 6574 206c 6973 7420 7769   'Target list wi
-00012640: 7468 2064 6570 656e 6465 6e63 6965 733d  th dependencies=
-00012650: 2573 2720 2520 6675 6c6c 5f74 6e6c 5f6d  %s' % full_tnl_m
-00012660: 6f64 756c 655f 6c69 7374 290a 2020 2020  odule_list).    
-00012670: 6f73 302e 776c 6f67 280a 2020 2020 2020  os0.wlog(.      
-00012680: 2020 274e 6f74 2061 7661 6961 626c 6520    'Not avaiable 
-00012690: 6d6f 6475 6c65 7320 6f6e 2074 6172 6765  modules on targe
-000126a0: 743d 2573 2720 2520 6261 645f 6d6f 6475  t=%s' % bad_modu
-000126b0: 6c65 5f6c 6973 7429 0a20 2020 2069 6620  le_list).    if 
-000126c0: 2862 6164 5f6d 6f64 756c 655f 6c69 7374  (bad_module_list
-000126d0: 2061 6e64 0a20 2020 2020 2020 2020 2020   and.           
-000126e0: 2073 7263 5f63 7478 5b27 7265 6475 6374   src_ctx['reduct
-000126f0: 6564 5f6d 6f64 756c 655f 7365 7427 5d20  ed_module_set'] 
-00012700: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-00012710: 6e6f 7420 7372 635f 6374 785b 2764 7279  not src_ctx['dry
-00012720: 5f72 756e 275d 293a 0a20 2020 2020 2020  _run']):.       
-00012730: 2066 6f72 2069 2c6d 6f64 756c 6520 696e   for i,module in
-00012740: 2065 6e75 6d65 7261 7465 2862 6164 5f6d   enumerate(bad_m
-00012750: 6f64 756c 655f 6c69 7374 293a 0a20 2020  odule_list):.   
-00012760: 2020 2020 2020 2020 2073 7473 203d 2064           sts = d
-00012770: 726f 705f 6d6f 6475 6c65 2873 7263 5f63  rop_module(src_c
-00012780: 7478 2c20 6d6f 6475 6c65 290a 2020 2020  tx, module).    
-00012790: 2020 2020 2020 2020 6966 2073 7473 3a0a          if sts:.
-000127a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127b0: 6465 6c20 6261 645f 6d6f 6475 6c65 5f6c  del bad_module_l
-000127c0: 6973 745b 695d 0a20 2020 2073 6f66 745f  ist[i].    soft_
-000127d0: 756e 696e 7374 616c 6c5f 6c69 7374 203d  uninstall_list =
-000127e0: 2068 6172 645f 756e 696e 7374 616c 6c5f   hard_uninstall_
-000127f0: 6c69 7374 203d 205b 5d0a 2020 2020 6966  list = [].    if
-00012800: 2074 6774 5f63 7478 5b27 6f63 615f 6d69   tgt_ctx['oca_mi
-00012810: 6772 6174 6527 5d20 616e 6420 7467 745f  grate'] and tgt_
-00012820: 6374 785b 2774 6774 5f6f 646f 6f5f 7665  ctx['tgt_odoo_ve
-00012830: 7227 5d20 3c20 3130 3a0a 2020 2020 2020  r'] < 10:.      
-00012840: 2020 6f75 5f76 6572 5f70 6174 6820 3d20    ou_ver_path = 
-00012850: 6c6f 6164 5f6f 7065 6e75 7067 7261 6465  load_openupgrade
-00012860: 2874 6774 5f63 7478 2c20 7467 745f 6374  (tgt_ctx, tgt_ct
-00012870: 785b 2774 6774 5f6f 646f 6f5f 6676 6572  x['tgt_odoo_fver
-00012880: 275d 290a 2020 2020 2020 2020 636d 6420  ']).        cmd 
-00012890: 3d20 6f73 2e70 6174 682e 6a6f 696e 286f  = os.path.join(o
-000128a0: 755f 7665 725f 7061 7468 2c20 2773 6372  u_ver_path, 'scr
-000128b0: 6970 7473 272c 2027 6d69 6772 6174 652e  ipts', 'migrate.
-000128c0: 7079 2729 0a20 2020 2020 2020 2069 6620  py').        if 
-000128d0: 7372 635f 6374 785b 276e 6f5f 7665 6e76  src_ctx['no_venv
-000128e0: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
-000128f0: 7275 6e5f 7472 6163 6564 2863 6d64 2c0a  run_traced(cmd,.
-00012900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012910: 2020 2020 2020 2027 2d43 272c 2073 7263         '-C', src
-00012920: 5f66 756c 6c5f 6c63 6f6e 662c 0a20 2020  _full_lconf,.   
-00012930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012940: 2020 2020 272d 4427 2c20 7372 635f 6374      '-D', src_ct
-00012950: 785b 2764 625f 6e61 6d65 275d 2c0a 2020  x['db_name'],.  
-00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012970: 2020 2020 2027 2d42 272c 2073 7263 5f63       '-B', src_c
-00012980: 7478 5b27 6f70 745f 6f75 7061 7468 275d  tx['opt_oupath']
-00012990: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000129a0: 2020 2020 2020 2020 2027 2d52 272c 2074           '-R', t
-000129b0: 6774 5f63 7478 5b27 7467 745f 6f64 6f6f  gt_ctx['tgt_odoo
-000129c0: 5f66 7665 7227 5d29 0a20 2020 2020 2020  _fver']).       
-000129d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000129e0: 2020 2073 6372 6970 7420 3d20 6f73 2e70     script = os.p
-000129f0: 6174 682e 6a6f 696e 286f 755f 7665 725f  ath.join(ou_ver_
-00012a00: 7061 7468 2c20 276d 6967 7261 7465 2e73  path, 'migrate.s
-00012a10: 6827 290a 2020 2020 2020 2020 2020 2020  h').            
-00012a20: 6664 203d 206f 7065 6e28 7363 7269 7074  fd = open(script
-00012a30: 2c20 2777 2729 0a20 2020 2020 2020 2020  , 'w').         
-00012a40: 2020 2066 642e 7772 6974 6528 2763 6420     fd.write('cd 
-00012a50: 2573 5c6e 2720 2520 7467 745f 6374 785b  %s\n' % tgt_ctx[
-00012a60: 2776 656e 765f 6f75 7061 7468 275d 290a  'venv_oupath']).
-00012a70: 2020 2020 2020 2020 2020 2020 6664 2e77              fd.w
-00012a80: 7269 7465 2827 736f 7572 6365 202e 2f62  rite('source ./b
-00012a90: 696e 2f61 6374 6976 6174 655c 6e27 290a  in/activate\n').
-00012aa0: 2020 2020 2020 2020 2020 2020 6664 2e77              fd.w
-00012ab0: 7269 7465 2827 2573 202d 4320 2573 202d  rite('%s -C %s -
-00012ac0: 4420 2573 202d 4220 2573 202d 5220 2573  D %s -B %s -R %s
-00012ad0: 5c6e 2720 2520 280a 2020 2020 2020 2020  \n' % (.        
-00012ae0: 2020 2020 2020 2020 636d 642c 2073 7263          cmd, src
-00012af0: 5f66 756c 6c5f 6c63 6f6e 662c 0a20 2020  _full_lconf,.   
-00012b00: 2020 2020 2020 2020 2020 2020 2073 7263               src
-00012b10: 5f63 7478 5b27 6462 5f6e 616d 6527 5d2c  _ctx['db_name'],
-00012b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012b30: 2073 7263 5f63 7478 5b27 6f70 745f 6f75   src_ctx['opt_ou
-00012b40: 7061 7468 275d 2c0a 2020 2020 2020 2020  path'],.        
-00012b50: 2020 2020 2020 2020 7467 745f 6374 785b          tgt_ctx[
-00012b60: 2774 6774 5f6f 646f 6f5f 6676 6572 275d  'tgt_odoo_fver']
-00012b70: 2929 0a20 2020 2020 2020 2020 2020 2066  )).            f
-00012b80: 642e 7772 6974 6528 2764 6561 6374 6976  d.write('deactiv
-00012b90: 6174 655c 6e27 290a 2020 2020 2020 2020  ate\n').        
-00012ba0: 2020 2020 6664 2e63 6c6f 7365 2829 0a20      fd.close(). 
-00012bb0: 2020 2020 2020 2020 2020 206f 732e 6368             os.ch
-00012bc0: 6d6f 6428 7363 7269 7074 2c20 306f 3734  mod(script, 0o74
-00012bd0: 3429 0a20 2020 2020 2020 2020 2020 2069  4).            i
-00012be0: 6620 6e6f 7420 7372 635f 6374 785b 2764  f not src_ctx['d
-00012bf0: 7279 5f72 756e 275d 3a0a 2020 2020 2020  ry_run']:.      
-00012c00: 2020 2020 2020 2020 2020 6f73 2e73 7973            os.sys
-00012c10: 7465 6d28 7363 7269 7074 290a 2020 2020  tem(script).    
-00012c20: 2020 2020 6966 206e 6f74 2073 7263 5f63      if not src_c
-00012c30: 7478 5b27 6472 795f 7275 6e27 5d3a 0a20  tx['dry_run']:. 
-00012c40: 2020 2020 2020 2020 2020 2074 696d 652e             time.
-00012c50: 736c 6565 7028 3529 0a20 2020 2020 2020  sleep(5).       
-00012c60: 2074 6d70 5f64 626e 616d 6520 3d20 6e65   tmp_dbname = ne
-00012c70: 775f 6462 6e61 6d65 2873 7263 5f63 7478  w_dbname(src_ctx
-00012c80: 5b27 6462 5f6e 616d 6527 5d2c 0a20 2020  ['db_name'],.   
-00012c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ca0: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
-00012cb0: 5f63 7478 5b27 7467 745f 6f64 6f6f 5f76  _ctx['tgt_odoo_v
-00012cc0: 6572 275d 2c0a 2020 2020 2020 2020 2020  er'],.          
-00012cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ce0: 2020 2020 2020 7467 745f 6374 785b 276f        tgt_ctx['o
-00012cf0: 6361 5f6d 6967 7261 7465 275d 290a 2020  ca_migrate']).  
-00012d00: 2020 2020 2020 6966 206e 6f74 2073 7263        if not src
-00012d10: 5f63 7478 5b27 6472 795f 7275 6e27 5d3a  _ctx['dry_run']:
-00012d20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00012d30: 7467 745f 6374 785b 2764 625f 6e61 6d65  tgt_ctx['db_name
-00012d40: 275d 2021 3d20 746d 705f 6462 6e61 6d65  '] != tmp_dbname
-00012d50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012d60: 2020 7265 6e5f 6462 2874 6d70 5f64 626e    ren_db(tmp_dbn
-00012d70: 616d 652c 2074 6774 5f63 7478 5b27 6462  ame, tgt_ctx['db
-00012d80: 5f6e 616d 6527 5d2c 2073 7263 5f63 7478  _name'], src_ctx
-00012d90: 5b27 6462 5f75 7365 7227 5d29 0a20 2020  ['db_user']).   
-00012da0: 2020 2020 2020 2020 2069 6620 7372 635f           if src_
-00012db0: 6374 785b 2764 625f 7573 6572 275d 2021  ctx['db_user'] !
-00012dc0: 3d20 7467 745f 6374 785b 2764 625f 7573  = tgt_ctx['db_us
-00012dd0: 6572 275d 3a0a 2020 2020 2020 2020 2020  er']:.          
-00012de0: 2020 2020 2020 7265 6173 7369 676e 5f64        reassign_d
-00012df0: 625f 6f77 6e65 7228 7467 745f 6374 782c  b_owner(tgt_ctx,
-00012e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e20: 2020 2074 6774 5f63 7478 5b27 6462 5f6e     tgt_ctx['db_n
-00012e30: 616d 6527 5d2c 0a20 2020 2020 2020 2020  ame'],.         
-00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e50: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
-00012e60: 5b27 6462 5f75 7365 7227 5d2c 0a20 2020  ['db_user'],.   
-00012e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e80: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00012e90: 6774 5f63 7478 5b27 6462 5f75 7365 7227  gt_ctx['db_user'
-00012ea0: 5d29 0a20 2020 2020 2020 2074 6774 5f66  ]).        tgt_f
-00012eb0: 756c 6c5f 6c63 6f6e 6620 3d20 7467 745f  ull_lconf = tgt_
-00012ec0: 6374 785b 2763 6f6e 665f 666e 275d 0a20  ctx['conf_fn']. 
-00012ed0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00012ee0: 206f 755f 7665 725f 7061 7468 203d 206c   ou_ver_path = l
-00012ef0: 6f61 645f 6f70 656e 7570 6772 6164 6528  oad_openupgrade(
-00012f00: 7467 745f 6374 782c 2074 6774 5f63 7478  tgt_ctx, tgt_ctx
-00012f10: 5b27 7467 745f 6f64 6f6f 5f66 7665 7227  ['tgt_odoo_fver'
-00012f20: 5d29 0a20 2020 2020 2020 2069 6620 6e6f  ]).        if no
-00012f30: 7420 7372 635f 6374 785b 2764 7279 5f72  t src_ctx['dry_r
-00012f40: 756e 275d 3a0a 2020 2020 2020 2020 2020  un']:.          
-00012f50: 2020 6c6f 6164 5f6f 7065 6e75 7067 7261    load_openupgra
-00012f60: 6465 6c69 6228 7372 635f 6374 782c 2074  delib(src_ctx, t
-00012f70: 6774 5f63 7478 5b27 7467 745f 6f64 6f6f  gt_ctx['tgt_odoo
-00012f80: 5f66 7665 7227 5d29 0a20 2020 2020 2020  _fver']).       
-00012f90: 2069 6620 7467 745f 6374 785b 2775 7064   if tgt_ctx['upd
-00012fa0: 5f74 7261 6e73 6c61 7469 6f6e 275d 3a0a  _translation']:.
-00012fb0: 2020 2020 2020 2020 2020 2020 6164 645f              add_
-00012fc0: 7665 7273 696f 6e65 645f 746e 6c28 7372  versioned_tnl(sr
-00012fd0: 635f 6374 782c 2073 7263 5f63 7478 5b27  c_ctx, src_ctx['
-00012fe0: 7372 635f 6f64 6f6f 5f66 7665 7227 5d2c  src_odoo_fver'],
-00012ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013000: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00013010: 6774 5f63 7478 5b27 7467 745f 6f64 6f6f  gt_ctx['tgt_odoo
-00013020: 5f66 7665 7227 5d29 0a20 2020 2020 2020  _fver']).       
-00013030: 2061 6464 6f6e 735f 7061 7468 203d 206f   addons_path = o
-00013040: 732e 7061 7468 2e6a 6f69 6e28 6f75 5f76  s.path.join(ou_v
-00013050: 6572 5f70 6174 682c 2027 6164 646f 6e73  er_path, 'addons
-00013060: 2729 0a20 2020 2020 2020 2069 6620 7467  ').        if tg
-00013070: 745f 6374 785b 2774 6774 5f6f 646f 6f5f  t_ctx['tgt_odoo_
-00013080: 7665 7227 5d20 3c20 3130 3a0a 2020 2020  ver'] < 10:.    
-00013090: 2020 2020 2020 2020 726f 6f74 5f70 6174          root_pat
-000130a0: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
-000130b0: 286f 755f 7665 725f 7061 7468 2c20 276f  (ou_ver_path, 'o
-000130c0: 7065 6e65 7270 272c 2027 6164 646f 6e73  penerp', 'addons
-000130d0: 2729 0a20 2020 2020 2020 2065 6c73 653a  ').        else:
-000130e0: 0a20 2020 2020 2020 2020 2020 2072 6f6f  .            roo
-000130f0: 745f 7061 7468 203d 206f 732e 7061 7468  t_path = os.path
-00013100: 2e6a 6f69 6e28 6f75 5f76 6572 5f70 6174  .join(ou_ver_pat
-00013110: 682c 2027 6f64 6f6f 272c 2027 6164 646f  h, 'odoo', 'addo
-00013120: 6e73 2729 0a20 2020 2020 2020 2069 6620  ns').        if 
-00013130: 6e6f 7420 7372 635f 6374 785b 2764 7279  not src_ctx['dry
-00013140: 5f72 756e 275d 3a0a 2020 2020 2020 2020  _run']:.        
-00013150: 2020 2020 666f 7220 7265 706f 2069 6e20      for repo in 
-00013160: 7467 745f 7061 7468 733a 0a20 2020 2020  tgt_paths:.     
-00013170: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
-00013180: 616d 6520 696e 206f 732e 6c69 7374 6469  ame in os.listdi
-00013190: 7228 7265 706f 293a 0a20 2020 2020 2020  r(repo):.       
-000131a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000131b0: 286f 732e 7061 7468 2e69 7364 6972 286f  (os.path.isdir(o
-000131c0: 732e 7061 7468 2e6a 6f69 6e28 7265 706f  s.path.join(repo
-000131d0: 2c20 6e61 6d65 2929 2061 6e64 0a20 2020  , name)) and.   
-000131e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131f0: 2020 2020 2020 2020 206e 6f74 206f 732e           not os.
-00013200: 7061 7468 2e69 7364 6972 280a 2020 2020  path.isdir(.    
-00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013220: 2020 2020 2020 2020 2020 2020 6f73 2e70              os.p
-00013230: 6174 682e 6a6f 696e 2861 6464 6f6e 735f  ath.join(addons_
-00013240: 7061 7468 2c20 6e61 6d65 2929 2061 6e64  path, name)) and
-00013250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013260: 2020 2020 2020 2020 2020 2020 206e 6f74               not
-00013270: 206f 732e 7061 7468 2e69 7364 6972 286f   os.path.isdir(o
-00013280: 732e 7061 7468 2e6a 6f69 6e28 726f 6f74  s.path.join(root
-00013290: 5f70 6174 682c 206e 616d 6529 2929 3a0a  _path, name))):.
-000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132b0: 2020 2020 2020 2020 6f73 2e73 796d 6c69          os.symli
-000132c0: 6e6b 286f 732e 7061 7468 2e6a 6f69 6e28  nk(os.path.join(
-000132d0: 7265 706f 2c20 6e61 6d65 292c 0a20 2020  repo, name),.   
-000132e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013300: 6f73 2e70 6174 682e 6a6f 696e 2861 6464  os.path.join(add
-00013310: 6f6e 735f 7061 7468 2c20 6e61 6d65 2929  ons_path, name))
-00013320: 0a20 2020 2020 2020 2074 6774 5f70 6174  .        tgt_pat
-00013330: 6873 203d 205b 5d0a 2020 2020 2020 2020  hs = [].        
-00013340: 7467 745f 7061 7468 732e 696e 7365 7274  tgt_paths.insert
-00013350: 2830 2c20 6164 646f 6e73 5f70 6174 6829  (0, addons_path)
-00013360: 0a20 2020 2020 2020 2074 6774 5f70 6174  .        tgt_pat
-00013370: 6873 2e69 6e73 6572 7428 302c 2072 6f6f  hs.insert(0, roo
-00013380: 745f 7061 7468 290a 2020 2020 2020 2020  t_path).        
-00013390: 7467 745f 6675 6c6c 5f6c 636f 6e66 203d  tgt_full_lconf =
-000133a0: 2070 7265 7061 7265 5f63 6f6e 6669 675f   prepare_config_
-000133b0: 6669 6c65 2874 6774 5f63 7478 2c20 7467  file(tgt_ctx, tg
-000133c0: 745f 636f 6e66 6967 2c0a 2020 2020 2020  t_config,.      
-000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133f0: 2020 2020 2020 206f 755f 7665 725f 7061         ou_ver_pa
-00013400: 7468 3d6f 755f 7665 725f 7061 7468 2c0a  th=ou_ver_path,.
-00013410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013430: 2020 2020 2020 2020 2020 2020 2070 6174               pat
-00013440: 6873 3d74 6774 5f70 6174 6873 290a 2020  hs=tgt_paths).  
-00013450: 2020 2020 2020 6966 206e 6f74 2073 7263        if not src
-00013460: 5f63 7478 5b27 6472 795f 7275 6e27 5d3a  _ctx['dry_run']:
-00013470: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013480: 6e6f 7420 636f 7079 5f64 6228 7372 635f  not copy_db(src_
-00013490: 6374 782c 2073 7263 5f63 7478 5b27 6462  ctx, src_ctx['db
-000134a0: 5f6e 616d 6527 5d2c 2074 6774 5f63 7478  _name'], tgt_ctx
-000134b0: 5b27 6462 5f6e 616d 6527 5d29 3a0a 2020  ['db_name']):.  
-000134c0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-000134d0: 6974 2831 290a 2020 2020 2020 2020 2020  it(1).          
-000134e0: 2020 6669 785f 6275 675f 7072 6528 7372    fix_bug_pre(sr
-000134f0: 635f 6374 782c 2074 6774 5f63 7478 2c20  c_ctx, tgt_ctx, 
-00013500: 7372 635f 6675 6c6c 5f6c 636f 6e66 2c20  src_full_lconf, 
-00013510: 7372 635f 7061 7468 7329 0a20 2020 2020  src_paths).     
-00013520: 2020 2020 2020 2069 6620 7372 635f 6374         if src_ct
-00013530: 785b 2764 625f 7573 6572 275d 2021 3d20  x['db_user'] != 
-00013540: 7467 745f 6374 785b 2764 625f 7573 6572  tgt_ctx['db_user
-00013550: 275d 3a0a 2020 2020 2020 2020 2020 2020  ']:.            
-00013560: 2020 2020 7265 6173 7369 676e 5f64 625f      reassign_db_
-00013570: 6f77 6e65 7228 7467 745f 6374 782c 0a20  owner(tgt_ctx,. 
-00013580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135a0: 2074 6774 5f63 7478 5b27 6462 5f6e 616d   tgt_ctx['db_nam
-000135b0: 6527 5d2c 0a20 2020 2020 2020 2020 2020  e'],.           
-000135c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135d0: 2020 2020 2020 2073 7263 5f63 7478 5b27         src_ctx['
-000135e0: 6462 5f75 7365 7227 5d2c 0a20 2020 2020  db_user'],.     
-000135f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013600: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
-00013610: 5f63 7478 5b27 6462 5f75 7365 7227 5d29  _ctx['db_user'])
-00013620: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
-00013630: 6f6d 6520 6d6f 6475 6c65 7320 6e6f 7420  ome modules not 
-00013640: 6176 6169 6c61 626c 6520 6f6e 2069 6e74  available on int
-00013650: 6572 6d65 6469 6174 6520 7665 7273 696f  ermediate versio
-00013660: 6e20 6d69 6768 7420 6265 0a20 2020 2020  n might be.     
-00013670: 2020 2020 2020 2023 2061 7661 696c 6162         # availab
-00013680: 6c65 206f 6e20 6375 7272 656e 7420 7461  le on current ta
-00013690: 7267 6574 206f 646f 6f20 7665 7273 696f  rget odoo versio
-000136a0: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
-000136b0: 2074 6774 5f63 7478 5b27 7472 795f 7265   tgt_ctx['try_re
-000136c0: 696e 7374 616c 6c27 5d3a 0a20 2020 2020  install']:.     
-000136d0: 2020 2020 2020 2020 2020 206d 6f64 756c             modul
-000136e0: 6573 5f74 6f5f 7265 7374 6f72 6520 3d20  es_to_restore = 
-000136f0: 6261 645f 6c69 7374 203d 205b 5d0a 2020  bad_list = [].  
-00013700: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00013710: 2073 7263 5f63 7478 5b27 6f72 6967 696e   src_ctx['origin
-00013720: 616c 5f6d 6f64 756c 655f 6c69 7374 275d  al_module_list']
-00013730: 2021 3d20 7372 635f 6374 785b 0a20 2020   != src_ctx[.   
-00013740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013750: 2020 2020 2027 7372 635f 6d6f 6475 6c65       'src_module
-00013760: 5f6c 6973 7427 5d3a 0a20 2020 2020 2020  _list']:.       
-00013770: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00013780: 756c 6573 5f74 6f5f 7265 7374 6f72 652c  ules_to_restore,
-00013790: 2062 6164 5f6c 6973 7420 3d20 646f 5f74   bad_list = do_t
-000137a0: 6e6c 5f6d 6f64 756c 655f 6c69 7374 280a  nl_module_list(.
-000137b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137c0: 2020 2020 2020 2020 7467 745f 6374 782c          tgt_ctx,
-000137d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000137e0: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
-000137f0: 5b27 6f72 6967 696e 616c 5f6d 6f64 756c  ['original_modul
-00013800: 655f 6c69 7374 275d 2c0a 2020 2020 2020  e_list'],.      
-00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013820: 2020 7372 635f 6374 785b 2766 726f 6d5f    src_ctx['from_
-00013830: 6f64 6f6f 5f66 7665 7227 5d2c 0a20 2020  odoo_fver'],.   
-00013840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013850: 2020 2020 2074 6774 5f63 7478 5b27 7467       tgt_ctx['tg
-00013860: 745f 6f64 6f6f 5f66 7665 7227 5d2c 0a20  t_odoo_fver'],. 
-00013870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013880: 2020 2020 2020 2074 6774 5f61 6c6c 5f6d         tgt_all_m
-00013890: 6f64 756c 655f 6c69 7374 2c0a 2020 2020  odule_list,.    
-000138a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138b0: 2020 2020 7075 7265 3d54 7275 6529 0a20      pure=True). 
-000138c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138d0: 2020 206d 6f64 756c 6573 5f74 6f5f 7265     modules_to_re
-000138e0: 7374 6f72 6520 3d20 6c69 7374 2873 6574  store = list(set
-000138f0: 286d 6f64 756c 6573 5f74 6f5f 7265 7374  (modules_to_rest
-00013900: 6f72 6529 202d 0a20 2020 2020 2020 2020  ore) -.         
-00013910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013930: 2020 2020 2073 6574 2873 7263 5f63 7478       set(src_ctx
-00013940: 5b27 7372 635f 6d6f 6475 6c65 5f6c 6973  ['src_module_lis
-00013950: 7427 5d29 290a 2020 2020 2020 2020 2020  t'])).          
-00013960: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-00013970: 756c 6573 5f74 6f5f 7265 7374 6f72 653a  ules_to_restore:
-00013980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013990: 2020 2020 2020 2020 2073 6574 5f69 6e73           set_ins
-000139a0: 7461 6c6c 6564 5f62 795f 7371 6c28 7467  talled_by_sql(tg
-000139b0: 745f 6374 782c 206d 6f64 756c 6573 5f74  t_ctx, modules_t
-000139c0: 6f5f 7265 7374 6f72 6529 0a20 2020 2020  o_restore).     
-000139d0: 2020 2020 2020 2064 726f 705f 7365 7373         drop_sess
-000139e0: 696f 6e28 7467 745f 6374 782c 2074 6774  ion(tgt_ctx, tgt
-000139f0: 5f63 7478 5b27 6462 5f6e 616d 6527 5d2c  _ctx['db_name'],
-00013a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013a10: 2020 2020 2020 2020 2020 6f64 6f6f 5f76            odoo_v
-00013a20: 6964 3d74 6774 5f63 7478 5b27 7467 745f  id=tgt_ctx['tgt_
-00013a30: 7669 6427 5d29 0a20 2020 2020 2020 2072  vid']).        r
-00013a40: 756e 5f6f 7065 6e75 7067 7261 6465 2874  un_openupgrade(t
-00013a50: 6774 5f63 7478 2c20 6f75 5f76 6572 5f70  gt_ctx, ou_ver_p
-00013a60: 6174 682c 2074 6774 5f66 756c 6c5f 6c63  ath, tgt_full_lc
-00013a70: 6f6e 6629 0a20 2020 2020 2020 2069 6620  onf).        if 
-00013a80: 6e6f 7420 7372 635f 6374 785b 2764 7279  not src_ctx['dry
-00013a90: 5f72 756e 275d 3a0a 2020 2020 2020 2020  _run']:.        
-00013aa0: 2020 2020 6669 785f 6275 675f 706f 7374      fix_bug_post
-00013ab0: 2873 7263 5f63 7478 2c20 7467 745f 6374  (src_ctx, tgt_ct
-00013ac0: 782c 2073 7263 5f66 756c 6c5f 6c63 6f6e  x, src_full_lcon
-00013ad0: 662c 2073 7263 5f70 6174 6873 290a 0a20  f, src_paths).. 
-00013ae0: 2020 2023 2054 6573 7420 666f 7220 6e6f     # Test for no
-00013af0: 7420 6d69 6772 6174 6564 206d 6f64 756c  t migrated modul
-00013b00: 6573 0a20 2020 2074 6774 5f63 7478 5b27  es.    tgt_ctx['
-00013b10: 636f 6e66 5f66 6e27 5d20 3d20 7467 745f  conf_fn'] = tgt_
-00013b20: 7361 7665 645f 6663 6f6e 660a 2020 2020  saved_fconf.    
-00013b30: 746f 5f75 6e69 6e73 7461 6c6c 5f6c 6973  to_uninstall_lis
-00013b40: 7420 3d20 6765 745f 7772 6f6e 675f 6d6f  t = get_wrong_mo
-00013b50: 6475 6c65 7328 7467 745f 6374 7829 0a20  dules(tgt_ctx). 
-00013b60: 2020 2069 6620 746f 5f75 6e69 6e73 7461     if to_uninsta
-00013b70: 6c6c 5f6c 6973 743a 0a20 2020 2020 2020  ll_list:.       
-00013b80: 206f 7330 2e77 6c6f 6728 272a 2a2a 2057   os0.wlog('*** W
-00013b90: 726f 6e67 2073 7461 7465 2066 6f72 206d  rong state for m
-00013ba0: 6f64 756c 6573 2025 7320 2a2a 2a27 2025  odules %s ***' %
-00013bb0: 2074 6f5f 756e 696e 7374 616c 6c5f 6c69   to_uninstall_li
-00013bc0: 7374 290a 2020 2020 6861 7264 5f75 6e69  st).    hard_uni
-00013bd0: 6e73 7461 6c6c 5f6c 6973 7420 3d20 6c69  nstall_list = li
-00013be0: 7374 280a 2020 2020 2020 2020 7365 7428  st(.        set(
-00013bf0: 746f 5f75 6e69 6e73 7461 6c6c 5f6c 6973  to_uninstall_lis
-00013c00: 7429 2026 2073 6574 284d 4f44 554c 4553  t) & set(MODULES
-00013c10: 5f32 5f4c 4541 5645 5f42 4548 494e 4429  _2_LEAVE_BEHIND)
-00013c20: 290a 2020 2020 736f 6674 5f75 6e69 6e73  ).    soft_unins
-00013c30: 7461 6c6c 5f6c 6973 7420 3d20 6c69 7374  tall_list = list
-00013c40: 280a 2020 2020 2020 2020 7365 7428 746f  (.        set(to
-00013c50: 5f75 6e69 6e73 7461 6c6c 5f6c 6973 7429  _uninstall_list)
-00013c60: 202d 2073 6574 2868 6172 645f 756e 696e   - set(hard_unin
-00013c70: 7374 616c 6c5f 6c69 7374 2929 0a20 2020  stall_list)).   
-00013c80: 2069 6620 736f 6674 5f75 6e69 6e73 7461   if soft_uninsta
-00013c90: 6c6c 5f6c 6973 743a 0a20 2020 2020 2020  ll_list:.       
-00013ca0: 2073 6574 5f75 6e69 6e73 7461 6c6c 6564   set_uninstalled
-00013cb0: 5f62 795f 7371 6c28 7467 745f 6374 782c  _by_sql(tgt_ctx,
-00013cc0: 2073 6f66 745f 756e 696e 7374 616c 6c5f   soft_uninstall_
-00013cd0: 6c69 7374 290a 2020 2020 6966 2068 6172  list).    if har
-00013ce0: 645f 756e 696e 7374 616c 6c5f 6c69 7374  d_uninstall_list
-00013cf0: 3a0a 2020 2020 2020 2020 6f73 302e 776c  :.        os0.wl
-00013d00: 6f67 2827 2a2a 2a20 556e 7374 6162 6c65  og('*** Unstable
-00013d10: 2044 423a 2077 726f 6e67 206d 6f64 756c   DB: wrong modul
-00013d20: 6520 7374 6174 6520 2573 202a 2a2a 2720  e state %s ***' 
-00013d30: 250a 2020 2020 2020 2020 2020 2020 2020  %.              
-00013d40: 2020 2068 6172 645f 756e 696e 7374 616c     hard_uninstal
-00013d50: 6c5f 6c69 7374 290a 2020 2020 666f 7220  l_list).    for 
-00013d60: 6d6f 6475 6c65 2069 6e20 6861 7264 5f75  module in hard_u
-00013d70: 6e69 6e73 7461 6c6c 5f6c 6973 743a 0a20  ninstall_list:. 
-00013d80: 2020 2020 2020 206f 7330 2e77 6c6f 6728         os0.wlog(
-00013d90: 2720 202b 2b20 4861 7264 2075 6e69 6e73  '  ++ Hard unins
-00013da0: 7461 6c6c 3a20 2573 2720 2520 6d6f 6475  tall: %s' % modu
-00013db0: 6c65 290a 2020 2020 2020 2020 6861 7264  le).        hard
-00013dc0: 5f63 6c65 616e 5f6d 6f64 756c 6528 7467  _clean_module(tg
-00013dd0: 745f 6374 782c 206d 6f64 756c 6529 0a20  t_ctx, module). 
-00013de0: 2020 2069 6620 736f 6674 5f75 6e69 6e73     if soft_unins
-00013df0: 7461 6c6c 5f6c 6973 7420 6f72 2068 6172  tall_list or har
-00013e00: 645f 756e 696e 7374 616c 6c5f 6c69 7374  d_uninstall_list
-00013e10: 3a0a 2020 2020 2020 2020 6261 645f 6d6f  :.        bad_mo
-00013e20: 6475 6c65 7320 3d20 6c69 7374 2873 6574  dules = list(set
-00013e30: 2873 6f66 745f 756e 696e 7374 616c 6c5f  (soft_uninstall_
-00013e40: 6c69 7374 2920 7c20 7365 7428 6861 7264  list) | set(hard
-00013e50: 5f75 6e69 6e73 7461 6c6c 5f6c 6973 7429  _uninstall_list)
-00013e60: 290a 2020 2020 2020 2020 7275 6e5f 6f64  ).        run_od
-00013e70: 6f6f 5f61 6c6c 7465 7374 2874 6774 5f63  oo_alltest(tgt_c
-00013e80: 7478 5b27 7467 745f 7669 6427 5d2c 2074  tx['tgt_vid'], t
-00013e90: 6774 5f63 7478 5b27 636f 6e66 5f66 6e27  gt_ctx['conf_fn'
-00013ea0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00013eb0: 2020 2020 2020 2020 2020 2020 7467 745f              tgt_
-00013ec0: 6374 785b 2764 625f 6e61 6d65 275d 2c20  ctx['db_name'], 
-00013ed0: 7467 745f 6374 785b 276c 6f67 6669 6c65  tgt_ctx['logfile
-00013ee0: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
-00013ef0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00013f00: 756c 6573 3d62 6164 5f6d 6f64 756c 6573  ules=bad_modules
-00013f10: 290a 2020 2020 656c 6966 2074 6774 5f63  ).    elif tgt_c
-00013f20: 7478 5b27 6f70 745f 7361 6665 275d 2061  tx['opt_safe'] a
-00013f30: 6e64 206e 6f74 2073 7263 5f63 7478 5b27  nd not src_ctx['
-00013f40: 6472 795f 7275 6e27 5d3a 0a20 2020 2020  dry_run']:.     
-00013f50: 2020 2072 756e 5f6f 646f 6f5f 616c 6c74     run_odoo_allt
-00013f60: 6573 7428 7467 745f 6374 785b 2774 6774  est(tgt_ctx['tgt
-00013f70: 5f76 6964 275d 2c20 7467 745f 6374 785b  _vid'], tgt_ctx[
-00013f80: 2763 6f6e 665f 666e 275d 2c0a 2020 2020  'conf_fn'],.    
-00013f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fa0: 2020 2020 2074 6774 5f63 7478 5b27 6462       tgt_ctx['db
-00013fb0: 5f6e 616d 6527 5d2c 2074 6774 5f63 7478  _name'], tgt_ctx
-00013fc0: 5b27 6c6f 6766 696c 6527 5d29 0a20 2020  ['logfile']).   
-00013fd0: 2062 6164 5f6d 6f64 756c 6573 203d 2067   bad_modules = g
-00013fe0: 6574 5f77 726f 6e67 5f6d 6f64 756c 6573  et_wrong_modules
-00013ff0: 2874 6774 5f63 7478 290a 2020 2020 6966  (tgt_ctx).    if
-00014000: 2062 6164 5f6d 6f64 756c 6573 3a0a 2020   bad_modules:.  
-00014010: 2020 2020 2020 6f73 302e 776c 6f67 2827        os0.wlog('
-00014020: 2a2a 2a20 556e 7374 6162 6c65 2044 4220  *** Unstable DB 
-00014030: 6166 7465 7220 636c 6561 6e3a 2077 726f  after clean: wro
-00014040: 6e67 206d 6f64 756c 6520 7374 6174 6520  ng module state 
-00014050: 2573 202a 2a2a 2720 250a 2020 2020 2020  %s ***' %.      
-00014060: 2020 2020 2020 2020 2020 2062 6164 5f6d             bad_m
-00014070: 6f64 756c 6573 290a 2020 2020 2020 2020  odules).        
-00014080: 6861 7264 5f75 6e69 6e73 7461 6c6c 5f6c  hard_uninstall_l
-00014090: 6973 7420 3d20 6c69 7374 280a 2020 2020  ist = list(.    
-000140a0: 2020 2020 2020 2020 7365 7428 6261 645f          set(bad_
-000140b0: 6d6f 6475 6c65 7329 2026 2073 6574 284d  modules) & set(M
-000140c0: 4f44 554c 4553 5f32 5f4c 4541 5645 5f42  ODULES_2_LEAVE_B
-000140d0: 4548 494e 4429 290a 2020 2020 2020 2020  EHIND)).        
-000140e0: 6261 645f 6d6f 6475 6c65 7320 3d20 6c69  bad_modules = li
-000140f0: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
-00014100: 7365 7428 6261 645f 6d6f 6475 6c65 7329  set(bad_modules)
-00014110: 202d 2073 6574 284d 4f44 554c 4553 5f32   - set(MODULES_2
-00014120: 5f4c 4541 5645 5f42 4548 494e 4429 290a  _LEAVE_BEHIND)).
-00014130: 2020 2020 2020 2020 6966 2062 6164 5f6d          if bad_m
-00014140: 6f64 756c 6573 3a0a 2020 2020 2020 2020  odules:.        
-00014150: 2020 2020 7365 745f 756e 696e 7374 616c      set_uninstal
-00014160: 6c65 645f 6279 5f73 716c 2874 6774 5f63  led_by_sql(tgt_c
-00014170: 7478 2c20 6261 645f 6d6f 6475 6c65 7329  tx, bad_modules)
-00014180: 0a20 2020 2020 2020 2069 6620 6861 7264  .        if hard
-00014190: 5f75 6e69 6e73 7461 6c6c 5f6c 6973 743a  _uninstall_list:
-000141a0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000141b0: 206d 6f64 756c 6520 696e 2068 6172 645f   module in hard_
-000141c0: 756e 696e 7374 616c 6c5f 6c69 7374 3a0a  uninstall_list:.
-000141d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141e0: 6f73 302e 776c 6f67 2827 2020 2b2b 2048  os0.wlog('  ++ H
-000141f0: 6172 6420 756e 696e 7374 616c 6c3a 2025  ard uninstall: %
-00014200: 7327 2025 206d 6f64 756c 6529 0a20 2020  s' % module).   
-00014210: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00014220: 6e6f 7420 7372 635f 6374 785b 2764 7279  not src_ctx['dry
-00014230: 5f72 756e 275d 3a0a 2020 2020 2020 2020  _run']:.        
-00014240: 2020 2020 2020 2020 2020 2020 6861 7264              hard
-00014250: 5f63 6c65 616e 5f6d 6f64 756c 6528 7467  _clean_module(tg
-00014260: 745f 6374 782c 206d 6f64 756c 6529 0a0a  t_ctx, module)..
-00014270: 2020 2020 6966 206e 6f74 2073 7263 5f63      if not src_c
-00014280: 7478 5b27 6472 795f 7275 6e27 5d3a 0a20  tx['dry_run']:. 
-00014290: 2020 2020 2020 206f 7330 2e77 6c6f 6728         os0.wlog(
-000142a0: 2754 6573 7420 636f 6e6e 6563 7469 6f6e  'Test connection
-000142b0: 2074 6f20 7461 7267 6574 2064 6220 2573   to target db %s
-000142c0: 2720 2520 7467 745f 6374 785b 2764 625f  ' % tgt_ctx['db_
-000142d0: 6e61 6d65 275d 290a 2020 2020 2020 2020  name']).        
-000142e0: 7569 642c 2074 6774 5f63 7478 203d 2063  uid, tgt_ctx = c
-000142f0: 6c6f 646f 6f2e 6f65 7270 5f73 6574 5f65  lodoo.oerp_set_e
-00014300: 6e76 280a 2020 2020 2020 2020 2020 2020  nv(.            
-00014310: 6374 783d 7467 745f 6374 782c 2063 6f6e  ctx=tgt_ctx, con
-00014320: 666e 3d74 6774 5f66 756c 6c5f 6c63 6f6e  fn=tgt_full_lcon
-00014330: 662c 2064 623d 7467 745f 6374 785b 2764  f, db=tgt_ctx['d
-00014340: 625f 6e61 6d65 275d 290a 2020 2020 2020  b_name']).      
-00014350: 2020 2320 4649 5820 6f65 7270 5f73 6574    # FIX oerp_set
-00014360: 5f65 6e76 2063 6861 6e67 6520 6472 795f  _env change dry_
-00014370: 7275 6e0a 2020 2020 2020 2020 7372 635f  run.        src_
-00014380: 6374 785b 2764 7279 5f72 756e 275d 203d  ctx['dry_run'] =
-00014390: 2074 6774 5f63 7478 5b27 6472 795f 7275   tgt_ctx['dry_ru
-000143a0: 6e27 5d0a 0a20 2020 2072 6574 7572 6e20  n']..    return 
-000143b0: 7467 745f 6675 6c6c 5f6c 636f 6e66 0a0a  tgt_full_lconf..
-000143c0: 0a64 6566 206d 6967 7261 7465 5f64 6174  .def migrate_dat
-000143d0: 6162 6173 655f 7061 7373 2873 7263 5f63  abase_pass(src_c
-000143e0: 7478 2c20 7467 745f 6374 782c 2070 6861  tx, tgt_ctx, pha
-000143f0: 7365 3d4e 6f6e 6529 3a0a 2020 2020 7068  se=None):.    ph
-00014400: 6173 6520 3d20 7068 6173 6520 6f72 2032  ase = phase or 2
-00014410: 0a20 2020 2064 6973 6162 6c65 5f76 656e  .    disable_ven
-00014420: 7620 3d20 4661 6c73 650a 2020 2020 6966  v = False.    if
-00014430: 2070 6861 7365 203d 3d20 313a 0a20 2020   phase == 1:.   
-00014440: 2020 2020 2073 6176 6564 5f64 7279 5f72       saved_dry_r
-00014450: 756e 203d 2073 7263 5f63 7478 5b27 6472  un = src_ctx['dr
-00014460: 795f 7275 6e27 5d0a 2020 2020 2020 2020  y_run'].        
-00014470: 7372 635f 6374 785b 2764 7279 5f72 756e  src_ctx['dry_run
-00014480: 275d 203d 2054 7275 650a 2020 2020 2020  '] = True.      
-00014490: 2020 7467 745f 6374 785b 2764 7279 5f72    tgt_ctx['dry_r
-000144a0: 756e 275d 203d 2073 7263 5f63 7478 5b27  un'] = src_ctx['
-000144b0: 6472 795f 7275 6e27 5d0a 2020 2020 7768  dry_run'].    wh
-000144c0: 696c 6520 313a 0a20 2020 2020 2020 206f  ile 1:.        o
-000144d0: 7330 2e77 6c6f 6728 272d 2720 2a20 3830  s0.wlog('-' * 80
-000144e0: 290a 2020 2020 2020 2020 7372 635f 6374  ).        src_ct
-000144f0: 782c 2074 6774 5f63 7478 2c20 7372 635f  x, tgt_ctx, src_
-00014500: 636f 6e66 6967 2c20 7467 745f 636f 6e66  config, tgt_conf
-00014510: 6967 203d 2061 646a 7573 745f 6374 7828  ig = adjust_ctx(
-00014520: 7372 635f 6374 782c 2074 6774 5f63 7478  src_ctx, tgt_ctx
-00014530: 290a 2020 2020 2020 2020 666f 7220 7061  ).        for pa
-00014540: 7261 6d20 696e 2028 2776 6964 272c 2027  ram in ('vid', '
-00014550: 6f64 6f6f 5f66 7665 7227 2c20 276f 646f  odoo_fver', 'odo
-00014560: 6f5f 7665 7227 293a 0a20 2020 2020 2020  o_ver'):.       
-00014570: 2020 2020 206f 7330 2e77 6c6f 6728 2750       os0.wlog('P
-00014580: 6173 7320 2564 206d 6967 7261 7469 6f6e  ass %d migration
-00014590: 3a20 2573 2066 726f 6d20 2573 2074 6f20  : %s from %s to 
-000145a0: 2573 202e 2e27 2025 0a20 2020 2020 2020  %s ..' %.       
-000145b0: 2020 2020 2020 2020 2020 2870 6861 7365            (phase
-000145c0: 2c20 7061 7261 6d2c 0a20 2020 2020 2020  , param,.       
-000145d0: 2020 2020 2020 2020 2020 2073 7263 5f63             src_c
-000145e0: 7478 5b27 7372 635f 2573 2720 2520 7061  tx['src_%s' % pa
-000145f0: 7261 6d5d 2c20 7467 745f 6374 785b 2774  ram], tgt_ctx['t
-00014600: 6774 5f25 7327 2025 2070 6172 616d 5d29  gt_%s' % param])
-00014610: 290a 2020 2020 2020 2020 666f 7220 7061  ).        for pa
-00014620: 7261 6d20 696e 2028 2764 625f 6e61 6d65  ram in ('db_name
-00014630: 272c 2027 636f 6e66 5f66 6e27 2c20 2778  ', 'conf_fn', 'x
-00014640: 6d6c 7270 635f 706f 7274 272c 2027 6462  mlrpc_port', 'db
-00014650: 5f75 7365 7227 293a 0a20 2020 2020 2020  _user'):.       
-00014660: 2020 2020 206f 7330 2e77 6c6f 6728 2750       os0.wlog('P
-00014670: 6173 7320 2564 206d 6967 7261 7469 6f6e  ass %d migration
-00014680: 3a20 2573 2066 726f 6d20 2573 2074 6f20  : %s from %s to 
-00014690: 2573 202e 2e27 2025 0a20 2020 2020 2020  %s ..' %.       
-000146a0: 2020 2020 2020 2020 2020 2870 6861 7365            (phase
-000146b0: 2c20 7061 7261 6d2c 2073 7263 5f63 7478  , param, src_ctx
-000146c0: 5b70 6172 616d 5d2c 2074 6774 5f63 7478  [param], tgt_ctx
-000146d0: 5b70 6172 616d 5d29 290a 2020 2020 2020  [param])).      
-000146e0: 2020 6966 2070 6861 7365 203d 3d20 313a    if phase == 1:
-000146f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00014700: 6e6f 7420 6f73 2e70 6174 682e 6973 6469  not os.path.isdi
-00014710: 7228 7467 745f 6374 785b 2776 656e 765f  r(tgt_ctx['venv_
-00014720: 6f75 7061 7468 275d 293a 0a20 2020 2020  oupath']):.     
-00014730: 2020 2020 2020 2020 2020 206f 7330 2e77             os0.w
-00014740: 6c6f 6728 2744 6972 6563 746f 7279 2025  log('Directory %
-00014750: 7320 6e6f 7420 666f 756e 6421 2720 2520  s not found!' % 
-00014760: 7467 745f 6374 785b 2776 656e 765f 6f75  tgt_ctx['venv_ou
-00014770: 7061 7468 275d 290a 2020 2020 2020 2020  path']).        
-00014780: 2020 2020 2020 2020 6469 7361 626c 655f          disable_
-00014790: 7665 6e76 203d 2054 7275 650a 2020 2020  venv = True.    
-000147a0: 2020 2020 656c 6966 206e 6f74 2073 7263      elif not src
-000147b0: 5f63 7478 5b27 6472 795f 7275 6e27 5d3a  _ctx['dry_run']:
-000147c0: 0a20 2020 2020 2020 2020 2020 2064 726f  .            dro
-000147d0: 705f 6462 2873 7263 5f63 7478 2c20 7467  p_db(src_ctx, tg
-000147e0: 745f 6374 782c 2074 6774 5f63 7478 5b27  t_ctx, tgt_ctx['
-000147f0: 6462 5f6e 616d 6527 5d2c 0a20 2020 2020  db_name'],.     
-00014800: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00014810: 6577 5f64 626e 616d 6528 7372 635f 6374  ew_dbname(src_ct
-00014820: 785b 2764 625f 6e61 6d65 275d 2c0a 2020  x['db_name'],.  
-00014830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014840: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
-00014850: 5f63 7478 5b27 7467 745f 6f64 6f6f 5f76  _ctx['tgt_odoo_v
-00014860: 6572 275d 2c0a 2020 2020 2020 2020 2020  er'],.          
-00014870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014880: 2020 2020 2074 6774 5f63 7478 5b27 6f63       tgt_ctx['oc
-00014890: 615f 6d69 6772 6174 6527 5d29 290a 2020  a_migrate'])).  
-000148a0: 2020 2020 2020 6675 6c6c 5f6c 636f 6e66        full_lconf
-000148b0: 203d 206d 6967 7261 7465 5f6f 646f 6f28   = migrate_odoo(
-000148c0: 7372 635f 6374 782c 2074 6774 5f63 7478  src_ctx, tgt_ctx
-000148d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000148e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148f0: 2020 2020 7372 635f 636f 6e66 6967 2c20      src_config, 
-00014900: 7467 745f 636f 6e66 6967 2c20 7068 6173  tgt_config, phas
-00014910: 653d 7068 6173 6529 0a20 2020 2020 2020  e=phase).       
-00014920: 2069 6620 7467 745f 6374 785b 2774 6774   if tgt_ctx['tgt
-00014930: 5f6f 646f 6f5f 7665 7227 5d20 3e3d 2073  _odoo_ver'] >= s
-00014940: 7263 5f63 7478 5b27 6669 6e61 6c5f 7665  rc_ctx['final_ve
-00014950: 7227 5d3a 0a20 2020 2020 2020 2020 2020  r']:.           
-00014960: 2069 6620 6469 7361 626c 655f 7665 6e76   if disable_venv
-00014970: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014980: 2020 7372 635f 6374 785b 2776 656e 765f    src_ctx['venv_
-00014990: 6f75 7061 7468 275d 203d 2073 7263 5f63  oupath'] = src_c
-000149a0: 7478 5b27 6f70 745f 6f75 7061 7468 275d  tx['opt_oupath']
-000149b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000149c0: 2074 6774 5f63 7478 5b27 7665 6e76 5f6f   tgt_ctx['venv_o
-000149d0: 7570 6174 6827 5d20 3d20 7372 635f 6374  upath'] = src_ct
-000149e0: 785b 2776 656e 765f 6f75 7061 7468 275d  x['venv_oupath']
-000149f0: 0a20 2020 2020 2020 2020 2020 2062 7265  .            bre
-00014a00: 616b 0a20 2020 2020 2020 2069 6620 6e6f  ak.        if no
-00014a10: 7420 7372 635f 6374 785b 276e 6f5f 7665  t src_ctx['no_ve
-00014a20: 6e76 275d 2061 6e64 206e 6f74 2073 7263  nv'] and not src
-00014a30: 5f63 7478 5b27 6472 795f 7275 6e27 5d3a  _ctx['dry_run']:
-00014a40: 0a20 2020 2020 2020 2020 2020 2076 656e  .            ven
-00014a50: 765f 7061 7468 203d 206f 732e 7061 7468  v_path = os.path
-00014a60: 2e6a 6f69 6e28 7467 745f 6374 785b 2776  .join(tgt_ctx['v
-00014a70: 656e 765f 6f75 7061 7468 275d 2c20 276f  env_oupath'], 'o
-00014a80: 7065 6e75 7067 7261 6465 2729 0a20 2020  penupgrade').   
-00014a90: 2020 2020 2020 2020 2023 2054 4f44 4f0a           # TODO.
-00014aa0: 2020 2020 2020 2020 2020 2020 2320 6966              # if
-00014ab0: 206e 6f74 206f 732e 7061 7468 2e69 7364   not os.path.isd
-00014ac0: 6972 2876 656e 765f 7061 7468 293a 0a20  ir(venv_path):. 
-00014ad0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-00014ae0: 6f73 2e75 6e6c 696e 6b28 6f73 2e70 6174  os.unlink(os.pat
-00014af0: 682e 6a6f 696e 2876 656e 765f 7061 7468  h.join(venv_path
-00014b00: 2c20 6f75 5f76 6572 5f70 6174 6829 290a  , ou_ver_path)).
-00014b10: 2020 2020 2020 2020 7372 635f 6374 782c          src_ctx,
-00014b20: 2074 6774 5f63 7478 203d 2073 6869 6674   tgt_ctx = shift
-00014b30: 5f63 7478 2873 7263 5f63 7478 2c20 7467  _ctx(src_ctx, tg
-00014b40: 745f 6374 782c 2070 6861 7365 3d70 6861  t_ctx, phase=pha
-00014b50: 7365 290a 0a20 2020 2069 6620 7068 6173  se)..    if phas
-00014b60: 6520 3d3d 2031 3a0a 2020 2020 2020 2020  e == 1:.        
-00014b70: 7372 635f 6374 785b 2764 7279 5f72 756e  src_ctx['dry_run
-00014b80: 275d 203d 2073 6176 6564 5f64 7279 5f72  '] = saved_dry_r
-00014b90: 756e 0a20 2020 2020 2020 2074 6774 5f63  un.        tgt_c
-00014ba0: 7478 5b27 6472 795f 7275 6e27 5d20 3d20  tx['dry_run'] = 
-00014bb0: 7372 635f 6374 785b 2764 7279 5f72 756e  src_ctx['dry_run
-00014bc0: 275d 0a0a 0a64 6566 206d 6967 7261 7465  ']...def migrate
-00014bd0: 5f64 6174 6162 6173 6528 7372 635f 6374  _database(src_ct
-00014be0: 782c 2074 6774 5f63 7478 293a 0a20 2020  x, tgt_ctx):.   
-00014bf0: 2069 6620 7372 635f 6374 785b 2770 6861   if src_ctx['pha
-00014c00: 7365 5f31 275d 3a0a 2020 2020 2020 2020  se_1']:.        
-00014c10: 7372 635f 6374 7820 3d20 696e 6974 5f63  src_ctx = init_c
-00014c20: 7478 2873 7263 5f63 7478 290a 2020 2020  tx(src_ctx).    
-00014c30: 2020 2020 6d69 6772 6174 655f 6461 7461      migrate_data
-00014c40: 6261 7365 5f70 6173 7328 7372 635f 6374  base_pass(src_ct
-00014c50: 782c 2074 6774 5f63 7478 2c20 7068 6173  x, tgt_ctx, phas
-00014c60: 653d 3129 0a20 2020 2020 2020 2066 6f72  e=1).        for
-00014c70: 206e 6d20 696e 2028 276f 7269 6769 6e61   nm in ('origina
-00014c80: 6c5f 6d6f 6475 6c65 5f6c 6973 7427 2c29  l_module_list',)
-00014c90: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-00014ca0: 6c20 7372 635f 6374 785b 6e6d 5d0a 2020  l src_ctx[nm].  
-00014cb0: 2020 7372 635f 6374 7820 3d20 696e 6974    src_ctx = init
-00014cc0: 5f63 7478 2873 7263 5f63 7478 290a 2020  _ctx(src_ctx).  
-00014cd0: 2020 6d69 6772 6174 655f 6461 7461 6261    migrate_databa
-00014ce0: 7365 5f70 6173 7328 7372 635f 6374 782c  se_pass(src_ctx,
-00014cf0: 2074 6774 5f63 7478 2c20 7068 6173 653d   tgt_ctx, phase=
-00014d00: 3229 0a20 2020 2070 7269 6e74 2827 4461  2).    print('Da
-00014d10: 7461 6261 7365 2025 7320 7375 6363 6573  tabase %s succes
-00014d20: 7366 756c 6c79 206d 696f 6772 6174 6564  sfully miograted
-00014d30: 2069 6e74 6f20 2573 2720 2520 280a 2020   into %s' % (.  
-00014d40: 2020 2020 2020 7372 635f 6374 785b 2766        src_ctx['f
-00014d50: 726f 6d5f 6462 6e61 6d65 275d 2c20 7467  rom_dbname'], tg
-00014d60: 745f 6374 785b 2764 625f 6e61 6d65 275d  t_ctx['db_name']
-00014d70: 2929 0a0a 0a64 6566 2070 6172 7365 5f63  ))...def parse_c
-00014d80: 7478 2873 7263 5f63 7478 293a 0a20 2020  tx(src_ctx):.   
-00014d90: 2067 6c6f 6261 6c20 4445 465f 434f 4e46   global DEF_CONF
-00014da0: 0a20 2020 2069 6620 6e6f 7420 7372 635f  .    if not src_
-00014db0: 6374 785b 2766 726f 6d5f 6272 616e 6368  ctx['from_branch
-00014dc0: 275d 2061 6e64 206e 6f74 2073 7263 5f63  '] and not src_c
-00014dd0: 7478 5b27 6672 6f6d 5f63 6f6e 666e 275d  tx['from_confn']
-00014de0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00014df0: 4b65 7945 7272 6f72 2827 4d69 7373 6564  KeyError('Missed
-00014e00: 206f 7269 6769 6e61 6c20 6f64 6f6f 2076   original odoo v
-00014e10: 6572 7369 6f6e 2120 506c 6561 7365 2075  ersion! Please u
-00014e20: 7365 202d 4620 7377 6974 6368 2729 0a20  se -F switch'). 
-00014e30: 2020 2065 6c69 6620 7372 635f 6374 785b     elif src_ctx[
-00014e40: 2766 726f 6d5f 6272 616e 6368 275d 3a0a  'from_branch']:.
-00014e50: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-00014e60: 2773 7263 5f6f 646f 6f5f 6676 6572 275d  'src_odoo_fver']
-00014e70: 203d 2063 6c6f 646f 6f2e 6275 696c 645f   = clodoo.build_
-00014e80: 6f64 6f6f 5f70 6172 616d 280a 2020 2020  odoo_param(.    
-00014e90: 2020 2020 2020 2020 2746 554c 4c56 4552          'FULLVER
-00014ea0: 272c 206f 646f 6f5f 7669 643d 7372 635f  ', odoo_vid=src_
-00014eb0: 6374 785b 2766 726f 6d5f 6272 616e 6368  ctx['from_branch
-00014ec0: 275d 2c20 6d75 6c74 693d 5472 7565 290a  '], multi=True).
-00014ed0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00014ee0: 7263 5f63 7478 5b27 6672 6f6d 5f63 6f6e  rc_ctx['from_con
-00014ef0: 666e 275d 3a0a 2020 2020 2020 2020 2020  fn']:.          
-00014f00: 2020 7372 635f 6374 785b 2766 726f 6d5f    src_ctx['from_
-00014f10: 636f 6e66 6e27 5d20 3d20 636c 6f64 6f6f  confn'] = clodoo
-00014f20: 2e62 7569 6c64 5f6f 646f 6f5f 7061 7261  .build_odoo_para
-00014f30: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
-00014f40: 2020 2027 434f 4e46 4e27 2c20 6f64 6f6f     'CONFN', odoo
-00014f50: 5f76 6964 3d73 7263 5f63 7478 5b27 6672  _vid=src_ctx['fr
-00014f60: 6f6d 5f62 7261 6e63 6827 5d2c 206d 756c  om_branch'], mul
-00014f70: 7469 3d54 7275 6529 0a20 2020 2069 6620  ti=True).    if 
-00014f80: 6e6f 7420 6f73 2e70 6174 682e 6973 6669  not os.path.isfi
-00014f90: 6c65 2873 7263 5f63 7478 5b27 6672 6f6d  le(src_ctx['from
-00014fa0: 5f63 6f6e 666e 275d 293a 0a20 2020 2020  _confn']):.     
-00014fb0: 2020 2072 6169 7365 2049 4f45 7272 6f72     raise IOError
-00014fc0: 2827 4669 6c65 2025 7320 6e6f 7420 666f  ('File %s not fo
-00014fd0: 756e 6427 2025 2073 7263 5f63 7478 5b27  und' % src_ctx['
-00014fe0: 6672 6f6d 5f63 6f6e 666e 275d 290a 2020  from_confn']).  
-00014ff0: 2020 6966 206e 6f74 2073 7263 5f63 7478    if not src_ctx
-00015000: 5b27 6672 6f6d 5f62 7261 6e63 6827 5d3a  ['from_branch']:
-00015010: 0a20 2020 2020 2020 2073 7263 5f63 6f6e  .        src_con
-00015020: 6669 6720 3d20 436f 6e66 6967 5061 7273  fig = ConfigPars
-00015030: 6572 2e53 6166 6543 6f6e 6669 6750 6172  er.SafeConfigPar
-00015040: 7365 7228 290a 2020 2020 2020 2020 7372  ser().        sr
-00015050: 635f 636f 6e66 6967 2e72 6561 6428 7372  c_config.read(sr
-00015060: 635f 6374 785b 2766 726f 6d5f 636f 6e66  c_ctx['from_conf
-00015070: 6e27 5d29 0a20 2020 2020 2020 2073 7263  n']).        src
-00015080: 5f63 7478 5b27 7372 635f 6f64 6f6f 5f66  _ctx['src_odoo_f
-00015090: 7665 7227 5d20 3d20 7372 635f 636f 6e66  ver'] = src_conf
-000150a0: 6967 2e67 6574 2827 6f70 7469 6f6e 7327  ig.get('options'
-000150b0: 2c20 276f 655f 7665 7273 696f 6e27 290a  , 'oe_version').
-000150c0: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-000150d0: 2766 726f 6d5f 6272 616e 6368 275d 203d  'from_branch'] =
-000150e0: 2073 7263 5f63 7478 5b27 7372 635f 6f64   src_ctx['src_od
-000150f0: 6f6f 5f66 7665 7227 5d0a 2020 2020 7372  oo_fver'].    sr
-00015100: 635f 6374 785b 2773 7263 5f6f 646f 6f5f  c_ctx['src_odoo_
-00015110: 7665 7227 5d20 3d20 636c 6f64 6f6f 2e62  ver'] = clodoo.b
-00015120: 7569 6c64 5f6f 646f 6f5f 7061 7261 6d28  uild_odoo_param(
-00015130: 0a20 2020 2020 2020 2020 2020 2027 4d41  .            'MA
-00015140: 4a56 4552 272c 206f 646f 6f5f 7669 643d  JVER', odoo_vid=
-00015150: 7372 635f 6374 785b 2766 726f 6d5f 6272  src_ctx['from_br
-00015160: 616e 6368 275d 2c20 6d75 6c74 693d 5472  anch'], multi=Tr
-00015170: 7565 290a 0a20 2020 2069 6620 6e6f 7420  ue)..    if not 
-00015180: 7372 635f 6374 785b 2766 696e 616c 5f62  src_ctx['final_b
-00015190: 7261 6e63 6827 5d20 616e 6420 6e6f 7420  ranch'] and not 
-000151a0: 7372 635f 6374 785b 2766 696e 616c 5f63  src_ctx['final_c
-000151b0: 6f6e 666e 275d 3a0a 2020 2020 2020 2020  onfn']:.        
-000151c0: 7261 6973 6520 4b65 7945 7272 6f72 2827  raise KeyError('
-000151d0: 4d69 7373 6564 2066 696e 616c 206f 646f  Missed final odo
-000151e0: 6f20 7665 7273 696f 6e21 2050 6c65 6173  o version! Pleas
-000151f0: 6520 7573 6520 2d62 2073 7769 7463 6827  e use -b switch'
-00015200: 290a 2020 2020 656c 6966 2073 7263 5f63  ).    elif src_c
-00015210: 7478 5b27 6669 6e61 6c5f 6272 616e 6368  tx['final_branch
-00015220: 275d 3a0a 2020 2020 2020 2020 7372 635f  ']:.        src_
-00015230: 6374 785b 2774 6774 5f6f 646f 6f5f 6676  ctx['tgt_odoo_fv
-00015240: 6572 275d 203d 2063 6c6f 646f 6f2e 6275  er'] = clodoo.bu
-00015250: 696c 645f 6f64 6f6f 5f70 6172 616d 280a  ild_odoo_param(.
-00015260: 2020 2020 2020 2020 2020 2020 2746 554c              'FUL
-00015270: 4c56 4552 272c 206f 646f 6f5f 7669 643d  LVER', odoo_vid=
-00015280: 7372 635f 6374 785b 2766 696e 616c 5f62  src_ctx['final_b
-00015290: 7261 6e63 6827 5d2c 206d 756c 7469 3d54  ranch'], multi=T
-000152a0: 7275 6529 0a20 2020 2020 2020 2069 6620  rue).        if 
-000152b0: 6e6f 7420 7372 635f 6374 785b 2766 696e  not src_ctx['fin
-000152c0: 616c 5f63 6f6e 666e 275d 3a0a 2020 2020  al_confn']:.    
-000152d0: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-000152e0: 2766 696e 616c 5f63 6f6e 666e 275d 203d  'final_confn'] =
-000152f0: 2063 6c6f 646f 6f2e 6275 696c 645f 6f64   clodoo.build_od
-00015300: 6f6f 5f70 6172 616d 280a 2020 2020 2020  oo_param(.      
-00015310: 2020 2020 2020 2020 2020 2743 4f4e 464e            'CONFN
-00015320: 272c 206f 646f 6f5f 7669 643d 7372 635f  ', odoo_vid=src_
-00015330: 6374 785b 2766 696e 616c 5f62 7261 6e63  ctx['final_branc
-00015340: 6827 5d2c 206d 756c 7469 3d54 7275 6529  h'], multi=True)
-00015350: 0a20 2020 2069 6620 6e6f 7420 6f73 2e70  .    if not os.p
-00015360: 6174 682e 6973 6669 6c65 2873 7263 5f63  ath.isfile(src_c
-00015370: 7478 5b27 6669 6e61 6c5f 636f 6e66 6e27  tx['final_confn'
-00015380: 5d29 3a0a 2020 2020 2020 2020 7261 6973  ]):.        rais
-00015390: 6520 494f 4572 726f 7228 2746 696c 6520  e IOError('File 
-000153a0: 2573 206e 6f74 2066 6f75 6e64 2720 2520  %s not found' % 
-000153b0: 7372 635f 6374 785b 2766 696e 616c 5f63  src_ctx['final_c
-000153c0: 6f6e 666e 275d 290a 2020 2020 6966 206e  onfn']).    if n
-000153d0: 6f74 2073 7263 5f63 7478 5b27 6669 6e61  ot src_ctx['fina
-000153e0: 6c5f 6272 616e 6368 275d 3a0a 2020 2020  l_branch']:.    
-000153f0: 2020 2020 7467 745f 636f 6e66 6967 203d      tgt_config =
-00015400: 2043 6f6e 6669 6750 6172 7365 722e 5361   ConfigParser.Sa
-00015410: 6665 436f 6e66 6967 5061 7273 6572 2829  feConfigParser()
-00015420: 0a20 2020 2020 2020 2074 6774 5f63 6f6e  .        tgt_con
-00015430: 6669 672e 7265 6164 2873 7263 5f63 7478  fig.read(src_ctx
-00015440: 5b27 6669 6e61 6c5f 636f 6e66 6e27 5d29  ['final_confn'])
-00015450: 0a20 2020 2020 2020 2073 7263 5f63 7478  .        src_ctx
-00015460: 5b27 7467 745f 6f64 6f6f 5f66 7665 7227  ['tgt_odoo_fver'
-00015470: 5d20 3d20 7467 745f 636f 6e66 6967 2e67  ] = tgt_config.g
-00015480: 6574 2827 6f70 7469 6f6e 7327 2c20 276f  et('options', 'o
-00015490: 655f 7665 7273 696f 6e27 290a 2020 2020  e_version').    
-000154a0: 2020 2020 7372 635f 6374 785b 2766 696e      src_ctx['fin
-000154b0: 616c 5f62 7261 6e63 6827 5d20 3d20 7372  al_branch'] = sr
-000154c0: 635f 6374 785b 2774 6774 5f6f 646f 6f5f  c_ctx['tgt_odoo_
-000154d0: 6676 6572 275d 0a20 2020 2073 7263 5f63  fver'].    src_c
-000154e0: 7478 5b27 7467 745f 6f64 6f6f 5f76 6572  tx['tgt_odoo_ver
-000154f0: 275d 203d 2063 6c6f 646f 6f2e 6275 696c  '] = clodoo.buil
-00015500: 645f 6f64 6f6f 5f70 6172 616d 280a 2020  d_odoo_param(.  
-00015510: 2020 2020 2020 2020 2020 274d 414a 5645            'MAJVE
-00015520: 5227 2c20 6f64 6f6f 5f76 6964 3d73 7263  R', odoo_vid=src
-00015530: 5f63 7478 5b27 6669 6e61 6c5f 6272 616e  _ctx['final_bran
-00015540: 6368 275d 2c20 6d75 6c74 693d 5472 7565  ch'], multi=True
-00015550: 290a 0a20 2020 2069 6620 2828 7372 635f  )..    if ((src_
-00015560: 6374 785b 2773 7263 5f6f 646f 6f5f 7665  ctx['src_odoo_ve
-00015570: 7227 5d20 3e3d 2073 7263 5f63 7478 5b27  r'] >= src_ctx['
-00015580: 7467 745f 6f64 6f6f 5f76 6572 275d 2061  tgt_odoo_ver'] a
-00015590: 6e64 0a20 2020 2020 2020 2020 2020 206e  nd.            n
-000155a0: 6f74 2073 7263 5f63 7478 5b27 7365 6c5f  ot src_ctx['sel_
-000155b0: 6d6f 6465 6c27 5d29 206f 720a 2020 2020  model']) or.    
-000155c0: 2020 2020 2873 7263 5f63 7478 5b27 7372      (src_ctx['sr
-000155d0: 635f 6f64 6f6f 5f76 6572 275d 203e 2073  c_odoo_ver'] > s
-000155e0: 7263 5f63 7478 5b27 7467 745f 6f64 6f6f  rc_ctx['tgt_odoo
-000155f0: 5f76 6572 275d 2061 6e64 0a20 2020 2020  _ver'] and.     
-00015600: 2020 2020 2020 2073 7263 5f63 7478 5b27         src_ctx['
-00015610: 7365 6c5f 6d6f 6465 6c27 5d29 293a 0a20  sel_model'])):. 
-00015620: 2020 2020 2020 2072 6169 7365 204b 6579         raise Key
-00015630: 4572 726f 7228 2746 696e 616c 2076 6572  Error('Final ver
-00015640: 7369 6f6e 206d 7573 7420 6265 2067 7265  sion must be gre
-00015650: 6174 6572 2074 6861 6e20 6f72 6967 696e  ater than origin
-00015660: 616c 2076 6572 7369 6f6e 2729 0a0a 2020  al version')..  
-00015670: 2020 6966 206e 6f74 2073 7263 5f63 7478    if not src_ctx
-00015680: 5b27 6f70 745f 6f75 7061 7468 275d 3a0a  ['opt_oupath']:.
-00015690: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-000156a0: 276f 7074 5f6f 7570 6174 6827 5d20 3d20  'opt_oupath'] = 
-000156b0: 6f73 2e70 6174 682e 6a6f 696e 286f 732e  os.path.join(os.
-000156c0: 7061 7468 2e65 7870 616e 6475 7365 7228  path.expanduser(
-000156d0: 277e 2729 2c20 2774 6d70 2729 0a20 2020  '~'), 'tmp').   
-000156e0: 2069 6620 6e6f 7420 7372 635f 6374 785b   if not src_ctx[
-000156f0: 276f 7074 5f6f 756c 7061 7468 275d 3a0a  'opt_oulpath']:.
-00015700: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-00015710: 276f 7074 5f6f 756c 7061 7468 275d 203d  'opt_oulpath'] =
-00015720: 206f 732e 7061 7468 2e6a 6f69 6e28 7372   os.path.join(sr
-00015730: 635f 6374 785b 276f 7074 5f6f 7570 6174  c_ctx['opt_oupat
-00015740: 6827 5d2c 0a20 2020 2020 2020 2020 2020  h'],.           
-00015750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015770: 2020 2027 6f70 656e 7570 6772 6164 656c     'openupgradel
-00015780: 6962 2729 0a0a 2020 2020 6966 2073 7263  ib')..    if src
-00015790: 5f63 7478 5b27 6669 6e61 6c5f 6462 6e61  _ctx['final_dbna
-000157a0: 6d65 275d 2061 6e64 206e 6f74 2073 7263  me'] and not src
-000157b0: 5f63 7478 5b27 6672 6f6d 5f64 626e 616d  _ctx['from_dbnam
-000157c0: 6527 5d3a 0a20 2020 2020 2020 2073 7263  e']:.        src
-000157d0: 5f63 7478 5b27 6672 6f6d 5f64 626e 616d  _ctx['from_dbnam
-000157e0: 6527 5d2c 2073 7263 5f63 7478 5b27 6669  e'], src_ctx['fi
-000157f0: 6e61 6c5f 6462 6e61 6d65 275d 203d 205c  nal_dbname'] = \
-00015800: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
-00015810: 5f63 7478 5b27 6669 6e61 6c5f 6462 6e61  _ctx['final_dbna
-00015820: 6d65 275d 2c20 2725 735f 3230 3231 2720  me'], '%s_2021' 
-00015830: 2520 7372 635f 6374 785b 2766 696e 616c  % src_ctx['final
-00015840: 5f64 626e 616d 6527 5d0a 2020 2020 656c  _dbname'].    el
-00015850: 6966 206e 6f74 2073 7263 5f63 7478 5b27  if not src_ctx['
-00015860: 6669 6e61 6c5f 6462 6e61 6d65 275d 2061  final_dbname'] a
-00015870: 6e64 2073 7263 5f63 7478 5b27 6672 6f6d  nd src_ctx['from
-00015880: 5f64 626e 616d 6527 5d3a 0a20 2020 2020  _dbname']:.     
-00015890: 2020 2073 7263 5f63 7478 5b27 6669 6e61     src_ctx['fina
-000158a0: 6c5f 6462 6e61 6d65 275d 203d 2027 2573  l_dbname'] = '%s
-000158b0: 5f32 3032 3127 2025 2073 7263 5f63 7478  _2021' % src_ctx
-000158c0: 5b27 6672 6f6d 5f64 626e 616d 6527 5d0a  ['from_dbname'].
-000158d0: 2020 2020 656c 6966 206e 6f74 2073 7263      elif not src
-000158e0: 5f63 7478 5b27 6669 6e61 6c5f 6462 6e61  _ctx['final_dbna
-000158f0: 6d65 275d 2061 6e64 206e 6f74 2073 7263  me'] and not src
-00015900: 5f63 7478 5b27 6672 6f6d 5f64 626e 616d  _ctx['from_dbnam
-00015910: 6527 5d3a 0a20 2020 2020 2020 2072 6169  e']:.        rai
-00015920: 7365 204b 6579 4572 726f 7228 274d 6973  se KeyError('Mis
-00015930: 7365 6420 6461 7461 6261 7365 2074 6f20  sed database to 
-00015940: 7570 6772 6164 6521 2050 6c65 6173 6520  upgrade! Please 
-00015950: 7573 6520 2d64 2073 7769 7463 6827 290a  use -d switch').
-00015960: 0a20 2020 2069 6620 6e6f 7420 7372 635f  .    if not src_
-00015970: 6374 785b 276c 6f67 666e 275d 3a0a 2020  ctx['logfn']:.  
-00015980: 2020 2020 2020 6966 2073 7263 5f63 7478        if src_ctx
-00015990: 5b27 6f63 615f 6d69 6772 6174 6527 5d3a  ['oca_migrate']:
-000159a0: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
-000159b0: 5f63 7478 5b27 6c6f 6766 6e27 5d20 3d20  _ctx['logfn'] = 
-000159c0: 6f73 2e70 6174 682e 6a6f 696e 2873 7263  os.path.join(src
-000159d0: 5f63 7478 5b27 6f70 745f 6f75 7061 7468  _ctx['opt_oupath
-000159e0: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
-000159f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a10: 276d 6967 7261 7465 5f62 795f 6f70 656e  'migrate_by_open
-00015a20: 7570 6772 6164 652e 6c6f 6727 290a 2020  upgrade.log').  
-00015a30: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00015a40: 2020 2020 2020 2020 7372 635f 6374 785b          src_ctx[
-00015a50: 276c 6f67 666e 275d 203d 206f 732e 7061  'logfn'] = os.pa
-00015a60: 7468 2e6a 6f69 6e28 7372 635f 6374 785b  th.join(src_ctx[
-00015a70: 276f 7074 5f6f 7570 6174 6827 5d2c 0a20  'opt_oupath'],. 
-00015a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015aa0: 2020 2020 2020 2020 2020 2027 6d69 6772             'migr
-00015ab0: 6174 655f 6f64 6f6f 5f64 622e 6c6f 6727  ate_odoo_db.log'
-00015ac0: 290a 2020 2020 7372 635f 6374 785b 276c  ).    src_ctx['l
-00015ad0: 6f67 6669 6c65 275d 203d 206f 732e 7061  ogfile'] = os.pa
-00015ae0: 7468 2e6a 6f69 6e28 7372 635f 6374 785b  th.join(src_ctx[
-00015af0: 276f 7074 5f6f 7570 6174 6827 5d2c 0a20  'opt_oupath'],. 
-00015b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b20: 2020 2020 2027 6d69 6772 6174 655f 6f64       'migrate_od
-00015b30: 6f6f 5f64 622d 7365 7276 6572 2e6c 6f67  oo_db-server.log
-00015b40: 2729 0a20 2020 2073 7263 5f63 7478 5b27  ').    src_ctx['
-00015b50: 6669 6e61 6c5f 7665 7227 5d20 3d20 7372  final_ver'] = sr
-00015b60: 635f 6374 785b 2774 6774 5f6f 646f 6f5f  c_ctx['tgt_odoo_
-00015b70: 7665 7227 5d0a 2020 2020 7467 745f 6374  ver'].    tgt_ct
-00015b80: 7820 3d20 7372 635f 6374 782e 636f 7079  x = src_ctx.copy
-00015b90: 2829 0a20 2020 2044 4546 5f43 4f4e 4620  ().    DEF_CONF 
-00015ba0: 3d20 636c 6f64 6f6f 2e64 6566 6175 6c74  = clodoo.default
-00015bb0: 5f63 6f6e 6628 7372 635f 6374 7829 0a20  _conf(src_ctx). 
-00015bc0: 2020 2072 6574 7572 6e20 7372 635f 6374     return src_ct
-00015bd0: 782c 2074 6774 5f63 7478 0a0a 0a5f 4445  x, tgt_ctx..._DE
-00015be0: 5052 4543 4154 4544 5f4d 4f44 554c 4553  PRECATED_MODULES
-00015bf0: 203d 205b 0a20 2020 2028 2261 6363 6f75   = [.    ("accou
-00015c00: 6e74 5f61 6e61 6c79 7469 635f 616e 616c  nt_analytic_anal
-00015c10: 7973 6973 222c 2022 6f63 615f 6d6f 7665  ysis", "oca_move
-00015c20: 6422 2c20 2263 6f6e 7472 6163 7422 2c0a  d", "contract",.
-00015c30: 2020 2020 2020 2020 224d 6f76 6564 2074          "Moved t
-00015c40: 6f20 4f43 412f 636f 6e74 7261 6374 2229  o OCA/contract")
-00015c50: 2c0a 2020 2020 2822 6163 636f 756e 745f  ,.    ("account_
-00015c60: 616e 616c 7974 6963 5f70 6c61 6e73 222c  analytic_plans",
-00015c70: 2022 6f63 615f 6d6f 7665 6422 2c20 2261   "oca_moved", "a
-00015c80: 6363 6f75 6e74 5f61 6e61 6c79 7469 635f  ccount_analytic_
-00015c90: 6469 7374 7269 6275 7469 6f6e 222c 0a20  distribution",. 
-00015ca0: 2020 2020 2020 2022 4d6f 7665 6420 746f         "Moved to
-00015cb0: 204f 4341 2f61 6363 6f75 6e74 5f61 6e61   OCA/account_ana
-00015cc0: 6c79 7469 6322 292c 0a20 2020 2028 2261  lytic"),.    ("a
-00015cd0: 6363 6f75 6e74 5f61 6e67 6c6f 5f73 6178  ccount_anglo_sax
-00015ce0: 6f6e 222c 2022 7265 6d6f 7665 6422 292c  on", "removed"),
-00015cf0: 0a20 2020 2028 2261 6363 6f75 6e74 5f62  .    ("account_b
-00015d00: 616e 6b5f 7374 6174 656d 656e 745f 6578  ank_statement_ex
-00015d10: 7465 6e73 696f 6e73 222c 2022 7265 6d6f  tensions", "remo
-00015d20: 7665 6422 292c 0a20 2020 2028 2261 6363  ved"),.    ("acc
-00015d30: 6f75 6e74 5f63 6861 7274 222c 2022 6d65  ount_chart", "me
-00015d40: 7267 6564 222c 2022 6163 636f 756e 7422  rged", "account"
-00015d50: 292c 0a20 2020 2028 2261 6363 6f75 6e74  ),.    ("account
-00015d60: 5f63 6865 636b 5f77 7269 7469 6e67 222c  _check_writing",
-00015d70: 2022 7265 6e61 6d65 6422 2c20 2261 6363   "renamed", "acc
-00015d80: 6f75 6e74 5f63 6865 636b 5f70 7269 6e74  ount_check_print
-00015d90: 696e 6722 292c 0a20 2020 2028 2261 6363  ing"),.    ("acc
-00015da0: 6f75 6e74 5f66 6f6c 6c6f 7775 7022 2c20  ount_followup", 
-00015db0: 2272 656d 6f76 6564 2229 2c0a 2020 2020  "removed"),.    
-00015dc0: 2822 6163 636f 756e 745f 7061 796d 656e  ("account_paymen
-00015dd0: 7422 2c20 226f 6361 5f6d 6f76 6564 222c  t", "oca_moved",
-00015de0: 2022 6163 636f 756e 745f 7061 796d 656e   "account_paymen
-00015df0: 745f 6f72 6465 7222 2c0a 2020 2020 2020  t_order",.      
-00015e00: 2020 224d 6f76 6564 2074 6f20 4f43 412f    "Moved to OCA/
-00015e10: 6261 6e6b 2d70 6179 6d65 6e74 2229 2c0a  bank-payment"),.
-00015e20: 2020 2020 2822 6163 636f 756e 745f 7365      ("account_se
-00015e30: 7175 656e 6365 222c 2022 7265 6d6f 7665  quence", "remove
-00015e40: 6422 292c 0a20 2020 2028 2261 6e61 6c79  d"),.    ("analy
-00015e50: 7469 635f 636f 6e74 7261 6374 5f68 725f  tic_contract_hr_
-00015e60: 6578 7065 6e73 6522 2c20 2272 656d 6f76  expense", "remov
-00015e70: 6564 2229 2c0a 2020 2020 2822 616e 616c  ed"),.    ("anal
-00015e80: 7974 6963 5f75 7365 725f 6675 6e63 7469  ytic_user_functi
-00015e90: 6f6e 222c 2022 7265 6d6f 7665 6422 292c  on", "removed"),
-00015ea0: 0a20 2020 2028 2261 6e67 6c6f 5f73 6178  .    ("anglo_sax
-00015eb0: 6f6e 5f64 726f 7073 6869 7070 696e 6722  on_dropshipping"
-00015ec0: 2c20 2272 656d 6f76 6564 2229 2c0a 2020  , "removed"),.  
-00015ed0: 2020 2822 6175 7468 5f6f 7065 6e69 6422    ("auth_openid"
-00015ee0: 2c20 2272 656d 6f76 6564 2229 2c0a 2020  , "removed"),.  
-00015ef0: 2020 2822 6261 7365 5f72 6570 6f72 745f    ("base_report_
-00015f00: 6465 7369 676e 6572 222c 2022 7265 6d6f  designer", "remo
-00015f10: 7665 6422 292c 0a20 2020 2028 2263 6f6e  ved"),.    ("con
-00015f20: 7461 6374 7322 2c20 226d 6572 6765 6422  tacts", "merged"
-00015f30: 2c20 226d 6169 6c22 292c 0a20 2020 2028  , "mail"),.    (
-00015f40: 2263 726d 5f68 656c 7064 6573 6b22 2c20  "crm_helpdesk", 
-00015f50: 2272 656d 6f76 6564 2229 2c0a 2020 2020  "removed"),.    
-00015f60: 2822 6372 6d5f 6d61 7373 5f6d 6169 6c69  ("crm_mass_maili
-00015f70: 6e67 222c 2022 7265 6d6f 7665 6422 292c  ng", "removed"),
-00015f80: 0a20 2020 2028 2263 726d 5f70 726f 6669  .    ("crm_profi
-00015f90: 6c69 6e67 222c 2022 7265 6d6f 7665 6422  ling", "removed"
-00015fa0: 292c 0a20 2020 2028 2265 6469 222c 2022  ),.    ("edi", "
-00015fb0: 7265 6d6f 7665 6422 292c 0a20 2020 2028  removed"),.    (
-00015fc0: 2265 6d61 696c 5f74 656d 706c 6174 6522  "email_template"
-00015fd0: 2c20 226d 6572 6765 6422 2c20 226d 6169  , "merged", "mai
-00015fe0: 6c5f 7465 6d70 6c61 7465 2229 2c0a 2020  l_template"),.  
-00015ff0: 2020 2822 6872 5f61 7070 6c69 6361 6e74    ("hr_applicant
-00016000: 5f64 6f63 756d 656e 7422 2c20 2272 656d  _document", "rem
-00016010: 6f76 6564 2229 2c0a 2020 2020 2822 6872  oved"),.    ("hr
-00016020: 5f74 696d 6573 6865 6574 5f69 6e76 6f69  _timesheet_invoi
-00016030: 6365 222c 2022 7265 6d6f 7665 6422 292c  ce", "removed"),
-00016040: 0a20 2020 2028 2269 6d5f 6368 6174 222c  .    ("im_chat",
-00016050: 2022 6d65 7267 6564 222c 2022 6d61 696c   "merged", "mail
-00016060: 2229 2c0a 2020 2020 2822 6b6e 6f77 6c65  "),.    ("knowle
-00016070: 6467 6522 2c20 226f 6361 5f6d 6f76 6564  dge", "oca_moved
-00016080: 222c 2022 6b6e 6f77 6c65 6467 6522 2c20  ", "knowledge", 
-00016090: 224d 6f76 6564 2074 6f20 4f43 412f 6b6e  "Moved to OCA/kn
-000160a0: 6f77 6c65 6467 6522 292c 0a20 2020 2028  owledge"),.    (
-000160b0: 226c 3130 6e5f 6265 5f63 6f64 6122 2c20  "l10n_be_coda", 
-000160c0: 2272 656d 6f76 6564 2229 2c0a 2020 2020  "removed"),.    
-000160d0: 2822 6c31 306e 5f66 725f 7269 6222 2c20  ("l10n_fr_rib", 
-000160e0: 2272 656d 6f76 6564 2229 2c0a 2020 2020  "removed"),.    
-000160f0: 2822 6d61 726b 6574 696e 675f 6372 6d22  ("marketing_crm"
-00016100: 2c20 226d 6572 6765 6422 2c20 2263 726d  , "merged", "crm
-00016110: 2229 2c0a 2020 2020 2822 6d75 6c74 695f  "),.    ("multi_
-00016120: 636f 6d70 616e 7922 2c20 2272 656d 6f76  company", "remov
-00016130: 6564 2229 2c0a 2020 2020 2822 706f 7274  ed"),.    ("port
-00016140: 616c 5f63 6c61 696d 222c 2022 7265 6e61  al_claim", "rena
-00016150: 6d65 6422 2c20 2277 6562 7369 7465 5f63  med", "website_c
-00016160: 726d 5f63 6c61 696d 2229 2c0a 2020 2020  rm_claim"),.    
-00016170: 2822 706f 7274 616c 5f70 726f 6a65 6374  ("portal_project
-00016180: 222c 2022 6d65 7267 6564 222c 2022 7072  ", "merged", "pr
-00016190: 6f6a 6563 7422 292c 0a20 2020 2028 2270  oject"),.    ("p
-000161a0: 6f72 7461 6c5f 7072 6f6a 6563 745f 6973  ortal_project_is
-000161b0: 7375 6522 2c20 226d 6572 6765 6422 2c20  sue", "merged", 
-000161c0: 2270 726f 6a65 6374 5f69 7373 7565 2229  "project_issue")
-000161d0: 2c0a 2020 2020 2822 7072 6f63 7572 656d  ,.    ("procurem
-000161e0: 656e 745f 6a69 745f 7374 6f63 6b22 2c20  ent_jit_stock", 
-000161f0: 226d 6572 6765 6422 2c20 2270 726f 6375  "merged", "procu
-00016200: 7265 6d65 6e74 5f6a 6974 2229 2c0a 2020  rement_jit"),.  
-00016210: 2020 2822 7075 7263 6861 7365 5f61 6e61    ("purchase_ana
-00016220: 6c79 7469 635f 706c 616e 7322 2c20 226f  lytic_plans", "o
-00016230: 6361 5f6d 6f76 6564 222c 2022 7075 7263  ca_moved", "purc
-00016240: 6861 7365 5f61 6e61 6c79 7469 635f 6469  hase_analytic_di
-00016250: 7374 7269 6275 7469 6f6e 222c 0a20 2020  stribution",.   
-00016260: 2020 2020 2022 4d6f 7665 6420 746f 204f       "Moved to O
-00016270: 4341 2f61 6363 6f75 6e74 2d61 6e61 6c79  CA/account-analy
-00016280: 7469 6322 292c 0a20 2020 2028 2270 7572  tic"),.    ("pur
-00016290: 6368 6173 655f 646f 7562 6c65 5f76 616c  chase_double_val
-000162a0: 6964 6174 696f 6e22 2c20 2272 656d 6f76  idation", "remov
-000162b0: 6564 2229 2c0a 2020 2020 2822 7361 6c65  ed"),.    ("sale
-000162c0: 5f61 6e61 6c79 7469 635f 706c 616e 7322  _analytic_plans"
-000162d0: 2c20 226f 6361 5f6d 6f76 6564 222c 2022  , "oca_moved", "
-000162e0: 7361 6c65 5f61 6e61 6c79 7469 635f 6469  sale_analytic_di
-000162f0: 7374 7269 6275 7469 6f6e 222c 0a20 2020  stribution",.   
-00016300: 2020 2020 2022 4d6f 7665 6420 746f 204f       "Moved to O
-00016310: 4341 2f61 6363 6f75 6e74 2d61 6e61 6c79  CA/account-analy
-00016320: 7469 6322 292c 0a20 2020 2028 2273 616c  tic"),.    ("sal
-00016330: 655f 6a6f 7572 6e61 6c22 2c20 2272 656d  e_journal", "rem
-00016340: 6f76 6564 2229 2c0a 2020 2020 2822 7368  oved"),.    ("sh
-00016350: 6172 6522 2c20 2272 656d 6f76 6564 2229  are", "removed")
-00016360: 2c0a 2020 2020 2822 7374 6f63 6b5f 696e  ,.    ("stock_in
-00016370: 766f 6963 655f 6469 7265 6374 6c79 222c  voice_directly",
-00016380: 2022 7265 6d6f 7665 6422 292c 0a20 2020   "removed"),.   
-00016390: 2028 2277 6562 5f61 7069 222c 2022 7265   ("web_api", "re
-000163a0: 6d6f 7665 6422 292c 0a20 2020 2028 2277  moved"),.    ("w
-000163b0: 6562 5f67 616e 7474 222c 2022 6d65 7267  eb_gantt", "merg
-000163c0: 6564 222c 2022 7765 6222 292c 0a20 2020  ed", "web"),.   
-000163d0: 2028 2277 6562 5f67 7261 7068 222c 2022   ("web_graph", "
-000163e0: 6d65 7267 6564 222c 2022 7765 6222 292c  merged", "web"),
-000163f0: 0a20 2020 2028 2277 6562 5f6b 616e 6261  .    ("web_kanba
-00016400: 6e5f 7370 6172 6b6c 696e 6522 2c20 226d  n_sparkline", "m
-00016410: 6572 6765 6422 2c20 2277 6562 2229 2c0a  erged", "web"),.
-00016420: 2020 2020 2822 7765 625f 7465 7374 7322      ("web_tests"
-00016430: 2c20 226d 6572 6765 6422 2c20 2277 6562  , "merged", "web
-00016440: 2229 2c0a 2020 2020 2822 7765 625f 7465  "),.    ("web_te
-00016450: 7374 735f 6465 6d6f 222c 2022 7265 6d6f  sts_demo", "remo
-00016460: 7665 6422 292c 0a20 2020 2028 2277 6562  ved"),.    ("web
-00016470: 7369 7465 5f63 6572 7469 6669 6361 7469  site_certificati
-00016480: 6f6e 222c 2022 7265 6d6f 7665 6422 292c  on", "removed"),
-00016490: 0a20 2020 2028 2277 6562 7369 7465 5f69  .    ("website_i
-000164a0: 6e73 7461 6e74 636c 6963 6b22 2c20 2272  nstantclick", "r
-000164b0: 656d 6f76 6564 2229 2c0a 2020 2020 2822  emoved"),.    ("
-000164c0: 7765 6273 6974 655f 6d61 696c 5f67 726f  website_mail_gro
-000164d0: 7570 222c 2022 7265 6e61 6d65 6422 2c20  up", "renamed", 
-000164e0: 2277 6562 7369 7465 5f6d 6169 6c5f 6368  "website_mail_ch
-000164f0: 616e 6e65 6c22 292c 0a20 2020 2028 2277  annel"),.    ("w
-00016500: 6562 7369 7465 5f72 6570 6f72 7422 2c20  ebsite_report", 
-00016510: 226d 6572 6765 6422 2c20 2272 6570 6f72  "merged", "repor
-00016520: 7422 292c 0a5d 0a0a 6966 205f 5f6e 616d  t"),.]..if __nam
-00016530: 655f 5f20 3d3d 2022 5f5f 6d61 696e 5f5f  e__ == "__main__
-00016540: 223a 0a20 2020 2070 6172 7365 7220 3d20  ":.    parser = 
-00016550: 7a30 6c69 622e 7061 7273 656f 7074 6172  z0lib.parseoptar
-00016560: 6773 2822 4d69 6772 6174 6520 4f64 6f6f  gs("Migrate Odoo
-00016570: 2044 4222 2c0a 2020 2020 2020 2020 2020   DB",.          
-00016580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016590: 2020 2020 2020 22c2 a920 3230 3139 2d32        ".. 2019-2
-000165a0: 3120 6279 2053 4853 2d41 5620 732e 722e  1 by SHS-AV s.r.
-000165b0: 6c2e 222c 0a20 2020 2020 2020 2020 2020  l.",.           
-000165c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000165d0: 2020 2020 2076 6572 7369 6f6e 3d5f 5f76       version=__v
-000165e0: 6572 7369 6f6e 5f5f 290a 2020 2020 7061  ersion__).    pa
-000165f0: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
-00016600: 7428 272d 6827 290a 2020 2020 7061 7273  t('-h').    pars
-00016610: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-00016620: 222d 4222 2c20 222d 2d6f 7065 6e75 7067  "-B", "--openupg
-00016630: 7261 6465 2d62 7261 6e63 682d 7061 7468  rade-branch-path
-00016640: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00016650: 2020 2020 2020 2020 2020 2068 656c 703d             help=
-00016660: 226f 7065 6e75 7067 7261 6465 2062 7261  "openupgrade bra
-00016670: 6e63 6820 7061 7468 222c 0a20 2020 2020  nch path",.     
-00016680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016690: 2020 2064 6573 743d 226f 7074 5f6f 7570     dest="opt_oup
-000166a0: 6174 6822 2c0a 2020 2020 2020 2020 2020  ath",.          
-000166b0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-000166c0: 7461 7661 723d 2270 6174 6822 290a 2020  tavar="path").  
-000166d0: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-000166e0: 756d 656e 7428 272d 6227 2c20 272d 2d62  ument('-b', '--b
-000166f0: 7261 6e63 6827 2c0a 2020 2020 2020 2020  ranch',.        
-00016700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016710: 6163 7469 6f6e 3d27 7374 6f72 6527 2c0a  action='store',.
-00016720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016730: 2020 2020 2020 2020 6465 7374 3d27 6669          dest='fi
-00016740: 6e61 6c5f 6272 616e 6368 272c 0a20 2020  nal_branch',.   
-00016750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016760: 2020 2020 206d 6574 6176 6172 3d27 7665       metavar='ve
-00016770: 7273 696f 6e27 290a 2020 2020 7061 7273  rsion').    pars
-00016780: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-00016790: 222d 4322 2c20 222d 2d62 792d 636f 6d70  "-C", "--by-comp
-000167a0: 616e 7922 2c0a 2020 2020 2020 2020 2020  any",.          
-000167b0: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-000167c0: 7469 6f6e 3d22 7374 6f72 655f 7472 7565  tion="store_true
-000167d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000167e0: 2020 2020 2020 2020 2020 2068 656c 703d             help=
-000167f0: 2273 656c 6563 7420 6f6e 6c79 2072 6563  "select only rec
-00016800: 6f72 6473 206f 6620 6d61 696e 2063 6f6d  ords of main com
-00016810: 7061 6e79 222c 0a20 2020 2020 2020 2020  pany",.         
-00016820: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00016830: 6573 743d 2262 795f 636f 6d70 616e 7922  est="by_company"
-00016840: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
-00016850: 5f61 7267 756d 656e 7428 222d 6322 2c20  _argument("-c", 
-00016860: 222d 2d74 6774 2d63 6f6e 6669 6722 2c0a  "--tgt-config",.
-00016870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016880: 2020 2020 2020 2020 6865 6c70 3d22 7461          help="ta
-00016890: 7267 6574 2044 4220 636f 6e66 6967 7572  rget DB configur
-000168a0: 6174 696f 6e20 6669 6c65 222c 0a20 2020  ation file",.   
-000168b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168c0: 2020 2020 2064 6573 743d 2266 696e 616c       dest="final
-000168d0: 5f63 6f6e 666e 222c 0a20 2020 2020 2020  _confn",.       
-000168e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168f0: 206d 6574 6176 6172 3d22 6669 6c65 2229   metavar="file")
-00016900: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
-00016910: 6172 6775 6d65 6e74 2822 2d44 222c 2022  argument("-D", "
-00016920: 2d2d 6465 6c2d 6462 2d69 662d 6578 6973  --del-db-if-exis
-00016930: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00016940: 2020 2020 2020 2020 2020 2020 6163 7469              acti
-00016950: 6f6e 3d22 7374 6f72 655f 7472 7565 222c  on="store_true",
-00016960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016970: 2020 2020 2020 2020 2064 6573 743d 226f           dest="o
-00016980: 7074 5f64 656c 2229 0a20 2020 2070 6172  pt_del").    par
-00016990: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
-000169a0: 2822 2d64 222c 2022 2d2d 7467 742d 6462  ("-d", "--tgt-db
-000169b0: 5f6e 616d 6522 2c0a 2020 2020 2020 2020  _name",.        
-000169c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169d0: 6865 6c70 3d22 7461 7267 6574 2064 6174  help="target dat
-000169e0: 6162 6173 6520 6e61 6d65 222c 0a20 2020  abase name",.   
-000169f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a00: 2020 2020 2064 6573 743d 2266 696e 616c       dest="final
-00016a10: 5f64 626e 616d 6522 2c0a 2020 2020 2020  _dbname",.      
-00016a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a30: 2020 6d65 7461 7661 723d 226e 616d 6522    metavar="name"
-00016a40: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
-00016a50: 5f61 7267 756d 656e 7428 222d 4522 2c20  _argument("-E", 
-00016a60: 222d 2d6e 6f2d 7665 6e76 222c 0a20 2020  "--no-venv",.   
-00016a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a80: 2020 2020 2068 656c 703d 2264 6973 6162       help="disab
-00016a90: 6c65 2076 6972 7475 616c 656e 7622 2c0a  le virtualenv",.
-00016aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ab0: 2020 2020 2020 2020 6163 7469 6f6e 3d27          action='
-00016ac0: 7374 6f72 655f 7472 7565 272c 0a20 2020  store_true',.   
-00016ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ae0: 2020 2020 2064 6573 743d 226e 6f5f 7665       dest="no_ve
-00016af0: 6e76 2229 0a20 2020 2070 6172 7365 722e  nv").    parser.
-00016b00: 6164 645f 6172 6775 6d65 6e74 2827 2d46  add_argument('-F
-00016b10: 272c 2027 2d2d 6672 6f6d 2d6f 646f 6f2d  ', '--from-odoo-
-00016b20: 7665 7227 2c0a 2020 2020 2020 2020 2020  ver',.          
-00016b30: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-00016b40: 7469 6f6e 3d27 7374 6f72 6527 2c0a 2020  tion='store',.  
-00016b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b60: 2020 2020 2020 6465 7374 3d27 6672 6f6d        dest='from
-00016b70: 5f62 7261 6e63 6827 2c0a 2020 2020 2020  _branch',.      
-00016b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b90: 2020 6d65 7461 7661 723d 2276 6572 2229    metavar="ver")
-00016ba0: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
-00016bb0: 6172 6775 6d65 6e74 2822 2d49 222c 2022  argument("-I", "
-00016bc0: 2d2d 696d 6167 6522 2c0a 2020 2020 2020  --image",.      
-00016bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016be0: 2020 6865 6c70 3d22 696d 6167 6520 6d6f    help="image mo
-00016bf0: 6465 222c 0a20 2020 2020 2020 2020 2020  de",.           
-00016c00: 2020 2020 2020 2020 2020 2020 2061 6374               act
-00016c10: 696f 6e3d 2773 746f 7265 5f74 7275 6527  ion='store_true'
-00016c20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00016c30: 2020 2020 2020 2020 2020 6465 7374 3d22            dest="
-00016c40: 696d 6167 655f 6d6f 6465 222c 0a20 2020  image_mode",.   
-00016c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c60: 2020 2020 2064 6566 6175 6c74 3d46 616c       default=Fal
-00016c70: 7365 290a 2020 2020 7061 7273 6572 2e61  se).    parser.a
-00016c80: 6464 5f61 7267 756d 656e 7428 222d 6922  dd_argument("-i"
-00016c90: 2c20 222d 2d69 6473 222c 0a20 2020 2020  , "--ids",.     
-00016ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016cb0: 2020 2068 656c 703d 2269 6473 2074 6f20     help="ids to 
-00016cc0: 6d69 6772 6174 6522 2c0a 2020 2020 2020  migrate",.      
-00016cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ce0: 2020 6465 7374 3d22 7365 6c5f 6964 7322    dest="sel_ids"
-00016cf0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00016d00: 2020 2020 2020 2020 2020 6d65 7461 7661            metava
-00016d10: 723d 226c 6973 7422 290a 2020 2020 7061  r="list").    pa
-00016d20: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
-00016d30: 7428 222d 4a22 2c20 222d 2d74 7279 2d72  t("-J", "--try-r
-00016d40: 6569 6e73 7461 6c6c 222c 0a20 2020 2020  einstall",.     
-00016d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d60: 2020 2068 656c 703d 2274 7279 2074 6f20     help="try to 
-00016d70: 7265 696e 7374 616c 6c22 2c0a 2020 2020  reinstall",.    
-00016d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d90: 2020 2020 6163 7469 6f6e 3d27 7374 6f72      action='stor
-00016da0: 655f 7472 7565 272c 0a20 2020 2020 2020  e_true',.       
-00016db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016dc0: 2064 6573 743d 2274 7279 5f72 6569 6e73   dest="try_reins
-00016dd0: 7461 6c6c 222c 0a20 2020 2020 2020 2020  tall",.         
-00016de0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00016df0: 6566 6175 6c74 3d46 616c 7365 290a 2020  efault=False).  
-00016e00: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-00016e10: 756d 656e 7428 222d 4b22 2c20 222d 2d63  ument("-K", "--c
-00016e20: 6f6d 6d61 6e64 2d66 696c 6522 2c0a 2020  ommand-file",.  
-00016e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e40: 2020 2020 2020 6865 6c70 3d22 6d69 6772        help="migr
-00016e50: 6174 696f 6e20 636f 6d6d 616e 6420 6669  ation command fi
-00016e60: 6c65 222c 0a20 2020 2020 2020 2020 2020  le",.           
-00016e70: 2020 2020 2020 2020 2020 2020 2064 6573               des
-00016e80: 743d 2263 6f6d 6d61 6e64 5f66 696c 6522  t="command_file"
-00016e90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00016ea0: 2020 2020 2020 2020 2020 6d65 7461 7661            metava
-00016eb0: 723d 2266 696c 6522 2c0a 2020 2020 2020  r="file",.      
-00016ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ed0: 2020 6465 6661 756c 743d 272e 2f6d 6967    default='./mig
-00016ee0: 7261 7465 5f6f 646f 6f2e 6373 7627 290a  rate_odoo.csv').
-00016ef0: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
-00016f00: 7267 756d 656e 7428 222d 6b22 2c20 222d  rgument("-k", "-
-00016f10: 2d64 6566 6175 6c74 2d62 6568 6176 696f  -default-behavio
-00016f20: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
-00016f30: 2020 2020 2020 2020 2020 2020 6865 6c70              help
-00016f40: 3d22 6465 6661 756c 7420 6265 6861 7669  ="default behavi
-00016f50: 6f72 222c 0a20 2020 2020 2020 2020 2020  or",.           
-00016f60: 2020 2020 2020 2020 2020 2020 2061 6374               act
-00016f70: 696f 6e3d 2273 746f 7265 5f74 7275 6522  ion="store_true"
-00016f80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00016f90: 2020 2020 2020 2020 2020 6465 7374 3d22            dest="
-00016fa0: 6465 6661 756c 745f 6265 6861 7669 6f72  default_behavior
-00016fb0: 2229 0a20 2020 2070 6172 7365 722e 6164  ").    parser.ad
-00016fc0: 645f 6172 6775 6d65 6e74 2822 2d6c 222c  d_argument("-l",
-00016fd0: 2022 2d2d 6669 6c65 2d6c 6f67 222c 0a20   "--file-log",. 
-00016fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ff0: 2020 2020 2020 2068 656c 703d 226c 6f67         help="log
-00017000: 2066 696c 6522 2c0a 2020 2020 2020 2020   file",.        
-00017010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017020: 6465 7374 3d22 6c6f 6766 6e22 2c0a 2020  dest="logfn",.  
-00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017040: 2020 2020 2020 6d65 7461 7661 723d 2266        metavar="f
-00017050: 696c 6522 290a 2020 2020 7061 7273 6572  ile").    parser
-00017060: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
-00017070: 4d22 2c20 222d 2d6f 6361 2d6d 6967 7261  M", "--oca-migra
-00017080: 7465 222c 0a20 2020 2020 2020 2020 2020  te",.           
-00017090: 2020 2020 2020 2020 2020 2020 2061 6374               act
-000170a0: 696f 6e3d 2273 746f 7265 5f74 7275 6522  ion="store_true"
-000170b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000170c0: 2020 2020 2020 2020 2020 6465 7374 3d22            dest="
-000170d0: 6f63 615f 6d69 6772 6174 6522 2c0a 2020  oca_migrate",.  
-000170e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170f0: 2020 2020 2020 6865 6c70 3d22 7573 6520        help="use 
-00017100: 4f43 4120 6d69 6772 6174 6520 2866 696e  OCA migrate (fin
-00017110: 616c 2076 6572 7369 6f6e 203c 2031 302e  al version < 10.
-00017120: 3029 2229 0a20 2020 2070 6172 7365 722e  0)").    parser.
-00017130: 6164 645f 6172 6775 6d65 6e74 2822 2d6d  add_argument("-m
-00017140: 222c 2022 2d2d 7365 6c2d 6d6f 6465 6c22  ", "--sel-model"
-00017150: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00017160: 2020 2020 2020 2020 2020 6865 6c70 3d22            help="
-00017170: 6d6f 6465 6c20 746f 206d 6967 7261 7465  model to migrate
-00017180: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00017190: 2020 2020 2020 2020 2020 2064 6573 743d             dest=
-000171a0: 2273 656c 5f6d 6f64 656c 222c 0a20 2020  "sel_model",.   
-000171b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171c0: 2020 2020 206d 6574 6176 6172 3d22 6e61       metavar="na
-000171d0: 6d65 2229 0a20 2020 2070 6172 7365 722e  me").    parser.
-000171e0: 6164 645f 6172 6775 6d65 6e74 2827 2d6e  add_argument('-n
-000171f0: 2729 0a20 2020 2070 6172 7365 722e 6164  ').    parser.ad
-00017200: 645f 6172 6775 6d65 6e74 2822 2d4f 222c  d_argument("-O",
-00017210: 2022 2d2d 6f70 656e 7570 6772 6164 656c   "--openupgradel
-00017220: 6962 2d70 6174 6822 2c0a 2020 2020 2020  ib-path",.      
-00017230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017240: 2020 6865 6c70 3d22 4f70 656e 7570 6772    help="Openupgr
-00017250: 6164 656c 6962 2070 6174 6822 2c0a 2020  adelib path",.  
-00017260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017270: 2020 2020 2020 6465 7374 3d22 6f70 745f        dest="opt_
-00017280: 6f75 6c70 6174 6822 2c0a 2020 2020 2020  oulpath",.      
-00017290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172a0: 2020 6d65 7461 7661 723d 2270 6174 6822    metavar="path"
-000172b0: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
-000172c0: 5f61 7267 756d 656e 7428 272d 7127 290a  _argument('-q').
-000172d0: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
-000172e0: 7267 756d 656e 7428 222d 5222 2c20 222d  rgument("-R", "-
-000172f0: 2d72 6564 7563 7465 642d 6d6f 6475 6c65  -reducted-module
-00017300: 2d73 6574 222c 0a20 2020 2020 2020 2020  -set",.         
-00017310: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00017320: 6374 696f 6e3d 2773 746f 7265 5f74 7275  ction='store_tru
-00017330: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
-00017340: 2020 2020 2020 2020 2020 2020 6465 7374              dest
-00017350: 3d22 7265 6475 6374 6564 5f6d 6f64 756c  ="reducted_modul
-00017360: 655f 7365 7422 2c0a 2020 2020 2020 2020  e_set",.        
-00017370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017380: 6465 6661 756c 743d 4661 6c73 6529 0a20  default=False). 
-00017390: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
-000173a0: 6775 6d65 6e74 2822 2d53 222c 2022 2d2d  gument("-S", "--
-000173b0: 7361 6665 2d6d 6f64 6522 2c0a 2020 2020  safe-mode",.    
-000173c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173d0: 2020 2020 6163 7469 6f6e 3d22 7374 6f72      action="stor
-000173e0: 655f 7472 7565 222c 0a20 2020 2020 2020  e_true",.       
-000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017400: 2064 6573 743d 226f 7074 5f73 6166 6522   dest="opt_safe"
-00017410: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00017420: 2020 2020 2020 2020 2020 6865 6c70 3d22            help="
-00017430: 7361 6665 206d 6f64 6522 290a 2020 2020  safe mode").    
-00017440: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-00017450: 656e 7428 222d 7322 2c20 222d 2d75 7365  ent("-s", "--use
-00017460: 2d73 796e 6368 726f 222c 0a20 2020 2020  -synchro",.     
-00017470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017480: 2020 2068 656c 703d 2275 7365 206d 6f64     help="use mod
-00017490: 756c 6520 7379 6e63 6872 6f22 2c0a 2020  ule synchro",.  
-000174a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174b0: 2020 2020 2020 6163 7469 6f6e 3d27 7374        action='st
-000174c0: 6f72 655f 7472 7565 272c 0a20 2020 2020  ore_true',.     
-000174d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174e0: 2020 2064 6573 743d 2275 7365 5f73 796e     dest="use_syn
-000174f0: 6368 726f 222c 0a20 2020 2020 2020 2020  chro",.         
-00017500: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00017510: 6566 6175 6c74 3d46 616c 7365 290a 2020  efault=False).  
-00017520: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
-00017530: 756d 656e 7428 222d 5422 2c20 222d 2d75  ument("-T", "--u
-00017540: 7064 2d74 7261 6e73 6c61 7469 6f6e 222c  pd-translation",
-00017550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017560: 2020 2020 2020 2020 2061 6374 696f 6e3d           action=
-00017570: 2773 746f 7265 5f74 7275 6527 2c0a 2020  'store_true',.  
-00017580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017590: 2020 2020 2020 6465 7374 3d22 7570 645f        dest="upd_
-000175a0: 7472 616e 736c 6174 696f 6e22 2c0a 2020  translation",.  
-000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175c0: 2020 2020 2020 6465 6661 756c 743d 4661        default=Fa
-000175d0: 6c73 6529 0a20 2020 2070 6172 7365 722e  lse).    parser.
-000175e0: 6164 645f 6172 6775 6d65 6e74 2822 2d55  add_argument("-U
-000175f0: 222c 2022 2d2d 7573 6572 222c 0a20 2020  ", "--user",.   
-00017600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017610: 2020 2020 2068 656c 703d 226c 6f67 696e       help="login
-00017620: 2075 7365 726e 616d 6522 2c0a 2020 2020   username",.    
-00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017640: 2020 2020 6465 7374 3d22 6c67 695f 7573      dest="lgi_us
-00017650: 6572 222c 0a20 2020 2020 2020 2020 2020  er",.           
-00017660: 2020 2020 2020 2020 2020 2020 206d 6574               met
-00017670: 6176 6172 3d22 7573 6572 6e61 6d65 222c  avar="username",
-00017680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017690: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-000176a0: 3d22 6164 6d69 6e22 290a 2020 2020 7061  ="admin").    pa
-000176b0: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
-000176c0: 7428 272d 5627 290a 2020 2020 7061 7273  t('-V').    pars
-000176d0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-000176e0: 272d 7627 290a 2020 2020 7061 7273 6572  '-v').    parser
-000176f0: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
-00017700: 5722 2c20 222d 2d77 6570 2d6c 6f67 222c  W", "--wep-log",
-00017710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017720: 2020 2020 2020 2020 2068 656c 703d 2264           help="d
-00017730: 656c 206c 6f67 7320 6265 666f 7265 206d  el logs before m
-00017740: 6967 7261 7469 6f6e 222c 0a20 2020 2020  igration",.     
-00017750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017760: 2020 2061 6374 696f 6e3d 2773 746f 7265     action='store
-00017770: 5f74 7275 6527 2c0a 2020 2020 2020 2020  _true',.        
-00017780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017790: 6465 7374 3d22 7765 705f 6c6f 6773 222c  dest="wep_logs",
-000177a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000177b0: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-000177c0: 3d46 616c 7365 290a 2020 2020 7061 7273  =False).    pars
-000177d0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
-000177e0: 222d 7722 2c20 222d 2d73 7263 2d63 6f6e  "-w", "--src-con
-000177f0: 6669 6722 2c0a 2020 2020 2020 2020 2020  fig",.          
-00017800: 2020 2020 2020 2020 2020 2020 2020 6865                he
-00017810: 6c70 3d22 736f 7572 6365 2044 4220 636f  lp="source DB co
-00017820: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00017830: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00017840: 2020 2020 2020 2020 2020 2064 6573 743d             dest=
-00017850: 2266 726f 6d5f 636f 6e66 6e22 2c0a 2020  "from_confn",.  
-00017860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017870: 2020 2020 2020 6d65 7461 7661 723d 2266        metavar="f
-00017880: 696c 6522 290a 2020 2020 7061 7273 6572  ile").    parser
-00017890: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
-000178a0: 5922 2c20 222d 2d75 6e69 6e73 7461 6c6c  Y", "--uninstall
-000178b0: 2d6d 6f64 756c 6573 222c 0a20 2020 2020  -modules",.     
-000178c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178d0: 2020 2068 656c 703d 226d 6f64 756c 6573     help="modules
-000178e0: 2074 6f20 756e 696e 7374 616c 6c61 2062   to uninstalla b
-000178f0: 6566 6f72 6520 6d69 6772 6174 696f 6e22  efore migration"
-00017900: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00017910: 2020 2020 2020 2020 2020 6465 7374 3d22            dest="
-00017920: 756e 696e 7374 616c 6c5f 6d6f 6475 6c65  uninstall_module
-00017930: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00017940: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-00017950: 7661 723d 226c 6973 7422 290a 2020 2020  var="list").    
-00017960: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-00017970: 656e 7428 222d 7922 2c20 222d 2d61 7373  ent("-y", "--ass
-00017980: 756d 652d 7965 7322 2c0a 2020 2020 2020  ume-yes",.      
-00017990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179a0: 2020 6865 6c70 3d22 6173 7375 6d65 2079    help="assume y
-000179b0: 6573 222c 0a20 2020 2020 2020 2020 2020  es",.           
-000179c0: 2020 2020 2020 2020 2020 2020 2061 6374               act
-000179d0: 696f 6e3d 2773 746f 7265 5f74 7275 6527  ion='store_true'
-000179e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000179f0: 2020 2020 2020 2020 2020 6465 7374 3d22            dest="
-00017a00: 6173 7375 6d65 5f79 6573 222c 0a20 2020  assume_yes",.   
-00017a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a20: 2020 2020 2064 6566 6175 6c74 3d46 616c       default=Fal
-00017a30: 7365 290a 2020 2020 7061 7273 6572 2e61  se).    parser.a
-00017a40: 6464 5f61 7267 756d 656e 7428 222d 7a22  dd_argument("-z"
-00017a50: 2c20 222d 2d73 7263 2d64 625f 6e61 6d65  , "--src-db_name
-00017a60: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00017a70: 2020 2020 2020 2020 2020 2068 656c 703d             help=
-00017a80: 2273 6f75 7263 6520 6461 7461 6261 7365  "source database
-00017a90: 206e 616d 6522 2c0a 2020 2020 2020 2020   name",.        
-00017aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ab0: 6465 7374 3d22 6672 6f6d 5f64 626e 616d  dest="from_dbnam
-00017ac0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00017ad0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-00017ae0: 7661 723d 226e 616d 6522 290a 2020 2020  var="name").    
-00017af0: 7061 7273 6572 2e61 6464 5f61 7267 756d  parser.add_argum
-00017b00: 656e 7428 222d 3122 2c20 222d 2d64 6f2d  ent("-1", "--do-
-00017b10: 7061 7373 3122 2c0a 2020 2020 2020 2020  pass1",.        
-00017b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b30: 6865 6c70 3d22 6578 6563 2070 6173 7320  help="exec pass 
-00017b40: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
-00017b50: 2020 2020 2020 2020 2020 2020 6163 7469              acti
-00017b60: 6f6e 3d27 7374 6f72 655f 7472 7565 272c  on='store_true',
-00017b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017b80: 2020 2020 2020 2020 2064 6573 743d 2270           dest="p
-00017b90: 6861 7365 5f31 2229 0a0a 2020 2020 7372  hase_1")..    sr
-00017ba0: 635f 6374 7820 3d20 7061 7273 6572 2e70  c_ctx = parser.p
-00017bb0: 6172 7365 6f70 7461 7267 7328 7379 732e  arseoptargs(sys.
-00017bc0: 6172 6776 5b31 3a5d 2c20 6170 706c 795f  argv[1:], apply_
-00017bd0: 636f 6e66 3d46 616c 7365 290a 2020 2020  conf=False).    
-00017be0: 7372 635f 6374 782c 2074 6774 5f63 7478  src_ctx, tgt_ctx
-00017bf0: 203d 2070 6172 7365 5f63 7478 2873 7263   = parse_ctx(src
-00017c00: 5f63 7478 290a 2020 2020 6966 2073 7263  _ctx).    if src
-00017c10: 5f63 7478 5b27 7765 705f 6c6f 6773 275d  _ctx['wep_logs']
-00017c20: 3a0a 2020 2020 2020 2020 7765 705f 6c6f  :.        wep_lo
-00017c30: 6773 2873 7263 5f63 7478 290a 2020 2020  gs(src_ctx).    
-00017c40: 6f73 302e 7365 745f 746c 6f67 5f66 696c  os0.set_tlog_fil
-00017c50: 6528 7372 635f 6374 785b 276c 6f67 666e  e(src_ctx['logfn
-00017c60: 275d 2c20 6563 686f 3d54 7275 6529 0a20  '], echo=True). 
-00017c70: 2020 206f 7330 2e77 6c6f 6728 273d 2720     os0.wlog('=' 
-00017c80: 2a20 3830 290a 2020 2020 6f73 302e 776c  * 80).    os0.wl
-00017c90: 6f67 2822 4d69 6772 6174 696f 6e20 6461  og("Migration da
-00017ca0: 7461 6261 7365 2025 7320 6265 6769 6e6e  tabase %s beginn
-00017cb0: 696e 6720 2e2e 2e22 2c20 5f5f 7665 7273  ing ...", __vers
-00017cc0: 696f 6e5f 5f29 0a20 2020 2069 6620 7372  ion__).    if sr
-00017cd0: 635f 6374 785b 2773 656c 5f6d 6f64 656c  c_ctx['sel_model
-00017ce0: 275d 3a0a 2020 2020 2020 2020 6d69 6772  ']:.        migr
-00017cf0: 6174 655f 7365 6c5f 7461 626c 6573 2873  ate_sel_tables(s
-00017d00: 7263 5f63 7478 2c20 7467 745f 6374 7829  rc_ctx, tgt_ctx)
-00017d10: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00017d20: 2020 206d 6967 7261 7465 5f64 6174 6162     migrate_datab
-00017d30: 6173 6528 7372 635f 6374 782c 2074 6774  ase(src_ctx, tgt
-00017d40: 5f63 7478 290a                           _ctx).
+0000f2f0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000f300: 2020 2020 2069 6620 7467 745f 6374 782e       if tgt_ctx.
+0000f310: 6765 7428 6e6d 293a 0a20 2020 2020 2020  get(nm):.       
+0000f320: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
+0000f330: 5f63 6f6e 6669 672e 7365 7428 276f 7074  _config.set('opt
+0000f340: 696f 6e73 272c 206e 6d2c 2074 6774 5f63  ions', nm, tgt_c
+0000f350: 7478 5b6e 6d5d 290a 2020 2020 2020 2020  tx[nm]).        
+0000f360: 2020 2020 2020 2020 656c 6966 2074 6774          elif tgt
+0000f370: 5f63 6f6e 6669 672e 6861 735f 6f70 7469  _config.has_opti
+0000f380: 6f6e 2827 6f70 7469 6f6e 7327 2c20 6e6d  on('options', nm
+0000f390: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000f3a0: 2020 2020 2020 2074 6774 5f63 7478 5b6e         tgt_ctx[n
+0000f3b0: 6d5d 203d 2074 6774 5f63 6f6e 6669 672e  m] = tgt_config.
+0000f3c0: 6765 7428 276f 7074 696f 6e73 272c 206e  get('options', n
+0000f3d0: 6d29 0a20 2020 2020 2020 2020 2020 2020  m).             
+0000f3e0: 2020 2065 6c69 6620 7372 635f 6374 782e     elif src_ctx.
+0000f3f0: 6765 7428 6e6d 293a 0a20 2020 2020 2020  get(nm):.       
+0000f400: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
+0000f410: 5f63 7478 5b6e 6d5d 203d 2073 7263 5f63  _ctx[nm] = src_c
+0000f420: 7478 5b6e 6d5d 0a20 2020 2020 2020 2020  tx[nm].         
+0000f430: 2020 2020 2020 2020 2020 2074 6774 5f63             tgt_c
+0000f440: 6f6e 6669 672e 7365 7428 276f 7074 696f  onfig.set('optio
+0000f450: 6e73 272c 206e 6d2c 2074 6774 5f63 7478  ns', nm, tgt_ctx
+0000f460: 5b6e 6d5d 290a 2020 2020 2020 2020 656c  [nm]).        el
+0000f470: 6966 2069 7465 6d20 3d3d 2027 7769 7468  if item == 'with
+0000f480: 6f75 745f 6465 6d6f 273a 0a20 2020 2020  out_demo':.     
+0000f490: 2020 2020 2020 2073 7263 5f63 7478 5b69         src_ctx[i
+0000f4a0: 7465 6d5d 203d 2027 5472 7565 270a 2020  tem] = 'True'.  
+0000f4b0: 2020 2020 2020 2020 2020 7372 635f 636f            src_co
+0000f4c0: 6e66 6967 2e73 6574 2827 6f70 7469 6f6e  nfig.set('option
+0000f4d0: 7327 2c20 6974 656d 2c20 7372 635f 6374  s', item, src_ct
+0000f4e0: 785b 6974 656d 5d29 0a20 2020 2020 2020  x[item]).       
+0000f4f0: 2020 2020 2074 6774 5f63 7478 5b69 7465       tgt_ctx[ite
+0000f500: 6d5d 203d 2027 5472 7565 270a 2020 2020  m] = 'True'.    
+0000f510: 2020 2020 2020 2020 7467 745f 636f 6e66          tgt_conf
+0000f520: 6967 2e73 6574 2827 6f70 7469 6f6e 7327  ig.set('options'
+0000f530: 2c20 6974 656d 2c20 7467 745f 6374 785b  , item, tgt_ctx[
+0000f540: 6974 656d 5d29 0a20 2020 2069 6620 7372  item]).    if sr
+0000f550: 635f 6374 785b 276e 6f5f 7665 6e76 275d  c_ctx['no_venv']
+0000f560: 3a0a 2020 2020 2020 2020 7372 635f 6374  :.        src_ct
+0000f570: 785b 2776 656e 765f 6f75 7061 7468 275d  x['venv_oupath']
+0000f580: 203d 2073 7263 5f63 7478 5b27 6f70 745f   = src_ctx['opt_
+0000f590: 6f75 7061 7468 275d 0a20 2020 2065 6c73  oupath'].    els
+0000f5a0: 653a 0a20 2020 2020 2020 2073 7263 5f63  e:.        src_c
+0000f5b0: 7478 5b27 7665 6e76 5f6f 7570 6174 6827  tx['venv_oupath'
+0000f5c0: 5d20 3d20 6f73 2e70 6174 682e 6a6f 696e  ] = os.path.join
+0000f5d0: 280a 2020 2020 2020 2020 2020 2020 6f73  (.            os
+0000f5e0: 2e70 6174 682e 6578 7061 6e64 7573 6572  .path.expanduser
+0000f5f0: 2827 7e27 292c 2027 5645 4e56 2d25 7327  ('~'), 'VENV-%s'
+0000f600: 2025 2074 6774 5f63 7478 5b27 7467 745f   % tgt_ctx['tgt_
+0000f610: 6f64 6f6f 5f66 7665 7227 5d0a 2020 2020  odoo_fver'].    
+0000f620: 2020 2020 290a 2020 2020 7467 745f 6374      ).    tgt_ct
+0000f630: 785b 2776 656e 765f 6f75 7061 7468 275d  x['venv_oupath']
+0000f640: 203d 2073 7263 5f63 7478 5b27 7665 6e76   = src_ctx['venv
+0000f650: 5f6f 7570 6174 6827 5d0a 2020 2020 7265  _oupath'].    re
+0000f660: 7475 726e 2073 7263 5f63 7478 2c20 7467  turn src_ctx, tg
+0000f670: 745f 6374 782c 2073 7263 5f63 6f6e 6669  t_ctx, src_confi
+0000f680: 672c 2074 6774 5f63 6f6e 6669 670a 0a0a  g, tgt_config...
+0000f690: 6465 6620 7368 6966 745f 6374 7828 7372  def shift_ctx(sr
+0000f6a0: 635f 6374 782c 2074 6774 5f63 7478 2c20  c_ctx, tgt_ctx, 
+0000f6b0: 7068 6173 653d 4e6f 6e65 293a 0a20 2020  phase=None):.   
+0000f6c0: 2070 6861 7365 203d 2070 6861 7365 206f   phase = phase o
+0000f6d0: 7220 310a 2020 2020 666f 7220 6974 656d  r 1.    for item
+0000f6e0: 2069 6e20 2827 7669 6427 2c20 276f 646f   in ('vid', 'odo
+0000f6f0: 6f5f 6676 6572 272c 2027 6f64 6f6f 5f76  o_fver', 'odoo_v
+0000f700: 6572 2729 3a0a 2020 2020 2020 2020 7372  er'):.        sr
+0000f710: 635f 6374 785b 2773 7263 5f25 7327 2025  c_ctx['src_%s' %
+0000f720: 2069 7465 6d5d 2c20 7467 745f 6374 785b   item], tgt_ctx[
+0000f730: 2774 6774 5f25 7327 2025 2069 7465 6d5d  'tgt_%s' % item]
+0000f740: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+0000f750: 2074 6774 5f63 7478 5b27 7467 745f 2573   tgt_ctx['tgt_%s
+0000f760: 2720 2520 6974 656d 5d2c 0a20 2020 2020  ' % item],.     
+0000f770: 2020 2020 2020 2046 616c 7365 2c0a 2020         False,.  
+0000f780: 2020 2020 2020 290a 2020 2020 666f 7220        ).    for 
+0000f790: 6974 656d 2069 6e20 2827 6462 5f6e 616d  item in ('db_nam
+0000f7a0: 6527 2c20 2763 6f6e 665f 666e 272c 2027  e', 'conf_fn', '
+0000f7b0: 786d 6c72 7063 5f70 6f72 7427 2c20 2764  xmlrpc_port', 'd
+0000f7c0: 625f 7573 6572 2729 3a0a 2020 2020 2020  b_user'):.      
+0000f7d0: 2020 7372 635f 6374 785b 6974 656d 5d2c    src_ctx[item],
+0000f7e0: 2074 6774 5f63 7478 5b69 7465 6d5d 203d   tgt_ctx[item] =
+0000f7f0: 2074 6774 5f63 7478 5b69 7465 6d5d 2c20   tgt_ctx[item], 
+0000f800: 4661 6c73 650a 2020 2020 666f 7220 6974  False.    for it
+0000f810: 656d 2069 6e20 2827 6462 5f68 6f73 7427  em in ('db_host'
+0000f820: 2c20 276c 6f67 696e 5f75 7365 7227 2c20  , 'login_user', 
+0000f830: 276c 6f67 696e 5f70 6173 7377 6f72 6427  'login_password'
+0000f840: 2c20 2763 7279 7074 5f70 6173 7377 6f72  , 'crypt_passwor
+0000f850: 6427 293a 0a20 2020 2020 2020 2069 6620  d'):.        if 
+0000f860: 7467 745f 6374 782e 6765 7428 6974 656d  tgt_ctx.get(item
+0000f870: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000f880: 7263 5f63 7478 5b69 7465 6d5d 203d 2074  rc_ctx[item] = t
+0000f890: 6774 5f63 7478 5b69 7465 6d5d 0a20 2020  gt_ctx[item].   
+0000f8a0: 2072 6574 7572 6e20 7372 635f 6374 782c   return src_ctx,
+0000f8b0: 2074 6774 5f63 7478 0a0a 0a64 6566 2070   tgt_ctx...def p
+0000f8c0: 7265 7061 7265 5f63 6f6e 6669 675f 6669  repare_config_fi
+0000f8d0: 6c65 2863 7478 2c20 7372 635f 636f 6e66  le(ctx, src_conf
+0000f8e0: 6967 2c20 6f75 5f76 6572 5f70 6174 683d  ig, ou_ver_path=
+0000f8f0: 4e6f 6e65 2c20 7061 7468 733d 4e6f 6e65  None, paths=None
+0000f900: 293a 0a20 2020 2069 6620 6f75 5f76 6572  ):.    if ou_ver
+0000f910: 5f70 6174 683a 0a20 2020 2020 2020 2073  _path:.        s
+0000f920: 7263 5f6c 636f 6e66 203d 2027 6f70 656e  rc_lconf = 'open
+0000f930: 7570 6772 6164 652e 636f 6e66 270a 2020  upgrade.conf'.  
+0000f940: 2020 2020 2020 6675 6c6c 5f6c 636f 6e66        full_lconf
+0000f950: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+0000f960: 6f75 5f76 6572 5f70 6174 682c 2073 7263  ou_ver_path, src
+0000f970: 5f6c 636f 6e66 290a 2020 2020 656c 7365  _lconf).    else
+0000f980: 3a0a 2020 2020 2020 2020 7372 635f 6c63  :.        src_lc
+0000f990: 6f6e 6620 3d20 636c 6f64 6f6f 2e62 7569  onf = clodoo.bui
+0000f9a0: 6c64 5f6f 646f 6f5f 7061 7261 6d28 0a20  ld_odoo_param(. 
+0000f9b0: 2020 2020 2020 2020 2020 2027 4c43 4f4e             'LCON
+0000f9c0: 464e 272c 206f 646f 6f5f 7669 643d 6374  FN', odoo_vid=ct
+0000f9d0: 785b 2773 7263 5f76 6964 275d 2c20 6d75  x['src_vid'], mu
+0000f9e0: 6c74 693d 5472 7565 0a20 2020 2020 2020  lti=True.       
+0000f9f0: 2029 0a20 2020 2020 2020 2066 756c 6c5f   ).        full_
+0000fa00: 6c63 6f6e 6620 3d20 6f73 2e70 6174 682e  lconf = os.path.
+0000fa10: 6a6f 696e 286f 732e 7061 7468 2e65 7870  join(os.path.exp
+0000fa20: 616e 6475 7365 7228 277e 2729 2c20 7372  anduser('~'), sr
+0000fa30: 635f 6c63 6f6e 6629 0a20 2020 2020 2020  c_lconf).       
+0000fa40: 2066 6f72 2066 6e20 696e 2028 272e 6f70   for fn in ('.op
+0000fa50: 656e 6572 705f 7365 7276 6572 7263 272c  enerp_serverrc',
+0000fa60: 2027 2e6f 646f 6f72 6327 293a 0a20 2020   '.odoorc'):.   
+0000fa70: 2020 2020 2020 2020 2074 6d70 5f6c 636f           tmp_lco
+0000fa80: 6e66 203d 206f 732e 7061 7468 2e6a 6f69  nf = os.path.joi
+0000fa90: 6e28 6f73 2e70 6174 682e 6578 7061 6e64  n(os.path.expand
+0000faa0: 7573 6572 2827 7e27 292c 2066 6e29 0a20  user('~'), fn). 
+0000fab0: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
+0000fac0: 2e70 6174 682e 6973 6669 6c65 2874 6d70  .path.isfile(tmp
+0000fad0: 5f6c 636f 6e66 293a 0a20 2020 2020 2020  _lconf):.       
+0000fae0: 2020 2020 2020 2020 206f 732e 7265 6d6f           os.remo
+0000faf0: 7665 2874 6d70 5f6c 636f 6e66 290a 2020  ve(tmp_lconf).  
+0000fb00: 2020 6966 2070 6174 6873 3a0a 2020 2020    if paths:.    
+0000fb10: 2020 2020 7372 635f 636f 6e66 6967 2e73      src_config.s
+0000fb20: 6574 2827 6f70 7469 6f6e 7327 2c20 2761  et('options', 'a
+0000fb30: 6464 6f6e 735f 7061 7468 272c 2027 2c27  ddons_path', ','
+0000fb40: 2e6a 6f69 6e28 7061 7468 7329 290a 2020  .join(paths)).  
+0000fb50: 2020 6966 206f 755f 7665 725f 7061 7468    if ou_ver_path
+0000fb60: 3a0a 2020 2020 2020 2020 7372 635f 636f  :.        src_co
+0000fb70: 6e66 6967 2e73 6574 2827 6f70 7469 6f6e  nfig.set('option
+0000fb80: 7327 2c20 2772 6f6f 745f 7061 7468 272c  s', 'root_path',
+0000fb90: 206f 755f 7665 725f 7061 7468 290a 2020   ou_ver_path).  
+0000fba0: 2020 7372 635f 636f 6e66 6967 2e77 7269    src_config.wri
+0000fbb0: 7465 286f 7065 6e28 6675 6c6c 5f6c 636f  te(open(full_lco
+0000fbc0: 6e66 2c20 2777 2b27 2929 0a20 2020 2073  nf, 'w+')).    s
+0000fbd0: 7263 5f63 6f6e 6669 672e 7265 6164 2866  rc_config.read(f
+0000fbe0: 756c 6c5f 6c63 6f6e 6629 0a20 2020 2072  ull_lconf).    r
+0000fbf0: 6574 7572 6e20 6675 6c6c 5f6c 636f 6e66  eturn full_lconf
+0000fc00: 0a0a 0a64 6566 2068 6172 645f 636c 6561  ...def hard_clea
+0000fc10: 6e5f 6d6f 6475 6c65 2863 7478 2c20 6d6f  n_module(ctx, mo
+0000fc20: 6475 6c65 5f6e 616d 6529 3a0a 2020 2020  dule_name):.    
+0000fc30: 6465 6620 6472 6f70 5f64 6174 615f 7461  def drop_data_ta
+0000fc40: 626c 6528 6374 782c 206d 6f64 656c 2c20  ble(ctx, model, 
+0000fc50: 6d6f 6475 6c65 5f6e 616d 652c 2063 6f6c  module_name, col
+0000fc60: 6e3d 4e6f 6e65 2c20 6964 3d4e 6f6e 6529  n=None, id=None)
+0000fc70: 3a0a 2020 2020 2020 2020 636f 6c6e 203d  :.        coln =
+0000fc80: 2063 6f6c 6e20 6f72 2027 6d6f 6475 6c65   coln or 'module
+0000fc90: 270a 2020 2020 2020 2020 6966 2069 643a  '.        if id:
+0000fca0: 0a20 2020 2020 2020 2020 2020 2071 7565  .            que
+0000fcb0: 7279 203d 2022 6465 6c65 7465 2066 726f  ry = "delete fro
+0000fcc0: 6d20 2573 2077 6865 7265 2025 733d 2564  m %s where %s=%d
+0000fcd0: 2220 2520 286d 6f64 656c 2c20 636f 6c6e  " % (model, coln
+0000fce0: 2c20 6964 290a 2020 2020 2020 2020 656c  , id).        el
+0000fcf0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000fd00: 7175 6572 7920 3d20 2264 656c 6574 6520  query = "delete 
+0000fd10: 6672 6f6d 2025 7320 7768 6572 6520 2573  from %s where %s
+0000fd20: 3d27 2573 2722 2025 2028 6d6f 6465 6c2c  ='%s'" % (model,
+0000fd30: 2063 6f6c 6e2c 206d 6f64 756c 655f 6e61   coln, module_na
+0000fd40: 6d65 290a 2020 2020 2020 2020 7265 6373  me).        recs
+0000fd50: 203d 2065 7865 635f 7371 6c28 6374 782c   = exec_sql(ctx,
+0000fd60: 2071 7565 7279 290a 0a20 2020 2071 7565   query)..    que
+0000fd70: 7279 203d 2022 7365 6c65 6374 2069 642c  ry = "select id,
+0000fd80: 6e61 6d65 2c73 7461 7465 2066 726f 6d20  name,state from 
+0000fd90: 6972 5f6d 6f64 756c 655f 6d6f 6475 6c65  ir_module_module
+0000fda0: 2077 6865 7265 206e 616d 653d 2725 7327   where name='%s'
+0000fdb0: 2220 2520 6d6f 6475 6c65 5f6e 616d 650a  " % module_name.
+0000fdc0: 2020 2020 7265 6373 203d 2065 7865 635f      recs = exec_
+0000fdd0: 7371 6c28 6374 782c 2071 7565 7279 2c20  sql(ctx, query, 
+0000fde0: 7265 7370 6f6e 7365 3d54 7275 6529 0a20  response=True). 
+0000fdf0: 2020 2069 6620 6e6f 7420 6c65 6e28 7265     if not len(re
+0000fe00: 6373 293a 0a20 2020 2020 2020 2072 6574  cs):.        ret
+0000fe10: 7572 6e0a 2020 2020 7374 6174 6520 3d20  urn.    state = 
+0000fe20: 7265 6373 5b30 5d5b 325d 0a20 2020 2069  recs[0][2].    i
+0000fe30: 6420 3d20 7265 6373 5b30 5d5b 305d 0a20  d = recs[0][0]. 
+0000fe40: 2020 2069 6620 7374 6174 6520 3d3d 2027     if state == '
+0000fe50: 696e 7374 616c 6c65 6427 3a0a 2020 2020  installed':.    
+0000fe60: 2020 2020 7265 7475 726e 0a20 2020 2064      return.    d
+0000fe70: 726f 705f 6461 7461 5f74 6162 6c65 2863  rop_data_table(c
+0000fe80: 7478 2c20 2769 725f 6d6f 6465 6c5f 6461  tx, 'ir_model_da
+0000fe90: 7461 272c 206d 6f64 756c 655f 6e61 6d65  ta', module_name
+0000fea0: 290a 2020 2020 6472 6f70 5f64 6174 615f  ).    drop_data_
+0000feb0: 7461 626c 6528 0a20 2020 2020 2020 2063  table(.        c
+0000fec0: 7478 2c20 2769 725f 6d6f 6475 6c65 5f6d  tx, 'ir_module_m
+0000fed0: 6f64 756c 655f 6465 7065 6e64 656e 6379  odule_dependency
+0000fee0: 272c 206d 6f64 756c 655f 6e61 6d65 2c20  ', module_name, 
+0000fef0: 636f 6c6e 3d27 6d6f 6475 6c65 5f69 6427  coln='module_id'
+0000ff00: 2c20 6964 3d69 640a 2020 2020 290a 2020  , id=id.    ).  
+0000ff10: 2020 6472 6f70 5f64 6174 615f 7461 626c    drop_data_tabl
+0000ff20: 6528 6374 782c 2027 6972 5f74 7261 6e73  e(ctx, 'ir_trans
+0000ff30: 6c61 7469 6f6e 272c 206d 6f64 756c 655f  lation', module_
+0000ff40: 6e61 6d65 290a 2020 2020 7365 745f 756e  name).    set_un
+0000ff50: 696e 7374 616c 6c65 645f 6279 5f73 716c  installed_by_sql
+0000ff60: 2863 7478 2c20 5b5f 6228 6d6f 6475 6c65  (ctx, [_b(module
+0000ff70: 5f6e 616d 6529 5d29 0a0a 0a64 6566 2066  _name)])...def f
+0000ff80: 6978 5f62 7567 5f70 7265 2873 7263 5f63  ix_bug_pre(src_c
+0000ff90: 7478 2c20 7467 745f 6374 782c 2073 7263  tx, tgt_ctx, src
+0000ffa0: 5f66 756c 6c5f 6c63 6f6e 662c 2073 7263  _full_lconf, src
+0000ffb0: 5f70 6174 6873 293a 0a20 2020 2073 6176  _paths):.    sav
+0000ffc0: 6564 5f64 622c 2073 7263 5f63 7478 5b27  ed_db, src_ctx['
+0000ffd0: 6462 5f6e 616d 6527 5d20 3d20 7372 635f  db_name'] = src_
+0000ffe0: 6374 785b 2764 625f 6e61 6d65 275d 2c20  ctx['db_name'], 
+0000fff0: 7467 745f 6374 785b 2764 625f 6e61 6d65  tgt_ctx['db_name
+00010000: 275d 0a20 2020 2069 6620 7372 635f 6374  '].    if src_ct
+00010010: 785b 2773 7263 5f6f 646f 6f5f 6676 6572  x['src_odoo_fver
+00010020: 275d 203d 3d20 2737 2e30 2720 616e 6420  '] == '7.0' and 
+00010030: 7467 745f 6374 785b 2774 6774 5f6f 646f  tgt_ctx['tgt_odo
+00010040: 6f5f 6676 6572 275d 203d 3d20 2738 2e30  o_fver'] == '8.0
+00010050: 273a 0a20 2020 2020 2020 2071 7565 7279  ':.        query
+00010060: 203d 2027 2727 7570 6461 7465 2069 725f   = '''update ir_
+00010070: 7569 5f76 6965 770a 2020 2020 2020 2020  ui_view.        
+00010080: 2020 2020 2020 2020 7365 7420 6172 6368          set arch
+00010090: 3d52 4547 4558 505f 5245 504c 4143 4528  =REGEXP_REPLACE(
+000100a0: 6172 6368 2c20 273c 6669 656c 6420 6e61  arch, '<field na
+000100b0: 6d65 3d22 6d65 6e75 5f69 6422 2e2a 2f3e  me="menu_id".*/>
+000100c0: 272c 2027 2729 0a20 2020 2020 2020 2020  ', '').         
+000100d0: 2020 2020 2020 2077 6865 7265 206d 6f64         where mod
+000100e0: 656c 3d27 7265 732e 7573 6572 7327 2061  el='res.users' a
+000100f0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+00010100: 2020 2020 2020 2020 2061 7263 6820 6c69           arch li
+00010110: 6b65 2027 253c 6669 656c 6420 6e61 6d65  ke '%<field name
+00010120: 3d5f 6d65 6e75 5f69 645f 2527 3b27 2727  =_menu_id_%';'''
+00010130: 0a20 2020 2020 2020 2065 7865 635f 7371  .        exec_sq
+00010140: 6c28 7372 635f 6374 782c 2071 7565 7279  l(src_ctx, query
+00010150: 290a 2020 2020 656c 6966 2073 7263 5f63  ).    elif src_c
+00010160: 7478 5b27 7372 635f 6f64 6f6f 5f66 7665  tx['src_odoo_fve
+00010170: 7227 5d20 3d3d 2027 382e 3027 2061 6e64  r'] == '8.0' and
+00010180: 2074 6774 5f63 7478 5b27 7467 745f 6f64   tgt_ctx['tgt_od
+00010190: 6f6f 5f66 7665 7227 5d20 3d3d 2027 392e  oo_fver'] == '9.
+000101a0: 3027 3a0a 2020 2020 2020 2020 6966 2027  0':.        if '
+000101b0: 6163 636f 756e 745f 7061 796d 656e 7427  account_payment'
+000101c0: 2069 6e20 7372 635f 6374 785b 2773 7263   in src_ctx['src
+000101d0: 5f6d 6f64 756c 655f 6c69 7374 275d 3a0a  _module_list']:.
+000101e0: 2020 2020 2020 2020 2020 2020 7374 7320              sts 
+000101f0: 3d20 636c 6f64 6f6f 2e61 6374 5f69 6e73  = clodoo.act_ins
+00010200: 7461 6c6c 5f6d 6f64 756c 6573 280a 2020  tall_modules(.  
+00010210: 2020 2020 2020 2020 2020 2020 2020 7372                sr
+00010220: 635f 6374 782c 206d 6f64 756c 655f 6c69  c_ctx, module_li
+00010230: 7374 3d5b 2761 6363 6f75 6e74 5f62 616e  st=['account_ban
+00010240: 6b69 6e67 5f70 6179 6d65 6e74 5f65 7870  king_payment_exp
+00010250: 6f72 7427 5d0a 2020 2020 2020 2020 2020  ort'].          
+00010260: 2020 290a 2020 2020 7372 635f 6374 785b    ).    src_ctx[
+00010270: 2764 625f 6e61 6d65 275d 203d 2073 6176  'db_name'] = sav
+00010280: 6564 5f64 620a 0a0a 6465 6620 6669 785f  ed_db...def fix_
+00010290: 6275 675f 706f 7374 2873 7263 5f63 7478  bug_post(src_ctx
+000102a0: 2c20 7467 745f 6374 782c 2074 6774 5f66  , tgt_ctx, tgt_f
+000102b0: 756c 6c5f 6c63 6f6e 662c 2074 6774 5f70  ull_lconf, tgt_p
+000102c0: 6174 6873 293a 0a20 2020 2069 6620 7372  aths):.    if sr
+000102d0: 635f 6374 785b 2773 7263 5f6f 646f 6f5f  c_ctx['src_odoo_
+000102e0: 6676 6572 275d 203d 3d20 2737 2e30 2720  fver'] == '7.0' 
+000102f0: 616e 6420 7467 745f 6374 785b 2774 6774  and tgt_ctx['tgt
+00010300: 5f6f 646f 6f5f 6676 6572 275d 203d 3d20  _odoo_fver'] == 
+00010310: 2738 2e30 273a 0a20 2020 2020 2020 2070  '8.0':.        p
+00010320: 6173 730a 0a0a 6465 6620 6d69 6772 6174  ass...def migrat
+00010330: 655f 6f64 6f6f 2873 7263 5f63 7478 2c20  e_odoo(src_ctx, 
+00010340: 7467 745f 6374 782c 2073 7263 5f63 6f6e  tgt_ctx, src_con
+00010350: 6669 672c 2074 6774 5f63 6f6e 6669 672c  fig, tgt_config,
+00010360: 2070 6861 7365 3d4e 6f6e 6529 3a0a 2020   phase=None):.  
+00010370: 2020 6465 6620 6765 745f 7772 6f6e 675f    def get_wrong_
+00010380: 6d6f 6475 6c65 7328 6374 782c 2062 6164  modules(ctx, bad
+00010390: 5f6d 6f64 756c 655f 6c69 7374 3d4e 6f6e  _module_list=Non
+000103a0: 6529 3a0a 2020 2020 2020 2020 6966 2073  e):.        if s
+000103b0: 7263 5f63 7478 5b27 6472 795f 7275 6e27  rc_ctx['dry_run'
+000103c0: 5d3a 0a20 2020 2020 2020 2020 2020 2072  ]:.            r
+000103d0: 6574 7572 6e20 5b5d 0a20 2020 2020 2020  eturn [].       
+000103e0: 2069 6620 6261 645f 6d6f 6475 6c65 5f6c   if bad_module_l
+000103f0: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
+00010400: 2069 6620 6c65 6e28 6261 645f 6d6f 6475   if len(bad_modu
+00010410: 6c65 5f6c 6973 7429 203d 3d20 313a 0a20  le_list) == 1:. 
+00010420: 2020 2020 2020 2020 2020 2020 2020 2071                 q
+00010430: 7565 7279 203d 2028 0a20 2020 2020 2020  uery = (.       
+00010440: 2020 2020 2020 2020 2020 2020 2027 2727               '''
+00010450: 7365 6c65 6374 2069 642c 6e61 6d65 2c73  select id,name,s
+00010460: 7461 7465 2066 726f 6d20 6972 5f6d 6f64  tate from ir_mod
+00010470: 756c 655f 6d6f 6475 6c65 0a20 2020 2020  ule_module.     
+00010480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010490: 2020 2020 2020 7768 6572 6520 7374 6174        where stat
+000104a0: 6520 6e6f 7420 696e 0a20 2020 2020 2020  e not in.       
+000104b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000104c0: 2020 2020 2827 696e 7374 616c 6c65 6427      ('installed'
+000104d0: 2c20 2775 6e69 6e73 7461 6c6c 6564 272c  , 'uninstalled',
+000104e0: 2027 756e 696e 7374 616c 6c61 626c 6527   'uninstallable'
+000104f0: 2920 616e 640a 2020 2020 2020 2020 2020  ) and.          
+00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010510: 206e 616d 6520 3d20 2725 7327 3b27 2727   name = '%s';'''
+00010520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010530: 2020 2020 2025 2062 6164 5f6d 6f64 756c       % bad_modul
+00010540: 655f 6c69 7374 5b30 5d0a 2020 2020 2020  e_list[0].      
+00010550: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00010560: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00010570: 2020 2020 2020 2020 2020 2020 2020 7175                qu
+00010580: 6572 7920 3d20 2727 2773 656c 6563 7420  ery = '''select 
+00010590: 6964 2c6e 616d 652c 7374 6174 6520 6672  id,name,state fr
+000105a0: 6f6d 2069 725f 6d6f 6475 6c65 5f6d 6f64  om ir_module_mod
+000105b0: 756c 650a 2020 2020 2020 2020 2020 2020  ule.            
+000105c0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+000105d0: 6865 7265 2073 7461 7465 206e 6f74 2069  here state not i
+000105e0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+000105f0: 2020 2020 2020 2020 2020 2020 2028 2769               ('i
+00010600: 6e73 7461 6c6c 6564 272c 2027 756e 696e  nstalled', 'unin
+00010610: 7374 616c 6c65 6427 2c20 2775 6e69 6e73  stalled', 'unins
+00010620: 7461 6c6c 6162 6c65 2729 2061 6e64 0a20  tallable') and. 
+00010630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010640: 2020 2020 2020 2020 2020 6e61 6d65 2069            name i
+00010650: 6e20 2825 7329 3b27 2727 2025 2028 0a20  n (%s);''' % (. 
+00010660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010670: 2020 2022 2725 7327 2220 2520 2227 2c27     "'%s'" % "','
+00010680: 222e 6a6f 696e 2862 6164 5f6d 6f64 756c  ".join(bad_modul
+00010690: 655f 6c69 7374 290a 2020 2020 2020 2020  e_list).        
+000106a0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+000106b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000106c0: 2020 2020 2071 7565 7279 203d 2027 2727       query = '''
+000106d0: 7365 6c65 6374 2069 642c 6e61 6d65 2c73  select id,name,s
+000106e0: 7461 7465 2066 726f 6d20 6972 5f6d 6f64  tate from ir_mod
+000106f0: 756c 655f 6d6f 6475 6c65 0a20 2020 2020  ule_module.     
+00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010710: 2020 7768 6572 6520 7374 6174 6520 6e6f    where state no
+00010720: 7420 696e 0a20 2020 2020 2020 2020 2020  t in.           
+00010730: 2020 2020 2020 2020 2020 2020 2827 696e              ('in
+00010740: 7374 616c 6c65 6427 2c20 2775 6e69 6e73  stalled', 'unins
+00010750: 7461 6c6c 6564 272c 2027 756e 696e 7374  talled', 'uninst
+00010760: 616c 6c61 626c 6527 293b 2727 270a 2020  allable');'''.  
+00010770: 2020 2020 2020 726f 7773 203d 2065 7865        rows = exe
+00010780: 635f 7371 6c28 6374 782c 2071 7565 7279  c_sql(ctx, query
+00010790: 2c20 7265 7370 6f6e 7365 3d54 7275 6529  , response=True)
+000107a0: 0a20 2020 2020 2020 2077 726f 6e67 5f6c  .        wrong_l
+000107b0: 6973 7420 3d20 5b5d 0a20 2020 2020 2020  ist = [].       
+000107c0: 2066 6f72 2072 6f77 2069 6e20 726f 7773   for row in rows
+000107d0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000107e0: 206e 6f74 2062 6164 5f6d 6f64 756c 655f   not bad_module_
+000107f0: 6c69 7374 206f 7220 726f 775b 315d 206e  list or row[1] n
+00010800: 6f74 2069 6e20 6261 645f 6d6f 6475 6c65  ot in bad_module
+00010810: 5f6c 6973 743a 0a20 2020 2020 2020 2020  _list:.         
+00010820: 2020 2020 2020 2077 726f 6e67 5f6c 6973         wrong_lis
+00010830: 742e 6170 7065 6e64 2872 6f77 5b31 5d29  t.append(row[1])
+00010840: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00010850: 7772 6f6e 675f 6c69 7374 0a0a 2020 2020  wrong_list..    
+00010860: 6465 6620 7275 6e5f 6f70 656e 7570 6772  def run_openupgr
+00010870: 6164 6528 7467 745f 6374 782c 206f 755f  ade(tgt_ctx, ou_
+00010880: 7665 725f 7061 7468 2c20 7467 745f 6675  ver_path, tgt_fu
+00010890: 6c6c 5f6c 636f 6e66 293a 0a20 2020 2020  ll_lconf):.     
+000108a0: 2020 206f 7570 6174 685f 7363 7269 7074     oupath_script
+000108b0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+000108c0: 2066 6f72 2070 2069 6e20 2827 272c 2027   for p in ('', '
+000108d0: 6f64 6f6f 272c 2027 6f70 656e 6572 7027  odoo', 'openerp'
+000108e0: 2c20 2773 6572 7665 7227 293a 0a20 2020  , 'server'):.   
+000108f0: 2020 2020 2020 2020 2069 6620 6f75 7061           if oupa
+00010900: 7468 5f73 6372 6970 743a 0a20 2020 2020  th_script:.     
+00010910: 2020 2020 2020 2020 2020 2062 7265 616b             break
+00010920: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00010930: 206e 2069 6e20 2827 6f64 6f6f 2d62 696e   n in ('odoo-bin
+00010940: 272c 2027 6f70 656e 6572 702d 7365 7276  ', 'openerp-serv
+00010950: 6572 2729 3a0a 2020 2020 2020 2020 2020  er'):.          
+00010960: 2020 2020 2020 6966 2070 3a0a 2020 2020        if p:.    
+00010970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010980: 7363 7269 7074 203d 206f 732e 7061 7468  script = os.path
+00010990: 2e6a 6f69 6e28 6f75 5f76 6572 5f70 6174  .join(ou_ver_pat
+000109a0: 682c 2070 2c20 6e29 0a20 2020 2020 2020  h, p, n).       
+000109b0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+000109c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109d0: 2020 2073 6372 6970 7420 3d20 6f73 2e70     script = os.p
+000109e0: 6174 682e 6a6f 696e 286f 755f 7665 725f  ath.join(ou_ver_
+000109f0: 7061 7468 2c20 6e29 0a20 2020 2020 2020  path, n).       
+00010a00: 2020 2020 2020 2020 2069 6620 6f73 2e70           if os.p
+00010a10: 6174 682e 6973 6669 6c65 2873 6372 6970  ath.isfile(scrip
+00010a20: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00010a30: 2020 2020 2020 2020 6f75 7061 7468 5f73          oupath_s
+00010a40: 6372 6970 7420 3d20 7363 7269 7074 0a20  cript = script. 
+00010a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010a60: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00010a70: 2069 6620 7372 635f 6374 785b 276e 6f5f   if src_ctx['no_
+00010a80: 7665 6e76 275d 3a0a 2020 2020 2020 2020  venv']:.        
+00010a90: 2020 2020 7374 7320 3d20 7275 6e5f 7472      sts = run_tr
+00010aa0: 6163 6564 280a 2020 2020 2020 2020 2020  aced(.          
+00010ab0: 2020 2020 2020 6f75 7061 7468 5f73 6372        oupath_scr
+00010ac0: 6970 742c 0a20 2020 2020 2020 2020 2020  ipt,.           
+00010ad0: 2020 2020 2027 2d63 272c 0a20 2020 2020       '-c',.     
+00010ae0: 2020 2020 2020 2020 2020 2074 6774 5f66             tgt_f
+00010af0: 756c 6c5f 6c63 6f6e 662c 0a20 2020 2020  ull_lconf,.     
+00010b00: 2020 2020 2020 2020 2020 2027 2d64 272c             '-d',
+00010b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b20: 2074 6774 5f63 7478 5b27 6462 5f6e 616d   tgt_ctx['db_nam
+00010b30: 6527 5d2c 0a20 2020 2020 2020 2020 2020  e'],.           
+00010b40: 2020 2020 2027 2d75 272c 0a20 2020 2020       '-u',.     
+00010b50: 2020 2020 2020 2020 2020 2027 616c 6c27             'all'
+00010b60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010b70: 2020 272d 2d73 746f 702d 6166 7465 722d    '--stop-after-
+00010b80: 696e 6974 272c 0a20 2020 2020 2020 2020  init',.         
+00010b90: 2020 2020 2020 2027 2d2d 6e6f 2d78 6d6c         '--no-xml
+00010ba0: 7270 6327 2c0a 2020 2020 2020 2020 2020  rpc',.          
+00010bb0: 2020 2020 2020 272d 2d6c 6f67 6669 6c65        '--logfile
+00010bc0: 3d25 7327 2025 2074 6774 5f63 7478 5b27  =%s' % tgt_ctx['
+00010bd0: 6c6f 6766 696c 6527 5d2c 0a20 2020 2020  logfile'],.     
+00010be0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00010bf0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00010c00: 2020 2073 6372 6970 7420 3d20 6f73 2e70     script = os.p
+00010c10: 6174 682e 6a6f 696e 286f 755f 7665 725f  ath.join(ou_ver_
+00010c20: 7061 7468 2c20 276d 6967 7261 7465 2e73  path, 'migrate.s
+00010c30: 6827 290a 2020 2020 2020 2020 2020 2020  h').            
+00010c40: 6664 203d 206f 7065 6e28 7363 7269 7074  fd = open(script
+00010c50: 2c20 2777 2729 0a20 2020 2020 2020 2020  , 'w').         
+00010c60: 2020 2066 642e 7772 6974 6528 2763 6420     fd.write('cd 
+00010c70: 2573 5c6e 2720 2520 7467 745f 6374 785b  %s\n' % tgt_ctx[
+00010c80: 2776 656e 765f 6f75 7061 7468 275d 290a  'venv_oupath']).
+00010c90: 2020 2020 2020 2020 2020 2020 6664 2e77              fd.w
+00010ca0: 7269 7465 2862 2773 6f75 7263 6520 2e2f  rite(b'source ./
+00010cb0: 6269 6e2f 6163 7469 7661 7465 5c6e 2729  bin/activate\n')
+00010cc0: 0a20 2020 2020 2020 2020 2020 2066 642e  .            fd.
+00010cd0: 7772 6974 6528 0a20 2020 2020 2020 2020  write(.         
+00010ce0: 2020 2020 2020 2062 2725 7320 2d63 2025         b'%s -c %
+00010cf0: 7320 2d64 2025 7320 2d75 2061 6c6c 202d  s -d %s -u all -
+00010d00: 2d73 746f 702d 6166 7465 722d 696e 6974  -stop-after-init
+00010d10: 202d 2d6e 6f2d 786d 6c72 7063 270a 2020   --no-xmlrpc'.  
+00010d20: 2020 2020 2020 2020 2020 2020 2020 6227                b'
+00010d30: 202d 2d6c 6f67 6669 6c65 3d25 735c 6e27   --logfile=%s\n'
+00010d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010d50: 2025 2028 0a20 2020 2020 2020 2020 2020   % (.           
+00010d60: 2020 2020 2020 2020 206f 7570 6174 685f           oupath_
+00010d70: 7363 7269 7074 2c0a 2020 2020 2020 2020  script,.        
+00010d80: 2020 2020 2020 2020 2020 2020 7467 745f              tgt_
+00010d90: 6675 6c6c 5f6c 636f 6e66 2c0a 2020 2020  full_lconf,.    
+00010da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010db0: 7467 745f 6374 785b 2764 625f 6e61 6d65  tgt_ctx['db_name
+00010dc0: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
+00010dd0: 2020 2020 2020 2020 7467 745f 6374 785b          tgt_ctx[
+00010de0: 276c 6f67 6669 6c65 275d 2c0a 2020 2020  'logfile'],.    
+00010df0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00010e00: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00010e10: 2020 2020 2020 2020 6664 2e77 7269 7465          fd.write
+00010e20: 2862 2773 7473 3d24 3f5c 6e27 290a 2020  (b'sts=$?\n').  
+00010e30: 2020 2020 2020 2020 2020 6664 2e77 7269            fd.wri
+00010e40: 7465 2862 2764 6561 6374 6976 6174 655c  te(b'deactivate\
+00010e50: 6e27 290a 2020 2020 2020 2020 2020 2020  n').            
+00010e60: 6664 2e77 7269 7465 2862 2765 7869 7420  fd.write(b'exit 
+00010e70: 2473 7473 5c6e 2729 0a20 2020 2020 2020  $sts\n').       
+00010e80: 2020 2020 2066 642e 636c 6f73 6528 290a       fd.close().
+00010e90: 2020 2020 2020 2020 2020 2020 6f73 2e63              os.c
+00010ea0: 686d 6f64 2873 6372 6970 742c 2030 6f37  hmod(script, 0o7
+00010eb0: 3434 290a 2020 2020 2020 2020 2020 2020  44).            
+00010ec0: 7374 7320 3d20 300a 2020 2020 2020 2020  sts = 0.        
+00010ed0: 2020 2020 6966 206e 6f74 2073 7263 5f63      if not src_c
+00010ee0: 7478 5b27 6472 795f 7275 6e27 5d3a 0a20  tx['dry_run']:. 
+00010ef0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010f00: 7473 203d 206f 732e 7379 7374 656d 2873  ts = os.system(s
+00010f10: 6372 6970 7429 0a20 2020 2020 2020 2069  cript).        i
+00010f20: 6620 7374 733a 0a20 2020 2020 2020 2020  f sts:.         
+00010f30: 2020 206f 7330 2e77 6c6f 6728 272a 2a2a     os0.wlog('***
+00010f40: 2052 6574 7572 6e20 636f 6465 2025 6420   Return code %d 
+00010f50: 2a2a 2a27 290a 2020 2020 2020 2020 656c  ***').        el
+00010f60: 6966 206e 6f74 2073 7263 5f63 7478 5b27  if not src_ctx['
+00010f70: 6472 795f 7275 6e27 5d3a 0a20 2020 2020  dry_run']:.     
+00010f80: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
+00010f90: 7028 3529 0a0a 2020 2020 7068 6173 6520  p(5)..    phase 
+00010fa0: 3d20 7068 6173 6520 6f72 2032 0a20 2020  = phase or 2.   
+00010fb0: 2074 6774 5f73 6176 6564 5f66 636f 6e66   tgt_saved_fconf
+00010fc0: 203d 2074 6774 5f63 7478 5b27 636f 6e66   = tgt_ctx['conf
+00010fd0: 5f66 6e27 5d0a 2020 2020 7372 635f 6675  _fn'].    src_fu
+00010fe0: 6c6c 5f6c 636f 6e66 203d 2070 7265 7061  ll_lconf = prepa
+00010ff0: 7265 5f63 6f6e 6669 675f 6669 6c65 2873  re_config_file(s
+00011000: 7263 5f63 7478 2c20 7372 635f 636f 6e66  rc_ctx, src_conf
+00011010: 6967 290a 2020 2020 6966 2073 7263 5f63  ig).    if src_c
+00011020: 7478 5b27 7372 635f 7669 6427 5d20 3d3d  tx['src_vid'] ==
+00011030: 2073 7263 5f63 7478 5b27 6672 6f6d 5f62   src_ctx['from_b
+00011040: 7261 6e63 6827 5d20 616e 6420 6765 745f  ranch'] and get_
+00011050: 7772 6f6e 675f 6d6f 6475 6c65 7328 7372  wrong_modules(sr
+00011060: 635f 6374 7829 3a0a 2020 2020 2020 2020  c_ctx):.        
+00011070: 6966 2070 6861 7365 203d 3d20 313a 0a20  if phase == 1:. 
+00011080: 2020 2020 2020 2020 2020 206f 7330 2e77             os0.w
+00011090: 6c6f 6728 272a 2a2a 2055 6e73 7461 626c  log('*** Unstabl
+000110a0: 6520 696e 7374 616c 6c61 7469 6f6e 202a  e installation *
+000110b0: 2a2a 2729 0a20 2020 2020 2020 2065 6c73  **').        els
+000110c0: 653a 0a20 2020 2020 2020 2020 2020 206f  e:.            o
+000110d0: 7330 2e77 6c6f 6728 272a 2a2a 2055 6e73  s0.wlog('*** Uns
+000110e0: 7461 626c 6520 696e 7374 616c 6c61 7469  table installati
+000110f0: 6f6e 3a20 7472 7920 746f 2063 6f72 7265  on: try to corre
+00011100: 6374 2065 7272 6f72 7320 2a2a 2a27 290a  ct errors ***').
+00011110: 2020 2020 2020 2020 2020 2020 7275 6e5f              run_
+00011120: 6f64 6f6f 5f61 6c6c 7465 7374 280a 2020  odoo_alltest(.  
+00011130: 2020 2020 2020 2020 2020 2020 2020 7372                sr
+00011140: 635f 6374 785b 2774 6774 5f76 6964 275d  c_ctx['tgt_vid']
+00011150: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011160: 2020 7372 635f 6675 6c6c 5f6c 636f 6e66    src_full_lconf
+00011170: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011180: 2020 7372 635f 6374 785b 2764 625f 6e61    src_ctx['db_na
+00011190: 6d65 275d 2c0a 2020 2020 2020 2020 2020  me'],.          
+000111a0: 2020 2020 2020 7372 635f 6374 785b 276c        src_ctx['l
+000111b0: 6f67 6669 6c65 275d 2c0a 2020 2020 2020  ogfile'],.      
+000111c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000111d0: 2020 2020 6261 645f 6d6f 6475 6c65 7320      bad_modules 
+000111e0: 3d20 6765 745f 7772 6f6e 675f 6d6f 6475  = get_wrong_modu
+000111f0: 6c65 7328 7372 635f 6374 7829 0a20 2020  les(src_ctx).   
+00011200: 2020 2020 2020 2020 2069 6620 6261 645f           if bad_
+00011210: 6d6f 6475 6c65 733a 0a20 2020 2020 2020  modules:.       
+00011220: 2020 2020 2020 2020 206f 7330 2e77 6c6f           os0.wlo
+00011230: 6728 272a 2a2a 2055 6e73 7461 626c 6520  g('*** Unstable 
+00011240: 696e 7374 616c 6c61 7469 6f6e 2064 7565  installation due
+00011250: 2074 6f20 2573 202a 2a2a 2720 2520 6261   to %s ***' % ba
+00011260: 645f 6d6f 6475 6c65 7329 0a20 2020 2020  d_modules).     
+00011270: 2020 2020 2020 2020 2020 206f 7330 2e77             os0.w
+00011280: 6c6f 6728 272a 2a2a 204d 4947 5241 5449  log('*** MIGRATI
+00011290: 4f4e 2053 544f 5050 4544 202a 2a2a 2729  ON STOPPED ***')
+000112a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000112b0: 2073 7973 2e65 7869 7428 3129 0a0a 2020   sys.exit(1)..  
+000112c0: 2020 7372 635f 7061 7468 7320 3d20 636f    src_paths = co
+000112d0: 6e66 6967 5f67 6574 5f6c 6973 7428 7372  nfig_get_list(sr
+000112e0: 635f 636f 6e66 6967 2c20 2761 6464 6f6e  c_config, 'addon
+000112f0: 735f 7061 7468 2729 0a20 2020 2074 6774  s_path').    tgt
+00011300: 5f70 6174 6873 203d 2063 6f6e 6669 675f  _paths = config_
+00011310: 6765 745f 6c69 7374 2874 6774 5f63 6f6e  get_list(tgt_con
+00011320: 6669 672c 2027 6164 646f 6e73 5f70 6174  fig, 'addons_pat
+00011330: 6827 290a 2020 2020 6f73 302e 776c 6f67  h').    os0.wlog
+00011340: 2827 6164 646f 6e73 5f70 6174 683d 2573  ('addons_path=%s
+00011350: 2720 2520 7372 635f 7061 7468 7329 0a20  ' % src_paths). 
+00011360: 2020 2069 6620 7068 6173 6520 3e20 3120     if phase > 1 
+00011370: 6f72 2073 7263 5f63 7478 5b27 7372 635f  or src_ctx['src_
+00011380: 7669 6427 5d20 3d3d 2073 7263 5f63 7478  vid'] == src_ctx
+00011390: 5b27 6672 6f6d 5f62 7261 6e63 6827 5d3a  ['from_branch']:
+000113a0: 0a20 2020 2020 2020 206f 7330 2e77 6c6f  .        os0.wlo
+000113b0: 6728 2754 6573 7420 636f 6e6e 6563 7469  g('Test connecti
+000113c0: 6f6e 2074 6f20 736f 7572 6365 2064 6220  on to source db 
+000113d0: 2573 2720 2520 7372 635f 6374 785b 2764  %s' % src_ctx['d
+000113e0: 625f 6e61 6d65 275d 290a 2020 2020 2020  b_name']).      
+000113f0: 2020 7569 642c 2073 7263 5f63 7478 203d    uid, src_ctx =
+00011400: 2063 6c6f 646f 6f2e 6f65 7270 5f73 6574   clodoo.oerp_set
+00011410: 5f65 6e76 280a 2020 2020 2020 2020 2020  _env(.          
+00011420: 2020 6374 783d 7372 635f 6374 782c 2063    ctx=src_ctx, c
+00011430: 6f6e 666e 3d73 7263 5f66 756c 6c5f 6c63  onfn=src_full_lc
+00011440: 6f6e 662c 2064 623d 7372 635f 6374 785b  onf, db=src_ctx[
+00011450: 2764 625f 6e61 6d65 275d 0a20 2020 2020  'db_name'].     
+00011460: 2020 2029 0a20 2020 2020 2020 2023 2046     ).        # F
+00011470: 4958 206f 6572 705f 7365 745f 656e 7620  IX oerp_set_env 
+00011480: 6368 616e 6765 2064 7279 5f72 756e 0a20  change dry_run. 
+00011490: 2020 2020 2020 2073 7263 5f63 7478 5b27         src_ctx['
+000114a0: 6472 795f 7275 6e27 5d20 3d20 7467 745f  dry_run'] = tgt_
+000114b0: 6374 785b 2764 7279 5f72 756e 275d 0a20  ctx['dry_run']. 
+000114c0: 2020 2020 2020 2069 6620 7068 6173 6520         if phase 
+000114d0: 3e20 313a 0a20 2020 2020 2020 2020 2020  > 1:.           
+000114e0: 2069 6620 7372 635f 6374 785b 276f 7074   if src_ctx['opt
+000114f0: 5f73 6166 6527 5d20 616e 6420 7372 635f  _safe'] and src_
+00011500: 6374 785b 2773 7263 5f76 6964 275d 203d  ctx['src_vid'] =
+00011510: 3d20 7372 635f 6374 785b 2766 726f 6d5f  = src_ctx['from_
+00011520: 6272 616e 6368 275d 3a0a 2020 2020 2020  branch']:.      
+00011530: 2020 2020 2020 2020 2020 636c 6f64 6f6f            clodoo
+00011540: 2e61 6374 5f63 6865 636b 5f63 6f6e 6669  .act_check_confi
+00011550: 6728 7372 635f 6374 7829 0a20 2020 2020  g(src_ctx).     
+00011560: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
+00011570: 2020 2020 2020 2020 2020 2020 7372 635f              src_
+00011580: 6374 785b 2775 6e69 6e73 7461 6c6c 5f6d  ctx['uninstall_m
+00011590: 6f64 756c 6573 275d 0a20 2020 2020 2020  odules'].       
+000115a0: 2020 2020 2020 2020 2061 6e64 2073 7263           and src
+000115b0: 5f63 7478 5b27 7372 635f 7669 6427 5d20  _ctx['src_vid'] 
+000115c0: 3d3d 2073 7263 5f63 7478 5b27 6672 6f6d  == src_ctx['from
+000115d0: 5f62 7261 6e63 6827 5d0a 2020 2020 2020  _branch'].      
+000115e0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+000115f0: 2020 2020 2020 2020 2066 6f72 206d 6f64           for mod
+00011600: 756c 6520 696e 2073 7263 5f63 7478 5b27  ule in src_ctx['
+00011610: 756e 696e 7374 616c 6c5f 6d6f 6475 6c65  uninstall_module
+00011620: 7327 5d2e 7370 6c69 7428 272c 2729 3a0a  s'].split(','):.
+00011630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011640: 2020 2020 6472 6f70 5f6d 6f64 756c 6528      drop_module(
+00011650: 7372 635f 6374 782c 206d 6f64 756c 652c  src_ctx, module,
+00011660: 2066 6f72 6365 3d54 7275 6529 0a20 2020   force=True).   
+00011670: 2020 2020 2073 7263 5f63 7478 5b27 7372       src_ctx['sr
+00011680: 635f 6d6f 6475 6c65 5f6c 6973 7427 5d20  c_module_list'] 
+00011690: 3d20 6f64 6f6f 5f64 6570 656e 6465 6e63  = odoo_dependenc
+000116a0: 6965 7328 0a20 2020 2020 2020 2020 2020  ies(.           
+000116b0: 2073 7263 5f63 7478 2c0a 2020 2020 2020   src_ctx,.      
+000116c0: 2020 2020 2020 276d 6f64 272c 0a20 2020        'mod',.   
+000116d0: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
+000116e0: 5b27 6462 5f6e 616d 6527 5d2c 0a20 2020  ['db_name'],.   
+000116f0: 2020 2020 2020 2020 2073 7263 5f66 756c           src_ful
+00011700: 6c5f 6c63 6f6e 662c 0a20 2020 2020 2020  l_lconf,.       
+00011710: 2020 2020 2073 7263 5f70 6174 6873 2c0a       src_paths,.
+00011720: 2020 2020 2020 2020 2020 2020 7372 635f              src_
+00011730: 6374 785b 2773 7263 5f6f 646f 6f5f 6676  ctx['src_odoo_fv
+00011740: 6572 275d 2c0a 2020 2020 2020 2020 290a  er'],.        ).
+00011750: 2020 2020 2020 2020 6f73 302e 776c 6f67          os0.wlog
+00011760: 2827 4d6f 6475 6c65 206c 6973 7420 746f  ('Module list to
+00011770: 206d 6967 7261 7465 3d25 7327 2025 2073   migrate=%s' % s
+00011780: 7263 5f63 7478 5b27 7372 635f 6d6f 6475  rc_ctx['src_modu
+00011790: 6c65 5f6c 6973 7427 5d29 0a20 2020 2069  le_list']).    i
+000117a0: 6620 6e6f 7420 7372 635f 6374 782e 6765  f not src_ctx.ge
+000117b0: 7428 276f 7269 6769 6e61 6c5f 6d6f 6475  t('original_modu
+000117c0: 6c65 5f6c 6973 7427 293a 0a20 2020 2020  le_list'):.     
+000117d0: 2020 2073 7263 5f63 7478 5b27 6f72 6967     src_ctx['orig
+000117e0: 696e 616c 5f6d 6f64 756c 655f 6c69 7374  inal_module_list
+000117f0: 275d 203d 2073 7263 5f63 7478 5b27 7372  '] = src_ctx['sr
+00011800: 635f 6d6f 6475 6c65 5f6c 6973 7427 5d0a  c_module_list'].
+00011810: 2020 2020 7372 635f 616c 6c5f 6d6f 6475      src_all_modu
+00011820: 6c65 5f6c 6973 7420 3d20 6f64 6f6f 5f64  le_list = odoo_d
+00011830: 6570 656e 6465 6e63 6965 7328 0a20 2020  ependencies(.   
+00011840: 2020 2020 2073 7263 5f63 7478 2c20 276d       src_ctx, 'm
+00011850: 6f64 272c 2046 616c 7365 2c20 4661 6c73  od', False, Fals
+00011860: 652c 2073 7263 5f70 6174 6873 2c20 7372  e, src_paths, sr
+00011870: 635f 6374 785b 2773 7263 5f6f 646f 6f5f  c_ctx['src_odoo_
+00011880: 6676 6572 275d 0a20 2020 2029 0a20 2020  fver'].    ).   
+00011890: 2074 6774 5f61 6c6c 5f6d 6f64 756c 655f   tgt_all_module_
+000118a0: 6c69 7374 203d 206f 646f 6f5f 6465 7065  list = odoo_depe
+000118b0: 6e64 656e 6369 6573 280a 2020 2020 2020  ndencies(.      
+000118c0: 2020 7467 745f 6374 782c 2027 6d6f 6427    tgt_ctx, 'mod'
+000118d0: 2c20 4661 6c73 652c 2046 616c 7365 2c20  , False, False, 
+000118e0: 7467 745f 7061 7468 732c 2074 6774 5f63  tgt_paths, tgt_c
+000118f0: 7478 5b27 7467 745f 6f64 6f6f 5f66 7665  tx['tgt_odoo_fve
+00011900: 7227 5d0a 2020 2020 290a 2020 2020 7372  r'].    ).    sr
+00011910: 635f 6374 785b 2774 6e6c 5f6d 6f64 756c  c_ctx['tnl_modul
+00011920: 655f 6c69 7374 275d 2c20 6261 645f 6d6f  e_list'], bad_mo
+00011930: 6475 6c65 5f6c 6973 7420 3d20 646f 5f74  dule_list = do_t
+00011940: 6e6c 5f6d 6f64 756c 655f 6c69 7374 280a  nl_module_list(.
+00011950: 2020 2020 2020 2020 7372 635f 6374 782c          src_ctx,
+00011960: 0a20 2020 2020 2020 2073 7263 5f63 7478  .        src_ctx
+00011970: 5b27 7372 635f 6d6f 6475 6c65 5f6c 6973  ['src_module_lis
+00011980: 7427 5d2c 0a20 2020 2020 2020 2073 7263  t'],.        src
+00011990: 5f63 7478 5b27 7372 635f 6f64 6f6f 5f66  _ctx['src_odoo_f
+000119a0: 7665 7227 5d2c 0a20 2020 2020 2020 2074  ver'],.        t
+000119b0: 6774 5f63 7478 5b27 7467 745f 6f64 6f6f  gt_ctx['tgt_odoo
+000119c0: 5f66 7665 7227 5d2c 0a20 2020 2020 2020  _fver'],.       
+000119d0: 2074 6774 5f61 6c6c 5f6d 6f64 756c 655f   tgt_all_module_
+000119e0: 6c69 7374 2c0a 2020 2020 2020 2020 7075  list,.        pu
+000119f0: 7265 3d54 7275 652c 0a20 2020 2029 0a20  re=True,.    ). 
+00011a00: 2020 206f 7330 2e77 6c6f 6728 2754 7261     os0.wlog('Tra
+00011a10: 6e73 6c61 7465 6420 6c69 7374 2061 6674  nslated list aft
+00011a20: 6572 206d 6967 7261 7469 6f6e 3d25 7327  er migration=%s'
+00011a30: 2025 2073 7263 5f63 7478 5b27 746e 6c5f   % src_ctx['tnl_
+00011a40: 6d6f 6475 6c65 5f6c 6973 7427 5d29 0a20  module_list']). 
+00011a50: 2020 2066 756c 6c5f 746e 6c5f 6d6f 6475     full_tnl_modu
+00011a60: 6c65 5f6c 6973 7420 3d20 6f64 6f6f 5f64  le_list = odoo_d
+00011a70: 6570 656e 6465 6e63 6965 7328 0a20 2020  ependencies(.   
+00011a80: 2020 2020 2074 6774 5f63 7478 2c0a 2020       tgt_ctx,.  
+00011a90: 2020 2020 2020 2764 6570 272c 0a20 2020        'dep',.   
+00011aa0: 2020 2020 2046 616c 7365 2c0a 2020 2020       False,.    
+00011ab0: 2020 2020 4661 6c73 652c 0a20 2020 2020      False,.     
+00011ac0: 2020 2074 6774 5f70 6174 6873 2c0a 2020     tgt_paths,.  
+00011ad0: 2020 2020 2020 7467 745f 6374 785b 2773        tgt_ctx['s
+00011ae0: 7263 5f6f 646f 6f5f 6676 6572 275d 2c0a  rc_odoo_fver'],.
+00011af0: 2020 2020 2020 2020 6d61 7463 6865 733d          matches=
+00011b00: 7372 635f 6374 785b 2774 6e6c 5f6d 6f64  src_ctx['tnl_mod
+00011b10: 756c 655f 6c69 7374 275d 2c0a 2020 2020  ule_list'],.    
+00011b20: 290a 2020 2020 6f73 302e 776c 6f67 2827  ).    os0.wlog('
+00011b30: 5461 7267 6574 206c 6973 7420 7769 7468  Target list with
+00011b40: 2064 6570 656e 6465 6e63 6965 733d 2573   dependencies=%s
+00011b50: 2720 2520 6675 6c6c 5f74 6e6c 5f6d 6f64  ' % full_tnl_mod
+00011b60: 756c 655f 6c69 7374 290a 2020 2020 6f73  ule_list).    os
+00011b70: 302e 776c 6f67 2827 4e6f 7420 6176 6169  0.wlog('Not avai
+00011b80: 6162 6c65 206d 6f64 756c 6573 206f 6e20  able modules on 
+00011b90: 7461 7267 6574 3d25 7327 2025 2062 6164  target=%s' % bad
+00011ba0: 5f6d 6f64 756c 655f 6c69 7374 290a 2020  _module_list).  
+00011bb0: 2020 6966 2062 6164 5f6d 6f64 756c 655f    if bad_module_
+00011bc0: 6c69 7374 2061 6e64 2073 7263 5f63 7478  list and src_ctx
+00011bd0: 5b27 7265 6475 6374 6564 5f6d 6f64 756c  ['reducted_modul
+00011be0: 655f 7365 7427 5d20 616e 6420 6e6f 7420  e_set'] and not 
+00011bf0: 7372 635f 6374 785b 2764 7279 5f72 756e  src_ctx['dry_run
+00011c00: 275d 3a0a 2020 2020 2020 2020 666f 7220  ']:.        for 
+00011c10: 692c 206d 6f64 756c 6520 696e 2065 6e75  i, module in enu
+00011c20: 6d65 7261 7465 2862 6164 5f6d 6f64 756c  merate(bad_modul
+00011c30: 655f 6c69 7374 293a 0a20 2020 2020 2020  e_list):.       
+00011c40: 2020 2020 2073 7473 203d 2064 726f 705f       sts = drop_
+00011c50: 6d6f 6475 6c65 2873 7263 5f63 7478 2c20  module(src_ctx, 
+00011c60: 6d6f 6475 6c65 290a 2020 2020 2020 2020  module).        
+00011c70: 2020 2020 6966 2073 7473 3a0a 2020 2020      if sts:.    
+00011c80: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
+00011c90: 6261 645f 6d6f 6475 6c65 5f6c 6973 745b  bad_module_list[
+00011ca0: 695d 0a20 2020 2073 6f66 745f 756e 696e  i].    soft_unin
+00011cb0: 7374 616c 6c5f 6c69 7374 203d 2068 6172  stall_list = har
+00011cc0: 645f 756e 696e 7374 616c 6c5f 6c69 7374  d_uninstall_list
+00011cd0: 203d 205b 5d0a 2020 2020 6966 2074 6774   = [].    if tgt
+00011ce0: 5f63 7478 5b27 6f63 615f 6d69 6772 6174  _ctx['oca_migrat
+00011cf0: 6527 5d20 616e 6420 7467 745f 6374 785b  e'] and tgt_ctx[
+00011d00: 2774 6774 5f6f 646f 6f5f 7665 7227 5d20  'tgt_odoo_ver'] 
+00011d10: 3c20 3130 3a0a 2020 2020 2020 2020 6f75  < 10:.        ou
+00011d20: 5f76 6572 5f70 6174 6820 3d20 6c6f 6164  _ver_path = load
+00011d30: 5f6f 7065 6e75 7067 7261 6465 2874 6774  _openupgrade(tgt
+00011d40: 5f63 7478 2c20 7467 745f 6374 785b 2774  _ctx, tgt_ctx['t
+00011d50: 6774 5f6f 646f 6f5f 6676 6572 275d 290a  gt_odoo_fver']).
+00011d60: 2020 2020 2020 2020 636d 6420 3d20 6f73          cmd = os
+00011d70: 2e70 6174 682e 6a6f 696e 286f 755f 7665  .path.join(ou_ve
+00011d80: 725f 7061 7468 2c20 2773 6372 6970 7473  r_path, 'scripts
+00011d90: 272c 2027 6d69 6772 6174 652e 7079 2729  ', 'migrate.py')
+00011da0: 0a20 2020 2020 2020 2069 6620 7372 635f  .        if src_
+00011db0: 6374 785b 276e 6f5f 7665 6e76 275d 3a0a  ctx['no_venv']:.
+00011dc0: 2020 2020 2020 2020 2020 2020 7275 6e5f              run_
+00011dd0: 7472 6163 6564 280a 2020 2020 2020 2020  traced(.        
+00011de0: 2020 2020 2020 2020 636d 642c 0a20 2020          cmd,.   
+00011df0: 2020 2020 2020 2020 2020 2020 2027 2d43               '-C
+00011e00: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00011e10: 2020 2073 7263 5f66 756c 6c5f 6c63 6f6e     src_full_lcon
+00011e20: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+00011e30: 2020 2027 2d44 272c 0a20 2020 2020 2020     '-D',.       
+00011e40: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
+00011e50: 5b27 6462 5f6e 616d 6527 5d2c 0a20 2020  ['db_name'],.   
+00011e60: 2020 2020 2020 2020 2020 2020 2027 2d42               '-B
+00011e70: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00011e80: 2020 2073 7263 5f63 7478 5b27 6f70 745f     src_ctx['opt_
+00011e90: 6f75 7061 7468 275d 2c0a 2020 2020 2020  oupath'],.      
+00011ea0: 2020 2020 2020 2020 2020 272d 5227 2c0a            '-R',.
+00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ec0: 7467 745f 6374 785b 2774 6774 5f6f 646f  tgt_ctx['tgt_odo
+00011ed0: 6f5f 6676 6572 275d 2c0a 2020 2020 2020  o_fver'],.      
+00011ee0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00011ef0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00011f00: 2020 7363 7269 7074 203d 206f 732e 7061    script = os.pa
+00011f10: 7468 2e6a 6f69 6e28 6f75 5f76 6572 5f70  th.join(ou_ver_p
+00011f20: 6174 682c 2027 6d69 6772 6174 652e 7368  ath, 'migrate.sh
+00011f30: 2729 0a20 2020 2020 2020 2020 2020 2066  ').            f
+00011f40: 6420 3d20 6f70 656e 2873 6372 6970 742c  d = open(script,
+00011f50: 2027 7727 290a 2020 2020 2020 2020 2020   'w').          
+00011f60: 2020 6664 2e77 7269 7465 2827 6364 2025    fd.write('cd %
+00011f70: 735c 6e27 2025 2074 6774 5f63 7478 5b27  s\n' % tgt_ctx['
+00011f80: 7665 6e76 5f6f 7570 6174 6827 5d29 0a20  venv_oupath']). 
+00011f90: 2020 2020 2020 2020 2020 2066 642e 7772             fd.wr
+00011fa0: 6974 6528 2773 6f75 7263 6520 2e2f 6269  ite('source ./bi
+00011fb0: 6e2f 6163 7469 7661 7465 5c6e 2729 0a20  n/activate\n'). 
+00011fc0: 2020 2020 2020 2020 2020 2066 642e 7772             fd.wr
+00011fd0: 6974 6528 0a20 2020 2020 2020 2020 2020  ite(.           
+00011fe0: 2020 2020 2027 2573 202d 4320 2573 202d       '%s -C %s -
+00011ff0: 4420 2573 202d 4220 2573 202d 5220 2573  D %s -B %s -R %s
+00012000: 5c6e 270a 2020 2020 2020 2020 2020 2020  \n'.            
+00012010: 2020 2020 2520 280a 2020 2020 2020 2020      % (.        
+00012020: 2020 2020 2020 2020 2020 2020 636d 642c              cmd,
+00012030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012040: 2020 2020 2073 7263 5f66 756c 6c5f 6c63       src_full_lc
+00012050: 6f6e 662c 0a20 2020 2020 2020 2020 2020  onf,.           
+00012060: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
+00012070: 5b27 6462 5f6e 616d 6527 5d2c 0a20 2020  ['db_name'],.   
+00012080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012090: 2073 7263 5f63 7478 5b27 6f70 745f 6f75   src_ctx['opt_ou
+000120a0: 7061 7468 275d 2c0a 2020 2020 2020 2020  path'],.        
+000120b0: 2020 2020 2020 2020 2020 2020 7467 745f              tgt_
+000120c0: 6374 785b 2774 6774 5f6f 646f 6f5f 6676  ctx['tgt_odoo_fv
+000120d0: 6572 275d 2c0a 2020 2020 2020 2020 2020  er'],.          
+000120e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000120f0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00012100: 2020 6664 2e77 7269 7465 2827 6465 6163    fd.write('deac
+00012110: 7469 7661 7465 5c6e 2729 0a20 2020 2020  tivate\n').     
+00012120: 2020 2020 2020 2066 642e 636c 6f73 6528         fd.close(
+00012130: 290a 2020 2020 2020 2020 2020 2020 6f73  ).            os
+00012140: 2e63 686d 6f64 2873 6372 6970 742c 2030  .chmod(script, 0
+00012150: 6f37 3434 290a 2020 2020 2020 2020 2020  o744).          
+00012160: 2020 6966 206e 6f74 2073 7263 5f63 7478    if not src_ctx
+00012170: 5b27 6472 795f 7275 6e27 5d3a 0a20 2020  ['dry_run']:.   
+00012180: 2020 2020 2020 2020 2020 2020 206f 732e               os.
+00012190: 7379 7374 656d 2873 6372 6970 7429 0a20  system(script). 
+000121a0: 2020 2020 2020 2069 6620 6e6f 7420 7372         if not sr
+000121b0: 635f 6374 785b 2764 7279 5f72 756e 275d  c_ctx['dry_run']
+000121c0: 3a0a 2020 2020 2020 2020 2020 2020 7469  :.            ti
+000121d0: 6d65 2e73 6c65 6570 2835 290a 2020 2020  me.sleep(5).    
+000121e0: 2020 2020 746d 705f 6462 6e61 6d65 203d      tmp_dbname =
+000121f0: 206e 6577 5f64 626e 616d 6528 0a20 2020   new_dbname(.   
+00012200: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
+00012210: 5b27 6462 5f6e 616d 6527 5d2c 2074 6774  ['db_name'], tgt
+00012220: 5f63 7478 5b27 7467 745f 6f64 6f6f 5f76  _ctx['tgt_odoo_v
+00012230: 6572 275d 2c20 7467 745f 6374 785b 276f  er'], tgt_ctx['o
+00012240: 6361 5f6d 6967 7261 7465 275d 0a20 2020  ca_migrate'].   
+00012250: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+00012260: 6620 6e6f 7420 7372 635f 6374 785b 2764  f not src_ctx['d
+00012270: 7279 5f72 756e 275d 3a0a 2020 2020 2020  ry_run']:.      
+00012280: 2020 2020 2020 6966 2074 6774 5f63 7478        if tgt_ctx
+00012290: 5b27 6462 5f6e 616d 6527 5d20 213d 2074  ['db_name'] != t
+000122a0: 6d70 5f64 626e 616d 653a 0a20 2020 2020  mp_dbname:.     
+000122b0: 2020 2020 2020 2020 2020 2072 656e 5f64             ren_d
+000122c0: 6228 746d 705f 6462 6e61 6d65 2c20 7467  b(tmp_dbname, tg
+000122d0: 745f 6374 785b 2764 625f 6e61 6d65 275d  t_ctx['db_name']
+000122e0: 2c20 7372 635f 6374 785b 2764 625f 7573  , src_ctx['db_us
+000122f0: 6572 275d 290a 2020 2020 2020 2020 2020  er']).          
+00012300: 2020 6966 2073 7263 5f63 7478 5b27 6462    if src_ctx['db
+00012310: 5f75 7365 7227 5d20 213d 2074 6774 5f63  _user'] != tgt_c
+00012320: 7478 5b27 6462 5f75 7365 7227 5d3a 0a20  tx['db_user']:. 
+00012330: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00012340: 6561 7373 6967 6e5f 6462 5f6f 776e 6572  eassign_db_owner
+00012350: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00012360: 2020 2020 2020 7467 745f 6374 782c 2074        tgt_ctx, t
+00012370: 6774 5f63 7478 5b27 6462 5f6e 616d 6527  gt_ctx['db_name'
+00012380: 5d2c 2073 7263 5f63 7478 5b27 6462 5f75  ], src_ctx['db_u
+00012390: 7365 7227 5d2c 2074 6774 5f63 7478 5b27  ser'], tgt_ctx['
+000123a0: 6462 5f75 7365 7227 5d0a 2020 2020 2020  db_user'].      
+000123b0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000123c0: 2020 2020 7467 745f 6675 6c6c 5f6c 636f      tgt_full_lco
+000123d0: 6e66 203d 2074 6774 5f63 7478 5b27 636f  nf = tgt_ctx['co
+000123e0: 6e66 5f66 6e27 5d0a 2020 2020 656c 7365  nf_fn'].    else
+000123f0: 3a0a 2020 2020 2020 2020 6f75 5f76 6572  :.        ou_ver
+00012400: 5f70 6174 6820 3d20 6c6f 6164 5f6f 7065  _path = load_ope
+00012410: 6e75 7067 7261 6465 2874 6774 5f63 7478  nupgrade(tgt_ctx
+00012420: 2c20 7467 745f 6374 785b 2774 6774 5f6f  , tgt_ctx['tgt_o
+00012430: 646f 6f5f 6676 6572 275d 290a 2020 2020  doo_fver']).    
+00012440: 2020 2020 6966 206e 6f74 2073 7263 5f63      if not src_c
+00012450: 7478 5b27 6472 795f 7275 6e27 5d3a 0a20  tx['dry_run']:. 
+00012460: 2020 2020 2020 2020 2020 206c 6f61 645f             load_
+00012470: 6f70 656e 7570 6772 6164 656c 6962 2873  openupgradelib(s
+00012480: 7263 5f63 7478 2c20 7467 745f 6374 785b  rc_ctx, tgt_ctx[
+00012490: 2774 6774 5f6f 646f 6f5f 6676 6572 275d  'tgt_odoo_fver']
+000124a0: 290a 2020 2020 2020 2020 6966 2074 6774  ).        if tgt
+000124b0: 5f63 7478 5b27 7570 645f 7472 616e 736c  _ctx['upd_transl
+000124c0: 6174 696f 6e27 5d3a 0a20 2020 2020 2020  ation']:.       
+000124d0: 2020 2020 2061 6464 5f76 6572 7369 6f6e       add_version
+000124e0: 6564 5f74 6e6c 280a 2020 2020 2020 2020  ed_tnl(.        
+000124f0: 2020 2020 2020 2020 7372 635f 6374 782c          src_ctx,
+00012500: 2073 7263 5f63 7478 5b27 7372 635f 6f64   src_ctx['src_od
+00012510: 6f6f 5f66 7665 7227 5d2c 2074 6774 5f63  oo_fver'], tgt_c
+00012520: 7478 5b27 7467 745f 6f64 6f6f 5f66 7665  tx['tgt_odoo_fve
+00012530: 7227 5d0a 2020 2020 2020 2020 2020 2020  r'].            
+00012540: 290a 2020 2020 2020 2020 6164 646f 6e73  ).        addons
+00012550: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
+00012560: 6a6f 696e 286f 755f 7665 725f 7061 7468  join(ou_ver_path
+00012570: 2c20 2761 6464 6f6e 7327 290a 2020 2020  , 'addons').    
+00012580: 2020 2020 6966 2074 6774 5f63 7478 5b27      if tgt_ctx['
+00012590: 7467 745f 6f64 6f6f 5f76 6572 275d 203c  tgt_odoo_ver'] <
+000125a0: 2031 303a 0a20 2020 2020 2020 2020 2020   10:.           
+000125b0: 2072 6f6f 745f 7061 7468 203d 206f 732e   root_path = os.
+000125c0: 7061 7468 2e6a 6f69 6e28 6f75 5f76 6572  path.join(ou_ver
+000125d0: 5f70 6174 682c 2027 6f70 656e 6572 7027  _path, 'openerp'
+000125e0: 2c20 2761 6464 6f6e 7327 290a 2020 2020  , 'addons').    
+000125f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00012600: 2020 2020 2020 726f 6f74 5f70 6174 6820        root_path 
+00012610: 3d20 6f73 2e70 6174 682e 6a6f 696e 286f  = os.path.join(o
+00012620: 755f 7665 725f 7061 7468 2c20 276f 646f  u_ver_path, 'odo
+00012630: 6f27 2c20 2761 6464 6f6e 7327 290a 2020  o', 'addons').  
+00012640: 2020 2020 2020 6966 206e 6f74 2073 7263        if not src
+00012650: 5f63 7478 5b27 6472 795f 7275 6e27 5d3a  _ctx['dry_run']:
+00012660: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00012670: 2072 6570 6f20 696e 2074 6774 5f70 6174   repo in tgt_pat
+00012680: 6873 3a0a 2020 2020 2020 2020 2020 2020  hs:.            
+00012690: 2020 2020 666f 7220 6e61 6d65 2069 6e20      for name in 
+000126a0: 6f73 2e6c 6973 7464 6972 2872 6570 6f29  os.listdir(repo)
+000126b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000126c0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+000126d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126e0: 2020 206f 732e 7061 7468 2e69 7364 6972     os.path.isdir
+000126f0: 286f 732e 7061 7468 2e6a 6f69 6e28 7265  (os.path.join(re
+00012700: 706f 2c20 6e61 6d65 2929 0a20 2020 2020  po, name)).     
+00012710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012720: 2020 2061 6e64 206e 6f74 206f 732e 7061     and not os.pa
+00012730: 7468 2e69 7364 6972 286f 732e 7061 7468  th.isdir(os.path
+00012740: 2e6a 6f69 6e28 6164 646f 6e73 5f70 6174  .join(addons_pat
+00012750: 682c 206e 616d 6529 290a 2020 2020 2020  h, name)).      
+00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012770: 2020 616e 6420 6e6f 7420 6f73 2e70 6174    and not os.pat
+00012780: 682e 6973 6469 7228 6f73 2e70 6174 682e  h.isdir(os.path.
+00012790: 6a6f 696e 2872 6f6f 745f 7061 7468 2c20  join(root_path, 
+000127a0: 6e61 6d65 2929 0a20 2020 2020 2020 2020  name)).         
+000127b0: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
+000127c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127d0: 2020 2020 2020 6f73 2e73 796d 6c69 6e6b        os.symlink
+000127e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000127f0: 2020 2020 2020 2020 2020 2020 2020 6f73                os
+00012800: 2e70 6174 682e 6a6f 696e 2872 6570 6f2c  .path.join(repo,
+00012810: 206e 616d 6529 2c20 6f73 2e70 6174 682e   name), os.path.
+00012820: 6a6f 696e 2861 6464 6f6e 735f 7061 7468  join(addons_path
+00012830: 2c20 6e61 6d65 290a 2020 2020 2020 2020  , name).        
+00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012850: 290a 2020 2020 2020 2020 7467 745f 7061  ).        tgt_pa
+00012860: 7468 7320 3d20 5b5d 0a20 2020 2020 2020  ths = [].       
+00012870: 2074 6774 5f70 6174 6873 2e69 6e73 6572   tgt_paths.inser
+00012880: 7428 302c 2061 6464 6f6e 735f 7061 7468  t(0, addons_path
+00012890: 290a 2020 2020 2020 2020 7467 745f 7061  ).        tgt_pa
+000128a0: 7468 732e 696e 7365 7274 2830 2c20 726f  ths.insert(0, ro
+000128b0: 6f74 5f70 6174 6829 0a20 2020 2020 2020  ot_path).       
+000128c0: 2074 6774 5f66 756c 6c5f 6c63 6f6e 6620   tgt_full_lconf 
+000128d0: 3d20 7072 6570 6172 655f 636f 6e66 6967  = prepare_config
+000128e0: 5f66 696c 6528 0a20 2020 2020 2020 2020  _file(.         
+000128f0: 2020 2074 6774 5f63 7478 2c20 7467 745f     tgt_ctx, tgt_
+00012900: 636f 6e66 6967 2c20 6f75 5f76 6572 5f70  config, ou_ver_p
+00012910: 6174 683d 6f75 5f76 6572 5f70 6174 682c  ath=ou_ver_path,
+00012920: 2070 6174 6873 3d74 6774 5f70 6174 6873   paths=tgt_paths
+00012930: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00012940: 2020 2069 6620 6e6f 7420 7372 635f 6374     if not src_ct
+00012950: 785b 2764 7279 5f72 756e 275d 3a0a 2020  x['dry_run']:.  
+00012960: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00012970: 2063 6f70 795f 6462 2873 7263 5f63 7478   copy_db(src_ctx
+00012980: 2c20 7372 635f 6374 785b 2764 625f 6e61  , src_ctx['db_na
+00012990: 6d65 275d 2c20 7467 745f 6374 785b 2764  me'], tgt_ctx['d
+000129a0: 625f 6e61 6d65 275d 293a 0a20 2020 2020  b_name']):.     
+000129b0: 2020 2020 2020 2020 2020 2065 7869 7428             exit(
+000129c0: 3129 0a20 2020 2020 2020 2020 2020 2066  1).            f
+000129d0: 6978 5f62 7567 5f70 7265 2873 7263 5f63  ix_bug_pre(src_c
+000129e0: 7478 2c20 7467 745f 6374 782c 2073 7263  tx, tgt_ctx, src
+000129f0: 5f66 756c 6c5f 6c63 6f6e 662c 2073 7263  _full_lconf, src
+00012a00: 5f70 6174 6873 290a 2020 2020 2020 2020  _paths).        
+00012a10: 2020 2020 6966 2073 7263 5f63 7478 5b27      if src_ctx['
+00012a20: 6462 5f75 7365 7227 5d20 213d 2074 6774  db_user'] != tgt
+00012a30: 5f63 7478 5b27 6462 5f75 7365 7227 5d3a  _ctx['db_user']:
+00012a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012a50: 2072 6561 7373 6967 6e5f 6462 5f6f 776e   reassign_db_own
+00012a60: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
+00012a70: 2020 2020 2020 2020 7467 745f 6374 782c          tgt_ctx,
+00012a80: 2074 6774 5f63 7478 5b27 6462 5f6e 616d   tgt_ctx['db_nam
+00012a90: 6527 5d2c 2073 7263 5f63 7478 5b27 6462  e'], src_ctx['db
+00012aa0: 5f75 7365 7227 5d2c 2074 6774 5f63 7478  _user'], tgt_ctx
+00012ab0: 5b27 6462 5f75 7365 7227 5d0a 2020 2020  ['db_user'].    
+00012ac0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00012ad0: 2020 2020 2020 2020 2020 2320 536f 6d65            # Some
+00012ae0: 206d 6f64 756c 6573 206e 6f74 2061 7661   modules not ava
+00012af0: 696c 6162 6c65 206f 6e20 696e 7465 726d  ilable on interm
+00012b00: 6564 6961 7465 2076 6572 7369 6f6e 206d  ediate version m
+00012b10: 6967 6874 2062 650a 2020 2020 2020 2020  ight be.        
+00012b20: 2020 2020 2320 6176 6169 6c61 626c 6520      # available 
+00012b30: 6f6e 2063 7572 7265 6e74 2074 6172 6765  on current targe
+00012b40: 7420 6f64 6f6f 2076 6572 7369 6f6e 0a20  t odoo version. 
+00012b50: 2020 2020 2020 2020 2020 2069 6620 7467             if tg
+00012b60: 745f 6374 785b 2774 7279 5f72 6569 6e73  t_ctx['try_reins
+00012b70: 7461 6c6c 275d 3a0a 2020 2020 2020 2020  tall']:.        
+00012b80: 2020 2020 2020 2020 6d6f 6475 6c65 735f          modules_
+00012b90: 746f 5f72 6573 746f 7265 203d 2062 6164  to_restore = bad
+00012ba0: 5f6c 6973 7420 3d20 5b5d 0a20 2020 2020  _list = [].     
+00012bb0: 2020 2020 2020 2020 2020 2069 6620 7372             if sr
+00012bc0: 635f 6374 785b 276f 7269 6769 6e61 6c5f  c_ctx['original_
+00012bd0: 6d6f 6475 6c65 5f6c 6973 7427 5d20 213d  module_list'] !=
+00012be0: 2073 7263 5f63 7478 5b27 7372 635f 6d6f   src_ctx['src_mo
+00012bf0: 6475 6c65 5f6c 6973 7427 5d3a 0a20 2020  dule_list']:.   
+00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c10: 206d 6f64 756c 6573 5f74 6f5f 7265 7374   modules_to_rest
+00012c20: 6f72 652c 2062 6164 5f6c 6973 7420 3d20  ore, bad_list = 
+00012c30: 646f 5f74 6e6c 5f6d 6f64 756c 655f 6c69  do_tnl_module_li
+00012c40: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
+00012c50: 2020 2020 2020 2020 2020 2020 7467 745f              tgt_
+00012c60: 6374 782c 0a20 2020 2020 2020 2020 2020  ctx,.           
+00012c70: 2020 2020 2020 2020 2020 2020 2073 7263               src
+00012c80: 5f63 7478 5b27 6f72 6967 696e 616c 5f6d  _ctx['original_m
+00012c90: 6f64 756c 655f 6c69 7374 275d 2c0a 2020  odule_list'],.  
+00012ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cb0: 2020 2020 2020 7372 635f 6374 785b 2766        src_ctx['f
+00012cc0: 726f 6d5f 6f64 6f6f 5f66 7665 7227 5d2c  rom_odoo_fver'],
+00012cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012ce0: 2020 2020 2020 2020 2074 6774 5f63 7478           tgt_ctx
+00012cf0: 5b27 7467 745f 6f64 6f6f 5f66 7665 7227  ['tgt_odoo_fver'
+00012d00: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00012d10: 2020 2020 2020 2020 2020 2074 6774 5f61             tgt_a
+00012d20: 6c6c 5f6d 6f64 756c 655f 6c69 7374 2c0a  ll_module_list,.
+00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d40: 2020 2020 2020 2020 7075 7265 3d54 7275          pure=Tru
+00012d50: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00012d60: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00012d70: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+00012d80: 756c 6573 5f74 6f5f 7265 7374 6f72 6520  ules_to_restore 
+00012d90: 3d20 6c69 7374 280a 2020 2020 2020 2020  = list(.        
+00012da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012db0: 7365 7428 6d6f 6475 6c65 735f 746f 5f72  set(modules_to_r
+00012dc0: 6573 746f 7265 2920 2d20 7365 7428 7372  estore) - set(sr
+00012dd0: 635f 6374 785b 2773 7263 5f6d 6f64 756c  c_ctx['src_modul
+00012de0: 655f 6c69 7374 275d 290a 2020 2020 2020  e_list']).      
+00012df0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e10: 2020 2020 6966 206d 6f64 756c 6573 5f74      if modules_t
+00012e20: 6f5f 7265 7374 6f72 653a 0a20 2020 2020  o_restore:.     
+00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e40: 2020 2073 6574 5f69 6e73 7461 6c6c 6564     set_installed
+00012e50: 5f62 795f 7371 6c28 7467 745f 6374 782c  _by_sql(tgt_ctx,
+00012e60: 206d 6f64 756c 6573 5f74 6f5f 7265 7374   modules_to_rest
+00012e70: 6f72 6529 0a20 2020 2020 2020 2020 2020  ore).           
+00012e80: 2064 726f 705f 7365 7373 696f 6e28 7467   drop_session(tg
+00012e90: 745f 6374 782c 2074 6774 5f63 7478 5b27  t_ctx, tgt_ctx['
+00012ea0: 6462 5f6e 616d 6527 5d2c 206f 646f 6f5f  db_name'], odoo_
+00012eb0: 7669 643d 7467 745f 6374 785b 2774 6774  vid=tgt_ctx['tgt
+00012ec0: 5f76 6964 275d 290a 2020 2020 2020 2020  _vid']).        
+00012ed0: 7275 6e5f 6f70 656e 7570 6772 6164 6528  run_openupgrade(
+00012ee0: 7467 745f 6374 782c 206f 755f 7665 725f  tgt_ctx, ou_ver_
+00012ef0: 7061 7468 2c20 7467 745f 6675 6c6c 5f6c  path, tgt_full_l
+00012f00: 636f 6e66 290a 2020 2020 2020 2020 6966  conf).        if
+00012f10: 206e 6f74 2073 7263 5f63 7478 5b27 6472   not src_ctx['dr
+00012f20: 795f 7275 6e27 5d3a 0a20 2020 2020 2020  y_run']:.       
+00012f30: 2020 2020 2066 6978 5f62 7567 5f70 6f73       fix_bug_pos
+00012f40: 7428 7372 635f 6374 782c 2074 6774 5f63  t(src_ctx, tgt_c
+00012f50: 7478 2c20 7372 635f 6675 6c6c 5f6c 636f  tx, src_full_lco
+00012f60: 6e66 2c20 7372 635f 7061 7468 7329 0a0a  nf, src_paths)..
+00012f70: 2020 2020 2320 5465 7374 2066 6f72 206e      # Test for n
+00012f80: 6f74 206d 6967 7261 7465 6420 6d6f 6475  ot migrated modu
+00012f90: 6c65 730a 2020 2020 7467 745f 6374 785b  les.    tgt_ctx[
+00012fa0: 2763 6f6e 665f 666e 275d 203d 2074 6774  'conf_fn'] = tgt
+00012fb0: 5f73 6176 6564 5f66 636f 6e66 0a20 2020  _saved_fconf.   
+00012fc0: 2074 6f5f 756e 696e 7374 616c 6c5f 6c69   to_uninstall_li
+00012fd0: 7374 203d 2067 6574 5f77 726f 6e67 5f6d  st = get_wrong_m
+00012fe0: 6f64 756c 6573 2874 6774 5f63 7478 290a  odules(tgt_ctx).
+00012ff0: 2020 2020 6966 2074 6f5f 756e 696e 7374      if to_uninst
+00013000: 616c 6c5f 6c69 7374 3a0a 2020 2020 2020  all_list:.      
+00013010: 2020 6f73 302e 776c 6f67 2827 2a2a 2a20    os0.wlog('*** 
+00013020: 5772 6f6e 6720 7374 6174 6520 666f 7220  Wrong state for 
+00013030: 6d6f 6475 6c65 7320 2573 202a 2a2a 2720  modules %s ***' 
+00013040: 2520 746f 5f75 6e69 6e73 7461 6c6c 5f6c  % to_uninstall_l
+00013050: 6973 7429 0a20 2020 2068 6172 645f 756e  ist).    hard_un
+00013060: 696e 7374 616c 6c5f 6c69 7374 203d 206c  install_list = l
+00013070: 6973 7428 7365 7428 746f 5f75 6e69 6e73  ist(set(to_unins
+00013080: 7461 6c6c 5f6c 6973 7429 2026 2073 6574  tall_list) & set
+00013090: 284d 4f44 554c 4553 5f32 5f4c 4541 5645  (MODULES_2_LEAVE
+000130a0: 5f42 4548 494e 4429 290a 2020 2020 736f  _BEHIND)).    so
+000130b0: 6674 5f75 6e69 6e73 7461 6c6c 5f6c 6973  ft_uninstall_lis
+000130c0: 7420 3d20 6c69 7374 2873 6574 2874 6f5f  t = list(set(to_
+000130d0: 756e 696e 7374 616c 6c5f 6c69 7374 2920  uninstall_list) 
+000130e0: 2d20 7365 7428 6861 7264 5f75 6e69 6e73  - set(hard_unins
+000130f0: 7461 6c6c 5f6c 6973 7429 290a 2020 2020  tall_list)).    
+00013100: 6966 2073 6f66 745f 756e 696e 7374 616c  if soft_uninstal
+00013110: 6c5f 6c69 7374 3a0a 2020 2020 2020 2020  l_list:.        
+00013120: 7365 745f 756e 696e 7374 616c 6c65 645f  set_uninstalled_
+00013130: 6279 5f73 716c 2874 6774 5f63 7478 2c20  by_sql(tgt_ctx, 
+00013140: 736f 6674 5f75 6e69 6e73 7461 6c6c 5f6c  soft_uninstall_l
+00013150: 6973 7429 0a20 2020 2069 6620 6861 7264  ist).    if hard
+00013160: 5f75 6e69 6e73 7461 6c6c 5f6c 6973 743a  _uninstall_list:
+00013170: 0a20 2020 2020 2020 206f 7330 2e77 6c6f  .        os0.wlo
+00013180: 6728 272a 2a2a 2055 6e73 7461 626c 6520  g('*** Unstable 
+00013190: 4442 3a20 7772 6f6e 6720 6d6f 6475 6c65  DB: wrong module
+000131a0: 2073 7461 7465 2025 7320 2a2a 2a27 2025   state %s ***' %
+000131b0: 2068 6172 645f 756e 696e 7374 616c 6c5f   hard_uninstall_
+000131c0: 6c69 7374 290a 2020 2020 666f 7220 6d6f  list).    for mo
+000131d0: 6475 6c65 2069 6e20 6861 7264 5f75 6e69  dule in hard_uni
+000131e0: 6e73 7461 6c6c 5f6c 6973 743a 0a20 2020  nstall_list:.   
+000131f0: 2020 2020 206f 7330 2e77 6c6f 6728 2720       os0.wlog(' 
+00013200: 202b 2b20 4861 7264 2075 6e69 6e73 7461   ++ Hard uninsta
+00013210: 6c6c 3a20 2573 2720 2520 6d6f 6475 6c65  ll: %s' % module
+00013220: 290a 2020 2020 2020 2020 6861 7264 5f63  ).        hard_c
+00013230: 6c65 616e 5f6d 6f64 756c 6528 7467 745f  lean_module(tgt_
+00013240: 6374 782c 206d 6f64 756c 6529 0a20 2020  ctx, module).   
+00013250: 2069 6620 736f 6674 5f75 6e69 6e73 7461   if soft_uninsta
+00013260: 6c6c 5f6c 6973 7420 6f72 2068 6172 645f  ll_list or hard_
+00013270: 756e 696e 7374 616c 6c5f 6c69 7374 3a0a  uninstall_list:.
+00013280: 2020 2020 2020 2020 6261 645f 6d6f 6475          bad_modu
+00013290: 6c65 7320 3d20 6c69 7374 2873 6574 2873  les = list(set(s
+000132a0: 6f66 745f 756e 696e 7374 616c 6c5f 6c69  oft_uninstall_li
+000132b0: 7374 2920 7c20 7365 7428 6861 7264 5f75  st) | set(hard_u
+000132c0: 6e69 6e73 7461 6c6c 5f6c 6973 7429 290a  ninstall_list)).
+000132d0: 2020 2020 2020 2020 7275 6e5f 6f64 6f6f          run_odoo
+000132e0: 5f61 6c6c 7465 7374 280a 2020 2020 2020  _alltest(.      
+000132f0: 2020 2020 2020 7467 745f 6374 785b 2774        tgt_ctx['t
+00013300: 6774 5f76 6964 275d 2c0a 2020 2020 2020  gt_vid'],.      
+00013310: 2020 2020 2020 7467 745f 6374 785b 2763        tgt_ctx['c
+00013320: 6f6e 665f 666e 275d 2c0a 2020 2020 2020  onf_fn'],.      
+00013330: 2020 2020 2020 7467 745f 6374 785b 2764        tgt_ctx['d
+00013340: 625f 6e61 6d65 275d 2c0a 2020 2020 2020  b_name'],.      
+00013350: 2020 2020 2020 7467 745f 6374 785b 276c        tgt_ctx['l
+00013360: 6f67 6669 6c65 275d 2c0a 2020 2020 2020  ogfile'],.      
+00013370: 2020 2020 2020 6d6f 6475 6c65 733d 6261        modules=ba
+00013380: 645f 6d6f 6475 6c65 732c 0a20 2020 2020  d_modules,.     
+00013390: 2020 2029 0a20 2020 2065 6c69 6620 7467     ).    elif tg
+000133a0: 745f 6374 785b 276f 7074 5f73 6166 6527  t_ctx['opt_safe'
+000133b0: 5d20 616e 6420 6e6f 7420 7372 635f 6374  ] and not src_ct
+000133c0: 785b 2764 7279 5f72 756e 275d 3a0a 2020  x['dry_run']:.  
+000133d0: 2020 2020 2020 7275 6e5f 6f64 6f6f 5f61        run_odoo_a
+000133e0: 6c6c 7465 7374 280a 2020 2020 2020 2020  lltest(.        
+000133f0: 2020 2020 7467 745f 6374 785b 2774 6774      tgt_ctx['tgt
+00013400: 5f76 6964 275d 2c0a 2020 2020 2020 2020  _vid'],.        
+00013410: 2020 2020 7467 745f 6374 785b 2763 6f6e      tgt_ctx['con
+00013420: 665f 666e 275d 2c0a 2020 2020 2020 2020  f_fn'],.        
+00013430: 2020 2020 7467 745f 6374 785b 2764 625f      tgt_ctx['db_
+00013440: 6e61 6d65 275d 2c0a 2020 2020 2020 2020  name'],.        
+00013450: 2020 2020 7467 745f 6374 785b 276c 6f67      tgt_ctx['log
+00013460: 6669 6c65 275d 2c0a 2020 2020 2020 2020  file'],.        
+00013470: 290a 2020 2020 6261 645f 6d6f 6475 6c65  ).    bad_module
+00013480: 7320 3d20 6765 745f 7772 6f6e 675f 6d6f  s = get_wrong_mo
+00013490: 6475 6c65 7328 7467 745f 6374 7829 0a20  dules(tgt_ctx). 
+000134a0: 2020 2069 6620 6261 645f 6d6f 6475 6c65     if bad_module
+000134b0: 733a 0a20 2020 2020 2020 206f 7330 2e77  s:.        os0.w
+000134c0: 6c6f 6728 272a 2a2a 2055 6e73 7461 626c  log('*** Unstabl
+000134d0: 6520 4442 2061 6674 6572 2063 6c65 616e  e DB after clean
+000134e0: 3a20 7772 6f6e 6720 6d6f 6475 6c65 2073  : wrong module s
+000134f0: 7461 7465 2025 7320 2a2a 2a27 2025 2062  tate %s ***' % b
+00013500: 6164 5f6d 6f64 756c 6573 290a 2020 2020  ad_modules).    
+00013510: 2020 2020 6861 7264 5f75 6e69 6e73 7461      hard_uninsta
+00013520: 6c6c 5f6c 6973 7420 3d20 6c69 7374 2873  ll_list = list(s
+00013530: 6574 2862 6164 5f6d 6f64 756c 6573 2920  et(bad_modules) 
+00013540: 2620 7365 7428 4d4f 4455 4c45 535f 325f  & set(MODULES_2_
+00013550: 4c45 4156 455f 4245 4849 4e44 2929 0a20  LEAVE_BEHIND)). 
+00013560: 2020 2020 2020 2062 6164 5f6d 6f64 756c         bad_modul
+00013570: 6573 203d 206c 6973 7428 7365 7428 6261  es = list(set(ba
+00013580: 645f 6d6f 6475 6c65 7329 202d 2073 6574  d_modules) - set
+00013590: 284d 4f44 554c 4553 5f32 5f4c 4541 5645  (MODULES_2_LEAVE
+000135a0: 5f42 4548 494e 4429 290a 2020 2020 2020  _BEHIND)).      
+000135b0: 2020 6966 2062 6164 5f6d 6f64 756c 6573    if bad_modules
+000135c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000135d0: 745f 756e 696e 7374 616c 6c65 645f 6279  t_uninstalled_by
+000135e0: 5f73 716c 2874 6774 5f63 7478 2c20 6261  _sql(tgt_ctx, ba
+000135f0: 645f 6d6f 6475 6c65 7329 0a20 2020 2020  d_modules).     
+00013600: 2020 2069 6620 6861 7264 5f75 6e69 6e73     if hard_unins
+00013610: 7461 6c6c 5f6c 6973 743a 0a20 2020 2020  tall_list:.     
+00013620: 2020 2020 2020 2066 6f72 206d 6f64 756c         for modul
+00013630: 6520 696e 2068 6172 645f 756e 696e 7374  e in hard_uninst
+00013640: 616c 6c5f 6c69 7374 3a0a 2020 2020 2020  all_list:.      
+00013650: 2020 2020 2020 2020 2020 6f73 302e 776c            os0.wl
+00013660: 6f67 2827 2020 2b2b 2048 6172 6420 756e  og('  ++ Hard un
+00013670: 696e 7374 616c 6c3a 2025 7327 2025 206d  install: %s' % m
+00013680: 6f64 756c 6529 0a20 2020 2020 2020 2020  odule).         
+00013690: 2020 2020 2020 2069 6620 6e6f 7420 7372         if not sr
+000136a0: 635f 6374 785b 2764 7279 5f72 756e 275d  c_ctx['dry_run']
+000136b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000136c0: 2020 2020 2020 6861 7264 5f63 6c65 616e        hard_clean
+000136d0: 5f6d 6f64 756c 6528 7467 745f 6374 782c  _module(tgt_ctx,
+000136e0: 206d 6f64 756c 6529 0a0a 2020 2020 6966   module)..    if
+000136f0: 206e 6f74 2073 7263 5f63 7478 5b27 6472   not src_ctx['dr
+00013700: 795f 7275 6e27 5d3a 0a20 2020 2020 2020  y_run']:.       
+00013710: 206f 7330 2e77 6c6f 6728 2754 6573 7420   os0.wlog('Test 
+00013720: 636f 6e6e 6563 7469 6f6e 2074 6f20 7461  connection to ta
+00013730: 7267 6574 2064 6220 2573 2720 2520 7467  rget db %s' % tg
+00013740: 745f 6374 785b 2764 625f 6e61 6d65 275d  t_ctx['db_name']
+00013750: 290a 2020 2020 2020 2020 7569 642c 2074  ).        uid, t
+00013760: 6774 5f63 7478 203d 2063 6c6f 646f 6f2e  gt_ctx = clodoo.
+00013770: 6f65 7270 5f73 6574 5f65 6e76 280a 2020  oerp_set_env(.  
+00013780: 2020 2020 2020 2020 2020 6374 783d 7467            ctx=tg
+00013790: 745f 6374 782c 2063 6f6e 666e 3d74 6774  t_ctx, confn=tgt
+000137a0: 5f66 756c 6c5f 6c63 6f6e 662c 2064 623d  _full_lconf, db=
+000137b0: 7467 745f 6374 785b 2764 625f 6e61 6d65  tgt_ctx['db_name
+000137c0: 275d 0a20 2020 2020 2020 2029 0a20 2020  '].        ).   
+000137d0: 2020 2020 2023 2046 4958 206f 6572 705f       # FIX oerp_
+000137e0: 7365 745f 656e 7620 6368 616e 6765 2064  set_env change d
+000137f0: 7279 5f72 756e 0a20 2020 2020 2020 2073  ry_run.        s
+00013800: 7263 5f63 7478 5b27 6472 795f 7275 6e27  rc_ctx['dry_run'
+00013810: 5d20 3d20 7467 745f 6374 785b 2764 7279  ] = tgt_ctx['dry
+00013820: 5f72 756e 275d 0a0a 2020 2020 7265 7475  _run']..    retu
+00013830: 726e 2074 6774 5f66 756c 6c5f 6c63 6f6e  rn tgt_full_lcon
+00013840: 660a 0a0a 6465 6620 6d69 6772 6174 655f  f...def migrate_
+00013850: 6461 7461 6261 7365 5f70 6173 7328 7372  database_pass(sr
+00013860: 635f 6374 782c 2074 6774 5f63 7478 2c20  c_ctx, tgt_ctx, 
+00013870: 7068 6173 653d 4e6f 6e65 293a 0a20 2020  phase=None):.   
+00013880: 2070 6861 7365 203d 2070 6861 7365 206f   phase = phase o
+00013890: 7220 320a 2020 2020 6469 7361 626c 655f  r 2.    disable_
+000138a0: 7665 6e76 203d 2046 616c 7365 0a20 2020  venv = False.   
+000138b0: 2069 6620 7068 6173 6520 3d3d 2031 3a0a   if phase == 1:.
+000138c0: 2020 2020 2020 2020 7361 7665 645f 6472          saved_dr
+000138d0: 795f 7275 6e20 3d20 7372 635f 6374 785b  y_run = src_ctx[
+000138e0: 2764 7279 5f72 756e 275d 0a20 2020 2020  'dry_run'].     
+000138f0: 2020 2073 7263 5f63 7478 5b27 6472 795f     src_ctx['dry_
+00013900: 7275 6e27 5d20 3d20 5472 7565 0a20 2020  run'] = True.   
+00013910: 2020 2020 2074 6774 5f63 7478 5b27 6472       tgt_ctx['dr
+00013920: 795f 7275 6e27 5d20 3d20 7372 635f 6374  y_run'] = src_ct
+00013930: 785b 2764 7279 5f72 756e 275d 0a20 2020  x['dry_run'].   
+00013940: 2077 6869 6c65 2031 3a0a 2020 2020 2020   while 1:.      
+00013950: 2020 6f73 302e 776c 6f67 2827 2d27 202a    os0.wlog('-' *
+00013960: 2038 3029 0a20 2020 2020 2020 2073 7263   80).        src
+00013970: 5f63 7478 2c20 7467 745f 6374 782c 2073  _ctx, tgt_ctx, s
+00013980: 7263 5f63 6f6e 6669 672c 2074 6774 5f63  rc_config, tgt_c
+00013990: 6f6e 6669 6720 3d20 6164 6a75 7374 5f63  onfig = adjust_c
+000139a0: 7478 2873 7263 5f63 7478 2c20 7467 745f  tx(src_ctx, tgt_
+000139b0: 6374 7829 0a20 2020 2020 2020 2066 6f72  ctx).        for
+000139c0: 2070 6172 616d 2069 6e20 2827 7669 6427   param in ('vid'
+000139d0: 2c20 276f 646f 6f5f 6676 6572 272c 2027  , 'odoo_fver', '
+000139e0: 6f64 6f6f 5f76 6572 2729 3a0a 2020 2020  odoo_ver'):.    
+000139f0: 2020 2020 2020 2020 6f73 302e 776c 6f67          os0.wlog
+00013a00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00013a10: 2020 2750 6173 7320 2564 206d 6967 7261    'Pass %d migra
+00013a20: 7469 6f6e 3a20 2573 2066 726f 6d20 2573  tion: %s from %s
+00013a30: 2074 6f20 2573 202e 2e27 0a20 2020 2020   to %s ..'.     
+00013a40: 2020 2020 2020 2020 2020 2025 2028 7068             % (ph
+00013a50: 6173 652c 2070 6172 616d 2c20 7372 635f  ase, param, src_
+00013a60: 6374 785b 2773 7263 5f25 7327 2025 2070  ctx['src_%s' % p
+00013a70: 6172 616d 5d2c 2074 6774 5f63 7478 5b27  aram], tgt_ctx['
+00013a80: 7467 745f 2573 2720 2520 7061 7261 6d5d  tgt_%s' % param]
+00013a90: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+00013aa0: 2020 2020 2020 2020 666f 7220 7061 7261          for para
+00013ab0: 6d20 696e 2028 2764 625f 6e61 6d65 272c  m in ('db_name',
+00013ac0: 2027 636f 6e66 5f66 6e27 2c20 2778 6d6c   'conf_fn', 'xml
+00013ad0: 7270 635f 706f 7274 272c 2027 6462 5f75  rpc_port', 'db_u
+00013ae0: 7365 7227 293a 0a20 2020 2020 2020 2020  ser'):.         
+00013af0: 2020 206f 7330 2e77 6c6f 6728 0a20 2020     os0.wlog(.   
+00013b00: 2020 2020 2020 2020 2020 2020 2027 5061               'Pa
+00013b10: 7373 2025 6420 6d69 6772 6174 696f 6e3a  ss %d migration:
+00013b20: 2025 7320 6672 6f6d 2025 7320 746f 2025   %s from %s to %
+00013b30: 7320 2e2e 270a 2020 2020 2020 2020 2020  s ..'.          
+00013b40: 2020 2020 2020 2520 2870 6861 7365 2c20        % (phase, 
+00013b50: 7061 7261 6d2c 2073 7263 5f63 7478 5b70  param, src_ctx[p
+00013b60: 6172 616d 5d2c 2074 6774 5f63 7478 5b70  aram], tgt_ctx[p
+00013b70: 6172 616d 5d29 0a20 2020 2020 2020 2020  aram]).         
+00013b80: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00013b90: 7068 6173 6520 3d3d 2031 3a0a 2020 2020  phase == 1:.    
+00013ba0: 2020 2020 2020 2020 6966 206e 6f74 206f          if not o
+00013bb0: 732e 7061 7468 2e69 7364 6972 2874 6774  s.path.isdir(tgt
+00013bc0: 5f63 7478 5b27 7665 6e76 5f6f 7570 6174  _ctx['venv_oupat
+00013bd0: 6827 5d29 3a0a 2020 2020 2020 2020 2020  h']):.          
+00013be0: 2020 2020 2020 6f73 302e 776c 6f67 2827        os0.wlog('
+00013bf0: 4469 7265 6374 6f72 7920 2573 206e 6f74  Directory %s not
+00013c00: 2066 6f75 6e64 2127 2025 2074 6774 5f63   found!' % tgt_c
+00013c10: 7478 5b27 7665 6e76 5f6f 7570 6174 6827  tx['venv_oupath'
+00013c20: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00013c30: 2020 2064 6973 6162 6c65 5f76 656e 7620     disable_venv 
+00013c40: 3d20 5472 7565 0a20 2020 2020 2020 2065  = True.        e
+00013c50: 6c69 6620 6e6f 7420 7372 635f 6374 785b  lif not src_ctx[
+00013c60: 2764 7279 5f72 756e 275d 3a0a 2020 2020  'dry_run']:.    
+00013c70: 2020 2020 2020 2020 6472 6f70 5f64 6228          drop_db(
+00013c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013c90: 2073 7263 5f63 7478 2c0a 2020 2020 2020   src_ctx,.      
+00013ca0: 2020 2020 2020 2020 2020 7467 745f 6374            tgt_ct
+00013cb0: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
+00013cc0: 2020 2074 6774 5f63 7478 5b27 6462 5f6e     tgt_ctx['db_n
+00013cd0: 616d 6527 5d2c 0a20 2020 2020 2020 2020  ame'],.         
+00013ce0: 2020 2020 2020 206e 6577 5f64 626e 616d         new_dbnam
+00013cf0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00013d00: 2020 2020 2020 2073 7263 5f63 7478 5b27         src_ctx['
+00013d10: 6462 5f6e 616d 6527 5d2c 2074 6774 5f63  db_name'], tgt_c
+00013d20: 7478 5b27 7467 745f 6f64 6f6f 5f76 6572  tx['tgt_odoo_ver
+00013d30: 275d 2c20 7467 745f 6374 785b 276f 6361  '], tgt_ctx['oca
+00013d40: 5f6d 6967 7261 7465 275d 0a20 2020 2020  _migrate'].     
+00013d50: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+00013d60: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00013d70: 2020 2020 6675 6c6c 5f6c 636f 6e66 203d      full_lconf =
+00013d80: 206d 6967 7261 7465 5f6f 646f 6f28 7372   migrate_odoo(sr
+00013d90: 635f 6374 782c 2074 6774 5f63 7478 2c20  c_ctx, tgt_ctx, 
+00013da0: 7372 635f 636f 6e66 6967 2c20 7467 745f  src_config, tgt_
+00013db0: 636f 6e66 6967 2c20 7068 6173 653d 7068  config, phase=ph
+00013dc0: 6173 6529 0a20 2020 2020 2020 2069 6620  ase).        if 
+00013dd0: 7467 745f 6374 785b 2774 6774 5f6f 646f  tgt_ctx['tgt_odo
+00013de0: 6f5f 7665 7227 5d20 3e3d 2073 7263 5f63  o_ver'] >= src_c
+00013df0: 7478 5b27 6669 6e61 6c5f 7665 7227 5d3a  tx['final_ver']:
+00013e00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00013e10: 6469 7361 626c 655f 7665 6e76 3a0a 2020  disable_venv:.  
+00013e20: 2020 2020 2020 2020 2020 2020 2020 7372                sr
+00013e30: 635f 6374 785b 2776 656e 765f 6f75 7061  c_ctx['venv_oupa
+00013e40: 7468 275d 203d 2073 7263 5f63 7478 5b27  th'] = src_ctx['
+00013e50: 6f70 745f 6f75 7061 7468 275d 0a20 2020  opt_oupath'].   
+00013e60: 2020 2020 2020 2020 2020 2020 2074 6774               tgt
+00013e70: 5f63 7478 5b27 7665 6e76 5f6f 7570 6174  _ctx['venv_oupat
+00013e80: 6827 5d20 3d20 7372 635f 6374 785b 2776  h'] = src_ctx['v
+00013e90: 656e 765f 6f75 7061 7468 275d 0a20 2020  env_oupath'].   
+00013ea0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+00013eb0: 2020 2020 2020 2069 6620 6e6f 7420 7372         if not sr
+00013ec0: 635f 6374 785b 276e 6f5f 7665 6e76 275d  c_ctx['no_venv']
+00013ed0: 2061 6e64 206e 6f74 2073 7263 5f63 7478   and not src_ctx
+00013ee0: 5b27 6472 795f 7275 6e27 5d3a 0a20 2020  ['dry_run']:.   
+00013ef0: 2020 2020 2020 2020 2076 656e 765f 7061           venv_pa
+00013f00: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
+00013f10: 6e28 7467 745f 6374 785b 2776 656e 765f  n(tgt_ctx['venv_
+00013f20: 6f75 7061 7468 275d 2c20 276f 7065 6e75  oupath'], 'openu
+00013f30: 7067 7261 6465 2729 0a20 2020 2020 2020  pgrade').       
+00013f40: 2020 2020 2023 2054 4f44 4f0a 2020 2020       # TODO.    
+00013f50: 2020 2020 2020 2020 2320 6966 206e 6f74          # if not
+00013f60: 206f 732e 7061 7468 2e69 7364 6972 2876   os.path.isdir(v
+00013f70: 656e 765f 7061 7468 293a 0a20 2020 2020  env_path):.     
+00013f80: 2020 2020 2020 2023 2020 2020 6f73 2e75         #    os.u
+00013f90: 6e6c 696e 6b28 6f73 2e70 6174 682e 6a6f  nlink(os.path.jo
+00013fa0: 696e 2876 656e 765f 7061 7468 2c20 6f75  in(venv_path, ou
+00013fb0: 5f76 6572 5f70 6174 6829 290a 2020 2020  _ver_path)).    
+00013fc0: 2020 2020 7372 635f 6374 782c 2074 6774      src_ctx, tgt
+00013fd0: 5f63 7478 203d 2073 6869 6674 5f63 7478  _ctx = shift_ctx
+00013fe0: 2873 7263 5f63 7478 2c20 7467 745f 6374  (src_ctx, tgt_ct
+00013ff0: 782c 2070 6861 7365 3d70 6861 7365 290a  x, phase=phase).
+00014000: 0a20 2020 2069 6620 7068 6173 6520 3d3d  .    if phase ==
+00014010: 2031 3a0a 2020 2020 2020 2020 7372 635f   1:.        src_
+00014020: 6374 785b 2764 7279 5f72 756e 275d 203d  ctx['dry_run'] =
+00014030: 2073 6176 6564 5f64 7279 5f72 756e 0a20   saved_dry_run. 
+00014040: 2020 2020 2020 2074 6774 5f63 7478 5b27         tgt_ctx['
+00014050: 6472 795f 7275 6e27 5d20 3d20 7372 635f  dry_run'] = src_
+00014060: 6374 785b 2764 7279 5f72 756e 275d 0a0a  ctx['dry_run']..
+00014070: 0a64 6566 206d 6967 7261 7465 5f64 6174  .def migrate_dat
+00014080: 6162 6173 6528 7372 635f 6374 782c 2074  abase(src_ctx, t
+00014090: 6774 5f63 7478 293a 0a20 2020 2069 6620  gt_ctx):.    if 
+000140a0: 7372 635f 6374 785b 2770 6861 7365 5f31  src_ctx['phase_1
+000140b0: 275d 3a0a 2020 2020 2020 2020 7372 635f  ']:.        src_
+000140c0: 6374 7820 3d20 696e 6974 5f63 7478 2873  ctx = init_ctx(s
+000140d0: 7263 5f63 7478 290a 2020 2020 2020 2020  rc_ctx).        
+000140e0: 6d69 6772 6174 655f 6461 7461 6261 7365  migrate_database
+000140f0: 5f70 6173 7328 7372 635f 6374 782c 2074  _pass(src_ctx, t
+00014100: 6774 5f63 7478 2c20 7068 6173 653d 3129  gt_ctx, phase=1)
+00014110: 0a20 2020 2020 2020 2066 6f72 206e 6d20  .        for nm 
+00014120: 696e 2028 276f 7269 6769 6e61 6c5f 6d6f  in ('original_mo
+00014130: 6475 6c65 5f6c 6973 7427 2c29 3a0a 2020  dule_list',):.  
+00014140: 2020 2020 2020 2020 2020 6465 6c20 7372            del sr
+00014150: 635f 6374 785b 6e6d 5d0a 2020 2020 7372  c_ctx[nm].    sr
+00014160: 635f 6374 7820 3d20 696e 6974 5f63 7478  c_ctx = init_ctx
+00014170: 2873 7263 5f63 7478 290a 2020 2020 6d69  (src_ctx).    mi
+00014180: 6772 6174 655f 6461 7461 6261 7365 5f70  grate_database_p
+00014190: 6173 7328 7372 635f 6374 782c 2074 6774  ass(src_ctx, tgt
+000141a0: 5f63 7478 2c20 7068 6173 653d 3229 0a20  _ctx, phase=2). 
+000141b0: 2020 2070 7269 6e74 280a 2020 2020 2020     print(.      
+000141c0: 2020 2744 6174 6162 6173 6520 2573 2073    'Database %s s
+000141d0: 7563 6365 7373 6675 6c6c 7920 6d69 6f67  uccessfully miog
+000141e0: 7261 7465 6420 696e 746f 2025 7327 0a20  rated into %s'. 
+000141f0: 2020 2020 2020 2025 2028 7372 635f 6374         % (src_ct
+00014200: 785b 2766 726f 6d5f 6462 6e61 6d65 275d  x['from_dbname']
+00014210: 2c20 7467 745f 6374 785b 2764 625f 6e61  , tgt_ctx['db_na
+00014220: 6d65 275d 290a 2020 2020 290a 0a0a 6465  me']).    )...de
+00014230: 6620 7061 7273 655f 6374 7828 7372 635f  f parse_ctx(src_
+00014240: 6374 7829 3a0a 2020 2020 676c 6f62 616c  ctx):.    global
+00014250: 2044 4546 5f43 4f4e 460a 2020 2020 6966   DEF_CONF.    if
+00014260: 206e 6f74 2073 7263 5f63 7478 5b27 6672   not src_ctx['fr
+00014270: 6f6d 5f62 7261 6e63 6827 5d20 616e 6420  om_branch'] and 
+00014280: 6e6f 7420 7372 635f 6374 785b 2766 726f  not src_ctx['fro
+00014290: 6d5f 636f 6e66 6e27 5d3a 0a20 2020 2020  m_confn']:.     
+000142a0: 2020 2072 6169 7365 204b 6579 4572 726f     raise KeyErro
+000142b0: 7228 274d 6973 7365 6420 6f72 6967 696e  r('Missed origin
+000142c0: 616c 206f 646f 6f20 7665 7273 696f 6e21  al odoo version!
+000142d0: 2050 6c65 6173 6520 7573 6520 2d46 2073   Please use -F s
+000142e0: 7769 7463 6827 290a 2020 2020 656c 6966  witch').    elif
+000142f0: 2073 7263 5f63 7478 5b27 6672 6f6d 5f62   src_ctx['from_b
+00014300: 7261 6e63 6827 5d3a 0a20 2020 2020 2020  ranch']:.       
+00014310: 2073 7263 5f63 7478 5b27 7372 635f 6f64   src_ctx['src_od
+00014320: 6f6f 5f66 7665 7227 5d20 3d20 636c 6f64  oo_fver'] = clod
+00014330: 6f6f 2e62 7569 6c64 5f6f 646f 6f5f 7061  oo.build_odoo_pa
+00014340: 7261 6d28 0a20 2020 2020 2020 2020 2020  ram(.           
+00014350: 2027 4655 4c4c 5645 5227 2c20 6f64 6f6f   'FULLVER', odoo
+00014360: 5f76 6964 3d73 7263 5f63 7478 5b27 6672  _vid=src_ctx['fr
+00014370: 6f6d 5f62 7261 6e63 6827 5d2c 206d 756c  om_branch'], mul
+00014380: 7469 3d54 7275 650a 2020 2020 2020 2020  ti=True.        
+00014390: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+000143a0: 2073 7263 5f63 7478 5b27 6672 6f6d 5f63   src_ctx['from_c
+000143b0: 6f6e 666e 275d 3a0a 2020 2020 2020 2020  onfn']:.        
+000143c0: 2020 2020 7372 635f 6374 785b 2766 726f      src_ctx['fro
+000143d0: 6d5f 636f 6e66 6e27 5d20 3d20 636c 6f64  m_confn'] = clod
+000143e0: 6f6f 2e62 7569 6c64 5f6f 646f 6f5f 7061  oo.build_odoo_pa
+000143f0: 7261 6d28 0a20 2020 2020 2020 2020 2020  ram(.           
+00014400: 2020 2020 2027 434f 4e46 4e27 2c20 6f64       'CONFN', od
+00014410: 6f6f 5f76 6964 3d73 7263 5f63 7478 5b27  oo_vid=src_ctx['
+00014420: 6672 6f6d 5f62 7261 6e63 6827 5d2c 206d  from_branch'], m
+00014430: 756c 7469 3d54 7275 650a 2020 2020 2020  ulti=True.      
+00014440: 2020 2020 2020 290a 2020 2020 6966 206e        ).    if n
+00014450: 6f74 206f 732e 7061 7468 2e69 7366 696c  ot os.path.isfil
+00014460: 6528 7372 635f 6374 785b 2766 726f 6d5f  e(src_ctx['from_
+00014470: 636f 6e66 6e27 5d29 3a0a 2020 2020 2020  confn']):.      
+00014480: 2020 7261 6973 6520 494f 4572 726f 7228    raise IOError(
+00014490: 2746 696c 6520 2573 206e 6f74 2066 6f75  'File %s not fou
+000144a0: 6e64 2720 2520 7372 635f 6374 785b 2766  nd' % src_ctx['f
+000144b0: 726f 6d5f 636f 6e66 6e27 5d29 0a20 2020  rom_confn']).   
+000144c0: 2069 6620 6e6f 7420 7372 635f 6374 785b   if not src_ctx[
+000144d0: 2766 726f 6d5f 6272 616e 6368 275d 3a0a  'from_branch']:.
+000144e0: 2020 2020 2020 2020 7372 635f 636f 6e66          src_conf
+000144f0: 6967 203d 2043 6f6e 6669 6750 6172 7365  ig = ConfigParse
+00014500: 722e 5361 6665 436f 6e66 6967 5061 7273  r.SafeConfigPars
+00014510: 6572 2829 0a20 2020 2020 2020 2073 7263  er().        src
+00014520: 5f63 6f6e 6669 672e 7265 6164 2873 7263  _config.read(src
+00014530: 5f63 7478 5b27 6672 6f6d 5f63 6f6e 666e  _ctx['from_confn
+00014540: 275d 290a 2020 2020 2020 2020 7372 635f  ']).        src_
+00014550: 6374 785b 2773 7263 5f6f 646f 6f5f 6676  ctx['src_odoo_fv
+00014560: 6572 275d 203d 2073 7263 5f63 6f6e 6669  er'] = src_confi
+00014570: 672e 6765 7428 276f 7074 696f 6e73 272c  g.get('options',
+00014580: 2027 6f65 5f76 6572 7369 6f6e 2729 0a20   'oe_version'). 
+00014590: 2020 2020 2020 2073 7263 5f63 7478 5b27         src_ctx['
+000145a0: 6672 6f6d 5f62 7261 6e63 6827 5d20 3d20  from_branch'] = 
+000145b0: 7372 635f 6374 785b 2773 7263 5f6f 646f  src_ctx['src_odo
+000145c0: 6f5f 6676 6572 275d 0a20 2020 2073 7263  o_fver'].    src
+000145d0: 5f63 7478 5b27 7372 635f 6f64 6f6f 5f76  _ctx['src_odoo_v
+000145e0: 6572 275d 203d 2063 6c6f 646f 6f2e 6275  er'] = clodoo.bu
+000145f0: 696c 645f 6f64 6f6f 5f70 6172 616d 280a  ild_odoo_param(.
+00014600: 2020 2020 2020 2020 274d 414a 5645 5227          'MAJVER'
+00014610: 2c20 6f64 6f6f 5f76 6964 3d73 7263 5f63  , odoo_vid=src_c
+00014620: 7478 5b27 6672 6f6d 5f62 7261 6e63 6827  tx['from_branch'
+00014630: 5d2c 206d 756c 7469 3d54 7275 650a 2020  ], multi=True.  
+00014640: 2020 290a 0a20 2020 2069 6620 6e6f 7420    )..    if not 
+00014650: 7372 635f 6374 785b 2766 696e 616c 5f62  src_ctx['final_b
+00014660: 7261 6e63 6827 5d20 616e 6420 6e6f 7420  ranch'] and not 
+00014670: 7372 635f 6374 785b 2766 696e 616c 5f63  src_ctx['final_c
+00014680: 6f6e 666e 275d 3a0a 2020 2020 2020 2020  onfn']:.        
+00014690: 7261 6973 6520 4b65 7945 7272 6f72 2827  raise KeyError('
+000146a0: 4d69 7373 6564 2066 696e 616c 206f 646f  Missed final odo
+000146b0: 6f20 7665 7273 696f 6e21 2050 6c65 6173  o version! Pleas
+000146c0: 6520 7573 6520 2d62 2073 7769 7463 6827  e use -b switch'
+000146d0: 290a 2020 2020 656c 6966 2073 7263 5f63  ).    elif src_c
+000146e0: 7478 5b27 6669 6e61 6c5f 6272 616e 6368  tx['final_branch
+000146f0: 275d 3a0a 2020 2020 2020 2020 7372 635f  ']:.        src_
+00014700: 6374 785b 2774 6774 5f6f 646f 6f5f 6676  ctx['tgt_odoo_fv
+00014710: 6572 275d 203d 2063 6c6f 646f 6f2e 6275  er'] = clodoo.bu
+00014720: 696c 645f 6f64 6f6f 5f70 6172 616d 280a  ild_odoo_param(.
+00014730: 2020 2020 2020 2020 2020 2020 2746 554c              'FUL
+00014740: 4c56 4552 272c 206f 646f 6f5f 7669 643d  LVER', odoo_vid=
+00014750: 7372 635f 6374 785b 2766 696e 616c 5f62  src_ctx['final_b
+00014760: 7261 6e63 6827 5d2c 206d 756c 7469 3d54  ranch'], multi=T
+00014770: 7275 650a 2020 2020 2020 2020 290a 2020  rue.        ).  
+00014780: 2020 2020 2020 6966 206e 6f74 2073 7263        if not src
+00014790: 5f63 7478 5b27 6669 6e61 6c5f 636f 6e66  _ctx['final_conf
+000147a0: 6e27 5d3a 0a20 2020 2020 2020 2020 2020  n']:.           
+000147b0: 2073 7263 5f63 7478 5b27 6669 6e61 6c5f   src_ctx['final_
+000147c0: 636f 6e66 6e27 5d20 3d20 636c 6f64 6f6f  confn'] = clodoo
+000147d0: 2e62 7569 6c64 5f6f 646f 6f5f 7061 7261  .build_odoo_para
+000147e0: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
+000147f0: 2020 2027 434f 4e46 4e27 2c20 6f64 6f6f     'CONFN', odoo
+00014800: 5f76 6964 3d73 7263 5f63 7478 5b27 6669  _vid=src_ctx['fi
+00014810: 6e61 6c5f 6272 616e 6368 275d 2c20 6d75  nal_branch'], mu
+00014820: 6c74 693d 5472 7565 0a20 2020 2020 2020  lti=True.       
+00014830: 2020 2020 2029 0a20 2020 2069 6620 6e6f       ).    if no
+00014840: 7420 6f73 2e70 6174 682e 6973 6669 6c65  t os.path.isfile
+00014850: 2873 7263 5f63 7478 5b27 6669 6e61 6c5f  (src_ctx['final_
+00014860: 636f 6e66 6e27 5d29 3a0a 2020 2020 2020  confn']):.      
+00014870: 2020 7261 6973 6520 494f 4572 726f 7228    raise IOError(
+00014880: 2746 696c 6520 2573 206e 6f74 2066 6f75  'File %s not fou
+00014890: 6e64 2720 2520 7372 635f 6374 785b 2766  nd' % src_ctx['f
+000148a0: 696e 616c 5f63 6f6e 666e 275d 290a 2020  inal_confn']).  
+000148b0: 2020 6966 206e 6f74 2073 7263 5f63 7478    if not src_ctx
+000148c0: 5b27 6669 6e61 6c5f 6272 616e 6368 275d  ['final_branch']
+000148d0: 3a0a 2020 2020 2020 2020 7467 745f 636f  :.        tgt_co
+000148e0: 6e66 6967 203d 2043 6f6e 6669 6750 6172  nfig = ConfigPar
+000148f0: 7365 722e 5361 6665 436f 6e66 6967 5061  ser.SafeConfigPa
+00014900: 7273 6572 2829 0a20 2020 2020 2020 2074  rser().        t
+00014910: 6774 5f63 6f6e 6669 672e 7265 6164 2873  gt_config.read(s
+00014920: 7263 5f63 7478 5b27 6669 6e61 6c5f 636f  rc_ctx['final_co
+00014930: 6e66 6e27 5d29 0a20 2020 2020 2020 2073  nfn']).        s
+00014940: 7263 5f63 7478 5b27 7467 745f 6f64 6f6f  rc_ctx['tgt_odoo
+00014950: 5f66 7665 7227 5d20 3d20 7467 745f 636f  _fver'] = tgt_co
+00014960: 6e66 6967 2e67 6574 2827 6f70 7469 6f6e  nfig.get('option
+00014970: 7327 2c20 276f 655f 7665 7273 696f 6e27  s', 'oe_version'
+00014980: 290a 2020 2020 2020 2020 7372 635f 6374  ).        src_ct
+00014990: 785b 2766 696e 616c 5f62 7261 6e63 6827  x['final_branch'
+000149a0: 5d20 3d20 7372 635f 6374 785b 2774 6774  ] = src_ctx['tgt
+000149b0: 5f6f 646f 6f5f 6676 6572 275d 0a20 2020  _odoo_fver'].   
+000149c0: 2073 7263 5f63 7478 5b27 7467 745f 6f64   src_ctx['tgt_od
+000149d0: 6f6f 5f76 6572 275d 203d 2063 6c6f 646f  oo_ver'] = clodo
+000149e0: 6f2e 6275 696c 645f 6f64 6f6f 5f70 6172  o.build_odoo_par
+000149f0: 616d 280a 2020 2020 2020 2020 274d 414a  am(.        'MAJ
+00014a00: 5645 5227 2c20 6f64 6f6f 5f76 6964 3d73  VER', odoo_vid=s
+00014a10: 7263 5f63 7478 5b27 6669 6e61 6c5f 6272  rc_ctx['final_br
+00014a20: 616e 6368 275d 2c20 6d75 6c74 693d 5472  anch'], multi=Tr
+00014a30: 7565 0a20 2020 2029 0a0a 2020 2020 6966  ue.    )..    if
+00014a40: 2028 0a20 2020 2020 2020 2073 7263 5f63   (.        src_c
+00014a50: 7478 5b27 7372 635f 6f64 6f6f 5f76 6572  tx['src_odoo_ver
+00014a60: 275d 203e 3d20 7372 635f 6374 785b 2774  '] >= src_ctx['t
+00014a70: 6774 5f6f 646f 6f5f 7665 7227 5d20 616e  gt_odoo_ver'] an
+00014a80: 6420 6e6f 7420 7372 635f 6374 785b 2773  d not src_ctx['s
+00014a90: 656c 5f6d 6f64 656c 275d 0a20 2020 2029  el_model'].    )
+00014aa0: 206f 7220 2873 7263 5f63 7478 5b27 7372   or (src_ctx['sr
+00014ab0: 635f 6f64 6f6f 5f76 6572 275d 203e 2073  c_odoo_ver'] > s
+00014ac0: 7263 5f63 7478 5b27 7467 745f 6f64 6f6f  rc_ctx['tgt_odoo
+00014ad0: 5f76 6572 275d 2061 6e64 2073 7263 5f63  _ver'] and src_c
+00014ae0: 7478 5b27 7365 6c5f 6d6f 6465 6c27 5d29  tx['sel_model'])
+00014af0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+00014b00: 4b65 7945 7272 6f72 2827 4669 6e61 6c20  KeyError('Final 
+00014b10: 7665 7273 696f 6e20 6d75 7374 2062 6520  version must be 
+00014b20: 6772 6561 7465 7220 7468 616e 206f 7269  greater than ori
+00014b30: 6769 6e61 6c20 7665 7273 696f 6e27 290a  ginal version').
+00014b40: 0a20 2020 2069 6620 6e6f 7420 7372 635f  .    if not src_
+00014b50: 6374 785b 276f 7074 5f6f 7570 6174 6827  ctx['opt_oupath'
+00014b60: 5d3a 0a20 2020 2020 2020 2073 7263 5f63  ]:.        src_c
+00014b70: 7478 5b27 6f70 745f 6f75 7061 7468 275d  tx['opt_oupath']
+00014b80: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00014b90: 6f73 2e70 6174 682e 6578 7061 6e64 7573  os.path.expandus
+00014ba0: 6572 2827 7e27 292c 2027 746d 7027 290a  er('~'), 'tmp').
+00014bb0: 2020 2020 6966 206e 6f74 2073 7263 5f63      if not src_c
+00014bc0: 7478 5b27 6f70 745f 6f75 6c70 6174 6827  tx['opt_oulpath'
+00014bd0: 5d3a 0a20 2020 2020 2020 2073 7263 5f63  ]:.        src_c
+00014be0: 7478 5b27 6f70 745f 6f75 6c70 6174 6827  tx['opt_oulpath'
+00014bf0: 5d20 3d20 6f73 2e70 6174 682e 6a6f 696e  ] = os.path.join
+00014c00: 2873 7263 5f63 7478 5b27 6f70 745f 6f75  (src_ctx['opt_ou
+00014c10: 7061 7468 275d 2c20 276f 7065 6e75 7067  path'], 'openupg
+00014c20: 7261 6465 6c69 6227 290a 0a20 2020 2069  radelib')..    i
+00014c30: 6620 7372 635f 6374 785b 2766 696e 616c  f src_ctx['final
+00014c40: 5f64 626e 616d 6527 5d20 616e 6420 6e6f  _dbname'] and no
+00014c50: 7420 7372 635f 6374 785b 2766 726f 6d5f  t src_ctx['from_
+00014c60: 6462 6e61 6d65 275d 3a0a 2020 2020 2020  dbname']:.      
+00014c70: 2020 7372 635f 6374 785b 2766 726f 6d5f    src_ctx['from_
+00014c80: 6462 6e61 6d65 275d 2c20 7372 635f 6374  dbname'], src_ct
+00014c90: 785b 2766 696e 616c 5f64 626e 616d 6527  x['final_dbname'
+00014ca0: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
+00014cb0: 2020 7372 635f 6374 785b 2766 696e 616c    src_ctx['final
+00014cc0: 5f64 626e 616d 6527 5d2c 0a20 2020 2020  _dbname'],.     
+00014cd0: 2020 2020 2020 2027 2573 5f32 3032 3127         '%s_2021'
+00014ce0: 2025 2073 7263 5f63 7478 5b27 6669 6e61   % src_ctx['fina
+00014cf0: 6c5f 6462 6e61 6d65 275d 2c0a 2020 2020  l_dbname'],.    
+00014d00: 2020 2020 290a 2020 2020 656c 6966 206e      ).    elif n
+00014d10: 6f74 2073 7263 5f63 7478 5b27 6669 6e61  ot src_ctx['fina
+00014d20: 6c5f 6462 6e61 6d65 275d 2061 6e64 2073  l_dbname'] and s
+00014d30: 7263 5f63 7478 5b27 6672 6f6d 5f64 626e  rc_ctx['from_dbn
+00014d40: 616d 6527 5d3a 0a20 2020 2020 2020 2073  ame']:.        s
+00014d50: 7263 5f63 7478 5b27 6669 6e61 6c5f 6462  rc_ctx['final_db
+00014d60: 6e61 6d65 275d 203d 2027 2573 5f32 3032  name'] = '%s_202
+00014d70: 3127 2025 2073 7263 5f63 7478 5b27 6672  1' % src_ctx['fr
+00014d80: 6f6d 5f64 626e 616d 6527 5d0a 2020 2020  om_dbname'].    
+00014d90: 656c 6966 206e 6f74 2073 7263 5f63 7478  elif not src_ctx
+00014da0: 5b27 6669 6e61 6c5f 6462 6e61 6d65 275d  ['final_dbname']
+00014db0: 2061 6e64 206e 6f74 2073 7263 5f63 7478   and not src_ctx
+00014dc0: 5b27 6672 6f6d 5f64 626e 616d 6527 5d3a  ['from_dbname']:
+00014dd0: 0a20 2020 2020 2020 2072 6169 7365 204b  .        raise K
+00014de0: 6579 4572 726f 7228 274d 6973 7365 6420  eyError('Missed 
+00014df0: 6461 7461 6261 7365 2074 6f20 7570 6772  database to upgr
+00014e00: 6164 6521 2050 6c65 6173 6520 7573 6520  ade! Please use 
+00014e10: 2d64 2073 7769 7463 6827 290a 0a20 2020  -d switch')..   
+00014e20: 2069 6620 6e6f 7420 7372 635f 6374 785b   if not src_ctx[
+00014e30: 276c 6f67 666e 275d 3a0a 2020 2020 2020  'logfn']:.      
+00014e40: 2020 6966 2073 7263 5f63 7478 5b27 6f63    if src_ctx['oc
+00014e50: 615f 6d69 6772 6174 6527 5d3a 0a20 2020  a_migrate']:.   
+00014e60: 2020 2020 2020 2020 2073 7263 5f63 7478           src_ctx
+00014e70: 5b27 6c6f 6766 6e27 5d20 3d20 6f73 2e70  ['logfn'] = os.p
+00014e80: 6174 682e 6a6f 696e 280a 2020 2020 2020  ath.join(.      
+00014e90: 2020 2020 2020 2020 2020 7372 635f 6374            src_ct
+00014ea0: 785b 276f 7074 5f6f 7570 6174 6827 5d2c  x['opt_oupath'],
+00014eb0: 2027 6d69 6772 6174 655f 6279 5f6f 7065   'migrate_by_ope
+00014ec0: 6e75 7067 7261 6465 2e6c 6f67 270a 2020  nupgrade.log'.  
+00014ed0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00014ee0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00014ef0: 2020 2020 2020 7372 635f 6374 785b 276c        src_ctx['l
+00014f00: 6f67 666e 275d 203d 206f 732e 7061 7468  ogfn'] = os.path
+00014f10: 2e6a 6f69 6e28 0a20 2020 2020 2020 2020  .join(.         
+00014f20: 2020 2020 2020 2073 7263 5f63 7478 5b27         src_ctx['
+00014f30: 6f70 745f 6f75 7061 7468 275d 2c20 276d  opt_oupath'], 'm
+00014f40: 6967 7261 7465 5f6f 646f 6f5f 6462 2e6c  igrate_odoo_db.l
+00014f50: 6f67 270a 2020 2020 2020 2020 2020 2020  og'.            
+00014f60: 290a 2020 2020 7372 635f 6374 785b 276c  ).    src_ctx['l
+00014f70: 6f67 6669 6c65 275d 203d 206f 732e 7061  ogfile'] = os.pa
+00014f80: 7468 2e6a 6f69 6e28 0a20 2020 2020 2020  th.join(.       
+00014f90: 2073 7263 5f63 7478 5b27 6f70 745f 6f75   src_ctx['opt_ou
+00014fa0: 7061 7468 275d 2c20 276d 6967 7261 7465  path'], 'migrate
+00014fb0: 5f6f 646f 6f5f 6462 2d73 6572 7665 722e  _odoo_db-server.
+00014fc0: 6c6f 6727 0a20 2020 2029 0a20 2020 2073  log'.    ).    s
+00014fd0: 7263 5f63 7478 5b27 6669 6e61 6c5f 7665  rc_ctx['final_ve
+00014fe0: 7227 5d20 3d20 7372 635f 6374 785b 2774  r'] = src_ctx['t
+00014ff0: 6774 5f6f 646f 6f5f 7665 7227 5d0a 2020  gt_odoo_ver'].  
+00015000: 2020 7467 745f 6374 7820 3d20 7372 635f    tgt_ctx = src_
+00015010: 6374 782e 636f 7079 2829 0a20 2020 2044  ctx.copy().    D
+00015020: 4546 5f43 4f4e 4620 3d20 636c 6f64 6f6f  EF_CONF = clodoo
+00015030: 2e64 6566 6175 6c74 5f63 6f6e 6628 7372  .default_conf(sr
+00015040: 635f 6374 7829 0a20 2020 2072 6574 7572  c_ctx).    retur
+00015050: 6e20 7372 635f 6374 782c 2074 6774 5f63  n src_ctx, tgt_c
+00015060: 7478 0a0a 0a5f 4445 5052 4543 4154 4544  tx..._DEPRECATED
+00015070: 5f4d 4f44 554c 4553 203d 205b 0a20 2020  _MODULES = [.   
+00015080: 2028 2261 6363 6f75 6e74 5f61 6e61 6c79   ("account_analy
+00015090: 7469 635f 616e 616c 7973 6973 222c 2022  tic_analysis", "
+000150a0: 6f63 615f 6d6f 7665 6422 2c20 2263 6f6e  oca_moved", "con
+000150b0: 7472 6163 7422 2c20 224d 6f76 6564 2074  tract", "Moved t
+000150c0: 6f20 4f43 412f 636f 6e74 7261 6374 2229  o OCA/contract")
+000150d0: 2c0a 2020 2020 280a 2020 2020 2020 2020  ,.    (.        
+000150e0: 2261 6363 6f75 6e74 5f61 6e61 6c79 7469  "account_analyti
+000150f0: 635f 706c 616e 7322 2c0a 2020 2020 2020  c_plans",.      
+00015100: 2020 226f 6361 5f6d 6f76 6564 222c 0a20    "oca_moved",. 
+00015110: 2020 2020 2020 2022 6163 636f 756e 745f         "account_
+00015120: 616e 616c 7974 6963 5f64 6973 7472 6962  analytic_distrib
+00015130: 7574 696f 6e22 2c0a 2020 2020 2020 2020  ution",.        
+00015140: 224d 6f76 6564 2074 6f20 4f43 412f 6163  "Moved to OCA/ac
+00015150: 636f 756e 745f 616e 616c 7974 6963 222c  count_analytic",
+00015160: 0a20 2020 2029 2c0a 2020 2020 2822 6163  .    ),.    ("ac
+00015170: 636f 756e 745f 616e 676c 6f5f 7361 786f  count_anglo_saxo
+00015180: 6e22 2c20 2272 656d 6f76 6564 2229 2c0a  n", "removed"),.
+00015190: 2020 2020 2822 6163 636f 756e 745f 6261      ("account_ba
+000151a0: 6e6b 5f73 7461 7465 6d65 6e74 5f65 7874  nk_statement_ext
+000151b0: 656e 7369 6f6e 7322 2c20 2272 656d 6f76  ensions", "remov
+000151c0: 6564 2229 2c0a 2020 2020 2822 6163 636f  ed"),.    ("acco
+000151d0: 756e 745f 6368 6172 7422 2c20 226d 6572  unt_chart", "mer
+000151e0: 6765 6422 2c20 2261 6363 6f75 6e74 2229  ged", "account")
+000151f0: 2c0a 2020 2020 2822 6163 636f 756e 745f  ,.    ("account_
+00015200: 6368 6563 6b5f 7772 6974 696e 6722 2c20  check_writing", 
+00015210: 2272 656e 616d 6564 222c 2022 6163 636f  "renamed", "acco
+00015220: 756e 745f 6368 6563 6b5f 7072 696e 7469  unt_check_printi
+00015230: 6e67 2229 2c0a 2020 2020 2822 6163 636f  ng"),.    ("acco
+00015240: 756e 745f 666f 6c6c 6f77 7570 222c 2022  unt_followup", "
+00015250: 7265 6d6f 7665 6422 292c 0a20 2020 2028  removed"),.    (
+00015260: 0a20 2020 2020 2020 2022 6163 636f 756e  .        "accoun
+00015270: 745f 7061 796d 656e 7422 2c0a 2020 2020  t_payment",.    
+00015280: 2020 2020 226f 6361 5f6d 6f76 6564 222c      "oca_moved",
+00015290: 0a20 2020 2020 2020 2022 6163 636f 756e  .        "accoun
+000152a0: 745f 7061 796d 656e 745f 6f72 6465 7222  t_payment_order"
+000152b0: 2c0a 2020 2020 2020 2020 224d 6f76 6564  ,.        "Moved
+000152c0: 2074 6f20 4f43 412f 6261 6e6b 2d70 6179   to OCA/bank-pay
+000152d0: 6d65 6e74 222c 0a20 2020 2029 2c0a 2020  ment",.    ),.  
+000152e0: 2020 2822 6163 636f 756e 745f 7365 7175    ("account_sequ
+000152f0: 656e 6365 222c 2022 7265 6d6f 7665 6422  ence", "removed"
+00015300: 292c 0a20 2020 2028 2261 6e61 6c79 7469  ),.    ("analyti
+00015310: 635f 636f 6e74 7261 6374 5f68 725f 6578  c_contract_hr_ex
+00015320: 7065 6e73 6522 2c20 2272 656d 6f76 6564  pense", "removed
+00015330: 2229 2c0a 2020 2020 2822 616e 616c 7974  "),.    ("analyt
+00015340: 6963 5f75 7365 725f 6675 6e63 7469 6f6e  ic_user_function
+00015350: 222c 2022 7265 6d6f 7665 6422 292c 0a20  ", "removed"),. 
+00015360: 2020 2028 2261 6e67 6c6f 5f73 6178 6f6e     ("anglo_saxon
+00015370: 5f64 726f 7073 6869 7070 696e 6722 2c20  _dropshipping", 
+00015380: 2272 656d 6f76 6564 2229 2c0a 2020 2020  "removed"),.    
+00015390: 2822 6175 7468 5f6f 7065 6e69 6422 2c20  ("auth_openid", 
+000153a0: 2272 656d 6f76 6564 2229 2c0a 2020 2020  "removed"),.    
+000153b0: 2822 6261 7365 5f72 6570 6f72 745f 6465  ("base_report_de
+000153c0: 7369 676e 6572 222c 2022 7265 6d6f 7665  signer", "remove
+000153d0: 6422 292c 0a20 2020 2028 2263 6f6e 7461  d"),.    ("conta
+000153e0: 6374 7322 2c20 226d 6572 6765 6422 2c20  cts", "merged", 
+000153f0: 226d 6169 6c22 292c 0a20 2020 2028 2263  "mail"),.    ("c
+00015400: 726d 5f68 656c 7064 6573 6b22 2c20 2272  rm_helpdesk", "r
+00015410: 656d 6f76 6564 2229 2c0a 2020 2020 2822  emoved"),.    ("
+00015420: 6372 6d5f 6d61 7373 5f6d 6169 6c69 6e67  crm_mass_mailing
+00015430: 222c 2022 7265 6d6f 7665 6422 292c 0a20  ", "removed"),. 
+00015440: 2020 2028 2263 726d 5f70 726f 6669 6c69     ("crm_profili
+00015450: 6e67 222c 2022 7265 6d6f 7665 6422 292c  ng", "removed"),
+00015460: 0a20 2020 2028 2265 6469 222c 2022 7265  .    ("edi", "re
+00015470: 6d6f 7665 6422 292c 0a20 2020 2028 2265  moved"),.    ("e
+00015480: 6d61 696c 5f74 656d 706c 6174 6522 2c20  mail_template", 
+00015490: 226d 6572 6765 6422 2c20 226d 6169 6c5f  "merged", "mail_
+000154a0: 7465 6d70 6c61 7465 2229 2c0a 2020 2020  template"),.    
+000154b0: 2822 6872 5f61 7070 6c69 6361 6e74 5f64  ("hr_applicant_d
+000154c0: 6f63 756d 656e 7422 2c20 2272 656d 6f76  ocument", "remov
+000154d0: 6564 2229 2c0a 2020 2020 2822 6872 5f74  ed"),.    ("hr_t
+000154e0: 696d 6573 6865 6574 5f69 6e76 6f69 6365  imesheet_invoice
+000154f0: 222c 2022 7265 6d6f 7665 6422 292c 0a20  ", "removed"),. 
+00015500: 2020 2028 2269 6d5f 6368 6174 222c 2022     ("im_chat", "
+00015510: 6d65 7267 6564 222c 2022 6d61 696c 2229  merged", "mail")
+00015520: 2c0a 2020 2020 2822 6b6e 6f77 6c65 6467  ,.    ("knowledg
+00015530: 6522 2c20 226f 6361 5f6d 6f76 6564 222c  e", "oca_moved",
+00015540: 2022 6b6e 6f77 6c65 6467 6522 2c20 224d   "knowledge", "M
+00015550: 6f76 6564 2074 6f20 4f43 412f 6b6e 6f77  oved to OCA/know
+00015560: 6c65 6467 6522 292c 0a20 2020 2028 226c  ledge"),.    ("l
+00015570: 3130 6e5f 6265 5f63 6f64 6122 2c20 2272  10n_be_coda", "r
+00015580: 656d 6f76 6564 2229 2c0a 2020 2020 2822  emoved"),.    ("
+00015590: 6c31 306e 5f66 725f 7269 6222 2c20 2272  l10n_fr_rib", "r
+000155a0: 656d 6f76 6564 2229 2c0a 2020 2020 2822  emoved"),.    ("
+000155b0: 6d61 726b 6574 696e 675f 6372 6d22 2c20  marketing_crm", 
+000155c0: 226d 6572 6765 6422 2c20 2263 726d 2229  "merged", "crm")
+000155d0: 2c0a 2020 2020 2822 6d75 6c74 695f 636f  ,.    ("multi_co
+000155e0: 6d70 616e 7922 2c20 2272 656d 6f76 6564  mpany", "removed
+000155f0: 2229 2c0a 2020 2020 2822 706f 7274 616c  "),.    ("portal
+00015600: 5f63 6c61 696d 222c 2022 7265 6e61 6d65  _claim", "rename
+00015610: 6422 2c20 2277 6562 7369 7465 5f63 726d  d", "website_crm
+00015620: 5f63 6c61 696d 2229 2c0a 2020 2020 2822  _claim"),.    ("
+00015630: 706f 7274 616c 5f70 726f 6a65 6374 222c  portal_project",
+00015640: 2022 6d65 7267 6564 222c 2022 7072 6f6a   "merged", "proj
+00015650: 6563 7422 292c 0a20 2020 2028 2270 6f72  ect"),.    ("por
+00015660: 7461 6c5f 7072 6f6a 6563 745f 6973 7375  tal_project_issu
+00015670: 6522 2c20 226d 6572 6765 6422 2c20 2270  e", "merged", "p
+00015680: 726f 6a65 6374 5f69 7373 7565 2229 2c0a  roject_issue"),.
+00015690: 2020 2020 2822 7072 6f63 7572 656d 656e      ("procuremen
+000156a0: 745f 6a69 745f 7374 6f63 6b22 2c20 226d  t_jit_stock", "m
+000156b0: 6572 6765 6422 2c20 2270 726f 6375 7265  erged", "procure
+000156c0: 6d65 6e74 5f6a 6974 2229 2c0a 2020 2020  ment_jit"),.    
+000156d0: 280a 2020 2020 2020 2020 2270 7572 6368  (.        "purch
+000156e0: 6173 655f 616e 616c 7974 6963 5f70 6c61  ase_analytic_pla
+000156f0: 6e73 222c 0a20 2020 2020 2020 2022 6f63  ns",.        "oc
+00015700: 615f 6d6f 7665 6422 2c0a 2020 2020 2020  a_moved",.      
+00015710: 2020 2270 7572 6368 6173 655f 616e 616c    "purchase_anal
+00015720: 7974 6963 5f64 6973 7472 6962 7574 696f  ytic_distributio
+00015730: 6e22 2c0a 2020 2020 2020 2020 224d 6f76  n",.        "Mov
+00015740: 6564 2074 6f20 4f43 412f 6163 636f 756e  ed to OCA/accoun
+00015750: 742d 616e 616c 7974 6963 222c 0a20 2020  t-analytic",.   
+00015760: 2029 2c0a 2020 2020 2822 7075 7263 6861   ),.    ("purcha
+00015770: 7365 5f64 6f75 626c 655f 7661 6c69 6461  se_double_valida
+00015780: 7469 6f6e 222c 2022 7265 6d6f 7665 6422  tion", "removed"
+00015790: 292c 0a20 2020 2028 0a20 2020 2020 2020  ),.    (.       
+000157a0: 2022 7361 6c65 5f61 6e61 6c79 7469 635f   "sale_analytic_
+000157b0: 706c 616e 7322 2c0a 2020 2020 2020 2020  plans",.        
+000157c0: 226f 6361 5f6d 6f76 6564 222c 0a20 2020  "oca_moved",.   
+000157d0: 2020 2020 2022 7361 6c65 5f61 6e61 6c79       "sale_analy
+000157e0: 7469 635f 6469 7374 7269 6275 7469 6f6e  tic_distribution
+000157f0: 222c 0a20 2020 2020 2020 2022 4d6f 7665  ",.        "Move
+00015800: 6420 746f 204f 4341 2f61 6363 6f75 6e74  d to OCA/account
+00015810: 2d61 6e61 6c79 7469 6322 2c0a 2020 2020  -analytic",.    
+00015820: 292c 0a20 2020 2028 2273 616c 655f 6a6f  ),.    ("sale_jo
+00015830: 7572 6e61 6c22 2c20 2272 656d 6f76 6564  urnal", "removed
+00015840: 2229 2c0a 2020 2020 2822 7368 6172 6522  "),.    ("share"
+00015850: 2c20 2272 656d 6f76 6564 2229 2c0a 2020  , "removed"),.  
+00015860: 2020 2822 7374 6f63 6b5f 696e 766f 6963    ("stock_invoic
+00015870: 655f 6469 7265 6374 6c79 222c 2022 7265  e_directly", "re
+00015880: 6d6f 7665 6422 292c 0a20 2020 2028 2277  moved"),.    ("w
+00015890: 6562 5f61 7069 222c 2022 7265 6d6f 7665  eb_api", "remove
+000158a0: 6422 292c 0a20 2020 2028 2277 6562 5f67  d"),.    ("web_g
+000158b0: 616e 7474 222c 2022 6d65 7267 6564 222c  antt", "merged",
+000158c0: 2022 7765 6222 292c 0a20 2020 2028 2277   "web"),.    ("w
+000158d0: 6562 5f67 7261 7068 222c 2022 6d65 7267  eb_graph", "merg
+000158e0: 6564 222c 2022 7765 6222 292c 0a20 2020  ed", "web"),.   
+000158f0: 2028 2277 6562 5f6b 616e 6261 6e5f 7370   ("web_kanban_sp
+00015900: 6172 6b6c 696e 6522 2c20 226d 6572 6765  arkline", "merge
+00015910: 6422 2c20 2277 6562 2229 2c0a 2020 2020  d", "web"),.    
+00015920: 2822 7765 625f 7465 7374 7322 2c20 226d  ("web_tests", "m
+00015930: 6572 6765 6422 2c20 2277 6562 2229 2c0a  erged", "web"),.
+00015940: 2020 2020 2822 7765 625f 7465 7374 735f      ("web_tests_
+00015950: 6465 6d6f 222c 2022 7265 6d6f 7665 6422  demo", "removed"
+00015960: 292c 0a20 2020 2028 2277 6562 7369 7465  ),.    ("website
+00015970: 5f63 6572 7469 6669 6361 7469 6f6e 222c  _certification",
+00015980: 2022 7265 6d6f 7665 6422 292c 0a20 2020   "removed"),.   
+00015990: 2028 2277 6562 7369 7465 5f69 6e73 7461   ("website_insta
+000159a0: 6e74 636c 6963 6b22 2c20 2272 656d 6f76  ntclick", "remov
+000159b0: 6564 2229 2c0a 2020 2020 2822 7765 6273  ed"),.    ("webs
+000159c0: 6974 655f 6d61 696c 5f67 726f 7570 222c  ite_mail_group",
+000159d0: 2022 7265 6e61 6d65 6422 2c20 2277 6562   "renamed", "web
+000159e0: 7369 7465 5f6d 6169 6c5f 6368 616e 6e65  site_mail_channe
+000159f0: 6c22 292c 0a20 2020 2028 2277 6562 7369  l"),.    ("websi
+00015a00: 7465 5f72 6570 6f72 7422 2c20 226d 6572  te_report", "mer
+00015a10: 6765 6422 2c20 2272 6570 6f72 7422 292c  ged", "report"),
+00015a20: 0a5d 0a0a 6966 205f 5f6e 616d 655f 5f20  .]..if __name__ 
+00015a30: 3d3d 2022 5f5f 6d61 696e 5f5f 223a 0a20  == "__main__":. 
+00015a40: 2020 2070 6172 7365 7220 3d20 7a30 6c69     parser = z0li
+00015a50: 622e 7061 7273 656f 7074 6172 6773 280a  b.parseoptargs(.
+00015a60: 2020 2020 2020 2020 224d 6967 7261 7465          "Migrate
+00015a70: 204f 646f 6f20 4442 222c 2022 c2a9 2032   Odoo DB", ".. 2
+00015a80: 3031 392d 3231 2062 7920 5348 532d 4156  019-21 by SHS-AV
+00015a90: 2073 2e72 2e6c 2e22 2c20 7665 7273 696f   s.r.l.", versio
+00015aa0: 6e3d 5f5f 7665 7273 696f 6e5f 5f0a 2020  n=__version__.  
+00015ab0: 2020 290a 2020 2020 7061 7273 6572 2e61    ).    parser.a
+00015ac0: 6464 5f61 7267 756d 656e 7428 272d 6827  dd_argument('-h'
+00015ad0: 290a 2020 2020 7061 7273 6572 2e61 6464  ).    parser.add
+00015ae0: 5f61 7267 756d 656e 7428 0a20 2020 2020  _argument(.     
+00015af0: 2020 2022 2d42 222c 0a20 2020 2020 2020     "-B",.       
+00015b00: 2022 2d2d 6f70 656e 7570 6772 6164 652d   "--openupgrade-
+00015b10: 6272 616e 6368 2d70 6174 6822 2c0a 2020  branch-path",.  
+00015b20: 2020 2020 2020 6865 6c70 3d22 6f70 656e        help="open
+00015b30: 7570 6772 6164 6520 6272 616e 6368 2070  upgrade branch p
+00015b40: 6174 6822 2c0a 2020 2020 2020 2020 6465  ath",.        de
+00015b50: 7374 3d22 6f70 745f 6f75 7061 7468 222c  st="opt_oupath",
+00015b60: 0a20 2020 2020 2020 206d 6574 6176 6172  .        metavar
+00015b70: 3d22 7061 7468 222c 0a20 2020 2029 0a20  ="path",.    ). 
+00015b80: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
+00015b90: 6775 6d65 6e74 280a 2020 2020 2020 2020  gument(.        
+00015ba0: 272d 6227 2c20 272d 2d62 7261 6e63 6827  '-b', '--branch'
+00015bb0: 2c20 6163 7469 6f6e 3d27 7374 6f72 6527  , action='store'
+00015bc0: 2c20 6465 7374 3d27 6669 6e61 6c5f 6272  , dest='final_br
+00015bd0: 616e 6368 272c 206d 6574 6176 6172 3d27  anch', metavar='
+00015be0: 7665 7273 696f 6e27 0a20 2020 2029 0a20  version'.    ). 
+00015bf0: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
+00015c00: 6775 6d65 6e74 280a 2020 2020 2020 2020  gument(.        
+00015c10: 222d 4322 2c0a 2020 2020 2020 2020 222d  "-C",.        "-
+00015c20: 2d62 792d 636f 6d70 616e 7922 2c0a 2020  -by-company",.  
+00015c30: 2020 2020 2020 6163 7469 6f6e 3d22 7374        action="st
+00015c40: 6f72 655f 7472 7565 222c 0a20 2020 2020  ore_true",.     
+00015c50: 2020 2068 656c 703d 2273 656c 6563 7420     help="select 
+00015c60: 6f6e 6c79 2072 6563 6f72 6473 206f 6620  only records of 
+00015c70: 6d61 696e 2063 6f6d 7061 6e79 222c 0a20  main company",. 
+00015c80: 2020 2020 2020 2064 6573 743d 2262 795f         dest="by_
+00015c90: 636f 6d70 616e 7922 2c0a 2020 2020 290a  company",.    ).
+00015ca0: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
+00015cb0: 7267 756d 656e 7428 0a20 2020 2020 2020  rgument(.       
+00015cc0: 2022 2d63 222c 0a20 2020 2020 2020 2022   "-c",.        "
+00015cd0: 2d2d 7467 742d 636f 6e66 6967 222c 0a20  --tgt-config",. 
+00015ce0: 2020 2020 2020 2068 656c 703d 2274 6172         help="tar
+00015cf0: 6765 7420 4442 2063 6f6e 6669 6775 7261  get DB configura
+00015d00: 7469 6f6e 2066 696c 6522 2c0a 2020 2020  tion file",.    
+00015d10: 2020 2020 6465 7374 3d22 6669 6e61 6c5f      dest="final_
+00015d20: 636f 6e66 6e22 2c0a 2020 2020 2020 2020  confn",.        
+00015d30: 6d65 7461 7661 723d 2266 696c 6522 2c0a  metavar="file",.
+00015d40: 2020 2020 290a 2020 2020 7061 7273 6572      ).    parser
+00015d50: 2e61 6464 5f61 7267 756d 656e 7428 222d  .add_argument("-
+00015d60: 4422 2c20 222d 2d64 656c 2d64 622d 6966  D", "--del-db-if
+00015d70: 2d65 7869 7374 222c 2061 6374 696f 6e3d  -exist", action=
+00015d80: 2273 746f 7265 5f74 7275 6522 2c20 6465  "store_true", de
+00015d90: 7374 3d22 6f70 745f 6465 6c22 290a 2020  st="opt_del").  
+00015da0: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+00015db0: 756d 656e 7428 0a20 2020 2020 2020 2022  ument(.        "
+00015dc0: 2d64 222c 0a20 2020 2020 2020 2022 2d2d  -d",.        "--
+00015dd0: 7467 742d 6462 5f6e 616d 6522 2c0a 2020  tgt-db_name",.  
+00015de0: 2020 2020 2020 6865 6c70 3d22 7461 7267        help="targ
+00015df0: 6574 2064 6174 6162 6173 6520 6e61 6d65  et database name
+00015e00: 222c 0a20 2020 2020 2020 2064 6573 743d  ",.        dest=
+00015e10: 2266 696e 616c 5f64 626e 616d 6522 2c0a  "final_dbname",.
+00015e20: 2020 2020 2020 2020 6d65 7461 7661 723d          metavar=
+00015e30: 226e 616d 6522 2c0a 2020 2020 290a 2020  "name",.    ).  
+00015e40: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+00015e50: 756d 656e 7428 0a20 2020 2020 2020 2022  ument(.        "
+00015e60: 2d45 222c 0a20 2020 2020 2020 2022 2d2d  -E",.        "--
+00015e70: 6e6f 2d76 656e 7622 2c0a 2020 2020 2020  no-venv",.      
+00015e80: 2020 6865 6c70 3d22 6469 7361 626c 6520    help="disable 
+00015e90: 7669 7274 7561 6c65 6e76 222c 0a20 2020  virtualenv",.   
+00015ea0: 2020 2020 2061 6374 696f 6e3d 2773 746f       action='sto
+00015eb0: 7265 5f74 7275 6527 2c0a 2020 2020 2020  re_true',.      
+00015ec0: 2020 6465 7374 3d22 6e6f 5f76 656e 7622    dest="no_venv"
+00015ed0: 2c0a 2020 2020 290a 2020 2020 7061 7273  ,.    ).    pars
+00015ee0: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
+00015ef0: 0a20 2020 2020 2020 2027 2d46 272c 2027  .        '-F', '
+00015f00: 2d2d 6672 6f6d 2d6f 646f 6f2d 7665 7227  --from-odoo-ver'
+00015f10: 2c20 6163 7469 6f6e 3d27 7374 6f72 6527  , action='store'
+00015f20: 2c20 6465 7374 3d27 6672 6f6d 5f62 7261  , dest='from_bra
+00015f30: 6e63 6827 2c20 6d65 7461 7661 723d 2276  nch', metavar="v
+00015f40: 6572 220a 2020 2020 290a 2020 2020 7061  er".    ).    pa
+00015f50: 7273 6572 2e61 6464 5f61 7267 756d 656e  rser.add_argumen
+00015f60: 7428 0a20 2020 2020 2020 2022 2d49 222c  t(.        "-I",
+00015f70: 0a20 2020 2020 2020 2022 2d2d 696d 6167  .        "--imag
+00015f80: 6522 2c0a 2020 2020 2020 2020 6865 6c70  e",.        help
+00015f90: 3d22 696d 6167 6520 6d6f 6465 222c 0a20  ="image mode",. 
+00015fa0: 2020 2020 2020 2061 6374 696f 6e3d 2773         action='s
+00015fb0: 746f 7265 5f74 7275 6527 2c0a 2020 2020  tore_true',.    
+00015fc0: 2020 2020 6465 7374 3d22 696d 6167 655f      dest="image_
+00015fd0: 6d6f 6465 222c 0a20 2020 2020 2020 2064  mode",.        d
+00015fe0: 6566 6175 6c74 3d46 616c 7365 2c0a 2020  efault=False,.  
+00015ff0: 2020 290a 2020 2020 7061 7273 6572 2e61    ).    parser.a
+00016000: 6464 5f61 7267 756d 656e 7428 0a20 2020  dd_argument(.   
+00016010: 2020 2020 2022 2d69 222c 2022 2d2d 6964       "-i", "--id
+00016020: 7322 2c20 6865 6c70 3d22 6964 7320 746f  s", help="ids to
+00016030: 206d 6967 7261 7465 222c 2064 6573 743d   migrate", dest=
+00016040: 2273 656c 5f69 6473 222c 206d 6574 6176  "sel_ids", metav
+00016050: 6172 3d22 6c69 7374 220a 2020 2020 290a  ar="list".    ).
+00016060: 2020 2020 7061 7273 6572 2e61 6464 5f61      parser.add_a
+00016070: 7267 756d 656e 7428 0a20 2020 2020 2020  rgument(.       
+00016080: 2022 2d4a 222c 0a20 2020 2020 2020 2022   "-J",.        "
+00016090: 2d2d 7472 792d 7265 696e 7374 616c 6c22  --try-reinstall"
+000160a0: 2c0a 2020 2020 2020 2020 6865 6c70 3d22  ,.        help="
+000160b0: 7472 7920 746f 2072 6569 6e73 7461 6c6c  try to reinstall
+000160c0: 222c 0a20 2020 2020 2020 2061 6374 696f  ",.        actio
+000160d0: 6e3d 2773 746f 7265 5f74 7275 6527 2c0a  n='store_true',.
+000160e0: 2020 2020 2020 2020 6465 7374 3d22 7472          dest="tr
+000160f0: 795f 7265 696e 7374 616c 6c22 2c0a 2020  y_reinstall",.  
+00016100: 2020 2020 2020 6465 6661 756c 743d 4661        default=Fa
+00016110: 6c73 652c 0a20 2020 2029 0a20 2020 2070  lse,.    ).    p
+00016120: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+00016130: 6e74 280a 2020 2020 2020 2020 222d 4b22  nt(.        "-K"
+00016140: 2c0a 2020 2020 2020 2020 222d 2d63 6f6d  ,.        "--com
+00016150: 6d61 6e64 2d66 696c 6522 2c0a 2020 2020  mand-file",.    
+00016160: 2020 2020 6865 6c70 3d22 6d69 6772 6174      help="migrat
+00016170: 696f 6e20 636f 6d6d 616e 6420 6669 6c65  ion command file
+00016180: 222c 0a20 2020 2020 2020 2064 6573 743d  ",.        dest=
+00016190: 2263 6f6d 6d61 6e64 5f66 696c 6522 2c0a  "command_file",.
+000161a0: 2020 2020 2020 2020 6d65 7461 7661 723d          metavar=
+000161b0: 2266 696c 6522 2c0a 2020 2020 2020 2020  "file",.        
+000161c0: 6465 6661 756c 743d 272e 2f6d 6967 7261  default='./migra
+000161d0: 7465 5f6f 646f 6f2e 6373 7627 2c0a 2020  te_odoo.csv',.  
+000161e0: 2020 290a 2020 2020 7061 7273 6572 2e61    ).    parser.a
+000161f0: 6464 5f61 7267 756d 656e 7428 0a20 2020  dd_argument(.   
+00016200: 2020 2020 2022 2d6b 222c 0a20 2020 2020       "-k",.     
+00016210: 2020 2022 2d2d 6465 6661 756c 742d 6265     "--default-be
+00016220: 6861 7669 6f72 222c 0a20 2020 2020 2020  havior",.       
+00016230: 2068 656c 703d 2264 6566 6175 6c74 2062   help="default b
+00016240: 6568 6176 696f 7222 2c0a 2020 2020 2020  ehavior",.      
+00016250: 2020 6163 7469 6f6e 3d22 7374 6f72 655f    action="store_
+00016260: 7472 7565 222c 0a20 2020 2020 2020 2064  true",.        d
+00016270: 6573 743d 2264 6566 6175 6c74 5f62 6568  est="default_beh
+00016280: 6176 696f 7222 2c0a 2020 2020 290a 2020  avior",.    ).  
+00016290: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+000162a0: 756d 656e 7428 0a20 2020 2020 2020 2022  ument(.        "
+000162b0: 2d6c 222c 2022 2d2d 6669 6c65 2d6c 6f67  -l", "--file-log
+000162c0: 222c 2068 656c 703d 226c 6f67 2066 696c  ", help="log fil
+000162d0: 6522 2c20 6465 7374 3d22 6c6f 6766 6e22  e", dest="logfn"
+000162e0: 2c20 6d65 7461 7661 723d 2266 696c 6522  , metavar="file"
+000162f0: 0a20 2020 2029 0a20 2020 2070 6172 7365  .    ).    parse
+00016300: 722e 6164 645f 6172 6775 6d65 6e74 280a  r.add_argument(.
+00016310: 2020 2020 2020 2020 222d 4d22 2c0a 2020          "-M",.  
+00016320: 2020 2020 2020 222d 2d6f 6361 2d6d 6967        "--oca-mig
+00016330: 7261 7465 222c 0a20 2020 2020 2020 2061  rate",.        a
+00016340: 6374 696f 6e3d 2273 746f 7265 5f74 7275  ction="store_tru
+00016350: 6522 2c0a 2020 2020 2020 2020 6465 7374  e",.        dest
+00016360: 3d22 6f63 615f 6d69 6772 6174 6522 2c0a  ="oca_migrate",.
+00016370: 2020 2020 2020 2020 6865 6c70 3d22 7573          help="us
+00016380: 6520 4f43 4120 6d69 6772 6174 6520 2866  e OCA migrate (f
+00016390: 696e 616c 2076 6572 7369 6f6e 203c 2031  inal version < 1
+000163a0: 302e 3029 222c 0a20 2020 2029 0a20 2020  0.0)",.    ).   
+000163b0: 2070 6172 7365 722e 6164 645f 6172 6775   parser.add_argu
+000163c0: 6d65 6e74 280a 2020 2020 2020 2020 222d  ment(.        "-
+000163d0: 6d22 2c20 222d 2d73 656c 2d6d 6f64 656c  m", "--sel-model
+000163e0: 222c 2068 656c 703d 226d 6f64 656c 2074  ", help="model t
+000163f0: 6f20 6d69 6772 6174 6522 2c20 6465 7374  o migrate", dest
+00016400: 3d22 7365 6c5f 6d6f 6465 6c22 2c20 6d65  ="sel_model", me
+00016410: 7461 7661 723d 226e 616d 6522 0a20 2020  tavar="name".   
+00016420: 2029 0a20 2020 2070 6172 7365 722e 6164   ).    parser.ad
+00016430: 645f 6172 6775 6d65 6e74 2827 2d6e 2729  d_argument('-n')
+00016440: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
+00016450: 6172 6775 6d65 6e74 280a 2020 2020 2020  argument(.      
+00016460: 2020 222d 4f22 2c0a 2020 2020 2020 2020    "-O",.        
+00016470: 222d 2d6f 7065 6e75 7067 7261 6465 6c69  "--openupgradeli
+00016480: 622d 7061 7468 222c 0a20 2020 2020 2020  b-path",.       
+00016490: 2068 656c 703d 224f 7065 6e75 7067 7261   help="Openupgra
+000164a0: 6465 6c69 6220 7061 7468 222c 0a20 2020  delib path",.   
+000164b0: 2020 2020 2064 6573 743d 226f 7074 5f6f       dest="opt_o
+000164c0: 756c 7061 7468 222c 0a20 2020 2020 2020  ulpath",.       
+000164d0: 206d 6574 6176 6172 3d22 7061 7468 222c   metavar="path",
+000164e0: 0a20 2020 2029 0a20 2020 2070 6172 7365  .    ).    parse
+000164f0: 722e 6164 645f 6172 6775 6d65 6e74 2827  r.add_argument('
+00016500: 2d71 2729 0a20 2020 2070 6172 7365 722e  -q').    parser.
+00016510: 6164 645f 6172 6775 6d65 6e74 280a 2020  add_argument(.  
+00016520: 2020 2020 2020 222d 5222 2c0a 2020 2020        "-R",.    
+00016530: 2020 2020 222d 2d72 6564 7563 7465 642d      "--reducted-
+00016540: 6d6f 6475 6c65 2d73 6574 222c 0a20 2020  module-set",.   
+00016550: 2020 2020 2061 6374 696f 6e3d 2773 746f       action='sto
+00016560: 7265 5f74 7275 6527 2c0a 2020 2020 2020  re_true',.      
+00016570: 2020 6465 7374 3d22 7265 6475 6374 6564    dest="reducted
+00016580: 5f6d 6f64 756c 655f 7365 7422 2c0a 2020  _module_set",.  
+00016590: 2020 2020 2020 6465 6661 756c 743d 4661        default=Fa
+000165a0: 6c73 652c 0a20 2020 2029 0a20 2020 2070  lse,.    ).    p
+000165b0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+000165c0: 6e74 280a 2020 2020 2020 2020 222d 5322  nt(.        "-S"
+000165d0: 2c20 222d 2d73 6166 652d 6d6f 6465 222c  , "--safe-mode",
+000165e0: 2061 6374 696f 6e3d 2273 746f 7265 5f74   action="store_t
+000165f0: 7275 6522 2c20 6465 7374 3d22 6f70 745f  rue", dest="opt_
+00016600: 7361 6665 222c 2068 656c 703d 2273 6166  safe", help="saf
+00016610: 6520 6d6f 6465 220a 2020 2020 290a 2020  e mode".    ).  
+00016620: 2020 7061 7273 6572 2e61 6464 5f61 7267    parser.add_arg
+00016630: 756d 656e 7428 0a20 2020 2020 2020 2022  ument(.        "
+00016640: 2d73 222c 0a20 2020 2020 2020 2022 2d2d  -s",.        "--
+00016650: 7573 652d 7379 6e63 6872 6f22 2c0a 2020  use-synchro",.  
+00016660: 2020 2020 2020 6865 6c70 3d22 7573 6520        help="use 
+00016670: 6d6f 6475 6c65 2073 796e 6368 726f 222c  module synchro",
+00016680: 0a20 2020 2020 2020 2061 6374 696f 6e3d  .        action=
+00016690: 2773 746f 7265 5f74 7275 6527 2c0a 2020  'store_true',.  
+000166a0: 2020 2020 2020 6465 7374 3d22 7573 655f        dest="use_
+000166b0: 7379 6e63 6872 6f22 2c0a 2020 2020 2020  synchro",.      
+000166c0: 2020 6465 6661 756c 743d 4661 6c73 652c    default=False,
+000166d0: 0a20 2020 2029 0a20 2020 2070 6172 7365  .    ).    parse
+000166e0: 722e 6164 645f 6172 6775 6d65 6e74 280a  r.add_argument(.
+000166f0: 2020 2020 2020 2020 222d 5422 2c0a 2020          "-T",.  
+00016700: 2020 2020 2020 222d 2d75 7064 2d74 7261        "--upd-tra
+00016710: 6e73 6c61 7469 6f6e 222c 0a20 2020 2020  nslation",.     
+00016720: 2020 2061 6374 696f 6e3d 2773 746f 7265     action='store
+00016730: 5f74 7275 6527 2c0a 2020 2020 2020 2020  _true',.        
+00016740: 6465 7374 3d22 7570 645f 7472 616e 736c  dest="upd_transl
+00016750: 6174 696f 6e22 2c0a 2020 2020 2020 2020  ation",.        
+00016760: 6465 6661 756c 743d 4661 6c73 652c 0a20  default=False,. 
+00016770: 2020 2029 0a20 2020 2070 6172 7365 722e     ).    parser.
+00016780: 6164 645f 6172 6775 6d65 6e74 280a 2020  add_argument(.  
+00016790: 2020 2020 2020 222d 5522 2c0a 2020 2020        "-U",.    
+000167a0: 2020 2020 222d 2d75 7365 7222 2c0a 2020      "--user",.  
+000167b0: 2020 2020 2020 6865 6c70 3d22 6c6f 6769        help="logi
+000167c0: 6e20 7573 6572 6e61 6d65 222c 0a20 2020  n username",.   
+000167d0: 2020 2020 2064 6573 743d 226c 6769 5f75       dest="lgi_u
+000167e0: 7365 7222 2c0a 2020 2020 2020 2020 6d65  ser",.        me
+000167f0: 7461 7661 723d 2275 7365 726e 616d 6522  tavar="username"
+00016800: 2c0a 2020 2020 2020 2020 6465 6661 756c  ,.        defaul
+00016810: 743d 2261 646d 696e 222c 0a20 2020 2029  t="admin",.    )
+00016820: 0a20 2020 2070 6172 7365 722e 6164 645f  .    parser.add_
+00016830: 6172 6775 6d65 6e74 2827 2d56 2729 0a20  argument('-V'). 
+00016840: 2020 2070 6172 7365 722e 6164 645f 6172     parser.add_ar
+00016850: 6775 6d65 6e74 2827 2d76 2729 0a20 2020  gument('-v').   
+00016860: 2070 6172 7365 722e 6164 645f 6172 6775   parser.add_argu
+00016870: 6d65 6e74 280a 2020 2020 2020 2020 222d  ment(.        "-
+00016880: 5722 2c0a 2020 2020 2020 2020 222d 2d77  W",.        "--w
+00016890: 6570 2d6c 6f67 222c 0a20 2020 2020 2020  ep-log",.       
+000168a0: 2068 656c 703d 2264 656c 206c 6f67 7320   help="del logs 
+000168b0: 6265 666f 7265 206d 6967 7261 7469 6f6e  before migration
+000168c0: 222c 0a20 2020 2020 2020 2061 6374 696f  ",.        actio
+000168d0: 6e3d 2773 746f 7265 5f74 7275 6527 2c0a  n='store_true',.
+000168e0: 2020 2020 2020 2020 6465 7374 3d22 7765          dest="we
+000168f0: 705f 6c6f 6773 222c 0a20 2020 2020 2020  p_logs",.       
+00016900: 2064 6566 6175 6c74 3d46 616c 7365 2c0a   default=False,.
+00016910: 2020 2020 290a 2020 2020 7061 7273 6572      ).    parser
+00016920: 2e61 6464 5f61 7267 756d 656e 7428 0a20  .add_argument(. 
+00016930: 2020 2020 2020 2022 2d77 222c 0a20 2020         "-w",.   
+00016940: 2020 2020 2022 2d2d 7372 632d 636f 6e66       "--src-conf
+00016950: 6967 222c 0a20 2020 2020 2020 2068 656c  ig",.        hel
+00016960: 703d 2273 6f75 7263 6520 4442 2063 6f6e  p="source DB con
+00016970: 6669 6775 7261 7469 6f6e 2066 696c 6522  figuration file"
+00016980: 2c0a 2020 2020 2020 2020 6465 7374 3d22  ,.        dest="
+00016990: 6672 6f6d 5f63 6f6e 666e 222c 0a20 2020  from_confn",.   
+000169a0: 2020 2020 206d 6574 6176 6172 3d22 6669       metavar="fi
+000169b0: 6c65 222c 0a20 2020 2029 0a20 2020 2070  le",.    ).    p
+000169c0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+000169d0: 6e74 280a 2020 2020 2020 2020 222d 5922  nt(.        "-Y"
+000169e0: 2c0a 2020 2020 2020 2020 222d 2d75 6e69  ,.        "--uni
+000169f0: 6e73 7461 6c6c 2d6d 6f64 756c 6573 222c  nstall-modules",
+00016a00: 0a20 2020 2020 2020 2068 656c 703d 226d  .        help="m
+00016a10: 6f64 756c 6573 2074 6f20 756e 696e 7374  odules to uninst
+00016a20: 616c 6c61 2062 6566 6f72 6520 6d69 6772  alla before migr
+00016a30: 6174 696f 6e22 2c0a 2020 2020 2020 2020  ation",.        
+00016a40: 6465 7374 3d22 756e 696e 7374 616c 6c5f  dest="uninstall_
+00016a50: 6d6f 6475 6c65 7322 2c0a 2020 2020 2020  modules",.      
+00016a60: 2020 6d65 7461 7661 723d 226c 6973 7422    metavar="list"
+00016a70: 2c0a 2020 2020 290a 2020 2020 7061 7273  ,.    ).    pars
+00016a80: 6572 2e61 6464 5f61 7267 756d 656e 7428  er.add_argument(
+00016a90: 0a20 2020 2020 2020 2022 2d79 222c 0a20  .        "-y",. 
+00016aa0: 2020 2020 2020 2022 2d2d 6173 7375 6d65         "--assume
+00016ab0: 2d79 6573 222c 0a20 2020 2020 2020 2068  -yes",.        h
+00016ac0: 656c 703d 2261 7373 756d 6520 7965 7322  elp="assume yes"
+00016ad0: 2c0a 2020 2020 2020 2020 6163 7469 6f6e  ,.        action
+00016ae0: 3d27 7374 6f72 655f 7472 7565 272c 0a20  ='store_true',. 
+00016af0: 2020 2020 2020 2064 6573 743d 2261 7373         dest="ass
+00016b00: 756d 655f 7965 7322 2c0a 2020 2020 2020  ume_yes",.      
+00016b10: 2020 6465 6661 756c 743d 4661 6c73 652c    default=False,
+00016b20: 0a20 2020 2029 0a20 2020 2070 6172 7365  .    ).    parse
+00016b30: 722e 6164 645f 6172 6775 6d65 6e74 280a  r.add_argument(.
+00016b40: 2020 2020 2020 2020 222d 7a22 2c0a 2020          "-z",.  
+00016b50: 2020 2020 2020 222d 2d73 7263 2d64 625f        "--src-db_
+00016b60: 6e61 6d65 222c 0a20 2020 2020 2020 2068  name",.        h
+00016b70: 656c 703d 2273 6f75 7263 6520 6461 7461  elp="source data
+00016b80: 6261 7365 206e 616d 6522 2c0a 2020 2020  base name",.    
+00016b90: 2020 2020 6465 7374 3d22 6672 6f6d 5f64      dest="from_d
+00016ba0: 626e 616d 6522 2c0a 2020 2020 2020 2020  bname",.        
+00016bb0: 6d65 7461 7661 723d 226e 616d 6522 2c0a  metavar="name",.
+00016bc0: 2020 2020 290a 2020 2020 7061 7273 6572      ).    parser
+00016bd0: 2e61 6464 5f61 7267 756d 656e 7428 0a20  .add_argument(. 
+00016be0: 2020 2020 2020 2022 2d31 222c 2022 2d2d         "-1", "--
+00016bf0: 646f 2d70 6173 7331 222c 2068 656c 703d  do-pass1", help=
+00016c00: 2265 7865 6320 7061 7373 2031 222c 2061  "exec pass 1", a
+00016c10: 6374 696f 6e3d 2773 746f 7265 5f74 7275  ction='store_tru
+00016c20: 6527 2c20 6465 7374 3d22 7068 6173 655f  e', dest="phase_
+00016c30: 3122 0a20 2020 2029 0a0a 2020 2020 7372  1".    )..    sr
+00016c40: 635f 6374 7820 3d20 7061 7273 6572 2e70  c_ctx = parser.p
+00016c50: 6172 7365 6f70 7461 7267 7328 7379 732e  arseoptargs(sys.
+00016c60: 6172 6776 5b31 3a5d 2c20 6170 706c 795f  argv[1:], apply_
+00016c70: 636f 6e66 3d46 616c 7365 290a 2020 2020  conf=False).    
+00016c80: 7372 635f 6374 782c 2074 6774 5f63 7478  src_ctx, tgt_ctx
+00016c90: 203d 2070 6172 7365 5f63 7478 2873 7263   = parse_ctx(src
+00016ca0: 5f63 7478 290a 2020 2020 6966 2073 7263  _ctx).    if src
+00016cb0: 5f63 7478 5b27 7765 705f 6c6f 6773 275d  _ctx['wep_logs']
+00016cc0: 3a0a 2020 2020 2020 2020 7765 705f 6c6f  :.        wep_lo
+00016cd0: 6773 2873 7263 5f63 7478 290a 2020 2020  gs(src_ctx).    
+00016ce0: 6f73 302e 7365 745f 746c 6f67 5f66 696c  os0.set_tlog_fil
+00016cf0: 6528 7372 635f 6374 785b 276c 6f67 666e  e(src_ctx['logfn
+00016d00: 275d 2c20 6563 686f 3d54 7275 6529 0a20  '], echo=True). 
+00016d10: 2020 206f 7330 2e77 6c6f 6728 273d 2720     os0.wlog('=' 
+00016d20: 2a20 3830 290a 2020 2020 6f73 302e 776c  * 80).    os0.wl
+00016d30: 6f67 2822 4d69 6772 6174 696f 6e20 6461  og("Migration da
+00016d40: 7461 6261 7365 2025 7320 6265 6769 6e6e  tabase %s beginn
+00016d50: 696e 6720 2e2e 2e22 2c20 5f5f 7665 7273  ing ...", __vers
+00016d60: 696f 6e5f 5f29 0a20 2020 2069 6620 7372  ion__).    if sr
+00016d70: 635f 6374 785b 2773 656c 5f6d 6f64 656c  c_ctx['sel_model
+00016d80: 275d 3a0a 2020 2020 2020 2020 6d69 6772  ']:.        migr
+00016d90: 6174 655f 7365 6c5f 7461 626c 6573 2873  ate_sel_tables(s
+00016da0: 7263 5f63 7478 2c20 7467 745f 6374 7829  rc_ctx, tgt_ctx)
+00016db0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00016dc0: 2020 206d 6967 7261 7465 5f64 6174 6162     migrate_datab
+00016dd0: 6173 6528 7372 635f 6374 782c 2074 6774  ase(src_ctx, tgt
+00016de0: 5f63 7478 290a                           _ctx).
```

### Comparing `clodoo-2.0.5/clodoo/odoorc` & `clodoo-2.0.6/clodoo/odoorc`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # GIT_ORGID    Identification of git organization
 # GIT_ORGNM    Name of git organization of specific Odoo version
 # GIT_PROT     Git protocol (git or https)
 # GIT_URL      URL to download git project (ends with .git)
 # HOME         Specific Odoo repository directory (i.e /opt/odoo/11.0/l10n-italy)
 # INVALID_MODNAMES
 # INVALID_MODNAMES_RE
+# IS_MULTI     Odoo multi version/instance
 # LICENSE      License (AGPL or LGPL or OPL)
 # LCONFN       Local Configuration filename (+)
 # LPPORT       Long polling port
 # MAJVER       Major Odoo version
 # MANIFEST     Manifest filename (__openerp__.py or __manifest__.py)
 # OCB_SUBDIRS
 # OCB_SUBDIRS_RE
@@ -59,15 +60,15 @@
 # ODOO_GIT_ORGID    -> default git organization
 # ODOO_GIT_HOSTNAME -> git hostname (def github.com)
 # ODOO_GIT_PROT     -> default protocol (git|https) for default git organization
 # ODOO_GIT_SHORT    -> regex of git organizations with short name (def /(oca)/)
 # ODOO_GIT_MULTI    -> multi version environment
 #
 
-__version__=2.0.5
+__version__=2.0.6
 
 
 ODOO_FVERS="16\.0|15\.0|14\.0|13\.0|12\.0|11\.0|10\.0|9\.0|8\.0|7\.0|6\.1"
 ODOO_VERS="16|15|14|13|12|11|10|9|8|7|6"
 DEFMLIST="OCB account-analytic account-budgeting account-closing
  account-consolidation account-financial-reporting account-financial-tools
  account-fiscal-rule account-invoice-reporting account-invoicing
@@ -201,22 +202,32 @@
             [[ ! $r =~ $rex && ! $r =~ $INVALID_MODNAMES_RE ]] && REPOS=$r && PRJPATH=$1
         fi
     fi
     echo "$PKGNAME|$PKGPATH|$PARENTDIR|$REPOS|$PRJPATH"
 }
 
 build_odoo_param() {
-    # build_odoo_param(ALL|BIN|CONFN|DB_USER|DDIR|DIRLEVEL|FLOG|FPID|FULLVER|FULL_SVCNAME|GIT_BRANCH|GIT_OPTS|GIT_ORG|GIT_ORGNM|GIT_PROT|GIT_URL|HOME|INVALID_MODNAMES|INVALID_MODNAMES_RE|LICENSE|LCONFN|LPPORT|MAJVER|MANIFEST|OCB_SUBDIRS|OCB_SUBDIRS_RE|OPTS_ASM|PARENTDIR|PKGNAME|PKGPATH|REPOS|ROOT|RORIGIN|RPCPORT|RUPSTREAM|SESS_PATH|SVCNAME|UPSTREAM|URL|URL_BRANCH|USER|VCS|VDIR|VENV
+    # build_odoo_param(ALL|BIN|CONFN|DB_USER|DDIR|DIRLEVEL|FLOG|FPID|FULLVER|FULL_SVCNAME|GIT_BRANCH|GIT_OPTS|GIT_ORG|GIT_ORGNM|GIT_PROT|GIT_URL|HOME|INVALID_MODNAMES|INVALID_MODNAMES_RE|IS_MULTI|LICENSE|LCONFN|LPPORT|MAJVER|MANIFEST|OCB_SUBDIRS|OCB_SUBDIRS_RE|OPTS_ASM|PARENTDIR|PKGNAME|PKGPATH|REPOS|ROOT|RORIGIN|RPCPORT|RUPSTREAM|SESS_PATH|SVCNAME|UPSTREAM|URL|URL_BRANCH|USER|VCS|VDIR|VENV
     #                  vid [(search|DEBUG|default|tree|SERVER|<rptname>|<modname>)] [oca|zero|zero-http|zero-git|librerp|flectra] [(search|DEBUG|default|tree|SERVER)])
     [[ :$SHELLOPTS: =~ :xtrace: ]] && set +x && local SETX="set -x"
     if [[ $1 =~ (INVALID_MODNAMES|INVALID_MODNAMES_RE|OCB_SUBDIRS|OCB_SUBDIRS_RE) ]]; then
         echo "${!1}"
         $SETX
         return
     fi
+    if [[ $1 == "IS_MULTI" ]]; then
+        if [[ -n $ODOO_ODOO_GIT_MULTI ]]; then
+          echo $ODOO_GIT_MULTI
+        else
+          discover_multi
+          echo "${opt_multi}"
+        fi
+        $SETX
+        return
+    fi
     [[ $1 == "_VER" ]] && echo $__version__ && return
     [[ $1 == "_FILE" ]] && echo ${BASH_SOURCE-} && return
     local ODOO_ROOT
     local VENV=0 main exorg spec
     local ITEM=$1 ROOT PARENTDIR PRJPATH
     local DIRLEVEL FULLVER LICENSE MAJVER odoo_vid noenv_vid MULTIVER REPOS
     local GIT_URL GIT_ORG GIT_ORGID GIT_ORGNM GIT_PROT GIT_OPTS ORGSFX OPTS_ASM
@@ -705,9 +716,25 @@
       [[ -z "$excl_list" || ! $fn =~ $excl_list ]] && res="$res $fn"
     done
     echo $res
 }
 
 
 if [ "${BASH_SOURCE-}" == "$0" ]; then
+    THIS=$(basename "$0")
+    TDIR=$(readlink -f $(dirname $0))
+    [ $BASH_VERSINFO -lt 4 ] && echo "This script $0 requires bash 4.0+!" && exit 4
+    if [[ -z $HOME_DEVEL || ! -d $HOME_DEVEL ]]; then
+      [[ -d $HOME/odoo/devel ]] && HOME_DEVEL="$HOME/odoo/devel" || HOME_DEVEL="$HOME/devel"
+    fi
+    [[ -x $TDIR/../bin/python3 ]] && PYTHON=$(readlink -f $TDIR/../bin/python3) || [[ -x $TDIR/python3 ]] && PYTHON="$TDIR/python3" || PYTHON=$(which python3 2>/dev/null) || PYTHON="python"
+    [[ -z $PYPATH ]] && PYPATH=$(echo -e "import os,sys\no=os.path\na=o.abspath\nj=o.join\nd=o.dirname\nb=o.basename\nf=o.isfile\np=o.isdir\nC=a('"$TDIR"')\nD='"$HOME_DEVEL"'\nif not p(D) and '/devel/' in C:\n D=C\n while b(D)!='devel':  D=d(D)\nN='venv_tools'\nU='setup.py'\nO='tools'\nH=o.expanduser('~')\nT=j(d(D),O)\nR=j(d(D),'pypi') if b(D)==N else j(D,'pypi')\nW=D if b(D)==N else j(D,'venv')\nS='site-packages'\nX='scripts'\ndef pt(P):\n P=a(P)\n if b(P) in (X,'tests','travis','_travis'):\n  P=d(P)\n if b(P)==b(d(P)) and f(j(P,'..',U)):\n  P=d(d(P))\n elif b(d(C))==O and f(j(P,U)):\n  P=d(P)\n return P\ndef ik(P):\n return P.startswith((H,D,K,W)) and p(P) and p(j(P,X)) and f(j(P,'__init__.py')) and f(j(P,'__main__.py'))\ndef ak(L,P):\n if P not in L:\n  L.append(P)\nL=[C]\nK=pt(C)\nfor B in ('z0lib','zerobug','clodoo','travis_emulator'):\n for P in [C]+sys.path+os.environ['PATH'].split(':')+[W,R,T]:\n  P=pt(P)\n  if B==b(P) and ik(P):\n   ak(L,P)\n   break\n  elif ik(j(P,B,B)):\n   ak(L,j(P,B,B))\n   break\n  elif ik(j(P,B)):\n   ak(L,j(P,B))\n   break\n  elif ik(j(P,S,B)):\n   ak(L,j(P,S,B))\n   break\nak(L,os.getcwd())\nprint(' '.join(L))\n"|$PYTHON)
+    [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "PYPATH=$PYPATH"
+    for d in $PYPATH /etc; do
+      if [[ -e $d/z0librc ]]; then
+        . $d/z0librc
+        Z0LIBDIR=$(readlink -e $d)
+        break
+      fi
+    done
     build_odoo_param "$@"
 fi
```

### Comparing `clodoo-2.0.5/setup.py` & `clodoo-2.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+# -*- coding: utf-8 -*-
 import sys
 
 from setuptools import find_packages, setup
 
 if sys.version_info >= (3, 0):
     install_requires = [
         "future",
         "jsonlib-python3",
         "openpyxl",
         "odoorpc",
-        "oerplib",
+        "oerplib3",
+        "odoo-client-lib",
         "os0",
         "psycopg2-binary",
         "python-plus",
         "unidecode",
         "z0lib",
     ]
 else:
@@ -27,15 +29,15 @@
         "python-plus",
         "unidecode==1.2.0",
         "z0lib",
     ]
 
 setup(
     name="clodoo",
-    version="2.0.5",
+    version="2.0.6",
     description="Do massive operations on Odoo Cloud",
     long_description="""
 Clodoo is a set of tools to manage to manage multiple Odoo installations with many DBs.
 
 With clodoo you can do massive operations on 1 or more Odoo databases based on
 different Odoo versions. Main operation are:
```

### Comparing `clodoo-2.0.5/PKG-INFO` & `clodoo-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: clodoo
-Version: 2.0.5
+Version: 2.0.6
 Summary: Do massive operations on Odoo Cloud
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `clodoo-2.0.5/clodoo.egg-info/SOURCES.txt` & `clodoo-2.0.6/clodoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clodoo-2.0.5/clodoo.egg-info/PKG-INFO` & `clodoo-2.0.6/clodoo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: clodoo
-Version: 2.0.5
+Version: 2.0.6
 Summary: Do massive operations on Odoo Cloud
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

