# Comparing `tmp/idftools-0.1.5.tar.gz` & `tmp/idftools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idftools-0.1.5.tar", last modified: Fri Jul 14 19:47:12 2023, max compression
+gzip compressed data, was "idftools-0.1.6.tar", last modified: Fri Jul 14 20:33:56 2023, max compression
```

## Comparing `idftools-0.1.5.tar` & `idftools-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 19:47:12.943990 idftools-0.1.5/
--rw-rw-r--   0 enio      (1000) enio      (1000)     5869 2023-07-14 19:47:12.939990 idftools-0.1.5/PKG-INFO
--rw-rw-r--   0 enio      (1000) enio      (1000)     3909 2023-07-14 19:46:57.000000 idftools-0.1.5/README.md
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 19:47:12.939990 idftools-0.1.5/idftools/
--rw-rw-r--   0 enio      (1000) enio      (1000)    34945 2023-05-25 18:44:21.000000 idftools-0.1.5/idftools/certificate.py
--rwxrwxr-x   0 enio      (1000) enio      (1000)    22099 2023-07-13 20:03:14.000000 idftools-0.1.5/idftools/driversfactory.py
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 19:47:12.939990 idftools-0.1.5/idftools/idftools.egg-info/
--rw-rw-r--   0 enio      (1000) enio      (1000)     5869 2023-07-14 19:47:12.000000 idftools-0.1.5/idftools/idftools.egg-info/PKG-INFO
--rw-rw-r--   0 enio      (1000) enio      (1000)      295 2023-07-14 19:47:12.000000 idftools-0.1.5/idftools/idftools.egg-info/SOURCES.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)        1 2023-07-14 19:47:12.000000 idftools-0.1.5/idftools/idftools.egg-info/dependency_links.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)      373 2023-07-14 19:47:12.000000 idftools-0.1.5/idftools/idftools.egg-info/requires.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)       37 2023-07-14 19:47:12.000000 idftools-0.1.5/idftools/idftools.egg-info/top_level.txt
--rwxrwxr-x   0 enio      (1000) enio      (1000)    70637 2023-07-13 20:10:20.000000 idftools-0.1.5/idftools/utilities.py
--rw-rw-r--   0 enio      (1000) enio      (1000)       38 2023-07-14 19:47:12.943990 idftools-0.1.5/setup.cfg
--rw-rw-r--   0 enio      (1000) enio      (1000)      917 2023-07-14 19:45:21.000000 idftools-0.1.5/setup.py
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 20:33:56.525880 idftools-0.1.6/
+-rw-rw-r--   0 enio      (1000) enio      (1000)     6274 2023-07-14 20:33:56.525880 idftools-0.1.6/PKG-INFO
+-rw-rw-r--   0 enio      (1000) enio      (1000)     4242 2023-07-14 20:33:15.000000 idftools-0.1.6/README.md
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 20:33:56.521883 idftools-0.1.6/idftools/
+-rw-rw-r--   0 enio      (1000) enio      (1000)    34945 2023-05-25 18:44:21.000000 idftools-0.1.6/idftools/certificate.py
+-rwxrwxr-x   0 enio      (1000) enio      (1000)    22099 2023-07-13 20:03:14.000000 idftools-0.1.6/idftools/driversfactory.py
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 20:33:56.525880 idftools-0.1.6/idftools/idftools.egg-info/
+-rw-rw-r--   0 enio      (1000) enio      (1000)     6274 2023-07-14 20:33:56.000000 idftools-0.1.6/idftools/idftools.egg-info/PKG-INFO
+-rw-rw-r--   0 enio      (1000) enio      (1000)      295 2023-07-14 20:33:56.000000 idftools-0.1.6/idftools/idftools.egg-info/SOURCES.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)        1 2023-07-14 20:33:56.000000 idftools-0.1.6/idftools/idftools.egg-info/dependency_links.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)      373 2023-07-14 20:33:56.000000 idftools-0.1.6/idftools/idftools.egg-info/requires.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)       37 2023-07-14 20:33:56.000000 idftools-0.1.6/idftools/idftools.egg-info/top_level.txt
+-rwxrwxr-x   0 enio      (1000) enio      (1000)    70637 2023-07-13 20:10:20.000000 idftools-0.1.6/idftools/utilities.py
+-rw-rw-r--   0 enio      (1000) enio      (1000)       38 2023-07-14 20:33:56.525880 idftools-0.1.6/setup.cfg
+-rw-rw-r--   0 enio      (1000) enio      (1000)      917 2023-07-14 20:33:42.000000 idftools-0.1.6/setup.py
```

### Comparing `idftools-0.1.5/PKG-INFO` & `idftools-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: idftools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Um pacote com alguns utilitarios uteis
 Home-page: https://github.com/eniodefarias/pypi-idftools
 Author: eniodefarias
 Author-email: eniodefarias@gmail.com
 License: UNKNOWN
