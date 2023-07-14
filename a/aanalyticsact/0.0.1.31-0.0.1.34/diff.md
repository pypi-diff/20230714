# Comparing `tmp/aanalyticsact-0.0.1.31.tar.gz` & `tmp/aanalyticsact-0.0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aanalyticsact-0.0.1.31.tar", last modified: Tue Jun 13 02:26:05 2023, max compression
+gzip compressed data, was "aanalyticsact-0.0.1.34.tar", last modified: Fri Jul 14 07:12:15 2023, max compression
```

## Comparing `aanalyticsact-0.0.1.31.tar` & `aanalyticsact-0.0.1.34.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 02:26:05.447511 aanalyticsact-0.0.1.31/
--rw-rw-rw-   0        0        0     1216 2023-06-13 02:26:05.448400 aanalyticsact-0.0.1.31/PKG-INFO
--rw-rw-rw-   0        0        0      765 2022-01-17 15:45:46.000000 aanalyticsact-0.0.1.31/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 02:26:05.404913 aanalyticsact-0.0.1.31/aanalyticsact/
--rw-rw-rw-   0        0        0      176 2022-01-17 15:38:59.000000 aanalyticsact-0.0.1.31/aanalyticsact/__init__.py
--rw-rw-rw-   0        0        0       24 2023-06-13 02:25:01.000000 aanalyticsact-0.0.1.31/aanalyticsact/__version__.py
--rw-rw-rw-   0        0        0     6303 2022-02-16 05:16:30.000000 aanalyticsact-0.0.1.31/aanalyticsact/actCreateSeg.py
--rw-rw-rw-   0        0        0     6543 2023-05-09 08:26:00.000000 aanalyticsact-0.0.1.31/aanalyticsact/actExecute.py
--rw-rw-rw-   0        0        0    13653 2023-06-13 02:21:23.000000 aanalyticsact-0.0.1.31/aanalyticsact/actModuler.py
--rw-rw-rw-   0        0        0     8870 2023-06-01 06:30:28.000000 aanalyticsact-0.0.1.31/aanalyticsact/actRunner.py
-drwxrwxrwx   0        0        0        0 2023-06-13 02:26:05.439424 aanalyticsact-0.0.1.31/aanalyticsact.egg-info/
--rw-rw-rw-   0        0        0     1216 2023-06-13 02:26:04.000000 aanalyticsact-0.0.1.31/aanalyticsact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-06-13 02:26:05.000000 aanalyticsact-0.0.1.31/aanalyticsact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 02:26:04.000000 aanalyticsact-0.0.1.31/aanalyticsact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 02:26:04.000000 aanalyticsact-0.0.1.31/aanalyticsact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 02:26:05.454384 aanalyticsact-0.0.1.31/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-06-13 02:25:02.000000 aanalyticsact-0.0.1.31/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:12:15.571471 aanalyticsact-0.0.1.34/
+-rw-rw-rw-   0        0        0     1216 2023-07-14 07:12:15.572468 aanalyticsact-0.0.1.34/PKG-INFO
+-rw-rw-rw-   0        0        0      765 2022-01-17 15:45:46.000000 aanalyticsact-0.0.1.34/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 07:12:15.527168 aanalyticsact-0.0.1.34/aanalyticsact/
+-rw-rw-rw-   0        0        0      118 2023-07-12 05:33:21.000000 aanalyticsact-0.0.1.34/aanalyticsact/__init__.py
+-rw-rw-rw-   0        0        0       24 2023-07-14 07:11:43.000000 aanalyticsact-0.0.1.34/aanalyticsact/__version__.py
+-rw-rw-rw-   0        0        0     6667 2023-07-14 06:58:21.000000 aanalyticsact-0.0.1.34/aanalyticsact/actExecute.py
+-rw-rw-rw-   0        0        0    15266 2023-07-14 07:00:13.000000 aanalyticsact-0.0.1.34/aanalyticsact/actModuler.py
+-rw-rw-rw-   0        0        0     8870 2023-06-01 06:30:28.000000 aanalyticsact-0.0.1.34/aanalyticsact/actRunner.py
+drwxrwxrwx   0        0        0        0 2023-07-14 07:12:15.565484 aanalyticsact-0.0.1.34/aanalyticsact.egg-info/
+-rw-rw-rw-   0        0        0     1216 2023-07-14 07:12:15.000000 aanalyticsact-0.0.1.34/aanalyticsact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-07-14 07:12:15.000000 aanalyticsact-0.0.1.34/aanalyticsact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 07:12:15.000000 aanalyticsact-0.0.1.34/aanalyticsact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-14 07:12:15.000000 aanalyticsact-0.0.1.34/aanalyticsact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-14 07:12:15.579002 aanalyticsact-0.0.1.34/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-07-14 07:11:42.000000 aanalyticsact-0.0.1.34/setup.py
```

### Comparing `aanalyticsact-0.0.1.31/PKG-INFO` & `aanalyticsact-0.0.1.34/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aanalyticsact
-Version: 0.0.1.31
+Version: 0.0.1.34
 Summary: adobe analytics library for Team ACT
 Home-page: https://github.com/SunkyeongLee/aanalyticsact
 Author: Sunkyeong Lee
 Author-email: sunkyeong.lee@concentrix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aanalyticsact-0.0.1.31/README.md` & `aanalyticsact-0.0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.1.31/aanalyticsact/actExecute.py` & `aanalyticsact-0.0.1.34/aanalyticsact/actExecute.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # from actModuler import *
 # from actRunner import *
 from .actModuler import *
 from .actRunner import *
 import time
 
 
