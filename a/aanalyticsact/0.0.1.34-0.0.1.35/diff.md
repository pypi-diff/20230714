# Comparing `tmp/aanalyticsact-0.0.1.34.tar.gz` & `tmp/aanalyticsact-0.0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aanalyticsact-0.0.1.34.tar", last modified: Fri Jul 14 07:12:15 2023, max compression
+gzip compressed data, was "aanalyticsact-0.0.1.35.tar", last modified: Fri Jul 14 07:51:11 2023, max compression
```

## Comparing `aanalyticsact-0.0.1.34.tar` & `aanalyticsact-0.0.1.35.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 07:12:15.571471 aanalyticsact-0.0.1.34/
--rw-rw-rw-   0        0        0     1216 2023-07-14 07:12:15.572468 aanalyticsact-0.0.1.34/PKG-INFO
--rw-rw-rw-   0        0        0      765 2022-01-17 15:45:46.000000 aanalyticsact-0.0.1.34/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 07:12:15.527168 aanalyticsact-0.0.1.34/aanalyticsact/
--rw-rw-rw-   0        0        0      118 2023-07-12 05:33:21.000000 aanalyticsact-0.0.1.34/aanalyticsact/__init__.py
--rw-rw-rw-   0        0        0       24 2023-07-14 07:11:43.000000 aanalyticsact-0.0.1.34/aanalyticsact/__version__.py
--rw-rw-rw-   0        0        0     6667 2023-07-14 06:58:21.000000 aanalyticsact-0.0.1.34/aanalyticsact/actExecute.py
--rw-rw-rw-   0        0        0    15266 2023-07-14 07:00:13.000000 aanalyticsact-0.0.1.34/aanalyticsact/actModuler.py
--rw-rw-rw-   0        0        0     8870 2023-06-01 06:30:28.000000 aanalyticsact-0.0.1.34/aanalyticsact/actRunner.py
-drwxrwxrwx   0        0        0        0 2023-07-14 07:12:15.565484 aanalyticsact-0.0.1.34/aanalyticsact.egg-info/
--rw-rw-rw-   0        0        0     1216 2023-07-14 07:12:15.000000 aanalyticsact-0.0.1.34/aanalyticsact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-07-14 07:12:15.000000 aanalyticsact-0.0.1.34/aanalyticsact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 07:12:15.000000 aanalyticsact-0.0.1.34/aanalyticsact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-14 07:12:15.000000 aanalyticsact-0.0.1.34/aanalyticsact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-14 07:12:15.579002 aanalyticsact-0.0.1.34/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-07-14 07:11:42.000000 aanalyticsact-0.0.1.34/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:51:11.326009 aanalyticsact-0.0.1.35/
+-rw-rw-rw-   0        0        0     1216 2023-07-14 07:51:11.328160 aanalyticsact-0.0.1.35/PKG-INFO
+-rw-rw-rw-   0        0        0      765 2022-01-17 15:45:46.000000 aanalyticsact-0.0.1.35/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 07:51:11.268162 aanalyticsact-0.0.1.35/aanalyticsact/
+-rw-rw-rw-   0        0        0      118 2023-07-12 05:33:21.000000 aanalyticsact-0.0.1.35/aanalyticsact/__init__.py
+-rw-rw-rw-   0        0        0       24 2023-07-14 07:47:22.000000 aanalyticsact-0.0.1.35/aanalyticsact/__version__.py
+-rw-rw-rw-   0        0        0     6727 2023-07-14 07:50:20.000000 aanalyticsact-0.0.1.35/aanalyticsact/actExecute.py
+-rw-rw-rw-   0        0        0    15471 2023-07-14 07:50:04.000000 aanalyticsact-0.0.1.35/aanalyticsact/actModuler.py
+-rw-rw-rw-   0        0        0     8870 2023-06-01 06:30:28.000000 aanalyticsact-0.0.1.35/aanalyticsact/actRunner.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:51:11.318601 aanalyticsact-0.0.1.35/aanalyticsact.egg-info/
+-rw-rw-rw-   0        0        0     1216 2023-07-14 07:51:10.000000 aanalyticsact-0.0.1.35/aanalyticsact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-07-14 07:51:11.000000 aanalyticsact-0.0.1.35/aanalyticsact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:51:10.000000 aanalyticsact-0.0.1.35/aanalyticsact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-14 07:51:10.000000 aanalyticsact-0.0.1.35/aanalyticsact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-14 07:51:11.335253 aanalyticsact-0.0.1.35/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-07-14 07:47:27.000000 aanalyticsact-0.0.1.35/setup.py
```

### Comparing `aanalyticsact-0.0.1.34/PKG-INFO` & `aanalyticsact-0.0.1.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aanalyticsact
-Version: 0.0.1.34
+Version: 0.0.1.35
 Summary: adobe analytics library for Team ACT
 Home-page: https://github.com/SunkyeongLee/aanalyticsact
 Author: Sunkyeong Lee
 Author-email: sunkyeong.lee@concentrix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aanalyticsact-0.0.1.34/README.md` & `aanalyticsact-0.0.1.35/README.md`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.1.34/aanalyticsact/actExecute.py` & `aanalyticsact-0.0.1.35/aanalyticsact/actExecute.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,28 +90,28 @@
 
             except ConnectionResetError:
                 print("Connection Error occurred, please wait for the next response")
                 continue
 
             break
 
-def retrieve_by_RS(start_date, end_date, period, jsonLocation, rsInput, tbColumn, dbTableName, epp):
+def retrieve_by_RS(start_date, end_date, period, jsonLocation, rsInput, tbColumn, dbTableName, epp, start_hour="00:00", end_hour="00:00"):
     dateCaller = dateGenerator(start_date, end_date, period)
     site_code_rs = False
     tbColumn = tbColumnGenerator(tbColumn, False, False, True, site_code_rs)
     
     startDate = dateCaller[0]
     endDate = dateCaller[1]
 
     rsList = returnRsList(epp, rsInput)
 
     for i in range(len(startDate)):
         for j in range(len(rsList)):
             try:
-                sample = refineRsIDChange(startDate[i], endDate[i], jsonLocation, rsList[j], period, tbColumn, epp)
+                sample = refineRsIDChange(startDate[i], endDate[i], jsonLocation, rsList[j], period, tbColumn, epp, start_hour, end_hour)
 
             except KeyError:
                 print("Server Error occurred, please wait for the next response")
                 continue
 
             except IndexError:
                 print("Index Error occurred, please wait for the next response")
```

