# Comparing `tmp/checkvsphere-0.2.3.tar.gz` & `tmp/checkvsphere-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkvsphere-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "checkvsphere-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `checkvsphere-0.2.3.tar` & `checkvsphere-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      275 2023-05-03 13:33:32.671674 checkvsphere-0.2.3/README.md
--rw-r--r--   0        0        0      174 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/__init__.py
--rw-r--r--   0        0        0     3882 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/cli.py
--rw-r--r--   0        0        0      760 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/tools/__init__.py
--rw-r--r--   0        0        0    16614 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/tools/cli.py
--rw-r--r--   0        0        0     6363 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/tools/helper.py
--rw-r--r--   0        0        0     5200 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/tools/pchelper.py
--rw-r--r--   0        0        0     2183 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/tools/service_instance.py
--rw-r--r--   0        0        0     4153 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/tools/serviceutil.py
--rw-r--r--   0        0        0      760 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/vcmd/__init__.py
--rw-r--r--   0        0        0     1819 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/vcmd/about.py
--rw-r--r--   0        0        0     6692 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/vcmd/datastores.py
--rw-r--r--   0        0        0     4497 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/vcmd/hostnic.py
--rw-r--r--   0        0        0    11076 2023-05-24 13:31:30.446500 checkvsphere-0.2.3/checkvsphere/vcmd/hostruntime.py
--rw-r--r--   0        0        0     4038 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/vcmd/hostservice.py
--rw-r--r--   0        0        0     7633 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/vcmd/hoststorage.py
--rw-r--r--   0        0        0     2039 2023-05-03 13:33:32.679674 checkvsphere-0.2.3/checkvsphere/vcmd/listmetrics.py
--rw-r--r--   0        0        0     3341 2023-05-03 13:33:32.679674 checkvsphere-0.2.3/checkvsphere/vcmd/media.py
--rw-r--r--   0        0        0     8301 2023-05-03 13:33:32.679674 checkvsphere-0.2.3/checkvsphere/vcmd/perf.py
--rw-r--r--   0        0        0     4929 2023-05-03 13:33:32.679674 checkvsphere-0.2.3/checkvsphere/vcmd/snapshots.py
--rw-r--r--   0        0        0     8945 2023-05-03 13:33:32.679674 checkvsphere-0.2.3/checkvsphere/vcmd/vsan.py
--rw-r--r--   0        0        0      941 2023-05-25 08:27:33.439404 checkvsphere-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 checkvsphere-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      275 2023-05-03 13:33:32.671674 checkvsphere-0.3.0/README.md
+-rw-r--r--   0        0        0      174 2023-05-03 13:33:32.675674 checkvsphere-0.3.0/checkvsphere/__init__.py
+-rw-r--r--   0        0        0     4118 2023-06-28 08:05:59.203872 checkvsphere-0.3.0/checkvsphere/cli.py
+-rw-r--r--   0        0        0      760 2023-05-03 13:33:32.675674 checkvsphere-0.3.0/checkvsphere/tools/__init__.py
+-rw-r--r--   0        0        0    16614 2023-05-03 13:33:32.675674 checkvsphere-0.3.0/checkvsphere/tools/cli.py
+-rw-r--r--   0        0        0     6363 2023-05-03 13:33:32.675674 checkvsphere-0.3.0/checkvsphere/tools/helper.py
+-rw-r--r--   0        0        0     5200 2023-05-03 13:33:32.675674 checkvsphere-0.3.0/checkvsphere/tools/pchelper.py
+-rw-r--r--   0        0        0     2183 2023-05-03 13:33:32.675674 checkvsphere-0.3.0/checkvsphere/tools/service_instance.py
+-rw-r--r--   0        0        0     4153 2023-05-03 13:33:32.675674 checkvsphere-0.3.0/checkvsphere/tools/serviceutil.py
+-rw-r--r--   0        0        0      760 2023-05-03 13:33:32.675674 checkvsphere-0.3.0/checkvsphere/vcmd/__init__.py
+-rw-r--r--   0        0        0     1819 2023-05-03 13:33:32.675674 checkvsphere-0.3.0/checkvsphere/vcmd/about.py
+-rw-r--r--   0        0        0     6678 2023-06-28 07:44:46.526312 checkvsphere-0.3.0/checkvsphere/vcmd/datastores.py
+-rw-r--r--   0        0        0     4497 2023-05-03 13:33:32.675674 checkvsphere-0.3.0/checkvsphere/vcmd/hostnic.py
+-rw-r--r--   0        0        0    11076 2023-05-24 13:31:30.446500 checkvsphere-0.3.0/checkvsphere/vcmd/hostruntime.py
+-rw-r--r--   0        0        0     4038 2023-05-03 13:33:32.675674 checkvsphere-0.3.0/checkvsphere/vcmd/hostservice.py
+-rw-r--r--   0        0        0     7633 2023-05-03 13:33:32.675674 checkvsphere-0.3.0/checkvsphere/vcmd/hoststorage.py
+-rw-r--r--   0        0        0     2039 2023-05-03 13:33:32.679674 checkvsphere-0.3.0/checkvsphere/vcmd/listmetrics.py
+-rw-r--r--   0        0        0     3341 2023-05-03 13:33:32.679674 checkvsphere-0.3.0/checkvsphere/vcmd/media.py
+-rw-r--r--   0        0        0     8129 2023-06-28 08:00:15.469817 checkvsphere-0.3.0/checkvsphere/vcmd/perf.py
+-rw-r--r--   0        0        0     4624 2023-06-29 13:48:44.462164 checkvsphere-0.3.0/checkvsphere/vcmd/powerstate.py
+-rw-r--r--   0        0        0     5238 2023-06-29 13:49:25.229440 checkvsphere-0.3.0/checkvsphere/vcmd/snapshots.py
+-rw-r--r--   0        0        0     9053 2023-06-28 07:52:30.478067 checkvsphere-0.3.0/checkvsphere/vcmd/vsan.py
+-rw-r--r--   0        0        0      941 2023-06-28 15:35:05.070510 checkvsphere-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 checkvsphere-0.3.0/PKG-INFO
```

### Comparing `checkvsphere-0.2.3/checkvsphere/cli.py` & `checkvsphere-0.3.0/checkvsphere/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,14 +69,22 @@
         for cmd in sorted(cmds):
             print(f"  {cmd}")
         print()
 
 
 def main():
     import traceback