-def Retrive_FirstLevel(start_date, end_date, period, jsonLocation, tbColumn, dbTableName, epp, site_code_rs, limit):
+def retrieve_FirstLevel(start_date, end_date, period, jsonLocation, tbColumn, dbTableName, epp, site_code_rs, limit, start_hour="00:00", end_hour="00:00"):
     if limit > 1000:
         raise Error("limit은 0 ~ 1000 사이 값으로 넣어주세요")
 
     dateCaller = dateGenerator(start_date, end_date, period)
     if_site_code = checkSiteCode(readJson(jsonLocation)["dimension"])
     
     tbColumn = tbColumnGenerator(tbColumn, if_site_code, False, False, site_code_rs)
@@ -21,15 +21,15 @@
     startDate = dateCaller[0]
     endDate = dateCaller[1]
 
     for i in range(len(startDate)):
         while True:
             try:
                 start = time.time()
-                jsonToDb(startDate[i], endDate[i], period, jsonLocation, tbColumn, dbTableName, epp, if_site_code, site_code_rs, limit)
+                jsonToDb(startDate[i], endDate[i], period, jsonLocation, tbColumn, dbTableName, epp, if_site_code, site_code_rs, limit, start_hour, end_hour)
                 timeSec = round(time.time() - start, 2)
                 print("Time took: ", timeSec, "sec")
   
             except KeyError:
                 print("Server Error occurred, please wait for the next response")
                 continue
 
@@ -47,15 +47,15 @@
 
             except ConnectionResetError:
                 print("Connection Error occurred, please wait for the next response")
                 continue 
             
             break
 
-def Retrive_SecondLevel(start_date, end_date, period, jsonLocation, jsonLocation_breakdown,tbColumn, dbTableName, epp, limit):
+def retrieve_SecondLevel(start_date, end_date, period, jsonLocation, jsonLocation_breakdown,tbColumn, dbTableName, epp, limit, start_hour="00:00", end_hour="00:00"):
     dateCaller = dateGenerator(start_date, end_date, period)
     if_site_code = checkSiteCode(readJson(jsonLocation)["dimension"])
 
     if returnRsID(jsonLocation) == "sssamsungnewus":
         if_site_code = True
 
     site_code_rs = False
@@ -64,15 +64,15 @@
     startDate = dateCaller[0]
     endDate = dateCaller[1]
 
     for i in range(len(startDate)):
         while True:
             try:
                 start = time.time()
-                StackbreakValue(startDate[i], endDate[i], period, jsonLocation, jsonLocation_breakdown, tbColumn, dbTableName, epp, limit)
+                StackbreakValue(startDate[i], endDate[i], period, jsonLocation, jsonLocation_breakdown, tbColumn, dbTableName, epp, limit, start_hour, end_hour)
                 timeSec = round(time.time() - start, 2)
                 print("Time took: ", timeSec, "sec")
 
             except KeyError:
                 print("Server Error occurred, please wait for the next response")
                 continue
 
