# Comparing `tmp/zeugvars-0.2.6.tar.gz` & `tmp/zeugvars-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeugvars-0.2.6.tar", max compression
+gzip compressed data, was "zeugvars-0.2.7.tar", max compression
```

## Comparing `zeugvars-0.2.6.tar` & `zeugvars-0.2.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.2.6/LICENSE
--rw-r--r--   0        0        0     3450 2023-07-04 18:59:26.237845 zeugvars-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     4160 2023-07-04 18:43:08.544957 zeugvars-0.2.6/README.md
--rw-r--r--   0        0        0    10756 2023-07-04 18:57:13.132379 zeugvars-0.2.6/zeugvars/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 10:15:47.964651 zeugvars-0.2.6/zeugvars/py.typed
--rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 zeugvars-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-29 20:37:00.152930 zeugvars-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3450 2023-07-13 23:31:25.624178 zeugvars-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     4160 2023-07-04 18:43:08.544957 zeugvars-0.2.7/README.md
+-rw-r--r--   0        0        0     9514 2023-07-13 23:31:16.860583 zeugvars-0.2.7/zeugvars/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 10:15:47.964651 zeugvars-0.2.7/zeugvars/py.typed
+-rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 zeugvars-0.2.7/PKG-INFO
```

### Comparing `zeugvars-0.2.6/LICENSE` & `zeugvars-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zeugvars-0.2.6/pyproject.toml` & `zeugvars-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeugvars"
-version = "0.2.6"
+version = "0.2.7"
 description = "A simple & straight-forward Python module for creating context-dependent proxy objects."
 authors = ["bswck <bswck.dev@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/bswck/zeugvars"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `zeugvars-0.2.6/README.md` & `zeugvars-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `zeugvars-0.2.6/zeugvars/__init__.py` & `zeugvars-0.2.7/zeugvars/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,330 +1,301 @@
-"""`zeugvars`.
-
-A simple & straight-forward Python library for creating context-dependent proxy objects.
-
-(C) bswck, 2023
-"""
-
-from collections.abc import Callable
-from contextlib import suppress
-from functools import partial
-from typing import Any, Protocol, TypeVar, cast, runtime_checkable
-
-__all__ = ("zeugvar", "proxy")
-
-_T = TypeVar("_T")
-
-
-@runtime_checkable
-class Manager(Protocol[_T]):
-    """Protocol for zeugvars managers.
-
-    Matches `contextvars.ContextVar`.
-    """
-
-    def get(self) -> _T:
-        """Get the current value of the manager.
-
-        Raises
-        ------
-        LookupError
-            If no object is bound to the manager.
-        """
-
-    def set(self, value: _T) -> Any:
-        """Set the current value of the manager."""
-
-
-def zeugvar_descriptor(
-    cls: type[_T] | None,
-    mgr: Manager[_T],
-    getter: Callable[[Manager[_T]], _T],
-    setter: Callable[[Manager[_T], _T], None],
-    *,
-    undefined: Callable[..., Any] | None = None,
-    fallback: Callable[..., Any] | None = None,
-    custom_mro: bool = False,
-    inplace: bool = False,
-) -> Any:
-    """Descriptor factory for zeugvars.
-
-    Parameters
-    ----------
-    cls
-        The class of the underlying variable accessed within the manager.
-    mgr
-        Manager object.
-    getter
-        A function that returns the underlying variable from the manager.
-    setter
-        A function that sets the underlying variable within the manager.
-    undefined
-        Callable to be used as a fallback in case the variable is undefined
-        (manager raises a `LookupError`).
-    fallback
-        Callable to be used as a fallback in case the attribute is undefined
-        (the underlying variable raises an `AttributeError`).
-    custom_mro
-        Whether the class implements a custom `mro()` method.
-    inplace
-        Whether to treat the attribute as an inplace operator.
-        Calls the setter with the result of the attribute call.
-
-    Returns
-    -------
-    descriptor
-        A descriptor object that can be used to create zeugvars delegates.
-
-    """
-
-    class _ZeugVarDescriptor:
-        attr_name: str
-
-        def __init__(self) -> None:
-            self.attr_name = None  # type: ignore[assignment]
-
-        def __set_name__(self, owner: type[_T], name: str) -> None:
-            self.attr_name = name
-
-        def __get__(self, instance: _T, owner: type[_T] | None) -> Any:
-            if self.attr_name == "__getattr__":
-
-                def attribute(name: str) -> Any:
-                    return getattr(getter(mgr), name)
-
-            elif self.attr_name in ("__repr__", "__str__"):
-                with suppress(RuntimeError):
-                    return getattr(getter(mgr), self.attr_name)
-
-                def attribute() -> str:  # type: ignore[misc]
-                    if cls is None:
-                        return "<unbound zeugvar>"
-                    return f"<unbound {cls.__name__!r} object>"
-
-            else:
-                try:
-                    obj = getter(mgr)
-                except RuntimeError:
-                    if self.attr_name == "__dir__" and not custom_mro:
-
-                        def attribute() -> list[str]:  # type: ignore[misc]
-                            return list(set(dir(cls)) - {"mro"})
-
-                    elif callable(undefined):
-                        attribute = undefined
-
-                    else:
-                        raise
-                else:
-                    try:
-                        attribute = getattr(obj, self.attr_name)
-                    except AttributeError:
-                        if not callable(fallback):
-                            raise
-
-                        attribute = partial(fallback, obj)
-
-            if inplace:
-                def _apply_inplace(*args: Any, **kwargs: Any) -> _T:
-                    ret = attribute(*args, **kwargs)
-                    setter(mgr, ret)
-                    return instance
-
-                return _apply_inplace
-            return attribute
-
-        def __set__(self, instance: _T, value: Any) -> None:
-            setattr(getter(mgr), self.attr_name, value)
-
-        def __delete__(self, instance: _T) -> None:
-            delattr(getter(mgr), self.attr_name)
-
-    return _ZeugVarDescriptor()
-
-
-def _op_fallback(op_name: str) -> Callable[[Any, Any], Any]:
-    return lambda obj, op: getattr(obj, op_name)(op)
-
-
-def _cv_getter(mgr: Manager[_T]) -> _T:
-    try:
-        obj = mgr.get()
-    except LookupError:
-        msg = f"No object in {mgr}"
-        raise RuntimeError(msg) from None
-    return obj
-
-
-def _cv_setter(mgr: Manager[_T], value: _T) -> None:
-    mgr.set(value)
-
-
-def zeugvar(
-    mgr: Manager[_T],
-    cls: type[_T] | None = None,
-    getter: Callable[[Manager[_T]], _T] = None,  # type: ignore[assignment]
-    setter: Callable[[Manager[_T], _T], None] = None,  # type: ignore[assignment]
-) -> _T:
-    """Create a zeugvar proxy object.
-
-    Parameters
-    ----------
-    mgr
-        Manager object. Must implement the `Manager` protocol.
-        Matches `contextvars.ContextVar`.
-    cls
-        The class of the underlying variable accessed within the manager.
-    getter
-        A function that returns the underlying variable from the manager.
-    setter
-        A function that sets the underlying variable within the manager.
-
-    Returns
-    -------
-    proxy
-        A proxy object.
-    """
-
-    # pylint: disable=too-many-statements
-
-    if getter is None:
-        getter = _cv_getter
-
-    if setter is None:
-        setter = _cv_setter
-
-    if cls is None:
-        with suppress(RuntimeError):
-            cls = type(getter(mgr))
-
-    if cls is None:
-        custom_mro = False
-
-        def mro() -> list[type[Any]]:
-            return [object]
-
-    else:
-        mro: Callable[[], list[type[Any]]] = object.__getattribute__(cls, "mro")
-        custom_mro = not hasattr(mro, "__self__")
-
-    descriptor = partial(
-        zeugvar_descriptor, cls, mgr, getter, setter, custom_mro=custom_mro,
-    )
-
-    class _ZeugVarMeta(type):
-        __doc__ = descriptor()
-        __wrapped__ = descriptor()
-        __repr__ = descriptor()
-        __str__ = descriptor()
-        __bytes__ = descriptor()
-        __format__ = descriptor()
-        __lt__ = descriptor()
-        __le__ = descriptor()
-        __eq__ = descriptor()
-        __ne__ = descriptor()
-        __gt__ = descriptor()
-        __ge__ = descriptor()
-        __hash__ = descriptor()
-        __bool__ = descriptor(undefined=lambda: False)
-        __getattr__ = descriptor()
-        __setattr__ = descriptor()
-        __delattr__ = descriptor()
-        if cls is None:
-            __dir__ = descriptor()
-            __class__ = descriptor()
-        else:
-            __dir__ = descriptor(undefined=lambda: dir(cls))
-            __class__ = descriptor(undefined=lambda: cls)
-        __instancecheck__ = descriptor()
-        __subclasscheck__ = descriptor()
-        __call__ = descriptor()
-        __len__ = descriptor()
-        __length_hint__ = descriptor()
-        __getitem__ = descriptor()
-        __setitem__ = descriptor()
-        __delitem__ = descriptor()
-        __iter__ = descriptor()
-        __next__ = descriptor()
-        __reversed__ = descriptor()
-        __contains__ = descriptor()
-        __add__ = descriptor()
-        __sub__ = descriptor()
-        __mul__ = descriptor()
-        __matmul__ = descriptor()
-        __truediv__ = descriptor()
-        __floordiv__ = descriptor()
-        __mod__ = descriptor()
-        __divmod__ = descriptor()
-        __pow__ = descriptor()
-        __lshift__ = descriptor()
-        __rshift__ = descriptor()
-        __and__ = descriptor()
-        __xor__ = descriptor()
-        __or__ = descriptor()
-        __radd__ = descriptor()
-        __rsub__ = descriptor()
-        __rmul__ = descriptor()
-        __rmatmul__ = descriptor()
-        __rtruediv__ = descriptor()
-        __rfloordiv__ = descriptor()
-        __rmod__ = descriptor()
-        __rdivmod__ = descriptor()
-        __rpow__ = descriptor()
-        __rlshift__ = descriptor()
-        __rrshift__ = descriptor()
-        __rand__ = descriptor()
-        __rxor__ = descriptor()
-        __ror__ = descriptor()
-        __iadd__ = descriptor(fallback=_op_fallback("__add__"), inplace=True)
-        __isub__ = descriptor(fallback=_op_fallback("__sub__"), inplace=True)
-        __imul__ = descriptor(fallback=_op_fallback("__mul__"), inplace=True)
-        __imatmul__ = descriptor(fallback=_op_fallback("__matmul__"), inplace=True)
-        __itruediv__ = descriptor(fallback=_op_fallback("__truediv__"), inplace=True)
-        __ifloordiv__ = descriptor(fallback=_op_fallback("__floordiv__"), inplace=True)
-        __imod__ = descriptor(fallback=_op_fallback("__mod__"), inplace=True)
-        __ipow__ = descriptor(fallback=_op_fallback("__pow__"), inplace=True)
-        __ilshift__ = descriptor(fallback=_op_fallback("__lshift_"), inplace=True)
-        __irshift__ = descriptor(fallback=_op_fallback("__rshift__"), inplace=True)
-        __iand__ = descriptor(fallback=_op_fallback("__and__"), inplace=True)
-        __ixor__ = descriptor(fallback=_op_fallback("__xor__"), inplace=True)
-        __ior__ = descriptor(fallback=_op_fallback("__or__"), inplace=True)
-        __neg__ = descriptor()
-        __pos__ = descriptor()
-        __abs__ = descriptor()
-        __invert__ = descriptor()
-        __complex__ = descriptor()
-        __int__ = descriptor()
-        __float__ = descriptor()
-        __index__ = descriptor()
-        __round__ = descriptor()
-        __trunc__ = descriptor()
-        __floor__ = descriptor()
-        __ceil__ = descriptor()
-        __enter__ = descriptor()
-        __exit__ = descriptor()
-        __await__ = descriptor()
-        __aiter__ = descriptor()
-        __anext__ = descriptor()
-        __aenter__ = descriptor()
-        __aexit__ = descriptor()
-        __copy__ = descriptor()
-        __deepcopy__ = descriptor()
-
-    cls_name = cls.__name__ if cls is not None else f"zeugvar_{id(mgr):x}"
-
-    zv_proxy = cast(_T, _ZeugVarMeta(cls_name, (), {}))
-    if not custom_mro:
-
-        def _mro_wrapper() -> list[type[Any]]:
-            try:
-                obj = getter(mgr)
-            except RuntimeError:
-                return mro()
-            msg = f"{type(obj).__name__!r} object has no attribute 'mro'"
-            raise AttributeError(msg) from None
-
-        type.__setattr__(zv_proxy, "mro", _mro_wrapper)
-    return zv_proxy
-
-
-proxy = zeugvar
+"""`zeugvars`.
+
+A simple & straight-forward Python library for creating context-dependent proxy objects.
+
+(C) bswck, 2023
+"""
+
+from collections.abc import Callable
+from contextlib import suppress
+from functools import partial
+from typing import Any, Protocol, TypeVar, cast, runtime_checkable
+
+__all__ = ("zeugvar", "proxy")
+
+_T = TypeVar("_T")
+
+
+@runtime_checkable
+class Manager(Protocol[_T]):
+    """Protocol for zeugvars managers.
+
+    Matches `contextvars.ContextVar`.
+    """
+
+    def get(self) -> _T:
+        """Get the current value of the manager.
+
+        Raises
+        ------
+        LookupError
+            If no object is bound to the manager.
+        """
+
+    def set(self, value: _T) -> Any:
+        """Set the current value of the manager."""
+
+
+def zeugvar_descriptor(
+    cls: type[_T] | None,
+    mgr: Manager[_T],
+    getter: Callable[[Manager[_T]], _T],
+    setter: Callable[[Manager[_T], _T], None],
+    *,
+    undefined: Callable[..., Any] | None = None,
+    fallback: Callable[..., Any] | None = None,
+    inplace: bool = False,
+) -> Any:
+    """Descriptor factory for zeugvars.
+
+    Parameters
+    ----------
+    cls
+        The class of the underlying variable accessed within the manager.
+    mgr
+        Manager object.
+    getter
+        A function that returns the underlying variable from the manager.
+    setter
+        A function that sets the underlying variable within the manager.
+    undefined
+        Callable to be used as a fallback in case the variable is undefined
+        (manager raises a `LookupError`).
+    fallback
+        Callable to be used as a fallback in case the attribute is undefined
+        (the underlying variable raises an `AttributeError`).
+    inplace
+        Whether to treat the attribute as an inplace operator.
+        Calls the setter with the result of the attribute call.
+
+    Returns
+    -------
+    descriptor
+        A descriptor object that can be used to create zeugvars delegates.
+
+    """
+
+    class _ZeugVarDescriptor:
+        attr_name: str
+
+        def __init__(self) -> None:
+            self.attr_name = None  # type: ignore[assignment]
+
+        def __set_name__(self, owner: type[_T], name: str) -> None:
+            self.attr_name = name
+
+        def __get__(self, instance: _T, owner: type[_T] | None) -> Any:
+            if self.attr_name == "__getattr__":
+
+                def attribute(name: str) -> Any:
+                    return getattr(getter(mgr), name)
+
+            elif self.attr_name in ("__repr__", "__str__"):
+                with suppress(RuntimeError):
+                    return getattr(getter(mgr), self.attr_name)
+
+                def attribute() -> str:  # type: ignore[misc]
+                    if cls is None:
+                        return "<unbound zeugvar>"
+                    return f"<unbound {cls.__name__!r} object>"
+
+            else:
+                try:
+                    obj = getter(mgr)
+                except RuntimeError:
+                    if callable(undefined):
+                        attribute = undefined
+
+                    else:
+                        raise
+                else:
+                    try:
+                        attribute = getattr(obj, self.attr_name)
+                    except AttributeError:
+                        if not callable(fallback):
+                            raise
+
+                        attribute = partial(fallback, obj)
+
+            if inplace:
+
+                def _apply_inplace(*args: Any, **kwargs: Any) -> _T:
+                    ret = attribute(*args, **kwargs)
+                    setter(mgr, ret)
+                    return instance
+
+                return _apply_inplace
+            return attribute
+
+        def __set__(self, instance: _T, value: Any) -> None:
+            setattr(getter(mgr), self.attr_name, value)
+
+        def __delete__(self, instance: _T) -> None:
+            delattr(getter(mgr), self.attr_name)
+
+    return _ZeugVarDescriptor()
+
+
+def _op_fallback(op_name: str) -> Callable[[Any, Any], Any]:
+    return lambda obj, op: getattr(obj, op_name)(op)
+
+
+def _cv_getter(mgr: Manager[_T]) -> _T:
+    try:
+        obj = mgr.get()
+    except LookupError:
+        msg = f"No object in {mgr}"
+        raise RuntimeError(msg) from None
+    return obj
+
+
+def _cv_setter(mgr: Manager[_T], value: _T) -> None:
+    mgr.set(value)
+
+
+def zeugvar(
+    mgr: Manager[_T],
+    cls: type[_T] | None = None,
+    getter: Callable[[Manager[_T]], _T] = None,  # type: ignore[assignment]
+    setter: Callable[[Manager[_T], _T], None] = None,  # type: ignore[assignment]
+) -> _T:
+    """Create a zeugvar proxy object.
+
+    Parameters
+    ----------
+    mgr
+        Manager object. Must implement the `Manager` protocol.
+        Matches `contextvars.ContextVar`.
+    cls
+        The class of the underlying variable accessed within the manager.
+    getter
+        A function that returns the underlying variable from the manager.
+    setter
+        A function that sets the underlying variable within the manager.
+
+    Returns
+    -------
+    proxy
+        A proxy object.
+    """
+
+    # pylint: disable=too-many-statements
+
+    if getter is None:
+        getter = _cv_getter
+
+    if setter is None:
+        setter = _cv_setter
+
+    if cls is None:
+        with suppress(RuntimeError):
+            cls = type(getter(mgr))
+
+    descriptor = partial(zeugvar_descriptor, cls, mgr, getter, setter)
+
+    class _ZeugVarMeta:
+        __doc__ = descriptor()
+        __wrapped__ = descriptor()
+        __repr__ = descriptor()
+        __str__ = descriptor()
+        __bytes__ = descriptor()
+        __format__ = descriptor()
+        __lt__ = descriptor()
+        __le__ = descriptor()
+        __eq__ = descriptor()
+        __ne__ = descriptor()
+        __gt__ = descriptor()
+        __ge__ = descriptor()
+        __hash__ = descriptor()
+        __bool__ = descriptor(undefined=lambda: False)
+        __getattr__ = descriptor()
+        __setattr__ = descriptor()
+        __delattr__ = descriptor()
+        if cls is None:
+            __dir__ = descriptor()
+            __class__ = descriptor()
+        else:
+            __dir__ = descriptor(undefined=lambda: dir(cls))
+            __class__ = descriptor(undefined=lambda: cls)
+        __call__ = descriptor()
+        __instancecheck__ = descriptor()
+        __subclasscheck__ = descriptor()
+        __len__ = descriptor()
+        __length_hint__ = descriptor()
+        __getitem__ = descriptor()
+        __setitem__ = descriptor()
+        __delitem__ = descriptor()
+        __iter__ = descriptor()
+        __next__ = descriptor()
+        __reversed__ = descriptor()
+        __contains__ = descriptor()
+        __add__ = descriptor()
+        __sub__ = descriptor()
+        __mul__ = descriptor()
+        __matmul__ = descriptor()
+        __truediv__ = descriptor()
+        __floordiv__ = descriptor()
+        __mod__ = descriptor()
+        __divmod__ = descriptor()
+        __pow__ = descriptor()
+        __lshift__ = descriptor()
+        __rshift__ = descriptor()
+        __and__ = descriptor()
+        __xor__ = descriptor()
+        __or__ = descriptor()
+        __radd__ = descriptor()
+        __rsub__ = descriptor()
+        __rmul__ = descriptor()
+        __rmatmul__ = descriptor()
+        __rtruediv__ = descriptor()
+        __rfloordiv__ = descriptor()
+        __rmod__ = descriptor()
+        __rdivmod__ = descriptor()
+        __rpow__ = descriptor()
+        __rlshift__ = descriptor()
+        __rrshift__ = descriptor()
+        __rand__ = descriptor()
+        __rxor__ = descriptor()
+        __ror__ = descriptor()
+        __iadd__ = descriptor(fallback=_op_fallback("__add__"), inplace=True)
+        __isub__ = descriptor(fallback=_op_fallback("__sub__"), inplace=True)
+        __imul__ = descriptor(fallback=_op_fallback("__mul__"), inplace=True)
+        __imatmul__ = descriptor(fallback=_op_fallback("__matmul__"), inplace=True)
+        __itruediv__ = descriptor(fallback=_op_fallback("__truediv__"), inplace=True)
+        __ifloordiv__ = descriptor(fallback=_op_fallback("__floordiv__"), inplace=True)
+        __imod__ = descriptor(fallback=_op_fallback("__mod__"), inplace=True)
+        __ipow__ = descriptor(fallback=_op_fallback("__pow__"), inplace=True)
+        __ilshift__ = descriptor(fallback=_op_fallback("__lshift_"), inplace=True)
+        __irshift__ = descriptor(fallback=_op_fallback("__rshift__"), inplace=True)
+        __iand__ = descriptor(fallback=_op_fallback("__and__"), inplace=True)
+        __ixor__ = descriptor(fallback=_op_fallback("__xor__"), inplace=True)
+        __ior__ = descriptor(fallback=_op_fallback("__or__"), inplace=True)
+        __neg__ = descriptor()
+        __pos__ = descriptor()
+        __abs__ = descriptor()
+        __invert__ = descriptor()
+        __complex__ = descriptor()
+        __int__ = descriptor()
+        __float__ = descriptor()
+        __index__ = descriptor()
+        __round__ = descriptor()
+        __trunc__ = descriptor()
+        __floor__ = descriptor()
+        __ceil__ = descriptor()
+        __enter__ = descriptor()
+        __exit__ = descriptor()
+        __await__ = descriptor()
+        __aiter__ = descriptor()
+        __anext__ = descriptor()
+        __aenter__ = descriptor()
+        __aexit__ = descriptor()
+        __copy__ = descriptor()
+        __deepcopy__ = descriptor()
+
+    if cls is not None:
+        _ZeugVarMeta.__name__ = _ZeugVarMeta.__qualname__ = cls.__name__
+    else:
+        _ZeugVarMeta.__name__ = _ZeugVarMeta.__qualname__ = f"zeugvar_{id(mgr):x}"
+    return cast(_T, _ZeugVarMeta())
+
+
+proxy = zeugvar
```

### Comparing `zeugvars-0.2.6/PKG-INFO` & `zeugvars-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeugvars
-Version: 0.2.6
+Version: 0.2.7
 Summary: A simple & straight-forward Python module for creating context-dependent proxy objects.
 Home-page: https://github.com/bswck/zeugvars
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

