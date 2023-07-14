# Comparing `tmp/timezoneutils-0.0.1.tar.gz` & `tmp/timezoneutils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timezoneutils-0.0.1.tar", last modified: Fri Jul 14 11:20:09 2023, max compression
+gzip compressed data, was "timezoneutils-0.1.0.tar", last modified: Fri Jul 14 11:31:00 2023, max compression
```

## Comparing `timezoneutils-0.0.1.tar` & `timezoneutils-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 gohyuhan   (501) staff       (20)        0 2023-07-14 11:20:09.790032 timezoneutils-0.0.1/
--rw-r--r--   0 gohyuhan   (501) staff       (20)     1066 2023-07-14 09:35:42.000000 timezoneutils-0.0.1/LICENSE
--rw-r--r--   0 gohyuhan   (501) staff       (20)      958 2023-07-14 11:20:09.790261 timezoneutils-0.0.1/PKG-INFO
--rw-r--r--   0 gohyuhan   (501) staff       (20)      395 2023-07-14 10:52:35.000000 timezoneutils-0.0.1/README.md
--rw-r--r--   0 gohyuhan   (501) staff       (20)      103 2023-07-14 11:04:15.000000 timezoneutils-0.0.1/pyproject.toml
--rw-r--r--   0 gohyuhan   (501) staff       (20)      934 2023-07-14 11:20:09.791242 timezoneutils-0.0.1/setup.cfg
-drwxr-xr-x   0 gohyuhan   (501) staff       (20)        0 2023-07-14 11:20:09.785906 timezoneutils-0.0.1/timezoneutils/
--rw-r--r--   0 gohyuhan   (501) staff       (20)        0 2023-07-13 16:22:35.000000 timezoneutils-0.0.1/timezoneutils/__init__.py
--rw-r--r--   0 gohyuhan   (501) staff       (20)     3337 2023-07-14 11:18:37.000000 timezoneutils-0.0.1/timezoneutils/convert.py
--rw-r--r--   0 gohyuhan   (501) staff       (20)     1605 2023-07-14 11:13:25.000000 timezoneutils-0.0.1/timezoneutils/timezone_middleware.py
--rw-r--r--   0 gohyuhan   (501) staff       (20)      661 2023-07-14 08:41:17.000000 timezoneutils-0.0.1/timezoneutils/tools.py
--rw-r--r--   0 gohyuhan   (501) staff       (20)     6290 2023-07-14 11:17:54.000000 timezoneutils-0.0.1/timezoneutils/utils.py
-drwxr-xr-x   0 gohyuhan   (501) staff       (20)        0 2023-07-14 11:20:09.789592 timezoneutils-0.0.1/timezoneutils.egg-info/
--rw-r--r--   0 gohyuhan   (501) staff       (20)      958 2023-07-14 11:20:09.000000 timezoneutils-0.0.1/timezoneutils.egg-info/PKG-INFO
--rw-r--r--   0 gohyuhan   (501) staff       (20)      360 2023-07-14 11:20:09.000000 timezoneutils-0.0.1/timezoneutils.egg-info/SOURCES.txt
--rw-r--r--   0 gohyuhan   (501) staff       (20)        1 2023-07-14 11:20:09.000000 timezoneutils-0.0.1/timezoneutils.egg-info/dependency_links.txt
--rw-r--r--   0 gohyuhan   (501) staff       (20)      284 2023-07-14 11:20:09.000000 timezoneutils-0.0.1/timezoneutils.egg-info/requires.txt
--rw-r--r--   0 gohyuhan   (501) staff       (20)       14 2023-07-14 11:20:09.000000 timezoneutils-0.0.1/timezoneutils.egg-info/top_level.txt
+drwxr-xr-x   0 gohyuhan   (501) staff       (20)        0 2023-07-14 11:31:00.475064 timezoneutils-0.1.0/
+-rw-r--r--   0 gohyuhan   (501) staff       (20)     1066 2023-07-14 09:35:42.000000 timezoneutils-0.1.0/LICENSE
+-rw-r--r--   0 gohyuhan   (501) staff       (20)     1120 2023-07-14 11:31:00.475269 timezoneutils-0.1.0/PKG-INFO
+-rw-r--r--   0 gohyuhan   (501) staff       (20)      557 2023-07-14 11:30:40.000000 timezoneutils-0.1.0/README.md
+-rw-r--r--   0 gohyuhan   (501) staff       (20)      103 2023-07-14 11:04:15.000000 timezoneutils-0.1.0/pyproject.toml
+-rw-r--r--   0 gohyuhan   (501) staff       (20)      934 2023-07-14 11:31:00.476318 timezoneutils-0.1.0/setup.cfg
+drwxr-xr-x   0 gohyuhan   (501) staff       (20)        0 2023-07-14 11:31:00.470939 timezoneutils-0.1.0/timezoneutils/
+-rw-r--r--   0 gohyuhan   (501) staff       (20)        0 2023-07-13 16:22:35.000000 timezoneutils-0.1.0/timezoneutils/__init__.py
+-rw-r--r--   0 gohyuhan   (501) staff       (20)     3337 2023-07-14 11:18:37.000000 timezoneutils-0.1.0/timezoneutils/convert.py
+-rw-r--r--   0 gohyuhan   (501) staff       (20)     1665 2023-07-14 11:27:31.000000 timezoneutils-0.1.0/timezoneutils/timezone_middleware.py
+-rw-r--r--   0 gohyuhan   (501) staff       (20)      661 2023-07-14 08:41:17.000000 timezoneutils-0.1.0/timezoneutils/tools.py
+-rw-r--r--   0 gohyuhan   (501) staff       (20)     6290 2023-07-14 11:17:54.000000 timezoneutils-0.1.0/timezoneutils/utils.py
+drwxr-xr-x   0 gohyuhan   (501) staff       (20)        0 2023-07-14 11:31:00.474607 timezoneutils-0.1.0/timezoneutils.egg-info/
+-rw-r--r--   0 gohyuhan   (501) staff       (20)     1120 2023-07-14 11:31:00.000000 timezoneutils-0.1.0/timezoneutils.egg-info/PKG-INFO
+-rw-r--r--   0 gohyuhan   (501) staff       (20)      360 2023-07-14 11:31:00.000000 timezoneutils-0.1.0/timezoneutils.egg-info/SOURCES.txt
+-rw-r--r--   0 gohyuhan   (501) staff       (20)        1 2023-07-14 11:31:00.000000 timezoneutils-0.1.0/timezoneutils.egg-info/dependency_links.txt
+-rw-r--r--   0 gohyuhan   (501) staff       (20)      284 2023-07-14 11:31:00.000000 timezoneutils-0.1.0/timezoneutils.egg-info/requires.txt
+-rw-r--r--   0 gohyuhan   (501) staff       (20)       14 2023-07-14 11:31:00.000000 timezoneutils-0.1.0/timezoneutils.egg-info/top_level.txt
```

### Comparing `timezoneutils-0.0.1/LICENSE` & `timezoneutils-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timezoneutils-0.0.1/setup.cfg` & `timezoneutils-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = timezoneutils
-version = 0.0.1
+version = 0.1.0
 author = GOH YU HAN
 author_email = gohyuhan123456@gmail.com
 description = Package For timezoneutils
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `timezoneutils-0.0.1/timezoneutils/convert.py` & `timezoneutils-0.1.0/timezoneutils/convert.py`

 * *Files identical despite different names*

