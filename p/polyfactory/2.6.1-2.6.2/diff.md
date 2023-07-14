# Comparing `tmp/polyfactory-2.6.1.tar.gz` & `tmp/polyfactory-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.6.1.tar", max compression
+gzip compressed data, was "polyfactory-2.6.2.tar", max compression
```

## Comparing `polyfactory-2.6.1.tar` & `polyfactory-2.6.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1092 2023-07-10 17:12:49.123486 polyfactory-2.6.1/LICENSE
--rw-r--r--   0        0        0    24136 2023-07-10 17:12:49.123486 polyfactory-2.6.1/docs/PYPI_README.md
--rw-r--r--   0        0        0      425 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/__init__.py
--rw-r--r--   0        0        0     2525 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/collection_extender.py
--rw-r--r--   0        0        0      912 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    33696 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2758 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1912 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     2751 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/factories/msgspec_factory.py
--rw-r--r--   0        0        0     2192 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0    13500 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1650 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     8230 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3317 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/fields.py
--rw-r--r--   0        0        0     1192 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/py.typed
--rw-r--r--   0        0        0     2850 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     3852 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3764 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     1948 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1885 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1125 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13429 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0      433 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/value_generators/constrained_path.py
--rw-r--r--   0        0        0     3846 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0      440 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/value_generators/constrained_url.py
--rw-r--r--   0        0        0      446 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/value_generators/constrained_uuid.py
--rw-r--r--   0        0        0     3635 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6172 2023-07-10 17:12:49.127486 polyfactory-2.6.1/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6900 2023-07-10 17:12:49.127486 polyfactory-2.6.1/pyproject.toml
--rw-r--r--   0        0        0    26005 1970-01-01 00:00:00.000000 polyfactory-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-14 15:44:51.527690 polyfactory-2.6.2/LICENSE
+-rw-r--r--   0        0        0    24136 2023-07-14 15:44:51.527690 polyfactory-2.6.2/docs/PYPI_README.md
+-rw-r--r--   0        0        0      425 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/__init__.py
+-rw-r--r--   0        0        0     2525 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/collection_extender.py
+-rw-r--r--   0        0        0      912 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    33713 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2758 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1912 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     2751 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/msgspec_factory.py
+-rw-r--r--   0        0        0     2192 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0    13803 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1699 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     8246 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3317 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/fields.py
+-rw-r--r--   0        0        0     1192 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/py.typed
+-rw-r--r--   0        0        0     2850 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     3908 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3764 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     1948 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1885 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1125 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13429 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0      433 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_path.py
+-rw-r--r--   0        0        0     3846 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0      440 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_url.py
+-rw-r--r--   0        0        0      446 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/constrained_uuid.py
+-rw-r--r--   0        0        0     3635 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6172 2023-07-14 15:44:51.531690 polyfactory-2.6.2/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6777 2023-07-14 15:44:51.531690 polyfactory-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0    26005 1970-01-01 00:00:00.000000 polyfactory-2.6.2/PKG-INFO
```

### Comparing `polyfactory-2.6.1/LICENSE` & `polyfactory-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/docs/PYPI_README.md` & `polyfactory-2.6.2/docs/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/collection_extender.py` & `polyfactory-2.6.2/polyfactory/collection_extender.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/constants.py` & `polyfactory-2.6.2/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/decorators.py` & `polyfactory-2.6.2/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/exceptions.py` & `polyfactory-2.6.2/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/factories/base.py` & `polyfactory-2.6.2/polyfactory/factories/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,15 +398,15 @@
         """Seed faker and random with the given integer.
 
         :param seed: An integer to set as seed.
         :returns: 'None'
 
         """
         cls.__random__.seed(seed, version=3)
