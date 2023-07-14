# Comparing `tmp/travis_emulator-2.0.5.tar.gz` & `tmp/travis_emulator-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/travis_emulator-2.0.5.tar", last modified: Sat Jun  3 06:22:52 2023, max compression
+gzip compressed data, was "dist/travis_emulator-2.0.6.tar", last modified: Fri Jul 14 15:49:40 2023, max compression
```

## Comparing `travis_emulator-2.0.5.tar` & `travis_emulator-2.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 travis_emulator-2.0.5/travis_emulator/__main__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5097 2023-04-14 13:30:50.000000 travis_emulator-2.0.5/travis_emulator/make_travis_conf.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3683 2023-05-20 06:25:25.000000 travis_emulator-2.0.5/travis_emulator/template_travis.yml
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3324 2023-06-02 13:07:37.000000 travis_emulator-2.0.5/travis_emulator/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7868 2023-05-20 06:25:25.000000 travis_emulator-2.0.5/travis_emulator/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 travis_emulator-2.0.5/travis_emulator/scripts/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     9772 2022-12-09 05:08:44.000000 travis_emulator-2.0.5/travis_emulator/travis.man
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    38654 2023-05-29 13:26:46.000000 travis_emulator-2.0.5/travis_emulator/travisrc
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    46782 2023-05-21 06:35:50.000000 travis_emulator-2.0.5/travis_emulator/travis
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       77 2022-12-09 05:08:44.000000 travis_emulator-2.0.5/travis_emulator/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/setup.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3324 2023-05-20 06:25:25.000000 travis_emulator-2.0.5/setup.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       16 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:51:08.000000 travis_emulator-2.0.5/travis_emulator.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      145 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      599 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       13 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2898 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/travis_emulator.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2898 2023-06-03 06:22:52.000000 travis_emulator-2.0.5/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    17054 2023-05-21 12:21:55.000000 travis_emulator-2.0.5/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 15:49:40.000000 travis_emulator-2.0.6/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 15:49:40.000000 travis_emulator-2.0.6/travis_emulator/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 travis_emulator-2.0.6/travis_emulator/__main__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5121 2023-06-24 06:17:11.000000 travis_emulator-2.0.6/travis_emulator/make_travis_conf.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3683 2023-07-14 05:51:06.000000 travis_emulator-2.0.6/travis_emulator/template_travis.yml
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 15:49:40.000000 travis_emulator-2.0.6/travis_emulator/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3348 2023-07-14 05:51:06.000000 travis_emulator-2.0.6/travis_emulator/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7868 2023-07-14 05:51:06.000000 travis_emulator-2.0.6/travis_emulator/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 travis_emulator-2.0.6/travis_emulator/scripts/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     9772 2022-12-09 05:08:44.000000 travis_emulator-2.0.6/travis_emulator/travis.man
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    38910 2023-07-14 05:51:06.000000 travis_emulator-2.0.6/travis_emulator/travisrc
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    47066 2023-07-14 05:51:06.000000 travis_emulator-2.0.6/travis_emulator/travis
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       77 2022-12-09 05:08:44.000000 travis_emulator-2.0.6/travis_emulator/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-07-14 15:49:40.000000 travis_emulator-2.0.6/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3348 2023-07-14 05:51:06.000000 travis_emulator-2.0.6/setup.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-07-14 15:49:40.000000 travis_emulator-2.0.6/travis_emulator.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       16 2023-07-14 15:49:40.000000 travis_emulator-2.0.6/travis_emulator.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-07-14 15:49:40.000000 travis_emulator-2.0.6/travis_emulator.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:51:08.000000 travis_emulator-2.0.6/travis_emulator.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      145 2023-07-14 15:49:40.000000 travis_emulator-2.0.6/travis_emulator.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      599 2023-07-14 15:49:40.000000 travis_emulator-2.0.6/travis_emulator.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       13 2023-07-14 15:49:40.000000 travis_emulator-2.0.6/travis_emulator.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2898 2023-07-14 15:49:40.000000 travis_emulator-2.0.6/travis_emulator.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2898 2023-07-14 15:49:40.000000 travis_emulator-2.0.6/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    20115 2023-07-14 05:51:06.000000 travis_emulator-2.0.6/README.rst
```

### Comparing `travis_emulator-2.0.5/travis_emulator/make_travis_conf.py` & `travis_emulator-2.0.6/travis_emulator/make_travis_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 import os
 import sys
 import re
 
 
 def os_env(item, default=None):
     default = default or item
```

### Comparing `travis_emulator-2.0.5/travis_emulator/template_travis.yml` & `travis_emulator-2.0.6/travis_emulator/template_travis.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Odoo yaml template for travis-ci
-# __version__=2.0.5
+# __version__=2.0.6
 # Can used both in local travis emulator both in travis environment
 # Notice: in local travis emulator macroes are substituted in 2 steps:
 # - format: ${macro} are replaced before execution (at travis.yml read)
 # - format: $macro are replace by shell during execution
 
 language: python
 sudo: false
