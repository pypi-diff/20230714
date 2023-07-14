# Comparing `tmp/REFPROP_connector-0.3.2.tar.gz` & `tmp/REFPROP_connector-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "REFPROP_connector-0.3.2.tar", last modified: Tue Apr 11 17:38:50 2023, max compression
+gzip compressed data, was "REFPROP_connector-0.3.3.tar", last modified: Fri Jul 14 14:23:34 2023, max compression
```

## Comparing `REFPROP_connector-0.3.2.tar` & `REFPROP_connector-0.3.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.816597 REFPROP_connector-0.3.2/
--rw-rw-rw-   0        0        0       26 2022-06-23 09:23:17.000000 REFPROP_connector-0.3.2/.gitignore
--rw-rw-rw-   0        0        0    35823 2021-12-10 08:32:10.000000 REFPROP_connector-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     6186 2023-04-11 17:38:50.816597 REFPROP_connector-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4376 2021-12-10 10:47:30.000000 REFPROP_connector-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.783423 REFPROP_connector-0.3.2/REFPROPConnector/
--rwxrwxrwx   0        0        0  5280688 2021-12-10 08:32:10.000000 REFPROP_connector-0.3.2/REFPROPConnector/NIST2310.EXE
-drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.786471 REFPROP_connector-0.3.2/REFPROPConnector/Support/
--rw-rw-rw-   0        0        0        0 2022-02-03 11:33:25.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/__init__.py
--rw-rw-rw-   0        0        0     1558 2022-02-03 16:21:28.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/constants.py
--rw-rw-rw-   0        0        0    10679 2022-02-03 16:47:42.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/refprop_names_tree.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.798484 REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/
--rw-rw-rw-   0        0        0       30 2023-04-11 17:32:53.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/REFPROP_exec.dat
--rw-rw-rw-   0        0        0    16788 2023-04-11 17:29:02.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/REFPROP_names.xml
--rw-rw-rw-   0        0        0        0 2022-02-03 11:35:20.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/__init__.py
--rw-rw-rw-   0        0        0     2906 2023-03-23 09:57:25.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/file_handler.py
--rw-rw-rw-   0        0        0    17049 2023-04-11 17:29:02.000000 REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/rp_names_file_generator.py
--rw-rw-rw-   0        0        0      190 2022-02-03 11:47:19.000000 REFPROP_connector-0.3.2/REFPROPConnector/__init__.py
--rw-rw-rw-   0        0        0    27241 2023-01-27 16:53:10.000000 REFPROP_connector-0.3.2/REFPROPConnector/refprop_calculator.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.785436 REFPROP_connector-0.3.2/REFPROPConnectorTest/
--rw-rw-rw-   0        0        0        0 2021-12-10 10:12:18.000000 REFPROP_connector-0.3.2/REFPROPConnectorTest/__init__.py
--rw-rw-rw-   0        0        0     2828 2023-04-11 17:32:51.000000 REFPROP_connector-0.3.2/REFPROPConnectorTest/test_file.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.815597 REFPROP_connector-0.3.2/REFPROP_connector.egg-info/
--rw-rw-rw-   0        0        0     6186 2023-04-11 17:38:50.000000 REFPROP_connector-0.3.2/REFPROP_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-04-11 17:38:50.000000 REFPROP_connector-0.3.2/REFPROP_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 17:38:50.000000 REFPROP_connector-0.3.2/REFPROP_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-11 17:38:50.000000 REFPROP_connector-0.3.2/REFPROP_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-04-11 17:38:50.000000 REFPROP_connector-0.3.2/REFPROP_connector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       87 2023-03-23 10:11:51.000000 REFPROP_connector-0.3.2/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-04-11 17:38:50.817580 REFPROP_connector-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     2228 2023-04-11 17:37:39.000000 REFPROP_connector-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 17:38:50.816597 REFPROP_connector-0.3.2/twine_upload/
--rw-rw-rw-   0        0        0     1089 2022-06-21 16:26:22.000000 REFPROP_connector-0.3.2/twine_upload/pip_upload.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:23:34.043933 REFPROP_connector-0.3.3/
+-rw-rw-rw-   0        0        0       26 2022-06-23 09:23:17.000000 REFPROP_connector-0.3.3/.gitignore
+-rw-rw-rw-   0        0        0    35823 2021-12-10 08:32:10.000000 REFPROP_connector-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     7423 2023-07-14 14:23:34.043933 REFPROP_connector-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5261 2023-07-14 14:18:47.000000 REFPROP_connector-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 14:23:34.014933 REFPROP_connector-0.3.3/REFPROPConnector/
+-rwxrwxrwx   0        0        0  5280688 2021-12-10 08:32:10.000000 REFPROP_connector-0.3.3/REFPROPConnector/NIST2310.EXE
+drwxrwxrwx   0        0        0        0 2023-07-14 14:23:34.017933 REFPROP_connector-0.3.3/REFPROPConnector/Support/
+-rw-rw-rw-   0        0        0        0 2022-02-03 11:33:25.000000 REFPROP_connector-0.3.3/REFPROPConnector/Support/__init__.py
+-rw-rw-rw-   0        0        0     1558 2022-02-03 16:21:28.000000 REFPROP_connector-0.3.3/REFPROPConnector/Support/constants.py
+-rw-rw-rw-   0        0        0    10679 2022-02-03 16:47:42.000000 REFPROP_connector-0.3.3/REFPROPConnector/Support/refprop_names_tree.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:23:34.021933 REFPROP_connector-0.3.3/REFPROPConnector/Support/resources/
+-rw-rw-rw-   0        0        0       30 2023-07-14 14:03:33.000000 REFPROP_connector-0.3.3/REFPROPConnector/Support/resources/REFPROP_exec.dat
+-rw-rw-rw-   0        0        0    16788 2023-04-11 17:29:02.000000 REFPROP_connector-0.3.3/REFPROPConnector/Support/resources/REFPROP_names.xml
+-rw-rw-rw-   0        0        0        0 2022-02-03 11:35:20.000000 REFPROP_connector-0.3.3/REFPROPConnector/Support/resources/__init__.py
+-rw-rw-rw-   0        0        0     2906 2023-03-23 09:57:25.000000 REFPROP_connector-0.3.3/REFPROPConnector/Support/resources/file_handler.py
+-rw-rw-rw-   0        0        0    17049 2023-04-11 17:29:02.000000 REFPROP_connector-0.3.3/REFPROPConnector/Support/resources/rp_names_file_generator.py
+-rw-rw-rw-   0        0        0      274 2023-07-14 13:26:58.000000 REFPROP_connector-0.3.3/REFPROPConnector/__init__.py
+-rw-rw-rw-   0        0        0    27241 2023-01-27 16:53:10.000000 REFPROP_connector-0.3.3/REFPROPConnector/refprop_calculator.py
+-rw-rw-rw-   0        0        0    12110 2023-07-14 14:17:58.000000 REFPROP_connector-0.3.3/REFPROPConnector/refprop_plotter.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:23:34.015933 REFPROP_connector-0.3.3/REFPROPConnectorTest/
+-rw-rw-rw-   0        0        0        0 2021-12-10 10:12:18.000000 REFPROP_connector-0.3.3/REFPROPConnectorTest/__init__.py
+-rw-rw-rw-   0        0        0     3525 2023-07-14 14:03:32.000000 REFPROP_connector-0.3.3/REFPROPConnectorTest/test_file.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:23:34.042933 REFPROP_connector-0.3.3/REFPROP_connector.egg-info/
+-rw-rw-rw-   0        0        0     7423 2023-07-14 14:23:33.000000 REFPROP_connector-0.3.3/REFPROP_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      883 2023-07-14 14:23:33.000000 REFPROP_connector-0.3.3/REFPROP_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 14:23:33.000000 REFPROP_connector-0.3.3/REFPROP_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-14 14:23:33.000000 REFPROP_connector-0.3.3/REFPROP_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-07-14 14:23:33.000000 REFPROP_connector-0.3.3/REFPROP_connector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-07-14 13:26:58.000000 REFPROP_connector-0.3.3/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-07-14 14:23:34.047933 REFPROP_connector-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     2268 2023-07-14 13:26:58.000000 REFPROP_connector-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 14:23:34.042933 REFPROP_connector-0.3.3/twine_upload/
+-rw-rw-rw-   0        0        0     1089 2022-06-21 16:26:22.000000 REFPROP_connector-0.3.3/twine_upload/pip_upload.py
```

### Comparing `REFPROP_connector-0.3.2/LICENSE` & `REFPROP_connector-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.2/PKG-INFO` & `REFPROP_connector-0.3.3/REFPROP_connector.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
-Name: REFPROP_connector
-Version: 0.3.2
+Name: REFPROP-connector
+Version: 0.3.3
 Summary: Tools for launching REFPROP calculation and retrieving results from python
 Home-page: https://www.dief.unifi.it/vp-177-serg-group-english-version.html
 Author: Pietro Ungar
 Author-email: pietro.ungar@unifi.it
 License: GNU GPLv3
