# Comparing `tmp/SpaceShare-0.1.tar.gz` & `tmp/SpaceShare-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpaceShare-0.1.tar", last modified: Thu Jul 13 19:49:19 2023, max compression
+gzip compressed data, was "SpaceShare-0.1.1.tar", last modified: Fri Jul 14 02:40:24 2023, max compression
```

## Comparing `SpaceShare-0.1.tar` & `SpaceShare-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 anne       (501) staff       (20)        0 2023-07-13 19:49:19.104572 SpaceShare-0.1/
--rw-r--r--   0 anne       (501) staff       (20)    35149 2023-07-11 21:35:39.000000 SpaceShare-0.1/LICENSE
--rw-r--r--   0 anne       (501) staff       (20)      241 2023-07-13 19:49:19.104201 SpaceShare-0.1/PKG-INFO
--rw-r--r--   0 anne       (501) staff       (20)       59 2023-07-13 19:46:56.000000 SpaceShare-0.1/README.md
-drwxr-xr-x   0 anne       (501) staff       (20)        0 2023-07-13 19:49:19.100568 SpaceShare-0.1/SpaceShare/
--rw-r--r--   0 anne       (501) staff       (20)       20 2023-07-13 19:46:56.000000 SpaceShare-0.1/SpaceShare/__init__.py
--rw-r--r--   0 anne       (501) staff       (20)     3338 2023-07-13 19:46:56.000000 SpaceShare-0.1/SpaceShare/optimize_rideshares.py
--rw-r--r--   0 anne       (501) staff       (20)     1644 2023-07-13 19:46:56.000000 SpaceShare-0.1/SpaceShare/reader.py
--rw-r--r--   0 anne       (501) staff       (20)     2026 2023-07-13 19:46:56.000000 SpaceShare-0.1/SpaceShare/run.py
--rw-r--r--   0 anne       (501) staff       (20)     8859 2023-07-13 19:46:56.000000 SpaceShare-0.1/SpaceShare/write_email.py
-drwxr-xr-x   0 anne       (501) staff       (20)        0 2023-07-13 19:49:19.103571 SpaceShare-0.1/SpaceShare.egg-info/
--rw-r--r--   0 anne       (501) staff       (20)      241 2023-07-13 19:49:18.000000 SpaceShare-0.1/SpaceShare.egg-info/PKG-INFO
--rw-r--r--   0 anne       (501) staff       (20)      317 2023-07-13 19:49:19.000000 SpaceShare-0.1/SpaceShare.egg-info/SOURCES.txt
--rw-r--r--   0 anne       (501) staff       (20)        1 2023-07-13 19:49:18.000000 SpaceShare-0.1/SpaceShare.egg-info/dependency_links.txt
--rw-r--r--   0 anne       (501) staff       (20)       41 2023-07-13 19:49:18.000000 SpaceShare-0.1/SpaceShare.egg-info/requires.txt
--rw-r--r--   0 anne       (501) staff       (20)       11 2023-07-13 19:49:18.000000 SpaceShare-0.1/SpaceShare.egg-info/top_level.txt
--rw-r--r--   0 anne       (501) staff       (20)       38 2023-07-13 19:49:19.104668 SpaceShare-0.1/setup.cfg
--rw-r--r--   0 anne       (501) staff       (20)      752 2023-07-13 19:46:56.000000 SpaceShare-0.1/setup.py
+drwxr-xr-x   0 anne       (501) staff       (20)        0 2023-07-14 02:40:24.792250 SpaceShare-0.1.1/
+-rw-r--r--   0 anne       (501) staff       (20)    35149 2023-07-11 21:35:39.000000 SpaceShare-0.1.1/LICENSE
+-rw-r--r--   0 anne       (501) staff       (20)      324 2023-07-14 02:40:24.791876 SpaceShare-0.1.1/PKG-INFO
+-rw-r--r--   0 anne       (501) staff       (20)      141 2023-07-14 02:25:22.000000 SpaceShare-0.1.1/README.md
+drwxr-xr-x   0 anne       (501) staff       (20)        0 2023-07-14 02:40:24.760663 SpaceShare-0.1.1/SpaceShare/
+-rw-r--r--   0 anne       (501) staff       (20)       64 2023-07-14 02:39:26.000000 SpaceShare-0.1.1/SpaceShare/__init__.py
+-rw-r--r--   0 anne       (501) staff       (20)     3271 2023-07-14 02:25:22.000000 SpaceShare-0.1.1/SpaceShare/optimize_rideshares.py
+-rw-r--r--   0 anne       (501) staff       (20)     1845 2023-07-14 02:25:22.000000 SpaceShare-0.1.1/SpaceShare/reader.py
+-rw-r--r--   0 anne       (501) staff       (20)     2169 2023-07-14 02:25:22.000000 SpaceShare-0.1.1/SpaceShare/run.py
+-rw-r--r--   0 anne       (501) staff       (20)     9087 2023-07-14 02:25:22.000000 SpaceShare-0.1.1/SpaceShare/write_email.py
+drwxr-xr-x   0 anne       (501) staff       (20)        0 2023-07-14 02:40:24.764032 SpaceShare-0.1.1/SpaceShare.egg-info/
+-rw-r--r--   0 anne       (501) staff       (20)      324 2023-07-14 02:40:24.000000 SpaceShare-0.1.1/SpaceShare.egg-info/PKG-INFO
+-rw-r--r--   0 anne       (501) staff       (20)      414 2023-07-14 02:40:24.000000 SpaceShare-0.1.1/SpaceShare.egg-info/SOURCES.txt
+-rw-r--r--   0 anne       (501) staff       (20)        1 2023-07-14 02:40:24.000000 SpaceShare-0.1.1/SpaceShare.egg-info/dependency_links.txt
+-rw-r--r--   0 anne       (501) staff       (20)       32 2023-07-14 02:40:24.000000 SpaceShare-0.1.1/SpaceShare.egg-info/requires.txt
+-rw-r--r--   0 anne       (501) staff       (20)       11 2023-07-14 02:40:24.000000 SpaceShare-0.1.1/SpaceShare.egg-info/top_level.txt
+-rw-r--r--   0 anne       (501) staff       (20)       38 2023-07-14 02:40:24.792351 SpaceShare-0.1.1/setup.cfg
+-rw-r--r--   0 anne       (501) staff       (20)      752 2023-07-14 02:32:08.000000 SpaceShare-0.1.1/setup.py
+drwxr-xr-x   0 anne       (501) staff       (20)        0 2023-07-14 02:40:24.791272 SpaceShare-0.1.1/tests/
+-rw-r--r--   0 anne       (501) staff       (20)     1310 2023-07-14 02:25:22.000000 SpaceShare-0.1.1/tests/test_optimize_reqs.py
+-rw-r--r--   0 anne       (501) staff       (20)      624 2023-07-14 02:25:22.000000 SpaceShare-0.1.1/tests/test_reader.py
+-rw-r--r--   0 anne       (501) staff       (20)       92 2023-07-14 02:25:22.000000 SpaceShare-0.1.1/tests/test_run.py
+-rw-r--r--   0 anne       (501) staff       (20)      958 2023-07-14 02:25:22.000000 SpaceShare-0.1.1/tests/test_time_conversion.py
```

### Comparing `SpaceShare-0.1/LICENSE` & `SpaceShare-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SpaceShare-0.1/SpaceShare/optimize_rideshares.py` & `SpaceShare-0.1.1/SpaceShare/optimize_rideshares.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from scipy.cluster.hierarchy import linkage, fcluster
-from datetime import timedelta
+
 
 def get_time_of_year(time):
     """
     Calculates the time as a float in hours, given a datetime object.
 
     Args:
         time (datetime): The datetime object to be converted.
@@ -18,15 +18,15 @@
         representation, it's a representation of time in hours converted to 
         an approximate month scale.
 
     Raises:
         AttributeError: If the input datetime object doesn't have day, hour, minute, 
         and second attributes.
     """
