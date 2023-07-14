# Comparing `tmp/promptwatch-0.2.4.tar.gz` & `tmp/promptwatch-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.2.4.tar", last modified: Tue Jun 13 21:09:55 2023, max compression
+gzip compressed data, was "promptwatch-0.2.5.tar", last modified: Fri Jul 14 21:46:30 2023, max compression
```

## Comparing `promptwatch-0.2.4.tar` & `promptwatch-0.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 21:09:55.235713 promptwatch-0.2.4/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-06-13 21:09:55.235532 promptwatch-0.2.4/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.4/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.4/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-13 21:09:55.235907 promptwatch-0.2.4/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.4/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 21:09:55.227377 promptwatch-0.2.4/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 21:09:55.230923 promptwatch-0.2.4/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-06-13 21:07:34.000000 promptwatch-0.2.4/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-05-31 21:34:19.000000 promptwatch-0.2.4/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.4/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.4/src/promptwatch/constants.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5281 2023-06-12 19:17:03.000000 promptwatch-0.2.4/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.4/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 21:09:55.233983 promptwatch-0.2.4/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.4/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12414 2023-05-31 20:26:52.000000 promptwatch-0.2.4/src/promptwatch/langchain/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    30554 2023-06-13 19:09:53.000000 promptwatch-0.2.4/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.4/src/promptwatch/langchain/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    17902 2023-06-12 10:33:52.000000 promptwatch-0.2.4/src/promptwatch/promptwatch_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 21:09:55.235004 promptwatch-0.2.4/src/promptwatch/unit_tests/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.4/src/promptwatch/unit_tests/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.4/src/promptwatch/unit_tests/evaluation.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.4/src/promptwatch/unit_tests/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.4/src/promptwatch/unit_tests/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1105 2023-05-24 13:30:08.000000 promptwatch-0.2.4/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 21:09:55.232277 promptwatch-0.2.4/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-06-13 21:09:55.000000 promptwatch-0.2.4/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-06-13 21:09:55.000000 promptwatch-0.2.4/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-13 21:09:55.000000 promptwatch-0.2.4/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.4/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-06-13 21:09:55.000000 promptwatch-0.2.4/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-06-13 21:09:55.000000 promptwatch-0.2.4/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-14 21:46:30.647209 promptwatch-0.2.5/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-07-14 21:46:30.647000 promptwatch-0.2.5/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.5/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.5/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-07-14 21:46:30.647261 promptwatch-0.2.5/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.5/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-14 21:46:30.635634 promptwatch-0.2.5/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-14 21:46:30.637903 promptwatch-0.2.5/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-07-14 21:46:22.000000 promptwatch-0.2.5/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-05-31 21:34:19.000000 promptwatch-0.2.5/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.5/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.5/src/promptwatch/constants.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5282 2023-07-14 21:41:17.000000 promptwatch-0.2.5/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.5/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-14 21:46:30.642052 promptwatch-0.2.5/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.5/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12414 2023-05-31 20:26:52.000000 promptwatch-0.2.5/src/promptwatch/langchain/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    31317 2023-07-14 21:31:59.000000 promptwatch-0.2.5/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.5/src/promptwatch/langchain/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    18104 2023-06-15 22:09:53.000000 promptwatch-0.2.5/src/promptwatch/promptwatch_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-14 21:46:30.645444 promptwatch-0.2.5/src/promptwatch/unit_tests/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.5/src/promptwatch/unit_tests/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.5/src/promptwatch/unit_tests/evaluation.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.5/src/promptwatch/unit_tests/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.5/src/promptwatch/unit_tests/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2368 2023-06-17 16:42:18.000000 promptwatch-0.2.5/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-14 21:46:30.640329 promptwatch-0.2.5/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-07-14 21:46:30.000000 promptwatch-0.2.5/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-07-14 21:46:30.000000 promptwatch-0.2.5/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-07-14 21:46:30.000000 promptwatch-0.2.5/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.5/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-07-14 21:46:30.000000 promptwatch-0.2.5/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-07-14 21:46:30.000000 promptwatch-0.2.5/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.2.4/PKG-INFO` & `promptwatch-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.4
+Version: 0.2.5
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.4/README.md` & `promptwatch-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.4/setup.py` & `promptwatch-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.4/src/promptwatch/caching.py` & `promptwatch-0.2.5/src/promptwatch/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.4/src/promptwatch/client.py` & `promptwatch-0.2.5/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.4/src/promptwatch/data_model.py` & `promptwatch-0.2.5/src/promptwatch/data_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,15 @@
     format:Optional[str]
     
 class ChatMessage(BaseModel):
     """ Explicit chat message used as a parameter value for chat history or template"""
     role:Optional[str]
     text:str
 