```

### Comparing `travis_emulator-2.0.5/travis_emulator/scripts/setup.info` & `travis_emulator-2.0.6/travis_emulator/scripts/setup.info`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 setup(
     name='travis_emulator',
-    version='2.0.5',
+    version='2.0.6',
     description='Travis CI emulator for local develop environment',
     long_description="""
 Travis emulator can emulate TravisCi parsing the **.travis.yml** file in local Linux machine.
 You can test your application before pushing code to github.com web site.
 
 Travis emulator can creates all the build declared in **.travis.yml**;
 all the builds are executed in sequential way.
```

### Comparing `travis_emulator-2.0.5/travis_emulator/scripts/main.py` & `travis_emulator-2.0.6/travis_emulator/scripts/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
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

### Comparing `travis_emulator-2.0.5/travis_emulator/travis.man` & `travis_emulator-2.0.6/travis_emulator/travis.man`

 * *Files identical despite different names*

### Comparing `travis_emulator-2.0.5/travis_emulator/travisrc` & `travis_emulator-2.0.6/travis_emulator/travisrc`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env bash
 #
 # Common file for travis emulator scripts
 #
-#__version__=2.0.5
+#__version__=2.0.6
 
 [[ "${BASH_SOURCE-}" == "$0" ]] && echo "You must source this script: \$ source $0" >&2 && exit 33
 XRGI="^(.*\/|)conf\/.*sample$"
 READLINK=$(which greadlink 2>/dev/null) || READLINK=$(which readlink 2>/dev/null)
 export READLINK
 # Based on template 2.0.0
 THIS=$(basename "$0")
