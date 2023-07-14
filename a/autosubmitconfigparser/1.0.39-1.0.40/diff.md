# Comparing `tmp/autosubmitconfigparser-1.0.39.tar.gz` & `tmp/autosubmitconfigparser-1.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmitconfigparser-1.0.39.tar", last modified: Wed Jun 28 15:27:04 2023, max compression
+gzip compressed data, was "autosubmitconfigparser-1.0.40.tar", last modified: Fri Jul 14 13:52:50 2023, max compression
```

## Comparing `autosubmitconfigparser-1.0.39.tar` & `autosubmitconfigparser-1.0.40.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-28 15:27:04.458413 autosubmitconfigparser-1.0.39/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.39/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-06-28 15:27:04.458413 autosubmitconfigparser-1.0.39/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.39/README.md
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-28 15:27:04.454413 autosubmitconfigparser-1.0.39/autosubmitconfigparser/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:48:23.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-28 15:27:04.454413 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:49:24.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/__init__.py
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/basicconfig.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   104598 2023-06-28 13:30:13.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/configcommon.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-28 15:27:04.458413 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/autosubmit-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/autosubmit.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/expdef-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/expdef.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/git-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/jobs-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/jobs.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/local-minimal.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/platforms-dummy.yml
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/platforms.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      275 2023-06-07 12:06:41.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/yamlparser.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-28 15:27:04.454413 autosubmitconfigparser-1.0.39/autosubmitconfigparser.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2086 2023-06-28 15:27:04.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1029 2023-06-28 15:27:04.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-06-28 15:27:04.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      321 2023-06-28 15:27:04.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-06-28 15:27:04.000000 autosubmitconfigparser-1.0.39/autosubmitconfigparser.egg-info/top_level.txt
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-28 15:27:04.458413 autosubmitconfigparser-1.0.39/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.39/log/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.39/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.39/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-06-28 15:27:04.458413 autosubmitconfigparser-1.0.39/setup.cfg
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1461 2023-06-28 13:40:33.000000 autosubmitconfigparser-1.0.39/setup.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       41 2023-03-03 13:49:23.000000 autosubmitconfigparser-1.0.40/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2123 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1493 2022-12-05 09:31:33.000000 autosubmitconfigparser-1.0.40/README.md
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/autosubmitconfigparser/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:48:23.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-06-07 13:49:24.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/__init__.py
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     7990 2023-04-25 12:49:03.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/basicconfig.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   107450 2023-07-14 13:47:59.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/configcommon.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/autosubmit-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      269 2023-02-14 09:38:41.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/autosubmit.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      562 2023-02-14 09:24:09.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/expdef-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      557 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/expdef.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      401 2023-03-03 11:06:17.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/git-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/jobs-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      669 2022-10-26 08:50:59.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/jobs.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)      321 2023-03-03 12:26:14.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/local-minimal.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/platforms-dummy.yml
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1247 2023-02-14 10:53:51.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/platforms.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      275 2023-06-07 12:06:41.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/yamlparser.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2123 2023-07-14 13:52:50.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1029 2023-07-14 13:52:50.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-07-14 13:52:50.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      321 2023-07-14 13:52:50.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2023-07-14 13:52:50.000000 autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/top_level.txt
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.40/log/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.40/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13106 2022-10-26 08:51:23.000000 autosubmitconfigparser-1.0.40/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-07-14 13:52:50.922066 autosubmitconfigparser-1.0.40/setup.cfg
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     1461 2023-07-14 13:50:19.000000 autosubmitconfigparser-1.0.40/setup.py
```

### Comparing `autosubmitconfigparser-1.0.39/PKG-INFO` & `autosubmitconfigparser-1.0.40/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.39
+Version: 1.0.40
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
+License: UNKNOWN
 Keywords: climate,weather,workflow,HPC
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 
 Simple library that allows to read the data of an Autosubmit experiment.