+
 class ChatMessagePromptTemplate(PromptTemplateDescription):
     role:Optional[str]
     
     
 class NamedPromptTemplateDescription(PromptTemplateDescription):
     template_name:str
     template_version:Optional[str]
```

### Comparing `promptwatch-0.2.4/src/promptwatch/decorators.py` & `promptwatch-0.2.5/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.4/src/promptwatch/langchain/caching.py` & `promptwatch-0.2.5/src/promptwatch/langchain/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.4/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.2.5/src/promptwatch/langchain/langchain_support.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 from langchain.llms.base import LLM
 from langchain.chat_models.base import BaseChatModel
 from langchain.chains import LLMChain
 from langchain.embeddings.base import Embeddings
 from langchain.schema import HumanMessage, ChatMessage as LangChainChatMessage, AIMessage, SystemMessage, BaseMessage 
 from langchain.prompts import ChatMessagePromptTemplate as LangChainChatMessagePromptTemplate
 from langchain.callbacks.base import BaseCallbackHandler
-from langchain.agents import initialize_agent, Tool, Agent, BaseSingleActionAgent
+from langchain.agents import Tool, Agent, BaseSingleActionAgent
 from langchain.tools.base import BaseTool
 from langchain.chains.base import Chain
 
 from langchain.schema import AgentAction, AgentFinish, LLMResult,  Document
 from ..client import Client
 from ..data_model import NamedPromptTemplateDescription,PromptTemplateDescription, LlmPrompt, ParallelPrompt, ChainSequence, ChatMessage, Answer, Action, Question, RetrievedDocuments, DocumentSnippet, ChatMessagePromptTemplate
-from ..utils import find_the_caller_in_the_stack, is_primitive_type, wrap_a_method
+from ..utils import find_the_caller_in_the_stack, wrap_a_method, copy_dict_serializable_values
 from .caching import CachedLLM, CachedChatLLM
 from ..decorators import FORMATTED_PROMPT_CONTEXT_KEY, TEMPLATE_NAME_CONTEXT_KEY, LLM_CHAIN_CONTEXT_KEY
 
 from typing import List, Dict
 from ..promptwatch_context import PromptWatch, ContextTrackerSingleton
 
 
@@ -139,66 +139,68 @@
 
     def reverse_monkey_patching(self):
         for func in self.monkey_patched_functions:
             #TODO: .. we should restore the state of the things as were before...
             pass
             
         