@@ -90,15 +90,15 @@
 
             except ConnectionResetError:
                 print("Connection Error occurred, please wait for the next response")
                 continue
 
             break
 
-def Retrive_by_RS(start_date, end_date, period, jsonLocation, rsInput, tbColumn, dbTableName, epp):
+def retrieve_by_RS(start_date, end_date, period, jsonLocation, rsInput, tbColumn, dbTableName, epp):
     dateCaller = dateGenerator(start_date, end_date, period)
     site_code_rs = False
     tbColumn = tbColumnGenerator(tbColumn, False, False, True, site_code_rs)
     
     startDate = dateCaller[0]
     endDate = dateCaller[1]
 
@@ -128,15 +128,15 @@
             except ConnectionResetError:
                 print("Connection Error occurred, please wait for the next response")
                 continue
 
             stackTodb(sample, dbTableName)
 
 ## 22.04.30 added
-def Retrive_by_RS_breakdown(start_date, end_date, period, jsonLocation, jsonLocation_breakdown, rsInput, tbColumn, dbTableName, epp, limit):
+def retrieve_by_RS_breakdown(start_date, end_date, period, jsonLocation, jsonLocation_breakdown, rsInput, tbColumn, dbTableName, epp, limit):
     dateCaller = dateGenerator(start_date, end_date, period)
     # site_code_rs = False
     # tbColumn = tbColumnGenerator(tbColumn, False, True, True, site_code_rs)
     tbColumn = ["rs_name", "dimension", "breakdown", "period", "start_date", "end_date", "is_epp", "is_epp_integ"]
     
     startDate = dateCaller[0]
     endDate = dateCaller[1]
```

### Comparing `aanalyticsact-0.0.1.31/aanalyticsact/actModuler.py` & `aanalyticsact-0.0.1.34/aanalyticsact/actModuler.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,24 +18,24 @@
     cid = "samsun0"
     ags = api2.Analytics(cid)
     ags.header
     rsids = ags.getReportSuites()
     print(rsids)
 
 
-# data retriving function
-def dataRetriver_data(jsonFile):
+# data retrieving function
+def dataretriever_data(jsonFile):
     cid = "samsun0"
     ags = api2.Analytics(cid)
     ags.header
     myreport = ags.getReport(jsonFile)
     return myreport['data']
 
 
-def dataRetriver_data_breakdown(jsonFile):
+def dataretriever_data_breakdown(jsonFile):
     cid = "samsun0"
     ags = api2.Analytics(cid)
     ags.header
     myreport1 = ags.getReport(jsonFile, item_id=True)
     data_report = myreport1['data']
 
     return data_report
@@ -58,45 +58,47 @@
     endDate = datetime.strptime(endDate, '%Y-%m-%d').date()
     endDate += timedelta(days=1)
     endDate = str(endDate)
 
     return startDate, endDate
 
 
-def jsonDateChange(startDate, endDate, jsonFile):
-    date = EndDateCalculation(startDate, endDate)
-    startDate = date[0]
-    endDate = date[1]
-
-    with open(jsonFile, 'r') as bla:
-        json_data = json.loads(bla.read())
+def timeChanger(time_obj, start):
+    if start == True:
+        return str('T' + time_obj + ':00.000/')
+    else:
+        time_obj = datetime.strptime(time_obj, "%H:%M")
+        time_obj += timedelta(minutes=1)
+        return str('T' + str(time_obj.strftime("%H:%M"))+ ':00.000')
+    
 
-    globalFilterElement = json_data['globalFilters']
+def jsonDateChange(startDate, endDate, jsonFile, start_hour, end_hour):
 
-    for i in range(len(globalFilterElement)):
-        jsonDate = globalFilterElement[i]
+    if start_hour == "00:00" and end_hour == "00:00":
+        startDate = EndDateCalculation(startDate, endDate)[0]
+        endDate = EndDateCalculation(startDate, endDate)[1]
+    else:
+        pass
 
-    tobeDate = str(startDate + "T00:00:00.000/" + endDate + "T00:00:00.000")
-    jsonDate['dateRange'] = tobeDate
+    with open(jsonFile, 'r') as bla:
+        json_data = json.load(bla)
 
