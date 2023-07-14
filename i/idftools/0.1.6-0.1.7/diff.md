# Comparing `tmp/idftools-0.1.6.tar.gz` & `tmp/idftools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idftools-0.1.6.tar", last modified: Fri Jul 14 20:33:56 2023, max compression
+gzip compressed data, was "idftools-0.1.7.tar", last modified: Fri Jul 14 20:57:27 2023, max compression
```

## Comparing `idftools-0.1.6.tar` & `idftools-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 20:33:56.525880 idftools-0.1.6/
--rw-rw-r--   0 enio      (1000) enio      (1000)     6274 2023-07-14 20:33:56.525880 idftools-0.1.6/PKG-INFO
--rw-rw-r--   0 enio      (1000) enio      (1000)     4242 2023-07-14 20:33:15.000000 idftools-0.1.6/README.md
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 20:33:56.521883 idftools-0.1.6/idftools/
--rw-rw-r--   0 enio      (1000) enio      (1000)    34945 2023-05-25 18:44:21.000000 idftools-0.1.6/idftools/certificate.py
--rwxrwxr-x   0 enio      (1000) enio      (1000)    22099 2023-07-13 20:03:14.000000 idftools-0.1.6/idftools/driversfactory.py
-drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 20:33:56.525880 idftools-0.1.6/idftools/idftools.egg-info/
--rw-rw-r--   0 enio      (1000) enio      (1000)     6274 2023-07-14 20:33:56.000000 idftools-0.1.6/idftools/idftools.egg-info/PKG-INFO
--rw-rw-r--   0 enio      (1000) enio      (1000)      295 2023-07-14 20:33:56.000000 idftools-0.1.6/idftools/idftools.egg-info/SOURCES.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)        1 2023-07-14 20:33:56.000000 idftools-0.1.6/idftools/idftools.egg-info/dependency_links.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)      373 2023-07-14 20:33:56.000000 idftools-0.1.6/idftools/idftools.egg-info/requires.txt
--rw-rw-r--   0 enio      (1000) enio      (1000)       37 2023-07-14 20:33:56.000000 idftools-0.1.6/idftools/idftools.egg-info/top_level.txt
--rwxrwxr-x   0 enio      (1000) enio      (1000)    70637 2023-07-13 20:10:20.000000 idftools-0.1.6/idftools/utilities.py
--rw-rw-r--   0 enio      (1000) enio      (1000)       38 2023-07-14 20:33:56.525880 idftools-0.1.6/setup.cfg
--rw-rw-r--   0 enio      (1000) enio      (1000)      917 2023-07-14 20:33:42.000000 idftools-0.1.6/setup.py
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 20:57:27.835754 idftools-0.1.7/
+-rw-rw-r--   0 enio      (1000) enio      (1000)     6293 2023-07-14 20:57:27.835754 idftools-0.1.7/PKG-INFO
+-rw-rw-r--   0 enio      (1000) enio      (1000)     4261 2023-07-14 20:37:31.000000 idftools-0.1.7/README.md
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 20:57:27.835754 idftools-0.1.7/idftools/
+-rw-rw-r--   0 enio      (1000) enio      (1000)    34945 2023-05-25 18:44:21.000000 idftools-0.1.7/idftools/certificate.py
+-rwxrwxr-x   0 enio      (1000) enio      (1000)    22099 2023-07-13 20:03:14.000000 idftools-0.1.7/idftools/driversfactory.py
+drwxrwxr-x   0 enio      (1000) enio      (1000)        0 2023-07-14 20:57:27.835754 idftools-0.1.7/idftools/idftools.egg-info/
+-rw-rw-r--   0 enio      (1000) enio      (1000)     6293 2023-07-14 20:57:27.000000 idftools-0.1.7/idftools/idftools.egg-info/PKG-INFO
+-rw-rw-r--   0 enio      (1000) enio      (1000)      255 2023-07-14 20:57:27.000000 idftools-0.1.7/idftools/idftools.egg-info/SOURCES.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)        1 2023-07-14 20:57:27.000000 idftools-0.1.7/idftools/idftools.egg-info/dependency_links.txt
+-rw-rw-r--   0 enio      (1000) enio      (1000)       37 2023-07-14 20:57:27.000000 idftools-0.1.7/idftools/idftools.egg-info/top_level.txt
+-rwxrwxr-x   0 enio      (1000) enio      (1000)    70637 2023-07-13 20:10:20.000000 idftools-0.1.7/idftools/utilities.py
+-rw-rw-r--   0 enio      (1000) enio      (1000)       38 2023-07-14 20:57:27.835754 idftools-0.1.7/setup.cfg
+-rw-rw-r--   0 enio      (1000) enio      (1000)      919 2023-07-14 20:57:17.000000 idftools-0.1.7/setup.py
```

### Comparing `idftools-0.1.6/PKG-INFO` & `idftools-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: idftools
-Version: 0.1.6
+Version: 0.1.7
 Summary: Um pacote com alguns utilitarios uteis
 Home-page: https://github.com/eniodefarias/pypi-idftools
 Author: eniodefarias
 Author-email: eniodefarias@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img src="http://ideiadofuturo.com.br/img/logo_ideia.png" width="120" title="supervisão"  alt="Supervisao Contabilidade e Consultoria">  
         </p>
         
         