+    import logging
+
+    if int(os.environ.get("VSPHERE_DEBUG", "0")) > 0:
+        logging.basicConfig(
+            level=logging.DEBUG,
+            format='%(asctime)s %(levelname)s %(message)s',
+            stream=sys.stderr
+        )
 
     try:
         run()
     except VsphereConnectException as e:
         print("Cannot connect")
         sys.exit(0)
     except SystemExit as e:
```

### Comparing `checkvsphere-0.2.3/checkvsphere/tools/__init__.py` & `checkvsphere-0.3.0/checkvsphere/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/tools/cli.py` & `checkvsphere-0.3.0/checkvsphere/tools/cli.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/tools/helper.py` & `checkvsphere-0.3.0/checkvsphere/tools/helper.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/tools/pchelper.py` & `checkvsphere-0.3.0/checkvsphere/tools/pchelper.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/tools/service_instance.py` & `checkvsphere-0.3.0/checkvsphere/tools/service_instance.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/tools/serviceutil.py` & `checkvsphere-0.3.0/checkvsphere/tools/serviceutil.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/vcmd/__init__.py` & `checkvsphere-0.3.0/checkvsphere/vcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/vcmd/about.py` & `checkvsphere-0.3.0/checkvsphere/vcmd/about.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/vcmd/datastores.py` & `checkvsphere-0.3.0/checkvsphere/vcmd/datastores.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,15 @@
                     threshold['critical'] = range_in_bytes(Range(args.critical), uom)
                 opts['threshold'] = Threshold(**threshold)
 
                 if s != Status.OK:
                     check.add_message(s, f"{args.metric} on {name} is in state {s.name}: {value :.2f}{uom}")
 
             puom = '%' if metric == 'usage' else 'B'