-    def on_chat_model_start(
+    async def on_chat_model_start(
         self,
         serialized: Dict[str, Any],
         messages: List[List[BaseMessage]],
         *,
         run_id,
         parent_run_id = None,
         **kwargs: Any,
     ) -> Any:
-        self.on_llm_start(serialized, messages, run_id=run_id, parent_run_id=parent_run_id, **kwargs)
+        await self.on_llm_start(serialized, messages, run_id=run_id, parent_run_id=parent_run_id, **kwargs)
     
 
-    def on_llm_start(
+    async  def on_llm_start(
         self, serialized: Dict[str, Any], prompts: List[str, List[BaseMessage]], **kwargs: Any
     ) -> Any:
         """Run when LLM starts running."""
 
         prompt_template = None
         prompt_input_values=None
         llm_info=None
         info_message=None
         formatted_prompt=None
 
-        
+        if prompts and prompts[0] and isinstance(prompts[0][0],BaseMessage):
+            prompts=[convert_chat_messages(prompts_set) for prompts_set in prompts]
 
         current_llm_chain:LLMChain= self.prompt_watch.get_context(LLM_CHAIN_CONTEXT_KEY)
 
         template_name = self.prompt_watch.get_context(TEMPLATE_NAME_CONTEXT_KEY)
         if template_name:
             prompt_template = PromptWatch.prompt_template_register_cache.get(template_name)
             
         # this should ensure that all the additional data is available in the context
+        llm_info = kwargs.get("invocation_params")  
         if current_llm_chain:
             if current_llm_chain.llm and current_llm_chain.llm.dict:
                 llm = current_llm_chain.llm
                 if hasattr(current_llm_chain.llm,"inner_llm"): # cachedLLM
                     llm = llm.inner_llm
-                llm_info = {k:v for k,v in llm.dict().items() if is_primitive_type(v)}
+                llm_info = copy_dict_serializable_values(llm.dict())
                 llm_info["stop"] = self.prompt_watch.current_activity.inputs.get("stop")
             # lets try to retrieve registered named template first... it's faster
             
 
             if not prompt_template:
                 # lets create anonymous prompt template description
                 prompt_template = create_prompt_template_description(current_llm_chain.prompt)
 
             prompt_input_values = self.prompt_watch.current_activity.inputs
 
             formatted_prompt = self.prompt_watch.get_context(FORMATTED_PROMPT_CONTEXT_KEY)
 
             
-            if prompts and prompts[0] and isinstance(prompts[0][0],LangChainChatMessage):
+            if prompts and prompts[0] and isinstance(prompts[0][0],BaseMessage):
                 
                 prompts=[convert_chat_messages(prompts_set) for prompts_set in prompts]
             # this is probably unnecessary now, but keeping it for now
             elif isinstance(current_llm_chain.prompt,ChatPromptTemplate):
                 if not formatted_prompt:
                     # we need to reformat the prompt so we can get the original values, not the strings
                     formatted_prompt = current_llm_chain.prep_prompts([prompt_input_values])[0][0]
@@ -254,60 +256,66 @@
                     info_message=info_message,
                 )
             )
 
 
 
     
-    def on_llm_new_token(self, token: str, **kwargs: Any) -> Any:
+    async  def on_llm_new_token(self, token: str, **kwargs: Any) -> Any:
         """Run on new LLM token. Only available when streaming is enabled."""
         pass
 
     
-    def on_llm_end(self, response: LLMResult, **kwargs: Any) -> Any:
+    async def on_llm_end(self, response: LLMResult, **kwargs: Any) -> Any:
         """Run when LLM ends running."""
         if len(response.generations)>1:
             prompts =  self.prompt_watch.current_activity.prompts
         else:
             prompts=[self.prompt_watch.current_activity]
         
         
         if not self.prompt_watch.current_activity.metadata:
             self.prompt_watch.current_activity.metadata={}
 
         for prompt, generated_responses in zip(prompts, response.generations):
             prompt.generated = "\n---\n".join([resp.text for resp in generated_responses])
             prompt.metadata["generation_info"] = [resp.generation_info for resp in generated_responses] if len(generated_responses)>1 else generated_responses[0].generation_info
+            
+            if generated_responses and getattr(generated_responses[0],"message",None):
+                function_calls= [resp.message.additional_kwargs.get("function_call") for resp in generated_responses] 
+
+                prompt.metadata["function_call"] = function_calls if len(function_calls)>1 else function_calls[0]
+            
 
         if response.llm_output is not None:
             self.prompt_watch.current_activity.metadata["llm_output"]=response.llm_output
             token_usage= response.llm_output.get("token_usage")
             if token_usage and isinstance(token_usage,dict):
                 total_tokens = token_usage.get("total_tokens")
                 
                 if total_tokens:
                     self.prompt_watch.current_activity.metadata["total_tokens"] = self.prompt_watch.current_activity.metadata.get("total_tokens",0)+ token_usage["total_tokens"]
         self.prompt_watch._close_current_activity()
 
         
 
     
