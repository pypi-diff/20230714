# Comparing `tmp/mycluster-2.0.4.tar.gz` & `tmp/mycluster-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mycluster-2.0.4.tar", last modified: Thu Mar 23 14:32:38 2023, max compression
+gzip compressed data, was "mycluster-2.0.5.tar", last modified: Fri Jul 14 11:37:06 2023, max compression
```

## Comparing `mycluster-2.0.4.tar` & `mycluster-2.0.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:32:38.869760 mycluster-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-23 14:32:26.000000 mycluster-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-23 14:32:26.000000 mycluster-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-03-23 14:32:38.869760 mycluster-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-23 14:32:26.000000 mycluster-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:32:38.869760 mycluster-2.0.4/mycluster/
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-03-23 14:32:26.000000 mycluster-2.0.4/mycluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-03-23 14:32:26.000000 mycluster-2.0.4/mycluster/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-23 14:32:26.000000 mycluster-2.0.4/mycluster/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:32:38.869760 mycluster-2.0.4/mycluster/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-23 14:32:26.000000 mycluster-2.0.4/mycluster/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-03-23 14:32:26.000000 mycluster-2.0.4/mycluster/schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-03-23 14:32:26.000000 mycluster-2.0.4/mycluster/schedulers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-03-23 14:32:26.000000 mycluster-2.0.4/mycluster/schedulers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15928 2023-03-23 14:32:26.000000 mycluster-2.0.4/mycluster/schedulers/sge.py
--rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-03-23 14:32:26.000000 mycluster-2.0.4/mycluster/schedulers/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:32:38.869760 mycluster-2.0.4/mycluster/schedulers/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-23 14:32:26.000000 mycluster-2.0.4/mycluster/schedulers/templates/lsf.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-23 14:32:26.000000 mycluster-2.0.4/mycluster/schedulers/templates/pbs.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-03-23 14:32:26.000000 mycluster-2.0.4/mycluster/schedulers/templates/sge.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-03-23 14:32:26.000000 mycluster-2.0.4/mycluster/schedulers/templates/slurm.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:32:38.869760 mycluster-2.0.4/mycluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-03-23 14:32:38.000000 mycluster-2.0.4/mycluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-23 14:32:38.000000 mycluster-2.0.4/mycluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:32:38.000000 mycluster-2.0.4/mycluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-23 14:32:38.000000 mycluster-2.0.4/mycluster.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-23 14:32:38.000000 mycluster-2.0.4/mycluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-23 14:32:38.000000 mycluster-2.0.4/mycluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-23 14:32:26.000000 mycluster-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-23 14:32:38.869760 mycluster-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-23 14:32:26.000000 mycluster-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:32:38.869760 mycluster-2.0.4/share/
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-03-23 14:32:26.000000 mycluster-2.0.4/share/mycluster-OF-simpleFoam.bsh
--rwxr-xr-x   0 runner    (1001) docker     (123)      112 2023-03-23 14:32:26.000000 mycluster-2.0.4/share/mycluster-fluent.bsh
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-03-23 14:32:26.000000 mycluster-2.0.4/share/mycluster-paraview.bsh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1435 2023-03-23 14:32:26.000000 mycluster-2.0.4/share/mycluster-zcfd.bsh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:06.745287 mycluster-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-14 11:36:57.000000 mycluster-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 11:36:57.000000 mycluster-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-14 11:37:06.745287 mycluster-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-14 11:36:57.000000 mycluster-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:06.741287 mycluster-2.0.5/mycluster/
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:06.745287 mycluster-2.0.5/mycluster/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11138 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:06.745287 mycluster-2.0.5/mycluster/schedulers/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/templates/lsf.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/templates/pbs.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/templates/sge.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-14 11:36:57.000000 mycluster-2.0.5/mycluster/schedulers/templates/slurm.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:06.741287 mycluster-2.0.5/mycluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-14 11:37:06.000000 mycluster-2.0.5/mycluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-14 11:37:06.000000 mycluster-2.0.5/mycluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:37:06.000000 mycluster-2.0.5/mycluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 11:37:06.000000 mycluster-2.0.5/mycluster.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 11:37:06.000000 mycluster-2.0.5/mycluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 11:37:06.000000 mycluster-2.0.5/mycluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-14 11:36:57.000000 mycluster-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-14 11:37:06.745287 mycluster-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-14 11:36:57.000000 mycluster-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:37:06.745287 mycluster-2.0.5/share/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-07-14 11:36:57.000000 mycluster-2.0.5/share/mycluster-OF-simpleFoam.bsh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      112 2023-07-14 11:36:57.000000 mycluster-2.0.5/share/mycluster-fluent.bsh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-07-14 11:36:57.000000 mycluster-2.0.5/share/mycluster-paraview.bsh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1435 2023-07-14 11:36:57.000000 mycluster-2.0.5/share/mycluster-zcfd.bsh
```

### Comparing `mycluster-2.0.4/LICENSE` & `mycluster-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.4/PKG-INFO` & `mycluster-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mycluster
-Version: 2.0.4
+Version: 2.0.5
 Summary: "Utilities to support interacting with multiple HPC clusters"
 Home-page: https://github.com/zenotech/MyCluster
 Author: "Zenotech Ltd"
 Author-email: "support@zenotech.com"
 License: BSD 3-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mycluster-2.0.4/README.md` & `mycluster-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.4/mycluster/__init__.py` & `mycluster-2.0.5/mycluster/__init__.py`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.4/mycluster/cli.py` & `mycluster-2.0.5/mycluster/cli.py`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.4/mycluster/exceptions.py` & `mycluster-2.0.5/mycluster/exceptions.py`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.4/mycluster/schedulers/__init__.py` & `mycluster-2.0.5/mycluster/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.4/mycluster/schedulers/base.py` & `mycluster-2.0.5/mycluster/schedulers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         project_name="default",
         tasks_per_node=None,
         threads_per_task=1,
         user_email=None,
         qos=None,
         exclusive=True,
         output_name=None,
+        gres=None,
     ):
         """
         Write a new job file
         """
         pass
 
     @abstractmethod
```