### Comparing `timezoneutils-0.0.1/timezoneutils/timezone_middleware.py` & `timezoneutils-0.1.0/timezoneutils/timezone_middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,28 @@
         # the ip_address retrieved is the ip address of your network
         # your ip_address decided by your network provider
         # if vpn is used, the ip_address will be decide by vpn used
         ip_address = request.META.get('HTTP_X_FORWARDED_FOR')
         private_ip_address = request.META.get('REMOTE_ADDR')
         print("public ip address: {}".format(ip_address))
         print("private ip address: {}".format(private_ip_address))
-        g = geocoder.ip(ip_address)
+        g = None
+        if ip_address is not None:
+            g = geocoder.ip(ip_address)
 
         if g and g[0].raw:
             timezone_name = g[0].raw["timezone"]
             timezone_obj = pytz.timezone(timezone_name)
+            request.ip_info = g[0].raw
         else:
             # Default timezone if geolocation or timezone not found
             timezone_obj = pytz.timezone('UTC')
         # ip_info will be a dictionary of info regarding the ip_address provided
         # e.g., {'ip': <ip address>, 'city': <city>, 'region': <region>, 'country': <country code>, 'loc': <location coordinates e.g., (lat,lng)>,
         #  'org': <network provider>, 'postal': <post code>, 'timezone': <timezone>, 'readme': 'https://ipinfo.io/missingauth'}
-        request.ip_info = g[0].raw
         request.timezone = timezone_obj
         request.time = datetime.now().astimezone(request.timezone)
         response = self.get_response(request)
         
 
         print("{} client timezone: {}".format(ip_address,request.time))
         return response
```

### Comparing `timezoneutils-0.0.1/timezoneutils/tools.py` & `timezoneutils-0.1.0/timezoneutils/tools.py`

 * *Files identical despite different names*

### Comparing `timezoneutils-0.0.1/timezoneutils/utils.py` & `timezoneutils-0.1.0/timezoneutils/utils.py`

 * *Files identical despite different names*