+    globalFilterElement = json_data['globalFilters']
+    if start_hour == "00:00" and end_hour == "00:00":
+        tobeDate = str(startDate + "T00:00:00.000/" + endDate + "T00:00:00.000")
+    else :
+        tobeDate = str(startDate + timeChanger(start_hour, True) + endDate + timeChanger(end_hour, False))
+        
     for i in range(len(globalFilterElement)):
-        globalFilterElement[i] = jsonDate
+        globalFilterElement[i]['dateRange'] = tobeDate
 
     json_data['globalFilters'] = globalFilterElement
     
     return json_data
 
-def convertToList(dataSet):
-    place = []
-    for i in range(len(dataSet)):
-        place.append(dataSet[i])
-
-    return place
-
-
 def addStartEndDateColumn(startDate, endDate, rowNum):
     startDateList = []
     endDateList = []
 
     for i in range(rowNum):
         startDateList.append(startDate)
         endDateList.append(endDate)
@@ -107,18 +109,18 @@
     if (dimension == "variables/prop1" or dimension == "variables/evar1" or dimension == "variables/entryprop1"):
         return True
 
     else:
         return False
 
 # 1st Level data Caller
-def refinedFrame(startDate, endDate, period, jsonFile, epp, if_site_code, site_code_rs):
+def refinedFrame(startDate, endDate, period, jsonFile, epp, if_site_code, site_code_rs, start_hour, end_hour):
     dataInitiator()
-    dateChange = jsonDateChange(startDate, endDate, jsonFile)
-    dataFrame = dataRetriver_data(dateChange)
+    dateChange = jsonDateChange(startDate, endDate, jsonFile, start_hour, end_hour)
+    dataFrame = dataretriever_data(dateChange)
 
     if dateChange['rsid'] != "sssamsung4mstglobal":
         columnList = []
         for i in range(dataFrame.shape[1]):
             columnList.append(i)
 
         dataFrame.columns = columnList
@@ -135,36 +137,43 @@
                 dataFrame.insert(0, "site_code", rsName[-1].replace('epp', ''), True)
                 epp = "Y"
             else:
                 dataFrame.insert(0, "site_code", rsName[-1], True)
 
     if (if_site_code == True or site_code_rs == True):
         dataFrame.insert(1, "period", period, True)
-        dataFrame.insert(2, "start_date", startDate, True)
-        dataFrame.insert(3, "end_date", endDate, True)
+        if start_hour == "00:00" and end_hour == "00:00":
+            dataFrame.insert(2, "start_date", startDate, True)
+            dataFrame.insert(3, "end_date", endDate, True)
+        else :
+            dataFrame.insert(2, "start_date", "{0} {1}".format(startDate, start_hour), True)
+            dataFrame.insert(3, "end_date", "{0} {1}".format(endDate, end_hour), True)     
         dataFrame.insert(4, "is_epp", epp, True)
     else:
         if dateChange['rsid'] == "sssamsung4mstglobal":
             dataFrame.insert(0, "site_code", "MST", True)
         dataFrame.insert(2, "period", period, True)
-        dataFrame.insert(3, "start_date", startDate, True)
-        dataFrame.insert(4, "end_date", endDate, True)
+        if start_hour == "00:00" and end_hour == "00:00":
+            dataFrame.insert(3, "start_date", startDate, True)
+            dataFrame.insert(4, "end_date", endDate, True)        
+        else :
+            dataFrame.insert(3, "start_date", "{0} {1}".format(startDate, start_hour), True)
+            dataFrame.insert(4, "end_date", "{0} {1}".format(endDate, end_hour), True)
         dataFrame.insert(5, "is_epp", epp, True)
 
     return dataFrame  
 # updated 220527. smb site code added
 # updated 221202. my bday! :D smb site code added (10.31 open)
 def filterSiteCode(dataframe):