-    def on_llm_error(
+    async def on_llm_error(
         self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when LLM errors."""
         self.prompt_watch._on_error(error, kwargs)
 
     
-    def on_chain_start(
+    async def on_chain_start(
         self, serialized: Dict[str, Any], inputs: Dict[str, Any], **kwargs: Any
     ) -> Any:
         """Run when chain starts running."""
         
-        if "LLM" in serialized.get("name","") :
+        if "LLM" in serialized.get("name","") or "LLM" in ".".join(serialized.get("id",[])) :
             current_llm_chain = find_the_caller_in_the_stack(serialized["name"])
             self.prompt_watch.add_context(LLM_CHAIN_CONTEXT_KEY,current_llm_chain)
 
         self.try_get_retrieved_documents(inputs)
                   
 
 
@@ -349,20 +357,20 @@
                 docs.append(DocumentSnippet(
                     text=doc.page_content, 
                     source=source,
                     metadata=metadata if metadata else None # to not pass empty objects
                     ))
             self.prompt_watch._add_activity(RetrievedDocuments(documents=docs))
     
-    def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> Any:
+    async  def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> Any:
         """Run when chain ends running."""
         
         
         self.prompt_watch._remove_context(LLM_CHAIN_CONTEXT_KEY)
-            
+        outputs = copy_dict_serializable_values(outputs)
         self.prompt_watch.current_activity.outputs=outputs
         if outputs.get("answer"):
             self.prompt_watch._add_activity(Answer(text=outputs["answer"]),as_root=True)
         if kwargs:
             self.prompt_watch.current_activity.metadata["output_kwargs"]=kwargs
         
         if "total_tokens" in self.prompt_watch.current_activity.metadata and len(self.prompt_watch.chain_hierarchy)>1:
@@ -371,61 +379,61 @@
                 parent_activity.metadata={"total_tokens":self.prompt_watch.current_activity.metadata["total_tokens"]}
             else:
                 parent_activity.metadata["total_tokens"] = parent_activity.metadata.get("total_tokens",0)+ self.prompt_watch.current_activity.metadata["total_tokens"]
         
         self.prompt_watch._close_current_activity()
 
     
-    def on_chain_error(
+    async  def on_chain_error(
         self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when chain errors."""
         self.prompt_watch._on_error(error, kwargs)
 
     
-    def on_tool_start(
+    async def on_tool_start(
         self, serialized: Dict[str, Any], input_str: str, **kwargs: Any
     ) -> Any:
         """Run when tool starts running."""
         self.prompt_watch._open_activity(
                 Action(tool_type=serialized.get("name") or "undefined", input=input_str, input_data=kwargs)
             )
 
     
-    def on_tool_end(self, output: str, **kwargs: Any) -> Any:
+    async  def on_tool_end(self, output: str, **kwargs: Any) -> Any:
         """Run when tool ends running."""
         self.prompt_watch.current_activity.output=output
         self.prompt_watch.current_activity.output_data=kwargs
         self.prompt_watch._close_current_activity()
 
 
         
     
 
     
-    def on_tool_error(
+    async  def on_tool_error(
         self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when tool errors."""
         self.prompt_watch._on_error(error, kwargs)
 
     
-    def on_text(self, text: str, **kwargs: Any) -> Any:
+    async def on_text(self, text: str, **kwargs: Any) -> Any:
         """Run on arbitrary text."""
 
     
-    def on_agent_action(self, action: AgentAction, **kwargs: Any) -> Any:
+    async def on_agent_action(self, action: AgentAction, **kwargs: Any) -> Any:
         """Run on agent action."""
         
         
 
 
 
     
-    def on_agent_finish(self, finish: AgentFinish, **kwargs: Any) -> Any:
+    async def on_agent_finish(self, finish: AgentFinish, **kwargs: Any) -> Any:
         """Run on agent end."""
         answer_text = finish[0].get("output")
         answer_activity = Answer(text=answer_text)
         self.prompt_watch._add_activity(answer_activity, as_root=True)
         if finish.return_values:
             answer_activity.metadata["outputs"]:finish.return_values
         
@@ -585,15 +593,16 @@
                     role="user"
                 elif isinstance(msg,LangChainChatMessage):
                     role = msg.role
                 elif isinstance(msg,AIMessage):
                     role="assistant"
                 elif isinstance(msg,SystemMessage):
                     role="system"
-                    
+                elif msg.type=="function":
+                    role="function"
                 return (ChatMessage(role=role,text=msg.content))
         elif isinstance(msg, list):
             return [convert_chat_messages(msg) for msg in msg]
         else:
             raise ValueError("msg must be either BaseMessage or List[BaseMessage]")
         
 def reconstruct_langchain_chat_messages( msg:Union[ChatMessage, List[ChatMessage]]):
```

### Comparing `promptwatch-0.2.4/src/promptwatch/langchain/unit_tests.py` & `promptwatch-0.2.5/src/promptwatch/langchain/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.4/src/promptwatch/promptwatch_context.py` & `promptwatch-0.2.5/src/promptwatch/promptwatch_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,64 +11,62 @@
 from .data_model import Session, ActivityBase,  ChainSequence, Log, Answer, Action, Question, RetrievedDocuments, DocumentSnippet
 from uuid import uuid4
 import types
 from .utils import wrap_a_method, classproperty
 from .caching import PromptWatchCacheManager
 from .constants import EnvVariables
 from abc import ABCMeta
+import contextvars
 
-
+session_context = contextvars.ContextVar("promptwatch_context")
 
 class ContextTrackerSingleton(ABCMeta,type):
     """
     Singleton metaclass for ensuring only one instance of a class per thread
     """
 
-    _thread_local = threading.local()
-    _cross_thread_storage = {}
+    #_thread_local = threading.local()
+    #_cross_thread_storage = {}
 
     def __call__(cls, *args, **kwargs)->PromptWatch:
         """Call method for the singleton metaclass."""
-        if not hasattr(ContextTrackerSingleton._thread_local, "_instance"):
+        prompt_watch_context = session_context.get(None)
+        if not prompt_watch_context:
             prompt_watch_context = super(ContextTrackerSingleton, cls).__call__(*args, **kwargs)
             if not prompt_watch_context.session_id:
                 raise Exception("PromptWatch: Session ID was not initialized. Please report this as a bug.")
-            ContextTrackerSingleton._cross_thread_storage[prompt_watch_context.session_id] = prompt_watch_context
-            ContextTrackerSingleton._thread_local._instance = prompt_watch_context
+            session_context.set(prompt_watch_context)
+            
+            # ContextTrackerSingleton._cross_thread_storage[prompt_watch_context.session_id] = prompt_watch_context
+            # ContextTrackerSingleton._thread_local._instance = prompt_watch_context
        
-        return ContextTrackerSingleton._thread_local._instance 
+        return prompt_watch_context
         
     def get_current(session_id:str=None)->PromptWatch:
         """ return the current instance
         for sync context session_id is not required
         for async context session_id is required, otherwise it the instance wont be found
         """
-        if hasattr(ContextTrackerSingleton._thread_local, "_instance"):
-            # in thread context ... this will work unless async is used... then we loose track...
-            # it is OK for nesting context in single thread...
-            current_instance = ContextTrackerSingleton._thread_local._instance
-            if current_instance and session_id and current_instance.session_id != session_id:
-                logging.warn(f"PromptWatch: Session ID {session_id} is not the same as the current session ID {current_instance.session_id}.  Please report this as a bug, ignoring the current context.")
-            else:
-                return current_instance
-        
-        # in async context... we need to use cross thread storage    
-        if session_id and ContextTrackerSingleton._cross_thread_storage.get(session_id):
-            current_session_context =  ContextTrackerSingleton._cross_thread_storage[session_id]
-            # also introduce it to the thread local storage
-            ContextTrackerSingleton._thread_local._instance = current_session_context
-            return current_session_context
-        else:
+        prompt_watch_context =  session_context.get(None)
+        if not prompt_watch_context:
             return None
+        elif session_id and prompt_watch_context.session_id != session_id:
+            raise Exception("PromptWatch: Session ID mismatch. Please report this as a bug.")
+        else:
+            return prompt_watch_context
 
     @classmethod
     def remove_active_instance(cls):
-        session_id = ContextTrackerSingleton._thread_local._instance.session_id
-        del ContextTrackerSingleton._cross_thread_storage[session_id]
-        del ContextTrackerSingleton._thread_local._instance 
+        session_context.set(None)
+        # session_id = ContextTrackerSingleton._thread_local._instance.session_id
+        # del ContextTrackerSingleton._cross_thread_storage[session_id]
+        # del ContextTrackerSingleton._thread_local._instance 
+
+
+
 
 class PromptWatch(metaclass=ContextTrackerSingleton):
     
     prompt_template_register_cache={}
 
     def __init__(self, session_id: Optional[str] = None, tracking_project: Optional[str] = None, tracking_tenant: Optional[str] = None, api_key: Optional[str] = None):
         """
@@ -113,28 +111,51 @@
         self.client = Client(api_key=api_key)
         
         # assign session_id if not provided
         # we will used to track the session across multiple threads
         if not self.session_id:
             self.session_id = str(uuid4())
         
-        self.chain_hierarchy:List[ChainSequence]=[]
+        #self.chain_hierarchy_context = contextvars.ContextVar("chain_hierarchy")
+        #self.context_storage=contextvars.ContextVar("context_storage")
+        self.context={}
+        self.chain_hierarchy=[]
+
         self.pending_session_save=True
         self.pending_stack:List[ActivityBase]=[]
         
         self.current_session=None
-        self.context={}
         self._cache_manager = PromptWatchCacheManager(self)
         self.tracing_handlers={}
         self.session_entered=False
 
         #event handlers that lasts only
         self.on_activity_event_handlers=[]
         
 
+    # @property
+    # def context(self)->dict:
+    #     current_context= self.context_storage.get(None)
+    #     if not current_context:
+    #         current_context={}
+    #         self.context_storage.set(current_context)
+    #     return current_context
+
+    # @property
+    # def chain_hierarchy(self)->List[ChainSequence]:
+    #     current_chain_hierarchy= self.chain_hierarchy_context.get(None)
+    #     if not current_chain_hierarchy:
+    #         current_chain_hierarchy=[]
+    #         self.chain_hierarchy_context.set(current_chain_hierarchy)
+    #     return current_chain_hierarchy
+
+    @property
+    def caching(self):
+        return self._cache_manager
+    
     @property
     def caching(self):
         return self._cache_manager
 
     @property
     def langchain(self):
         if not hasattr(self,"_langchain"):
@@ -143,15 +164,15 @@
             
         
         return self._langchain
     
 
 
     def __enter__(self):
-        
+        _ = self.chain_hierarchy
         if not self.tracing_handlers:
             # lets enable tracing by default
             self.langchain.init_tracing()
             #raise Exception("PromptWatch: LangChain callback handler is not set. Please call langchain_tracing() before entering the context.")
 
         if not self.current_session:
             self.start_session()
@@ -304,30 +325,30 @@
 
 
         
 
         
 
     def _open_activity(self, activity:ActivityBase):
-            
+
         if not self.current_session.session_name and isinstance(activity,ChainSequence) and activity.inputs:
             # if current session doesn't have a name, use first non empty input of first chain
             self.current_session.session_name = next((v for k,v in activity.inputs.items() if v and isinstance(v,str)), None)
 
         if not self.current_session.start_time:
             self.start_session()
         self.current_session.steps_count+=1
         activity.order=self.current_session.steps_count
 
         if self.current_activity:
             if isinstance(self.current_activity,ChainSequence) or isinstance(self.current_activity,Action):
                 activity.parent_activity_id=self.current_activity.id
             else:
                 activity.parent_activity_id=self.current_activity.parent_activity_id
-    
+        
         self.pending_stack.append(activity)
         self.chain_hierarchy.append(activity)
         return
         
     
 
     def _add_activity(self, activity:ActivityBase, as_root:bool=False):
```

### Comparing `promptwatch-0.2.4/src/promptwatch/unit_tests/evaluation.py` & `promptwatch-0.2.5/src/promptwatch/unit_tests/evaluation.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.4/src/promptwatch/unit_tests/schema.py` & `promptwatch-0.2.5/src/promptwatch/unit_tests/schema.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.4/src/promptwatch/unit_tests/unit_tests.py` & `promptwatch-0.2.5/src/promptwatch/unit_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.4/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.2.5/src/promptwatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.4
+Version: 0.2.5
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.4/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.2.5/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