-            check.add_perfmultidata(name, 'datastores',  label=metric, value=space[metric], uom=puom, **opts)
+            check.add_perfdata(label=f"{name} {metric}", value=space[metric], uom=puom, **opts)
 
     (code, message) = check.check_messages(separator="\n")#, allok=okmessage)
     check.exit(
         code=code,
         message=( message or "everything ok" )
     )
```

### Comparing `checkvsphere-0.2.3/checkvsphere/vcmd/hostnic.py` & `checkvsphere-0.3.0/checkvsphere/vcmd/hostnic.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/vcmd/hostruntime.py` & `checkvsphere-0.3.0/checkvsphere/vcmd/hostruntime.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/vcmd/hostservice.py` & `checkvsphere-0.3.0/checkvsphere/vcmd/hostservice.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/vcmd/hoststorage.py` & `checkvsphere-0.3.0/checkvsphere/vcmd/hoststorage.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/vcmd/listmetrics.py` & `checkvsphere-0.3.0/checkvsphere/vcmd/listmetrics.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/vcmd/media.py` & `checkvsphere-0.3.0/checkvsphere/vcmd/media.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.3/checkvsphere/vcmd/perf.py` & `checkvsphere-0.3.0/checkvsphere/vcmd/perf.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,17 +136,15 @@
     if not values.value:
         check.exit(code=Status.UNKNOWN, message="No data returned")
 
     if args.perfinstance == '':
         for instance in values.value:
             val = instance.value[0] * counterInfo['factor']
             if instance.id.instance == args.perfinstance:
-                check.add_perfmultidata(
-                    args.perfcounter if instance.id.instance == '' else instance.id.instance,
-                    'perf',
+                check.add_perfdata(
                     label=args.perfcounter,
                     value=val,
                     threshold=check.threshold,
                     uom=counterInfo['perfUnit'],
                 )
                 check.exit(
                     code=check.check_threshold(val),
@@ -155,25 +153,23 @@
     else:
         for instance in values.value:
             if instance.id.instance == '':
                 # ignore the aggregate if we query a specific or all instances
                 continue
             if args.perfinstance == '*' or args.perfinstance == instance.id.instance:
                 val = instance.value[0] * counterInfo['factor']
-                check.add_perfmultidata(
-                    instance.id.instance,
-                    'perf',
-                    label=args.perfcounter,
+                check.add_perfdata(
+                    label=f'{instance.id.instance} {args.perfcounter}',
                     value=val,
                     threshold=check.threshold,
                     uom=counterInfo['perfUnit'],
                 )
                 check.add_message(
                     check.threshold.get_status(val),
-                    f"{args.perfcounter}_{instance.id.instance} has value {val} {counterInfo['unit']}",
+                    f"'{instance.id.instance} {args.perfcounter}' has value {val} {counterInfo['unit']}",
                 )
 
         (code, message) = check.check_messages(separator='\n  ')
         check.exit(code=code, message=message)
 
 
 def get_perf_values(args, obj, metricId):
```

### Comparing `checkvsphere-0.2.3/checkvsphere/vcmd/snapshots.py` & `checkvsphere-0.3.0/checkvsphere/vcmd/snapshots.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
 import logging
 from pyVmomi import vim
 from monplugin import Check, Status, Threshold
 from ..tools import cli, service_instance
 from datetime import datetime, timedelta, timezone
 from ..tools.helper import (
-	CheckArgument,
-	find_entity_views,
-	get_metric,
+    CheckArgument,
+    find_entity_views,
+    get_metric,
     isbanned,
     isallowed
 )
 
 check = None
 args = None
 
@@ -118,40 +118,47 @@
 
     args._si = service_instance.connect(args)
 
     vms = find_entity_views(
         args._si,
         vim.VirtualMachine,
         begin_entity=args._si.content.rootFolder,
-        properties=['name', 'snapshot']
+        properties=['name', 'snapshot', 'resourcePool', 'config.template']
     )
 
     for vm in vms:
         name = vm['props']['name']
+        isTemplate = vm['props'].get('config.template', None)
+
         if 'snapshot' not in vm['props']:
+            logging.debug(f"vm {name} has no snapshots")
+            continue
+
+        if isTemplate:
+            logging.debug(f"{name} is a template vm, ignoring ...")
             continue
 
+        adj = None
         if args.mode == 'age':
+            adj = 'old'
             check_by_age(vm, vm['props']['snapshot'].rootSnapshotList)
         elif args.mode == 'count':
+            adj = 'many'
             count = count_snapshots(vm, vm['props']['snapshot'].rootSnapshotList)
             code = check.check_threshold(count)
             if code != Status.OK:
                 check.add_message(code, f"«{name}» has {count} snapshots")
         else:
             raise RuntimeError("Unknown mode {args.mode}")
 
-    (code, message) = check.check_messages(separator=', ', separator_all='; ')
-    if code != Status.OK:
-        check.exit(
-            code=code,
-            message=message,
-        )
-    else:
-        check.exit(code=Status.OK, message='snapshots ok')
+    (code, message) = check.check_messages(separator='\n', separator_all='\n')
+    check.exit(
+        code=code,
+        message=f"snapshots ok" if code == Status.OK else f"too {adj} snapshots found\n" + message,
+    )
 
 if __name__ == "__main__":
     try:
         run()
     except SystemExit as e:
         if e.code > 3 or e.code < 0:
             print("UNKNOWN EXIT CODE")
```

### Comparing `checkvsphere-0.2.3/checkvsphere/vcmd/vsan.py` & `checkvsphere-0.3.0/checkvsphere/vcmd/vsan.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,27 +68,29 @@
 
     args._si = service_instance.connect(args)
 
     clusters = find_entity_views(
         args._si,
         vim.ClusterComputeResource,
         begin_entity=args._si.content.rootFolder,
-        properties=['name']
+        properties=['name', 'configurationEx']
     )
 
     clusters = process_retrieve_content(list(map(lambda x: x['obj'], clusters)))
 
     apiVersion = vsu.GetLatestVmodlVersion(args.host, int(args.port))
     vcMos =  vsu.GetVsanVcMos( #vsu.GetVsanVcMos(
         args._si._stub,
         context=sslContext(args),
         version=apiVersion
     )
     vhs = vcMos['vsan-cluster-health-system']
 
+    clusters = list(filter(lambda x: x['configurationEx'].vsanConfigInfo.enabled, clusters))
+
     for cluster in clusters:
         if isbanned(args, cluster['name'], 'exclude'):
             continue
         if not isallowed(args, cluster['name'], 'include'):
             continue
 
         fields = ['vsanConfig']
@@ -154,15 +156,15 @@
 
         if oh is None:
             # cluster doesn't have objectHealth
             check.add_message(OK, f"cluster {cluster['name']} doesn't have objectHealth")
             continue
 
         for detail in oh.objectHealthDetail:
-            check.add_perfmultidata(cluster['name'], None, label=detail.health, value=detail.numObjects)
+            check.add_perfdata(label=f"{cluster['name']} {detail.health}", value=detail.numObjects)
 
             if detail.health == 'remoteAccessible':
                 # ignore them, should be checked on the remote side
                 continue
 
             if detail.numObjects == 0:
                 continue
```

### Comparing `checkvsphere-0.2.3/pyproject.toml` & `checkvsphere-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "checkvsphere"
 readme = "README.md"
 description = "check_vsphere monitoring plugin"
-version = "0.2.3"
+version = "0.3.0"
 requires-python = ">= 3.6"
 authors = [
     { name = "Danijel Tasov", email = "danijel.tasov@consol.de" }
 ]
 dependencies = [
     "pyvmomi >= 8.0.0.1, < 9",
     "monplugin >= 0.6.1",
```

### Comparing `checkvsphere-0.2.3/PKG-INFO` & `checkvsphere-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkvsphere
-Version: 0.2.3
+Version: 0.3.0
 Summary: check_vsphere monitoring plugin
 Author-email: Danijel Tasov <danijel.tasov@consol.de>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

