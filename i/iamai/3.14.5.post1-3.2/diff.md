# Comparing `tmp/iamai-3.14.5.post1.tar.gz` & `tmp/iamai-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai-3.14.5.post1.tar", max compression
+gzip compressed data, was "iamai-3.2.tar", max compression
```

## Comparing `iamai-3.14.5.post1.tar` & `iamai-3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-18 16:36:06.690341 iamai-3.14.5.post1/LICENSE
--rw-r--r--   0        0        0     9629 2023-04-18 16:36:06.690341 iamai-3.14.5.post1/README.md
--rw-r--r--   0        0        0      543 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/__init__.py
--rw-r--r--   0        0        0     4432 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/adapter/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/adapter/http_server_test_adapter.py
--rw-r--r--   0        0        0     1059 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/adapter/test.py
--rw-r--r--   0        0        0     7955 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/adapter/utils.py
--rw-r--r--   0        0        0    34820 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/bot.py
--rw-r--r--   0        0        0     1970 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/config.py
--rw-r--r--   0        0        0     1907 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/event.py
--rw-r--r--   0        0        0     1088 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/exceptions.py
--rw-r--r--   0        0        0      689 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/log.py
--rw-r--r--   0        0        0    13843 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/message.py
--rw-r--r--   0        0        0     3503 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/plugin.py
--rw-r--r--   0        0        0     1052 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/typing.py
--rw-r--r--   0        0        0     5529 2023-04-18 16:36:06.702341 iamai-3.14.5.post1/iamai/utils.py
--rw-r--r--   0        0        0     2317 2023-04-18 16:36:06.714341 iamai-3.14.5.post1/pyproject.toml
--rw-r--r--   0        0        0    10930 1970-01-01 00:00:00.000000 iamai-3.14.5.post1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-14 12:11:24.499442 iamai-3.2/LICENSE
+-rw-r--r--   0        0        0     9810 2023-07-14 12:11:24.499442 iamai-3.2/README.md
+-rw-r--r--   0        0        0      543 2023-07-14 12:11:24.507443 iamai-3.2/iamai/__init__.py
+-rw-r--r--   0        0        0     4432 2023-07-14 12:11:24.507443 iamai-3.2/iamai/adapter/__init__.py
+-rw-r--r--   0        0        0     1211 2023-07-14 12:11:24.507443 iamai-3.2/iamai/adapter/http_server_test_adapter.py
+-rw-r--r--   0        0        0     1059 2023-07-14 12:11:24.507443 iamai-3.2/iamai/adapter/test.py
+-rw-r--r--   0        0        0     7955 2023-07-14 12:11:24.507443 iamai-3.2/iamai/adapter/utils.py
+-rw-r--r--   0        0        0    35506 2023-07-14 12:11:24.507443 iamai-3.2/iamai/bot.py
+-rw-r--r--   0        0        0     1970 2023-07-14 12:11:24.507443 iamai-3.2/iamai/config.py
+-rw-r--r--   0        0        0     1907 2023-07-14 12:11:24.507443 iamai-3.2/iamai/event.py
+-rw-r--r--   0        0        0     1088 2023-07-14 12:11:24.507443 iamai-3.2/iamai/exceptions.py
+-rw-r--r--   0        0        0      986 2023-07-14 12:11:24.507443 iamai-3.2/iamai/log.py
+-rw-r--r--   0        0        0    13843 2023-07-14 12:11:24.507443 iamai-3.2/iamai/message.py
+-rw-r--r--   0        0        0     3503 2023-07-14 12:11:24.507443 iamai-3.2/iamai/plugin.py
+-rw-r--r--   0        0        0     1052 2023-07-14 12:11:24.507443 iamai-3.2/iamai/typing.py
+-rw-r--r--   0        0        0     5529 2023-07-14 12:11:24.507443 iamai-3.2/iamai/utils.py
+-rw-r--r--   0        0        0     2446 2023-07-14 12:11:24.515443 iamai-3.2/pyproject.toml
+-rw-r--r--   0        0        0    11071 1970-01-01 00:00:00.000000 iamai-3.2/PKG-INFO
```

### Comparing `iamai-3.14.5.post1/LICENSE` & `iamai-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iamai-3.14.5.post1/README.md` & `iamai-3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 <p align="center">
 </p>
 <p align="center">
 <!-- onebot -->
   <a style="text-decoration:none" href="https://onebot.dev" target="_blank">
     <img src="https://img.shields.io/badge/-Onebot%2011-000020?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHAAAABwCAMAAADxPgR5AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAAxQTFRF////29vbr6+vAAAAk1hCcwAAAAR0Uk5T////AEAqqfQAAAKcSURBVHja7NrbctswDATQXfD//zlpO7FlmwAWIOnOtNaTM5JwDMa8E+PNFz7g3waJ24fviyDPgfhz8fHP39cBcBL9KoJbQUxjA2iYqHL3FAnvzhL4GtVNUcoSZe6eSHizBcK5LL7dBr2AUZlev1ARRHCljzRALIEog6H3U6bCIyqIZdAT0eBuJYaGiJaHSjmkYIZd+qSGWAQnIaz2OArVnX6vrItQvbhZJtVGB5qX9wKqCMkb9W7aexfCO/rwQRBzsDIsYx4AOz0nhAtWu7bqkEQBO0Pr+Ftjt5fFCUEbm0Sbgdu8WSgJ5NgH2iu46R/o1UcBXJsFusWF/QUaz3RwJMEgngfaGGdSxJkE/Yg4lOBryBiMwvAhZrVMUUvwqU7F05b5WLaUIN4M4hRocQQRnEedgsn7TZB3UCpRrIJwQfqvGwsg18EnI2uSVNC8t+0QmMXogvbPg/xk+Mnw/6kW/rraUlvqgmFreAA09xW5t0AFlHrQZ3CsgvZm0FbHNKyBmheBKIF2cCA8A600aHPmFtRB1XvMsJAiza7LpPog0UJwccKdzw8rdf8MyN2ePYF896LC5hTzdZqxb6VNXInaupARLDNBWgI8spq4T0Qb5H4vWfPmHo8OyB1ito+AysNNz0oglj1U955sjUN9d41LnrX2D/u7eRwxyOaOpfyevCWbTgDEoilsOnu7zsKhjRCsnD/QzhdkYLBLXjiK4f3UWmcx2M7PO21CKVTH84638NTplt6JIQH0ZwCNuiWAfvuLhdrcOYPVO9eW3A67l7hZtgaY9GZo9AFc6cryjoeFBIWeU+npnk/nLE0OxCHL1eQsc1IciehjpJv5mqCsjeopaH6r15/MrxNnVhu7tmcslay2gO2Z1QfcfX0JMACG41/u0RrI9QAAAABJRU5ErkJggg==&logoColor=white" alt="onebotv11" />
     </a>