-Download-URL: https://github.com/SERGGroup/REFPROPConnector/archive/refs/tags/0.3.2.tar.gz
+Download-URL: https://github.com/SERGGroup/REFPROPConnector/archive/refs/tags/0.3.3.tar.gz
 Project-URL: Source, https://github.com/SERGGroup/REFPROPConnector
 Project-URL: Tracker, https://github.com/SERGGroup/REFPROPConnector/issues
 Description: # REFPROP connector
         
         __REFPROP connector__ is a tools developed by the [SERG research group](https://www.dief.unifi.it/vp-177-serg-group-english-version.html) 
         of the [University of Florence](https://www.unifi.it/changelang-eng.html) for launching [REFPROP](https://www.nist.gov/srd/refprop) 
         calculation and retrieving results from python. 
         
         In order to use the code you must have both REFPROP and the [REFPROP wrappers for Python](https://github.com/usnistgov/REFPROP-wrappers) 
         installed and properly working.
         
         The scope of this library is to make the usage of the refprop wrappers simpler.
         
+        ### Download and installation 
+        
         The beta version can be downloaded using __PIP__:
         
         ```
         pip install REFPROP_connector
         ```
+        
+        ### First Steps
         Once the installation has been completed the user can import the tool and initialize the connector itself.
         ```python
         from REFPROPConnector import ThermodynamicPoint
         
         tp = ThermodynamicPoint(["air"], [1.])
         
         ```
@@ -41,14 +45,15 @@
             
         ```python
         from REFPROPConnector import retreive_RP_exec
         
         retreive_RP_exec()
         ```
             
+        ### Basic Usage
         
         Each _ThermodynamicPoint_ class instance represent a thermodynamic state, hence you had to provide at least 
         __two indipendent state variables__ in order to calculate the others.
         
         
         ```python
         from REFPROPConnector import ThermodynamicPoint
@@ -57,14 +62,16 @@
         
         tp.set_variable("P", 0.101325)     # P in MPa (ambient pressure)
         tp.set_variable("Q", 0.5)          # vapour quality for multiphase condition
         
         T_sat = tp.get_variable("T")       # saturation temperature in celsius (100 °C)
         ```
         
+        ### Abstract Class
+        
         _AbstractThermodynamicPoint_ is a class that can be overwritten in order to perform some calculation once both 
         independent state variable have been set. It can be useful for example for the evaluation of the reynolds number 
         for a fluid flowing in a pipe.
         
         ```python
         from REFPROPConnector import AbstractThermodynamicPoint, RefPropHandler
         import numpy as np
@@ -91,15 +98,15 @@
         if __name__ == "__main__":
         
             section = TubeSection(0.5, 1)
             
             """
             
                 The following line will return 0. as the function "other_calculation" 
-                is called only when 2 independent state variable is provided 
+                is called only when 2 independent state variables are provided 
                 
             """
             print(section.get_variable("Re"))   
             
             section.set_variable("P", 0.5)
             section.set_variable("T", 20)
             
@@ -107,34 +114,71 @@
             
                 The following line will return the actual Reynolds number
                 
             """
             print(section.get_variable("Re"))
         ```
         
+        ### Unit system and state variable list
+        
         Variable that can be calculated can be listed using _list_properties_ method from both _ThermodynamicPoint_ and 
         _AbstractThermodynamicPoint_ (the name __is not case-sensitive__). Finally, user can also select the unit system to be 
         used in the calculation, a list of possible unit system can be revived calling the method _list_unit_systems()_ 
         (current unit_system will be highlighted):  
         
         ```python
         from REFPROPConnector import ThermodynamicPoint
         
         tp = ThermodynamicPoint(["water"], [1.], unit_system="MASS BASE SI")
         tp.list_properties()
         tp.list_unit_systems()
         ```
-        Defaul unit system is __SI with C__
+        Default unit system is __SI with C__
+        
+        ### Diagram Plotter
+        The _DiagramPlotter_ class can be used to plot a specific state diagram that can be then used to describe state 
+        transformations. The diagram can be personalized using the _DiagramPlotterOptions_ class. 
+        The following is an example on how to use the class.
+        
+        
+        ```python
+        from REFPROPConnector import (
+            
+            ThermodynamicPoint, 
+            DiagramPlotter, 
+            DiagramPlotterOptions
+        
+        )
+        
+        tp = ThermodynamicPoint(["Carbon Dioxide"], [1])
+        options = DiagramPlotterOptions(
+        
+            x_variable="T",
+            x_var_range = (0, 150), x_var_log=False,
+            y_var_range = (4, 15),
+            isoline_ranges={
         
-        For other information please contact: _pietro.ungar@unifi.it_
+                "rho": (50, 1000, 25),
+                "H": (200, 550, 25)
+        
+            }
+        
+        )
+        plotter = DiagramPlotter(tp, options=options)
+        plotter.calculate()
+        
+        fig, (ax_1) = plt.subplots(1, 1, dpi=200)
+        fig.set_size_inches(10, 5)
+        plotter.plot(ax_1)
+        plt.show()
+        ```
         
         __-------------------------- !!! THIS IS A BETA VERSION !!! --------------------------__ 
         
         please report any bug or problems in the installation to _pietro.ungar@unifi.it_<br/>
-        for further information visit: https://tinyurl.com/SERG-3ETool
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `REFPROP_connector-0.3.2/README.md` & `REFPROP_connector-0.3.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 calculation and retrieving results from python. 
 
 In order to use the code you must have both REFPROP and the [REFPROP wrappers for Python](https://github.com/usnistgov/REFPROP-wrappers) 
 installed and properly working.
 
 The scope of this library is to make the usage of the refprop wrappers simpler.
 
+### Download and installation 
+
 The beta version can be downloaded using __PIP__:
 
 ```
 pip install REFPROP_connector
 ```
+
+### First Steps
 Once the installation has been completed the user can import the tool and initialize the connector itself.
 ```python
 from REFPROPConnector import ThermodynamicPoint
 
 tp = ThermodynamicPoint(["air"], [1.])
 
 ```
@@ -30,14 +34,15 @@
     
 ```python
 from REFPROPConnector import retreive_RP_exec
 
 retreive_RP_exec()
 ```
     
+### Basic Usage
 
 Each _ThermodynamicPoint_ class instance represent a thermodynamic state, hence you had to provide at least 
 __two indipendent state variables__ in order to calculate the others.
 
 
 ```python
 from REFPROPConnector import ThermodynamicPoint
@@ -46,14 +51,16 @@
 
 tp.set_variable("P", 0.101325)     # P in MPa (ambient pressure)
 tp.set_variable("Q", 0.5)          # vapour quality for multiphase condition
 
 T_sat = tp.get_variable("T")       # saturation temperature in celsius (100 °C)
 ```
 
+### Abstract Class
+
 _AbstractThermodynamicPoint_ is a class that can be overwritten in order to perform some calculation once both 
 independent state variable have been set. It can be useful for example for the evaluation of the reynolds number 
 for a fluid flowing in a pipe.
 
 ```python
 from REFPROPConnector import AbstractThermodynamicPoint, RefPropHandler
 import numpy as np
@@ -80,15 +87,15 @@
 if __name__ == "__main__":
 
     section = TubeSection(0.5, 1)
     
     """
     
         The following line will return 0. as the function "other_calculation" 
-        is called only when 2 independent state variable is provided 
+        is called only when 2 independent state variables are provided 
         
     """
     print(section.get_variable("Re"))   
     
     section.set_variable("P", 0.5)
     section.set_variable("T", 20)
     
@@ -96,27 +103,64 @@
     
         The following line will return the actual Reynolds number
         
     """
     print(section.get_variable("Re"))
 ```
 
+### Unit system and state variable list
+
 Variable that can be calculated can be listed using _list_properties_ method from both _ThermodynamicPoint_ and 
 _AbstractThermodynamicPoint_ (the name __is not case-sensitive__). Finally, user can also select the unit system to be 
 used in the calculation, a list of possible unit system can be revived calling the method _list_unit_systems()_ 
 (current unit_system will be highlighted):  
 
 ```python
 from REFPROPConnector import ThermodynamicPoint
 
 tp = ThermodynamicPoint(["water"], [1.], unit_system="MASS BASE SI")
 tp.list_properties()
 tp.list_unit_systems()
 ```
-Defaul unit system is __SI with C__
+Default unit system is __SI with C__
+
+### Diagram Plotter
+The _DiagramPlotter_ class can be used to plot a specific state diagram that can be then used to describe state 
+transformations. The diagram can be personalized using the _DiagramPlotterOptions_ class. 
+The following is an example on how to use the class.
+
+
+```python
+from REFPROPConnector import (
+    
+    ThermodynamicPoint, 
+    DiagramPlotter, 
+    DiagramPlotterOptions
+
+)
+
+tp = ThermodynamicPoint(["Carbon Dioxide"], [1])
+options = DiagramPlotterOptions(
+
+    x_variable="T",
+    x_var_range = (0, 150), x_var_log=False,
+    y_var_range = (4, 15),
+    isoline_ranges={
 
-For other information please contact: _pietro.ungar@unifi.it_
+        "rho": (50, 1000, 25),
+        "H": (200, 550, 25)
+
+    }
+
+)
+plotter = DiagramPlotter(tp, options=options)
+plotter.calculate()
+
+fig, (ax_1) = plt.subplots(1, 1, dpi=200)
+fig.set_size_inches(10, 5)
+plotter.plot(ax_1)
+plt.show()
+```
 
 __-------------------------- !!! THIS IS A BETA VERSION !!! --------------------------__ 
 
 please report any bug or problems in the installation to _pietro.ungar@unifi.it_<br/>
-for further information visit: https://tinyurl.com/SERG-3ETool
```

### Comparing `REFPROP_connector-0.3.2/REFPROPConnector/NIST2310.EXE` & `REFPROP_connector-0.3.3/REFPROPConnector/NIST2310.EXE`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.2/REFPROPConnector/Support/constants.py` & `REFPROP_connector-0.3.3/REFPROPConnector/Support/constants.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.2/REFPROPConnector/Support/refprop_names_tree.py` & `REFPROP_connector-0.3.3/REFPROPConnector/Support/refprop_names_tree.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/REFPROP_names.xml` & `REFPROP_connector-0.3.3/REFPROPConnector/Support/resources/REFPROP_names.xml`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/file_handler.py` & `REFPROP_connector-0.3.3/REFPROPConnector/Support/resources/file_handler.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.2/REFPROPConnector/Support/resources/rp_names_file_generator.py` & `REFPROP_connector-0.3.3/REFPROPConnector/Support/resources/rp_names_file_generator.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.2/REFPROPConnector/refprop_calculator.py` & `REFPROP_connector-0.3.3/REFPROPConnector/refprop_calculator.py`

 * *Files identical despite different names*

### Comparing `REFPROP_connector-0.3.2/REFPROP_connector.egg-info/PKG-INFO` & `REFPROP_connector-0.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
-Name: REFPROP-connector
-Version: 0.3.2
+Name: REFPROP_connector
+Version: 0.3.3
 Summary: Tools for launching REFPROP calculation and retrieving results from python
 Home-page: https://www.dief.unifi.it/vp-177-serg-group-english-version.html
 Author: Pietro Ungar
 Author-email: pietro.ungar@unifi.it
 License: GNU GPLv3
-Download-URL: https://github.com/SERGGroup/REFPROPConnector/archive/refs/tags/0.3.2.tar.gz
+Download-URL: https://github.com/SERGGroup/REFPROPConnector/archive/refs/tags/0.3.3.tar.gz
 Project-URL: Source, https://github.com/SERGGroup/REFPROPConnector
 Project-URL: Tracker, https://github.com/SERGGroup/REFPROPConnector/issues
 Description: # REFPROP connector
         
         __REFPROP connector__ is a tools developed by the [SERG research group](https://www.dief.unifi.it/vp-177-serg-group-english-version.html) 
         of the [University of Florence](https://www.unifi.it/changelang-eng.html) for launching [REFPROP](https://www.nist.gov/srd/refprop) 
         calculation and retrieving results from python. 
         
         In order to use the code you must have both REFPROP and the [REFPROP wrappers for Python](https://github.com/usnistgov/REFPROP-wrappers) 
         installed and properly working.
         
         The scope of this library is to make the usage of the refprop wrappers simpler.
         
+        ### Download and installation 
+        
         The beta version can be downloaded using __PIP__:
         
         ```
         pip install REFPROP_connector
         ```
+        
+        ### First Steps
         Once the installation has been completed the user can import the tool and initialize the connector itself.
         ```python
         from REFPROPConnector import ThermodynamicPoint
         
         tp = ThermodynamicPoint(["air"], [1.])
         
         ```
@@ -41,14 +45,15 @@
             
         ```python
         from REFPROPConnector import retreive_RP_exec
         
         retreive_RP_exec()
         ```
             
+        ### Basic Usage
         
         Each _ThermodynamicPoint_ class instance represent a thermodynamic state, hence you had to provide at least 
         __two indipendent state variables__ in order to calculate the others.
         
         
         ```python
         from REFPROPConnector import ThermodynamicPoint
@@ -57,14 +62,16 @@
         
         tp.set_variable("P", 0.101325)     # P in MPa (ambient pressure)
         tp.set_variable("Q", 0.5)          # vapour quality for multiphase condition
         
         T_sat = tp.get_variable("T")       # saturation temperature in celsius (100 °C)
         ```
         
+        ### Abstract Class
+        
         _AbstractThermodynamicPoint_ is a class that can be overwritten in order to perform some calculation once both 
         independent state variable have been set. It can be useful for example for the evaluation of the reynolds number 
         for a fluid flowing in a pipe.
         
         ```python
         from REFPROPConnector import AbstractThermodynamicPoint, RefPropHandler
         import numpy as np
@@ -91,15 +98,15 @@
         if __name__ == "__main__":
         
             section = TubeSection(0.5, 1)
             
             """
             
                 The following line will return 0. as the function "other_calculation" 
-                is called only when 2 independent state variable is provided 
+                is called only when 2 independent state variables are provided 
                 
             """
             print(section.get_variable("Re"))   
             
             section.set_variable("P", 0.5)
             section.set_variable("T", 20)
             
@@ -107,34 +114,71 @@
             
                 The following line will return the actual Reynolds number
                 
             """
             print(section.get_variable("Re"))
         ```
         
+        ### Unit system and state variable list
+        
         Variable that can be calculated can be listed using _list_properties_ method from both _ThermodynamicPoint_ and 
         _AbstractThermodynamicPoint_ (the name __is not case-sensitive__). Finally, user can also select the unit system to be 
         used in the calculation, a list of possible unit system can be revived calling the method _list_unit_systems()_ 
         (current unit_system will be highlighted):  
         
         ```python
         from REFPROPConnector import ThermodynamicPoint
         
         tp = ThermodynamicPoint(["water"], [1.], unit_system="MASS BASE SI")
         tp.list_properties()
         tp.list_unit_systems()
         ```
-        Defaul unit system is __SI with C__
+        Default unit system is __SI with C__
+        
+        ### Diagram Plotter
+        The _DiagramPlotter_ class can be used to plot a specific state diagram that can be then used to describe state 
+        transformations. The diagram can be personalized using the _DiagramPlotterOptions_ class. 
+        The following is an example on how to use the class.
+        
+        
+        ```python
+        from REFPROPConnector import (
+            
+            ThermodynamicPoint, 
+            DiagramPlotter, 
+            DiagramPlotterOptions
+        
+        )
+        
+        tp = ThermodynamicPoint(["Carbon Dioxide"], [1])
+        options = DiagramPlotterOptions(
+        
+            x_variable="T",
+            x_var_range = (0, 150), x_var_log=False,
+            y_var_range = (4, 15),
+            isoline_ranges={
         
-        For other information please contact: _pietro.ungar@unifi.it_
+                "rho": (50, 1000, 25),
+                "H": (200, 550, 25)
+        
+            }
+        
+        )
+        plotter = DiagramPlotter(tp, options=options)
+        plotter.calculate()
+        
+        fig, (ax_1) = plt.subplots(1, 1, dpi=200)
+        fig.set_size_inches(10, 5)
+        plotter.plot(ax_1)
+        plt.show()
+        ```
         
         __-------------------------- !!! THIS IS A BETA VERSION !!! --------------------------__ 
         
         please report any bug or problems in the installation to _pietro.ungar@unifi.it_<br/>
-        for further information visit: https://tinyurl.com/SERG-3ETool
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `REFPROP_connector-0.3.2/REFPROP_connector.egg-info/SOURCES.txt` & `REFPROP_connector-0.3.3/REFPROP_connector.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 requirements.txt
 setup.cfg
 setup.py
 REFPROPConnector/NIST2310.EXE
 REFPROPConnector/__init__.py
 REFPROPConnector/refprop_calculator.py
+REFPROPConnector/refprop_plotter.py
 REFPROPConnectorTest/__init__.py
 REFPROPConnectorTest/test_file.py
 REFPROPConnector/Support/__init__.py
 REFPROPConnector/Support/constants.py
 REFPROPConnector/Support/refprop_names_tree.py
 REFPROPConnector/Support/resources/REFPROP_exec.dat
 REFPROPConnector/Support/resources/REFPROP_names.xml
```

### Comparing `REFPROP_connector-0.3.2/setup.py` & `REFPROP_connector-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from setuptools import setup
 from os import path, listdir
+import setuptools
 
-VERSION = "0.3.2"
+VERSION = "0.3.3"
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
 
     long_description = f.read()
 
 
@@ -35,15 +35,15 @@
             for sub_name in listdir(element_path):
 
                 input_list = append_sub_dir(path.join(element_path, sub_name), input_list, parent_name=name)
 
     return input_list
 
 
-setup(
+setuptools.setup(
 
     name='REFPROP_connector',
     version=VERSION,
     license='GNU GPLv3',
 
     author='Pietro Ungar',
     author_email='pietro.ungar@unifi.it',
@@ -63,17 +63,19 @@
     },
 
     packages=__get_packages(),
 
     install_requires=[
 
         'setuptools',
+        'matplotlib',
         'ctREFPROP',
         'requests',
         'future',
+        'tqdm',
         'sty'
 
     ],
 
     classifiers=[
 
         'Development Status :: 4 - Beta',
```

### Comparing `REFPROP_connector-0.3.2/twine_upload/pip_upload.py` & `REFPROP_connector-0.3.3/twine_upload/pip_upload.py`

 * *Files identical despite different names*

