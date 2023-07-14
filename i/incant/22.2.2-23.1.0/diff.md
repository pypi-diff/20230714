# Comparing `tmp/incant-22.2.2.tar.gz` & `tmp/incant-23.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incant-22.2.2.tar", last modified: Fri Dec 30 23:27:18 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `incant-22.2.2.tar` & `incant-23.1.0.tar`

### file list

```diff
@@ -1,7 +1,70 @@
--rw-r--r--   0        0        0    24079 2022-12-30 23:26:42.930341 incant-22.2.2/README.rst
--rw-r--r--   0        0        0      991 2022-12-30 23:26:33.402301 incant-22.2.2/pyproject.toml
--rw-r--r--   0        0        0    15169 2022-12-28 23:44:28.611889 incant-22.2.2/src/incant/__init__.py
--rw-r--r--   0        0        0     8823 2022-12-28 23:44:49.986644 incant-22.2.2/src/incant/_codegen.py
--rw-r--r--   0        0        0     1061 2022-12-28 23:36:41.848059 incant-22.2.2/src/incant/_compat.py
--rw-r--r--   0        0        0        0 2021-12-29 23:37:18.571000 incant-22.2.2/src/incant/py.typed
--rw-r--r--   0        0        0    25133 1970-01-01 00:00:00.000000 incant-22.2.2/PKG-INFO
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 incant-23.1.0/.coverage
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 incant-23.1.0/.pdm-python
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 incant-23.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 incant-23.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 incant-23.1.0/Makefile
+-rw-r--r--   0        0        0   124105 2020-02-02 00:00:00.000000 incant-23.1.0/pdm.lock
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 incant-23.1.0/tox.ini
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 incant-23.1.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 incant-23.1.0/_bench/Makefile
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 incant-23.1.0/_bench/single_dep.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 incant-23.1.0/_bench/two_deps.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 incant-23.1.0/docs/Makefile
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 incant-23.1.0/docs/changelog.md
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 incant-23.1.0/docs/conf.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 incant-23.1.0/docs/incant.rst
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 incant-23.1.0/docs/index.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 incant-23.1.0/docs/modules.rst
+-rw-r--r--   0        0        0    13865 2020-02-02 00:00:00.000000 incant-23.1.0/docs/tutorial.md
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 incant-23.1.0/docs/usage.md
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/custom.css
+-rw-r--r--   0        0        0    28948 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/roboto-v30-latin-ext_latin-700.woff
+-rw-r--r--   0        0        0    22580 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/roboto-v30-latin-ext_latin-700.woff2
+-rw-r--r--   0        0        0    30796 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/roboto-v30-latin-ext_latin-700italic.woff
+-rw-r--r--   0        0        0    24264 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/roboto-v30-latin-ext_latin-700italic.woff2
+-rw-r--r--   0        0        0    30960 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/roboto-v30-latin-ext_latin-italic.woff
+-rw-r--r--   0        0        0    24496 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/roboto-v30-latin-ext_latin-italic.woff2
+-rw-r--r--   0        0        0    28892 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/roboto-v30-latin-ext_latin-regular.woff
+-rw-r--r--   0        0        0    22560 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/roboto-v30-latin-ext_latin-regular.woff2
+-rw-r--r--   0        0        0    30388 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/ubuntu-mono-v15-latin-700.woff
+-rw-r--r--   0        0        0    25748 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/ubuntu-mono-v15-latin-700.woff2
+-rw-r--r--   0        0        0    32332 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/ubuntu-mono-v15-latin-700italic.woff
+-rw-r--r--   0        0        0    27824 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/ubuntu-mono-v15-latin-700italic.woff2
+-rw-r--r--   0        0        0    31508 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/ubuntu-mono-v15-latin-italic.woff
+-rw-r--r--   0        0        0    26600 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/ubuntu-mono-v15-latin-italic.woff2
+-rw-r--r--   0        0        0    32188 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/ubuntu-mono-v15-latin-regular.woff
+-rw-r--r--   0        0        0    27384 2020-02-02 00:00:00.000000 incant-23.1.0/docs/_static/fonts/ubuntu-mono-v15-latin-regular.woff2
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 incant-23.1.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    20650 2020-02-02 00:00:00.000000 incant-23.1.0/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0   132937 2020-02-02 00:00:00.000000 incant-23.1.0/htmlcov/d_4fe43248250da893___init___py.html
+-rw-r--r--   0        0        0    75060 2020-02-02 00:00:00.000000 incant-23.1.0/htmlcov/d_4fe43248250da893__codegen_py.html
+-rw-r--r--   0        0        0    15735 2020-02-02 00:00:00.000000 incant-23.1.0/htmlcov/d_4fe43248250da893__compat_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 incant-23.1.0/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 incant-23.1.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 incant-23.1.0/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 incant-23.1.0/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 incant-23.1.0/htmlcov/status.json
+-rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 incant-23.1.0/htmlcov/style.css
+-rw-r--r--   0        0        0    15402 2020-02-02 00:00:00.000000 incant-23.1.0/src/incant/__init__.py
+-rw-r--r--   0        0        0     8995 2020-02-02 00:00:00.000000 incant-23.1.0/src/incant/_codegen.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 incant-23.1.0/src/incant/_compat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incant-23.1.0/src/incant/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 incant-23.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 incant-23.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 incant-23.1.0/tests/quickapi.py
+-rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 incant-23.1.0/tests/test_dependencies.py
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 incant-23.1.0/tests/test_dependencies_async.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 incant-23.1.0/tests/test_forced_deps.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 incant-23.1.0/tests/test_incant.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 incant-23.1.0/tests/test_misc.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 incant-23.1.0/tests/test_overriding.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 incant-23.1.0/tests/test_params.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 incant-23.1.0/tests/test_passthrough.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 incant-23.1.0/tests/test_quickapi.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 incant-23.1.0/tests/test_string_annotations.py
+-rw-r--r--   0        0        0     8079 2020-02-02 00:00:00.000000 incant-23.1.0/tests/test_wired.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 incant-23.1.0/.gitignore
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 incant-23.1.0/LICENSE
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 incant-23.1.0/README.md
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 incant-23.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 incant-23.1.0/PKG-INFO
```

