# Comparing `tmp/pysdbots-0.1.1.tar.gz` & `tmp/pysdbots-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysdbots-0.1.1.tar", last modified: Sat Aug 27 10:53:47 2022, max compression
+gzip compressed data, was "pysdbots-2.0.tar", last modified: Fri Jul 14 21:33:13 2023, max compression
```

## Comparing `pysdbots-0.1.1.tar` & `pysdbots-2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-08-27 10:53:47.403654 pysdbots-0.1.1/
--rw-rw-rw-   0        0        0     1093 2022-07-13 13:01:52.000000 pysdbots-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2307 2022-08-27 10:53:47.237656 pysdbots-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1155 2022-08-27 10:43:55.000000 pysdbots-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-08-27 10:53:46.334656 pysdbots-0.1.1/pysdbots/
--rw-rw-rw-   0        0        0      263 2022-08-27 10:52:46.000000 pysdbots-0.1.1/pysdbots/__init__.py
--rw-rw-rw-   0        0        0     1553 2022-08-27 03:45:51.000000 pysdbots-0.1.1/pysdbots/pysdbots.py
-drwxrwxrwx   0        0        0        0 2022-08-27 10:53:47.234656 pysdbots-0.1.1/pysdbots.egg-info/
--rw-rw-rw-   0        0        0     2307 2022-08-27 10:53:45.000000 pysdbots-0.1.1/pysdbots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2022-08-27 10:53:45.000000 pysdbots-0.1.1/pysdbots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-27 10:53:45.000000 pysdbots-0.1.1/pysdbots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-08-27 10:53:45.000000 pysdbots-0.1.1/pysdbots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-27 10:53:45.000000 pysdbots-0.1.1/pysdbots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-27 10:53:47.403654 pysdbots-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1483 2022-08-27 10:50:26.000000 pysdbots-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 21:33:13.669564 pysdbots-2.0/
+-rw-rw-rw-   0        0        0     1093 2022-08-26 22:30:10.000000 pysdbots-2.0/LICENSE
+-rw-rw-rw-   0        0        0     2313 2023-07-14 21:33:13.663005 pysdbots-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1161 2023-07-14 21:25:18.000000 pysdbots-2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 21:33:13.547073 pysdbots-2.0/pysdbots/
+-rw-rw-rw-   0        0        0      263 2022-08-26 22:30:10.000000 pysdbots-2.0/pysdbots/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-07-14 21:27:21.000000 pysdbots-2.0/pysdbots/pysdbots.py
+drwxrwxrwx   0        0        0        0 2023-07-14 21:33:13.652471 pysdbots-2.0/pysdbots.egg-info/
+-rw-rw-rw-   0        0        0     2313 2023-07-14 21:33:13.000000 pysdbots-2.0/pysdbots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-07-14 21:33:13.000000 pysdbots-2.0/pysdbots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 21:33:13.000000 pysdbots-2.0/pysdbots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-14 21:33:13.000000 pysdbots-2.0/pysdbots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-14 21:33:13.000000 pysdbots-2.0/pysdbots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 21:33:13.670553 pysdbots-2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1483 2023-07-14 21:22:03.000000 pysdbots-2.0/setup.py
```

### Comparing `pysdbots-0.1.1/LICENSE` & `pysdbots-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysdbots-0.1.1/PKG-INFO` & `pysdbots-2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pysdbots
-Version: 0.1.1
+Version: 2.0
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/damantha126/pysdbots
 Author: DamanthaJasinghe
 Author-email: damanthaja@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/damantha126/pysdbots/issues
 Project-URL: Community, https://t.me/SDBOTs_inifinity
 Project-URL: Source, https://github.com/damantha126/pysdbots
-Project-URL: Documentation, https://docs.sdbots.tk
+Project-URL: Documentation, https://docs.sdbots.tech
 Keywords: sdbots,python-pakage,sd-api,api,damanthaja,mritzme,damantha126
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -22,24 +22,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <a href="https://t.me/SDBOTs_inifinity">
-        <img src="https://telegra.ph/file/9ea8fd64fa13fe8759877.jpg" alt="Pyrogram" width="500">
+        <img src="https://telegra.ph/file/835058034ef2f776b475e.jpg" alt="Pyrogram" width="500">
     </a>
     <br>
     <b>A Project Made To Centralize Various APIs 📖 No Authorization Needed :)</b>
     <br>
-    <a href="https://sdbots.tk">
+    <a href="https://sdbots.tech">
         Homepage
     </a>
     •
-    <a href="https://docs.sdbots.tk">
+    <a href="https://docs.sdbots.tech">
         Documentation
     </a>
     •
     <a href="https://t.me/SDBOTs_inifinity">
         Channel
     </a>
 </p>
