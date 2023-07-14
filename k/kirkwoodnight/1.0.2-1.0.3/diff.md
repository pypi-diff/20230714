# Comparing `tmp/kirkwoodnight-1.0.2.tar.gz` & `tmp/kirkwoodnight-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kirkwoodnight-1.0.2.tar", last modified: Fri Jul 14 03:19:54 2023, max compression
+gzip compressed data, was "kirkwoodnight-1.0.3.tar", last modified: Fri Jul 14 17:40:57 2023, max compression
```

## Comparing `kirkwoodnight-1.0.2.tar` & `kirkwoodnight-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:19:54.282594 kirkwoodnight-1.0.2/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-1.0.2/LICENSE.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)     5710 2023-07-14 03:19:54.281952 kirkwoodnight-1.0.2/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)     5247 2023-07-14 03:17:45.000000 kirkwoodnight-1.0.2/README.md
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:19:54.277367 kirkwoodnight-1.0.2/kirkwoodnight/
--rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-1.0.2/kirkwoodnight/__init__.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)     4304 2023-07-14 02:42:02.000000 kirkwoodnight-1.0.2/kirkwoodnight/command_line.py
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:19:54.281152 kirkwoodnight-1.0.2/kirkwoodnight/data/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     7833 2023-07-13 23:53:52.000000 kirkwoodnight-1.0.2/kirkwoodnight/data/obj_list.csv
--rw-r--r--   0 armaangoyal   (501) staff       (20)     6350 2023-07-14 03:09:07.000000 kirkwoodnight-1.0.2/kirkwoodnight/plotting.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)    18480 2023-07-14 02:43:02.000000 kirkwoodnight-1.0.2/kirkwoodnight/source.py
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 03:19:54.280509 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     5710 2023-07-14 03:19:54.000000 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)      392 2023-07-14 03:19:54.000000 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/SOURCES.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-14 03:19:54.000000 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/dependency_links.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-14 03:19:54.000000 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/entry_points.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       69 2023-07-14 03:19:54.000000 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/requires.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-14 03:19:54.000000 kirkwoodnight-1.0.2/kirkwoodnight.egg-info/top_level.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-14 03:19:54.282788 kirkwoodnight-1.0.2/setup.cfg
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-14 03:19:16.000000 kirkwoodnight-1.0.2/setup.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 17:40:57.446102 kirkwoodnight-1.0.3/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-1.0.3/LICENSE.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     5951 2023-07-14 17:40:57.445554 kirkwoodnight-1.0.3/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     5488 2023-07-14 17:39:27.000000 kirkwoodnight-1.0.3/README.md
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 17:40:57.436800 kirkwoodnight-1.0.3/kirkwoodnight/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-1.0.3/kirkwoodnight/__init__.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     4304 2023-07-14 02:42:02.000000 kirkwoodnight-1.0.3/kirkwoodnight/command_line.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 17:40:57.444035 kirkwoodnight-1.0.3/kirkwoodnight/data/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     7833 2023-07-13 23:53:52.000000 kirkwoodnight-1.0.3/kirkwoodnight/data/obj_list.csv
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     6350 2023-07-14 03:09:07.000000 kirkwoodnight-1.0.3/kirkwoodnight/plotting.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)    18480 2023-07-14 17:40:08.000000 kirkwoodnight-1.0.3/kirkwoodnight/source.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 17:40:57.443296 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     5951 2023-07-14 17:40:57.000000 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)      392 2023-07-14 17:40:57.000000 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/SOURCES.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-14 17:40:57.000000 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/dependency_links.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-14 17:40:57.000000 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/entry_points.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       69 2023-07-14 17:40:57.000000 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/requires.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-14 17:40:57.000000 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/top_level.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-14 17:40:57.446322 kirkwoodnight-1.0.3/setup.cfg
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-14 17:40:02.000000 kirkwoodnight-1.0.3/setup.py
```

### Comparing `kirkwoodnight-1.0.2/LICENSE.txt` & `kirkwoodnight-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.2/PKG-INFO` & `kirkwoodnight-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 1.0.2
+Version: 1.0.3
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # kirkwoodnight
 
 [![A rectangular badge, half black half purple containing the text made at Code Astro](https://img.shields.io/badge/Made%20at-Code/Astro-blueviolet.svg)](https://semaphorep.github.io/codeastro/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![Static Badge](https://img.shields.io/badge/PyPI_Package-1.0.3-green)
+[![DOI](https://zenodo.org/badge/665627819.svg)](https://zenodo.org/badge/latestdoi/665627819)
 
 Interactive command line tool to assist with planning and conducting observations at Indiana University's Kirkwood Observatory. Given a desired date, time, and duration of observation, this program allows the user to toggle various observational constraints to generate an observing schedule for over 100 objects of interest, including solar system planets, bright stars, and Messier objects. The user may then select specific objects (or types of objects) they would like to observe during the night, upon which the program will generate a file for each object containing characteristic information (constellation, magnitude, type of object, etc.) as well as an observing schedule with sky positions (Alt, Az) tabulated at various time intervals. The user also has the option of generating star charts for these selected objects at each interval of the observing schedule.
 
 ### Prerequisites
 [Python 3](https://www.python.org/downloads/) or greater.
 
 The following dependencies may be installed with kirkwoodnight:
@@ -55,19 +57,23 @@
 - How often the user wants to re-check observability (hours), default is 0.5 (every 30 minutes)
 
 Default values may be accepted automatically at each prompt by pressing ENTER. 
 To accept all further default values beyond a given prompt, type "finish".
 To restart the program at any of these prompts, type "restart".
 To terminate the program at any point in time, type "exit".
 
-Following the input of the initial settings and constraints, the user will be asked for the number, type (e.g. Star), and/or subtype (e.g. Main Sequence, Red Supergiant) of objects they would like displayed in the printed tables (hitting ENTER will keep all objects). Since these objects are sorted by observability, the tables will represent the objects that present the best combination of visibility and brightness. The printed tables will contain relevant information about these objects, as well as observability over the course of the night.
+Following the input of the initial settings and constraints, the user will be asked for the number, type (e.g. Star), and/or subtype (e.g. Main Sequence, Red Supergiant) of objects they would like displayed in the printed tables (hitting ENTER will keep all objects). Since these objects are sorted by observability, the tables will represent the objects that present the best combination of visibility and brightness. The printed tables will contain relevant information about these objects, as well as observability over the course of the night:
 
-The user will then be asked if they would like to generate information/schedule files for select objects in the table. If the use types "yes", they will be asked to input the ID numbers (second column, not the names!) of the objects they are most interested in. For each object, a text file will be generated containing characteristic information as well as an observing schedule (with Alt/Az sky positions) for the night. 
+![Screenshot](example_output.png)
 
-The user will then have the option to generate star charts illustrating the sky positions of the selected objects at each block of the observing schedule.
+The user will then be asked if they would like to generate information/schedule files for select objects in the table. If the user types "yes", they will be asked to input the ID numbers (second column, not the names!) of the objects they are most interested in. For each object, a text file will be generated containing characteristic information as well as an observing schedule (with Alt/Az sky positions) for the night. 
+
+The user will then have the option to generate star charts illustrating the sky positions of the selected objects at each block of the observing schedule:
+
+![Screenshot](example_star_chart.png)
 
 Finally, the user will be asked if they wish to save a log file describing the parameters and constraints used for the run.
 
 All output files are saved to an "output/[date_time]" directory automatically generated by the program.
 
 ## Collaboration and Individual Use
 This code is a work in progress, so comments are welcome and encouraged! Any suggestions for improvement are appreciated, and this code is free to be altered and adapted locally to suit varied individual or institutional needs.
```

### Comparing `kirkwoodnight-1.0.2/README.md` & `kirkwoodnight-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # kirkwoodnight
 
 [![A rectangular badge, half black half purple containing the text made at Code Astro](https://img.shields.io/badge/Made%20at-Code/Astro-blueviolet.svg)](https://semaphorep.github.io/codeastro/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![Static Badge](https://img.shields.io/badge/PyPI_Package-1.0.3-green)
+[![DOI](https://zenodo.org/badge/665627819.svg)](https://zenodo.org/badge/latestdoi/665627819)
 
 Interactive command line tool to assist with planning and conducting observations at Indiana University's Kirkwood Observatory. Given a desired date, time, and duration of observation, this program allows the user to toggle various observational constraints to generate an observing schedule for over 100 objects of interest, including solar system planets, bright stars, and Messier objects. The user may then select specific objects (or types of objects) they would like to observe during the night, upon which the program will generate a file for each object containing characteristic information (constellation, magnitude, type of object, etc.) as well as an observing schedule with sky positions (Alt, Az) tabulated at various time intervals. The user also has the option of generating star charts for these selected objects at each interval of the observing schedule.
 
 ### Prerequisites
 [Python 3](https://www.python.org/downloads/) or greater.
 
 The following dependencies may be installed with kirkwoodnight:
@@ -44,19 +46,23 @@
 - How often the user wants to re-check observability (hours), default is 0.5 (every 30 minutes)
 
 Default values may be accepted automatically at each prompt by pressing ENTER. 
 To accept all further default values beyond a given prompt, type "finish".
 To restart the program at any of these prompts, type "restart".
 To terminate the program at any point in time, type "exit".
 
-Following the input of the initial settings and constraints, the user will be asked for the number, type (e.g. Star), and/or subtype (e.g. Main Sequence, Red Supergiant) of objects they would like displayed in the printed tables (hitting ENTER will keep all objects). Since these objects are sorted by observability, the tables will represent the objects that present the best combination of visibility and brightness. The printed tables will contain relevant information about these objects, as well as observability over the course of the night.
+Following the input of the initial settings and constraints, the user will be asked for the number, type (e.g. Star), and/or subtype (e.g. Main Sequence, Red Supergiant) of objects they would like displayed in the printed tables (hitting ENTER will keep all objects). Since these objects are sorted by observability, the tables will represent the objects that present the best combination of visibility and brightness. The printed tables will contain relevant information about these objects, as well as observability over the course of the night:
 
-The user will then be asked if they would like to generate information/schedule files for select objects in the table. If the use types "yes", they will be asked to input the ID numbers (second column, not the names!) of the objects they are most interested in. For each object, a text file will be generated containing characteristic information as well as an observing schedule (with Alt/Az sky positions) for the night. 
+![Screenshot](example_output.png)
 
-The user will then have the option to generate star charts illustrating the sky positions of the selected objects at each block of the observing schedule.
+The user will then be asked if they would like to generate information/schedule files for select objects in the table. If the user types "yes", they will be asked to input the ID numbers (second column, not the names!) of the objects they are most interested in. For each object, a text file will be generated containing characteristic information as well as an observing schedule (with Alt/Az sky positions) for the night. 
+
+The user will then have the option to generate star charts illustrating the sky positions of the selected objects at each block of the observing schedule:
+
+![Screenshot](example_star_chart.png)
 
 Finally, the user will be asked if they wish to save a log file describing the parameters and constraints used for the run.
 
 All output files are saved to an "output/[date_time]" directory automatically generated by the program.
 
 ## Collaboration and Individual Use
 This code is a work in progress, so comments are welcome and encouraged! Any suggestions for improvement are appreciated, and this code is free to be altered and adapted locally to suit varied individual or institutional needs.
```

### Comparing `kirkwoodnight-1.0.2/kirkwoodnight/command_line.py` & `kirkwoodnight-1.0.3/kirkwoodnight/command_line.py`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.2/kirkwoodnight/data/obj_list.csv` & `kirkwoodnight-1.0.3/kirkwoodnight/data/obj_list.csv`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.2/kirkwoodnight/plotting.py` & `kirkwoodnight-1.0.3/kirkwoodnight/plotting.py`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.2/kirkwoodnight/source.py` & `kirkwoodnight-1.0.3/kirkwoodnight/source.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -221,17 +221,17 @@
     time_grid, total_obs, obs_percent = make_obs_grid(kirkwood, constraints, targets, t1_ust, t2_ust, dt)
     
     # build dataframe of all targets, add column for observability fraction
     target_df["Obs. Frac."] = obs_percent
     target_df = target_df.set_index("Name")
     target_df["V Mag"] = target_df["V Mag"].astype(float)
     target_names_all = list(target_df.index)
+    target_df.insert(0, "ID", range(1, len(target_df) + 1))
     target_df = target_df.sort_values(by=['Obs. Frac.', "V Mag"], ascending = [False, True]) # sort table by observability and brightness
     target_df = target_df.round(2)
-    target_df.insert(0, "ID", range(1, len(target_df) + 1))
 
     types = list(set(target_df["Type"]))
     types = [" " + item for item in types]
     print("Is/are there a particular type(s) of object you would like to look at? The options are:\n")
     print(",".join([i for i in types]))
     print("\nPlease enter the type(s) of the objects you would like to observe, separated by commas (if multiple). Hit ENTER to observe all listed types.")
     var = input()
```

### Comparing `kirkwoodnight-1.0.2/kirkwoodnight.egg-info/PKG-INFO` & `kirkwoodnight-1.0.3/kirkwoodnight.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 1.0.2
+Version: 1.0.3
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # kirkwoodnight
 
 [![A rectangular badge, half black half purple containing the text made at Code Astro](https://img.shields.io/badge/Made%20at-Code/Astro-blueviolet.svg)](https://semaphorep.github.io/codeastro/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![Static Badge](https://img.shields.io/badge/PyPI_Package-1.0.3-green)
+[![DOI](https://zenodo.org/badge/665627819.svg)](https://zenodo.org/badge/latestdoi/665627819)
 
 Interactive command line tool to assist with planning and conducting observations at Indiana University's Kirkwood Observatory. Given a desired date, time, and duration of observation, this program allows the user to toggle various observational constraints to generate an observing schedule for over 100 objects of interest, including solar system planets, bright stars, and Messier objects. The user may then select specific objects (or types of objects) they would like to observe during the night, upon which the program will generate a file for each object containing characteristic information (constellation, magnitude, type of object, etc.) as well as an observing schedule with sky positions (Alt, Az) tabulated at various time intervals. The user also has the option of generating star charts for these selected objects at each interval of the observing schedule.
 
 ### Prerequisites
 [Python 3](https://www.python.org/downloads/) or greater.
 
 The following dependencies may be installed with kirkwoodnight:
@@ -55,19 +57,23 @@
 - How often the user wants to re-check observability (hours), default is 0.5 (every 30 minutes)
 
 Default values may be accepted automatically at each prompt by pressing ENTER. 
 To accept all further default values beyond a given prompt, type "finish".
 To restart the program at any of these prompts, type "restart".
 To terminate the program at any point in time, type "exit".
 
-Following the input of the initial settings and constraints, the user will be asked for the number, type (e.g. Star), and/or subtype (e.g. Main Sequence, Red Supergiant) of objects they would like displayed in the printed tables (hitting ENTER will keep all objects). Since these objects are sorted by observability, the tables will represent the objects that present the best combination of visibility and brightness. The printed tables will contain relevant information about these objects, as well as observability over the course of the night.
+Following the input of the initial settings and constraints, the user will be asked for the number, type (e.g. Star), and/or subtype (e.g. Main Sequence, Red Supergiant) of objects they would like displayed in the printed tables (hitting ENTER will keep all objects). Since these objects are sorted by observability, the tables will represent the objects that present the best combination of visibility and brightness. The printed tables will contain relevant information about these objects, as well as observability over the course of the night:
 
-The user will then be asked if they would like to generate information/schedule files for select objects in the table. If the use types "yes", they will be asked to input the ID numbers (second column, not the names!) of the objects they are most interested in. For each object, a text file will be generated containing characteristic information as well as an observing schedule (with Alt/Az sky positions) for the night. 
+![Screenshot](example_output.png)
 
-The user will then have the option to generate star charts illustrating the sky positions of the selected objects at each block of the observing schedule.
+The user will then be asked if they would like to generate information/schedule files for select objects in the table. If the user types "yes", they will be asked to input the ID numbers (second column, not the names!) of the objects they are most interested in. For each object, a text file will be generated containing characteristic information as well as an observing schedule (with Alt/Az sky positions) for the night. 
+
+The user will then have the option to generate star charts illustrating the sky positions of the selected objects at each block of the observing schedule:
+
+![Screenshot](example_star_chart.png)
 
 Finally, the user will be asked if they wish to save a log file describing the parameters and constraints used for the run.
 
 All output files are saved to an "output/[date_time]" directory automatically generated by the program.
 
 ## Collaboration and Individual Use
 This code is a work in progress, so comments are welcome and encouraged! Any suggestions for improvement are appreciated, and this code is free to be altered and adapted locally to suit varied individual or institutional needs.
```

### Comparing `kirkwoodnight-1.0.2/setup.py` & `kirkwoodnight-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     reqs = []
     for line in open("requirements.txt", "r").readlines():
         reqs.append(line)
     return reqs
 
 setup(
     name="kirkwoodnight",
-    version="1.0.2",
+    version="1.0.3",
     packages=find_packages(),
 
     # Metadata
     author="Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang",
     author_email="armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu",
     description="Interactive command line tool to assist with observations at Kirkwood Observatory.",
     long_description=open('README.md').read(),
```