-Description: # I.d.F. tools
+Description: <p align="center">
+          <img src="http://ideiadofuturo.com.br/img/logo_ideia.png" width="120" title="supervisão"  alt="Supervisao Contabilidade e Consultoria">  
+        </p>
+        
+        
+        # I.d.F. tools
         
          - [https://pypi.org/project/idftools/](https://pypi.org/project/idftools/)
         
         ## pre-requirements.txt
         ```text
         webdriver_manager
         wincertstore
@@ -210,9 +215,13 @@
         ### terminal do gitbash
         ```bash
         set UPX= --ultra-brute --best --compress-icons#0 ; time .venv/Scripts/python.exe -m PyInstaller --upx-dir=./ --noconfirm --onefile --paths .venv/Lib/site-packages --icon=icone/logo.ico -n  app app.py ; rm app.exe ; mv dist/app.exe . ; ls -latrh *.exe
         ```
             
         
         ---
+        
+        <p align="center">
+          <img src="http://ideiadofuturo.com.br/img/logo_ideia.png" width="120" title="supervisão"  alt="Supervisao Contabilidade e Consultoria">  
+        </p>
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `idftools-0.1.5/README.md` & `idftools-0.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+<p align="center">
+  <img src="http://ideiadofuturo.com.br/img/logo_ideia.png" width="120" title="supervisão"  alt="Supervisao Contabilidade e Consultoria">  
+</p>
+
+
 # I.d.F. tools
 
  - [https://pypi.org/project/idftools/](https://pypi.org/project/idftools/)
 
 ## pre-requirements.txt
 ```text
 webdriver_manager
@@ -201,8 +206,12 @@
 
 ### terminal do gitbash
 ```bash
 set UPX= --ultra-brute --best --compress-icons#0 ; time .venv/Scripts/python.exe -m PyInstaller --upx-dir=./ --noconfirm --onefile --paths .venv/Lib/site-packages --icon=icone/logo.ico -n  app app.py ; rm app.exe ; mv dist/app.exe . ; ls -latrh *.exe
 ```
     
 
----
+---
+
+<p align="center">
+  <img src="http://ideiadofuturo.com.br/img/logo_ideia.png" width="120" title="supervisão"  alt="Supervisao Contabilidade e Consultoria">  
+</p>
```

### Comparing `idftools-0.1.5/idftools/certificate.py` & `idftools-0.1.6/idftools/certificate.py`

 * *Files identical despite different names*

### Comparing `idftools-0.1.5/idftools/driversfactory.py` & `idftools-0.1.6/idftools/driversfactory.py`

 * *Files identical despite different names*

### Comparing `idftools-0.1.5/idftools/idftools.egg-info/PKG-INFO` & `idftools-0.1.6/idftools/idftools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: idftools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Um pacote com alguns utilitarios uteis
 Home-page: https://github.com/eniodefarias/pypi-idftools
 Author: eniodefarias
 Author-email: eniodefarias@gmail.com
 License: UNKNOWN
-Description: # I.d.F. tools
+Description: <p align="center">
+          <img src="http://ideiadofuturo.com.br/img/logo_ideia.png" width="120" title="supervisão"  alt="Supervisao Contabilidade e Consultoria">  
+        </p>
+        
+        
+        # I.d.F. tools
         
          - [https://pypi.org/project/idftools/](https://pypi.org/project/idftools/)
         
         ## pre-requirements.txt
         ```text
         webdriver_manager
         wincertstore
@@ -210,9 +215,13 @@
         ### terminal do gitbash
         ```bash
         set UPX= --ultra-brute --best --compress-icons#0 ; time .venv/Scripts/python.exe -m PyInstaller --upx-dir=./ --noconfirm --onefile --paths .venv/Lib/site-packages --icon=icone/logo.ico -n  app app.py ; rm app.exe ; mv dist/app.exe . ; ls -latrh *.exe
         ```
             
         
         ---
+        
+        <p align="center">
+          <img src="http://ideiadofuturo.com.br/img/logo_ideia.png" width="120" title="supervisão"  alt="Supervisao Contabilidade e Consultoria">  
+        </p>
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `idftools-0.1.5/idftools/utilities.py` & `idftools-0.1.6/idftools/utilities.py`

 * *Files identical despite different names*

### Comparing `idftools-0.1.5/setup.py` & `idftools-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 print(f'long_description={long_description}')
 
 setup(
-    version="0.1.5",
+    version="0.1.6",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=requirements,
     name="idftools",
     author_email="eniodefarias@gmail.com",
     author="eniodefarias",
     url="https://github.com/eniodefarias/pypi-idftools",
```