@@ -67,9 +67,9 @@
 
 ``` bash
 pip3 install pysdbots
 ```
 
 ### API Url
 ```
-https://api.sdbots.tk
+https://api.sdbots.tech
 ```
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: pysdbots Version: 0.1.1 Summary: A Project Made To
+Metadata-Version: 2.1 Name: pysdbots Version: 2.0 Summary: A Project Made To
 Centralize Various APIs ð No Authorization Needed :) Home-page: https://
 github.com/damantha126/pysdbots Author: DamanthaJasinghe Author-email:
 damanthaja@gmail.com License: MIT Project-URL: Tracker, https://github.com/
 damantha126/pysdbots/issues Project-URL: Community, https://t.me/
 SDBOTs_inifinity Project-URL: Source, https://github.com/damantha126/pysdbots
-Project-URL: Documentation, https://docs.sdbots.tk Keywords: sdbots,python-
+Project-URL: Documentation, https://docs.sdbots.tech Keywords: sdbots,python-
 pakage,sd-api,api,damanthaja,mritzme,damantha126 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -26,8 +26,8 @@
 â¤ User Friendly
 â¤ JSON Response
 â¤ Easy To Use
 â¤ WEB Based API
 â¤ For All Platform
  ## â¢ Installations ### Install the library The best way to interact with our
 API is to use one of our official libraries ``` bash pip3 install pysdbots ```
-### API Url ``` https://api.sdbots.tk ```
+### API Url ``` https://api.sdbots.tech ```
```

### Comparing `pysdbots-0.1.1/README.md` & `pysdbots-2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <p align="center">
     <a href="https://t.me/SDBOTs_inifinity">
-        <img src="https://telegra.ph/file/9ea8fd64fa13fe8759877.jpg" alt="Pyrogram" width="500">
+        <img src="https://telegra.ph/file/835058034ef2f776b475e.jpg" alt="Pyrogram" width="500">
     </a>
     <br>
     <b>A Project Made To Centralize Various APIs 📖 No Authorization Needed :)</b>
     <br>
-    <a href="https://sdbots.tk">
+    <a href="https://sdbots.tech">
         Homepage
     </a>
     •
-    <a href="https://docs.sdbots.tk">
+    <a href="https://docs.sdbots.tech">
         Documentation
     </a>
     •
     <a href="https://t.me/SDBOTs_inifinity">
         Channel
     </a>
 </p>
@@ -41,9 +41,9 @@
 
 ``` bash
 pip3 install pysdbots
 ```
 
 ### API Url
 ```
-https://api.sdbots.tk
+https://api.sdbots.tech
 ```
```

#### html2text {}

```diff
@@ -11,8 +11,8 @@
 â¤ User Friendly
 â¤ JSON Response
 â¤ Easy To Use
 â¤ WEB Based API
 â¤ For All Platform
  ## â¢ Installations ### Install the library The best way to interact with our
 API is to use one of our official libraries ``` bash pip3 install pysdbots ```
-### API Url ``` https://api.sdbots.tk ```
+### API Url ``` https://api.sdbots.tech ```
```

### Comparing `pysdbots-0.1.1/pysdbots/pysdbots.py` & `pysdbots-2.0/pysdbots/pysdbots.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 import requests
 
 
 headers={'Content-Type': 'application/json'}
 
 
 def anime_logo(name):
-    API = f"https://api.sdbots.tk/anime-logo?name={name}"
+    API = f"https://api.sdbots.tech/anime-logo?name={name}"
     req = requests.get(API).url
     return(req)
 
 def tiktok(url):
-    API = f"https://api.sdbots.tk/tiktok?url={url}"
+    API = f"https://api.sdbots.tech/tiktok?url={url}"
     req = requests.get(API).json()
     return(req)
 
 def apod():
-    API = "https://api.sdbots.tk/apod"
+    API = "https://api.sdbots.tech/apod"
     req = requests.get(API).json()
     return(req)
 
 def detect_lang(text):
-    req = requests.get(f"https://api.sdbots.tk/detect?text={text}").json()
+    req = requests.get(f"https://api.sdbots.tech/detect?text={text}").json()
     return(req)
 
 def write(text):
     body = {
         "text": f"{text}"
     }
-    url = "https://api.sdbots.tk/write"
+    url = "https://api.sdbots.tech/write"
     req = requests.post(url=url, headers=headers, json=body).url
     return(req)
 
 def chk(cc):
-    API = f"https://api.sdbots.tk/chk?cc={cc}"
+    API = f"https://api.sdbots.tech/chk?cc={cc}"
     req = requests.get(API).json()
     return(req)
 
 def sk_checker(key):
-    req = requests.get(f"https://api.sdbots.tk/sk?key={key}").json()
+    req = requests.get(f"https://api.sdbots.tech/sk?key={key}").json()
     return(req)
 
 def lyrics(song):
-    req = requests.get(f"https://api.sdbots.tk/lyrics?song={song}").json()
+    req = requests.get(f"https://api.sdbots.tech/lyrics?song={song}").json()
     return(req)
 
 def ipinfo(ip):
