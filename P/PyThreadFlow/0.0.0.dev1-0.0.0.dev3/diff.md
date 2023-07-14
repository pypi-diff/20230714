# Comparing `tmp/pythreadflow-0.0.0.dev1.tar.gz` & `tmp/pythreadflow-0.0.0.dev3.tar.gz`

## Comparing `pythreadflow-0.0.0.dev1.tar` & `pythreadflow-0.0.0.dev3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev1/PyThreadFlow/threadFlowManager/__init__.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev1/PyThreadFlow/threadFlowManager/advthreads.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev1/LICENCE
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev1/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev3/PyThreadFlow/threadFlowManager/__init__.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev3/PyThreadFlow/threadFlowManager/advthreads.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev3/LICENCE
+-rw-r--r--   0        0        0     7928 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev3/README.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 pythreadflow-0.0.0.dev3/PKG-INFO
```

### Comparing `pythreadflow-0.0.0.dev1/.github/workflows/python-publish.yml` & `pythreadflow-0.0.0.dev3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pythreadflow-0.0.0.dev1/PyThreadFlow/threadFlowManager/advthreads.py` & `pythreadflow-0.0.0.dev3/PyThreadFlow/threadFlowManager/advthreads.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import threading as thread
 import queue as cue
 import warnings
+import time as sun
 
 class LegacyWarning(Warning):
     pass
 
 def __deprecated(func):
     def wrapper(*args, **kwargs):
         warnings.warn(f"Call to deprecated function \"{func.__name__}\".", category=DeprecationWarning)
@@ -46,13 +47,33 @@
     t.start() # start the threads
     time.sleep(40) # wait for the execution to finish
     t.stop() # calls the exitNetwork function, then exits the thread
     #...
     ```
     
     """
-    def __init__(self, mainLoop:object, openLoop:object, exitloop:object, daemon:bool=False, arguments:tuple=()):
-        self.data = [mainLoop, openLoop, exitloop, daemon, arguments]
+    def __init__(self, mainLoop:object, openLoop:object, exitloop:object, daemon:bool=False, arguments:tuple=(), delay=0.5):
+        self.data = [mainLoop, openLoop, exitloop, daemon, arguments, delay]
         self.flags = [0 if arguments == () else 1, 1 if __name__ != "__main__" else 0]
     
+    def __mloopy(this, argTuple, mloop, delay):
+        while globals()['running'] == True:
+            mloop(*argTuple)
+            sun.sleep(delay)
+        x = this.data[2]
+        x()
+
+    def start(self):
+        globals()['running'] = True
+
+        ithread = thread.Thread(target=self.data[1], daemon=self.data[3])
+        self.ml = thread.Thread(target=self.__mloopy, daemon=self.data[3], args=(self.data[4], self.data[0], self.data[5]))
+        ithread.start()
+        ithread.join()
+        self.ml.start()
+
+    def stop(self):
+        globals()['running'] = False
+        self.ml.join()
+
     def instanceChecker(self):
         print(f"{self.data=}\n{self.flags=}")
```

### Comparing `pythreadflow-0.0.0.dev1/LICENCE` & `pythreadflow-0.0.0.dev3/LICENCE`

 * *Files identical despite different names*

### Comparing `pythreadflow-0.0.0.dev1/README.md` & `pythreadflow-0.0.0.dev3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 # PyThreadFlow V0.0.1.dev1
 