-    return dataframe.loc[dataframe['site_code'].isin(["uk", "de", "fr", "au", "in"])]
-    # return dataframe.loc[dataframe['site_code'].isin(["kw", "kw_ar", "bh", "bh_ar", "om", "om_ar", "eg_en", "jo", "jo_ar", "ma", "africa_en", "africa_fr", "africa_pt", "al", "ar", "au", "at", "az", "be", "be_fr", "br", "ba", "bd", "bg", "ca", "ca_fr", "cl", "cn", "co", "hr", "cz", "dk", "eg", "ee", "fi", "fr", "de", "gr", "hk", "hk_en", "hu", "in", "id", "iran", "ie", "il", "it", "jp", "kz_ru", "kz_kz", "sec", "lv", "levant", "levant_ar", "lt", "mk", "my", "mx", "mm", "nl", "nz", "n_africa", "no", "pk", "latin", "latin_en", "py", "pe", "ph", "pl", "pt", "ro", "ps", "ru", "sa", "sa_en", "rs", "sg", "sk", "si", "za", "es", "se", "ch", "ch_fr", "tw", "th", "tr", "ae", "ae_ar", "uk", "ua", "uy", "uz_ru", "uz_uz", "vn", "au-smb", "uk-smb", "fr-smb", "at-smb", "it-smb", "es-smb", "th-smb", "id-smb", "vn-smb", "my-smb", "se-smb", "dk-smb", "fi-smb", "no-smb", "ca-smb", "ca_fr-smb", "de-smb", "nl-smb", "be-smb", "be_fr-smb", "jo-smb", "jo_ar-smb", "ae-smb", "ae_ar-smb", "nz-smb", "ph-smb", "ru-smb", "iq_ar", "iq_ku", "lb", "qa", "qa_ar", "eg-smb", "pl-smb", "pt-smb", "sa_en-smb", "sa-smb", "sg-smb", "eg_en-smb", "mn", "ge"])]
+    return dataframe.loc[dataframe['site_code'].isin(["kw", "kw_ar", "bh", "bh_ar", "om", "om_ar", "eg_en", "jo", "jo_ar", "ma", "africa_en", "africa_fr", "africa_pt", "al", "ar", "au", "at", "az", "be", "be_fr", "br", "ba", "bd", "bg", "ca", "ca_fr", "cl", "cn", "co", "hr", "cz", "dk", "eg", "ee", "fi", "fr", "de", "gr", "hk", "hk_en", "hu", "in", "id", "iran", "ie", "il", "it", "jp", "kz_ru", "kz_kz", "sec", "lv", "levant", "levant_ar", "lt", "mk", "my", "mx", "mm", "nl", "nz", "n_africa", "no", "pk", "latin", "latin_en", "py", "pe", "ph", "pl", "pt", "ro", "ps", "ru", "sa", "sa_en", "rs", "sg", "sk", "si", "za", "es", "se", "ch", "ch_fr", "tw", "th", "tr", "ae", "ae_ar", "uk", "ua", "uy", "uz_ru", "uz_uz", "vn", "au-smb", "uk-smb", "fr-smb", "at-smb", "it-smb", "es-smb", "th-smb", "id-smb", "vn-smb", "my-smb", "se-smb", "dk-smb", "fi-smb", "no-smb", "ca-smb", "ca_fr-smb", "de-smb", "nl-smb", "be-smb", "be_fr-smb", "jo-smb", "jo_ar-smb", "ae-smb", "ae_ar-smb", "nz-smb", "ph-smb", "ru-smb", "iq_ar", "iq_ku", "lb", "qa", "qa_ar", "eg-smb", "pl-smb", "pt-smb", "sa_en-smb", "sa-smb", "sg-smb", "eg_en-smb", "mn", "ge"])]
 
 
 # updated 210907. added site_code_rs for us integration(due to the fact that us has no site code)
-def jsonToDb(startDate, endDate, period, jsonLocation, tbColumn, dbTableName, epp, if_site_code, site_code_rs, limit):
-    df = refinedFrame(startDate, endDate, period, jsonLocation, epp, if_site_code, site_code_rs)
+def jsonToDb(startDate, endDate, period, jsonLocation, tbColumn, dbTableName, epp, if_site_code, site_code_rs, limit, start_hour, end_hour):
+    df = refinedFrame(startDate, endDate, period, jsonLocation, epp, if_site_code, site_code_rs, start_hour, end_hour)
     df.columns = tbColumn
 
     if limit == 0:
         df = df
     else:
         df = df.head(limit)
 
