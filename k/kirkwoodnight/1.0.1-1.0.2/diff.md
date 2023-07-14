# Comparing `tmp/kirkwoodnight-1.0.1.tar.gz` & `tmp/kirkwoodnight-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kirkwoodnight-1.0.1.tar", last modified: Fri Jul 14 03:13:22 2023, max compression
+gzip compressed data, was "kirkwoodnight-1.0.2.tar", last modified: Fri Jul 14 03:19:54 2023, max compression
```

## Comparing `kirkwoodnight-1.0.1.tar` & `kirkwoodnight-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:13:22.322105 kirkwoodnight-1.0.1/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-1.0.1/LICENSE.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)     5023 2023-07-14 03:13:22.321600 kirkwoodnight-1.0.1/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)     4560 2023-07-13 00:00:36.000000 kirkwoodnight-1.0.1/README.md
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:13:22.315791 kirkwoodnight-1.0.1/kirkwoodnight/
--rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-1.0.1/kirkwoodnight/__init__.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)     4304 2023-07-14 02:42:02.000000 kirkwoodnight-1.0.1/kirkwoodnight/command_line.py
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:13:22.320799 kirkwoodnight-1.0.1/kirkwoodnight/data/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     7833 2023-07-13 23:53:52.000000 kirkwoodnight-1.0.1/kirkwoodnight/data/obj_list.csv
--rw-r--r--   0 armaangoyal   (501) staff       (20)     6350 2023-07-14 03:09:07.000000 kirkwoodnight-1.0.1/kirkwoodnight/plotting.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)    18480 2023-07-14 02:43:02.000000 kirkwoodnight-1.0.1/kirkwoodnight/source.py
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:13:22.320114 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     5023 2023-07-14 03:13:22.000000 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)      392 2023-07-14 03:13:22.000000 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/SOURCES.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-14 03:13:22.000000 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/dependency_links.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-14 03:13:22.000000 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/entry_points.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       69 2023-07-14 03:13:22.000000 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/requires.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-14 03:13:22.000000 kirkwoodnight-1.0.1/kirkwoodnight.egg-info/top_level.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-14 03:13:22.322317 kirkwoodnight-1.0.1/setup.cfg
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-14 03:13:08.000000 kirkwoodnight-1.0.1/setup.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:19:54.282594 kirkwoodnight-1.0.2/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-1.0.2/LICENSE.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     5710 2023-07-14 03:19:54.281952 kirkwoodnight-1.0.2/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     5247 2023-07-14 03:17:45.000000 kirkwoodnight-1.0.2/README.md
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:19:54.277367 kirkwoodnight-1.0.2/kirkwoodnight/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-1.0.2/kirkwoodnight/__init__.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     4304 2023-07-14 02:42:02.000000 kirkwoodnight-1.0.2/kirkwoodnight/command_line.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:19:54.281152 kirkwoodnight-1.0.2/kirkwoodnight/data/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     7833 2023-07-13 23:53:52.000000 kirkwoodnight-1.0.2/kirkwoodnight/data/obj_list.csv
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     6350 2023-07-14 03:09:07.000000 kirkwoodnight-1.0.2/kirkwoodnight/plotting.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)    18480 2023-07-14 02:43:02.000000 kirkwoodnight-1.0.2/kirkwoodnight/source.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:19:54.280509 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     5710 2023-07-14 03:19:54.000000 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)      392 2023-07-14 03:19:54.000000 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/SOURCES.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-14 03:19:54.000000 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/dependency_links.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-14 03:19:54.000000 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/entry_points.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       69 2023-07-14 03:19:54.000000 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/requires.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-14 03:19:54.000000 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/top_level.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-14 03:19:54.282788 kirkwoodnight-1.0.2/setup.cfg
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-14 03:19:16.000000 kirkwoodnight-1.0.2/setup.py
```

### Comparing `kirkwoodnight-1.0.1/LICENSE.txt` & `kirkwoodnight-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.1/PKG-INFO` & `kirkwoodnight-1.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,70 @@
-Metadata-Version: 2.1
-Name: kirkwoodnight
-Version: 1.0.1
-Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
-Home-page: http://packages.python.org/kirkwoodnight
-Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
-Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # kirkwoodnight
 
 [![A rectangular badge, half black half purple containing the text made at Code Astro](https://img.shields.io/badge/Made%20at-Code/Astro-blueviolet.svg)](https://semaphorep.github.io/codeastro/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![PyPI version](https://badge.fury.io/py/kirkwoodnight.svg)](https://badge.fury.io/py/kirkwoodnight)
 
-Interactive command line tool to assist with planning and conducting observations at Indiana University's Kirkwood Observatory. Given a desired date, time, and duration of observation, this program allows the user to toggle various observational constraints to generate an observing schedule for up to 130 objects of interest, including solar system planets, bright stars, and Messier objects. The user may then select the specific objects they would like to observe during the night, upon text files will be generated for each object containing useful information (constellation, magnitude, type of object, etc.) as well as an observing schedule with observability and sky positions (Alt, Az) tabulated at various time intervals.
+Interactive command line tool to assist with planning and conducting observations at Indiana University's Kirkwood Observatory. Given a desired date, time, and duration of observation, this program allows the user to toggle various observational constraints to generate an observing schedule for over 100 objects of interest, including solar system planets, bright stars, and Messier objects. The user may then select specific objects (or types of objects) they would like to observe during the night, upon which the program will generate a file for each object containing characteristic information (constellation, magnitude, type of object, etc.) as well as an observing schedule with sky positions (Alt, Az) tabulated at various time intervals. The user also has the option of generating star charts for these selected objects at each interval of the observing schedule.
 
 ### Prerequisites
-- [Python 3](https://www.python.org/downloads/) or greater
+[Python 3](https://www.python.org/downloads/) or greater.
+
+The following dependencies may be installed with kirkwoodnight:
 - [numpy](https://numpy.org)
 - [pandas](https://pandas.pydata.org)
 - [astropy](https://www.astropy.org)
 - [astroplan](https://astroplan.readthedocs.io/en/latest/#)
 - [skyfield](https://rhodesmill.org/skyfield/)
 - [tabulate](https://pypi.org/project/tabulate/)
 - [colorama](https://pypi.org/project/colorama/)
 
 ### Installing
 
-kirkwoodnight may be installed simply with pip:
+kirkwoodnight may be installed (and updated) simply with pip:
 
     $pip install kirkwoodnight
+    $pip install kirkwoodnight --upgrade
 
 The package repository may also be accessed in full at https://github.com/ag161920/kirkwoodnight.
 
 ## Usage
 
 It is highly recommended that this program is run from a new directory (e.g. "kirkwoodnights"). We also recommend that the terminal is maximized to fill the screen to best display the output tables.
 
 Once the user is in the desired directory, the program may be initiated simply by typing its name in the command line:
 
     $kirkwoodnight
 
-A series of prompts will then be displayed requesting the user to input the desired date (YYYY-MM-DD), time (HH:DD, military time in EST), and duration of their observing run. Then, the user will be asked about a series of observational constraints (hit ENTER to accept the defaults):
+A series of prompts will then be displayed requesting the user to input the desired date (YYYY-MM-DD), time (HH:DD, military time in EST), and duration of their observing run. Then, the user will be asked about a series of observational constraints:
 - Kirkwood's minimum altitude (deg), default is 20
 - Kirkwood's maximum altitude (deg), default is 85
 - Minimum separation from the moon (deg), default is 5
 - Maximum allowable airmass, default is None
 - Desired level of nighttime darkness (options are "civ", "naut", and "astro" respectively for "civil", "nautical", and "astronomical" conventions of nighttime), default is None
 - Desired brightness level for the Moon (options are "grey" or "dark"), default is None
 - How often the user wants to re-check observability (hours), default is 0.5 (every 30 minutes)
 
-Finally, the user will be asked the number of objects they would like displayed in the output tables. Since these objects are sorted by observability, the tables returned will represent the objects that present the best combination of visibility and brightness. The output tables will contain relevant information about these objects, as well as observability over the course of the night.
+Default values may be accepted automatically at each prompt by pressing ENTER. 
+To accept all further default values beyond a given prompt, type "finish".
+To restart the program at any of these prompts, type "restart".
+To terminate the program at any point in time, type "exit".
+
+Following the input of the initial settings and constraints, the user will be asked for the number, type (e.g. Star), and/or subtype (e.g. Main Sequence, Red Supergiant) of objects they would like displayed in the printed tables (hitting ENTER will keep all objects). Since these objects are sorted by observability, the tables will represent the objects that present the best combination of visibility and brightness. The printed tables will contain relevant information about these objects, as well as observability over the course of the night.
 
-The user will then be requested to input the ID numbers (second column, not the names!) of the objects they are most interested in. For each object, a text file will be generated containing characteristic information as well as an observing schedule (with Alt/Az sky positions) for the night. 
+The user will then be asked if they would like to generate information/schedule files for select objects in the table. If the use types "yes", they will be asked to input the ID numbers (second column, not the names!) of the objects they are most interested in. For each object, a text file will be generated containing characteristic information as well as an observing schedule (with Alt/Az sky positions) for the night. 
 
-These text files, as well as a log file describing the parameters and constraints used for the run, will be collected and saved in a 
-"output/[date_time]" directory automatically generated by the program. Each run of the program generates an additional subdirectory in "output", so it is recommended to either delete these output files or save elsewhere those associated with useful runs. 
+The user will then have the option to generate star charts illustrating the sky positions of the selected objects at each block of the observing schedule.
+
+Finally, the user will be asked if they wish to save a log file describing the parameters and constraints used for the run.
+
+All output files are saved to an "output/[date_time]" directory automatically generated by the program.
 
 ## Collaboration and Individual Use
 This code is a work in progress, so comments are welcome and encouraged! Any suggestions for improvement are appreciated, and this code is free to be altered and adapted locally to suit varied individual or institutional needs.
 
-
 ## Authors
   - Armaan Goyal (armgoyal@iu.edu)
   - Brandon Radzom (bradzom@iu.edu)
   - Jessica Ranshaw (jranshaw@iu.edu)
   - Xian-Yu Wang (xwa5@iu.edu)
 
 ## License
```

### Comparing `kirkwoodnight-1.0.1/kirkwoodnight/command_line.py` & `kirkwoodnight-1.0.2/kirkwoodnight/command_line.py`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.1/kirkwoodnight/data/obj_list.csv` & `kirkwoodnight-1.0.2/kirkwoodnight/data/obj_list.csv`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.1/kirkwoodnight/plotting.py` & `kirkwoodnight-1.0.2/kirkwoodnight/plotting.py`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.1/kirkwoodnight/source.py` & `kirkwoodnight-1.0.2/kirkwoodnight/source.py`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.1/setup.py` & `kirkwoodnight-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     reqs = []
     for line in open("requirements.txt", "r").readlines():
         reqs.append(line)
     return reqs
 
 setup(
     name="kirkwoodnight",
-    version="1.0.1",
+    version="1.0.2",
     packages=find_packages(),
 
     # Metadata
     author="Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang",
     author_email="armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu",
     description="Interactive command line tool to assist with observations at Kirkwood Observatory.",
     long_description=open('README.md').read(),
```

