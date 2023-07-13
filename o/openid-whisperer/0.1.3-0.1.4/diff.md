# Comparing `tmp/openid_whisperer-0.1.3.tar.gz` & `tmp/openid_whisperer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openid_whisperer-0.1.3.tar", max compression
+gzip compressed data, was "openid_whisperer-0.1.4.tar", max compression
```

## Comparing `openid_whisperer-0.1.3.tar` & `openid_whisperer-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rw-r--r--   0        0        0     1153 2023-06-25 20:59:05.837711 openid_whisperer-0.1.3/LICENSE
--rw-r--r--   0        0        0     7097 2023-07-12 16:26:48.893540 openid_whisperer-0.1.3/README.md
--rw-r--r--   0        0        0     2143 2023-07-12 22:01:50.709606 openid_whisperer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-03 22:59:15.739113 openid_whisperer-0.1.3/src/openid_whisperer/__init__.py
--rw-r--r--   0        0        0       83 2023-06-03 22:59:15.739296 openid_whisperer-0.1.3/src/openid_whisperer/__main__.py
--rw-r--r--   0        0        0     7799 2023-07-10 20:59:59.115502 openid_whisperer-0.1.3/src/openid_whisperer/config.py
--rw-r--r--   0        0        0     1112 2023-07-11 21:48:13.064616 openid_whisperer-0.1.3/src/openid_whisperer/main.py
--rw-r--r--   0        0        0    20852 2023-07-12 17:42:03.339267 openid_whisperer-0.1.3/src/openid_whisperer/openid_blueprint.py
--rw-r--r--   0        0        0    26013 2023-07-11 22:18:31.791763 openid_whisperer-0.1.3/src/openid_whisperer/openid_interface.py
--rw-r--r--   0        0        0      922 2023-07-09 21:10:04.200881 openid_whisperer-0.1.3/src/openid_whisperer/openid_types.py
--rw-r--r--   0        0        0        0 2023-06-04 10:12:20.232971 openid_whisperer-0.1.3/src/openid_whisperer/py.typed
--rw-r--r--   0        0        0     7774 2023-07-04 18:12:57.431778 openid_whisperer-0.1.3/src/openid_whisperer/static/style.css
--rw-r--r--   0        0        0    29080 2023-07-11 19:49:56.711266 openid_whisperer-0.1.3/src/openid_whisperer/templates/authenticate.html
--rw-r--r--   0        0        0        0 2023-07-01 16:06:18.981399 openid_whisperer-0.1.3/src/openid_whisperer/utils/__init__.py
--rw-r--r--   0        0        0    13725 2023-07-05 20:49:35.637180 openid_whisperer-0.1.3/src/openid_whisperer/utils/cert_utils.py
--rw-r--r--   0        0        0     4074 2023-07-11 20:23:52.969778 openid_whisperer-0.1.3/src/openid_whisperer/utils/common.py
--rw-r--r--   0        0        0     4723 2023-07-10 20:57:32.222046 openid_whisperer-0.1.3/src/openid_whisperer/utils/config_utils.py
--rw-r--r--   0        0        0     3756 2023-07-11 22:11:18.564325 openid_whisperer-0.1.3/src/openid_whisperer/utils/credential_store.py
--rw-r--r--   0        0        0    11696 2023-07-11 22:15:16.409405 openid_whisperer-0.1.3/src/openid_whisperer/utils/token_store.py
--rw-r--r--   0        0        0     3150 2023-07-10 21:09:46.426743 openid_whisperer-0.1.3/src/openid_whisperer/utils/token_utils.py
--rw-r--r--   0        0        0     7094 2023-07-12 13:56:33.537165 openid_whisperer-0.1.3/src/openid_whisperer/utils/user_info_ext.py
--rw-r--r--   0        0        0     8183 1970-01-01 00:00:00.000000 openid_whisperer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-06-25 20:59:05.837711 openid_whisperer-0.1.4/LICENSE
+-rw-r--r--   0        0        0     7014 2023-07-13 18:28:11.127379 openid_whisperer-0.1.4/README.md
+-rw-r--r--   0        0        0     2123 2023-07-13 18:28:24.274371 openid_whisperer-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 22:59:15.739113 openid_whisperer-0.1.4/src/openid_whisperer/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-03 22:59:15.739296 openid_whisperer-0.1.4/src/openid_whisperer/__main__.py
+-rw-r--r--   0        0        0     8614 2023-07-13 23:09:05.728165 openid_whisperer-0.1.4/src/openid_whisperer/config.py
+-rw-r--r--   0        0        0     2539 2023-07-13 16:49:06.224941 openid_whisperer-0.1.4/src/openid_whisperer/demo_certs/ca_cert.pem
+-rw-r--r--   0        0        0     2681 2023-07-13 16:49:06.225650 openid_whisperer-0.1.4/src/openid_whisperer/demo_certs/cert.pem
+-rw-r--r--   0        0        0     1675 2023-07-13 16:49:06.226302 openid_whisperer-0.1.4/src/openid_whisperer/demo_certs/key.pem
+-rw-r--r--   0        0        0     1165 2023-07-13 16:49:06.227147 openid_whisperer-0.1.4/src/openid_whisperer/main.py
+-rw-r--r--   0        0        0    21263 2023-07-13 23:09:05.894001 openid_whisperer-0.1.4/src/openid_whisperer/openid_blueprint.py
+-rw-r--r--   0        0        0    27450 2023-07-13 23:09:05.900286 openid_whisperer-0.1.4/src/openid_whisperer/openid_interface.py
+-rw-r--r--   0        0        0      922 2023-07-09 21:10:04.200881 openid_whisperer-0.1.4/src/openid_whisperer/openid_types.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:12:20.232971 openid_whisperer-0.1.4/src/openid_whisperer/py.typed
+-rw-r--r--   0        0        0     7774 2023-07-04 18:12:57.431778 openid_whisperer-0.1.4/src/openid_whisperer/static/style.css
+-rw-r--r--   0        0        0    29028 2023-07-13 16:49:06.234092 openid_whisperer-0.1.4/src/openid_whisperer/templates/authenticate.html
+-rw-r--r--   0        0        0        0 2023-07-01 16:06:18.981399 openid_whisperer-0.1.4/src/openid_whisperer/utils/__init__.py
+-rw-r--r--   0        0        0     5162 2023-07-13 22:45:35.904006 openid_whisperer-0.1.4/src/openid_whisperer/utils/cert_utils.py
+-rw-r--r--   0        0        0     4074 2023-07-11 20:23:52.969778 openid_whisperer-0.1.4/src/openid_whisperer/utils/common.py
+-rw-r--r--   0        0        0     4723 2023-07-13 22:40:09.264988 openid_whisperer-0.1.4/src/openid_whisperer/utils/config_utils.py
+-rw-r--r--   0        0        0     4110 2023-07-13 23:09:05.684052 openid_whisperer-0.1.4/src/openid_whisperer/utils/credential_store.py
+-rw-r--r--   0        0        0    12286 2023-07-13 23:09:05.770097 openid_whisperer-0.1.4/src/openid_whisperer/utils/token_store.py
+-rw-r--r--   0        0        0     3145 2023-07-13 22:21:32.054429 openid_whisperer-0.1.4/src/openid_whisperer/utils/token_utils.py
+-rw-r--r--   0        0        0     7094 2023-07-12 13:56:33.537165 openid_whisperer-0.1.4/src/openid_whisperer/utils/user_info_ext.py
+-rw-r--r--   0        0        0     8100 1970-01-01 00:00:00.000000 openid_whisperer-0.1.4/PKG-INFO
```

### Comparing `openid_whisperer-0.1.3/LICENSE` & `openid_whisperer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.3/README.md` & `openid_whisperer-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -106,17 +106,14 @@
 ```commandline
 cd openid-whisperer
 poetry install
 poetry update
 ```
 6. Setup environment variables, default `.env` and `.env_${ENVIRONMENT:-TEST}`
 ```
-INTERNAL_HOST=${INTERNAL_HOST:-localhost}
-GATEWAY_HOST=${GATEWAY_HOST:-localhost}
-
 API_HOST=${INTERNAL_HOST:-localhost}
 API_PORT=${API_PORT:-5700}
 API_HOST_GW=${GATEWAY_HOST:-localhost}
 API_PORT_GW=${API_PORT_GW:-8100}
 
 ID_SERVICE_PORT=${ID_SERVICE_PORT:-5000}
 ID_SERVICE_HOST=${INTERNAL_HOST:-localhost}
@@ -144,10 +141,10 @@
 Run OpenID Whisperer (from project root)
 ```
 poetry run python -m openid_whisperer.main 
 ```
 
 Run within a Docker Container
 ```