@@ -207,21 +216,21 @@
 def readJson(jsonFile):
     with open(jsonFile, 'r') as bla:
         json_data = json.loads(bla.read())
 
     return json_data
         
 
-def returnItemID(startDate, endDate, jsonItemID):
+def returnItemID(startDate, endDate, jsonItemID, start_hour, end_hour):
     jsonFile = deepcopy(jsonItemID)
-    itemIDjson = jsonDateChange(startDate, endDate, jsonFile)
+    itemIDjson = jsonDateChange(startDate, endDate, jsonFile, start_hour, end_hour)
 
     dataInitiator()
 
-    itemIDdf = dataRetriver_data_breakdown(itemIDjson)
+    itemIDdf = dataretriever_data_breakdown(itemIDjson)
 
     columnList = list(map(str, range(itemIDdf.shape[1])))   
 
     columnList[0] = 'site_code'
     columnList[-1] = 'item_id'
 
     itemIDdf.columns = columnList
@@ -233,59 +242,63 @@
     else:
         itemIDlist = itemIDdf[['site_code', 'item_id']].values.tolist()
 
     return itemIDlist
 
 
 # Save as dictionary format return in tuple
-def ReturnJsonchanged(startDate, endDate, jsonFile, jsonFilebreakdown):
-    itemIDList = returnItemID(startDate, endDate, jsonFile)
+def ReturnJsonchanged(startDate, endDate, jsonFile, jsonFilebreakdown, start_hour, end_hour):
+    itemIDList = returnItemID(startDate, endDate, jsonFile, start_hour, end_hour)
 
     itemIDdict = {}
     for i in range(len(itemIDList)):
-        jsonbreakdown = jsonDateChange(startDate, endDate, jsonFilebreakdown)
-        itemIDdict[itemIDList[i][0]] = ChangeItemID(itemIDList[i][1], jsonbreakdown)
+        jsonbreakdown = jsonDateChange(startDate, endDate, jsonFilebreakdown, start_hour, end_hour)
+        itemIDdict[itemIDList[i][0]] = ChangeItemID(itemIDList[i][1], jsonbreakdown, start_hour, end_hour)
     
     itemIDdict = list(zip(itemIDdict.keys(), itemIDdict.values()))
     
     return itemIDdict
 
-def StackbreakValue(startDate, endDate, period, jsonFile, jsonFilebreakdown, tbColumn, dbTableName, epp, limit):
+def StackbreakValue(startDate, endDate, period, jsonFile, jsonFilebreakdown, tbColumn, dbTableName, epp, limit, start_hour, end_hour):
     if returnRsID(jsonFile) == "sssamsung4mstglobal":
-        itemIDdict = ReturnJsonchanged(startDate, endDate, jsonFile, jsonFilebreakdown)
+        itemIDdict = ReturnJsonchanged(startDate, endDate, jsonFile, jsonFilebreakdown, start_hour, end_hour)
 
         # iterable = list(map(int, range(len(itemIDdict))))
 
         # pool = multiprocessing.Pool(4)
         # func = partial(mstbreakDown, itemIDdict, startDate, endDate, period, tbColumn, dbTableName, epp, limit)
         # pool.map(func, iterable)
         # pool.close()
         # pool.join()
 
         for i in range(len(itemIDdict)):
-            dataFrame = dataRetriver_data(itemIDdict[i][1])
+            dataFrame = dataretriever_data(itemIDdict[i][1])
 
             if limit == 0:
                 dataFrame2 = dataFrame
             else:
                 dataFrame2 = dataFrame.head(limit)
 
             dataFrame2.insert(0, "site_code", itemIDdict[i][0], True)
             dataFrame2.insert(2, "period", period, True)
-            dataFrame2.insert(3, "start_date", startDate, True)
-            dataFrame2.insert(4, "end_date", endDate, True)
+            if start_hour == "00:00" and end_hour == "00:00":
+                dataFrame.insert(3, "start_date", startDate, True)
+                dataFrame.insert(4, "end_date", endDate, True)
+            else :
+                dataFrame.insert(3, "start_date", "{0} {1}".format(startDate, start_hour), True)
+                dataFrame.insert(4, "end_date", "{0} {1}".format(endDate, end_hour), True)
             dataFrame2.insert(5, "is_us_epp", epp, True)
 
             dataFrame2.columns = tbColumn
             stackTodb(dataFrame2, dbTableName)
 
     else:
         dataInitiator()
         dateChange = jsonDateChange(startDate, endDate, jsonFile)