-        Faker.seed(seed)
+        cls.__faker__.seed_instance(seed)
 
     @classmethod
     def is_ignored_type(cls, value: Any) -> bool:
         """Check whether a given value is an ignored type.
 
         :param value: An arbitrary value.
```

### Comparing `polyfactory-2.6.1/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.6.2/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.6.2/polyfactory/factories/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/factories/msgspec_factory.py` & `polyfactory-2.6.2/polyfactory/factories/msgspec_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.6.2/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.6.2/polyfactory/factories/pydantic_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from __future__ import annotations
 
 from contextlib import suppress
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
+    ForwardRef,
     Generic,
     Mapping,
     Tuple,
     TypeVar,
     cast,
 )
 
 from typing_extensions import Literal, get_args, get_origin
 
 from polyfactory.collection_extender import CollectionExtender
-from polyfactory.constants import MAX_COLLECTION_LENGTH, MIN_COLLECTION_LENGTH, RANDOMIZE_COLLECTION_LENGTH
+from polyfactory.constants import (
+    DEFAULT_RANDOM,
+    MAX_COLLECTION_LENGTH,
+    MIN_COLLECTION_LENGTH,
+    RANDOMIZE_COLLECTION_LENGTH,
+)
 from polyfactory.exceptions import MissingDependencyException
 from polyfactory.factories.base import BaseFactory
 from polyfactory.field_meta import Constraints, FieldMeta, Null
 from polyfactory.utils.helpers import unwrap_new_type, unwrap_optional
 from polyfactory.utils.predicates import is_optional_union, is_safe_subclass
 
 try:
@@ -48,15 +54,15 @@
 
     @classmethod
     def from_field_info(
         cls,
         field_name: str,
         field_info: FieldInfo,
         use_alias: bool,
-        random: Random,
+        random: Random | None,
         randomize_collection_length: bool = RANDOMIZE_COLLECTION_LENGTH,
         min_collection_length: int = MIN_COLLECTION_LENGTH,
         max_collection_length: int = MAX_COLLECTION_LENGTH,
     ) -> PydanticFieldMeta:
         """Create an instance from a pydantic field info.
 
         :param field_name: The name of the field.
@@ -87,41 +93,40 @@
 
         if "url" in constraints:
             # pydantic uses a sentinel value for url constraints
             annotation = str
 
         return PydanticFieldMeta.from_type(
             name=name,
-            random=random,
+            random=random or DEFAULT_RANDOM,
             annotation=annotation,
             default=default_value,
             constraints=cast("Constraints", {k: v for k, v in constraints.items() if v is not None}) or None,
             randomize_collection_length=randomize_collection_length,
             min_collection_length=min_collection_length,
             max_collection_length=max_collection_length,
         )
 
     @classmethod
     def from_model_field(  # pragma: no cover
         cls,
         model_field: ModelField,  # pyright: ignore
         use_alias: bool,
-        random: Random,
         randomize_collection_length: bool,
         min_collection_length: int,
         max_collection_length: int,
+        random: Random = DEFAULT_RANDOM,
     ) -> PydanticFieldMeta:
         """Create an instance from a pydantic model field.
-
         :param model_field: A pydantic ModelField.
         :param use_alias: Whether to use the field alias.
-        :param random: An instance of random.Random.
         :param randomize_collection_length: A boolean flag whether to randomize collections lengths
         :param min_collection_length: Minimum number of elements in randomized collection
         :param max_collection_length: Maximum number of elements in randomized collection
+        :param random: An instance of random.Random.
 
         :returns: A PydanticFieldMeta instance.
 
         """
         from pydantic import AmqpDsn, AnyHttpUrl, AnyUrl, HttpUrl, KafkaDsn, PostgresDsn, RedisDsn
         from pydantic.fields import DeferredType, Undefined  # type: ignore
 