-docker build -t opendid-whisperer:0.1.0 .
-docker run --name=openid-whisperer -p5005:5000  -eID_SERVICE_PORT_GW=5005 opendid-whisperer:0.1.0
+docker build -t opendid-whisperer:0.1.4 .
+docker run --name=openid-whisperer -p5005:5005  -eID_SERVICE_PORT_GW=5005 opendid-whisperer:0.1.4
 ```
```

### Comparing `openid_whisperer-0.1.3/pyproject.toml` & `openid_whisperer-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openid-whisperer"
-version = "0.1.3"
+version = "0.1.4"
 description = "OpenID 1.0 Mock Identity Service"
 license = "MIT"
 authors = ["Robert Betts <betts_robert@yahoo.com>"]
 maintainers = ["Robert Betts <betts_robert@yahoo.com>"]
 readme = "README.md"
 homepage = "https://github.com/robertbetts/openid-whisperer"
 repository = "https://github.com/robertbetts/openid-whisperer"
@@ -40,33 +40,32 @@
     "pragma: no cover",
     "if TYPE_CHECKING:"
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
 check_untyped_defs = true
-#files = "src, tests"
+#files = "src, example_src"
 files = "src"
 mypy_path = "src"
 namespace_packages = true
 explicit_package_bases = true
 show_error_codes = true
 strict = true
 enable_error_code = [
     "ignore-without-code",
     "redundant-expr",
     "truthy-bool",
 ]
 exclude = [
     "tests",
-    "src/mocking_examples"
 ]
 
 [tool.pylint]
-ignore-paths = "tests"
+#ignore-paths = "tests"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pyjwt = "^2.6.0"
 requests = {extras = ["security"], version = "^2.31.0"}
 types-requests = "^2.31.0.1"
 cryptography = "^41.0.1"
