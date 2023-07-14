# Comparing `tmp/gptfunctionutil-0.1.7.tar.gz` & `tmp/gptfunctionutil-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptfunctionutil-0.1.7.tar", last modified: Sun Jul  9 18:06:50 2023, max compression
+gzip compressed data, was "gptfunctionutil-0.1.8.tar", last modified: Fri Jul 14 20:18:06 2023, max compression
```

## Comparing `gptfunctionutil-0.1.7.tar` & `gptfunctionutil-0.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.683763 gptfunctionutil-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.683763 gptfunctionutil-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/.github/workflows/publishpackage.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/pytest.local.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/src/gptfunctionutil/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/src/gptfunctionutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14771 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/src/gptfunctionutil/functionlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/src/gptfunctionutil/functionlib_discord.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-07-09 18:06:50.000000 gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-09 18:06:50.000000 gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:06:50.000000 gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-09 18:06:50.000000 gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-09 18:06:50.000000 gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:06:50.687763 gptfunctionutil-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-09 18:06:27.000000 gptfunctionutil-0.1.7/tests/test_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:18:06.008259 gptfunctionutil-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:18:05.996259 gptfunctionutil-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:18:06.000259 gptfunctionutil-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/.github/workflows/publishpackage.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:18:06.000259 gptfunctionutil-0.1.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-07-14 20:18:06.008259 gptfunctionutil-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 20:18:06.008259 gptfunctionutil-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:18:06.004259 gptfunctionutil-0.1.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:18:06.004259 gptfunctionutil-0.1.8/src/gptfunctionutil/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/src/gptfunctionutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/src/gptfunctionutil/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15289 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/src/gptfunctionutil/functionlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/src/gptfunctionutil/functionlib_discord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:18:06.008259 gptfunctionutil-0.1.8/src/gptfunctionutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-07-14 20:18:05.000000 gptfunctionutil-0.1.8/src/gptfunctionutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-14 20:18:05.000000 gptfunctionutil-0.1.8/src/gptfunctionutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 20:18:05.000000 gptfunctionutil-0.1.8/src/gptfunctionutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-14 20:18:05.000000 gptfunctionutil-0.1.8/src/gptfunctionutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 20:18:05.000000 gptfunctionutil-0.1.8/src/gptfunctionutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:18:06.008259 gptfunctionutil-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-14 20:17:40.000000 gptfunctionutil-0.1.8/tests/test_methods.py
```

### Comparing `gptfunctionutil-0.1.7/.github/workflows/publishpackage.yaml` & `gptfunctionutil-0.1.8/.github/workflows/publishpackage.yaml`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.7/.gitignore` & `gptfunctionutil-0.1.8/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
-
+pytest.local.ini
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
```

### Comparing `gptfunctionutil-0.1.7/.vscode/settings.json` & `gptfunctionutil-0.1.8/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.7/LICENSE` & `gptfunctionutil-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.7/PKG-INFO` & `gptfunctionutil-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptfunctionutil
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API
 Author-email: Crosswave Omega <xtream2pro@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 CrosswaveOmega
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,47 +22,49 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/CrosswaveOmega/GPT-Function-Calling-Utility
-Keywords: discord.py,OpenAI,Function Calling API
+Keywords: OpenAI,Function Calling API,GPT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: discord
 Provides-Extra: spark
 Provides-Extra: test
 License-File: LICENSE
 
 # GPT Function Calling Utility
 
-The GPT Function Calling Utility is a Python package designed to streamline the process of calling Python functions using OpenAI's Function Calling API.
+The GPT Function Calling Utility is a Python package designed to streamline the process of calling Python methods using OpenAI's Function Calling API, without wrapping around the OpenAI library.
 
 Please note that GPT Function Calling Utility does not directly make calls to OpenAI's API, but rather helps with function modeling and formatting for function invocation.
+
 ##Installation
 ```
 python -m pip install -U gptfunctionutil
 
 ```
 ## Key Features
 
