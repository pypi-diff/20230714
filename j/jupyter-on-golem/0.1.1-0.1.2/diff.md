# Comparing `tmp/jupyter_on_golem-0.1.1.tar.gz` & `tmp/jupyter_on_golem-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_on_golem-0.1.1.tar", max compression
+gzip compressed data, was "jupyter_on_golem-0.1.2.tar", max compression
```

## Comparing `jupyter_on_golem-0.1.1.tar` & `jupyter_on_golem-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-07-13 11:20:06.802724 jupyter_on_golem-0.1.1/LICENSE
--rw-r--r--   0        0        0    13422 2023-07-13 11:20:06.802724 jupyter_on_golem-0.1.1/README.md
--rw-r--r--   0        0        0       73 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.1/jupyter_on_golem/__init__.py
--rw-r--r--   0        0        0     1283 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.1/jupyter_on_golem/__main__.py
--rw-r--r--   0        0        0    24503 2023-07-13 11:23:56.850117 jupyter_on_golem-0.1.1/jupyter_on_golem/golem.py
--rw-r--r--   0        0        0     2597 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.1/jupyter_on_golem/golem_kernel.py
--rw-r--r--   0        0        0      782 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.1/jupyter_on_golem/manifest.json
--rw-r--r--   0        0        0     3700 2023-07-13 11:20:06.810724 jupyter_on_golem-0.1.1/jupyter_on_golem/remote_python.py
--rw-r--r--   0        0        0      754 2023-07-13 11:25:02.465957 jupyter_on_golem-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    14498 1970-01-01 00:00:00.000000 jupyter_on_golem-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-14 12:00:18.341898 jupyter_on_golem-0.1.2/LICENSE
+-rw-r--r--   0        0        0    13354 2023-07-14 12:00:18.341898 jupyter_on_golem-0.1.2/README.md
+-rw-r--r--   0        0        0       73 2023-07-14 12:00:18.349898 jupyter_on_golem-0.1.2/jupyter_on_golem/__init__.py
+-rw-r--r--   0        0        0     1283 2023-07-14 12:00:18.349898 jupyter_on_golem-0.1.2/jupyter_on_golem/__main__.py
+-rw-r--r--   0        0        0    24507 2023-07-14 12:00:49.994194 jupyter_on_golem-0.1.2/jupyter_on_golem/golem.py
+-rw-r--r--   0        0        0     2597 2023-07-14 12:00:18.349898 jupyter_on_golem-0.1.2/jupyter_on_golem/golem_kernel.py
+-rw-r--r--   0        0        0      782 2023-07-14 12:00:18.349898 jupyter_on_golem-0.1.2/jupyter_on_golem/manifest.json
+-rw-r--r--   0        0        0     3700 2023-07-14 12:00:18.349898 jupyter_on_golem-0.1.2/jupyter_on_golem/remote_python.py
+-rw-r--r--   0        0        0      754 2023-07-14 12:00:40.830109 jupyter_on_golem-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    14430 1970-01-01 00:00:00.000000 jupyter_on_golem-0.1.2/PKG-INFO
```

### Comparing `jupyter_on_golem-0.1.1/LICENSE` & `jupyter_on_golem-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.1/README.md` & `jupyter_on_golem-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 Jupyter on Golem is a JupyterLab Python kernel (https://jupyterlab.readthedocs.io), which enables you to run your Python Notebooks using resources available on decentralized Golem Network (https://www.golem.network/). Providers of such resources are compensated for their work with GLM tokens.
 
 JupyterLab is an open-source project that is widely used by data scientists, analysts, researchers and developers. It allows you to create and share Notebooks - documents that combine code, equations, visualisations and narrative text. JupyterLab is part of Project Jupyter, umbrella project born from IPython Project (https://ipython.org/) and centered around providing tools for interactive computing with computational notebooks. Find more about Jupyter Project: https://jupyter.org/
 
 **Simplified view on JupyterLab:**
 
-![Simplified Diagram of a JupyterLab flow](https://github.com/golemfactory/golem-kernel-python/blob/2fac592d6dbcd88f73b830cabee774702c32326e/jupyterlab.png)
+![Simplified Diagram of a JupyterLab flow](https://raw.githubusercontent.com/golemfactory/golem-kernel-python/master/images/jupyterlab.png)
 
 **Simplified view on Jupyter on Golem:**
 
-![Simplified Diagram of a Jupyter on Golem flow](https://github.com/golemfactory/golem-kernel-python/blob/2fac592d6dbcd88f73b830cabee774702c32326e/jupyter_golem.png)
+![Simplified Diagram of a Jupyter on Golem flow](https://raw.githubusercontent.com/golemfactory/golem-kernel-python/master/images/jupyter_golem.png)
 
 Jupyter on Golem comes with following PyPI packages preinstallled:
 *   jupyter         - version 1.0.0
 *   pandas          - version 2.0.2
 *   tensorflow-cpu  - version 2.12.0
 *   matplotlib      - version 3.7.1
 
@@ -98,23 +98,23 @@
 
 ```
 jupyter-lab
 ```
 
 If installation process was completed correctly then Golem kernel should be visible and available in JupyterLab web interface:
 
-![Screenshot of a Golem kernel visible in JupyterLab web interface.](https://github.com/golemfactory/golem-kernel-python/blob/7f8669fbef78bfb4dc6ff9fbddc41e63d81bb2ba/Jupyter_on_Golem_kernel.png)
+![Screenshot of a Golem kernel visible in JupyterLab web interface.](https://raw.githubusercontent.com/golemfactory/golem-kernel-python/master/images/Jupyter_on_Golem_kernel.png)
 
 Click on the upper Golem icon (right under the Notebook section) to open new Notebook. You should be able to run Jupyter on Golem magic commands like _%help_ ,which will display the most important information about Jupyter on Golem:
 
 ```
 %help
 ```
 
-![Screenshot of a Golem help output in JupyterLab web interface.](https://github.com/golemfactory/golem-kernel-python/blob/7f8669fbef78bfb4dc6ff9fbddc41e63d81bb2ba/Jupyter_on_Golem_help.png)
+![Screenshot of a Golem help output in JupyterLab web interface.](https://raw.githubusercontent.com/golemfactory/golem-kernel-python/master/images/Jupyter_on_Golem_help.png)
 
 **When You finish using Jupyter on Golem You can close JupyterLab (File -> Shut Down) and press Ctrl+C in Yagna terminal window to turn it off.** 
 
 ## Commands
 
 Below You will find the list of all Jupter on Golem magic commands which are required to interact with this tool.
```

### Comparing `jupyter_on_golem-0.1.1/jupyter_on_golem/__main__.py` & `jupyter_on_golem-0.1.2/jupyter_on_golem/__main__.py`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.1/jupyter_on_golem/golem.py` & `jupyter_on_golem-0.1.2/jupyter_on_golem/golem.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,29 +42,29 @@
 '''
 
 HELP_TEMPLATE = '''\
      _                   _                             ____       _                
     | |_   _ _ __  _   _| |_ ___ _ __    ___  _ __    / ___| ___ | | ___ _ __ ___  
  _  | | | | | '_ \| | | | __/ _ \ '__|  / _ \| '_ \  | |  _ / _ \| |/ _ \ '_ ` _ \ 
 | |_| | |_| | |_) | |_| | ||  __/ |    | (_) | | | | | |_| | (_) | |  __/ | | | | |
- \___/ \__,_| .__/ \__, |\__\___|_|     \___/|_| |_|  \____|\___/|_|\___|_| |_| |_| version: 0.1.1
+ \___/ \__,_| .__/ \__, |\__\___|_|     \___/|_| |_|  \____|\___/|_|\___|_| |_| |_| version: 0.1.2
             |_|    |___/                                                           
 
 Easy to use tool to run Your Jupyter Notebooks on the Golem Network!
 
 COMMANDS:    
     %status		Shows current status of Jupyter on Golem
     %fund		Requests for testnet funds, e.g. '%fund goerli'
     %budget		Allocates GLM tokens for payments, e.g. '%budget goerli 2'. Available networks: goerli, polygon, mainnet.
     %connect		Looks for Provider which meets with defined criteria [mem|cores|disk], e.g. '%connect mem>1'				
     %disconnect 	Disconnects from the currently active Provider
     %download	 	Downloads file from Provider's ./workdir folder to local machine, e.g. '%download dataset.csv'
     %upload		Uploads file from local machine into Provider's ./workdir folder, e.g. '%upload results.csv'
     %help		Shows this message    
-    %pip install    Installs PyPI package on the Provider's host, e.g. "%pip install colorama"
+    %pip install        Installs PyPI package on the Provider's host, e.g. "%pip install colorama"
 
 '''
 
 PROVIDER_TEMPLATE = '''\
 Connected to {provider_name} [{provider_id}]
     RAM: {ram} GB
     DISK: {disk} GB
```

### Comparing `jupyter_on_golem-0.1.1/jupyter_on_golem/golem_kernel.py` & `jupyter_on_golem-0.1.2/jupyter_on_golem/golem_kernel.py`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.1/jupyter_on_golem/manifest.json` & `jupyter_on_golem-0.1.2/jupyter_on_golem/manifest.json`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.1/jupyter_on_golem/remote_python.py` & `jupyter_on_golem-0.1.2/jupyter_on_golem/remote_python.py`

 * *Files identical despite different names*

### Comparing `jupyter_on_golem-0.1.1/pyproject.toml` & `jupyter_on_golem-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "jupyter-on-golem"
-version = "0.1.1"
+version = "0.1.2"
 description = "Jupyter Python kernel running on Golem network (https://www.golem.network/)"
 readme = "README.md"
 authors = ["GolemFactory <contact.jupyter@golem.network>"]
 license = "LGPL-3.0-or-later"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: AsyncIO",
```

### Comparing `jupyter_on_golem-0.1.1/PKG-INFO` & `jupyter_on_golem-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-on-golem
-Version: 0.1.1
+Version: 0.1.2
 Summary: Jupyter Python kernel running on Golem network (https://www.golem.network/)
 License: LGPL-3.0-or-later
 Keywords: golem,jupyter,kernel,notebook
 Author: GolemFactory
 Author-email: contact.jupyter@golem.network
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -30,19 +30,19 @@
 
 Jupyter on Golem is a JupyterLab Python kernel (https://jupyterlab.readthedocs.io), which enables you to run your Python Notebooks using resources available on decentralized Golem Network (https://www.golem.network/). Providers of such resources are compensated for their work with GLM tokens.
 
 JupyterLab is an open-source project that is widely used by data scientists, analysts, researchers and developers. It allows you to create and share Notebooks - documents that combine code, equations, visualisations and narrative text. JupyterLab is part of Project Jupyter, umbrella project born from IPython Project (https://ipython.org/) and centered around providing tools for interactive computing with computational notebooks. Find more about Jupyter Project: https://jupyter.org/
 
 **Simplified view on JupyterLab:**
 
-![Simplified Diagram of a JupyterLab flow](https://github.com/golemfactory/golem-kernel-python/blob/2fac592d6dbcd88f73b830cabee774702c32326e/jupyterlab.png)
+![Simplified Diagram of a JupyterLab flow](https://raw.githubusercontent.com/golemfactory/golem-kernel-python/master/images/jupyterlab.png)
 
 **Simplified view on Jupyter on Golem:**
 
-![Simplified Diagram of a Jupyter on Golem flow](https://github.com/golemfactory/golem-kernel-python/blob/2fac592d6dbcd88f73b830cabee774702c32326e/jupyter_golem.png)
+![Simplified Diagram of a Jupyter on Golem flow](https://raw.githubusercontent.com/golemfactory/golem-kernel-python/master/images/jupyter_golem.png)
 
 Jupyter on Golem comes with following PyPI packages preinstallled:
 *   jupyter         - version 1.0.0
 *   pandas          - version 2.0.2
 *   tensorflow-cpu  - version 2.12.0
 *   matplotlib      - version 3.7.1
 
@@ -124,23 +124,23 @@
 
 ```
 jupyter-lab
 ```
 
 If installation process was completed correctly then Golem kernel should be visible and available in JupyterLab web interface:
 
-![Screenshot of a Golem kernel visible in JupyterLab web interface.](https://github.com/golemfactory/golem-kernel-python/blob/7f8669fbef78bfb4dc6ff9fbddc41e63d81bb2ba/Jupyter_on_Golem_kernel.png)
+![Screenshot of a Golem kernel visible in JupyterLab web interface.](https://raw.githubusercontent.com/golemfactory/golem-kernel-python/master/images/Jupyter_on_Golem_kernel.png)
 
 Click on the upper Golem icon (right under the Notebook section) to open new Notebook. You should be able to run Jupyter on Golem magic commands like _%help_ ,which will display the most important information about Jupyter on Golem:
 
 ```
 %help
 ```
 
-![Screenshot of a Golem help output in JupyterLab web interface.](https://github.com/golemfactory/golem-kernel-python/blob/7f8669fbef78bfb4dc6ff9fbddc41e63d81bb2ba/Jupyter_on_Golem_help.png)
+![Screenshot of a Golem help output in JupyterLab web interface.](https://raw.githubusercontent.com/golemfactory/golem-kernel-python/master/images/Jupyter_on_Golem_help.png)
 
 **When You finish using Jupyter on Golem You can close JupyterLab (File -> Shut Down) and press Ctrl+C in Yagna terminal window to turn it off.** 
 
 ## Commands
 
 Below You will find the list of all Jupter on Golem magic commands which are required to interact with this tool.
```