-    return timedelta(days=time.day, hours=time.hour, minutes=time.minute, seconds=time.second).total_seconds()/3600
+    return time.day_of_year*24 + time.hour + time.minute/60 + time.second/3600
 
 
 def optimize(df, kind="arrival", max_time_difference = 0.5, max_people_per_car = 3): 
     """ 
     Optimizes shared rides for participants based on airport arrival or departures times using a hierarchical clustering algorithm. 
 
     Args:
```

### Comparing `SpaceShare-0.1/SpaceShare/reader.py` & `SpaceShare-0.1.1/SpaceShare/reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import pandas as pd
-from datetime import datetime
 
 
-
-
-def read_google_sheet(sheet_id = None):
+def read_google_sheet(sheet_id):
     """
     Reads in a Google Sheet as a CSV file using pandas. 
     Ensure that the sharing setting for the sheet allows anyone with the link to access it.
 
     Args:
         sheet_id (str, optional): The ID of the Google Sheet, extracted from the webpage as '/d/{sheet_id}/gviz/tq?tqx=out:csv'. 
             If None, it uses a default ID. Defaults to None.
@@ -22,18 +19,29 @@
         pandas.errors.ParserError: If parsing the CSV file fails.
         urllib.error.HTTPError: If the sheet ID is invalid, or the sheet doesn't allow public access.
 
     Note:
         The default sheet ID used when none is provided is '1riOck-CL8RjVkt_dgcgWhd0DWhUWMifpyb6VLngTrHs'.
     """
     prefix = "https://docs.google.com/spreadsheets/d/"
-    if sheet_id is None: sheet_id = "1riOck-CL8RjVkt_dgcgWhd0DWhUWMifpyb6VLngTrHs"
     
     DF = pd.read_csv(prefix+ sheet_id+ "/gviz/tq?tqx=out:csv")
+    return clean_dataframe(DF)
+
+def clean_dataframe(DF):
+    """
+    Cleans the input DataFrame by dropping the 'Timestamp' column and converting the 'date_time_of_airport_arrival'
+    and 'date_time_of_hotel_departure' columns from strings to datetime objects.
+
+    Args:
+        DF (pandas.DataFrame): The DataFrame to clean.
+
+    Returns:
+        pandas.DataFrame: The cleaned DataFrame.
+    """
     DF = DF.drop(columns= "Timestamp")
 
     #convert day-time string into date_time object
-    format_string = "%m/%d/%Y %H:%M:%S"
-    DF["date_time_of_airport_arrival"]  = [datetime.strptime(tt, format_string) for tt in DF["date_time_of_airport_arrival"] ]
-    DF["date_time_of_hotel_departure"]  = [datetime.strptime(tt, format_string) for tt in DF["date_time_of_hotel_departure"] ]
+    DF["date_time_of_airport_arrival"]  = [pd.to_datetime(tt) for tt in DF["date_time_of_airport_arrival"] ]
+    DF["date_time_of_hotel_departure"]  = [pd.to_datetime(tt) for tt in DF["date_time_of_hotel_departure"] ]
 
     return DF
```

### Comparing `SpaceShare-0.1/SpaceShare/run.py` & `SpaceShare-0.1.1/SpaceShare/run.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
-from reader import read_google_sheet
-from optimize_rideshares import optimize
-from write_email import send_emails
+from .reader import read_google_sheet
+from .optimize_rideshares import optimize
+from .write_email import send_emails
 import pandas as pd
 import configparser
 
 # Read the config file
 config = configparser.ConfigParser()
 
-def run(config_file = "default.cfg"):
+def run_spaceshare(config_file = "default.cfg", dry_run = False):
     """
     Main function that uses the configuration file to read a google sheet, optimize ride share groups,
     and then send emails to the participants.
 
     Parameters
     ----------
     config_file : str, optional