```

### Comparing `openid_whisperer-0.1.3/src/openid_whisperer/config.py` & `openid_whisperer-0.1.4/src/openid_whisperer/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,105 +1,140 @@
-""" Configuration module for OpenID Whisperer
+""" Configuration module for Openid_whisperer
 """
+import importlib.resources
 import logging
 import os
 from uuid import uuid4
+from typing import Type, Optional, Tuple, TextIO, Any, Dict, Iterable
 
 from cryptography import x509
 from cryptography.hazmat.primitives.asymmetric import rsa
-from cryptography.hazmat.primitives.asymmetric.types import (
-    PrivateKeyTypes,
-)
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.backends import default_backend
 
+from openid_whisperer.utils.common import boolify
 from openid_whisperer.utils.config_utils import (
     load_environment_variables,
     default_config_type,
-    get_bind_address,
     initialize_logging,
 )
 
-cached_config = None
+_cached_config: Optional["Config"] = None
 
 
 class ConfigurationException(Exception):
     ...
 
 
 class Config:
     default_config: default_config_type = {
         "instance_id": (str, uuid4().hex),
-        "gateway_address": (str, "localhost:8100"),
-        "bind_address": (get_bind_address, "0.0.0.0:5000,[::]:5000"),
         "log_level": (str, "info"),
-        "flask_debug": (bool, "False"),
-        "validate_certs": (bool, "False"),
+        "flask_debug": (boolify, False),
+        "validate_certs": (boolify, False),
         "id_service_prefix": (str, "/adfs"),
-        "id_service_port": (int, "5000"),
+        "id_service_port": (int, 5005),
         "id_service_host": (str, "localhost"),
         "id_service_bind": (str, "0.0.0.0"),
-        "id_service_port_gw": (int, "8100"),
+        "id_service_port_gw": (int, 5005),
         "id_service_host_gw": (str, "localhost"),
-        "ca_key_filename": (str, "certs/ca_key.pem"),
-        "ca_key_password": (str, ""),
-        "ca_cert_filename": (str, "certs/ca_cert.pem"),
-        "org_key_filename": (str, "certs/key.pem"),
+        "validate_users": (boolify, False),
+        "json_user_file": (str, ""),
+        "session_expiry_seconds": (int, 0),
+        "maximum_login_attempts": (int, 0),
+        "ca_cert_filename": (str, ""),
+        "org_key_filename": (str, ""),
         "org_key_password": (str, ""),
-        "org_cert_filename": (str, "certs/cert.pem"),
+        "org_cert_filename": (str, ""),
     }
 
+    # General configuration parameters
+    env_target: str | None
+    log_level: str
+    flask_debug: bool
+    validate_certs: bool
+
+    # Networking related configuration
+    id_service_prefix: str
+    id_service_port: int
+    id_service_host: str
+    id_service_bind: str
+    id_service_port_gw: str
+    id_service_host_gw: str
+
+    # Credential related configuration
+    validate_users: bool
+    json_user_file: str
+    session_expiry_seconds: int
+    maximum_login_attempts: int
+
+    # Credential and Web API related configuration. If not all the configuration entries
+    # for these filenames are entered, then the demo certs in this package are used.
+    ca_cert_filename: str  # this entry is not mandatory
+    org_key_filename: str
+    org_key_password: str
+    org_cert_filename: str
+
+    # These class properties are initialised by self.init_certs()
+    ca_cert: Optional[x509.Certificate]
+    org_key: rsa.RSAPrivateKey
+    org_cert: x509.Certificate
+
     def __new__(cls, *args, **kwargs):
         instance = super().__new__(cls)
         init_config = {}
         init_config.update(cls.default_config)
         if "defaults" in kwargs and isinstance(kwargs["defaults"], dict):
             init_config.update(kwargs["defaults"])
         for key, value in init_config.items():
             _, default = value
             if not key.isidentifier():
-                raise ValueError(
-                    "configuration property %s, is not a valid identifier name", key
-                )
+                raise ValueError(f"Configuration property {key}, is not valid.")
             setattr(instance, key, default)
         return instance
 
     def __init__(
         self, defaults: default_config_type | None = None, env_target: str | None = None
     ) -> None:
         defaults = {} if defaults is None else defaults
-        self.env_target: str | None = env_target
-        self.log_level: str = "info"
-        self.flask_debug: bool = False
-        self.validate_certs = False
-
-        self.id_service_prefix: str = "/adfs"
-        self.id_service_port: int = 8100
-        self.id_service_host: str = "localhost"
-        self.id_service_bind: str = "0.0.0.0"
-        self.id_service_port_gw = "5000"
-        self.id_service_host_gw = "localhost"
-
-        self.ca_key_filename: str = "certs/ca_key.pem"
-        self.ca_key_password: str = ""
-        self.ca_cert_filename: str = "certs/ca_cert.pem"
-        self.org_key_filename: str = "certs/key.pem"
-        self.org_key_password: str = ""
-        self.org_cert_filename: str = "certs/cert.pem"
+        self.env_target = env_target
 
-        self.ca_key: rsa.RSAPrivateKey
-        self.ca_cert: x509.Certificate
-        self.org_key: rsa.RSAPrivateKey
-        self.org_cert: x509.Certificate
+        self.ca_cert_filename: str = ""
+        self.org_key_filename: str = ""
+        self.org_key_password: str = ""
+        self.org_cert_filename: str = ""
 
         self.init_defaults = {}
         self.init_defaults.update(defaults)
         self.load_config()
-
         self.init_logging()
+
+        # Checking for the required certificate/key file pair, if not found then default
+        # to the package provided demo certificate files, including a ca cert file.
+        if not os.path.exists(self.org_key_filename) or not os.path.exists(
+            self.org_cert_filename
+        ):
+            if self.org_key_filename and not os.path.exists(self.org_key_filename):
+                logging.critical(f"Private key file not found: {self.org_key_filename}")
+            if self.org_cert_filename and not os.path.exists(self.org_cert_filename):
+                logging.critical(
+                    f"Certificate file not found: {self.org_cert_filename}"
+                )
+            logging.critical("Defaulting to packaged demo certificate/key pair")
+            with importlib.resources.files("openid_whisperer") as module_resource:
+                self.ca_cert_filename = os.path.join(
+                    module_resource, "demo_certs", "ca_cert.pem"
+                )
+                self.org_key_filename = os.path.join(
+                    module_resource, "demo_certs", "key.pem"
+                )
+                self.org_cert_filename = os.path.join(
+                    module_resource, "demo_certs", "cert.pem"
+                )
+
         self.init_certs()
 
     @property
     def id_provider_base_url(self) -> str:
         """This url must be accessible to the client interacting with the identity provider"""
         return f"https://{self.id_service_host}:{self.id_service_port}"
 
@@ -129,66 +164,61 @@
                 )
 
     def init_logging(self, log_level: str | None = None) -> None:
         log_level = log_level if log_level else self.log_level
         initialize_logging(log_level=log_level, logger_name="openid_whisperer")
 
     def init_certs(self) -> None:
-        """Loads from files, CA and Org private keys and certificates. filenames are defaulted from
-        the environment variables:
-           CA_KEY_FILENAME, CA_CERT_FILENAME, ORG_KEY_FILENAME, ORG_CERT_FILENAME
+        """Loads CA certificate and Org private key and certificate from PEM formatted files.
+
+        Filenames are configured from the environment variables:
+           CA_CERT_FILENAME, ORG_KEY_FILENAME, ORG_CERT_FILENAME
+
+        If any of the files are missing, none of the certificates or private key are instantiated.
         """