@@ -236,18 +236,19 @@
 }
 
 drop_test_db() {
   if [[ "$PRJNAME" == "Odoo" ]]; then
     [[ -n $PGUSER ]] || PGUSER=$USER
     [[ -n $MQT_TEMPLATE_DB ]] || MQT_TEMPLATE_DB="template_odoo"
     [[ -n $MQT_TEST_DB ]] || MQT_TEST_DB="test_odoo"
-    pg_db_active -wa $MQT_TEMPLATE_DB
-    dropdb -U$PGUSER $MQT_TEMPLATE_DB --if-exists &>/dev/null
-    pg_db_active -wa $MQT_TEST_DB
-    dropdb -U$PGUSER $MQT_TEST_DB --if-exists &>/dev/null
+    pg_db_active -wa "$MQT_TEMPLATE_DB" && dropdb -U$PGUSER \"$MQT_TEMPLATE_DB\" --if-exists &>/dev/null
+    c=$(pg_db_active -c "$MQT_TEMPLATE_DB")
+    [[ $c -ne 0 ]] && echo "FATAL! There are $c other sessions using the database \"$MQT_TEMPLATE_DB\""
+    pg_db_active -wa "$MQT_TEST_DB" && dropdb -U$PGUSER "$MQT_TEST_DB" --if-exists &>/dev/null
+    [[ $c -ne 0 ]] && echo "FATAL! There are $c other sessions using the database \"$MQT_TEST_DB\""
   fi
 }
 
 custom_env() {
   # custom_env(VENV pyver)
   cd $1
   sed -i -e 's:VIRTUAL_ENV=.*:VIRTUAL_ENV="\$(readlink -f \$(dirname \$(readlink -f \$BASH_SOURCE))/..)":g' $PWD/bin/activate
```

### Comparing `travis_emulator-2.0.5/travis_emulator/travis` & `travis_emulator-2.0.6/travis_emulator/travis`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.5
+__version__=2.0.6
 
 
 store_cfg_param_value() {
   #store_cfg_param_value(tid key value [opt] [section])
   local p
   if [[ $2 =~ ^pip_pkgver__ ]]; then
     if [ -z "$PIPPKGVER" ]; then
@@ -1041,15 +1041,15 @@
 OPTARGS=(action sub sub2)
 
 parseoptargs "$@"
 if [[ "$opt_version" ]]; then
   echo "$__version__"
   exit $STS_SUCCESS
 fi
-ACTIONS="(help|emulate|force-lint|lint|force-test|test|force-test-multi|test-multi|force-testdeps|testdeps|force-translate|translate|chkconfig|parseyaml|show-log|show-color|summary|wep-db)"
+ACTIONS="(help|emulate|force-lint|lint|force-test|test|force-test-multi|test-multi|force-testdeps|testdeps|force-translate|translate|chkconfig|parseyaml|show|show-log|show-color|summary|wep-db)"
 if [[ $opt_help -gt 0 ]]; then
   print_help "Travis-ci emulator for local developer environment\nAction may be: ${ACTIONS//|/,}" \
   "© 2015-2022 by zeroincombenze®\nhttps://zeroincombenze-tools.readthedocs.io/\nAuthor: antoniomaria.vigliotti@gmail.com"
   exit $STS_SUCCESS
 fi
 
 export PYTHONWARNINGS="ignore"
@@ -1155,33 +1155,35 @@
       if [[ $df -gt $md ]]; then
         [[ $opt_verbose -gt 0 ]] && echo "\$ rm -fR $d ($(date -d@$df -u +"%H:%M:%S") old)"
         rm -fR $d
         ((done_ve++))
         sfx=$(echo "$d" | grep --color=never -Eo "[0-9]+$")
         if [[ -n $PGUSER ]]; then
           for db in template_odoo_$sfx test_odoo_$sfx; do
-            [[ $opt_verbose -gt 0 ]] && echo "\$ dropdb -U$PGUSER $db"
-            pg_db_active -wa $db
-            run_traced "dropdb -U$PGUSER $db --if-exists &>/dev/null"
-            ((done_db++))
+            [[ $opt_verbose -gt 0 ]] && echo "\$ dropdb -U$PGUSER \"$db\""
+            pg_db_active -wa "$db"
+            run_traced "dropdb -U$PGUSER \"$db\" --if-exists &>/dev/null"
+            c=$(pg_db_active -c "$db")
+            [[ $c -ne 0 ]] && echo "FATAL! There are $c other sessions using the database \"$db\"" || ((done_db++))
           done
         fi
       else
         ((dd = md - df))
         echo "$d ($(date -d@$df -u +"%H:%M:%S") old) will be removed in ${dd}s"
         all_dbs=0
       fi
     fi
   done
   if [[ -n $PGUSER && $all_dbs -ne 0 ]]; then
     for db in $(psql -U$PGUSER -Atl | grep -E "(openerp_test|openerp_template|test_openerp|template_openerp|test_odoo|template_odoo)[0-9]+" | awk -F"|" '{print $1}'); do
-      [[ $opt_verbose -gt 0 ]] && echo "\$ dropdb -U$PGUSER $db"
-      pg_db_active -wa $db
-      run_traced "dropdb -U$PGUSER $db --if-exists &>/dev/null"
-      ((done_db++))
+      [[ $opt_verbose -gt 0 ]] && echo "\$ dropdb -U$PGUSER \"$db\""
+      pg_db_active -wa "$db"
+      run_traced "dropdb -U$PGUSER \"$db\" --if-exists &>/dev/null"
+      c=$(pg_db_active -c "$db")
+      [[ $c -ne 0 ]] && echo "FATAL! There are $c other sessions using the database \"$db\"" || ((done_db++))
     done
   fi
   ((md = 60 * 60 * 24 * 90))
   if [[ -n "$LOGDIR" && -d $LOGDIR ]]; then
     for d in $LOGDIR/*; do
       dd=$(stat -c "%Y" $d)
       df=$(($dt - $dd))
@@ -1205,15 +1207,15 @@
     travis_status "$logfile"
     sts=$?
   else
     echo -e "\e[${PS_HDR3_COLOR}mFile $logfile not found!\e[${PS_TXT_COLOR}m"
     sts=1
   fi
   exit $sts
-elif [[ $action == "show-log" ]]; then
+elif [[ $action =~ ^(show|show-log)$ ]]; then
   [[ "$sub" == "old" ]] && logfile=$OLD_LOGFILE || logfile=$LOGFILE
   if [[ ${opt_dry_run:-0} -gt 0 ]]; then
     echo "> travis > $logfile"
     sts=0
   elif [[ -f $logfile ]]; then
     less -R $logfile
     sts=0
```

### Comparing `travis_emulator-2.0.5/setup.py` & `travis_emulator-2.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 setup(
     name='travis_emulator',
-    version='2.0.5',
+    version='2.0.6',
     description='Travis CI emulator for local develop environment',
     long_description="""
 Travis emulator can emulate TravisCi parsing the **.travis.yml** file in local Linux machine.
 You can test your application before pushing code to github.com web site.
 
 Travis emulator can creates all the build declared in **.travis.yml**;
 all the builds are executed in sequential way.
```

### Comparing `travis_emulator-2.0.5/travis_emulator.egg-info/SOURCES.txt` & `travis_emulator-2.0.6/travis_emulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `travis_emulator-2.0.5/travis_emulator.egg-info/PKG-INFO` & `travis_emulator-2.0.6/travis_emulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: travis-emulator
-Version: 2.0.5
+Version: 2.0.6
 Summary: Travis CI emulator for local develop environment
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `travis_emulator-2.0.5/PKG-INFO` & `travis_emulator-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: travis_emulator
-Version: 2.0.5
+Version: 2.0.6
 Summary: Travis CI emulator for local develop environment
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