### Comparing `aanalyticsact-0.0.1.34/aanalyticsact/actModuler.py` & `aanalyticsact-0.0.1.35/aanalyticsact/actModuler.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,19 +69,16 @@
         time_obj = datetime.strptime(time_obj, "%H:%M")
         time_obj += timedelta(minutes=1)
         return str('T' + str(time_obj.strftime("%H:%M"))+ ':00.000')
     
 
 def jsonDateChange(startDate, endDate, jsonFile, start_hour, end_hour):
 
-    if start_hour == "00:00" and end_hour == "00:00":
-        startDate = EndDateCalculation(startDate, endDate)[0]
-        endDate = EndDateCalculation(startDate, endDate)[1]
-    else:
-        pass
+    startDate = EndDateCalculation(startDate, endDate)[0]
+    endDate = EndDateCalculation(startDate, endDate)[1]
 
     with open(jsonFile, 'r') as bla:
         json_data = json.load(bla)
 
     globalFilterElement = json_data['globalFilters']
     if start_hour == "00:00" and end_hour == "00:00":
         tobeDate = str(startDate + "T00:00:00.000/" + endDate + "T00:00:00.000")
@@ -325,31 +322,35 @@
 
 def rsIDchange(jsonFile, rsID):
     temp_simple = deepcopy(jsonFile)
     temp_simple['rsid'] = rsID
 
     return temp_simple
 
-def refineRsIDChange(startDate, endDate, jsonFile, rsList, period, tbColumn, epp):
-    datechanged = jsonDateChange(startDate, endDate, jsonFile)
+def refineRsIDChange(startDate, endDate, jsonFile, rsList, period, tbColumn, epp, start_hour, end_hour):
+    datechanged = jsonDateChange(startDate, endDate, jsonFile, start_hour, end_hour)
     rschanged = rsIDchange(datechanged, rsList[1])
 
     dataInitiator()
     dataFrame = dataretriever_data(rschanged)
 
     columnList = []
     for i in range(dataFrame.shape[1]):
         columnList.append(i)
 
     dataFrame.columns = columnList
 
     dataFrame.insert(0, "site_code", rsList[0], True)
     dataFrame.insert(2, "period", period, True)
-    dataFrame.insert(3, "start_date", startDate, True)
-    dataFrame.insert(4, "end_date", endDate, True)
+    if start_hour == "00:00" and end_hour == "00:00":
+        dataFrame.insert(3, "start_date", startDate, True)
+        dataFrame.insert(4, "end_date", endDate, True)
+    else :
+        dataFrame.insert(3, "start_date", "{0} {1}".format(startDate, start_hour), True)
+        dataFrame.insert(4, "end_date", "{0} {1}".format(endDate, end_hour), True)
 
     if epp == True:
         dataFrame.insert(5, "is_epp", "Y", True)
     else:
         dataFrame.insert(5, "is_epp", "N", True)
 
     if (rsList[1] == "sssamsungnewus" or rsList[1] == "sssamsung4sec"):
```

### Comparing `aanalyticsact-0.0.1.34/aanalyticsact/actRunner.py` & `aanalyticsact-0.0.1.35/aanalyticsact/actRunner.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.1.34/aanalyticsact.egg-info/PKG-INFO` & `aanalyticsact-0.0.1.35/aanalyticsact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aanalyticsact
-Version: 0.0.1.34
+Version: 0.0.1.35
 Summary: adobe analytics library for Team ACT
 Home-page: https://github.com/SunkyeongLee/aanalyticsact
 Author: Sunkyeong Lee
 Author-email: sunkyeong.lee@concentrix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aanalyticsact-0.0.1.34/setup.py` & `aanalyticsact-0.0.1.35/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aanalyticsact",
-    version="0.0.1.34",
+    version="0.0.1.35",
     author="Sunkyeong Lee",
     author_email="sunkyeong.lee@concentrix.com",
     description="adobe analytics library for Team ACT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SunkyeongLee/aanalyticsact",
     packages=setuptools.find_packages(),
```