### Comparing `incant-22.2.2/src/incant/__init__.py` & `incant-23.1.0/src/incant/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ParameterDep,
     compile_incant_wrapper,
     compile_invoke,
 )
 from ._compat import NO_OVERRIDE, Override, get_annotated_override, signature
 
 
-__all__ = ["NO_OVERRIDE", "Override", "Hook", "Incanter"]
+__all__ = ["NO_OVERRIDE", "Override", "Hook", "Incanter", "IncantError"]
 
 _type = type
 
 
 R = TypeVar("R")
 
 
@@ -161,15 +161,15 @@
         if type is None:
             if isinstance(fn, _type):
                 type_to_reg = fn
             else:
                 sig = signature(fn)
                 type_to_reg = sig.return_annotation
                 if type_to_reg is Signature.empty:
-                    raise Exception("No return type found, provide a type.")
+                    raise IncantError("No return type found, provide a type.")
         else:
             type_to_reg = type
         self.register_hook(
             lambda p: is_subclass(p.annotation, type_to_reg), fn, is_ctx_manager
         )
         return fn
 
@@ -226,15 +226,15 @@
                 and (arg_name, arg.annotation) in kwargs
             ):
                 pos_arg_plan.append(arg_name)
                 found = True
             if found:
                 continue
 
-            elif arg.annotation is not Signature.empty:
+            if arg.annotation is not Signature.empty:
                 for ix, a in enumerate(pos_args_types):
                     if is_subclass(a, arg.annotation):
                         pos_arg_plan.append(ix)
                         found = True
                         break
             if found:
                 continue
@@ -252,18 +252,17 @@
         self,
         fn: Callable,
         pos_args_types: Tuple,
         kwargs_by_name_and_type: Set,
         is_async: Optional[bool] = False,
     ) -> Callable:
         plan = self._gen_incant_plan(fn, pos_args_types, kwargs_by_name_and_type)
