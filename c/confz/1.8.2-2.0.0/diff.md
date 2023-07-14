# Comparing `tmp/confz-1.8.2.tar.gz` & `tmp/confz-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confz-1.8.2.tar", max compression
+gzip compressed data, was "confz-2.0.0.tar", max compression
```

## Comparing `confz-1.8.2.tar` & `confz-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2023-06-29 11:43:37.180638 confz-1.8.2/LICENSE
--rw-r--r--   0        0        0     8288 2023-06-29 11:43:37.180638 confz-1.8.2/README.md
--rw-r--r--   0        0        0      488 2023-06-29 11:43:37.180638 confz-1.8.2/confz/__init__.py
--rw-r--r--   0        0        0     3281 2023-06-29 11:43:37.180638 confz-1.8.2/confz/change.py
--rw-r--r--   0        0        0     3859 2023-06-29 11:43:37.180638 confz-1.8.2/confz/confz.py
--rw-r--r--   0        0        0     4811 2023-06-29 11:43:37.180638 confz-1.8.2/confz/confz_source.py
--rw-r--r--   0        0        0      372 2023-06-29 11:43:37.180638 confz-1.8.2/confz/exceptions.py
--rw-r--r--   0        0        0      148 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/__init__.py
--rw-r--r--   0        0        0     1065 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/cl_arg_loader.py
--rw-r--r--   0        0        0      296 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/data_loader.py
--rw-r--r--   0        0        0     2716 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/env_loader.py
--rw-r--r--   0        0        0     5432 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/file_loader.py
--rw-r--r--   0        0        0     3113 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/loader.py
--rw-r--r--   0        0        0     1190 2023-06-29 11:43:37.180638 confz-1.8.2/confz/loaders/register.py
--rw-r--r--   0        0        0        0 2023-06-29 11:43:37.180638 confz-1.8.2/confz/py.typed
--rw-r--r--   0        0        0     1585 2023-06-29 11:43:37.180638 confz-1.8.2/confz/validate.py
--rw-r--r--   0        0        0     1990 2023-06-29 11:43:37.184638 confz-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     9459 1970-01-01 00:00:00.000000 confz-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-14 16:04:36.940773 confz-2.0.0/LICENSE
+-rw-r--r--   0        0        0     8324 2023-07-14 16:04:36.940773 confz-2.0.0/README.md
+-rw-r--r--   0        0        0      469 2023-07-14 16:04:36.940773 confz-2.0.0/confz/__init__.py
+-rw-r--r--   0        0        0     3791 2023-07-14 16:04:36.940773 confz-2.0.0/confz/base_config.py
+-rw-r--r--   0        0        0     3305 2023-07-14 16:04:36.940773 confz-2.0.0/confz/change.py
+-rw-r--r--   0        0        0     4804 2023-07-14 16:04:36.940773 confz-2.0.0/confz/config_source.py
+-rw-r--r--   0        0        0      365 2023-07-14 16:04:36.940773 confz-2.0.0/confz/exceptions.py
+-rw-r--r--   0        0        0      148 2023-07-14 16:04:36.940773 confz-2.0.0/confz/loaders/__init__.py
+-rw-r--r--   0        0        0     1064 2023-07-14 16:04:36.940773 confz-2.0.0/confz/loaders/cl_arg_loader.py
+-rw-r--r--   0        0        0      289 2023-07-14 16:04:36.940773 confz-2.0.0/confz/loaders/data_loader.py
+-rw-r--r--   0        0        0     2719 2023-07-14 16:04:36.940773 confz-2.0.0/confz/loaders/env_loader.py
+-rw-r--r--   0        0        0     5459 2023-07-14 16:04:36.940773 confz-2.0.0/confz/loaders/file_loader.py
+-rw-r--r--   0        0        0     3090 2023-07-14 16:04:36.940773 confz-2.0.0/confz/loaders/loader.py
+-rw-r--r--   0        0        0     1166 2023-07-14 16:04:36.940773 confz-2.0.0/confz/loaders/register.py
+-rw-r--r--   0        0        0        0 2023-07-14 16:04:36.940773 confz-2.0.0/confz/py.typed
+-rw-r--r--   0        0        0     1602 2023-07-14 16:04:36.940773 confz-2.0.0/confz/validate.py
+-rw-r--r--   0        0        0     1867 2023-07-14 16:04:36.944773 confz-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9495 1970-01-01 00:00:00.000000 confz-2.0.0/PKG-INFO
```

### Comparing `confz-1.8.2/LICENSE` & `confz-2.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Zühlke
+Copyright (c) 2023 Zühlke
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `confz-1.8.2/README.md` & `confz-2.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 It furthermore supports you in common use cases like:
 
 * Multiple environments
 * Singleton with lazy loading
 * Config changes for unit tests
 * Custom config sources
 
+**UPDATE**: ConfZ 2 is here, with support for pydantic 2 and improved naming conventions.
+Check out the [migration guide](https://confz.readthedocs.io/en/latest/migration_guide.html). 
 
 ## :package: Installation
 
 `ConfZ` is on [PyPI](https://pypi.org/project/confz/) and can be installed with pip:
 
 ```shell
 pip install confz