-- **Simplified Function Modeling**: The package provides a straightforward way to define and format Python functions to be used with OpenAI's Function Calling API. By subclassing the `GPTFunctionLibrary` class, you can quickly create a set of callable methods to be sent alongwith calls to OpenAi's Chat Completion.
+- **Simplified Function Modeling**: This package utilizes it's `GPTFunctionLibrary` class to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint, and can then invoke methods based on the returned function_call attribute.
+
+- **Decorate Invokable Functions**: OpenAI's Function Calling Feature needs a JSON object of every single function's name, description, and parameters.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`), as well as type annotation to create this schema for functions you want to use with the API.
+  + set a display name and description with (`@AILibFunction`).  You can also specify required parameters with this decorator, but it's not required.
+  + apply small descriptions to arguments with (`@LibParam`), to inform the API on what it does.
 
-- **Decorate Invokable Functions**: OpenAI's Function Calling api needs a json schema of a functions name, description, and parameters.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`) and type annotation to create this schema for functions you want to use with the API.
-  + set a display name, description, with (`@AILibFunction`).  You can also specify required parameters with this decorator, but it's not required.
-  + apply small descriptions to arguments with (`@LibParam`).
-These decorators enable clear documentation and help streamline the function formatting process.
 
 - **Parameter Descriptions and Typing:** To ensure clarity and facilitate proper function formatting, GPT Function Calling Utility requires that all parameters intended to be passed into the AI have an applied type;  strings, integers, floats, and bools.  parameters with a default value are automatically However, the utility is capable of converting some more complex data types to and from a json schema, such as datetimes and Literals, with support for custom converters coming at a later date.
 
 - **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
    +Simply import gptfunctionutil into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
 
-- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility offers a convenient method, `mylib.get_schema()`, to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the API call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `mylib.call_by_dict(function_call)` to invoke the corresponding function with the provided arguments.
+- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)` to invoke the corresponding function with the provided arguments.
+   +The method also checks if there is a function by that name
 
 ## Usage Example
 
 Using GPT Function Calling Utility with OpenAI to get the current time:
 
 ```python
```

### Comparing `gptfunctionutil-0.1.7/README.md` & `gptfunctionutil-0.1.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # GPT Function Calling Utility
 
-The GPT Function Calling Utility is a Python package designed to streamline the process of calling Python functions using OpenAI's Function Calling API.
+The GPT Function Calling Utility is a Python package designed to streamline the process of calling Python methods using OpenAI's Function Calling API, without wrapping around the OpenAI library.
 
 Please note that GPT Function Calling Utility does not directly make calls to OpenAI's API, but rather helps with function modeling and formatting for function invocation.
+
 ##Installation
 ```
 python -m pip install -U gptfunctionutil
 
 ```
 ## Key Features
 
-- **Simplified Function Modeling**: The package provides a straightforward way to define and format Python functions to be used with OpenAI's Function Calling API. By subclassing the `GPTFunctionLibrary` class, you can quickly create a set of callable methods to be sent alongwith calls to OpenAi's Chat Completion.
+- **Simplified Function Modeling**: This package utilizes it's `GPTFunctionLibrary` class to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint, and can then invoke methods based on the returned function_call attribute.
+
+- **Decorate Invokable Functions**: OpenAI's Function Calling Feature needs a JSON object of every single function's name, description, and parameters.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`), as well as type annotation to create this schema for functions you want to use with the API.
+  + set a display name and description with (`@AILibFunction`).  You can also specify required parameters with this decorator, but it's not required.
+  + apply small descriptions to arguments with (`@LibParam`), to inform the API on what it does.
 
-- **Decorate Invokable Functions**: OpenAI's Function Calling api needs a json schema of a functions name, description, and parameters.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`) and type annotation to create this schema for functions you want to use with the API.
-  + set a display name, description, with (`@AILibFunction`).  You can also specify required parameters with this decorator, but it's not required.
-  + apply small descriptions to arguments with (`@LibParam`).
-These decorators enable clear documentation and help streamline the function formatting process.
 
 - **Parameter Descriptions and Typing:** To ensure clarity and facilitate proper function formatting, GPT Function Calling Utility requires that all parameters intended to be passed into the AI have an applied type;  strings, integers, floats, and bools.  parameters with a default value are automatically However, the utility is capable of converting some more complex data types to and from a json schema, such as datetimes and Literals, with support for custom converters coming at a later date.
 
 - **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
    +Simply import gptfunctionutil into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
 
-- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility offers a convenient method, `mylib.get_schema()`, to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the API call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `mylib.call_by_dict(function_call)` to invoke the corresponding function with the provided arguments.
+- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)` to invoke the corresponding function with the provided arguments.
+   +The method also checks if there is a function by that name
 
 ## Usage Example
 
 Using GPT Function Calling Utility with OpenAI to get the current time:
 
 ```python
