# Comparing `tmp/litechain-0.1.1.tar.gz` & `tmp/litechain-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litechain-0.1.1.tar", last modified: Mon Jul 10 20:37:05 2023, max compression
+gzip compressed data, was "litechain-0.1.2.tar", last modified: Fri Jul 14 08:20:18 2023, max compression
```

## Comparing `litechain-0.1.1.tar` & `litechain-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:37:05.315293 litechain-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-10 20:36:54.000000 litechain-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-10 20:36:54.000000 litechain-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-10 20:37:05.315293 litechain-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-10 20:36:54.000000 litechain-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:37:05.315293 litechain-0.1.1/litechain/
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-10 20:36:54.000000 litechain-0.1.1/litechain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:37:05.315293 litechain-0.1.1/litechain/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-10 20:36:54.000000 litechain-0.1.1/litechain/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:37:05.315293 litechain-0.1.1/litechain/contrib/llms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:54.000000 litechain-0.1.1/litechain/contrib/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-10 20:36:54.000000 litechain-0.1.1/litechain/contrib/llms/gpt4all_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15096 2023-07-10 20:36:54.000000 litechain-0.1.1/litechain/contrib/llms/open_ai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:37:05.315293 litechain-0.1.1/litechain/contrib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:54.000000 litechain-0.1.1/litechain/contrib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-10 20:36:54.000000 litechain-0.1.1/litechain/contrib/utils/open_ai_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:37:05.315293 litechain-0.1.1/litechain/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:54.000000 litechain-0.1.1/litechain/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20678 2023-07-10 20:36:54.000000 litechain-0.1.1/litechain/core/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:37:05.315293 litechain-0.1.1/litechain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:54.000000 litechain-0.1.1/litechain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-10 20:36:54.000000 litechain-0.1.1/litechain/utils/async_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-10 20:36:54.000000 litechain-0.1.1/litechain/utils/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:37:05.315293 litechain-0.1.1/litechain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-10 20:37:05.000000 litechain-0.1.1/litechain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-10 20:37:05.000000 litechain-0.1.1/litechain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 20:37:05.000000 litechain-0.1.1/litechain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 20:37:05.000000 litechain-0.1.1/litechain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 20:37:05.000000 litechain-0.1.1/litechain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-10 20:36:54.000000 litechain-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 20:37:05.315293 litechain-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-10 20:36:54.000000 litechain-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 20:37:05.315293 litechain-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 20:36:54.000000 litechain-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.640052 litechain-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 08:20:02.000000 litechain-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 08:20:02.000000 litechain-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-14 08:20:18.640052 litechain-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-14 08:20:02.000000 litechain-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.636052 litechain-0.1.2/litechain/
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.636052 litechain-0.1.2/litechain/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.640052 litechain-0.1.2/litechain/contrib/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/contrib/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/contrib/llms/gpt4all_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/contrib/llms/open_ai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.640052 litechain-0.1.2/litechain/contrib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/contrib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/contrib/utils/open_ai_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.640052 litechain-0.1.2/litechain/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20678 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/core/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.640052 litechain-0.1.2/litechain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/utils/async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/utils/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.636052 litechain-0.1.2/litechain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-14 08:20:18.000000 litechain-0.1.2/litechain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-14 08:20:18.000000 litechain-0.1.2/litechain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:20:18.000000 litechain-0.1.2/litechain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-14 08:20:18.000000 litechain-0.1.2/litechain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 08:20:18.000000 litechain-0.1.2/litechain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 08:20:02.000000 litechain-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 08:20:18.640052 litechain-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-14 08:20:02.000000 litechain-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.640052 litechain-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:02.000000 litechain-0.1.2/tests/__init__.py
```

### Comparing `litechain-0.1.1/LICENSE` & `litechain-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `litechain-0.1.1/PKG-INFO` & `litechain-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litechain
-Version: 0.1.1
+Version: 0.1.2
 Summary: Build robust LLM applications with true composability 🔗
 Home-page: https://github.com/rogeriochaves/litechain
 Author: Rogerio Chaves
 Author-email: rogeriocfj@gmail.com
 License: MIT
 Project-URL: Documentation, https://rogeriochaves.github.io/litechain/
 Project-URL: Source Code, https://github.com/rogeriochaves/litechain
```

### Comparing `litechain-0.1.1/README.md` & `litechain-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `litechain-0.1.1/litechain/__init__.py` & `litechain-0.1.2/litechain/__init__.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.1/litechain/contrib/__init__.py` & `litechain-0.1.2/litechain/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.1/litechain/contrib/llms/gpt4all_chain.py` & `litechain-0.1.2/litechain/contrib/llms/gpt4all_chain.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.1/litechain/contrib/llms/open_ai.py` & `litechain-0.1.2/litechain/contrib/llms/open_ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,21 +99,28 @@
     OpenAIChatMessage is a data class that represents a chat message for building `OpenAIChatChain` prompt.
 
     Attributes
     ----------
     role : Literal["system", "user", "assistant", "function"]
         The role of who sent this message in the chat, can be one of `"system"`, `"user"`, `"assistant"` or "function"
 