@@ -56,7 +58,9 @@
 # This is a sample text with a placeholder expid
 
 # delete samples
 os.remove("as_sample.txt")
 os.remove("as_sample_parsed.txt")
 ```
 
+
+
```

### Comparing `autosubmitconfigparser-1.0.39/README.md` & `autosubmitconfigparser-1.0.40/README.md`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/basicconfig.py` & `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/basicconfig.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/configcommon.py` & `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/configcommon.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,41 +10,40 @@
 # (at your option) any later version.
 
 # Autosubmit is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
-# You should have received a copy of the GNU General Public License
-# along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
-import shutil
+import collections
+import copy
+import datetime
+import json
+import locale
 import numbers
-
 import os
 import re
+# You should have received a copy of the GNU General Public License
+# along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
+import shutil
 import subprocess
 import traceback
-import json
+from collections import defaultdict
+from datetime import datetime, timedelta
+from pathlib import Path
+
 import ruamel.yaml as yaml
-from .basicconfig import BasicConfig
-from .yamlparser import YAMLParserFactory
+from bscearth.utils.date import parse_date
 from configobj import ConfigObj
-from log.log import Log,AutosubmitCritical,AutosubmitError
-
 from pyparsing import nestedExpr
 
-from bscearth.utils.date import parse_date
+from log.log import Log, AutosubmitCritical, AutosubmitError
+from .basicconfig import BasicConfig
+from .yamlparser import YAMLParserFactory
 