```

### Comparing `gptfunctionutil-0.1.7/pyproject.toml` & `gptfunctionutil-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 [project]
 name = 'gptfunctionutil'
-version = "0.1.7"
+version = "0.1.8"
 license = {file = "LICENSE"}
 authors = [{name="Crosswave Omega",email= "xtream2pro@gmail.com"}]
 description = "A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API"
 readme = 'README.md'
 
-keywords = ['discord.py', 'OpenAI', 'Function Calling API']
+keywords = ['OpenAI', 'Function Calling API', 'GPT']
 requires-python = '>=3.10'
 
 [project.urls]
 "Homepage"= "https://github.com/CrosswaveOmega/GPT-Function-Calling-Utility"
 
 
 [options.packages.find]
```

### Comparing `gptfunctionutil-0.1.7/src/gptfunctionutil/__init__.py` & `gptfunctionutil-0.1.8/src/gptfunctionutil/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 from __future__ import annotations
 
 __version__ = "0.1.7"
 import importlib.util
 
+from .errors import *
 discord_install = importlib.util.find_spec("discord")
 if discord_install is not None:
     try:
         import discord
         from .functionlib_discord import LibCommandDisc as LibCommand
         from .functionlib_discord import GPTFunctionLibraryDisc as GPTFunctionLibrary
         from .functionlib_discord import AILibFunction
```

### Comparing `gptfunctionutil-0.1.7/src/gptfunctionutil/functionlib.py` & `gptfunctionutil-0.1.8/src/gptfunctionutil/functionlib.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import re
 from typing import Any, Coroutine, Dict, List, Union
 
 from enum import Enum, EnumMeta
 
 from datetime import datetime
 
+from .errors import *
 
 
 class CommandSingleton:
     _instance = None
     _commands = {}
 
     @classmethod
@@ -245,17 +246,16 @@
             return re.sub(expression_detect_pattern, lambda m: self.my_math_parser(m.group()), function_args)
         return function_args
 
     def parse_name_args(self, function_dict: Dict[str, Any]) -> Dict[str, Any]:
         '''parse the args within function_dict, and apply any needed corrections to the JSON.'''
         print(function_dict)
         function_name = function_dict.get('name')
+        function_args = function_dict.get('arguments', None)
         if function_name in self.FunctionDict:
-            method=self.FunctionDict[function_name]
-            function_args = function_dict.get('arguments', None)
             if isinstance(function_args,str):
                 #Making it so it won't break on poorly formatted function arguments.
                 function_args=function_args.replace("\\n",'\n')
                 quoteescapefixpattern = r"(?<=:\s\")(.*?)(?=\"(?:,|\s*\}))"
                 #In testing, I once had the API return a poorly escaped function_args attribute
                 #That could not be parsed by json.loads, so hence this regex.
                 function_args_str=re.sub(quoteescapefixpattern, lambda m: m.group().replace('"', r'\"'), function_args)
@@ -265,24 +265,29 @@
                 function_args_str=self.expression_match(function_args_str)
                 print(function_args_str)
                 try:
                     function_args=json.loads(function_args_str, strict=False)
                 except json.JSONDecodeError as e:
                     #Something went wrong while parsing, return where.
                     output=f"JSONDecodeError: {e.msg} at line {e.lineno} column {e.colno}: `{function_args_str[e.pos]}`"
-                    raise json.JSONDecodeError(msg=f"{output}\n{function_args_str}", doc=function_args_str,pos=1)
+                    raise ArgDecodeError(function_name=function_name,arguments=function_args_str,msg=f"{output}", er=e)
             return function_name,function_args
-        raise Exception(f"Function '{function_name}' not found.")
+        raise FunctionNotFound(function_name=function_name,arguments=function_args)
 
     def convert_args(self, function_name:str, function_args:Dict[str, Any]) -> Dict[str, Any]:
         '''Preform any needed conversion of the function arguments.'''
         libmethod=self.FunctionDict[function_name]
         return libmethod.convert_args(function_args)
 