-        ca_key: PrivateKeyTypes
-        org_key: PrivateKeyTypes
-        with open(self.ca_key_filename, "rb") as ca_key_file:
+
+        def load_cert_pair(
+            cert_file: TextIO,
+            key_file: Optional[TextIO] = None,
+            key_password: Optional[str] = None,
+        ) -> Tuple[x509.Certificate, Optional[rsa.RSAPrivateKey]]:
+            cert: x509.Certificate = x509.load_pem_x509_certificate(
+                cert_file.read(), default_backend()
+            )
+            if key_file is not None:
+                key_password = key_password.encode() if key_password else None
+                key = serialization.load_pem_private_key(
+                    data=key_file.read(),
+                    backend=default_backend(),
+                    password=key_password,
+                )
+                if not isinstance(key, rsa.RSAPrivateKey):
+                    raise ConfigurationException(
+                        "Only RSA private keys supported"
+                    )  # pragma: no cover
+            else:
+                key = None
+            return cert, key
+
+        self.ca_cert = None
+        if self.ca_cert_filename:
             with open(self.ca_cert_filename, "rb") as ca_cert_file:
-                with open(self.org_key_filename, "rb") as org_key_file:
-                    with open(self.org_cert_filename, "rb") as org_cert_file:
-                        ca_key_password = (
-                            self.ca_key_password.encode()
-                            if self.ca_key_password
-                            else None
-                        )
-                        ca_cert: x509.Certificate = x509.load_pem_x509_certificate(
-                            ca_cert_file.read(), default_backend()
-                        )
-                        ca_key = serialization.load_pem_private_key(
-                            data=ca_key_file.read(),
-                            backend=default_backend(),
-                            password=ca_key_password,
-                        )
-                        if not isinstance(ca_key, rsa.RSAPrivateKey):
-                            raise ConfigurationException(
-                                "Only RSA private keys supported"
-                            )  # pragma: no cover
-                        org_key_password = (
-                            self.org_key_password.encode()
-                            if self.org_key_password
-                            else None
-                        )
-                        org_cert: x509.Certificate = x509.load_pem_x509_certificate(
-                            org_cert_file.read(), default_backend()
-                        )
-                        org_key = serialization.load_pem_private_key(
-                            data=org_key_file.read(),
-                            backend=default_backend(),
-                            password=org_key_password,
-                        )
-                        if not isinstance(org_key, rsa.RSAPrivateKey):
-                            raise ConfigurationException(
-                                "Only RSA private keys supported"
-                            )  # pragma: no cover
-
-                        self.ca_key = ca_key
-                        self.ca_cert = ca_cert
-                        self.org_key = org_key
-                        self.org_cert = org_cert
+                self.ca_cert, _ = load_cert_pair(ca_cert_file, None, None)
+
+        with open(self.org_key_filename, "rb") as org_key_file:
+            with open(self.org_cert_filename, "rb") as org_cert_file:
+                self.org_cert, self.org_key = load_cert_pair(
+                    org_cert_file, org_key_file, self.org_key_password
+                )
 
 
 def get_cached_config(*args, **kwargs) -> Config:
-    """if an already cached config exists, then return an instance of that and if not then
-    initialise a new instance of the Config class.
+    """Returns a cached instance of Config, if one does not exist, then instantiate a new instance to the config cache.
+    :param args: positional arguments to instantiate Config
+    :param kwargs: Key-word arguments to instantiate Config
     """
-    global cached_config
-    if cached_config is None:
-        cached_config = Config(*args, **kwargs)
-    return cached_config
+    global _cached_config
+    if _cached_config is None:
+        _cached_config = Config(*args, **kwargs)
+        return _cached_config
+    else:
+        return _cached_config
```

### Comparing `openid_whisperer-0.1.3/src/openid_whisperer/main.py` & `openid_whisperer-0.1.4/src/openid_whisperer/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,20 +14,22 @@
     flask_app.register_blueprint(openid_blueprint)
     return flask_app
 
 
 def main() -> None:  # pragma: no cover
     """Main entrypoint for a standalone Python running instance"""
     config = get_cached_config()
+    ca_certs = [config.ca_cert] if config.ca_cert else None
+
     flask_app: Flask = app()
     flask_app.run(
         ssl_context=get_ssl_context(
             certificate=config.org_cert,
             private_key=config.org_key,
-            issuer_certs=[config.ca_cert],
+            issuer_certs=ca_certs,
             verify=False,
         ),
         host=config.id_service_bind,
         port=config.id_service_port,
         debug=config.flask_debug,
     )
```

### Comparing `openid_whisperer-0.1.3/src/openid_whisperer/openid_blueprint.py` & `openid_whisperer-0.1.4/src/openid_whisperer/openid_blueprint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """ Flask Blueprint with OpenID compatible endpoints
 """
 import logging
 import json
 from typing import Dict, Any, Type
-from urllib.parse import urljoin
 
 from flask import (
     Blueprint,
     request,
     make_response,
     render_template,
     redirect,
@@ -25,27 +24,22 @@
 from openid_whisperer.utils.credential_store import UserCredentialStoreException
 from openid_whisperer.utils.token_store import (
     TokenIssuerCertificateStoreException,
 )
 
 logger = logging.getLogger(__name__)
 
-config = get_cached_config()
-openid_api_interface = OpenidApiInterface()
-openid_blueprint: Blueprint = Blueprint(
-    "openid",
-    __name__,
-    url_prefix=config.id_service_prefix,
-    template_folder="templates",
-    static_folder="static",
-)
+
+class UserInfoExtensionTemplate:
+    pass
 
 
 def register_user_info_extension(
-    openid_api: Type[OpenidApiInterface], extension: str | Any | None = None
+    openid_api: Type[OpenidApiInterface],
+    extension: str | UserInfoExtensionTemplate | None = None,
 ) -> None:
     """Register an extension with the credential store that returns user_information claims
     :param openid_api:
     :param extension:
     """
     from openid_whisperer.utils.user_info_ext import (
         UserInfoExtensionTemplate,
@@ -58,24 +52,43 @@
         logger.info("Loading the UserInfoFakerExtension")
         extension_instance = UserInfoFakerExtension()
     elif isinstance(extension, str):
         logger.info(
             f"Unsupported extension '{extension}', loading the UserInfoExtension"
         )
     elif isinstance(extension, UserInfoExtensionTemplate):
-        logger.info(
-            f"Loading custom UserInfoExtension, '{extension.__class__}'"
-        )
+        logger.info(f"Loading custom UserInfoExtension, '{extension.__class__}'")
         extension_instance = extension
 
     if extension_instance is None:
         logger.info("loading the default UserInfoExtensions")
         extension_instance = UserInfoExtension()
 
-    openid_api.credential_store.end_user_info = extension_instance
+    openid_api.credential_store.user_info_extension = extension_instance
+
+
+config = get_cached_config()
+openid_api_interface = OpenidApiInterface(
+    ca_cert_filename=config.ca_cert_filename,
+    org_key_filename=config.org_key_filename,
+    org_key_password=config.org_key_password,
+    org_cert_filename=config.org_cert_filename,
+    validate_users=config.validate_users,
+    json_user_file=config.json_user_file,
+    session_expiry_seconds=config.session_expiry_seconds,
+    maximum_login_attempts=config.maximum_login_attempts,
+)
+
+openid_blueprint: Blueprint = Blueprint(
+    "openid",
+    __name__,
+    url_prefix=config.id_service_prefix,
+    template_folder="templates",
+    static_folder="static",
+)
 
 
 def update_redirect_url_query(
     redirect_uri: str, data: Dict[str, Any]
 ) -> ResponseReturnValue:
     if len(data) > 0:
         query_start: str = "&" if "?" in redirect_uri else "?"
```

### Comparing `openid_whisperer-0.1.3/src/openid_whisperer/openid_interface.py` & `openid_whisperer-0.1.4/src/openid_whisperer/openid_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Dict, Any, Optional, List
+from typing import Dict, Any, Optional, List, Type
 import datetime
 import hashlib
 import secrets
 from urllib.parse import urljoin
 import string
 
 from openid_whisperer.utils.common import (
@@ -13,14 +13,15 @@
     stringify,
     get_audience,
     boolify,
 )
 from openid_whisperer.utils.common import GeneralPackageException, get_seconds_epoch
 from openid_whisperer.utils.credential_store import UserCredentialStore
 from openid_whisperer.utils.token_store import TokenIssuerCertificateStore
+from openid_whisperer.utils.user_info_ext import UserInfoExtensionTemplate
 
 logger = logging.getLogger(__name__)
 
 SCOPES_SUPPORTED = [
     "user_impersonation",
     "offline_access",
     "profile",
@@ -149,24 +150,57 @@
     return grant_type
 
 
 class OpenidApiInterface:
     def __init__(self, **kwargs) -> None:
         self.issuer_reference: str | None = None
         self.devicecode_expires_in: int | None = None
+
+        # Credential related configuration
+        self.validate_users: bool | None = None
+        self.json_users: str | None = None
+        self.session_expiry_seconds: int | None = None
+        self.maximum_login_attempts: int | None = None
+        self.user_info_extension: Type[UserInfoExtensionTemplate] | None = None
+
+        # Token issue related configuration
+        self.ca_cert_filename: str = ""
+        self.org_key_filename: str = ""
+        self.org_key_password: str = ""
+        self.org_cert_filename: str = ""
+
         # Update class properties from kwargs
         for key, value in kwargs.items():
+            if not hasattr(self, key):
+                logger.warning(
+                    "Invalid initialization parameter, ignoring. %s: %s",
+                    key,
+                    str(value)[:100],
+                )
+                continue
             setattr(self, key, value)
+
         if self.issuer_reference is None or self.issuer_reference == "":
             self.issuer_reference = "urn:issuer:name:openid-whisperer"
         if self.devicecode_expires_in is None or self.devicecode_expires_in <= 0:
             self.devicecode_expires_in = 15 * 60
 
-        self.credential_store = UserCredentialStore()
-        self.token_store = TokenIssuerCertificateStore()
+        self.credential_store = UserCredentialStore(
+            validate_users=self.validate_users,
+            json_users=self.json_users,
+            session_expiry_second=self.session_expiry_seconds,
+            maximum_login_attempts=self.maximum_login_attempts,
+            user_info_extension=self.user_info_extension,
+        )
+        self.token_store = TokenIssuerCertificateStore(
+            ca_cert_filename=self.ca_cert_filename,
+            org_key_filename=self.org_key_filename,
+            org_key_password=self.org_key_password,
+            org_cert_filename=self.org_cert_filename,
+        )
 
         self.devicecode_requests: Dict[
             str, Any
         ] = {}  # device_requests Indexed by device_code
         self.devicecode_user_codes: Dict[
             str, str
         ] = {}  # device_codes Indexed by user_code
@@ -349,16 +383,17 @@
                 if device_code is None:
                     raise OpenidApiInterfaceException(
                         "devicecode_error",
                         "Invalid user code.",
                     )
                 logger.debug("device code retrieved from user_code")
 
-                devicecode_request = self.devicecode_requests.pop(device_code, None)
                 # TODO: Check details of original devicecode request against, the provided inputs to this function
+                devicecode_request = self.devicecode_requests.pop(device_code, None)
+                _ = devicecode_request
 
             """ With authentication successful for end user code response or device_code flow, a token is generated 
             that will be later retrieved by the client application.
             """
             # TODO: if scope is blank default to "openid" and update scope with client_id and resource
             user_claims = self.credential_store.get_user_scope_claims(
                 username=username, scope=scope
@@ -514,17 +549,18 @@
 
         # OpenidApiInterfaceException is raised below for an invalid grant_type
         grant_type = validate_grant_type(grant_type)
 
         token_response: Dict[str, Any] | None = None
 
         if grant_type == "device_code":
-            devicecode_request = self.devicecode_requests.get(device_code, None)
             # TODO: check devicecode_request and handle additional unsuccessful
             #  error states, request expiry, authorization_declined etc.
+            devicecode_request = self.devicecode_requests.get(device_code, None)
+            _ = devicecode_request
 
             device_authorization = self.devicecode_authorization_codes.pop(
                 device_code, None
             )
             if device_authorization is None:
                 raise OpenidApiInterfaceException(
                     "devicecode_authorization_pending",
@@ -609,16 +645,16 @@
         if not self.validate_client(client_id, client_secret):
             raise OpenidApiInterfaceException(
                 "auth_processing_error", "A valid client_id is required"
             )
         else:
             scope = "openid profile email"
             return self.credential_store.get_user_scope_claims(
-                username=username,
-                scope=scope)
+                username=username, scope=scope
+            )
 
     def get_openid_configuration(self, tenant: str, base_url: str) -> Dict[str, Any]:
         openid_configuration: Dict[str, Any] = {
             "access_token_issuer": self.issuer_reference,
             "as_access_token_token_binding_supported": False,
             "as_refresh_token_token_binding_supported": False,
             "authorization_endpoint": urljoin(base_url, f"{tenant}/oauth2/authorize"),
```

### Comparing `openid_whisperer-0.1.3/src/openid_whisperer/openid_types.py` & `openid_whisperer-0.1.4/src/openid_whisperer/openid_types.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.3/src/openid_whisperer/static/style.css` & `openid_whisperer-0.1.4/src/openid_whisperer/static/style.css`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.3/src/openid_whisperer/templates/authenticate.html` & `openid_whisperer-0.1.4/src/openid_whisperer/templates/authenticate.html`

 * *Files 0% similar despite different names*

```diff
@@ -489,15 +489,14 @@
 
                                     if (codeChallenge && !codeChallenge.value) {
                                         u.setError(password, e.codeChallengeEmpty);
                                         return false;
                                     }
 
                                     document.forms['loginForm'].submit();
-                                    //return false;
                                 };
 
                                 InputUtil.makePlaceholder(Login.userNameInput);
                                 InputUtil.makePlaceholder(Login.passwordInput);
 
                                 //]]>
                             </script>
```

### Comparing `openid_whisperer-0.1.3/src/openid_whisperer/utils/common.py` & `openid_whisperer-0.1.4/src/openid_whisperer/utils/common.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.3/src/openid_whisperer/utils/config_utils.py` & `openid_whisperer-0.1.4/src/openid_whisperer/utils/config_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from logging import Formatter as LogFormatter
 import os
 import sys
 from typing import Dict, Any, Iterable, Callable, Tuple
 
 from dotenv import load_dotenv
 
-default_config_type = Dict[str, Tuple[Callable[[str], Any], str]]
+default_config_type = Dict[str, Tuple[Callable[[Any], Any], Any]]
 
 DEFAULT_LOGGING_FORMAT = "[%(levelname)1.1s %(asctime)s.%(msecs)03d %(process)d %(module)s:%(lineno)d %(name)s] %(message)s"
 
 logger = logging.getLogger(__name__)
 
 
 def load_environment_variables(env_target: str | None = None) -> None:
```

### Comparing `openid_whisperer-0.1.3/src/openid_whisperer/utils/credential_store.py` & `openid_whisperer-0.1.4/src/openid_whisperer/utils/credential_store.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,55 @@
+import logging
 from typing import Dict, Any, Optional, Type
 
 from openid_whisperer.utils.user_info_ext import (
     UserInfoExtension,
     UserInfoExtensionTemplate,
 )
 
 from openid_whisperer.utils.common import (
     GeneralPackageException,
     get_now_seconds_epoch,
 )
 
+logger = logging.getLogger(__name__)
+
 
 class UserCredentialStoreException(GeneralPackageException):
     """Exception raised when UserCredentialStore requirements are not met, other runtime
     exceptions are passed through.
     """
 
 
 class UserCredentialStore:
     """A class that provides end user management for an identity provider
 
     maximum_login_attempts of None or <=0 enables infinite authentication attempts
     """
 
     def __init__(self, **kwargs: Dict[str, Any]) -> None:
-        self.validate_user: bool | None = None
+        self.validate_users: bool | None = None
         self.json_users: str | None = None
         self.session_expiry_seconds: int | None = None
         self.maximum_login_attempts: int | None = None
-        self.end_user_info: Type[UserInfoExtensionTemplate] | None = None
+        self.user_info_extension: Type[UserInfoExtensionTemplate] | None = None
 
         # Update class properties from kwargs
         for key, value in kwargs.items():
+            if not hasattr(self, key):
+                logger.warning(
+                    "Invalid initialization parameter, ignoring. %s: %s",
+                    key,
+                    str(value)[:100],
+                )
+                continue
             setattr(self, key, value)
 
-        if self.end_user_info is None:
-            self.end_user_info = UserInfoExtension()
+        if self.user_info_extension is None:
+            self.user_info_extension = UserInfoExtension()
 
         self.authenticated_session: Dict[
             str, float
         ] = {}  # login_time_stamp indexed by username
         self.failed_login_attempts: Dict[str, int] = {}  # Indexed by username
 
     def logoff(self, tenant: str, username: str) -> None:
@@ -94,26 +104,25 @@
         ):
             return self.count_failed_authentication(username)
 
         # Mock user credentials require a non-zero length password
         if not password:
             return self.count_failed_authentication(username)
 
-        if self.validate_user:
-            user = self.end_user_info.get_user_claims(username)
-            if user is None:
-                return False
+        if self.validate_users:
+            user = self.user_info_extension.get_user_claims(username, scope="openid")
+            if user:
+                return True
+            return False
 
         # existing session will be extended by session_expiry_seconds
         self.authenticated_session[username] = get_now_seconds_epoch()
 
         return True
 
-    def get_user_scope_claims(
-        self, username: str, scope: str
-    ) -> Dict[str, Any]:
+    def get_user_scope_claims(self, username: str, scope: str) -> Dict[str, Any]:
         _ = scope
 
-        openid_claims_payload = self.end_user_info.get_user_claims(
+        openid_claims_payload = self.user_info_extension.get_user_claims(
             username=username, scope=scope, including_empty=False
         )
         return openid_claims_payload
```

### Comparing `openid_whisperer-0.1.3/src/openid_whisperer/utils/token_store.py` & `openid_whisperer-0.1.4/src/openid_whisperer/utils/token_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from openid_whisperer.utils.common import (
     GeneralPackageException,
     generate_s256_hash,
     get_now_seconds_epoch,
     get_seconds_epoch,
 )
 
+logger = logging.getLogger(__name__)
+
 TokenTypes = Literal["token", "refresh_token"]
 
 
 class CertificatePairType(TypedDict):
     certificate: x509.Certificate
     private_key: Optional[CertificateIssuerPrivateKeyTypes]
 
@@ -64,25 +66,30 @@
     """
 
     def __init__(self, **kwargs):
         """
         Parameters
         ----------
         """