@@ -133,15 +138,15 @@
             default_value = model_field.default if model_field.default is not Undefined else Null
 
         name = model_field.alias if model_field.alias and use_alias else model_field.name
 
         outer_type = unwrap_new_type(model_field.outer_type_)
         annotation = (
             model_field.outer_type_
-            if isinstance(model_field.annotation, DeferredType)
+            if isinstance(model_field.annotation, (DeferredType, ForwardRef))
             else unwrap_new_type(model_field.annotation)
         )
 
         constraints = cast(
             "Constraints",
             {
                 "ge": getattr(outer_type, "ge", model_field.field_info.ge),
@@ -205,27 +210,27 @@
             type_arg_to_sub_field = dict(zip(type_args, fields_to_iterate))
             if get_origin(outer_type) in (tuple, Tuple) and get_args(outer_type)[-1] == Ellipsis:
                 # pydantic removes ellipses from Tuples in sub_fields
                 type_args += (...,)
             extended_type_args = CollectionExtender.extend_type_args(annotation, type_args, number_of_args)
             children.extend(
                 PydanticFieldMeta.from_model_field(
-                    type_arg_to_sub_field[arg],
-                    use_alias,
-                    random,
-                    randomize_collection_length,
-                    min_collection_length,
-                    max_collection_length,
+                    model_field=type_arg_to_sub_field[arg],
+                    use_alias=use_alias,
+                    random=random,
+                    randomize_collection_length=randomize_collection_length,
+                    min_collection_length=min_collection_length,
+                    max_collection_length=max_collection_length,
                 )
                 for arg in extended_type_args
             )
 
         return PydanticFieldMeta(
             name=name,
-            random=cls.random,
+            random=random or DEFAULT_RANDOM,
             annotation=annotation,
             children=children or None,
             default=default_value,
             constraints=cast("Constraints", {k: v for k, v in constraints.items() if v is not None}) or None,
         )
 
 
@@ -234,15 +239,19 @@
 
     __forward_ref_resolution_type_mapping__: ClassVar[Mapping[str, type]] = {}
     __is_base_factory__ = True
 
     def __init_subclass__(cls, *args: Any, **kwargs: Any) -> None:
         super().__init_subclass__(*args, **kwargs)
 
-        if not cls.__is_base_factory__ and hasattr(cls.__model__, "update_forward_refs"):
+        if (
+            VERSION.startswith("1")
+            and getattr(cls, "__model__", None)
+            and hasattr(cls.__model__, "update_forward_refs")
+        ):
             with suppress(NameError):  # pragma: no cover
                 cls.__model__.update_forward_refs(**cls.__forward_ref_resolution_type_mapping__)
 
     @classmethod
     def is_supported_type(cls, value: Any) -> TypeGuard[type[T]]:
         """Determine whether the given value is supported by the factory.
```

### Comparing `polyfactory-2.6.1/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.6.2/polyfactory/factories/typed_dict_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, Generic, TypeVar
 
 from typing_extensions import TypeGuard, _TypedDictMeta, get_type_hints, is_typeddict  # type: ignore[attr-defined]
 
+from polyfactory.constants import DEFAULT_RANDOM
 from polyfactory.factories.base import BaseFactory
 from polyfactory.field_meta import FieldMeta, Null
 
 TypedDictT = TypeVar("TypedDictT", bound=_TypedDictMeta)
 
 
 class TypedDictFactory(Generic[TypedDictT], BaseFactory[TypedDictT]):
@@ -33,15 +34,15 @@
 
         """
         model_type_hints = get_type_hints(cls.__model__, include_extras=True)
 
         fields_meta: list["FieldMeta"] = [
             FieldMeta.from_type(
                 annotation=annotation,
-                random=cls.__random__,
+                random=DEFAULT_RANDOM,
                 name=field_name,
                 default=getattr(cls.__model__, field_name, Null),
                 randomize_collection_length=cls.__randomize_collection_length__,
                 min_collection_length=cls.__min_collection_length__,
                 max_collection_length=cls.__max_collection_length__,
             )
             for field_name, annotation in model_type_hints.items()
```

### Comparing `polyfactory-2.6.1/polyfactory/field_meta.py` & `polyfactory-2.6.2/polyfactory/field_meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,22 +72,22 @@
     constraints: Constraints | None
 
     def __init__(
         self,
         *,
         name: str,
         annotation: type,
-        random: Random = DEFAULT_RANDOM,
+        random: Random | None = None,
         default: Any = Null,
         children: list[FieldMeta] | None = None,
         constraints: Constraints | None = None,
     ) -> None:
         """Create a factory field metadata instance."""
         self.annotation = annotation
-        self.random = random
+        self.random = random or DEFAULT_RANDOM
         self.children = children
         self.default = default
         self.name = name
         self.constraints = constraints
 
     @property
     def type_args(self) -> tuple[Any, ...]:
@@ -140,14 +140,15 @@
             constraints=constraints,
         )
         if field.type_args:
             if randomize_collection_length:
                 number_of_args = random.randint(min_collection_length, max_collection_length)
             else:
                 number_of_args = 1
+
             extended_type_args = CollectionExtender.extend_type_args(field.annotation, field.type_args, number_of_args)
             field.children = [
                 FieldMeta.from_type(
                     annotation=unwrap_new_type(arg),
                     random=random,
                     randomize_collection_length=randomize_collection_length,
                     min_collection_length=min_collection_length,
```

### Comparing `polyfactory-2.6.1/polyfactory/fields.py` & `polyfactory-2.6.2/polyfactory/fields.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/persistence.py` & `polyfactory-2.6.2/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/pytest_plugin.py` & `polyfactory-2.6.2/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/utils/helpers.py` & `polyfactory-2.6.2/polyfactory/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 import sys
-from typing import TYPE_CHECKING, Any, get_args, get_origin
+from typing import TYPE_CHECKING, Any
+
+from typing_extensions import get_args, get_origin
 
 from polyfactory.constants import TYPE_MAPPING
 from polyfactory.utils.predicates import (
     is_annotated,
     is_new_type,
     is_optional_union,
     is_union,
@@ -32,15 +34,16 @@
     """Unwraps union types - recursively.
 
     :param annotation: A type annotation, possibly a type union.
     :param random: An instance of random.Random.
     :returns: A type annotation
     """
     while is_union(annotation):
-        annotation = random.choice(get_args(annotation))
+        args = list(get_args(annotation))
+        annotation = random.choice(args)
     return annotation
 
 
 def unwrap_optional(annotation: Any) -> Any:
     """Unwraps optional union types - recursively.
 
     :param annotation: A type annotation, possibly an optional union.
```

### Comparing `polyfactory-2.6.1/polyfactory/utils/predicates.py` & `polyfactory-2.6.2/polyfactory/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/value_generators/complex_types.py` & `polyfactory-2.6.2/polyfactory/value_generators/complex_types.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.6.2/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.6.2/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.6.2/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.6.2/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/value_generators/primitives.py` & `polyfactory-2.6.2/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/polyfactory/value_generators/regex.py` & `polyfactory-2.6.2/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.6.1/pyproject.toml` & `polyfactory-2.6.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.6.1"
+version = "2.6.2"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
 ]
@@ -67,18 +67,18 @@
 
 [tool.poetry.group.dev.dependencies]
 annotated-types = "*"
 beanie = "*"
 email-validator = "*"
 hypothesis = "*"
 mongomock-motor = "*"
-msgspec = { git = "https://github.com/jcrist/msgspec.git", branch = "main" }
+msgspec = "*"
 odmantic = "*"
 pre-commit = "*"
-pydantic = { git = "https://github.com/pydantic/pydantic", branch = "main" }
+pydantic = ">=2"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 sourcery = "*"
 
 [tool.poetry.group.docs.dependencies]
 auto-pytabs = "*"
```

### Comparing `polyfactory-2.6.1/PKG-INFO` & `polyfactory-2.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.6.1
+Version: 2.6.2
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
 Keywords: beanie,dataclasses,factory,faker,litestar,mock,msgspec,odmantic,pydantic,pytest,tdd,testing,typeddict
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
```