-
+    def default_callback(self,function_name:str,function_args:str="NONE")->str:
+        '''This is called whenever an invalid function is called.'''
+        output=f"{function_name} is not a valid function."
+        function_args=function_args.replace("\\n",'\n')
+        output+="\n```{function_args}```"
+        return output
     def call_by_dict(self, function_dict: Dict[str, Any]) -> Any:
         """
         Call a function based on the provided dictionary.
 
         Args:
             function_dict (Dict[str, Any]): The dictionary containing the function name and arguments.
 
@@ -290,15 +295,19 @@
             The result of the function call.
 
         Raises:
             AttributeError: If the function name is not found or not callable.
         """
         try:
             function_name,function_args=self.parse_name_args(function_dict)
-        except Exception as e:
+        except GPTLibError as e:
+            if isinstance(e, FunctionNotFound):
+                '''Invoke a default function so something is returned...'''
+                return self.default_callback(e.function_name,e.arguments)
+
             result=str(e)
             return result
         libmethod = self.FunctionDict.get(function_name)
         if libmethod.comm_type=='callable':
             if len(function_args)>0:
                 #for i, v in function_args.items():
                 #    print("st",i,v)
```

### Comparing `gptfunctionutil-0.1.7/src/gptfunctionutil/functionlib_discord.py` & `gptfunctionutil-0.1.8/src/gptfunctionutil/functionlib_discord.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Command,
     Context,
     Bot,
     CommandNotFound,
     CheckFailure
 )
 from .functionlib import GPTFunctionLibrary, LibCommand
-
+from .errors import *
 class CommandSingleton:
     _instance = None
     _commands = {}
 
     @classmethod
     def get_instance(cls):
         if not cls._instance:
@@ -237,15 +237,18 @@
             This is so something can be added to the bot's message_chain.
 
         Raises:
             AttributeError: If the function name is not found or not callable.
         """
         try:
             function_name,function_args=self.parse_name_args(function_dict)
-        except Exception as e:
+        except GPTLibError as e:
+            if isinstance(e, FunctionNotFound):
+                return self.default_callback(e.function_name,e.arguments)
+
             result=str(e)
             return result
         print(function_name, function_args,len(function_args))
         libmethod = self.FunctionDict.get(function_name)
         if libmethod.comm_type=='command':
             return await libmethod.invoke_command(ctx, function_args)
```

### Comparing `gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/PKG-INFO` & `gptfunctionutil-0.1.8/src/gptfunctionutil.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptfunctionutil
-Version: 0.1.7
+Version: 0.1.8
 Summary: A simple package for the purpose of providing a set of utilities that make it easier to invoke python methods and discord.py commands with the OpenAI Function Calling API
 Author-email: Crosswave Omega <xtream2pro@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 CrosswaveOmega
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,47 +22,49 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/CrosswaveOmega/GPT-Function-Calling-Utility
-Keywords: discord.py,OpenAI,Function Calling API
+Keywords: OpenAI,Function Calling API,GPT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: discord
 Provides-Extra: spark
 Provides-Extra: test
 License-File: LICENSE
 
 # GPT Function Calling Utility
 
-The GPT Function Calling Utility is a Python package designed to streamline the process of calling Python functions using OpenAI's Function Calling API.
+The GPT Function Calling Utility is a Python package designed to streamline the process of calling Python methods using OpenAI's Function Calling API, without wrapping around the OpenAI library.
 
 Please note that GPT Function Calling Utility does not directly make calls to OpenAI's API, but rather helps with function modeling and formatting for function invocation.
+
 ##Installation
 ```
 python -m pip install -U gptfunctionutil
 
 ```
 ## Key Features
 
-- **Simplified Function Modeling**: The package provides a straightforward way to define and format Python functions to be used with OpenAI's Function Calling API. By subclassing the `GPTFunctionLibrary` class, you can quickly create a set of callable methods to be sent alongwith calls to OpenAi's Chat Completion.
+- **Simplified Function Modeling**: This package utilizes it's `GPTFunctionLibrary` class to define sets of callable methods to be sent to OpenAI's Chat Completion endpoint, and can then invoke methods based on the returned function_call attribute.
+
+- **Decorate Invokable Functions**: OpenAI's Function Calling Feature needs a JSON object of every single function's name, description, and parameters.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`), as well as type annotation to create this schema for functions you want to use with the API.
+  + set a display name and description with (`@AILibFunction`).  You can also specify required parameters with this decorator, but it's not required.
+  + apply small descriptions to arguments with (`@LibParam`), to inform the API on what it does.
 
-- **Decorate Invokable Functions**: OpenAI's Function Calling api needs a json schema of a functions name, description, and parameters.  This utility uses two decorators, (`@AILibFunction`) and (`@LibParam`) and type annotation to create this schema for functions you want to use with the API.
-  + set a display name, description, with (`@AILibFunction`).  You can also specify required parameters with this decorator, but it's not required.
-  + apply small descriptions to arguments with (`@LibParam`).
-These decorators enable clear documentation and help streamline the function formatting process.
 
 - **Parameter Descriptions and Typing:** To ensure clarity and facilitate proper function formatting, GPT Function Calling Utility requires that all parameters intended to be passed into the AI have an applied type;  strings, integers, floats, and bools.  parameters with a default value are automatically However, the utility is capable of converting some more complex data types to and from a json schema, such as datetimes and Literals, with support for custom converters coming at a later date.
 
 - **Integration with Discord.py**: This utility was intended to be used with life as a discord.py utility, and can be easily integrated with discord.py bots.
    +Simply import gptfunctionutil into your Discord bot project, and decorate your commands with `@LibParam` and `@AILibFunction`.  After passing the Commands into a GPTFunctionLibrary subclass with  `add_in_commands(your_bot_object_here)`, your bot commands will become invokable in the same way as a decorated GPTFunctionLibrary method.
 
-- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility offers a convenient method, `mylib.get_schema()`, to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the API call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `mylib.call_by_dict(function_call)` to invoke the corresponding function with the provided arguments.
+- **Schema Generation for API Calls**: Before making a call to the OpenAI chat/completion endpoint, the utility has a `get_schema()` method to extract the formatted functions as a list of dictionaries. This schema is then passed as the `functions` field in the ChatCompletion call. If the AI determines that it should invoke a function call, the returned `function_call` dictionary is used with `call_by_dict(function_call)` to invoke the corresponding function with the provided arguments.
+   +The method also checks if there is a function by that name
 
 ## Usage Example
 
 Using GPT Function Calling Utility with OpenAI to get the current time:
 
 ```python
```

### Comparing `gptfunctionutil-0.1.7/src/gptfunctionutil.egg-info/SOURCES.txt` & `gptfunctionutil-0.1.8/src/gptfunctionutil.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 .gitattributes
 .gitignore
 LICENSE
 README.md
 pyproject.toml
-pytest.local.ini
 .github/workflows/publishpackage.yaml
 .vscode/settings.json
 src/README.md
 src/gptfunctionutil/__init__.py
+src/gptfunctionutil/errors.py
 src/gptfunctionutil/functionlib.py
 src/gptfunctionutil/functionlib_discord.py
 src/gptfunctionutil.egg-info/PKG-INFO
 src/gptfunctionutil.egg-info/SOURCES.txt
 src/gptfunctionutil.egg-info/dependency_links.txt
 src/gptfunctionutil.egg-info/requires.txt
 src/gptfunctionutil.egg-info/top_level.txt
```

### Comparing `gptfunctionutil-0.1.7/tests/conftest.py` & `gptfunctionutil-0.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gptfunctionutil-0.1.7/tests/test_methods.py` & `gptfunctionutil-0.1.8/tests/test_methods.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,7 +23,26 @@
     assert 'name' in schema[0]
     assert schema[0]['name'] == 'get_time'
 
     result=testlib.call_by_dict({'name':'get_time','arguments':"{\"comment\":\"This is an interesting, amusing remark.\"}"})
     assert result == "This is an interesting, amusing remark."
 
 
+import pytest
+@pytest.mark.asyncio
+async def test_command_function_errorsload():
+    class MyTestLib(GPTFunctionLibrary):
+        @AILibFunction(name='get_time',description='Get the current time and day in UTC.')
+        @LibParam(comment='An interesting, amusing remark.')
+        def get_time(self,comment:str):
+            #This is an example of a decorated coroutine command.
+            return f"{comment}"
+    #pass
+    testlib=MyTestLib()
+    schema = testlib.get_schema()
+    assert 'name' in schema[0]
+    assert schema[0]['name'] == 'get_time'
+
+    result=testlib.call_by_dict({'name':'notafunction','arguments':"{\"comment\":\"This is an interesting, amusing remark.\"}"})
+    assert 'is not a valid function' in result
+
+
```