-        self.ca_key_filename: str = "certs/ca_key.pem"
-        self.ca_key_password: str = ""
-        self.ca_cert_filename: str = "certs/ca_cert.pem"
-        self.org_key_filename: str = "certs/key.pem"
+        self.ca_cert_filename: str = ""
+        self.org_key_filename: str = ""
         self.org_key_password: str = ""
-        self.org_cert_filename: str = "certs/cert.pem"
+        self.org_cert_filename: str = ""
         self.token_expiry_seconds: int | None = 600
         self.refresh_token_expiry_seconds: int | None = 3600
 
         # Update class properties from kwargs
         for key, value in kwargs.items():
+            if not hasattr(self, key):
+                logger.warning(
+                    "Invalid initialization parameter, ignoring. %s: %s",
+                    key,
+                    str(value)[:100],
+                )
+                continue
             setattr(self, key, value)
 
         # Check config and update with reasonable defaults
         if self.token_expiry_seconds is None or self.token_expiry_seconds <= 0:
             self.token_expiry_seconds = 600  # 10 minutes
         if (
             self.refresh_token_expiry_seconds is None
@@ -121,52 +128,64 @@
 
     @property
     def token_issuer_certificate(self):
         return self.token_certificates[self.token_issuer_key_id]["certificate"]
 
     @classmethod
     def load_certificate_pair(
-        cls, cert_filename: str, key_filename: str | None, key_password: str | None
-    ) -> CertificatePairType:
+        cls,
+        cert_filename: str | None = None,
+        key_filename: str | None = None,
+        key_password: str | None = None,
+    ) -> Optional[CertificatePairType]:
+        """returns a Private Key / certificate pair, where:
+            * cert_filename is None, then return None
+            * key_filename is None, the return  CertificatePairType with only the certificate populated.
+
+        :param cert_filename:
+        :param key_filename:
+        :param key_password:
+        :return:
+        """
+        if cert_filename is None:
+            return None
         certificate: x509.Certificate
         with open(cert_filename, "rb") as cert_file:
             certificate = x509.load_pem_x509_certificate(
                 cert_file.read(), default_backend()
             )