+    <a href="https://www.kookapp.cn/">
+      <img src="https://img.shields.io/badge/-%E5%BC%80%E9%BB%91%E5%95%A6Kook-83700?style=flat-square&logo=Discord&logoColor=white">
+    </a>
     <!-- github -->
     <!-- <img src="https://img.shields.io/badge/-github-181717?style=flat-square&logo=github&logoColor=white"> -->
     <!-- discord -->
     <!-- <img src="https://img.shields.io/badge/-Discord-5865F2?style=flat-square&logo=Discord&logoColor=white"> -->
     <!-- <br> -->
     <!-- bilibili live -->
     <!-- <img src="https://img.shields.io/badge/-BiliBili Live-00A1D6?style=flat-square&logo=Bilibili&logoColor=white"> -->
```

#### html2text {}

```diff
@@ -3,18 +3,20 @@
                                [Discord] [QQç¾¤]
                       ç®ä½ä¸­æ ã«ã»ãã íêµ­ì´
             Cross-platform robot framework, mainly used for ML/DL.
                              [Website] [Website]
                                [pypi] [python]
      [https://results.pre-commit.ci/badge/github/retrofor/iamai/main.svg]
                          [Codacy_Badge] [Codacy Badge]
- [onebotv11]         [https://img.shields.io/badge/-Mirai%20api%20http%202.3+-
-      00B8AA?style=flat-square]  [https://img.shields.io/badge/-DingTalk-
-    blue?style=flat-square]         [https://img.shields.io/badge/-Console-
-          4EAA25?style=flat-square&logo=GNU bash&logoColor=white]
+  [onebotv11] [https://img.shields.io/badge/-%E5%BC%80%E9%BB%91%E5%95%A6Kook-
+    83700?style=flat-square&logo=Discord&logoColor=white]         [https://
+  img.shields.io/badge/-Mirai%20api%20http%202.3+-00B8AA?style=flat-square]
+[https://img.shields.io/badge/-DingTalk-blue?style=flat-square]         [https:
+       //img.shields.io/badge/-Console-4EAA25?style=flat-square&logo=GNU
+                           bash&logoColor=white]
   [https://img.shields.io/github/forks/retrofor/iamai?style=social] [https://
            img.shields.io/github/stars/retrofor/iamai?style=social]
 [https://img.shields.io/github/watchers/retrofor/iamai?style=social] [https://
         img.shields.io/github/search/retrofor/iamai/goto?style=social]
 [https://img.shields.io/github/repo-size/retrofor/iamai?style=social] [https://
        img.shields.io/github/languages/top/retrofor/iamai?style=social]
 ## ð Introduction A Cross-platform robot framework, mainly used for machine
```

### Comparing `iamai-3.14.5.post1/iamai/__init__.py` & `iamai-3.2/iamai/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.5.post1/iamai/adapter/__init__.py` & `iamai-3.2/iamai/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.5.post1/iamai/adapter/http_server_test_adapter.py` & `iamai-3.2/iamai/adapter/http_server_test_adapter.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.5.post1/iamai/adapter/test.py` & `iamai-3.2/iamai/adapter/test.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.5.post1/iamai/adapter/utils.py` & `iamai-3.2/iamai/adapter/utils.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.5.post1/iamai/bot.py` & `iamai-3.2/iamai/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import json
 import time
 import signal
 import asyncio
 import threading
 from pathlib import Path
 from itertools import chain
+from datetime import datetime
 from collections import defaultdict
 from typing import Any, Dict, List, Type, Union, Callable, Optional, Awaitable
 
 from pydantic import ValidationError, create_model
 
 from iamai.adapter import Adapter
 from iamai.plugin import Plugin, PluginLoadType
@@ -35,23 +36,28 @@
     get_classes_from_dir,
     get_classes_from_module_name,
 )
 
 try:
     import tomllib  # type: ignore[module]
 except ModuleNotFoundError:
-    import tomli as tomllib
+    import tomli as tomllib  # type: ignore[no-redef]
 
 __all__ = ["Bot"]
 
 HANDLED_SIGNALS = (
     signal.SIGINT,  # Unix signal 2. Sent by Ctrl+C.
     signal.SIGTERM,  # Unix signal 15. Sent by `kill <pid>`.
 )
 
+current_path = os.path.dirname(os.path.abspath("__file__"))
+log_path = os.path.join(
+    current_path, "logs", datetime.now().strftime("%Y-%m-%d") + ".log"
+)
+
 
 class Bot:
     """iamai 机器人对象，定义了机器人的基本方法。
         读取并储存配置 `Config`，加载适配器 `Adapter` 和插件 `Plugin`，并进行事件分发。
 
     Attributes:
         config: 机器人配置。
@@ -108,17 +114,17 @@
             config_file: 配置文件，如不指定则使用默认的 `config.toml`。
                 若指定为 None，则不加载配置文件。
             config_dict: 配置字典，默认为 None。
                 若指定字典，则会忽略 config_file 配置，不再读取配置文件。
             hot_reload: 热重载。
                 启用后将自动检查 `plugin_dir` 中的插件文件更新，并在更新时自动重新加载。
         """
-        self.config = MainConfig()
+        self.config = MainConfig()  # type: ignore[assignment]
         self.plugins_priority_dict = defaultdict(list)