-from collections import defaultdict
-import collections
-import datetime
-import copy
-from datetime import datetime, timedelta
-from pathlib import Path
-import locale
 
 class AutosubmitConfig(object):
     """
     Class to handle experiment configuration coming from file or database
 
     :param expid: experiment identifier
     :type expid: str
@@ -65,14 +64,15 @@
 
         self.current_loaded_files = dict()
         self.conf_folder_yaml = Path(BasicConfig.LOCAL_ROOT_DIR, expid, "conf")
 
         self.wrong_config = defaultdict(list)
         self.warn_config = defaultdict(list)
         self.dynamic_variables = list()
+        self.special_dynamic_variables = list() # variables that will be sustituted after all files is loaded
         self.starter_conf = dict()
 
     @property
     def jobs_data(self):
         return self.experiment_data["JOBS"]
 
     @property
@@ -655,74 +655,57 @@
         :param new_data: dict with new configuration
         :return: dict with new configuration taking priority over current configuration
         '''
         # Basic data
         current_data = self.deep_update(current_data, new_data)
         # Parser loops in custom config
         current_data = self.deep_read_loops(current_data)
-        current_data = self.parse_data_loops(current_data, self.data_loops)
         self.dynamic_variables = list(set(self.dynamic_variables))
+        self.special_dynamic_variables = list(set(self.special_dynamic_variables))
+        current_data = self.deep_normalize(current_data)
+        current_data = self.substitute_dynamic_variables(current_data) # before read the for loops
+        current_data = self.parse_data_loops(current_data, self.data_loops)
         return current_data
 
-    def parse_data_loops(self,exp_data,data_loops):
-        section_data = list()
+    def parse_data_loops(self,experiment_data,data_loops):
+        """
+        This function, looks for the FOR keyword, to generates N amount of subsections of the same section.
+        Looks for the "NAME" keyword, inside this FOR keyword to determine the name of the new sections
+        Experiment_data is the dictionary that contains all the sections, a subsection could be located at the root but also in a nested section
+        :param experiment_data: dictionary with all the sections
+        :param data_loops: list of lists with the path to the section that contains the FOR keyword
+        :return: Original experiment_data with the sections in the data_loops updated changing the FOR by multiple new sections
+        """
         for loops in data_loops:
-            #Extract section affected
-            current_data = exp_data.pop(loops[0])
-            section_data.append(current_data)
-            #Extract nested-section if any
-            for section in loops[1:]:
-                current_data = current_data.pop(section)
-                section_data.append(current_data)
-
+            pointer_to_last_data = experiment_data
+            for section in loops[:-1]:
+                pointer_to_last_data = pointer_to_last_data[section]
             section_basename = loops[-1]
-            for_sections = section_data[-1].pop("FOR")
-            #Delete old key
-            loops.pop()
-            # Delete old data
-            section_data.pop()
-            new_sections = dict()
-            section_ending_name = for_sections.get("NAME",[])
-            for_sections.pop("NAME")
-            n_sections_to_create = len(for_sections[list(for_sections)[0]])
-            if len(section_ending_name) == 0:
-                for i in range(0,n_sections_to_create):
-                    section_ending_name.append(str(i))
-            full_name = []
-            new_data = dict()
-
-            for i in range(0,n_sections_to_create):
-                full_name.append(section_basename + "_" + str(section_ending_name[i]))
-                new_data[full_name[i]] = copy.deepcopy(current_data)
-
-            # Last level must contain the new info
-            last_data = section_data.pop(-1)
-            last_level = loops.pop(-1)
-            #Fill new camps
-
-            for i in range(0, n_sections_to_create):
-                for key,val_list in for_sections.items():
-                    new_data[full_name[i]][key] = val_list[i]
-            #update last dict level
-            last_data.update(new_data)
-            # backtracking
-            next_section = dict()
-            next_section[last_level] = last_data
-            new_exp_data = next_section
-            while len(loops) > 0:
-                level_name = loops.pop(-1)
-                level_data = section_data.pop(-1)
-                level_data.update(new_exp_data)
-                new_exp_data[level_name] = level_data
-            else:
-                new_exp_data = next_section
-            exp_data.update(new_exp_data)
-            pass
+            current_data = copy.deepcopy(pointer_to_last_data[loops[-1]])
+            # Remove the original section  keyword from original data
+            pointer_to_last_data.pop(loops[-1])
+            for_sections = current_data.pop("FOR")
+            # Calculates new name
+            # And adds the dynamic values if any
+            for key, value in for_sections.items():
+                if type(value) == str:
+                    value_ = value.strip("[]")
+                    value_ = [ v.strip(" ") for v in value_.split(",") ]
+                    for_sections[key] = value_
+            for name_index in range(len(for_sections["NAME"])):
+                section_ending_name = section_basename + "_" + str(for_sections["NAME"][name_index])
+                pointer_to_last_data[section_ending_name] = copy.deepcopy(current_data)
+                for key,value in for_sections.items():
+                    if key != "NAME":
+                        pointer_to_last_data[section_ending_name][key] = value[name_index]
+            # Delete pointer, because we are going to use it in the next loop for a different section so we need to delete the pointer to avoid overwriting
+            del pointer_to_last_data
         self.data_loops = []
-        return exp_data
+        return experiment_data
+
     def get_placeholders(self,val,key):
 
         aux_name = val.split("/")
         full_name = []
         for aux in aux_name:
             full_name.extend(aux.split(" "))
         placeholders = []
@@ -747,68 +730,88 @@
             if count >= amount_of_keys_to_check:
                 break
         if count_dot >= int(count/2)+1:
             dict_keys_type = "long"
         else:
             dict_keys_type = "short"
         return dict_keys_type
-    def clean_dynamic_variables(self,pattern):
-        '''
-        Cleans dynamic variables
+    def clean_dynamic_variables(self,pattern,in_the_end = False):
+        """
+        Clean dynamic variables
+        :param pattern:
+        :param in_the_end:
         :return:
-        '''
+        """
         dynamic_variables = []
-        for dynamic_var in self.dynamic_variables:
+        if in_the_end:
+            dynamic_variables_ = self.special_dynamic_variables
+        else:
+            dynamic_variables_ = self.dynamic_variables
+
+        for dynamic_var in dynamic_variables_:
             # if not placeholder in dynamic_var[1], then it is not a dynamic variable
             match = (re.search(pattern, dynamic_var[1],flags=re.IGNORECASE))
             if match is not None:
                 dynamic_variables.append(dynamic_var)
-        self.dynamic_variables = dynamic_variables
-    def substitute_dynamic_variables(self,parameters=None,max_deep=25,dict_keys_type=None,not_in_data=""):
+        if in_the_end:
+            self.special_dynamic_variables = dynamic_variables
+        else:
+            self.dynamic_variables = dynamic_variables
+    def substitute_dynamic_variables(self,parameters=None,max_deep=25,dict_keys_type=None,not_in_data="",in_the_end = False):
         """
         Substitute dynamic variables in the experiment data
         :parameter
         :return:
         """
 
+        if not in_the_end:
+            dynamic_variables_ = self.dynamic_variables
+            pattern = '%[a-zA-Z0-9_.]*%'
+            start_long = 1
+        else:
+            dynamic_variables_ = self.special_dynamic_variables
+            pattern = '%\^[a-zA-Z0-9_.]*%'
+            start_long = 2
         if parameters is None:
             parameters = self.deep_parameters_export(self.experiment_data)
         # Check if the parameters key provided are long(%DEFAULT.EXPID%) or short(DEFAULT[EXPID]) if it is not specified.
         if dict_keys_type is None:
             dict_keys_type = self.check_dict_keys_type(parameters)
-        pattern = '%[a-zA-Z0-9_.]*%'
-        backup_variables = self.dynamic_variables
-        max_deep = max_deep + len(self.dynamic_variables)
 
-        while len(self.dynamic_variables) > 0 and max_deep > 0:
+        backup_variables = dynamic_variables_
+        max_deep = max_deep + len(dynamic_variables_)
+
+        while len(dynamic_variables_) > 0 and max_deep > 0:
             dynamic_variables = []
-            for dynamic_var in self.dynamic_variables:
+            for dynamic_var in dynamic_variables_:
                 #get value of placeholder with  name without %%
                 if dict_keys_type == "long":
-                    keys = parameters.get(str(dynamic_var[0][1:-1]),None)
+                    keys = parameters.get(str(dynamic_var[0][start_long:-1]),None)
                     if keys is None:
                         keys = parameters.get(str(dynamic_var[0]), None)
                 else:
                     keys = dynamic_var[1]
                     # get substring of key between %%
                 if keys is not None:
                     match = (re.search(pattern, keys,flags=re.IGNORECASE))
                 else:
                     match = None
                 if match is not None:
                     rest_of_keys_start = keys[:match.start()]
                     rest_of_keys_end = keys[match.end():]
                     keys = keys[match.start():match.end()]
                     if "." in keys and dict_keys_type != "long":
-                        keys = keys[1:-1].split(".")
+                        keys = keys[start_long:-1].split(".")
                     else:
-                        keys = [keys[1:-1]]
+                        keys = [keys[start_long:-1]]
                     aux_dict = parameters
                     for k in keys:
                         aux_dict = aux_dict.get(k.upper(),{})
+                        if type(aux_dict) == int:
+                            aux_dict = str(aux_dict)
                     if len(aux_dict) > 0:
                         full_value = str(rest_of_keys_start)+str(aux_dict)+str(rest_of_keys_end)
                         value = full_value
                     else:
                         value = None
                 else:
                     value = None
@@ -829,18 +832,25 @@
                     # This may be True instead of False
                     substituted = False
                 if not substituted:
                     if value is not None:
                         dynamic_variables.append((dynamic_var[0],value))
                     else:
                         dynamic_variables.append(dynamic_var)
-            self.dynamic_variables = dynamic_variables
+            if in_the_end:
+                self.special_dynamic_variables = dynamic_variables
+            else:
+                self.dynamic_variables = dynamic_variables
             max_deep = max_deep - 1
-        self.dynamic_variables = backup_variables
-        self.clean_dynamic_variables(pattern)
+        if in_the_end:
+            self.special_dynamic_variables = backup_variables
+            self.clean_dynamic_variables(pattern,in_the_end)
+        else:
+            self.dynamic_variables = backup_variables
+            self.clean_dynamic_variables(pattern)
         return parameters
     def substitute_placeholder_variables(self,key,val,parameters):
         substituted = False
         data = parameters
         placeholders=self.get_placeholders(val, False)
         new_placeholders = False
         for section in placeholders:
@@ -862,19 +872,30 @@
     def deep_read_loops(self,data,for_keys=[],long_key=""):
         """
         Update a nested dictionary or similar mapping.
         Modify ``source`` in place.
         """
         for key, val in data.items():
             # Placeholders variables
-            if not isinstance(val, collections.abc.Mapping) and "%" in str(val):
+            # Pattern to search a string starting with % and ending with % allowing the chars [],._ to exist in the middle
+            dynamic_var_pattern = '%[a-zA-Z0-9_.]*%'
+            # Pattern to search a string starting with %^ and ending with %
+            special_dynamic_var_pattern = '%\^[a-zA-Z0-9_.]*%'
+
+            if not isinstance(val, collections.abc.Mapping) and re.search(dynamic_var_pattern, str(val),flags=re.IGNORECASE) is not None:
                 self.dynamic_variables.append((long_key+key, val))
+            elif not isinstance(val, collections.abc.Mapping) and re.search(special_dynamic_var_pattern, str(val),flags=re.IGNORECASE) is not None:
+                self.special_dynamic_variables.append((long_key+key, val))
             if key == "FOR":
+                # special case: check dynamic variables in the for loop
+                for for_sections,for_values in data[key].items():
+                    if re.search(dynamic_var_pattern, str(for_values), flags=re.IGNORECASE) is not None:
+                        self.dynamic_variables.append((long_key+key, str(for_values)))
                 self.data_loops.append(for_keys)
-            elif isinstance(val, collections.abc.Mapping ):
+            if isinstance(val, collections.abc.Mapping ):
                 self.deep_read_loops(data.get(key, {}),for_keys+[key],long_key=long_key+key+".")
         return data
 
 
 
 
 
@@ -1310,14 +1331,18 @@
                     # Load a file and unify the current_data with the loaded data
                     current_data = self.substitute_dynamic_variables(self.unify_conf(self.substitute_dynamic_variables(current_data), self.load_config_file(current_data,filename)))
                     # Load next level if any
                     custom_conf_directive = current_data.get('DEFAULT', {}).get('CUSTOM_CONFIG', None)
                     filenames_to_load_level = self.parse_custom_conf_directive(custom_conf_directive)
                     if current_data.get('DEFAULT', {}).get('CUSTOM_CONFIG', None) is not None:
                         del current_data["DEFAULT"]["CUSTOM_CONFIG"]
+                    filenames_to_load_level["PRE"] = [to_load for to_load in filenames_to_load_level["PRE"] if
+                                                      to_load not in self.current_loaded_files]
+                    filenames_to_load_level["POST"] = [to_load for to_load in filenames_to_load_level["POST"] if
+                                                      to_load not in self.current_loaded_files]
                     if len(filenames_to_load_level["PRE"]) > 0:
                         current_data_pre = self.unify_conf(current_data_pre,self.load_custom_config_section(copy.deepcopy(current_data), filenames_to_load_level["PRE"]))
                     else:
                         current_data_pre = current_data
                     current_data = self.unify_conf(current_data_pre, current_data)
 
                     if len(filenames_to_load_level["POST"]) > 0:
@@ -1384,14 +1409,16 @@
             self.current_loaded_files.update(non_minimal_files)
             if "AS_TEMP" in self.experiment_data.keys():
                 del self.experiment_data["AS_TEMP"]
             # IF expid and hpcarch are not defined, use the ones from the minimal.yml file
             self.deep_add_missing_starter_conf(self.experiment_data,starter_conf)
             self.experiment_data = self.substitute_dynamic_variables(self.experiment_data)
             self.experiment_data = self.normalize_variables(self.experiment_data)
+            self.experiment_data = self.substitute_dynamic_variables(self.experiment_data,in_the_end=True)
+
     def load_last_run(self):
         self.metadata_folder = Path(self.conf_folder_yaml) / "metadata"
         if not self.metadata_folder.exists():
             os.makedirs(self.metadata_folder)
             os.chmod(self.metadata_folder, 0o775)
         if not os.access(self.metadata_folder, os.W_OK):
             print(f"WARNING: Can't save the experiment data into {self.metadata_folder}, no write permissions")
@@ -1409,15 +1436,15 @@
         Saves the experiment data into the experiment_folder/conf/metadata folder as a yaml file
         :return: True if the data has changed, False otherwise
         """
         changed = False
         # check if the folder exists and we have write permissions, if folder doesn't exist create it with rwx/rwx/r-x permissions
         # metadata folder is inside the experiment folder / conf folder / metadata folder
         # If this function is called before load_last_run, we need to load the last run
-        if len(self.last_experiment_data) == 0:
+        if self.last_experiment_data and len(self.last_experiment_data) == 0:
             self.load_last_run()
         if self.data_changed or not (Path(self.metadata_folder) / "experiment_data.yml").exists():
             # Backup the old file
             if (Path(self.metadata_folder) / "experiment_data.yml").exists():
                 shutil.copy(Path(self.metadata_folder) / "experiment_data.yml", Path(self.metadata_folder) / "experiment_data.yml.bak")
             with open(Path(self.metadata_folder) / "experiment_data.yml", 'w') as stream:
                 yaml.dump(self.experiment_data, stream, default_flow_style=False)
@@ -1450,15 +1477,15 @@
         :return: changed: boolean, True if the configuration has changed
         """
 
         if changed:
             return True
         for key, val in current_data.items():
             if isinstance(val, collections.abc.Mapping):
-                if key not in last_run_data.keys():
+                if not last_run_data or key not in last_run_data.keys():
                     changed = True
                     break
                 else:
                     changed = self.quick_deep_diff(last_run_data[key], val, changed)
             else:
                 if key not in last_run_data.keys() or last_run_data[key] != val:
                     changed = True
```

### Comparing `autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/expdef-dummy.yml` & `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/expdef-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/expdef.yml` & `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/expdef.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/jobs-dummy.yml` & `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/jobs-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/jobs.yml` & `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/jobs.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/platforms-dummy.yml` & `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/platforms-dummy.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.39/autosubmitconfigparser/config/files/platforms.yml` & `autosubmitconfigparser-1.0.40/autosubmitconfigparser/config/files/platforms.yml`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.39/autosubmitconfigparser.egg-info/PKG-INFO` & `autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: autosubmitconfigparser
-Version: 1.0.39
+Version: 1.0.40
 Summary: An utility library that allows to read an Autosubmit 4 experiment configuration.
 Home-page: https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
+License: UNKNOWN
 Keywords: climate,weather,workflow,HPC
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 
 Simple library that allows to read the data of an Autosubmit experiment.
@@ -56,7 +58,9 @@
 # This is a sample text with a placeholder expid
 
 # delete samples
 os.remove("as_sample.txt")
 os.remove("as_sample_parsed.txt")
 ```
 
+
+
```

### Comparing `autosubmitconfigparser-1.0.39/autosubmitconfigparser.egg-info/SOURCES.txt` & `autosubmitconfigparser-1.0.40/autosubmitconfigparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.39/log/fd_show.py` & `autosubmitconfigparser-1.0.40/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.39/log/log.py` & `autosubmitconfigparser-1.0.40/log/log.py`

 * *Files identical despite different names*

### Comparing `autosubmitconfigparser-1.0.39/setup.py` & `autosubmitconfigparser-1.0.40/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autosubmitconfigparser",
-    version="1.0.39",
+    version="1.0.40",
     author="Daniel Beltran Mora",
     author_email="daniel.beltran@bsc.es",
     description="An utility library that allows to read an Autosubmit 4 experiment configuration.",
     keywords=['climate', 'weather', 'workflow', 'HPC'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://earth.bsc.es/gitlab/ces/autosubmit4-config-parser.git",
```