@@ -23,27 +23,29 @@
     email_username = config["EMAIL"]["username"].replace(" ","")
     email_password = config.get("EMAIL","password",fallback=None)
     if email_password is not None:
         email_password = email_password.replace(" ","")
     email_smtp_domain = config["EMAIL"]["smtp_domain"].replace(" ","")
     email_smtp_port = int(config["EMAIL"]["smtp_port"])
 
-    google_sheet_id = config["GOOGLE_SHEET"]["sheet_id"].replace(" ","")
+    google_sheet_id = config["GOOGLE.SHEET"]["sheet_id"].replace(" ","")
 
     max_waittime = float(config["OPTIMIZATION"]["max_wait_time"])
     max_people_per_car = int(config["OPTIMIZATION"]["max_people_per_car"])
     
 
 
     df = read_google_sheet(sheet_id=google_sheet_id)
     for kind in ["arrival","departure"]:
-        df = optimize(df,kind=kind,max_waittime=max_waittime,max_people_per_car=max_people_per_car)
+        df = optimize(df,kind=kind,max_time_difference=max_waittime,max_people_per_car=max_people_per_car)
+    df.sort_values(by=["arrival_group","departure_group"],inplace=True)
     df.to_csv("optimized_clustering.csv")
     user_input = "n"
     while user_input.lower() not in ["y","yes"]:
         user_input = input("The groups have been assigned. Please take a moment to inspect the results in optimized_clustering.csv \n"\
                             +"If you want, you can manually make changes to the document. \n"\
                             +"Do you want to send the emails? (y/n)")
 
     df = pd.read_csv("optimized_clustering.csv")
     send_emails(df, email_username=email_username,email_smtp_domain=email_smtp_domain,
-                email_password=email_password,email_smtp_port=email_smtp_port)
+                email_password=email_password,email_smtp_port=email_smtp_port,
+                dry_run=dry_run)
```

### Comparing `SpaceShare-0.1/SpaceShare/write_email.py` & `SpaceShare-0.1.1/SpaceShare/write_email.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # We import necessary libraries 
 from getpass import getpass
 import smtplib
 from email.message import EmailMessage
 import numpy as np
+import pandas as pd
 
 # This class handles the process of sending emails
 class EmailHandler():
     """A class to handle email operations including sending emails and reading email content from a file."""
     def __init__(self, email_username, email_domain="smtp.gmail.com", port=587, password=None, verbose=False):
         """
         Initializes the EmailHandler class.
@@ -153,15 +154,19 @@
         
             address = ""
             for name in first_names:
                 address += name+", "
             
             deptimes = ""
             for x in range(len(first_names)):
-                deptimes += "\t"+names[x]+": "+arrival_times[x]+", contact number: "+phone_numbers[x]+"\n "
+                deptimes += "\t"+names[x]+": "+pd.to_datetime(arrival_times[x]).strftime("%b %d, %I:%M %p")
+                # if not phone_numbers[x]=="NaN":
+                #     deptimes +=", contact number: "+phone_numbers[x]
+                # TODO: to implement in later release
+                deptimes +="\n "
             message = f"""
 Dear {address}
 
 {helperstr[kind]}:\n{deptimes}
 Please contact each other and organize a ride together. If you have any questions, please contact us.
 
 Best regards,
```

### Comparing `SpaceShare-0.1/setup.py` & `SpaceShare-0.1.1/setup.py`

 * *Files identical despite different names*