-        dataFrame = dataRetriver_data(dateChange)
+        dataFrame = dataretriever_data(dateChange)
 
         dataFrame.columns = list(map(int, range(dataFrame.shape[1])))
         
         if limit == 0:
             dataFrame2 = dataFrame
         else:
             dataFrame2 = dataFrame.head(limit)
@@ -293,16 +306,20 @@
         if returnRsID(jsonFile) == "sssamsungnewus":
             dataFrame2.insert(0, "site_code", "us", True)
         else:
             rsName = dateChange['rsid'].split('4')
             dataFrame2.insert(0, "site_code", rsName[-1], True)   
 
         dataFrame2.insert(2, "period", period, True)
-        dataFrame2.insert(3, "start_date", startDate, True)
-        dataFrame2.insert(4, "end_date", endDate, True)
+        if start_hour == "00:00" and end_hour == "00:00":
+            dataFrame.insert(3, "start_date", startDate, True)
+            dataFrame.insert(4, "end_date", endDate, True)
+        else :
+            dataFrame.insert(3, "start_date", "{0} {1}".format(startDate, start_hour), True)
+            dataFrame.insert(4, "end_date", "{0} {1}".format(endDate, end_hour), True)
         dataFrame2.insert(5, "is_us_epp", epp, True)
 
         dataFrame2.columns = tbColumn
         stackTodb(dataFrame2, dbTableName)
 
 """Return after RS Name changed"""
 
@@ -313,16 +330,15 @@
     return temp_simple
 
 def refineRsIDChange(startDate, endDate, jsonFile, rsList, period, tbColumn, epp):
     datechanged = jsonDateChange(startDate, endDate, jsonFile)
     rschanged = rsIDchange(datechanged, rsList[1])
 
     dataInitiator()
-    dataFrame = dataRetriver_data(rschanged)
-
+    dataFrame = dataretriever_data(rschanged)
 
     columnList = []
     for i in range(dataFrame.shape[1]):
         columnList.append(i)
 
     dataFrame.columns = columnList
 
@@ -350,15 +366,15 @@
     datechanged = jsonDateChange(startDate, endDate, jsonFile)
     datechanged_breakdown = jsonDateChange(startDate, endDate, jsonFile_breakdown)
     rschanged_jsonFile = rsIDchange(datechanged, rsList[1])
     rschanged_jsonFile_breakdown = rsIDchange(datechanged_breakdown, rsList[1])
 
     itemIDdict = ReturnJsonchanged(startDate, endDate, rschanged_jsonFile, rschanged_jsonFile_breakdown)
     for i in range(len(itemIDdict)):
-        dataFrame = dataRetriver_data(itemIDdict[i][1])
+        dataFrame = dataretriever_data(itemIDdict[i][1])
 
         # limit 추가 시 넣기
         if limit == 0:
             dataFrame = dataFrame
         else:
             dataFrame = dataFrame.head(limit)
```

### Comparing `aanalyticsact-0.0.1.31/aanalyticsact/actRunner.py` & `aanalyticsact-0.0.1.34/aanalyticsact/actRunner.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.1.31/aanalyticsact.egg-info/PKG-INFO` & `aanalyticsact-0.0.1.34/aanalyticsact.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aanalyticsact
-Version: 0.0.1.31
+Version: 0.0.1.34
 Summary: adobe analytics library for Team ACT
 Home-page: https://github.com/SunkyeongLee/aanalyticsact
 Author: Sunkyeong Lee
 Author-email: sunkyeong.lee@concentrix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aanalyticsact-0.0.1.31/setup.py` & `aanalyticsact-0.0.1.34/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aanalyticsact",
-    version="0.0.1.31",
+    version="0.0.1.34",
     author="Sunkyeong Lee",
     author_email="sunkyeong.lee@concentrix.com",
     description="adobe analytics library for Team ACT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SunkyeongLee/aanalyticsact",
     packages=setuptools.find_packages(),
```

