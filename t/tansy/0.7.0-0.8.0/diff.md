# Comparing `tmp/tansy-0.7.0.tar.gz` & `tmp/tansy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tansy-0.7.0.tar", last modified: Wed Apr 12 16:42:27 2023, max compression
+gzip compressed data, was "tansy-0.8.0.tar", last modified: Fri Jul 14 04:20:43 2023, max compression
```

## Comparing `tansy-0.7.0.tar` & `tansy-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:42:27.825065 tansy-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-12 16:42:12.000000 tansy-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-12 16:42:27.821066 tansy-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-12 16:42:12.000000 tansy-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-12 16:42:12.000000 tansy-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:42:27.825065 tansy-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-12 16:42:12.000000 tansy-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:42:27.821066 tansy-0.7.0/tansy/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 16:42:12.000000 tansy-0.7.0/tansy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-04-12 16:42:12.000000 tansy-0.7.0/tansy/class_slash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-04-12 16:42:12.000000 tansy-0.7.0/tansy/slash_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-12 16:42:12.000000 tansy-0.7.0/tansy/slash_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-12 16:42:12.000000 tansy-0.7.0/tansy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:42:27.821066 tansy-0.7.0/tansy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-12 16:42:27.000000 tansy-0.7.0/tansy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-12 16:42:27.000000 tansy-0.7.0/tansy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:42:27.000000 tansy-0.7.0/tansy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 16:42:27.000000 tansy-0.7.0/tansy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 16:42:27.000000 tansy-0.7.0/tansy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 04:20:43.589475 tansy-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 04:20:27.000000 tansy-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-14 04:20:43.589475 tansy-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-14 04:20:27.000000 tansy-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 04:20:27.000000 tansy-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 04:20:43.589475 tansy-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-14 04:20:27.000000 tansy-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 04:20:43.589475 tansy-0.8.0/tansy/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-14 04:20:27.000000 tansy-0.8.0/tansy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-07-14 04:20:27.000000 tansy-0.8.0/tansy/class_slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32337 2023-07-14 04:20:27.000000 tansy-0.8.0/tansy/slash_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-14 04:20:27.000000 tansy-0.8.0/tansy/slash_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-14 04:20:27.000000 tansy-0.8.0/tansy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 04:20:43.589475 tansy-0.8.0/tansy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-14 04:20:43.000000 tansy-0.8.0/tansy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 04:20:43.000000 tansy-0.8.0/tansy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 04:20:43.000000 tansy-0.8.0/tansy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-14 04:20:43.000000 tansy-0.8.0/tansy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 04:20:43.000000 tansy-0.8.0/tansy.egg-info/top_level.txt
```

### Comparing `tansy-0.7.0/LICENSE` & `tansy-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tansy-0.7.0/PKG-INFO` & `tansy-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tansy
-Version: 0.7.0
+Version: 0.8.0
 Summary: Unstable experiments with interactions.py.
 Home-page: https://github.com/Astrea49/tansy
 Author: AstreaTSS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `tansy-0.7.0/README.md` & `tansy-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `tansy-0.7.0/setup.py` & `tansy-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 setup(
     name="tansy",
     description="Unstable experiments with interactions.py.",
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     author="AstreaTSS",
     url="https://github.com/Astrea49/tansy",
-    version="0.7.0",
+    version="0.8.0",
     packages=find_packages(),
     python_requires=">=3.10",
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `tansy-0.7.0/tansy/__init__.py` & `tansy-0.8.0/tansy/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 """
 Tansy
 Unstable experiments with interactions.py.
 :copyright: (c) 2022-present AstreaTSS
 :license: MIT, see LICENSE for more details.
 """
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 
 from .class_slash import *
 from .slash_commands import *
 from .slash_param import *
 
 __all__ = (
+    "__version__",
     "TansySlashCommandParameter",
     "TansySlashCommand",
+    "TansyHybridSlashCommand",
     "SlashCommand",
+    "HybridSlashCommand",
     "tansy_slash_command",
+    "tansy_hybrid_slash_command",
     "slash_command",
+    "hybrid_slash_command",
     "tansy_subcommand",
+    "tansy_hybrid_slash_subcommand",
     "subcommand",
+    "hybrid_slash_subcommand",
     "ParamInfo",
     "Param",
     "Option",
     "ClassSlashCommand",
     "class_slash_command",
     "class_subcommand",
     "describe",
```

### Comparing `tansy-0.7.0/tansy/class_slash.py` & `tansy-0.8.0/tansy/class_slash.py`

 * *Files identical despite different names*

### Comparing `tansy-0.7.0/tansy/slash_commands.py` & `tansy-0.8.0/tansy/slash_commands.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,26 +3,33 @@
 import functools
 import inspect
 import typing
 from builtins import getattr
 
 import attrs
 import interactions as ipy
+from interactions.ext import hybrid_commands as hybrid
 
 from . import slash_param
 from . import utils
 
 __all__ = (
     "TansySlashCommandParameter",
     "TansySlashCommand",
+    "TansyHybridSlashCommand",
     "tansy_slash_command",
     "tansy_subcommand",
+    "tansy_hybrid_slash_command",
+    "tansy_hybrid_slash_subcommand",
     "SlashCommand",
     "slash_command",
     "subcommand",
+    "HybridSlashCommand",
+    "hybrid_slash_command",
+    "hybrid_slash_subcommand",
 )
 
 
 def _get_converter(anno: type, name: str):
     if typing.get_origin(anno) == typing.Annotated:
         anno = utils.get_from_anno_type(anno)
 
@@ -146,176 +153,176 @@
 class TansySlashCommandParameter:
     """An object representing parameters in a command."""
 
     name: str = attrs.field(default=None)
     argument_name: str = attrs.field(default=None)
     default: typing.Any = attrs.field(default=ipy.MISSING)
     type: typing.Type = attrs.field(default=None)
+    kind: inspect._ParameterKind = attrs.field(default=ipy.MISSING)
     converter: typing.Optional[typing.Callable] = attrs.field(default=None)
 
     @property
     def optional(self) -> bool:
         return self.default != ipy.MISSING
 
 
-@attrs.define(eq=False, order=False, hash=False, kw_only=True)
-class TansySlashCommand(ipy.SlashCommand):
-    parameters: dict[str, TansySlashCommandParameter] = attrs.field(
-        factory=dict, metadata=ipy.utils.no_export_meta
-    )
-    _inspect_signature: typing.Optional[inspect.Signature] = attrs.field(
-        repr=False, default=None, metadata=ipy.utils.no_export_meta
+def _overwrite_with_parameters(cmd: "TansySlashCommand | TansyHybridSlashCommand"):
+    # i wont lie to you - what we're about to do is probably the
+    # most disgusting, hacky thing ive done in python, but there's a good
+    # reason for it
+    #
+    # you know how Option() exists in this lib? you know how you have to
+    # do arg: type = Option() in order to define an option usually when
+    # using tansy commands?
+    # well, now Option() is the default of arg in the command, which
+    # means if no value is provided for arg while using the raw callback,
+    # instead of erroring out or receiving the value specified in default=X
+    # (or None, if you used Optional and didn't explictly set a default value),
+    # the function will instead just pass in the ParamInfo generated by Option(),
+    # which is unintuitive and would result in a lot of bugs
+    #
+    # to prevent this, we overwrite the defaults in the function with ones
+    # that make more sense considering tansy's features
+    # explainations about the cursed _overwrite_defaults can be found
+    # in the function itself
+
+    defaults = {
+        p.argument_name: p.default for p in cmd.parameters.values() if p.optional
+    }
+    cmd.callback = _overwrite_defaults(
+        cmd.callback, defaults, cmd._inspect_signature.parameters
     )
 
-    def _overwrite_with_parameters(self):
-        # i wont lie to you - what we're about to do is probably the
-        # most disgusting, hacky thing ive done in python, but there's a good
-        # reason for it
-        #
-        # you know how Option() exists in this lib? you know how you have to
-        # do arg: type = Option() in order to define an option usually when
-        # using tansy commands?
-        # well, now Option() is the default of arg in the command, which
-        # means if no value is provided for arg while using the raw callback,
-        # instead of erroring out or receiving the value specified in default=X
-        # (or None, if you used Optional and didn't explictly set a default value),
-        # the function will instead just pass in the ParamInfo generated by Option(),
-        # which is unintuitive and would result in a lot of bugs
-        #
-        # to prevent this, we overwrite the defaults in the function with ones
-        # that make more sense considering tansy's features
-        # explainations about the cursed _overwrite_defaults can be found
-        # in the function itself
-
-        defaults = {
-            p.argument_name: p.default for p in self.parameters.values() if p.optional
-        }
-        self.callback = _overwrite_defaults(
-            self.callback, defaults, self._inspect_signature.parameters
-        )
 
-    def _parse_parameters(self):
-        if self.callback is None:
-            return
-
-        if self.parameters:
-            self._overwrite_with_parameters()
-            return
-
-        self.options = []
-
-        if not self._inspect_signature:
-            if self.has_binding:
-                callback = functools.partial(self.callback, None, None)
-            else:
-                callback = functools.partial(self.callback, None)
+def tansy_parse_parameters(cmd: "TansySlashCommand | TansyHybridSlashCommand"):
+    if cmd.callback is None:
+        return
+
+    if cmd.parameters:
+        _overwrite_with_parameters(cmd)
+        return
+
+    cmd.options = []
+
+    if not cmd._inspect_signature:
+        if cmd.has_binding:
+            callback = functools.partial(cmd.callback, None, None)
+        else:
+            callback = functools.partial(cmd.callback, None)
+
+        cmd._inspect_signature = inspect.signature(callback)
+
+    describes: dict[str, ipy.LocalisedDesc] = getattr(
+        cmd.callback, "__tansy_describe__", {}
+    )
 
-            self._inspect_signature = inspect.signature(callback)
+    for param in cmd._inspect_signature.parameters.values():
+        if param.kind == param.VAR_KEYWORD:
+            # something like **kwargs, that's fine so let it pass
+            continue
+
+        if param.kind not in {
+            param.POSITIONAL_OR_KEYWORD,
+            param.KEYWORD_ONLY,
+        }:
+            raise ValueError(
+                "All parameters must be able to be used via keyword arguments."
+            )
 
-        describes: dict[str, ipy.LocalisedDesc] = getattr(
-            self.callback, "__tansy_describe__", {}
+        cmd_param = TansySlashCommandParameter(kind=param.kind)
+        param_info = (
+            param.default if isinstance(param.default, slash_param.ParamInfo) else None
         )
 
-        for param in self._inspect_signature.parameters.values():
-            if param.kind == param.VAR_KEYWORD:
-                # something like **kwargs, that's fine so let it pass
-                continue
+        if param_info:
+            option = param_info.generate_option()
+        else:
+            try:
+                option_type = utils.get_option(param.annotation)
+            except ValueError:
+                raise ValueError(f"Invalid/no provided type for {param.name}") from None
+            option = ipy.SlashCommandOption(name=param.name, type=option_type)
+
+        cmd_param.name = str(option.name) if option.name else param.name
+        cmd_param.argument_name = param.name
+        option.name = option.name or ipy.LocalisedName.converter(cmd_param.name)
+
+        if desc := describes.get(option.name.default):
+            option.description = desc
+
+        if option.type is None:
+            try:
+                option.type = utils.get_option(param.annotation)
+            except ValueError:
+                raise ValueError(f"Invalid/no provided type for {param.name}") from None
+
+        if param_info:
+            cmd_param.default = param_info.default
+        elif param.default is not param.empty:
+            option.required = False
+            cmd_param.default = param.default
+        else:
+            cmd_param.default = ipy.MISSING
+
+        # what we're checking here is:
+        # - if we don't already have a default
+        # - if the user didn't already specify a type in
+        #   param_info that would indicate if its optional or not
+        # - if the annotation is marked as optional
+        # if so, we want to make the option not required, and the default be None
+        if (
+            cmd_param.default is ipy.MISSING
+            and (not param_info or not param_info._user_provided_type)
+            and utils.is_optional(param.annotation)
+        ):
+            option.required = False
+            cmd_param.default = None
 
-            if param.kind not in {
-                param.POSITIONAL_OR_KEYWORD,
-                param.KEYWORD_ONLY,
-            }:
+        if (
+            param_info
+            and option.type == ipy.OptionType.CHANNEL
+            and not option.channel_types
+        ):
+            option.channel_types = utils.resolve_channel_types(param.annotation)  # type: ignore
+
+        if param_info and param_info.converter:
+            if convert_func := _get_converter(param_info.converter, param.name):
+                cmd_param.converter = convert_func
+            else:
                 raise ValueError(
-                    "All parameters must be able to be used via keyword arguments."
+                    f"The converter for {param.name} is invalid. Please make"
+                    " sure it is either a Converter-like class or a function."
                 )
+        elif converter := _get_converter(param.annotation, param.name):
+            cmd_param.converter = converter
 
-            cmd_param = TansySlashCommandParameter()
-            param_info = (
-                param.default
-                if isinstance(param.default, slash_param.ParamInfo)
-                else None
-            )
+        # we bypassed validation earlier, so let's make sure everything's okay
+        # since we got the final option stuff now
+        attrs.validate(option)  # type: ignore
+        cmd.options.append(option)
+        cmd.parameters[cmd_param.name] = cmd_param
+
+    # make sure the options arent in an invalid order -
+    # both to safeguard against invalid slash commands and because
+    # we rely on optional arguments being after required arguments right after this
+    attrs.validate(cmd)
+    _overwrite_with_parameters(cmd)
 
-            if param_info:
-                option = param_info.generate_option()
-            else:
-                try:
-                    option_type = utils.get_option(param.annotation)
-                except ValueError:
-                    raise ValueError(
-                        f"Invalid/no provided type for {param.name}"
-                    ) from None
-                option = ipy.SlashCommandOption(name=param.name, type=option_type)
-
-            cmd_param.name = str(option.name) if option.name else param.name
-            cmd_param.argument_name = param.name
-            option.name = option.name or ipy.LocalisedName.converter(cmd_param.name)
-
-            if desc := describes.get(option.name.default):
-                option.description = desc
-
-            if option.type is None:
-                try:
-                    option.type = utils.get_option(param.annotation)
-                except ValueError:
-                    raise ValueError(
-                        f"Invalid/no provided type for {param.name}"
-                    ) from None
-
-            if param_info:
-                cmd_param.default = param_info.default
-            elif param.default is not param.empty:
-                option.required = False
-                cmd_param.default = param.default
-            else:
-                cmd_param.default = ipy.MISSING
 
-            # what we're checking here is:
-            # - if we don't already have a default
-            # - if the user didn't already specify a type in
-            #   param_info that would indicate if its optional or not
-            # - if the annotation is marked as optional
-            # if so, we want to make the option not required, and the default be None
-            if (
-                cmd_param.default is ipy.MISSING
-                and (not param_info or not param_info._user_provided_type)
-                and utils.is_optional(param.annotation)
-            ):
-                option.required = False
-                cmd_param.default = None
-
-            if (
-                param_info
-                and option.type == ipy.OptionType.CHANNEL
-                and not option.channel_types
-            ):
-                option.channel_types = utils.resolve_channel_types(param.annotation)  # type: ignore
-
-            if param_info and param_info.converter:
-                if convert_func := _get_converter(param_info.converter, param.name):
-                    cmd_param.converter = convert_func
-                else:
-                    raise ValueError(
-                        f"The converter for {param.name} is invalid. Please make"
-                        " sure it is either a Converter-like class or a function."
-                    )
-            elif converter := _get_converter(param.annotation, param.name):
-                cmd_param.converter = converter
-
-            # we bypassed validation earlier, so let's make sure everything's okay
-            # since we got the final option stuff now
-            attrs.validate(option)  # type: ignore
-            self.options.append(option)
-            self.parameters[cmd_param.name] = cmd_param
-
-        # make sure the options arent in an invalid order -
-        # both to safeguard against invalid slash commands and because
-        # we rely on optional arguments being after required arguments right after this
-        attrs.validate(self)  # type: ignore
-        self._overwrite_with_parameters()
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class TansySlashCommand(ipy.SlashCommand):
+    parameters: dict[str, TansySlashCommandParameter] = attrs.field(
+        factory=dict, metadata=ipy.utils.no_export_meta
+    )
+    _inspect_signature: typing.Optional[inspect.Signature] = attrs.field(
+        repr=False, default=None, metadata=ipy.utils.no_export_meta
+    )
+
+    def _parse_parameters(self) -> None:
+        tansy_parse_parameters(self)
 
     async def call_callback(
         self, callback: typing.Callable, ctx: ipy.InteractionContext
     ) -> None:
         """
         Runs the callback of this command.
         Args:
@@ -393,14 +400,120 @@
                 nsfw=nsfw,
                 checks=self.checks.copy() if inherit_checks else [],
             )
 
         return wrapper
 
 
+@attrs.define(eq=False, order=False, hash=False, kw_only=True)
+class TansyHybridSlashCommand(hybrid.HybridSlashCommand):
+    parameters: dict[str, TansySlashCommandParameter] = attrs.field(
+        factory=dict, metadata=ipy.utils.no_export_meta
+    )
+    _inspect_signature: typing.Optional[inspect.Signature] = attrs.field(
+        repr=False, default=None, metadata=ipy.utils.no_export_meta
+    )
+
+    def _parse_parameters(self) -> None:
+        tansy_parse_parameters(self)
+
+    async def call_callback(
+        self, callback: typing.Callable, ctx: hybrid.HybridContext
+    ) -> None:
+        """
+        Runs the callback of this command.
+        Args:
+            callback (Callable: The callback to run. This is provided for compatibility with ipy.
+            ctx (ipy.InteractionContext): The context to use for this command.
+        """
+        if not self.parameters:
+            return await callback(ctx, **ctx.kwargs)
+
+        new_kwargs = {}
+
+        for key, value in ctx.kwargs.items():
+            param = self.parameters.get(key)
+            if not param:
+                # hopefully you have **kwargs
+                new_kwargs[key] = value
+                continue
+
+            if param.converter:
+                converted = await ipy.utils.maybe_coroutine(param.converter, ctx, value)
+            else:
+                converted = value
+            new_kwargs[param.argument_name] = converted
+
+        return await self.call_with_binding(callback, ctx, **new_kwargs)
+
+    def group(
+        self,
+        name: str = None,
+        description: str = "No Description Set",
+        inherit_checks: bool = True,
+        aliases: list[str] | None = None,
+    ) -> "TansyHybridSlashCommand":
+        self._dummy_base = True
+        return TansyHybridSlashCommand(
+            name=self.name,
+            description=self.description,
+            group_name=name,
+            group_description=description,
+            scopes=self.scopes,
+            default_member_permissions=self.default_member_permissions,
+            dm_permission=self.dm_permission,
+            checks=self.checks.copy() if inherit_checks else [],
+            aliases=aliases or [],
+        )
+
+    def subcommand(
+        self,
+        sub_cmd_name: ipy.Absent[ipy.LocalisedName | str] = ipy.MISSING,
+        group_name: ipy.LocalisedName | str = None,
+        sub_cmd_description: ipy.Absent[ipy.LocalisedDesc | str] = ipy.MISSING,
+        group_description: ipy.Absent[ipy.LocalisedDesc | str] = ipy.MISSING,
+        options: list[typing.Union[ipy.SlashCommandOption, dict]] = None,
+        nsfw: bool = False,
+        inherit_checks: bool = True,
+        aliases: list[str] | None = None,
+        silence_autocomplete_errors: bool = True,
+    ) -> typing.Callable[..., "TansyHybridSlashCommand"]:
+        def wrapper(call: ipy.const.AsyncCallable) -> "TansyHybridSlashCommand":
+            nonlocal sub_cmd_name, sub_cmd_description
+
+            if not asyncio.iscoroutinefunction(call):
+                raise TypeError("Subcommand must be coroutine")
+
+            if sub_cmd_description is ipy.MISSING:
+                sub_cmd_description = call.__doc__ or "No Description Set"
+            if sub_cmd_name is ipy.MISSING:
+                sub_cmd_name = call.__name__
+
+            self._dummy_base = True
+            return TansyHybridSlashCommand(
+                name=self.name,
+                description=self.description,
+                group_name=group_name or self.group_name,
+                group_description=group_description or self.group_description,
+                sub_cmd_name=sub_cmd_name,
+                sub_cmd_description=sub_cmd_description,
+                default_member_permissions=self.default_member_permissions,
+                dm_permission=self.dm_permission,
+                options=options,
+                callback=call,
+                scopes=self.scopes,
+                nsfw=nsfw,
+                checks=self.checks.copy() if inherit_checks else [],
+                aliases=aliases or [],
+                silence_autocomplete_errors=silence_autocomplete_errors,
+            )
+
+        return wrapper
+
+
 def tansy_slash_command(
     name: ipy.Absent[str | ipy.LocalisedName] = ipy.MISSING,
     *,
     description: ipy.Absent[str | ipy.LocalisedDesc] = ipy.MISSING,
     scopes: ipy.Absent[typing.List["ipy.Snowflake_Type"]] = ipy.MISSING,
     default_member_permissions: typing.Optional["ipy.Permissions"] = None,
     dm_permission: bool = True,
@@ -528,10 +641,182 @@
             nsfw=nsfw,
         )
         return cmd
 
     return wrapper
 
 
+def tansy_hybrid_slash_command(
+    name: ipy.Absent[str | ipy.LocalisedName] = ipy.MISSING,
+    *,
+    aliases: typing.Optional[list[str]] = None,
+    description: ipy.Absent[str | ipy.LocalisedDesc] = ipy.MISSING,
+    scopes: ipy.Absent[list["ipy.Snowflake_Type"]] = ipy.MISSING,
+    options: typing.Optional[list[typing.Union[ipy.SlashCommandOption, dict]]] = None,
+    default_member_permissions: typing.Optional["ipy.Permissions"] = None,
+    dm_permission: bool = True,
+    sub_cmd_name: str | ipy.LocalisedName = None,
+    group_name: str | ipy.LocalisedName = None,
+    sub_cmd_description: str | ipy.LocalisedDesc = "No Description Set",
+    group_description: str | ipy.LocalisedDesc = "No Description Set",
+    nsfw: bool = False,
+    silence_autocomplete_errors: bool = False,
+) -> typing.Callable[[ipy.const.AsyncCallable], TansyHybridSlashCommand]:
+    """
+    A decorator to declare a coroutine as a Tansy hybrid slash command.
+
+    Hybrid commands are a slash command that can also function as a prefixed command.
+    These use a HybridContext instead of an SlashContext, but otherwise are mostly identical to normal slash commands.
+
+    Note that hybrid commands do not support autocompletes.
+    They also only partially support attachments, allowing one attachment option for a command.
+
+    !!! note
+        While the base and group descriptions arent visible in the discord client, currently.
+        We strongly advise defining them anyway, if you're using subcommands, as Discord has said they will be visible in
+        one of the future ui updates.
+
+    Args:
+        name: 1-32 character name of the command, defaults to the name of the coroutine.
+        aliases: Aliases for the prefixed command varient of the command. Has no effect on the slash command.
+        description: 1-100 character description of the command
+        scopes: The scope this command exists within
+        options: The parameters for the command, max 25
+        default_member_permissions: What permissions members need to have by default to use this command.
+        dm_permission: Should this command be available in DMs.
+        sub_cmd_name: 1-32 character name of the subcommand
+        sub_cmd_description: 1-100 character description of the subcommand
+        group_name: 1-32 character name of the group
+        group_description: 1-100 character description of the group
+        nsfw: This command should only work in NSFW channels
+        silence_autocomplete_errors: Should autocomplete errors be silenced. Don't use this unless you know what you're doing.
+
+    Returns:
+        TansyHybridSlashCommand Object
+
+    """
+
+    def wrapper(func: ipy.const.AsyncCallable) -> TansyHybridSlashCommand:
+        if not asyncio.iscoroutinefunction(func):
+            raise ValueError("Commands must be coroutines")
+
+        perm = default_member_permissions
+        if hasattr(func, "default_member_permissions"):
+            if perm:
+                perm = perm | func.default_member_permissions
+            else:
+                perm = func.default_member_permissions
+
+        _name = name
+        if _name is ipy.MISSING:
+            _name = func.__name__
+
+        _description = description
+        if _description is ipy.MISSING:
+            _description = func.__doc__ or "No Description Set"
+
+        cmd = TansyHybridSlashCommand(
+            name=_name,
+            group_name=group_name,
+            group_description=group_description,
+            sub_cmd_name=sub_cmd_name,
+            sub_cmd_description=sub_cmd_description,
+            description=_description,
+            scopes=scopes or [ipy.const.GLOBAL_SCOPE],
+            default_member_permissions=perm,
+            dm_permission=dm_permission,
+            callback=func,
+            options=options,
+            nsfw=nsfw,
+            aliases=aliases or [],
+            silence_autocomplete_errors=silence_autocomplete_errors,
+        )
+
+        return cmd
+
+    return wrapper
+
+
+def tansy_hybrid_slash_subcommand(
+    base: str | ipy.LocalisedName,
+    *,
+    subcommand_group: typing.Optional[str | ipy.LocalisedName] = None,
+    name: ipy.Absent[str | ipy.LocalisedName] = ipy.MISSING,
+    aliases: typing.Optional[list[str]] = None,
+    description: ipy.Absent[str | ipy.LocalisedDesc] = ipy.MISSING,
+    base_description: typing.Optional[str | ipy.LocalisedDesc] = None,
+    base_desc: typing.Optional[str | ipy.LocalisedDesc] = None,
+    base_default_member_permissions: typing.Optional["ipy.Permissions"] = None,
+    base_dm_permission: bool = True,
+    subcommand_group_description: typing.Optional[str | ipy.LocalisedDesc] = None,
+    sub_group_desc: typing.Optional[str | ipy.LocalisedDesc] = None,
+    scopes: list["ipy.Snowflake_Type"] = None,
+    options: list[dict] = None,
+    nsfw: bool = False,
+    silence_autocomplete_errors: bool = False,
+) -> typing.Callable[[ipy.const.AsyncCallable], TansyHybridSlashCommand]:
+    """
+    A decorator specifically tailored for creating Tansy hybrid slash subcommands.
+
+    Args:
+        base: The name of the base command
+        subcommand_group: The name of the subcommand group, if any.
+        name: The name of the subcommand, defaults to the name of the coroutine.
+        aliases: Aliases for the prefixed command varient of the subcommand. Has no effect on the slash command.
+        description: The description of the subcommand
+        base_description: The description of the base command
+        base_desc: An alias of `base_description`
+        base_default_member_permissions: What permissions members need to have by default to use this command.
+        base_dm_permission: Should this command be available in DMs.
+        subcommand_group_description: Description of the subcommand group
+        sub_group_desc: An alias for `subcommand_group_description`
+        scopes: The scopes of which this command is available, defaults to GLOBAL_SCOPE
+        options: The options for this command
+        nsfw: This command should only work in NSFW channels
+        silence_autocomplete_errors: Should autocomplete errors be silenced. Don't use this unless you know what you're doing.
+
+    Returns:
+        A TansyHybridSlashCommand object
+
+    """
+
+    def wrapper(func: ipy.const.AsyncCallable) -> TansyHybridSlashCommand:
+        if not asyncio.iscoroutinefunction(func):
+            raise ValueError("Commands must be coroutines")
+
+        _name = name
+        if _name is ipy.MISSING:
+            _name = func.__name__
+
+        _description = description
+        if _description is ipy.MISSING:
+            _description = func.__doc__ or "No Description Set"
+
+        cmd = TansyHybridSlashCommand(
+            name=base,
+            description=(base_description or base_desc) or "No Description Set",
+            group_name=subcommand_group,
+            group_description=(subcommand_group_description or sub_group_desc)
+            or "No Description Set",
+            sub_cmd_name=_name,
+            sub_cmd_description=_description,
+            default_member_permissions=base_default_member_permissions,
+            dm_permission=base_dm_permission,
+            scopes=scopes or [ipy.const.GLOBAL_SCOPE],
+            callback=func,
+            options=options,
+            nsfw=nsfw,
+            aliases=aliases or [],
+            silence_autocomplete_errors=silence_autocomplete_errors,
+        )
+        return cmd
+
+    return wrapper
+
+
 SlashCommand = TansySlashCommand
 slash_command = tansy_slash_command
 subcommand = tansy_subcommand
+
+HybridSlashCommand = TansyHybridSlashCommand
+hybrid_slash_command = tansy_hybrid_slash_command
+hybrid_slash_subcommand = tansy_hybrid_slash_subcommand
```

### Comparing `tansy-0.7.0/tansy/slash_param.py` & `tansy-0.8.0/tansy/slash_param.py`

 * *Files identical despite different names*

### Comparing `tansy-0.7.0/tansy/utils.py` & `tansy-0.8.0/tansy/utils.py`

 * *Files identical despite different names*

### Comparing `tansy-0.7.0/tansy.egg-info/PKG-INFO` & `tansy-0.8.0/tansy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tansy
-Version: 0.7.0
+Version: 0.8.0
 Summary: Unstable experiments with interactions.py.
 Home-page: https://github.com/Astrea49/tansy
 Author: AstreaTSS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