### Comparing `mycluster-2.0.4/mycluster/schedulers/lsf.py` & `mycluster-2.0.5/mycluster/schedulers/lsf.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,15 @@
         project_name="default",
         tasks_per_node=None,
         threads_per_task=1,
         user_email=None,
         qos=None,
         exclusive=True,
         output_name=None,
+        gres=None
     ):
         if tasks_per_node is None:
             tasks_per_node = self.tasks_per_node(queue_id)
         num_nodes = int(math.ceil(float(num_tasks) / float(tasks_per_node)))
 
         if threads_per_task is None:
             threads_per_task = 1
```

### Comparing `mycluster-2.0.4/mycluster/schedulers/pbs.py` & `mycluster-2.0.5/mycluster/schedulers/pbs.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,14 +150,15 @@
         project_name="default",
         tasks_per_node=None,
         threads_per_task=1,
         user_email=None,
         qos=None,
         exclusive=True,
         output_name=None,
+        gres=None
     ):
         queue_name = queue_id
         if tasks_per_node is None:
             tasks_per_node = self.tasks_per_node(queue_id)
         num_nodes = int(math.ceil(float(num_tasks) / float(tasks_per_node)))
 
         if threads_per_task is None:
```

### Comparing `mycluster-2.0.4/mycluster/schedulers/sge.py` & `mycluster-2.0.5/mycluster/schedulers/sge.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,14 +251,15 @@
         project_name="default",
         tasks_per_node=None,
         threads_per_task=1,
         user_email=None,
         qos=None,
         exclusive=True,
         output_name=None,
+        gres=None
     ):
         parallel_env = queue_id.split(":")[0]
         queue_name = queue_id.split(":")[1]
 
         if tasks_per_node is None:
             tasks_per_node = self.tasks_per_node(queue_id)
```

### Comparing `mycluster-2.0.4/mycluster/schedulers/slurm.py` & `mycluster-2.0.5/mycluster/schedulers/slurm.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
         project_name="default",
         tasks_per_node=None,
         threads_per_task=1,
         user_email=None,
         qos=None,
         exclusive=True,
         output_name=None,
+        gres=None
     ):
         queue_name = queue_id
         if tasks_per_node is None:
             tasks_per_node = self.tasks_per_node(queue_id)
         num_nodes = int(math.ceil(float(num_tasks) / float(tasks_per_node)))
         if threads_per_task is None:
             threads_per_task = -1
@@ -154,14 +155,15 @@
             num_threads_per_task=threads_per_task,
             num_nodes=num_nodes,
             project_name=project_name,
             wall_clock=wall_clock,
             openmpi_args=openmpi_args,
             qos=qos,
             exclusive=exclusive,
+            gres=gres
         )
         return script_str
 
     def submit(
         self, script_name, immediate=False, depends_on=None, depends_on_always_run=False
     ):
         additional_cmd = ""
```

### Comparing `mycluster-2.0.4/mycluster/schedulers/templates/lsf.jinja` & `mycluster-2.0.5/mycluster/schedulers/templates/lsf.jinja`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.4/mycluster/schedulers/templates/pbs.jinja` & `mycluster-2.0.5/mycluster/schedulers/templates/pbs.jinja`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.4/mycluster/schedulers/templates/sge.jinja` & `mycluster-2.0.5/mycluster/schedulers/templates/sge.jinja`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.4/mycluster/schedulers/templates/slurm.jinja` & `mycluster-2.0.5/mycluster/schedulers/templates/slurm.jinja`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 # High performance cpu governor
 #SBATCH --cpu-freq=Performance
 # How much wallclock time will be required?
 #SBATCH --time={{wall_clock}}
 {% if qos %}
 #SBATCH --qos {{qos}}
 {% endif %}
+{% if gres %}
+#SBATCH --gres={{gres}}
+{% endif %}
+
 
 export MYCLUSTER_QUEUE={{queue_name}}
 export MYCLUSTER_JOB_NAME={{my_name}}
 export NUM_TASKS={{num_tasks}}
 export TASKS_PER_NODE={{tpn}}
 export THREADS_PER_TASK={{num_threads_per_task}}
```

### Comparing `mycluster-2.0.4/mycluster.egg-info/PKG-INFO` & `mycluster-2.0.5/mycluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mycluster
-Version: 2.0.4
+Version: 2.0.5
 Summary: "Utilities to support interacting with multiple HPC clusters"
 Home-page: https://github.com/zenotech/MyCluster
 Author: "Zenotech Ltd"
 Author-email: "support@zenotech.com"
 License: BSD 3-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mycluster-2.0.4/mycluster.egg-info/SOURCES.txt` & `mycluster-2.0.5/mycluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.4/setup.cfg` & `mycluster-2.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `mycluster-2.0.4/share/mycluster-zcfd.bsh` & `mycluster-2.0.5/share/mycluster-zcfd.bsh`

 * *Files identical despite different names*