-    req = requests.get(f"https://api.sdbots.tk/ipinfo?ip={ip}").json()
+    req = requests.get(f"https://api.sdbots.tech/ipinfo?ip={ip}").json()
     return(req)
 
 def hirunews():
-    req = requests.get("https://api.sdbots.tk/hirunews").json()
+    req = requests.get("https://api.sdbots.tech/hirunews").json()
     return(req)
 
 def logohq(text):
-    req = requests.get(f"https://api.sdbots.tk/logohq?text={text}").url
+    req = requests.get(f"https://api.sdbots.tech/logohq?text={text}").url
     return(req)
 
 def fakeinfo():
-    req = requests.get("https://api.sdbots.tk/fakeinfo").json()
+    req = requests.get("https://api.sdbots.tech/fakeinfo").json()
     return(req)
 
 
-a = anime_logo("DamanthaJa")
-print(a)
+print("SD Bots API -> https://docs.sdbots.tech")
```

### Comparing `pysdbots-0.1.1/pysdbots.egg-info/PKG-INFO` & `pysdbots-2.0/pysdbots.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pysdbots
-Version: 0.1.1
+Version: 2.0
 Summary: A Project Made To Centralize Various APIs 📖 No Authorization Needed :)
 Home-page: https://github.com/damantha126/pysdbots
 Author: DamanthaJasinghe
 Author-email: damanthaja@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/damantha126/pysdbots/issues
 Project-URL: Community, https://t.me/SDBOTs_inifinity
 Project-URL: Source, https://github.com/damantha126/pysdbots
-Project-URL: Documentation, https://docs.sdbots.tk
+Project-URL: Documentation, https://docs.sdbots.tech
 Keywords: sdbots,python-pakage,sd-api,api,damanthaja,mritzme,damantha126
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -22,24 +22,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <a href="https://t.me/SDBOTs_inifinity">
-        <img src="https://telegra.ph/file/9ea8fd64fa13fe8759877.jpg" alt="Pyrogram" width="500">
+        <img src="https://telegra.ph/file/835058034ef2f776b475e.jpg" alt="Pyrogram" width="500">
     </a>
     <br>
     <b>A Project Made To Centralize Various APIs 📖 No Authorization Needed :)</b>
     <br>
-    <a href="https://sdbots.tk">
+    <a href="https://sdbots.tech">
         Homepage
     </a>
     •
-    <a href="https://docs.sdbots.tk">
+    <a href="https://docs.sdbots.tech">
         Documentation
     </a>
     •
     <a href="https://t.me/SDBOTs_inifinity">
         Channel
     </a>
 </p>
@@ -67,9 +67,9 @@
 
 ``` bash
 pip3 install pysdbots
 ```
 
 ### API Url
 ```
-https://api.sdbots.tk
+https://api.sdbots.tech
 ```
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: pysdbots Version: 0.1.1 Summary: A Project Made To
+Metadata-Version: 2.1 Name: pysdbots Version: 2.0 Summary: A Project Made To
 Centralize Various APIs ð No Authorization Needed :) Home-page: https://
 github.com/damantha126/pysdbots Author: DamanthaJasinghe Author-email:
 damanthaja@gmail.com License: MIT Project-URL: Tracker, https://github.com/
 damantha126/pysdbots/issues Project-URL: Community, https://t.me/
 SDBOTs_inifinity Project-URL: Source, https://github.com/damantha126/pysdbots
-Project-URL: Documentation, https://docs.sdbots.tk Keywords: sdbots,python-
+Project-URL: Documentation, https://docs.sdbots.tech Keywords: sdbots,python-
 pakage,sd-api,api,damanthaja,mritzme,damantha126 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -26,8 +26,8 @@
 â¤ User Friendly
 â¤ JSON Response
 â¤ Easy To Use
 â¤ WEB Based API
 â¤ For All Platform
  ## â¢ Installations ### Install the library The best way to interact with our
 API is to use one of our official libraries ``` bash pip3 install pysdbots ```
-### API Url ``` https://api.sdbots.tk ```
+### API Url ``` https://api.sdbots.tech ```
```

### Comparing `pysdbots-0.1.1/setup.py` & `pysdbots-2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 with open("README.md", encoding="utf8") as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name="pysdbots",
     packages=setuptools.find_packages(),
-    version="0.1.1",
+    version="2.0",
     license="MIT",
     description="A Project Made To Centralize Various APIs 📖 No Authorization Needed :)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DamanthaJasinghe",
     author_email="damanthaja@gmail.com",
     url="https://github.com/damantha126/pysdbots",
     keywords=["sdbots", "python-pakage", "sd-api", "api", "damanthaja", "mritzme", "damantha126"],
     install_requires=["requests>=2.28.1"],
     project_urls={
         "Tracker": "https://github.com/damantha126/pysdbots/issues",
         "Community": "https://t.me/SDBOTs_inifinity",
         "Source": "https://github.com/damantha126/pysdbots",
-        "Documentation": "https://docs.sdbots.tk",
+        "Documentation": "https://docs.sdbots.tech",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