@@ -31,29 +33,27 @@
 
 
 ## :rocket: Quick Start
 
 The first step of using `ConfZ` is to declare your config classes and sources, for example in `config.py`:
 
 ```python
-from pathlib import Path
-
-from confz import ConfZ, ConfZFileSource
+from confz import BaseConfig, FileSource
 from pydantic import SecretStr, AnyUrl
 
-class DBConfig(ConfZ):
+class DBConfig(BaseConfig):
     user: str
     password: SecretStr
 
-class APIConfig(ConfZ):
+class APIConfig(BaseConfig):
     host: AnyUrl
     port: int
     db: DBConfig
 
-    CONFIG_SOURCES = ConfZFileSource(file='/path/to/config.yml')
+    CONFIG_SOURCES = FileSource(file='/path/to/config.yml')
 ```
 
 Thanks to [pydantic](https://pydantic-docs.helpmanual.io/), you can use a wide variety of
 [field types](https://pydantic-docs.helpmanual.io/usage/types/) and
 [validators](https://pydantic-docs.helpmanual.io/usage/validators/).
 
 From now on, in any other file, you can access your config directly:
@@ -69,103 +69,96 @@
 happens the first time only, afterwards you get back a cached,
 [immutable](https://pydantic-docs.helpmanual.io/usage/models/#faux-immutability) instance, behaving like any other
 _pydantic_ instance.
 
 ```python
 assert APIConfig() is APIConfig()   # true because of singleton mechanism
 APIConfig().port = 1234             # raises an error because of immutability
-APIConfig().json()                  # call pydantic's method to get a json representation
+APIConfig().model_dump()            # call pydantic's method to get a dict representation
 ```
 
 **Note:** While the implicit and hidden loading of your config might be surprising and feel a bit like Python magic at
 first, it allows you to reduce a lot of boilerplate. Instead of having to load your config explicitly and then passing
 it down to all code layers that need it, you can directly access it from anywhere by just importing your config class
 and accessing for example `APIConfig().db.user` directly.
 
 ### More Config Sources
 
 `ConfZ` is highly flexible in defining the source of your config. Do you have multiple environments? No Problem:
 
 ```python
-from pathlib import Path
-
-from confz import ConfZ, ConfZFileSource
+from confz import BaseConfig, FileSource
 
-class MyConfig(ConfZ):
+class MyConfig(BaseConfig):
     ...
-    CONFIG_SOURCES = ConfZFileSource(
+    CONFIG_SOURCES = FileSource(
         folder='/path/to/config/folder',
         file_from_env='ENVIRONMENT'
     )
 ```
 
 Your config file can now be defined in the environment variable `ENVIRONMENT` and is relative to `folder`.
 
 You can also provide a list as config source and read for example from environment variables including a .env file and
 from command line arguments:
 
 ```python
-from pathlib import Path
-from confz import ConfZ, ConfZEnvSource, ConfZCLArgSource
+from confz import BaseConfig, EnvSource, CLArgSource
 
-class MyConfig(ConfZ):
+class MyConfig(BaseConfig):
     ...
     CONFIG_SOURCES = [
-        ConfZEnvSource(allow_all=True, file=".env.local"),
-        ConfZCLArgSource(prefix='conf_')
+        EnvSource(allow_all=True, file=".env.local"),
+        CLArgSource(prefix='conf_')
     ]
 ```
 
 `ConfZ` now tries to populate your config either from environment variables having the same name as your attributes or
 by reading command line arguments that start with `conf_`. Recursive models are supported too, for example if you want
 to control the user-name in the API above, you can either set the environment variable `DB.USER` or pass the command
 line argument `--conf_db.user`.
 
 ### Explicit Loading
 
 In some scenarios, the config should not be a global singleton, but loaded explicitly and passed around locally.
 Instead of defining `CONFIG_SOURCES` as class variable, the sources can also be defined in the constructor directly:
 
 ```python
-from pathlib import Path
+from confz import BaseConfig, FileSource, EnvSource
 
-from confz import ConfZ, ConfZFileSource, ConfZEnvSource
-
-class MyConfig(ConfZ):
+class MyConfig(BaseConfig):
     number: int
     text: str
 
-config1 = MyConfig(config_sources=ConfZFileSource(file='/path/to/config.yml'))
-config2 = MyConfig(config_sources=ConfZEnvSource(prefix='CONF_', allow=['text']), number=1)
+config1 = MyConfig(config_sources=FileSource(file='/path/to/config.yml'))
+config2 = MyConfig(config_sources=EnvSource(prefix='CONF_', allow=['text']), number=1)
 config3 = MyConfig(number=1, text='hello world')
 ```
 
 As can be seen, additional keyword-arguments can be provided as well.
 
-**Note:** If neither class variable `CONFIG_SOURCES` nor constructor argument `config_sources` is provided, `ConfZ`
+**Note:** If neither class variable `CONFIG_SOURCES` nor constructor argument `config_sources` is provided, `BaseConfig`
 behaves like a regular _pydantic_ class.
 
 ### Change Config Values
 
 In some scenarios, you might want to change your config values, for example within a unit test. However, if you set the
 `CONFIG_SOURCES` class variable, this is not directly possible. To overcome this, every config class provides a context
 manager to temporarily change your config:
 
 ```python
-from pathlib import Path
-
-from confz import ConfZ, ConfZFileSource, ConfZDataSource
+from confz import BaseConfig, FileSource, DataSource
 
-class MyConfig(ConfZ):
+class MyConfig(BaseConfig):
     number: int
-    CONFIG_SOURCES = ConfZFileSource(file="/path/to/config.yml")
+    CONFIG_SOURCES = FileSource(file="/path/to/config.yml")
 
 print(MyConfig().number)                            # will print the value from the config-file
 
-new_source = ConfZDataSource(data={'number': 42})
+new_source = DataSource(data={'number': 42})
 with MyConfig.change_config_sources(new_source):
     print(MyConfig().number)                        # will print '42'
 
 print(MyConfig().number)                            # will print the value from the config-file again
 ```
 
 ### Early Validation
```

### Comparing `confz-1.8.2/confz/change.py` & `confz-2.0.0/confz/change.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,25 @@
     Dict,
     TypeVar,
     Generic,
     Optional,
     TYPE_CHECKING,
 )
 
-from .confz_source import ConfZSources
+from .config_source import ConfigSources
 
 if TYPE_CHECKING:
-    from .confz import ConfZ
+    from .base_config import BaseConfig
 
 
 class SourceChangeManager(AbstractContextManager):
     """Config sources change context manager, allows to change config sources within a
     controlled context and resets everything afterwards."""
 
-    def __init__(self, config_class: Type["ConfZ"], config_sources: ConfZSources):
+    def __init__(self, config_class: Type["BaseConfig"], config_sources: ConfigSources):
         self._config_class = config_class
         self._config_sources = config_sources
         self._backup_instance = None
         self._backup_sources = None
 
     def __enter__(self):
         self._backup_instance = self._config_class.confz_instance
@@ -52,15 +52,15 @@
 
 T = TypeVar("T")
 
 
 class Listener(Generic[T]):
     """Listener of config, will add singleton mechanism, aware of config changes."""
 
-    def __init__(self, fn: Callable[[], T], config_classes: List[Type["ConfZ"]]):
+    def __init__(self, fn: Callable[[], T], config_classes: List[Type["BaseConfig"]]):
         if len(inspect.getfullargspec(fn).args) != 0:
             raise ValueError("Callable should not take any arguments")
 
         for config_class in config_classes:
             if config_class.listeners is None:
                 config_class.listeners = []
             config_class.listeners.append(self)
```

### Comparing `confz-1.8.2/confz/confz.py` & `confz-2.0.0/confz/base_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,87 +2,83 @@
 
 from contextlib import AbstractContextManager
 from typing import ClassVar, List, Optional, Any
 
 from pydantic import BaseModel
 
 from .change import SourceChangeManager
-from .confz_source import ConfZSources
-from .exceptions import ConfZException
+from .config_source import ConfigSources
+from .exceptions import ConfigException
 from .loaders import get_loader
 
 
-def _load_config(config_kwargs: dict, confz_sources: ConfZSources) -> dict:
+def _load_config(config_kwargs: dict, config_sources: ConfigSources) -> dict:
     config = config_kwargs.copy()
-    if isinstance(confz_sources, list):
-        for confz_source in confz_sources:
-            loader = get_loader(type(confz_source))
-            loader.populate_config(config, confz_source)
+    if isinstance(config_sources, list):
+        for config_source in config_sources:
+            loader = get_loader(type(config_source))
+            loader.populate_config(config, config_source)
     else:
-        loader = get_loader(type(confz_sources))
-        loader.populate_config(config, confz_sources)
+        loader = get_loader(type(config_sources))
+        loader.populate_config(config, config_sources)
     return config
 
 
 # Metaclass of pydantic.BaseModel is not in __all__, so use type(BaseModel).
-# ConfZ will be only class with this meta class.
-# Both of these things confuse mypy and pylint, so had to disable multiple times.
-class ConfZMetaclass(type(BaseModel)):  # type: ignore
-    """ConfZ Meta Class, inheriting from the pydantic `BaseModel` MetaClass."""
+# This confuses mypy and pylint, so had to disable multiple times.
+class BaseConfigMetaclass(type(BaseModel)):  # type: ignore
+    """BaseConfig Meta Class, inheriting from the pydantic `BaseModel` MetaClass."""
 
     # pylint: disable=no-self-argument,no-member
-    def __call__(cls, config_sources: Optional[ConfZSources] = None, **kwargs):
-        """Called every time an instance of any ConfZ object is created. Injects the
-        config value population and singleton mechanism."""
+    def __call__(cls, config_sources: Optional[ConfigSources] = None, **kwargs):
+        """Called every time an instance of any BaseConfig object is created. Injects
+        the config value population and singleton mechanism."""
         if config_sources is not None:
             config = _load_config(kwargs, config_sources)
             return super().__call__(**config)
 
         if cls.CONFIG_SOURCES is not None:  # type: ignore
             # pylint: disable=access-member-before-definition
             # pylint: disable=attribute-defined-outside-init
             if len(kwargs) > 0:
-                raise ConfZException(
+                raise ConfigException(
                     'Singleton mechanism enabled ("CONFIG_SOURCES" is defined), so '
                     "keyword arguments are not supported"
                 )
             if cls.confz_instance is None:  # type: ignore
                 config = _load_config(kwargs, cls.CONFIG_SOURCES)  # type: ignore
                 cls.confz_instance = super().__call__(**config)
             return cls.confz_instance
 
         return super().__call__(**kwargs)
 
 
-class ConfZ(BaseModel, metaclass=ConfZMetaclass):
-    """Base class, parent of every config class. Internally wraps :class:`BaseModel`of
+class BaseConfig(BaseModel, metaclass=BaseConfigMetaclass, frozen=True):
+    """Base class, parent of every config class. Internally wraps :class:`BaseModel` of
     pydantic and behaves transparent except for two cases:
 
     - If the constructor gets `config_sources` as kwarg, these sources are used as
       input to enrich the other kwargs.
     - If the class has the class variable `CONFIG_SOURCES` defined, these sources are
       used as input.
 
     In the latter case, a singleton mechanism is activated, returning the same config
     class instance every time the constructor is called."""
 
-    CONFIG_SOURCES: ClassVar[Optional[ConfZSources]] = None  #: Sources to use as input.
+    CONFIG_SOURCES: ClassVar[Optional[ConfigSources]] = None  #: Sources to use.
 
     # type is ClassVar[Optional["ConfZ"]] (pydantic throws error with forward ref)
     confz_instance: ClassVar[Optional[Any]] = None  #: *for internal use only*
 
     # type is ClassVar[Optional[List["Listener"]]] (same here)
     listeners: ClassVar[Optional[List[Any]]] = None  #: *for internal use only*
 
-    class Config:
-        allow_mutation = False
-
     @classmethod
     def change_config_sources(
-        cls, config_sources: ConfZSources
+        cls, config_sources: ConfigSources
     ) -> AbstractContextManager:
         """Change the `CONFIG_SOURCES` class variable within a controlled context.
         Within this context, the sources will be different and the singleton reset.
         This can be useful in unit tests to temporarily change a configuration.
 
         :param config_sources: The temporary config sources for within the context.
         :return: Context manager for change of config sources.
```

### Comparing `confz-1.8.2/confz/confz_source.py` & `confz-2.0.0/confz/config_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 from enum import Enum
 from os import PathLike
 from pathlib import Path
 from typing import Optional, Union, List, Dict, Any
 
 
 @dataclass
-class ConfZSource:
-    """Source configuration for :class:`~confz.ConfZ` models."""
+class ConfigSource:
+    """Source configuration for :class:`~confz.BaseConfig` models."""
 
 
-ConfZSources = Union[ConfZSource, List[ConfZSource]]
+ConfigSources = Union[ConfigSource, List[ConfigSource]]
 
 
 class FileFormat(Enum):
     """Enum for file format."""
 
     JSON = "json"  #: JSON file format
     YAML = "yaml"  #: YAML file format
     TOML = "toml"  #: TOML file format
 
 
 @dataclass
-class ConfZFileSource(ConfZSource):
+class FileSource(ConfigSource):
     """Source config for files."""
 
     file: Union[PathLike, str, bytes, None] = None
     """Specify a config file directly by a path or by providing its content as
     bytes-string."""
     file_from_env: Optional[str] = None
     """Alternatively, use this environment variable to get the file."""
@@ -45,15 +45,15 @@
     optional: bool = False
     """True if this config file is only optional. If set to True no error is
     thrown when the file was not found or when the environment variable or the
     command line argument were not set."""
 
 
 @dataclass
-class ConfZEnvSource(ConfZSource):
+class EnvSource(ConfigSource):
     """Source config for environment variables and .env files. On loading of the
     source, the dotenv file values (if available) are merged with the environment,
     with environment always taking precedence in case of name collusion. All loaded
     variable names are transformed to lowercase and all dashes are replaced by
     underscores. The definitions below are not case-sensitive and can be written with
     underscore or dash. An exception is `prefix`, which needs to match exactly.
     Dot-notation can be used to access nested configurations."""
@@ -77,15 +77,15 @@
     """Built in .env file loading with lower than environment precedence. Uses UTF-8
     for decoding."""
     nested_separator: str = "."
     """Separator will be used in nested environment variables."""
 
 
 @dataclass
-class ConfZCLArgSource(ConfZSource):
+class CLArgSource(ConfigSource):
     """Source config for command line arguments. Command line arguments are
     case-sensitive. Dot-notation can be used to access nested configurations. Only
     command line arguments starting with two dashes (\\-\\-) are considered. Between
     argument and value must be whitespace, an equal sign is not supported at the
     moment."""
 
     prefix: Optional[str] = None
@@ -96,14 +96,14 @@
     """Certain command line arguments can be mapped to config arguments with a different
     name. The map does not need to include the two dashes at the beginning."""
     nested_separator: str = "."
     """Separator will be used in nested command line arguments."""
 
 
 @dataclass
-class ConfZDataSource(ConfZSource):
+class DataSource(ConfigSource):
     """Source config for raw data, i.e. constants. This can be useful for unit-test
     together with :meth:`~confz.ConfZ.change_config_sources` to inject test data into
     the config."""
 
     data: Dict[str, Any]
     """All data should go into this (possibly nested) dict."""
```

### Comparing `confz-1.8.2/confz/loaders/cl_arg_loader.py` & `confz-2.0.0/confz/loaders/cl_arg_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import sys
 
-from confz.confz_source import ConfZCLArgSource
+from confz.config_source import CLArgSource
 from .loader import Loader
 
 
 class CLArgLoader(Loader):
     """Config loader for command line arguments."""
 
     @classmethod
-    def populate_config(cls, config: dict, confz_source: ConfZCLArgSource):
+    def populate_config(cls, config: dict, config_source: CLArgSource):
         cl_args = {}
         for idx, cl_arg in enumerate(sys.argv[1:]):
             if cl_arg.startswith("--") and idx + 2 < len(sys.argv):
                 cl_name = cl_arg[2:]
                 cl_value = sys.argv[idx + 2]
 
-                if confz_source.prefix is not None:
-                    if not cl_name.startswith(confz_source.prefix):
+                if config_source.prefix is not None:
+                    if not cl_name.startswith(config_source.prefix):
                         continue
-                    cl_name = cl_name[len(confz_source.prefix) :]
+                    cl_name = cl_name[len(config_source.prefix) :]
 
-                if confz_source.remap is not None and cl_name in confz_source.remap:
-                    cl_name = confz_source.remap[cl_name]
+                if config_source.remap is not None and cl_name in config_source.remap:
+                    cl_name = config_source.remap[cl_name]
 
                 cl_args[cl_name] = cl_value
 
         cl_args = cls.transform_nested_dicts(
-            cl_args, separator=confz_source.nested_separator
+            cl_args, separator=config_source.nested_separator
         )
         cls.update_dict_recursively(config, cl_args)
```

### Comparing `confz-1.8.2/confz/loaders/file_loader.py` & `confz-2.0.0/confz/loaders/file_loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,63 +5,63 @@
 import sys
 from pathlib import Path
 from typing import Iterator, Optional, TextIO, Union
 
 import toml
 import yaml
 
-from confz.confz_source import ConfZFileSource, FileFormat
-from confz.exceptions import ConfZFileException
+from confz.config_source import FileSource, FileFormat
+from confz.exceptions import FileException
 from .loader import Loader
 
 
 class FileLoader(Loader):
     """Config loader for config files."""
 
     @classmethod
-    def _get_filename(cls, confz_source: ConfZFileSource) -> Path:
-        if confz_source.file is not None:
-            if isinstance(confz_source.file, bytes):
-                raise ConfZFileException("Can not detect filename from type bytes")
-            file_path = Path(confz_source.file)
-        elif confz_source.file_from_env is not None:
-            if confz_source.file_from_env not in os.environ:
-                raise ConfZFileException(
-                    f"Environment variable '{confz_source.file_from_env}' is not set."
+    def _get_filename(cls, config_source: FileSource) -> Path:
+        if config_source.file is not None:
+            if isinstance(config_source.file, bytes):
+                raise FileException("Can not detect filename from type bytes")
+            file_path = Path(config_source.file)
+        elif config_source.file_from_env is not None:
+            if config_source.file_from_env not in os.environ:
+                raise FileException(
+                    f"Environment variable '{config_source.file_from_env}' is not set."
                 )
-            file_path = Path(os.environ[confz_source.file_from_env])
-        elif confz_source.file_from_cl is not None:
-            if isinstance(confz_source.file_from_cl, int):
+            file_path = Path(os.environ[config_source.file_from_env])
+        elif config_source.file_from_cl is not None:
+            if isinstance(config_source.file_from_cl, int):
                 try:
-                    file_path = Path(sys.argv[confz_source.file_from_cl])
+                    file_path = Path(sys.argv[config_source.file_from_cl])
                 except IndexError as e:
-                    raise ConfZFileException(
-                        f"Command-line argument number {confz_source.file_from_cl} "
+                    raise FileException(
+                        f"Command-line argument number {config_source.file_from_cl} "
                         f"is not set."
                     ) from e
             else:
                 try:
-                    idx = sys.argv.index(confz_source.file_from_cl)
+                    idx = sys.argv.index(config_source.file_from_cl)
                 except ValueError as e:
-                    raise ConfZFileException(
-                        f"Command-line argument '{confz_source.file_from_cl}' "
+                    raise FileException(
+                        f"Command-line argument '{config_source.file_from_cl}' "
                         f"not found."
                     ) from e
                 try:
                     file_path = Path(sys.argv[idx + 1])
                 except IndexError as e:
-                    raise ConfZFileException(
-                        f"Command-line argument '{confz_source.file_from_cl}' is not "
+                    raise FileException(
+                        f"Command-line argument '{config_source.file_from_cl}' is not "
                         f"set."
                     ) from e
         else:
-            raise ConfZFileException("No file source set.")
+            raise FileException("No file source set.")
 
-        if confz_source.folder is not None:
-            file_path = Path(confz_source.folder) / file_path
+        if config_source.folder is not None:
+            file_path = Path(config_source.folder) / file_path
 
         return file_path
 
     @classmethod
     def _get_format(
         cls, file_path: Path, file_format: Optional[FileFormat]
     ) -> FileFormat:
@@ -74,76 +74,76 @@
             ".json": FileFormat.JSON,
             ".toml": FileFormat.TOML,
         }
         suffix = file_path.suffix
         try:
             suffix_format = suffix_formats[suffix]
         except KeyError as e:
-            raise ConfZFileException(
+            raise FileException(
                 f"File-ending '{suffix}' is not known. Supported are: "
                 f"{', '.join(list(suffix_formats.keys()))}."
             ) from e
 
         return suffix_format
 
     @classmethod
     def _parse_stream(
         cls,
         stream: Union[TextIO],
         file_format: FileFormat,
     ) -> dict:
         if file_format == FileFormat.YAML:
-            file_content = yaml.safe_load(stream)
+            file_content = yaml.load(stream, Loader=yaml.BaseLoader)
         elif file_format == FileFormat.JSON:
             file_content = json.load(stream)
         elif file_format == FileFormat.TOML:
             file_content = toml.load(stream)
+        else:
+            raise FileException(f"Unknown file format {file_format}.")
         return file_content
 
     @classmethod
     @contextmanager
     def _create_stream(cls, file_path: Path, file_encoding: str) -> Iterator[TextIO]:
         try:
             stream = file_path.open(encoding=file_encoding)
         except OSError as e:
-            raise ConfZFileException(
-                f"Could not open config file '{file_path}'."
-            ) from e
+            raise FileException(f"Could not open config file '{file_path}'.") from e
         with stream:
             yield stream
 
     @classmethod
     def _populate_config_from_bytes(
-        cls, config: dict, data: bytes, confz_source: ConfZFileSource
+        cls, config: dict, data: bytes, config_source: FileSource
     ):
-        if confz_source.format is None:
-            raise ConfZFileException(
+        if config_source.format is None:
+            raise FileException(
                 "The format needs to be defined if the "
                 "configuration is passed as byte-string"
             )
         byte_stream = io.BytesIO(data)
-        text_stream = io.TextIOWrapper(byte_stream, encoding=confz_source.encoding)
-        file_content = cls._parse_stream(text_stream, confz_source.format)
+        text_stream = io.TextIOWrapper(byte_stream, encoding=config_source.encoding)
+        file_content = cls._parse_stream(text_stream, config_source.format)
         cls.update_dict_recursively(config, file_content)
 
     @classmethod
-    def populate_config(cls, config: dict, confz_source: ConfZFileSource):
-        if confz_source.file is not None and isinstance(confz_source.file, bytes):
+    def populate_config(cls, config: dict, config_source: FileSource):
+        if config_source.file is not None and isinstance(config_source.file, bytes):
             cls._populate_config_from_bytes(
-                config=config, data=confz_source.file, confz_source=confz_source
+                config=config, data=config_source.file, config_source=config_source
             )
             return
         try:
-            file_path = cls._get_filename(confz_source)
-        except ConfZFileException as e:
-            if confz_source.optional:
+            file_path = cls._get_filename(config_source)
+        except FileException as e:
+            if config_source.optional:
                 return
             raise e
-        file_format = cls._get_format(file_path, confz_source.format)
+        file_format = cls._get_format(file_path, config_source.format)
         try:
-            with cls._create_stream(file_path, confz_source.encoding) as file_stream:
+            with cls._create_stream(file_path, config_source.encoding) as file_stream:
                 file_content = cls._parse_stream(file_stream, file_format)
-        except ConfZFileException as e:
-            if confz_source.optional:
+        except FileException as e:
+            if config_source.optional:
                 return
             raise e
         cls.update_dict_recursively(config, file_content)
```

### Comparing `confz-1.8.2/confz/loaders/loader.py` & `confz-2.0.0/confz/loaders/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Any
 
-from confz.exceptions import ConfZUpdateException
+from confz.exceptions import UpdateException
 
 
 class Loader(ABC):
     """An abstract base class for all config loaders."""
 
     @classmethod
     def update_dict_recursively(cls, original_dict: Dict, update_dict: Dict):
         """Updates the original dict with the new data. Similar to `dict.update()`, but
         works with nested dicts.
 
         :param original_dict: The original dictionary to update in-place.
         :param update_dict: The new data.
-        :raises ConfZUpdateException: If dict keys contradict each other.
+        :raises UpdateException: If dict keys contradict each other.
         """
         for key, value in update_dict.items():
             if isinstance(value, dict) and key in original_dict:
                 if not isinstance(original_dict[key], dict):
-                    raise ConfZUpdateException(
+                    raise UpdateException(
                         f"Config variables contradict each other: "
                         f"Key '{key}' is both a value and a nested dict."
                     )
                 cls.update_dict_recursively(original_dict[key], value)
             else:
                 original_dict[key] = value
 
@@ -35,39 +35,39 @@
         keys as hint.
 
         :param dict_in: A dictionary with string-keys.
         :param separator: The string used to separate dict keys.
                           Default value will no longer be set in a future release.
         :return: The transformed dictionary, splitting keys at the separator and
             creating a new dictionary out of it.
-        :raises ConfZUpdateException: If dict keys contradict each other.
+        :raises UpdateException: If dict keys contradict each other.
         """
         dict_out: Dict[str, Any] = {}
         for key, value in dict_in.items():
             if separator in key and not key.startswith(separator):
                 inner_keys = key.split(separator)
                 dict_inner = dict_out
                 for idx, inner_key in enumerate(inner_keys):
                     if idx == len(inner_keys) - 1:
                         dict_inner[inner_key] = value
                     else:
                         if inner_key not in dict_inner:
                             dict_inner[inner_key] = {}
                         elif not isinstance(dict_inner[inner_key], dict):
-                            raise ConfZUpdateException(
+                            raise UpdateException(
                                 f"Config variables contradict each other: Key "
                                 f"'{inner_key}' is both a value and a nested dict."
                             )
                         dict_inner = dict_inner[inner_key]
             else:
                 dict_out[key] = value
 
         return dict_out
 
     @classmethod
     @abstractmethod
-    def populate_config(cls, config: dict, confz_source):
+    def populate_config(cls, config: dict, config_source):
         """Populate the config-dict with new config arguments based on the source.
 
         :param config: Config dictionary, gets extended with new arguments
-        :param confz_source: Source configuration.
+        :param config_source: Source configuration.
         """
```

### Comparing `confz-1.8.2/confz/loaders/register.py` & `confz-2.0.0/confz/loaders/register.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from typing import Type, Dict
 
-from confz.confz_source import (
-    ConfZSource,
-    ConfZFileSource,
-    ConfZEnvSource,
-    ConfZCLArgSource,
-    ConfZDataSource,
+from confz.config_source import (
+    ConfigSource,
+    FileSource,
+    EnvSource,
+    CLArgSource,
+    DataSource,
 )
-from confz.exceptions import ConfZException
+from confz.exceptions import ConfigException
 from .cl_arg_loader import CLArgLoader
 from .data_loader import DataLoader
 from .env_loader import EnvLoader
 from .file_loader import FileLoader
 from .loader import Loader
 
-_loaders: Dict[Type[ConfZSource], Type[Loader]] = {}
+_loaders: Dict[Type[ConfigSource], Type[Loader]] = {}
 
 
-def get_loader(confz_source: Type[ConfZSource]):
-    if confz_source in _loaders:
-        return _loaders[confz_source]
-    raise ConfZException(f"Unknown config source type '{confz_source}'")
+def get_loader(config_source: Type[ConfigSource]):
+    if config_source in _loaders:
+        return _loaders[config_source]
+    raise ConfigException(f"Unknown config source type '{config_source}'")
 
 
-def register_loader(confz_source: Type[ConfZSource], loader: Type[Loader]):
-    """Register a :class:`~confz.ConfZSource` with a specific loader. Can be used to
+def register_loader(config_source: Type[ConfigSource], loader: Type[Loader]):
+    """Register a :class:`~confz.ConfigSource` with a specific loader. Can be used to
     extend `ConfZ` with own loaders.
 
-    :param confz_source: The :class:`~confz.ConfZSource` sub-type.
+    :param config_source: The :class:`~confz.ConfigSource` sub-type.
     :param loader: The :class:`~confz.loaders.Loader` sub-type.
     """
-    _loaders[confz_source] = loader
+    _loaders[config_source] = loader
 
 
-register_loader(ConfZFileSource, FileLoader)
-register_loader(ConfZEnvSource, EnvLoader)
-register_loader(ConfZCLArgSource, CLArgLoader)
-register_loader(ConfZDataSource, DataLoader)
+register_loader(FileSource, FileLoader)
+register_loader(EnvSource, EnvLoader)
+register_loader(CLArgSource, CLArgLoader)
+register_loader(DataSource, DataLoader)
```

### Comparing `confz-1.8.2/confz/validate.py` & `confz-2.0.0/confz/validate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .confz import ConfZ
+from .base_config import BaseConfig
 
 
 def _get_sub_classes(cls):
     direct_sub_classes = cls.__subclasses__()
 
     all_sub_classes = direct_sub_classes.copy()
     for sub_class in direct_sub_classes:
@@ -14,20 +14,20 @@
 def validate_all_configs(include_listeners: bool = False):
     """Instantiates all config classes with a singleton mechanism
     (`CONFIG_SOURCES` set). This allows to catch validation errors early instead of
     waiting for the first access.
 
     :param include_listeners: Whether all listeners (marked with
         :func:`~confz.depends_on`) should be included.
-    :raises ConfZException: If any config could not be loaded.
+    :raises ConfigException: If any config could not be loaded.
     """
     config_classes = []
     sync_listeners = []
     async_listeners = []
-    for config_class in _get_sub_classes(ConfZ):
+    for config_class in _get_sub_classes(BaseConfig):
         if config_class.CONFIG_SOURCES is not None:
             config_classes.append(config_class)
             if include_listeners and config_class.listeners is not None:
                 for listener in config_class.listeners:
                     if listener.is_async:
                         async_listeners.append(listener)
                     else:
```

### Comparing `confz-1.8.2/pyproject.toml` & `confz-2.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "confz"
-version = "1.8.2"
+version = "2.0.0"
 description = "ConfZ is a configuration management library for Python based on pydantic."
 license = "MIT"
 authors = ["Zühlke"]
 readme = "README.md"
 homepage = "https://github.com/Zuehlke/ConfZ"
 repository = "https://github.com/Zuehlke/ConfZ"
 documentation = "https://confz.readthedocs.io"
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
-pydantic = "^1.9.0"
+pydantic = ">=1.9.0, <3.0.0"
 PyYAML = ">=5.4.1, <7.0.0"
 python-dotenv = ">=0.19.2, <2.0.0"
 toml = "^0.10.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 Sphinx = "^5.3.0"
@@ -41,16 +41,14 @@
 types-toml = "^0.10.8"
 
 [tool.black]
 # Use default black configuration
 
 [tool.pylint.messages_control]
 disable = [
-    "wrong-hanging-indentation",    # to work together with black
-    "bad-whitespace",               # to work together with black
     "missing-module-docstring",
     "missing-class-docstring",
     "missing-function-docstring",
     "invalid-name",
     "too-few-public-methods"
 ]
 extension-pkg-whitelist = "pydantic"
```

### Comparing `confz-1.8.2/PKG-INFO` & `confz-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confz
-Version: 1.8.2
+Version: 2.0.0
 Summary: ConfZ is a configuration management library for Python based on pydantic.
 Home-page: https://github.com/Zuehlke/ConfZ
 License: MIT
 Keywords: Configuration Management,Config Management
 Author: Zühlke
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=5.4.1,<7.0.0)
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: pydantic (>=1.9.0,<3.0.0)
 Requires-Dist: python-dotenv (>=0.19.2,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Documentation, https://confz.readthedocs.io
 Project-URL: Repository, https://github.com/Zuehlke/ConfZ
 Description-Content-Type: text/markdown
 
 # ConfZ – Pydantic Config Management
@@ -44,14 +44,16 @@
 It furthermore supports you in common use cases like:
 
 * Multiple environments
 * Singleton with lazy loading
 * Config changes for unit tests
 * Custom config sources
 
+**UPDATE**: ConfZ 2 is here, with support for pydantic 2 and improved naming conventions.
+Check out the [migration guide](https://confz.readthedocs.io/en/latest/migration_guide.html). 
 
 ## :package: Installation
 
 `ConfZ` is on [PyPI](https://pypi.org/project/confz/) and can be installed with pip:
 
 ```shell
 pip install confz
@@ -59,29 +61,27 @@
 
 
 ## :rocket: Quick Start
 
 The first step of using `ConfZ` is to declare your config classes and sources, for example in `config.py`:
 
 ```python
-from pathlib import Path
-
-from confz import ConfZ, ConfZFileSource
+from confz import BaseConfig, FileSource
 from pydantic import SecretStr, AnyUrl
 
-class DBConfig(ConfZ):
+class DBConfig(BaseConfig):
     user: str
     password: SecretStr
 
-class APIConfig(ConfZ):
+class APIConfig(BaseConfig):
     host: AnyUrl
     port: int
     db: DBConfig
 
-    CONFIG_SOURCES = ConfZFileSource(file='/path/to/config.yml')
+    CONFIG_SOURCES = FileSource(file='/path/to/config.yml')
 ```
 
 Thanks to [pydantic](https://pydantic-docs.helpmanual.io/), you can use a wide variety of
 [field types](https://pydantic-docs.helpmanual.io/usage/types/) and
 [validators](https://pydantic-docs.helpmanual.io/usage/validators/).
 
 From now on, in any other file, you can access your config directly:
@@ -97,103 +97,96 @@
 happens the first time only, afterwards you get back a cached,
 [immutable](https://pydantic-docs.helpmanual.io/usage/models/#faux-immutability) instance, behaving like any other
 _pydantic_ instance.
 
 ```python
 assert APIConfig() is APIConfig()   # true because of singleton mechanism
 APIConfig().port = 1234             # raises an error because of immutability
-APIConfig().json()                  # call pydantic's method to get a json representation
+APIConfig().model_dump()            # call pydantic's method to get a dict representation
 ```
 
 **Note:** While the implicit and hidden loading of your config might be surprising and feel a bit like Python magic at
 first, it allows you to reduce a lot of boilerplate. Instead of having to load your config explicitly and then passing
 it down to all code layers that need it, you can directly access it from anywhere by just importing your config class
 and accessing for example `APIConfig().db.user` directly.
 
 ### More Config Sources
 
 `ConfZ` is highly flexible in defining the source of your config. Do you have multiple environments? No Problem:
 
 ```python
-from pathlib import Path
-
-from confz import ConfZ, ConfZFileSource
+from confz import BaseConfig, FileSource
 
-class MyConfig(ConfZ):
+class MyConfig(BaseConfig):
     ...
-    CONFIG_SOURCES = ConfZFileSource(
+    CONFIG_SOURCES = FileSource(
         folder='/path/to/config/folder',
         file_from_env='ENVIRONMENT'
     )
 ```
 
 Your config file can now be defined in the environment variable `ENVIRONMENT` and is relative to `folder`.
 
 You can also provide a list as config source and read for example from environment variables including a .env file and
 from command line arguments:
 
 ```python
-from pathlib import Path
-from confz import ConfZ, ConfZEnvSource, ConfZCLArgSource
+from confz import BaseConfig, EnvSource, CLArgSource
 
-class MyConfig(ConfZ):
+class MyConfig(BaseConfig):
     ...
     CONFIG_SOURCES = [
-        ConfZEnvSource(allow_all=True, file=".env.local"),
-        ConfZCLArgSource(prefix='conf_')
+        EnvSource(allow_all=True, file=".env.local"),
+        CLArgSource(prefix='conf_')
     ]
 ```
 
 `ConfZ` now tries to populate your config either from environment variables having the same name as your attributes or
 by reading command line arguments that start with `conf_`. Recursive models are supported too, for example if you want
 to control the user-name in the API above, you can either set the environment variable `DB.USER` or pass the command
 line argument `--conf_db.user`.
 
 ### Explicit Loading
 
 In some scenarios, the config should not be a global singleton, but loaded explicitly and passed around locally.
 Instead of defining `CONFIG_SOURCES` as class variable, the sources can also be defined in the constructor directly:
 
 ```python
-from pathlib import Path
+from confz import BaseConfig, FileSource, EnvSource
 
-from confz import ConfZ, ConfZFileSource, ConfZEnvSource
-
-class MyConfig(ConfZ):
+class MyConfig(BaseConfig):
     number: int
     text: str
 
-config1 = MyConfig(config_sources=ConfZFileSource(file='/path/to/config.yml'))
-config2 = MyConfig(config_sources=ConfZEnvSource(prefix='CONF_', allow=['text']), number=1)
+config1 = MyConfig(config_sources=FileSource(file='/path/to/config.yml'))
+config2 = MyConfig(config_sources=EnvSource(prefix='CONF_', allow=['text']), number=1)
 config3 = MyConfig(number=1, text='hello world')
 ```
 
 As can be seen, additional keyword-arguments can be provided as well.
 
-**Note:** If neither class variable `CONFIG_SOURCES` nor constructor argument `config_sources` is provided, `ConfZ`
+**Note:** If neither class variable `CONFIG_SOURCES` nor constructor argument `config_sources` is provided, `BaseConfig`
 behaves like a regular _pydantic_ class.
 
 ### Change Config Values
 
 In some scenarios, you might want to change your config values, for example within a unit test. However, if you set the
 `CONFIG_SOURCES` class variable, this is not directly possible. To overcome this, every config class provides a context
 manager to temporarily change your config:
 
 ```python
-from pathlib import Path
-
-from confz import ConfZ, ConfZFileSource, ConfZDataSource
+from confz import BaseConfig, FileSource, DataSource
 
-class MyConfig(ConfZ):
+class MyConfig(BaseConfig):
     number: int
-    CONFIG_SOURCES = ConfZFileSource(file="/path/to/config.yml")
+    CONFIG_SOURCES = FileSource(file="/path/to/config.yml")
 
 print(MyConfig().number)                            # will print the value from the config-file
 
-new_source = ConfZDataSource(data={'number': 42})
+new_source = DataSource(data={'number': 42})
 with MyConfig.change_config_sources(new_source):
     print(MyConfig().number)                        # will print '42'
 
 print(MyConfig().number)                            # will print the value from the config-file again
 ```
 
 ### Early Validation
```