-        self.plugin_state = defaultdict(type(None))
+        self.plugin_state = defaultdict(type(None))  # type: ignore[assignment]
         self.global_state = {}
 
         self.adapters = []
         self._restart_flag = False
         self._module_path_finder = ModulePathFinder()
         self._raw_config_dict = {}
 
@@ -251,15 +257,20 @@
                     f'"{plugin_.__name__}" from file "{file}"'
                 )
         return removed_plugins
 
     async def _run_hot_reload(self):
         """热重载。"""
         try:
-            from watchfiles import Change, PythonFilter, DefaultFilter, awatch
+            from watchfiles import (  # type: ignore
+                Change,
+                PythonFilter,
+                DefaultFilter,
+                awatch,
+            )
         except ImportError:
             logger.warning(
                 'Hot reload needs to install "watchfiles", '
                 'try "pip install watchfiles"'
             )
             return
 
@@ -278,15 +289,15 @@
             stop_event=self.should_exit,
         ):
             # 按照 Change.deleted, Change.modified, Change.added 的顺序处理
             # 以确保发生重命名时先处理删除再处理新增
             for change_type, file in sorted(changes, key=lambda x: x[0], reverse=True):
                 # 更改配置文件
                 if (
-                    samefile(self._config_file, file)
+                    samefile(self._config_file, file)  # type: ignore
                     and change_type == change_type.modified
                 ):
                     logger.warning(f'Reload config file "{self._config_file}"')
                     old_config = self.config
                     self._reload_config_dict()
                     if (
                         self.config.bot != old_config.bot
@@ -332,15 +343,15 @@
             source: List, name: str, base: Type[ConfigModel]
         ) -> ConfigModel:
             config_update_dict = {}
             for i in source:
                 config_class = getattr(i, "Config", None)
                 if is_config_class(config_class):
                     try:
-                        default_value = config_class()
+                        default_value = config_class()  # type: ignore
                     except ValidationError:
                         default_value = ...
                     config_update_dict[getattr(config_class, "__config_name__")] = (
                         config_class,
                         default_value,
                     )
             return create_model(name, **config_update_dict, __base__=base)(
@@ -356,14 +367,15 @@
         # 更新 log 级别
         logger.remove()
         logger.add(
             sys.stderr,
             level=self.config.bot.log.level,
             format="<magenta>{time:YYYY-MM-DD HH:mm:ss.SSS}</magenta> <level>[{level}]</level> > <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>",
         )
+        logger.add(sink=log_path, level="INFO", rotation="10 MB")  # 每个日志文件最大为 10MB
 
     def _reload_config_dict(self):
         """重新加载配置文件。"""
         self._raw_config_dict = {}
         if self._config_dict is not None:
             self._raw_config_dict = self._config_dict
         elif self._config_file is not None:
@@ -385,40 +397,40 @@
                 error_or_exception(
                     "Read config file failed:", e, self.config.bot.log.verbose_exception
                 )
 
         try:
             self.config = MainConfig(**self._raw_config_dict)
         except ValidationError as e:
-            self.config = MainConfig()
+            self.config = MainConfig()  # type: ignore
             error_or_exception(
                 "Config dict parse error:", e, self.config.bot.log.verbose_exception
             )
         self._update_config()
 
     def reload_plugins(self):
         """手动重新加载所有插件。"""
         self.plugins_priority_dict.clear()
         self._load_plugins(*self.config.bot.plugins)
         self._load_plugins_from_dirs(*self.config.bot.plugin_dirs)
         self._load_plugins(*self._extend_plugins)
         self._load_plugins_from_dirs(*self._extend_plugin_dirs)
         self._update_config()
 
-    def _handle_exit(self, *args):  # noqa
+    def _handle_exit(self, *args):  # type: ignore
         """当机器人收到退出信号时，根据情况进行处理。"""
         logger.warning("Stopping iamai...")
         if self.should_exit.is_set():
             logger.critical("Force Exit iamai...")
             sys.exit()
         else:
             self.should_exit.set()
 
     async def handle_event(
-        self, current_event: T_Event, *, handle_get: bool = True, show_log: bool = True
+        self, current_event: T_Event, *, handle_get: bool = True, show_log: bool = True  # type: ignore
     ):
         """被适配器对象调用，根据优先级分发事件给所有插件，并处理插件的 `stop` 、 `skip` 等信号。
 
         此方法不应该被用户手动调用。
 
         Args:
             current_event: 当前待处理的 `Event`。
@@ -439,16 +451,16 @@
         else:
             asyncio.create_task(self._handle_event(current_event))
 
     async def _handle_event(self, current_event: Optional[T_Event] = None):
         if current_event is None:
             async with self._condition:
                 await self._condition.wait()
-                current_event = self._current_event
-            if current_event.__handled__:
+                current_event = self._current_event  # type: ignore
+            if current_event.__handled__:  # type: ignore
                 return
 
         for _hook_func in self._event_preprocessor_hooks:
             await _hook_func(current_event)
 
         for plugin_priority in sorted(self.plugins_priority_dict.keys()):
             try:
@@ -494,15 +506,15 @@
 
     async def get(
         self,
         func: Optional[Callable[[T_Event], Union[bool, Awaitable[bool]]]] = None,
         *,
         max_try_times: Optional[int] = None,
         timeout: Optional[Union[int, float]] = None,
-    ) -> T_Event:
+    ) -> T_Event:  # type: ignore
         """获取满足指定条件的的事件，协程会等待直到适配器接收到满足条件的事件、超过最大事件数或超时。
 
         Args:
             func: 协程或者函数，函数会被自动包装为协程执行。
                 要求接受一个事件作为参数，返回布尔值。当协程返回 `True` 时返回当前事件。
                 当为 `None` 时相当于输入对于任何事件均返回真的协程，即返回适配器接收到的下一个事件。
             max_try_times: 最大事件数。
@@ -513,15 +525,15 @@
 
         Raises:
             GetEventTimeout: 超过最大事件数或超时。
         """
         if func is None:
             func = sync_func_wrapper(lambda x: True)
         elif not asyncio.iscoroutinefunction(func):
-            func = sync_func_wrapper(func)
+            func = sync_func_wrapper(func)  # type: ignore
 
         try_times = 0
         start_time = time.time()
         while not self.should_exit.is_set():
             if max_try_times is not None and try_times > max_try_times:
                 break
             if timeout is not None and time.time() - start_time > timeout:
@@ -536,17 +548,17 @@
                             self._condition.wait(),
                             timeout=start_time + timeout - time.time(),
                         )
                     except asyncio.TimeoutError:
                         break
 
                 if not self._current_event.__handled__:
-                    if await func(self._current_event):
+                    if await func(self._current_event):  # type: ignore
                         self._current_event.__handled__ = True
-                        return self._current_event
+                        return self._current_event  # type: ignore
 
                 try_times += 1
 
         if not self.should_exit.is_set():
             raise GetEventTimeout
 
     def _load_plugin_class(
@@ -687,15 +699,15 @@
             *dirs: 储存包含插件的模块的模块路径。
                 例如：`pathlib.Path("path/of/plugins/")` 。
         """
         dirs = list(map(lambda x: str(x.resolve()), dirs))  # type: ignore  maybe remove?
         logger.warning(f'Loading plugins from dirs "{", ".join(map(str, dirs))}"')
         self._module_path_finder.path.extend(dirs)  # type: ignore
         # type: ignore
-        for plugin_class, module in get_classes_from_dir(dirs, Plugin):
+        for plugin_class, module in get_classes_from_dir(dirs, Plugin):  # type: ignore
             self._load_plugin_class(plugin_class, PluginLoadType.DIR, module.__file__)
 
     def load_plugins_from_dirs(self, *dirs: Path):
         """从目录中加载插件，以 `_` 开头的模块中的插件不会被导入。路径可以是相对路径或绝对路径。
 
         Args:
             *dirs: 储存包含插件的模块的模块路径。
@@ -756,15 +768,15 @@
 
         Args:
             *adapters: 适配器类或适配器名称，类型可以是 `Type[Adapter]` 或 `str`。
                 如果为 `Type[Adapter]` 类型时，将作为适配器类进行加载。
                 如果为 `str` 类型时，将作为适配器模块名称进行加载，格式和 Python `import` 语句相同。
                     例如：`path.of.adapter`。
         """
-        self._extend_adapters.extend(adapters)
+        self._extend_adapters.extend(adapters)  # type: ignore
         return self._load_adapters(*adapters)
 
     def get_adapter(self, name: str) -> Adapter:
         """按照名称获取已经加载的适配器。
 
         Args:
             name: 适配器名称。
@@ -789,15 +801,15 @@
         Returns:
             获取到的插件类。
 
         Raises:
             LookupError: 找不到此名称的插件类。
         """
         for _plugin in self.plugins:
-            if _plugin.name == name:
+            if _plugin.name == name:  # type: ignore
                 return _plugin
         raise LookupError(f'Can not find plugin named "{name}"')
 
     def bot_run_hook(self, func: T_BotHook) -> T_BotHook:
         """注册一个 Bot 启动时的函数。
 
         Args:
```

### Comparing `iamai-3.14.5.post1/iamai/config.py` & `iamai-3.2/iamai/config.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.5.post1/iamai/event.py` & `iamai-3.2/iamai/event.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.5.post1/iamai/exceptions.py` & `iamai-3.2/iamai/exceptions.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.5.post1/iamai/message.py` & `iamai-3.2/iamai/message.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.5.post1/iamai/plugin.py` & `iamai-3.2/iamai/plugin.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.5.post1/iamai/typing.py` & `iamai-3.2/iamai/typing.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.5.post1/iamai/utils.py` & `iamai-3.2/iamai/utils.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.5.post1/pyproject.toml` & `iamai-3.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai"
-version = "3.14.5.post1"
+version = "3.2"
 description = "bot framework."
 authors = ["简律纯 <admin@jyunko.cn>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
@@ -18,34 +18,37 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 tomli = { version = "^2.0.0", python = "<3.11" }
 pydantic = "^1.10.0"
 aiohttp = "^3.8.0"
-loguru = "^0.6.0"
+loguru = ">=0.6,<0.8"
 typing-extensions = "^4.4.0"
 
 [tool.poetry.group.dev.dependencies]
 watchfiles = "^0.18.0"
 sophia-doc = "^0.1.0"
+iamai-adapter-kook = { path = "./packages/iamai-adapter-kook", develop = true }
 iamai-adapter-cqhttp = { path = "./packages/iamai-adapter-cqhttp", develop = true }
 iamai-adapter-dingtalk = { path = "./packages/iamai-adapter-dingtalk", develop = true }
 iamai-adapter-apscheduler = { path = "./packages/iamai-adapter-apscheduler", develop = true }
 black = "^23.1.0"
 isort = "^5.12.0"
 pre-commit = "^3.1.0"
 pre-commit-hooks = "^4.4.0"
 
 [tool.poetry.extras]
+kook = ["iamai-adapter-kook"]
 cqhttp = ["iamai-adapter-cqhttp"]
 dingtalk = ["iamai-adapter-dingtalk"]
 apscheduler = ["iamai-adapter-apscheduler"]
 hot_reload = ["watchfiles"]
 all = [
+  "iamai-adapter-kook",
   "iamai-adapter-cqhttp",
   "iamai-adapter-dingtalk",
   "iamai-adapter-apscheduler",
   "watchfiles",
 ]
 
 [tool.black]
```

### Comparing `iamai-3.14.5.post1/PKG-INFO` & `iamai-3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai
-Version: 3.14.5.post1
+Version: 3.2
 Summary: bot framework.
 Home-page: https://retrofor.space/
 License: MIT
 Keywords: bot,qq,qqbot,mirai,coolq
 Author: 简律纯
 Author-email: admin@jyunko.cn
 Requires-Python: >=3.8,<4.0
@@ -14,22 +14,22 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Provides-Extra: all
 Provides-Extra: apscheduler
 Provides-Extra: cqhttp
 Provides-Extra: dingtalk
 Provides-Extra: hot-reload
+Provides-Extra: kook
 Requires-Dist: aiohttp (>=3.8.0,<4.0.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: loguru (>=0.6,<0.8)
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: tomli (>=2.0.0,<3.0.0) ; python_version < "3.11"
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Documentation, https://iamai.retrofor.space/
 Project-URL: Repository, https://github.com/retrofor/iamai
 Description-Content-Type: text/markdown
 
@@ -72,14 +72,17 @@
 <p align="center">
 </p>
 <p align="center">
 <!-- onebot -->
   <a style="text-decoration:none" href="https://onebot.dev" target="_blank">
     <img src="https://img.shields.io/badge/-Onebot%2011-000020?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAHAAAABwCAMAAADxPgR5AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAAxQTFRF////29vbr6+vAAAAk1hCcwAAAAR0Uk5T////AEAqqfQAAAKcSURBVHja7NrbctswDATQXfD//zlpO7FlmwAWIOnOtNaTM5JwDMa8E+PNFz7g3waJ24fviyDPgfhz8fHP39cBcBL9KoJbQUxjA2iYqHL3FAnvzhL4GtVNUcoSZe6eSHizBcK5LL7dBr2AUZlev1ARRHCljzRALIEog6H3U6bCIyqIZdAT0eBuJYaGiJaHSjmkYIZd+qSGWAQnIaz2OArVnX6vrItQvbhZJtVGB5qX9wKqCMkb9W7aexfCO/rwQRBzsDIsYx4AOz0nhAtWu7bqkEQBO0Pr+Ftjt5fFCUEbm0Sbgdu8WSgJ5NgH2iu46R/o1UcBXJsFusWF/QUaz3RwJMEgngfaGGdSxJkE/Yg4lOBryBiMwvAhZrVMUUvwqU7F05b5WLaUIN4M4hRocQQRnEedgsn7TZB3UCpRrIJwQfqvGwsg18EnI2uSVNC8t+0QmMXogvbPg/xk+Mnw/6kW/rraUlvqgmFreAA09xW5t0AFlHrQZ3CsgvZm0FbHNKyBmheBKIF2cCA8A600aHPmFtRB1XvMsJAiza7LpPog0UJwccKdzw8rdf8MyN2ePYF896LC5hTzdZqxb6VNXInaupARLDNBWgI8spq4T0Qb5H4vWfPmHo8OyB1ito+AysNNz0oglj1U955sjUN9d41LnrX2D/u7eRwxyOaOpfyevCWbTgDEoilsOnu7zsKhjRCsnD/QzhdkYLBLXjiK4f3UWmcx2M7PO21CKVTH84638NTplt6JIQH0ZwCNuiWAfvuLhdrcOYPVO9eW3A67l7hZtgaY9GZo9AFc6cryjoeFBIWeU+npnk/nLE0OxCHL1eQsc1IciehjpJv5mqCsjeopaH6r15/MrxNnVhu7tmcslay2gO2Z1QfcfX0JMACG41/u0RrI9QAAAABJRU5ErkJggg==&logoColor=white" alt="onebotv11" />
     </a>
+    <a href="https://www.kookapp.cn/">
+      <img src="https://img.shields.io/badge/-%E5%BC%80%E9%BB%91%E5%95%A6Kook-83700?style=flat-square&logo=Discord&logoColor=white">
+    </a>
     <!-- github -->
     <!-- <img src="https://img.shields.io/badge/-github-181717?style=flat-square&logo=github&logoColor=white"> -->
     <!-- discord -->
     <!-- <img src="https://img.shields.io/badge/-Discord-5865F2?style=flat-square&logo=Discord&logoColor=white"> -->
     <!-- <br> -->
     <!-- bilibili live -->
     <!-- <img src="https://img.shields.io/badge/-BiliBili Live-00A1D6?style=flat-square&logo=Bilibili&logoColor=white"> -->
```

#### html2text {}

```diff
@@ -1,38 +1,39 @@
-Metadata-Version: 2.1 Name: iamai Version: 3.14.5.post1 Summary: bot framework.
-Home-page: https://retrofor.space/ License: MIT Keywords:
-bot,qq,qqbot,mirai,coolq Author: ç®å¾çº¯ Author-email: admin@jyunko.cn
-Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5 - Production/
-Stable Classifier: Framework :: Robot Framework Classifier: Framework :: Robot
-Framework :: Library Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 Provides-Extra: all Provides-Extra:
+Metadata-Version: 2.1 Name: iamai Version: 3.2 Summary: bot framework. Home-
+page: https://retrofor.space/ License: MIT Keywords: bot,qq,qqbot,mirai,coolq
+Author: ç®å¾çº¯ Author-email: admin@jyunko.cn Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
+:: Robot Framework Classifier: Framework :: Robot Framework :: Library
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Provides-Extra: all Provides-Extra:
 apscheduler Provides-Extra: cqhttp Provides-Extra: dingtalk Provides-Extra:
-hot-reload Requires-Dist: aiohttp (>=3.8.0,<4.0.0) Requires-Dist: loguru
-(>=0.6.0,<0.7.0) Requires-Dist: pydantic (>=1.10.0,<2.0.0) Requires-Dist: tomli
-(>=2.0.0,<3.0.0) ; python_version < "3.11" Requires-Dist: typing-extensions
-(>=4.4.0,<5.0.0) Project-URL: Documentation, https://iamai.retrofor.space/
-Project-URL: Repository, https://github.com/retrofor/iamai Description-Content-
-Type: text/markdown
+hot-reload Provides-Extra: kook Requires-Dist: aiohttp (>=3.8.0,<4.0.0)
+Requires-Dist: loguru (>=0.6,<0.8) Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: tomli (>=2.0.0,<3.0.0) ; python_version < "3.11" Requires-Dist:
+typing-extensions (>=4.4.0,<5.0.0) Project-URL: Documentation, https://
+iamai.retrofor.space/ Project-URL: Repository, https://github.com/retrofor/
+iamai Description-Content-Type: text/markdown
                    [https://iamai.retrofor.space/retro.png]
                               ****** iamai ******
                                [Discord] [QQç¾¤]
                       ç®ä½ä¸­æ ã«ã»ãã íêµ­ì´
             Cross-platform robot framework, mainly used for ML/DL.
                              [Website] [Website]
                                [pypi] [python]
      [https://results.pre-commit.ci/badge/github/retrofor/iamai/main.svg]
                          [Codacy_Badge] [Codacy Badge]
- [onebotv11]         [https://img.shields.io/badge/-Mirai%20api%20http%202.3+-
-      00B8AA?style=flat-square]  [https://img.shields.io/badge/-DingTalk-
-    blue?style=flat-square]         [https://img.shields.io/badge/-Console-
-          4EAA25?style=flat-square&logo=GNU bash&logoColor=white]
+  [onebotv11] [https://img.shields.io/badge/-%E5%BC%80%E9%BB%91%E5%95%A6Kook-
+    83700?style=flat-square&logo=Discord&logoColor=white]         [https://
+  img.shields.io/badge/-Mirai%20api%20http%202.3+-00B8AA?style=flat-square]
+[https://img.shields.io/badge/-DingTalk-blue?style=flat-square]         [https:
+       //img.shields.io/badge/-Console-4EAA25?style=flat-square&logo=GNU
+                           bash&logoColor=white]
   [https://img.shields.io/github/forks/retrofor/iamai?style=social] [https://
            img.shields.io/github/stars/retrofor/iamai?style=social]
 [https://img.shields.io/github/watchers/retrofor/iamai?style=social] [https://
         img.shields.io/github/search/retrofor/iamai/goto?style=social]
 [https://img.shields.io/github/repo-size/retrofor/iamai?style=social] [https://
        img.shields.io/github/languages/top/retrofor/iamai?style=social]
 ## ð Introduction A Cross-platform robot framework, mainly used for machine
```