-        # I.d.F. tools
+        # Ideia do Futuro - IdFtools
         
          - [https://pypi.org/project/idftools/](https://pypi.org/project/idftools/)
         
         ## pre-requirements.txt
         ```text
         webdriver_manager
         wincertstore
@@ -168,32 +168,32 @@
         ```bash    
         /home/$(whoami)/.pyenv/shims/python3 -m venv .venv
         ```
         
         ### instalar os requirements.txt na mão
         #### usando o gitbash
         ```bash     
-        cat requirements.txt|sort|uniq | xargs -n 1 .venv/Scripts/pip3.exe install ; .venv/Scripts/python.exe -m pip install --upgrade pip
+        cat requirements.txt| grep -v "#"|sort|uniq | xargs -n 1 .venv/Scripts/pip3.exe install ; .venv/Scripts/python.exe -m pip install --upgrade pip
         ```
         
         #### usando o shell do linux
         ```bash    
-        cat requirements.txt|sort|uniq | xargs -n 1 .venv/bin/pip install ; .venv/bin/python3 -m pip install --upgrade pip
+        cat requirements.txt| grep -v "#"|sort|uniq | xargs -n 1 .venv/bin/pip install ; .venv/bin/python3 -m pip install --upgrade pip
         ```
         
         ### atualizar modulos no Gitbash
         ```bash    
         .venv/Scripts/python.exe -m pip install PyInstaller
         .venv/Scripts/python.exe -m pip install --upgrade pip
         .venv/Scripts/python.exe -m pip install --upgrade idftools
         ```
         
         ### enviar "git push" da branch
         ```bash    
-        git add . ; git add * ; git commit -m "fix: ajuste de log debug com prints" ; git push -f origin main
+        git add . ; git add * ; git commit -m "update: ajuste" ; git push -f origin main
         ```
         
         ## executar:
         
         ### terminal gitbash
         ```bash     
         .venv/Scripts/python.exe app.py
```

### Comparing `idftools-0.1.6/README.md` & `idftools-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <p align="center">
   <img src="http://ideiadofuturo.com.br/img/logo_ideia.png" width="120" title="supervisão"  alt="Supervisao Contabilidade e Consultoria">  
 </p>
 
 
-# I.d.F. tools
+# Ideia do Futuro - IdFtools
 
  - [https://pypi.org/project/idftools/](https://pypi.org/project/idftools/)
 
 ## pre-requirements.txt
 ```text
 webdriver_manager
 wincertstore
@@ -160,32 +160,32 @@
 ```bash    
 /home/$(whoami)/.pyenv/shims/python3 -m venv .venv
 ```
 
 ### instalar os requirements.txt na mão
 #### usando o gitbash
 ```bash     
-cat requirements.txt|sort|uniq | xargs -n 1 .venv/Scripts/pip3.exe install ; .venv/Scripts/python.exe -m pip install --upgrade pip
+cat requirements.txt| grep -v "#"|sort|uniq | xargs -n 1 .venv/Scripts/pip3.exe install ; .venv/Scripts/python.exe -m pip install --upgrade pip
 ```
 
 #### usando o shell do linux
 ```bash    
-cat requirements.txt|sort|uniq | xargs -n 1 .venv/bin/pip install ; .venv/bin/python3 -m pip install --upgrade pip
+cat requirements.txt| grep -v "#"|sort|uniq | xargs -n 1 .venv/bin/pip install ; .venv/bin/python3 -m pip install --upgrade pip
 ```
 
 ### atualizar modulos no Gitbash
 ```bash    
 .venv/Scripts/python.exe -m pip install PyInstaller
 .venv/Scripts/python.exe -m pip install --upgrade pip
 .venv/Scripts/python.exe -m pip install --upgrade idftools
 ```
 
 ### enviar "git push" da branch
 ```bash    
-git add . ; git add * ; git commit -m "fix: ajuste de log debug com prints" ; git push -f origin main
+git add . ; git add * ; git commit -m "update: ajuste" ; git push -f origin main
 ```
 
 ## executar:
 
 ### terminal gitbash
 ```bash     
 .venv/Scripts/python.exe app.py
```

### Comparing `idftools-0.1.6/idftools/certificate.py` & `idftools-0.1.7/idftools/certificate.py`

 * *Files identical despite different names*

### Comparing `idftools-0.1.6/idftools/driversfactory.py` & `idftools-0.1.7/idftools/driversfactory.py`

 * *Files identical despite different names*

### Comparing `idftools-0.1.6/idftools/idftools.egg-info/PKG-INFO` & `idftools-0.1.7/idftools/idftools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: idftools
-Version: 0.1.6
+Version: 0.1.7
 Summary: Um pacote com alguns utilitarios uteis
 Home-page: https://github.com/eniodefarias/pypi-idftools
 Author: eniodefarias
 Author-email: eniodefarias@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img src="http://ideiadofuturo.com.br/img/logo_ideia.png" width="120" title="supervisão"  alt="Supervisao Contabilidade e Consultoria">  
         </p>
         
         
-        # I.d.F. tools
+        # Ideia do Futuro - IdFtools
         
          - [https://pypi.org/project/idftools/](https://pypi.org/project/idftools/)
         
         ## pre-requirements.txt
         ```text
         webdriver_manager
         wincertstore
@@ -168,32 +168,32 @@
         ```bash    
         /home/$(whoami)/.pyenv/shims/python3 -m venv .venv
         ```
         
         ### instalar os requirements.txt na mão
         #### usando o gitbash
         ```bash     
-        cat requirements.txt|sort|uniq | xargs -n 1 .venv/Scripts/pip3.exe install ; .venv/Scripts/python.exe -m pip install --upgrade pip
+        cat requirements.txt| grep -v "#"|sort|uniq | xargs -n 1 .venv/Scripts/pip3.exe install ; .venv/Scripts/python.exe -m pip install --upgrade pip
         ```
         
         #### usando o shell do linux
         ```bash    
-        cat requirements.txt|sort|uniq | xargs -n 1 .venv/bin/pip install ; .venv/bin/python3 -m pip install --upgrade pip
+        cat requirements.txt| grep -v "#"|sort|uniq | xargs -n 1 .venv/bin/pip install ; .venv/bin/python3 -m pip install --upgrade pip
         ```
         
         ### atualizar modulos no Gitbash
         ```bash    
         .venv/Scripts/python.exe -m pip install PyInstaller
         .venv/Scripts/python.exe -m pip install --upgrade pip
         .venv/Scripts/python.exe -m pip install --upgrade idftools
         ```
         
         ### enviar "git push" da branch
         ```bash    
-        git add . ; git add * ; git commit -m "fix: ajuste de log debug com prints" ; git push -f origin main
+        git add . ; git add * ; git commit -m "update: ajuste" ; git push -f origin main
         ```
         
         ## executar:
         
         ### terminal gitbash
         ```bash     
         .venv/Scripts/python.exe app.py
```

### Comparing `idftools-0.1.6/idftools/utilities.py` & `idftools-0.1.7/idftools/utilities.py`

 * *Files identical despite different names*

### Comparing `idftools-0.1.6/setup.py` & `idftools-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 print(f'long_description={long_description}')
 
 setup(
-    version="0.1.6",
+    version="0.1.7",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    install_requires=requirements,
+    # install_requires=requirements,
     name="idftools",
     author_email="eniodefarias@gmail.com",
     author="eniodefarias",
     url="https://github.com/eniodefarias/pypi-idftools",
     description="Um pacote com alguns utilitarios uteis",
     py_modules=["utilities", "driversfactory", "certificate"],
     package_dir={"": "idftools"}
```