-            # TODO: certificate validation
 
         private_key: CertificateIssuerPrivateKeyTypes | None = None
         if key_filename:
             with open(key_filename, "rb") as key_file:
-                key_password: bytes = key_password.encode() if key_password else None
+                password: bytes = key_password.encode() if key_password else None
                 private_key = serialization.load_pem_private_key(
                     data=key_file.read(),
                     backend=default_backend(),
-                    password=key_password,
+                    password=password,
                 )
                 if not isinstance(private_key, CertificateIssuerPrivateKeyTypes):
                     raise TokenIssuerCertificateStoreException(
                         "invalid_private_key",
                         "Only private keys that support x509 certificates are allowed",
                     )  # pragma: no cover
 
         return {
             "private_key": private_key,
             "certificate": certificate,
         }
 
     def init_certificate_store(self) -> None:
         """Loads ca certificate and org private keys and certificate pairs."""
-        # Loading ca certificate
-        certificate_pair = self.load_certificate_pair(
-            self.ca_cert_filename, self.ca_key_filename, self.ca_key_password
-        )
-        certificate = certificate_pair["certificate"]
-        certificate_id = str(certificate.serial_number)
-        self.ca_certificates[certificate_id] = certificate
+        # Loading ca certificate if provided
+        certificate_pair = self.load_certificate_pair(self.ca_cert_filename, None, None)
+        if certificate_pair is not None:
+            certificate = certificate_pair["certificate"]
+            certificate_id = str(certificate.serial_number)
+            self.ca_certificates[certificate_id] = certificate
 
         # Init org cert-key pairs
         certificate_pair = self.load_certificate_pair(
             self.org_cert_filename, self.org_key_filename, self.org_key_password
         )
         certificate = certificate_pair["certificate"]
         certificate_id = str(certificate.serial_number)