-        incant = compile_incant_wrapper(
+        return compile_incant_wrapper(
             fn, plan, len(pos_args_types), len(kwargs_by_name_and_type)
         )
-        return incant
 
     def _gen_dep_tree(
         self,
         fn: Callable,
         additional_hooks: Sequence[Hook],
         forced_deps: Sequence[Tuple[Callable, Optional[CtxManagerKind]]] = (),
     ) -> List[Tuple[Callable, Optional[CtxManagerKind], List[Dep]]]:
@@ -297,14 +296,17 @@
                             # Match!
                             if hook.factory is None:
                                 dependents.append(
                                     ParameterDep(name, param_type, param.default)
                                 )
                             else:
                                 factory = hook.factory[0](param)
+                                if factory == node:
+                                    # A hook cannot satisfy itself.
+                                    continue
                                 if factory not in already_processed_hooks:
                                     to_process.append((factory, hook.factory[1]))
                                     already_processed_hooks.add(factory)
                                 dependents.append(
                                     FactoryDep(factory, name, hook.factory[1])
                                 )
 
@@ -390,18 +392,18 @@
                 # If there are multiple competing argument defs,
                 # we need to pick a winning type.
                 arg_type = Signature.empty
                 arg_default = Signature.empty
                 for arg in args:
                     try:
                         arg_type = _reconcile_types(arg_type, arg.type)
-                    except Exception:
-                        raise Exception(
+                    except Exception as exc:
+                        raise IncantError(
                             f"Unable to reconcile types {arg_type} and {arg.type} for argument {arg_name}"
-                        )
+                        ) from exc
                     if arg.default is not Signature.empty:
                         arg_default = arg.default
             outer_args.append(ParameterDep(arg_name, arg_type, arg_default))
 
         # outer_args need to be sorted by the presence of a default value
         outer_args.sort(key=lambda a: a.default is not Signature.empty)
 
@@ -433,7 +435,11 @@
 
 
 def _signature(f: Callable) -> Signature:
     """Return the signature of f, with potential overrides applied."""
     sig = signature(f)
     parameters = [get_annotated_override(val) for val in sig.parameters.values()]
     return sig.replace(parameters=parameters)
+
+
+class IncantError(Exception):
+    """An Incant error."""
```

### Comparing `incant-22.2.2/src/incant/_codegen.py` & `incant-23.1.0/src/incant/_codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,28 +35,31 @@
     outer_args: List[ParameterDep],
     invocations: List[Invocation],
     is_async: bool = False,
 ) -> Callable:
     """Generate the invocation wrapper for `fn`.
 
     :param fn_factory_args: Used names to avoid for local variables.
+    :param outer_args: Arguments that the generated function needs to retain.
 
     """
     # Some arguments need to be taken from outside.
     # Some arguments need to be calculated from factories.
     sig = signature(fn)
     fn_name = f"invoke_{fn.__name__}" if fn.__name__ != "<lambda>" else "invoke_lambda"
     globs: Dict[str, Any] = {}
     taken_local_vars = set()
     arg_lines = []
 
     for dep in outer_args:
         if dep.type is not Signature.empty:
-            type_name = dep.type.__name__
-            if type_name not in globs or globs[type_name] is dep.type:
+            # Some types, like new unions (`int|str`), do not have names.
+            if (type_name := getattr(dep.type, "__name__", None)) and (
+                type_name not in globs or globs[type_name] is dep.type
+            ):
                 arg_type_snippet = f": {type_name}"
                 globs[type_name] = dep.type
             else:
                 arg_type_snippet = f": _incant_arg_{dep.arg_name}"
                 globs[f"_incant_arg_{dep.arg_name}"] = dep.type
         else:
             arg_type_snippet = ""
@@ -151,15 +154,14 @@
                     local_counter += 1
                 else:
                     lines.append(
                         f"  {' ' * ind}{aw}with {global_fn_name}({', '.join(local_arg_lines)}):"
                     )
                 ind += 2
             else:
-
                 aw = "await " if iscoroutinefunction(invoc.factory) else ""
                 if not invoc.is_forced:
                     lines.append(
                         f"  {' ' * ind}{local_name} = {aw}{global_fn_name}({', '.join(local_arg_lines)})"
                     )
                     local_counter += 1
                 else:
@@ -197,16 +199,15 @@
     lines.append(f"  {' ' * ind}return {aw}{inner_name}({', '.join(incant_arg_lines)})")
 
     script = "\n".join(lines)
 
     fname = _generate_unique_filename(fn.__name__, "invoke", lines)
     eval(compile(script, fname, "exec"), globs)
 
-    fn = globs[fn_name]
-    return fn
+    return globs[fn_name]
 
 
 def compile_incant_wrapper(
     fn: Callable, incant_plan: List[Union[int, str]], num_pos_args: int, num_kwargs: int
 ):
     fn_name = f"incant_{fn.__name__}" if fn.__name__ != "<lambda>" else "incant_lambda"
     globs = {"_incant_inner_fn": fn}
@@ -230,16 +231,15 @@
     lines.append("  )")
 
     script = "\n".join(lines)
 
     fname = _generate_unique_filename(fn.__name__, "incant", lines)
     eval(compile(script, fname, "exec"), globs)
 
-    fn = globs[fn_name]
-    return fn
+    return globs[fn_name]
 
 
 def _generate_unique_filename(func_name: str, func_type: str, source: List[str]) -> str:
     """
     Create a "filename" suitable for a function being generated.
     """
     extra = ""
```

### Comparing `incant-22.2.2/src/incant/_compat.py` & `incant-23.1.0/src/incant/_compat.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 if sys.version_info >= (3, 9):
     from typing import _AnnotatedAlias  # type: ignore
 
 else:
     from typing_extensions import _AnnotatedAlias
 
 if sys.version_info >= (3, 10):
-
     signature = partial(sig, eval_str=True)
 
 else:
     signature = sig
 
 
 def get_annotated_override(p: Parameter) -> Parameter:
```