+    name: Optional[str]
+        The name is used for when `role` is `"function"`, it represents the name of the function that was called
+
     content : str
         A string with the full content of what the given role said
 
     """
 
     role: Literal["system", "user", "assistant", "function"]
     content: str
+    name: Optional[str] = None
+
+    def to_dict(self):
+        return {k: v for k, v in self.__dict__.items() if v is not None}
 
 
 @dataclass
 class _OpenAIFunctionCall:
     name: str
     arguments: str
 
@@ -126,31 +133,46 @@
     Attributes
     ----------
     role : Optional[Literal["assistant", "function"]]
         The role of the output message, the first message will have the role, while
         the subsequent partial content output ones will have the role as `None`.
         For now the only possible values it will have is either None or `"assistant"`
 
+    name: Optional[str]
+        The name is used for when `role` is `"function"`, it represents the name of the function that was called
+
     content : str
         A string with the partial content being outputted by the LLM, this generally
         translate to each token the LLM is producing
 
     """
 
     role: Optional[Literal["assistant", "function"]]
     content: str
+    name: Optional[str] = None
 
     def __chain_debug__(self):
         if self.role is not None:
             print(f"{Fore.YELLOW}{self.role.capitalize()}:{Fore.RESET} ", end="")
-        print(
-            self.content,
-            end="",
-            flush=True,
-        )
+        if self.role == "function":
+            arguments = json.loads(self.content)
+            stringified_keywords_list = ", ".join(
+                [f"{k}={repr(v)}" for k, v in arguments.items()]
+            )
+            print(
+                f"{self.name}({stringified_keywords_list})",
+                end="",
+                flush=True,
+            )
+        else:
+            print(
+                self.content,
+                end="",
+                flush=True,
+            )
 
 
 class OpenAIChatChain(Chain[T, U]):
     """
     `OpenAIChatChain` gives you access to the more powerful LLMs from OpenAI, like `gpt-3.5-turbo` and `gpt-4`, they are structured in a chat format with roles.
 
     The `OpenAIChatChain` takes a lambda function that should return a list of `OpenAIChatMessage` for the assistant to reply, it is stateless, so it doesn't keep
@@ -276,15 +298,15 @@
                 if functions is not None:
                     function_kwargs["functions"] = openai_functions
                 if function_call is not None:
                     function_kwargs["function_call"] = function_call
 
                 return openai.ChatCompletion.create(
                     model=model,
-                    messages=[m.__dict__ for m in messages],
+                    messages=[m.to_dict() for m in messages],
                     temperature=temperature,
                     stream=True,
                     max_tokens=max_tokens,
                     **function_kwargs,
                 )
 
             completions = await loop.run_in_executor(None, get_completions)
@@ -369,21 +391,19 @@
         pending_function_calls: List[_OpenAIFunctionCall],
     ) -> AsyncGenerator[ChainOutput, None]:
         for function_call in pending_function_calls:
             function_to_call = name_to_function[function_call.name]
             arguments = json.loads(function_call.arguments)
             output_chain_name = f"{self.name}@function_call->{function_call.name}"
 
-            stringified_keywords_list = ", ".join(
-                [f"{k}={repr(v)}" for k, v in arguments.items()]
-            )
             yield self._output_wrap(
                 OpenAIChatDelta(
                     role="function",
-                    content=f"{function_call.name}({stringified_keywords_list})",
+                    name=function_call.name,
+                    content=function_call.arguments,
                 ),
                 final=False,
             )
 
             result = function_to_call(**arguments)
             wrapped = self._wrap(result, name=output_chain_name)
             async for output in wrapped:
```

### Comparing `litechain-0.1.1/litechain/contrib/utils/open_ai_functions.py` & `litechain-0.1.2/litechain/contrib/utils/open_ai_functions.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.1/litechain/core/chain.py` & `litechain-0.1.2/litechain/core/chain.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.1/litechain/utils/async_generator.py` & `litechain-0.1.2/litechain/utils/async_generator.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.1/litechain/utils/chain.py` & `litechain-0.1.2/litechain/utils/chain.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.1/litechain.egg-info/PKG-INFO` & `litechain-0.1.2/litechain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litechain
-Version: 0.1.1
+Version: 0.1.2
 Summary: Build robust LLM applications with true composability 🔗
 Home-page: https://github.com/rogeriochaves/litechain
 Author: Rogerio Chaves
 Author-email: rogeriocfj@gmail.com
 License: MIT
 Project-URL: Documentation, https://rogeriochaves.github.io/litechain/
 Project-URL: Source Code, https://github.com/rogeriochaves/litechain
```

### Comparing `litechain-0.1.1/litechain.egg-info/SOURCES.txt` & `litechain-0.1.2/litechain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `litechain-0.1.1/setup.py` & `litechain-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="litechain",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=requirements,
     author="Rogerio Chaves",
     author_email="rogeriocfj@gmail.com",
     description="Build robust LLM applications with true composability 🔗",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