-[skip to changes](https://github.com/nilonic/PyThreadFlow#changes)
+[skip to changes](#changes)
 
 PyThreadFlow is a Python threading extension that simplifies and enhances threading functionality by providing an init call, an event loop, and an exit call. These additions make multithreading in Python easier and more reliable.
 
-## How can I download PyThreadFlow?
+PyThreadFlow is now conveniently available for download through the official PyPI page. This announcement marks a significant milestone in the accessibility and distribution of PyThreadFlow. If you're interested in obtaining PyThreadFlow, you can easily do so by following a few simple steps.
 
-for the moment, you can download it using this command:
+Firstly, navigate to the PyPI page dedicated to PyThreadFlow. You can access this page by clicking on the following link: [here](https://pypi.org/project/PyThreadFlow/). The PyPI page provides comprehensive information about PyThreadFlow, including its features, version history, and documentation.
+
+Once you have accessed the PyPI page, you will find the necessary command to download PyThreadFlow. To simplify the process, you can use the Python package manager, pip, which is a widely-used tool for installing Python packages. Open your preferred command-line interface, such as the terminal or command prompt, and execute the following command:
 
 ```bash
-pip install -i https://test.pypi.org/simple/ PyThreadFlow==0.0.4.dev2
+pip install PyThreadFlow
 ```
 
+By running this command, you initiate the download and installation process for PyThreadFlow. Pip automatically handles the retrieval of the package from PyPI and its installation onto your local machine. It ensures that any dependencies required by PyThreadFlow are also resolved and installed, making the process seamless for you.
+
+Once the installation is complete, you can start exploring and utilizing the functionalities provided by PyThreadFlow within your Python environment. Whether you're a developer, researcher, or enthusiast, PyThreadFlow offers a range of tools and capabilities to enhance your threading and parallel computing experiences.
+
+Remember, if you encounter any issues during the installation or have any questions regarding PyThreadFlow, the PyPI page may provide additional resources, such as documentation, FAQs, or a community forum, to assist you. Feel free to refer to these resources for further guidance.
+
+Congratulations! You're now equipped with the knowledge and steps required to download PyThreadFlow and unlock its potential for your projects. Happy coding!
+
 ## How can I use PyThreadFlow?
 
 To utilize PyThreadFlow, you can follow the example below:
 
 ```python
 from pyThreadFlow.threadFlowManager import advthreads
 # ...
@@ -39,12 +49,16 @@
 
 1. **Added framework for legacy, deprecated, and more wrappers**: This update includes the addition of a framework that handles legacy, deprecated, and other types of wrappers. This framework allows for better management and organization of different types of wrappers within the system. By implementing this framework, it becomes easier to identify and handle code that needs to be phased out or replaced due to being outdated or no longer supported. It also facilitates the introduction of new wrappers or modifications to existing ones.
 
 2. **Added framework for the thread multi-thread parts**: Another significant addition is the implementation of a framework specifically designed to handle the multi-threading aspects of the code. This framework provides the necessary structure and functionality to support multi-threaded operations within the application. While the framework has been implemented, the next step is to incorporate the appropriate callers that will utilize and interact with the multi-threading capabilities. Once these callers are added, the system will be able to effectively leverage multiple threads for concurrent execution, improving performance and efficiency.
 
 3. **Added check in `__init__` so it can't be run directly**: A check has been introduced in the `__init__` function to prevent it from being executed directly. This modification ensures that the initialization process follows the correct procedure and is triggered through the appropriate mechanisms. By disallowing direct execution of the `__init__` function, potential errors or unintended consequences arising from manual invocations can be avoided. This check adds an extra layer of safety and helps maintain the integrity and stability of the codebase.
 
+4. **Fixed the MD file again**: During the initial release of PyThreadFlow, we encountered an issue with the Markdown (MD) file associated with the project. However, rest assured that we have addressed this problem promptly. Our team has worked diligently to rectify the MD file, ensuring that it now functions correctly. We sincerely apologize for any inconvenience caused. With the MD file now fixed, you can proceed to enjoy PyThreadFlow V0.0.0.dev2, taking full advantage of its features and functionalities.
+
+5. **Updated the files**: We deeply regret to inform you that an incorrect version of the files was inadvertently uploaded during our previous release. We sincerely apologize for any confusion or inconvenience caused by this oversight. However, we want to assure you that we have swiftly rectified the situation. Our team has taken immediate action to update the files, ensuring that the correct version is now available for download. We understand the importance of delivering accurate and reliable software, and we appreciate your understanding and patience during this process. Thank you for your continued support as we strive to provide you with the best possible experience with PyThreadFlow.
+
 ## TODOs
 
 1. **Add functionality for the init, running, and exit calls for the threading flow manager**: The next task is to implement the necessary functionality for the initialization (`init`), running, and exit calls within the threading flow manager. This involves defining and integrating the required code to properly handle the initialization phase, manage the execution of threaded processes, and handle the clean-up and termination of threads upon program completion. Once these functionalities are in place, the threading flow manager will be able to orchestrate and control the multi-threading operations effectively.
 
 2. **Find more bugs to report**: As an ongoing process of improving the system's reliability and performance, the task of identifying and reporting bugs remains a priority. By actively searching for and documenting any existing issues or glitches in the codebase, it becomes possible to address them systematically and enhance the overall quality of the software. This task involves thorough testing, debugging, and reporting of any anomalies or unexpected behaviors encountered during the development and usage of the application. By continuously striving to find and resolve bugs, the stability and user experience of the software can be significantly improved.
```

### Comparing `pythreadflow-0.0.0.dev1/pyproject.toml` & `pythreadflow-0.0.0.dev3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyThreadFlow"
-version = "0.0.0.dev1"
+version = "0.0.0.dev3"
 authors = [
   { name="Nilonic", email="nilonic.suggestions@gmail.com" },
 ]
 description = "a python threadding extension meant to boost threading capabilities"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pythreadflow-0.0.0.dev1/PKG-INFO` & `pythreadflow-0.0.0.dev3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 Metadata-Version: 2.1
 Name: PyThreadFlow
-Version: 0.0.0.dev1
+Version: 0.0.0.dev3
 Summary: a python threadding extension meant to boost threading capabilities
 Project-URL: Homepage, https://nilonic.github.io/PyThreadFlow/
 Project-URL: Bug Tracker, https://github.com/nilonic/PyThreadFlow/issues
 Author-email: Nilonic <nilonic.suggestions@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # PyThreadFlow V0.0.1.dev1
 
-[skip to changes](https://github.com/nilonic/PyThreadFlow#changes)
+[skip to changes](#changes)
 
 PyThreadFlow is a Python threading extension that simplifies and enhances threading functionality by providing an init call, an event loop, and an exit call. These additions make multithreading in Python easier and more reliable.
 
-## How can I download PyThreadFlow?
+PyThreadFlow is now conveniently available for download through the official PyPI page. This announcement marks a significant milestone in the accessibility and distribution of PyThreadFlow. If you're interested in obtaining PyThreadFlow, you can easily do so by following a few simple steps.
 
-for the moment, you can download it using this command:
+Firstly, navigate to the PyPI page dedicated to PyThreadFlow. You can access this page by clicking on the following link: [here](https://pypi.org/project/PyThreadFlow/). The PyPI page provides comprehensive information about PyThreadFlow, including its features, version history, and documentation.
+
+Once you have accessed the PyPI page, you will find the necessary command to download PyThreadFlow. To simplify the process, you can use the Python package manager, pip, which is a widely-used tool for installing Python packages. Open your preferred command-line interface, such as the terminal or command prompt, and execute the following command:
 
 ```bash
-pip install -i https://test.pypi.org/simple/ PyThreadFlow==0.0.4.dev2
+pip install PyThreadFlow
 ```
 
+By running this command, you initiate the download and installation process for PyThreadFlow. Pip automatically handles the retrieval of the package from PyPI and its installation onto your local machine. It ensures that any dependencies required by PyThreadFlow are also resolved and installed, making the process seamless for you.
+
+Once the installation is complete, you can start exploring and utilizing the functionalities provided by PyThreadFlow within your Python environment. Whether you're a developer, researcher, or enthusiast, PyThreadFlow offers a range of tools and capabilities to enhance your threading and parallel computing experiences.
+
+Remember, if you encounter any issues during the installation or have any questions regarding PyThreadFlow, the PyPI page may provide additional resources, such as documentation, FAQs, or a community forum, to assist you. Feel free to refer to these resources for further guidance.
+
+Congratulations! You're now equipped with the knowledge and steps required to download PyThreadFlow and unlock its potential for your projects. Happy coding!
+
 ## How can I use PyThreadFlow?
 
 To utilize PyThreadFlow, you can follow the example below:
 
 ```python
 from pyThreadFlow.threadFlowManager import advthreads
 # ...
@@ -53,12 +63,16 @@
 
 1. **Added framework for legacy, deprecated, and more wrappers**: This update includes the addition of a framework that handles legacy, deprecated, and other types of wrappers. This framework allows for better management and organization of different types of wrappers within the system. By implementing this framework, it becomes easier to identify and handle code that needs to be phased out or replaced due to being outdated or no longer supported. It also facilitates the introduction of new wrappers or modifications to existing ones.
 
 2. **Added framework for the thread multi-thread parts**: Another significant addition is the implementation of a framework specifically designed to handle the multi-threading aspects of the code. This framework provides the necessary structure and functionality to support multi-threaded operations within the application. While the framework has been implemented, the next step is to incorporate the appropriate callers that will utilize and interact with the multi-threading capabilities. Once these callers are added, the system will be able to effectively leverage multiple threads for concurrent execution, improving performance and efficiency.
 
 3. **Added check in `__init__` so it can't be run directly**: A check has been introduced in the `__init__` function to prevent it from being executed directly. This modification ensures that the initialization process follows the correct procedure and is triggered through the appropriate mechanisms. By disallowing direct execution of the `__init__` function, potential errors or unintended consequences arising from manual invocations can be avoided. This check adds an extra layer of safety and helps maintain the integrity and stability of the codebase.
 
+4. **Fixed the MD file again**: During the initial release of PyThreadFlow, we encountered an issue with the Markdown (MD) file associated with the project. However, rest assured that we have addressed this problem promptly. Our team has worked diligently to rectify the MD file, ensuring that it now functions correctly. We sincerely apologize for any inconvenience caused. With the MD file now fixed, you can proceed to enjoy PyThreadFlow V0.0.0.dev2, taking full advantage of its features and functionalities.
+
+5. **Updated the files**: We deeply regret to inform you that an incorrect version of the files was inadvertently uploaded during our previous release. We sincerely apologize for any confusion or inconvenience caused by this oversight. However, we want to assure you that we have swiftly rectified the situation. Our team has taken immediate action to update the files, ensuring that the correct version is now available for download. We understand the importance of delivering accurate and reliable software, and we appreciate your understanding and patience during this process. Thank you for your continued support as we strive to provide you with the best possible experience with PyThreadFlow.
+
 ## TODOs
 
 1. **Add functionality for the init, running, and exit calls for the threading flow manager**: The next task is to implement the necessary functionality for the initialization (`init`), running, and exit calls within the threading flow manager. This involves defining and integrating the required code to properly handle the initialization phase, manage the execution of threaded processes, and handle the clean-up and termination of threads upon program completion. Once these functionalities are in place, the threading flow manager will be able to orchestrate and control the multi-threading operations effectively.
 
 2. **Find more bugs to report**: As an ongoing process of improving the system's reliability and performance, the task of identifying and reporting bugs remains a priority. By actively searching for and documenting any existing issues or glitches in the codebase, it becomes possible to address them systematically and enhance the overall quality of the software. This task involves thorough testing, debugging, and reporting of any anomalies or unexpected behaviors encountered during the development and usage of the application. By continuously striving to find and resolve bugs, the stability and user experience of the software can be significantly improved.
```