@@ -224,14 +243,15 @@
         The claims iss, sun, exp, iat, auth_time, appid, ver are overriden by the TokenIssuerCertificateStore
 
         :param client_id:
         :param issuer:
         :param sub:
         :param user_claims:
         :param audience:
+        :param nonce:
         :return:
         """
         auth_time = datetime.datetime.utcnow()
         expires_in = auth_time + datetime.timedelta(seconds=self.token_expiry_seconds)
         payload = {}
         payload.update(user_claims)
         payload["nonce"] = nonce
@@ -303,11 +323,11 @@
                 )
                 if claims["jti"] not in self.tokens_issued:
                     return False  # pragma: no cover
                 if get_now_seconds_epoch() > claims["exp"]:
                     return False  # pragma: no cover
                 return True
             except Exception as e:
-                logging.exception(e)
+                logger.exception(e)
                 return False
         else:
             return token in self.refresh_tokens_issued
```

### Comparing `openid_whisperer-0.1.3/src/openid_whisperer/utils/token_utils.py` & `openid_whisperer-0.1.4/src/openid_whisperer/utils/token_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         for _ in range(int(cer_len / 64)):
             temp_cer = temp_cer[:count] + ret_char + temp_cer[count:]
             count = count + 64 + len(ret_char)
 
         temp_cer = temp_cer + ret_char if ins_extra_ret else temp_cer
 
         tok_sign_cer = (
-            "-----BEGIN CERTIFICATE-----\r\n" + temp_cer + "-----END CERTIFICATE-----"
+            f"-----BEGIN CERTIFICATE-----\r\n{temp_cer}-----END CERTIFICATE-----"
         )
 
         cert = x509.load_pem_x509_certificate(tok_sign_cer.encode(), default_backend())
         public_key = cert.public_key()
 
         # Set the idp_keys discretionary entry
         jwks_keys[x5t] = public_key
```

### Comparing `openid_whisperer-0.1.3/src/openid_whisperer/utils/user_info_ext.py` & `openid_whisperer-0.1.4/src/openid_whisperer/utils/user_info_ext.py`

 * *Files identical despite different names*

### Comparing `openid_whisperer-0.1.3/PKG-INFO` & `openid_whisperer-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openid-whisperer
-Version: 0.1.3
+Version: 0.1.4
 Summary: OpenID 1.0 Mock Identity Service
 Home-page: https://github.com/robertbetts/openid-whisperer
 License: MIT
 Keywords: python,mock,api,oauth2,openid
 Author: Robert Betts
 Author-email: betts_robert@yahoo.com
 Maintainer: Robert Betts
@@ -134,17 +134,14 @@
 ```commandline
 cd openid-whisperer
 poetry install
 poetry update
 ```
 6. Setup environment variables, default `.env` and `.env_${ENVIRONMENT:-TEST}`
 ```
-INTERNAL_HOST=${INTERNAL_HOST:-localhost}
-GATEWAY_HOST=${GATEWAY_HOST:-localhost}
-
 API_HOST=${INTERNAL_HOST:-localhost}
 API_PORT=${API_PORT:-5700}
 API_HOST_GW=${GATEWAY_HOST:-localhost}
 API_PORT_GW=${API_PORT_GW:-8100}
 
 ID_SERVICE_PORT=${ID_SERVICE_PORT:-5000}
 ID_SERVICE_HOST=${INTERNAL_HOST:-localhost}
@@ -172,10 +169,10 @@
 Run OpenID Whisperer (from project root)
 ```
 poetry run python -m openid_whisperer.main 
 ```
 
 Run within a Docker Container
 ```
-docker build -t opendid-whisperer:0.1.0 .
-docker run --name=openid-whisperer -p5005:5000  -eID_SERVICE_PORT_GW=5005 opendid-whisperer:0.1.0
+docker build -t opendid-whisperer:0.1.4 .
+docker run --name=openid-whisperer -p5005:5005  -eID_SERVICE_PORT_GW=5005 opendid-whisperer:0.1.4
 ```
```

