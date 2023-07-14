# Comparing `tmp/openconnect-sso-0.7.3.tar.gz` & `tmp/openconnect_sso-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openconnect-sso-0.7.3.tar", last modified: Thu Apr 15 10:32:38 2021, max compression
+gzip compressed data, was "openconnect_sso-0.8.1.tar", max compression
```

## Comparing `openconnect-sso-0.7.3.tar` & `openconnect_sso-0.8.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    35149 2019-09-09 12:34:19.265972 openconnect-sso-0.7.3/LICENSE
--rw-r--r--   0        0        0     4883 2021-01-28 13:08:16.926336 openconnect-sso-0.7.3/README.md
--rw-r--r--   0        0        0      270 2020-02-23 21:19:10.446107 openconnect-sso-0.7.3/openconnect_sso/__init__.py
--rw-r--r--   0        0        0     6052 2021-04-15 10:30:21.509202 openconnect-sso-0.7.3/openconnect_sso/app.py
--rw-r--r--   0        0        0     7204 2021-03-30 18:52:03.471250 openconnect-sso-0.7.3/openconnect_sso/authenticator.py
--rw-r--r--   0        0        0      100 2020-02-23 22:34:18.915239 openconnect-sso-0.7.3/openconnect_sso/browser/__init__.py
--rw-r--r--   0        0        0     2481 2020-10-26 09:38:32.205993 openconnect-sso-0.7.3/openconnect_sso/browser/browser.py
--rw-r--r--   0        0        0       37 2020-10-19 13:48:00.913480 openconnect-sso-0.7.3/openconnect_sso/browser/user.js
--rw-r--r--   0        0        0     6794 2021-04-15 10:28:35.145673 openconnect-sso-0.7.3/openconnect_sso/browser/webengine_process.py
--rwxr-xr-x   0        0        0     4786 2021-03-30 18:52:03.471250 openconnect-sso-0.7.3/openconnect_sso/cli.py
--rw-r--r--   0        0        0     3529 2021-03-26 10:16:03.002612 openconnect-sso-0.7.3/openconnect_sso/config.py
--rw-r--r--   0        0        0     1180 2020-02-23 21:19:10.446107 openconnect-sso-0.7.3/openconnect_sso/profile.py
--rw-r--r--   0        0        0      518 2021-03-01 17:13:05.464958 openconnect-sso-0.7.3/openconnect_sso/saml_authenticator.py
--rw-r--r--   0        0        0       34 2020-02-23 21:19:10.447107 openconnect-sso-0.7.3/openconnect_sso/version.py
--rw-r--r--   0        0        0     1626 2021-04-15 10:29:48.439044 openconnect-sso-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     6363 2021-04-15 10:32:38.688772 openconnect-sso-0.7.3/setup.py
--rw-r--r--   0        0        0     6445 2021-04-15 10:32:38.689584 openconnect-sso-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-11-18 16:32:38.000000 openconnect_sso-0.8.1/LICENSE
+-rw-r--r--   0        0        0     5808 2023-07-14 14:54:12.457664 openconnect_sso-0.8.1/README.md
+-rw-r--r--   0        0        0      270 2021-11-18 16:32:38.000000 openconnect_sso-0.8.1/openconnect_sso/__init__.py
+-rw-r--r--   0        0        0     6899 2023-07-14 14:54:12.458664 openconnect_sso-0.8.1/openconnect_sso/app.py
+-rw-r--r--   0        0        0     7306 2023-07-14 14:54:12.458664 openconnect_sso-0.8.1/openconnect_sso/authenticator.py
+-rw-r--r--   0        0        0      100 2021-11-18 16:32:38.000000 openconnect_sso-0.8.1/openconnect_sso/browser/__init__.py
+-rw-r--r--   0        0        0     2481 2021-11-18 16:32:38.000000 openconnect_sso-0.8.1/openconnect_sso/browser/browser.py
+-rw-r--r--   0        0        0       37 2021-11-18 16:32:38.000000 openconnect_sso-0.8.1/openconnect_sso/browser/user.js
+-rw-r--r--   0        0        0     8163 2023-07-14 14:54:12.458664 openconnect_sso-0.8.1/openconnect_sso/browser/webengine_process.py
+-rwxr-xr-x   0        0        0     4979 2023-07-14 14:54:12.458664 openconnect_sso-0.8.1/openconnect_sso/cli.py
+-rw-r--r--   0        0        0     4499 2023-07-14 14:54:12.458664 openconnect_sso-0.8.1/openconnect_sso/config.py
+-rw-r--r--   0        0        0     1180 2021-11-18 16:32:38.000000 openconnect_sso-0.8.1/openconnect_sso/profile.py
+-rw-r--r--   0        0        0      518 2021-11-18 16:32:38.000000 openconnect_sso-0.8.1/openconnect_sso/saml_authenticator.py
+-rw-r--r--   0        0        0       34 2021-11-18 16:32:38.000000 openconnect_sso-0.8.1/openconnect_sso/version.py
+-rw-r--r--   0        0        0     1401 2023-07-14 15:05:32.900693 openconnect_sso-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7356 1970-01-01 00:00:00.000000 openconnect_sso-0.8.1/PKG-INFO
```

### Comparing `openconnect-sso-0.7.3/LICENSE` & `openconnect_sso-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openconnect-sso-0.7.3/README.md` & `openconnect_sso-0.8.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -33,20 +33,14 @@
 Consider adding shell completions for pipx. Run 'pipx completions' for
 instructions.
 
 You likely need to open a new terminal or re-login for the changes to take
 effect. ✨ 🌟 ✨
 ```
 
-If you have Qt 5.x installed, you can skip the installation of bundled Qt version:
-
-``` bash
-pipx install openconnect-sso
-```
-
 Of course you can also install via `pip` instead of `pipx` if you'd like to
 install system-wide or a virtualenv of your choice.
 
 ### On Arch Linux
 
 There is an unofficial package available for Arch Linux on
 [AUR](https://aur.archlinux.org/packages/openconnect-sso/). You can use your
@@ -123,14 +117,50 @@
 [info     ] Authenticating to VPN endpoint ...
 ```
 
 Configuration is saved in `$XDG_CONFIG_HOME/openconnect-sso/config.toml`. On
 typical Linux installations it is located under
 `$HOME/.config/openconnect-sso/config.toml`
 
+For CISCO-VPN and TOTP the following seems to work by tuning the config.toml
+and removing the default "submit"-action to the following:
+
+```
+[[auto_fill_rules."https://*"]]
+selector = "input[data-report-event=Signin_Submit]"
+action = "click"
+
+[[auto_fill_rules."https://*"]]
+selector = "input[type=tel]"
+fill = "totp"
+```
+
+### Adding custom `openconnect` arguments
+
+Sometimes you need to add custom `openconnect` arguments. One situation can be if you get similar error messages:
+
+```shell
+Failed to read from SSL socket: The transmitted packet is too large (EMSGSIZE).
+Failed to recv DPD request (-5)
+```
+
+or:
+
+```shell
+Detected MTU of 1370 bytes (was 1406)
+```
+
+Generally, you can add `openconnect` arguments after the `--` separator. This is called _"positional arguments"_. The
+solution of the previous errors is setting `--base-mtu` e.g.:
+
+```shell
+openconnect-sso --server vpn.server.com/group --user user@domain.com -- --base-mtu=1370
+#                                                          separator ^^|^^^^^^^^^^^^^^^ openconnect args
+```
+
 ## Development
 
 `openconnect-sso` is developed using [Nix](https://nixos.org/nix/). Refer to the
 [Quick Start section of the Nix
 manual](https://nixos.org/nix/manual/#chap-quick-start) to see how to get it
 installed on your machine.
```

### Comparing `openconnect-sso-0.7.3/openconnect_sso/app.py` & `openconnect_sso-0.8.1/openconnect_sso/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import asyncio
 import getpass
 import json
 import logging
 import os
-import shlex
 import signal
 import subprocess
 from pathlib import Path
 
+import shlex
+import shutil
 import structlog
 from prompt_toolkit import HTML
 from prompt_toolkit.shortcuts import radiolist_dialog
 
 from openconnect_sso import config
 from openconnect_sso.authenticator import Authenticator, AuthResponseError
 from openconnect_sso.browser import Terminated
@@ -68,15 +69,19 @@
             print(
                 "\n".join(f"{k.upper()}={shlex.quote(v)}" for k, v in details.items())
             )
         return 0
 
     try:
         return run_openconnect(
-            auth_response, selected_profile, args.proxy, args.openconnect_args
+            auth_response,
+            selected_profile,
+            args.proxy,
+            args.ac_version,
+            args.openconnect_args,
         )
     except KeyboardInterrupt:
         logger.warn("CTRL-C pressed, exiting")
         return 0
     finally:
         handle_disconnect(cfg.on_disconnect)
 
@@ -109,14 +114,20 @@
     elif args.user:
         credentials = Credentials(args.user)
 
     if credentials and not credentials.password:
         credentials.password = getpass.getpass(prompt=f"Password ({args.user}): ")
         cfg.credentials = credentials
 
+    if credentials and not credentials.totp:
+        credentials.totp = getpass.getpass(
+            prompt=f"TOTP secret (leave blank if not required) ({args.user}): "
+        )
+        cfg.credentials = credentials
+
     if cfg.default_profile and not (args.use_profile_selector or args.server):
         selected_profile = cfg.default_profile
     elif args.use_profile_selector or args.profile_path:
         profiles = get_profiles(Path(args.profile_path))
         if not profiles:
             raise ValueError("No profile found", 17)
 
@@ -128,20 +139,22 @@
             args.server, args.usergroup, args.authgroup
         )
     else:
         raise ValueError(
             "Cannot determine server address. Invalid arguments specified.", 19
         )
 
-    cfg.default_profile = selected_profile
+    cfg.default_profile = config.HostProfile(
+        selected_profile.address, selected_profile.user_group, selected_profile.name
+    )
 
     display_mode = config.DisplayMode[args.browser_display_mode.upper()]
 
     auth_response = await authenticate_to(
-        selected_profile, args.proxy, credentials, display_mode
+        selected_profile, args.proxy, credentials, display_mode, args.ac_version
     )
 
     if args.on_disconnect and not cfg.on_disconnect:
         cfg.on_disconnect = args.on_disconnect
 
     return auth_response, selected_profile
 
@@ -161,34 +174,45 @@
         asyncio.get_event_loop().remove_signal_handler(signal.SIGWINCH)
     if not selection:
         return selection
     logger.info("Selected profile", profile=selection.name)
     return selection
 
 
-def authenticate_to(host, proxy, credentials, display_mode):
+def authenticate_to(host, proxy, credentials, display_mode, version):
     logger.info("Authenticating to VPN endpoint", name=host.name, address=host.address)
-    return Authenticator(host, proxy, credentials).authenticate(display_mode)
+    return Authenticator(host, proxy, credentials, version).authenticate(display_mode)
+
 
+def run_openconnect(auth_info, host, proxy, version, args):
+    as_root = next((prog for prog in ("doas", "sudo") if shutil.which(prog)), None)
+    if not as_root:
+        logger.error(
+            "Cannot find suitable program to execute as superuser (doas/sudo), exiting"
+        )
+        return 20
 
-def run_openconnect(auth_info, host, proxy, args):
     command_line = [
-        "sudo",
+        as_root,
         "openconnect",
-        "--cookie",
-        auth_info.session_token,
+        "--useragent",
+        f"AnyConnect Linux_64 {version}",
+        "--version-string",
+        version,
+        "--cookie-on-stdin",
         "--servercert",
         auth_info.server_cert_hash,
         *args,
         host.vpn_url,
     ]
     if proxy:
         command_line.extend(["--proxy", proxy])
 
+    session_token = auth_info.session_token.encode("utf-8")
     logger.debug("Starting OpenConnect", command_line=command_line)
-    return subprocess.run(command_line).returncode
+    return subprocess.run(command_line, input=session_token).returncode
 
 
 def handle_disconnect(command):
     if command:
         logger.info("Running command on disconnect", command_line=command)
         return subprocess.run(command, timeout=5, shell=True).returncode
```

### Comparing `openconnect-sso-0.7.3/openconnect_sso/authenticator.py` & `openconnect_sso-0.8.1/openconnect_sso/authenticator.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from openconnect_sso.saml_authenticator import authenticate_in_browser
 
 
 logger = structlog.get_logger()
 
 
 class Authenticator:
-    def __init__(self, host, proxy=None, credentials=None):
+    def __init__(self, host, proxy=None, credentials=None, version=None):
         self.host = host
         self.proxy = proxy
         self.credentials = credentials
-        self.session = create_http_session(proxy)
+        self.version = version
+        self.session = create_http_session(proxy, version)
 
     async def authenticate(self, display_mode):
         self._detect_authentication_target_url()
 
         response = self._start_authentication()
         if not isinstance(response, AuthRequestResponse):
             logger.error(
@@ -56,28 +57,28 @@
         # Authentication will occcur using a POST request on the final URL
         response = requests.get(self.host.vpn_url)
         response.raise_for_status()
         self.host.address = response.url
         logger.debug("Auth target url", url=self.host.vpn_url)
 
     def _start_authentication(self):
-        request = _create_auth_init_request(self.host, self.host.vpn_url)
+        request = _create_auth_init_request(self.host, self.host.vpn_url, self.version)
         logger.debug("Sending auth init request", content=request)
         response = self.session.post(self.host.vpn_url, request)
         logger.debug("Auth init response received", content=response.content)
         return parse_response(response)
 
     async def _authenticate_in_browser(self, auth_request_response, display_mode):
         return await authenticate_in_browser(
             self.proxy, auth_request_response, self.credentials, display_mode
         )
 
     def _complete_authentication(self, auth_request_response, sso_token):
         request = _create_auth_finish_request(
-            self.host, auth_request_response, sso_token
+            self.host, auth_request_response, sso_token, self.version
         )
         logger.debug("Sending auth finish request", content=request)
         response = self.session.post(self.host.vpn_url, request)
         logger.debug("Auth finish response received", content=response.content)
         return parse_response(response)
 
 
@@ -85,20 +86,20 @@
     pass
 
 
 class AuthResponseError(AuthenticationError):
     pass
 
 
-def create_http_session(proxy):
+def create_http_session(proxy, version):
     session = requests.Session()
     session.proxies = {"http": proxy, "https": proxy}
     session.headers.update(
         {
-            "User-Agent": "AnyConnect Linux_64 4.7.00136",
+            "User-Agent": f"AnyConnect Linux_64 {version}",
             "Accept": "*/*",
             "Accept-Encoding": "identity",
             "X-Transcend-Version": "1",
             "X-Aggregate-Auth": "1",
             "X-Support-HTTP-Auth": "true",
             "Content-Type": "application/x-www-form-urlencoded",
             # I know, it is invalid but that’s what Anyconnect sends
@@ -106,26 +107,26 @@
     )
     return session
 
 
 E = objectify.ElementMaker(annotate=False)
 
 
-def _create_auth_init_request(host, url):
+def _create_auth_init_request(host, url, version):
     ConfigAuth = getattr(E, "config-auth")
     Version = E.version
     DeviceId = getattr(E, "device-id")
     GroupSelect = getattr(E, "group-select")
     GroupAccess = getattr(E, "group-access")
     Capabilities = E.capabilities
     AuthMethod = getattr(E, "auth-method")
 
     root = ConfigAuth(
         {"client": "vpn", "type": "init", "aggregate-auth-version": "2"},
-        Version({"who": "vpn"}, "4.7.00136"),
+        Version({"who": "vpn"}, version),
         DeviceId("linux-64"),
         GroupSelect(host.name),
         GroupAccess(url),
         Capabilities(AuthMethod("single-sign-on-v2")),
     )
     return etree.tostring(
         root, pretty_print=True, xml_declaration=True, encoding="UTF-8"
@@ -196,26 +197,26 @@
 class AuthCompleteResponse:
     auth_id = attr.ib(converter=str)
     auth_message = attr.ib(converter=str)
     session_token = attr.ib(converter=str)
     server_cert_hash = attr.ib(converter=str)
 
 
-def _create_auth_finish_request(host, auth_info, sso_token):
+def _create_auth_finish_request(host, auth_info, sso_token, version):
     ConfigAuth = getattr(E, "config-auth")
     Version = E.version
     DeviceId = getattr(E, "device-id")
     SessionToken = getattr(E, "session-token")
     SessionId = getattr(E, "session-id")
     Auth = E.auth
     SsoToken = getattr(E, "sso-token")
 
     root = ConfigAuth(
         {"client": "vpn", "type": "auth-reply", "aggregate-auth-version": "2"},
-        Version({"who": "vpn"}, "4.7.00136"),
+        Version({"who": "vpn"}, version),
         DeviceId("linux-64"),
         SessionToken(),
         SessionId(),
         auth_info.opaque,
         Auth(SsoToken(sso_token)),
     )
     return etree.tostring(
```

### Comparing `openconnect-sso-0.7.3/openconnect_sso/browser/browser.py` & `openconnect_sso-0.8.1/openconnect_sso/browser/browser.py`

 * *Files identical despite different names*

### Comparing `openconnect-sso-0.7.3/openconnect_sso/browser/webengine_process.py` & `openconnect_sso-0.8.1/openconnect_sso/browser/webengine_process.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 import sys
 from urllib.parse import urlparse
 
 import attr
 import pkg_resources
 import structlog
 
-from PyQt5.QtCore import QUrl, QTimer
-from PyQt5.QtNetwork import QNetworkCookie, QNetworkProxy
-from PyQt5.QtWebEngineWidgets import QWebEngineView, QWebEngineScript, QWebEngineProfile
-from PyQt5.QtWidgets import QApplication
+from PyQt6.QtCore import QUrl, QTimer, pyqtSlot, Qt
+from PyQt6.QtNetwork import QNetworkCookie, QNetworkProxy
+from PyQt6.QtWebEngineCore import QWebEngineScript, QWebEngineProfile, QWebEnginePage
+from PyQt6.QtWebEngineWidgets import QWebEngineView
+from PyQt6.QtWidgets import QApplication, QWidget, QSizePolicy, QVBoxLayout
 
 from openconnect_sso import config
 
 
 app = None
 logger = structlog.get_logger("webengine")
 
@@ -104,15 +105,15 @@
         logger.info("Browser started", startup_info=startup_info)
 
         logger.info("Loading page", url=startup_info.url)
 
         web.authenticate_at(QUrl(startup_info.url), startup_info.credentials)
 
         web.show()
-        rc = app.exec_()
+        rc = app.exec()
 
         logger.info("Exiting browser")
         return rc
 
     async def wait(self):
         while self.is_alive():
             await asyncio.sleep(0.01)
@@ -141,28 +142,33 @@
         super().__init__()
         self._on_update = on_update
         self._auto_fill_rules = auto_fill_rules
         cookie_store = self.page().profile().cookieStore()
         cookie_store.cookieAdded.connect(self._on_cookie_added)
         self.page().loadFinished.connect(self._on_load_finished)
 
+    def createWindow(self, type):
+        if type == QWebEnginePage.WebDialog:
+            self._popupWindow = WebPopupWindow(self.page().profile())
+            return self._popupWindow.view()
+
     def authenticate_at(self, url, credentials):
         script_source = pkg_resources.resource_string(__name__, "user.js").decode()
         script = QWebEngineScript()
-        script.setInjectionPoint(QWebEngineScript.DocumentCreation)
-        script.setWorldId(QWebEngineScript.ApplicationWorld)
+        script.setInjectionPoint(QWebEngineScript.InjectionPoint.DocumentCreation)
+        script.setWorldId(QWebEngineScript.ScriptWorldId.ApplicationWorld)
         script.setSourceCode(script_source)
         self.page().scripts().insert(script)
 
         if credentials:
             logger.info("Initiating autologin", cred=credentials)
             for url_pattern, rules in self._auto_fill_rules.items():
                 script = QWebEngineScript()
-                script.setInjectionPoint(QWebEngineScript.DocumentReady)
-                script.setWorldId(QWebEngineScript.ApplicationWorld)
+                script.setInjectionPoint(QWebEngineScript.InjectionPoint.DocumentReady)
+                script.setWorldId(QWebEngineScript.ScriptWorldId.ApplicationWorld)
                 script.setSourceCode(
                     f"""
 // ==UserScript==
 // @include {url_pattern}
 // ==/UserScript==
 
 function autoFill() {{
@@ -183,14 +189,45 @@
     def _on_load_finished(self, success):
         url = self.page().url().toString()
         logger.debug("Page loaded", url=url)
 
         self._on_update(Url(url))
 
 
+class WebPopupWindow(QWidget):
+    def __init__(self, profile):
+        super().__init__()
+        self._view = QWebEngineView(self)
+
+        super().setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose)
+        super().setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
+
+        layout = QVBoxLayout()
+        super().setLayout(layout)
+        layout.addWidget(self._view)
+
+        self._view.setPage(QWebEnginePage(profile, self._view))
+
+        self._view.titleChanged.connect(super().setWindowTitle)
+        self._view.page().geometryChangeRequested.connect(
+            self.handleGeometryChangeRequested
+        )
+        self._view.page().windowCloseRequested.connect(super().close)
+
+    def view(self):
+        return self._view
+
+    @pyqtSlot("const QRect")
+    def handleGeometryChangeRequested(self, newGeometry):
+        self._view.setMinimumSize(newGeometry.width(), newGeometry.height())
+        super().move(newGeometry.topLeft() - self._view.pos())
+        super().resize(0, 0)
+        super().show()
+
+
 def to_str(qval):
     return bytes(qval).decode()
 
 
 def get_selectors(rules, credentials):
     statements = []
     for rule in rules:
```

### Comparing `openconnect-sso-0.7.3/openconnect_sso/cli.py` & `openconnect_sso-0.8.1/openconnect_sso/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,14 +86,20 @@
     )
 
     parser.add_argument(
         "-V", "--version", action="version", version=f"%(prog)s {__version__}"
     )
 
     parser.add_argument(
+        "--ac-version",
+        help="AnyConnect Version used for authentication and for OpenConnect, defaults to %(default)s",
+        default="4.7.00136",
+    )
+
+    parser.add_argument(
         "-l",
         "--log-level",
         help="",
         type=LogLevel.parse,
         choices=LogLevel.choices(),
         default=LogLevel.INFO,
     )
@@ -112,15 +118,15 @@
     return parser
 
 
 class StoreOpenConnectArgs(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
         if "--" in values:
             values.remove("--")
-        setattr(namespace, self.dest, values)
+        setattr(namespace, self.dest, values[1:])
 
 
 class LogLevel(enum.IntEnum):
     ERROR = logging.ERROR
     WARNING = logging.WARNING
     INFO = logging.INFO
     DEBUG = logging.DEBUG
```

### Comparing `openconnect-sso-0.7.3/openconnect_sso/config.py` & `openconnect_sso-0.8.1/openconnect_sso/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import enum
 from pathlib import Path
 from urllib.parse import urlparse, urlunparse
 
 import attr
 import keyring
 import keyring.errors
+import pyotp
 import structlog
 import toml
 import xdg.BaseDirectory
 
 logger = structlog.get_logger()
 
 APP_NAME = "openconnect-sso"
@@ -83,16 +84,25 @@
 
 
 def get_default_auto_fill_rules():
     return {
         "https://*": [
             AutoFillRule(selector="div[id=passwordError]", action="stop").as_dict(),
             AutoFillRule(selector="input[type=email]", fill="username").as_dict(),
-            AutoFillRule(selector="input[type=password]", fill="password").as_dict(),
-            AutoFillRule(selector="input[type=submit]", action="click").as_dict(),
+            AutoFillRule(selector="input[name=passwd]", fill="password").as_dict(),
+            AutoFillRule(
+                selector="input[data-report-event=Signin_Submit]", action="click"
+            ).as_dict(),
+            AutoFillRule(
+                selector="div[data-value=PhoneAppOTP]", action="click"
+            ).as_dict(),
+            AutoFillRule(selector="a[id=signInAnotherWay]", action="click").as_dict(),
+            AutoFillRule(
+                selector="input[id=idTxtBx_SAOTCC_OTC]", fill="totp"
+            ).as_dict(),
         ]
     }
 
 
 @attr.s
 class Credentials(ConfigNode):
     username = attr.ib()
@@ -108,14 +118,30 @@
     @password.setter
     def password(self, value):
         try:
             keyring.set_password(APP_NAME, self.username, value)
         except keyring.errors.KeyringError:
             logger.info("Cannot save password to keyring.")
 
+    @property
+    def totp(self):
+        try:
+            totpsecret = keyring.get_password(APP_NAME, "totp/" + self.username)
+            return pyotp.TOTP(totpsecret).now() if totpsecret else None
+        except keyring.errors.KeyringError:
+            logger.info("Cannot retrieve saved totp info from keyring.")
+            return ""
+
+    @totp.setter
+    def totp(self, value):
+        try:
+            keyring.set_password(APP_NAME, "totp/" + self.username, value)
+        except keyring.errors.KeyringError:
+            logger.info("Cannot save totp secret to keyring.")
+
 
 @attr.s
 class Config(ConfigNode):
     default_profile = attr.ib(default=None, converter=HostProfile.from_dict)
     credentials = attr.ib(default=None, converter=Credentials.from_dict)
     auto_fill_rules = attr.ib(
         factory=get_default_auto_fill_rules,
```

### Comparing `openconnect-sso-0.7.3/openconnect_sso/profile.py` & `openconnect_sso-0.8.1/openconnect_sso/profile.py`

 * *Files identical despite different names*

### Comparing `openconnect-sso-0.7.3/openconnect_sso/saml_authenticator.py` & `openconnect_sso-0.8.1/openconnect_sso/saml_authenticator.py`

 * *Files identical despite different names*

### Comparing `openconnect-sso-0.7.3/pyproject.toml` & `openconnect_sso-0.8.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openconnect-sso"
-version = "0.7.3"
+version = "0.8.1"
 description = "Wrapper script for OpenConnect supporting Azure AD (SAMLv2) authentication to Cisco SSL-VPNs"
 license = "GPL-3.0-only"
 authors = ["László Vaskó <laszlo.vasko@outlook.com>"]
 readme = "README.md"
 homepage = "https://github.com/vlaci/openconnect-sso"
 repository = "https://github.com/vlaci/openconnect-sso"
 
@@ -16,43 +16,38 @@
     "Topic :: System :: Networking",
 ]
 
 [tool.poetry.scripts]
 openconnect-sso = "openconnect_sso.cli:main"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.8"
 attrs = ">=18.2"
 colorama = "^0.4"
 importlib-metadata = { version = "^3.10.0", python = "<3.8" }
 lxml = "^4.3"
 keyring = ">=21.1, <24.0.0"
 prompt-toolkit = "^3.0.3"
-pyxdg = ">=0.26, <0.28"
+pyxdg = ">=0.26, <0.29"
 requests = "^2.22"
-structlog = ">=20.1, <21.2.0"
+structlog = ">=20.1"
 toml = "^0.10"
 setuptools = ">40.0"
-
-PyQt5 = { version = "^5.12", optional = true }
-PyQtWebEngine = { version ="^5.12", optional = true }
 PySocks = "^1.7.1"
-
-[tool.poetry.extras]
-full = [ "PyQt5", "PyQtWebEngine" ]
+PyQt6 = "^6.3.0"
+PyQt6-WebEngine = "^6.3.0"
+pyotp = "^2.7.0"
 
 [tool.poetry.dev-dependencies]
 coverage_enable_subprocess = "^1.0"
-pytest = "^3.0"
-black = "=19.3b0"
-pytest-asyncio = "^0.10.0"
-pytest-cov = "^2.7"
+pytest = "^7.2"
+black = "=22.10"
+pytest-asyncio = "^0.20.1"
+pytest-cov = "^4.0"
 pytest-httpserver = "^1.0"
-# Fix installation of zipp dependency of importlib-metadata
-setuptools-scm = { version ="^3.4", extras = ["toml"] }
 
 [tool.black]
 target-version = ['py36', 'py37', 'py38']
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `openconnect-sso-0.7.3/setup.py` & `openconnect_sso-0.8.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,233 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: openconnect-sso
+Version: 0.8.1
+Summary: Wrapper script for OpenConnect supporting Azure AD (SAMLv2) authentication to Cisco SSL-VPNs
+Home-page: https://github.com/vlaci/openconnect-sso
+License: GPL-3.0-only
+Author: László Vaskó
+Author-email: laszlo.vasko@outlook.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: X11 Applications :: Qt
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Networking
+Requires-Dist: PyQt6 (>=6.3.0,<7.0.0)
+Requires-Dist: PyQt6-WebEngine (>=6.3.0,<7.0.0)
+Requires-Dist: PySocks (>=1.7.1,<2.0.0)
+Requires-Dist: attrs (>=18.2)
+Requires-Dist: colorama (>=0.4,<0.5)
+Requires-Dist: importlib-metadata (>=3.10.0,<4.0.0) ; python_version < "3.8"
+Requires-Dist: keyring (>=21.1,<24.0.0)
+Requires-Dist: lxml (>=4.3,<5.0)
+Requires-Dist: prompt-toolkit (>=3.0.3,<4.0.0)
+Requires-Dist: pyotp (>=2.7.0,<3.0.0)
+Requires-Dist: pyxdg (>=0.26,<0.29)
+Requires-Dist: requests (>=2.22,<3.0)
+Requires-Dist: setuptools (>40.0)
+Requires-Dist: structlog (>=20.1)
+Requires-Dist: toml (>=0.10,<0.11)
+Project-URL: Repository, https://github.com/vlaci/openconnect-sso
+Description-Content-Type: text/markdown
+
+# openconnect-sso
+
+Wrapper script for OpenConnect supporting Azure AD (SAMLv2) authentication
+to Cisco SSL-VPNs
+
+[![Tests Status
+](https://github.com/vlaci/openconnect-sso/workflows/Tests/badge.svg?branch=master&event=push)](https://github.com/vlaci/openconnect-sso/actions?query=workflow%3ATests+branch%3Amaster+event%3Apush)
+
+## Installation
+
+### Using pip/pipx
+
+A generic way that works on most 'standard' Linux distributions out of the box.
+The following example shows how to install `openconect-sso` along with its
+dependencies including Qt:
+
+```shell
+$ pip install --user pipx
+Successfully installed pipx
+$ pipx install "openconnect-sso[full]"
+⣾ installing openconnect-sso
+  installed package openconnect-sso 0.4.0, Python 3.7.5
+  These apps are now globally available
+    - openconnect-sso
+⚠️  Note: '/home/vlaci/.local/bin' is not on your PATH environment variable.
+These apps will not be globally accessible until your PATH is updated. Run
+`pipx ensurepath` to automatically add it, or manually modify your PATH in your
+shell's config file (i.e. ~/.bashrc).
+done! ✨ 🌟 ✨
+Successfully installed openconnect-sso
+$ pipx ensurepath
+Success! Added /home/vlaci/.local/bin to the PATH environment variable.
+Consider adding shell completions for pipx. Run 'pipx completions' for
+instructions.
+
+You likely need to open a new terminal or re-login for the changes to take
+effect. ✨ 🌟 ✨
+```
+
+Of course you can also install via `pip` instead of `pipx` if you'd like to
+install system-wide or a virtualenv of your choice.
+
+### On Arch Linux
+
+There is an unofficial package available for Arch Linux on
+[AUR](https://aur.archlinux.org/packages/openconnect-sso/). You can use your
+favorite AUR helper to install it:
+
+``` shell
+yay -S openconnect-sso
+```
+
+### Using nix
+
+The easiest method to try is by installing directly:
+
+```shell
+$ nix-env -i -f https://github.com/vlaci/openconnect-sso/archive/master.tar.gz
+unpacking 'https://github.com/vlaci/openconnect-sso/archive/master.tar.gz'...
+[...]
+installing 'openconnect-sso-0.4.0'
+these derivations will be built:
+  /nix/store/2z47740z1rr2cfqfin5lnq04sq3c5xjg-openconnect-sso-0.4.0.drv
+[...]
+building '/nix/store/50q496iqf840wi8b95cfmgn07k6y5b59-user-environment.drv'...
+created 606 symlinks in user environment
+$ openconnect-sso
+```
+
+An overlay is also available to use in nix expressions:
+
+``` nix
+let
+  openconnectOverlay = import "${builtins.fetchTarball https://github.com/vlaci/openconnect-sso/archive/master.tar.gz}/overlay.nix";
+  pkgs = import <nixpkgs> { overlays = [ openconnectOverlay ]; };
+in
+  #  pkgs.openconnect-sso is available in this context
+```
+
+... or to use in `configuration.nix`:
+
+``` nix
+{ config, ... }:
+
+{
+  nixpkgs.overlays = [
+    (import "${builtins.fetchTarball https://github.com/vlaci/openconnect-sso/archive/master.tar.gz}/overlay.nix")
+  ];
+}
+```
 
-packages = \
-['openconnect_sso', 'openconnect_sso.browser']
+### Windows *(EXPERIMENTAL)*
 
-package_data = \
-{'': ['*']}
+Install with [pip/pipx](#using-pippipx) and be sure that you have `sudo` and `openconnect`
+executable commands in your PATH.
 
-install_requires = \
-['PySocks>=1.7.1,<2.0.0',
- 'attrs>=18.2',
- 'colorama>=0.4,<0.5',
- 'keyring>=21.1,<24.0.0',
- 'lxml>=4.3,<5.0',
- 'prompt-toolkit>=3.0.3,<4.0.0',
- 'pyxdg>=0.26,<0.28',
- 'requests>=2.22,<3.0',
- 'setuptools>40.0',
- 'structlog>=20.1,<21.2.0',
- 'toml>=0.10,<0.11']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=3.10.0,<4.0.0'],
- 'full': ['PyQt5>=5.12,<6.0', 'PyQtWebEngine>=5.12,<6.0']}
-
-entry_points = \
-{'console_scripts': ['openconnect-sso = openconnect_sso.cli:main']}
-
-setup_kwargs = {
-    'name': 'openconnect-sso',
-    'version': '0.7.3',
-    'description': 'Wrapper script for OpenConnect supporting Azure AD (SAMLv2) authentication to Cisco SSL-VPNs',
-    'long_description': '# openconnect-sso\n\nWrapper script for OpenConnect supporting Azure AD (SAMLv2) authentication\nto Cisco SSL-VPNs\n\n[![Tests Status\n](https://github.com/vlaci/openconnect-sso/workflows/Tests/badge.svg?branch=master&event=push)](https://github.com/vlaci/openconnect-sso/actions?query=workflow%3ATests+branch%3Amaster+event%3Apush)\n\n## Installation\n\n### Using pip/pipx\n\nA generic way that works on most \'standard\' Linux distributions out of the box.\nThe following example shows how to install `openconect-sso` along with its\ndependencies including Qt:\n\n```shell\n$ pip install --user pipx\nSuccessfully installed pipx\n$ pipx install "openconnect-sso[full]"\n⣾ installing openconnect-sso\n  installed package openconnect-sso 0.4.0, Python 3.7.5\n  These apps are now globally available\n    - openconnect-sso\n⚠️  Note: \'/home/vlaci/.local/bin\' is not on your PATH environment variable.\nThese apps will not be globally accessible until your PATH is updated. Run\n`pipx ensurepath` to automatically add it, or manually modify your PATH in your\nshell\'s config file (i.e. ~/.bashrc).\ndone! ✨ 🌟 ✨\nSuccessfully installed openconnect-sso\n$ pipx ensurepath\nSuccess! Added /home/vlaci/.local/bin to the PATH environment variable.\nConsider adding shell completions for pipx. Run \'pipx completions\' for\ninstructions.\n\nYou likely need to open a new terminal or re-login for the changes to take\neffect. ✨ 🌟 ✨\n```\n\nIf you have Qt 5.x installed, you can skip the installation of bundled Qt version:\n\n``` bash\npipx install openconnect-sso\n```\n\nOf course you can also install via `pip` instead of `pipx` if you\'d like to\ninstall system-wide or a virtualenv of your choice.\n\n### On Arch Linux\n\nThere is an unofficial package available for Arch Linux on\n[AUR](https://aur.archlinux.org/packages/openconnect-sso/). You can use your\nfavorite AUR helper to install it:\n\n``` shell\nyay -S openconnect-sso\n```\n\n### Using nix\n\nThe easiest method to try is by installing directly:\n\n```shell\n$ nix-env -i -f https://github.com/vlaci/openconnect-sso/archive/master.tar.gz\nunpacking \'https://github.com/vlaci/openconnect-sso/archive/master.tar.gz\'...\n[...]\ninstalling \'openconnect-sso-0.4.0\'\nthese derivations will be built:\n  /nix/store/2z47740z1rr2cfqfin5lnq04sq3c5xjg-openconnect-sso-0.4.0.drv\n[...]\nbuilding \'/nix/store/50q496iqf840wi8b95cfmgn07k6y5b59-user-environment.drv\'...\ncreated 606 symlinks in user environment\n$ openconnect-sso\n```\n\nAn overlay is also available to use in nix expressions:\n\n``` nix\nlet\n  openconnectOverlay = import "${builtins.fetchTarball https://github.com/vlaci/openconnect-sso/archive/master.tar.gz}/overlay.nix";\n  pkgs = import <nixpkgs> { overlays = [ openconnectOverlay ]; };\nin\n  #  pkgs.openconnect-sso is available in this context\n```\n\n... or to use in `configuration.nix`:\n\n``` nix\n{ config, ... }:\n\n{\n  nixpkgs.overlays = [\n    (import "${builtins.fetchTarball https://github.com/vlaci/openconnect-sso/archive/master.tar.gz}/overlay.nix")\n  ];\n}\n```\n\n### Windows *(EXPERIMENTAL)*\n\nInstall with [pip/pipx](#using-pippipx) and be sure that you have `sudo` and `openconnect`\nexecutable commands in your PATH.\n\n## Usage\n\nIf you want to save credentials and get them automatically\ninjected in the web browser:\n\n```shell\n$ openconnect-sso --server vpn.server.com/group --user user@domain.com\nPassword (user@domain.com):\n[info     ] Authenticating to VPN endpoint ...\n```\n\nUser credentials are automatically saved to the users login keyring (if\navailable).\n\nIf you already have Cisco AnyConnect set-up, then `--server` argument is\noptional. Also, the last used `--server` address is saved between sessions so\nthere is no need to always type in the same arguments:\n\n```shell\n$ openconnect-sso\n[info     ] Authenticating to VPN endpoint ...\n```\n\nConfiguration is saved in `$XDG_CONFIG_HOME/openconnect-sso/config.toml`. On\ntypical Linux installations it is located under\n`$HOME/.config/openconnect-sso/config.toml`\n\n## Development\n\n`openconnect-sso` is developed using [Nix](https://nixos.org/nix/). Refer to the\n[Quick Start section of the Nix\nmanual](https://nixos.org/nix/manual/#chap-quick-start) to see how to get it\ninstalled on your machine.\n\nTo get dropped into a development environment, just type `nix-shell`:\n\n```shell\n$ nix-shell\nSourcing python-catch-conflicts-hook.sh\nSourcing python-remove-bin-bytecode-hook.sh\nSourcing pip-build-hook\nUsing pipBuildPhase\nSourcing pip-install-hook\nUsing pipInstallPhase\nSourcing python-imports-check-hook.sh\nUsing pythonImportsCheckPhase\nRun \'make help\' for available commands\n\n[nix-shell]$\n```\n\nTo try an installed version of the package, issue `nix-build`:\n\n```shell\n$ nix build\n[1 built, 0.0 MiB DL]\n\n$ result/bin/openconnect-sso --help\n```\n\nAlternatively you may just [get Poetry](https://python-poetry.org/docs/) and\nstart developing by using the included `Makefile`. Type `make help` to see the\npossible make targets.\n',
-    'author': 'László Vaskó',
-    'author_email': 'laszlo.vasko@outlook.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/vlaci/openconnect-sso',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
-}
+## Usage
+
+If you want to save credentials and get them automatically
+injected in the web browser:
+
+```shell
+$ openconnect-sso --server vpn.server.com/group --user user@domain.com
+Password (user@domain.com):
+[info     ] Authenticating to VPN endpoint ...
+```
+
+User credentials are automatically saved to the users login keyring (if
+available).
+
+If you already have Cisco AnyConnect set-up, then `--server` argument is
+optional. Also, the last used `--server` address is saved between sessions so
+there is no need to always type in the same arguments:
+
+```shell
+$ openconnect-sso
+[info     ] Authenticating to VPN endpoint ...
+```
+
+Configuration is saved in `$XDG_CONFIG_HOME/openconnect-sso/config.toml`. On
+typical Linux installations it is located under
+`$HOME/.config/openconnect-sso/config.toml`
+
+For CISCO-VPN and TOTP the following seems to work by tuning the config.toml
+and removing the default "submit"-action to the following:
+
+```
+[[auto_fill_rules."https://*"]]
+selector = "input[data-report-event=Signin_Submit]"
+action = "click"
+
+[[auto_fill_rules."https://*"]]
+selector = "input[type=tel]"
+fill = "totp"
+```
+
+### Adding custom `openconnect` arguments
+
+Sometimes you need to add custom `openconnect` arguments. One situation can be if you get similar error messages:
+
+```shell
+Failed to read from SSL socket: The transmitted packet is too large (EMSGSIZE).
+Failed to recv DPD request (-5)
+```
+
+or:
+
+```shell
+Detected MTU of 1370 bytes (was 1406)
+```
+
+Generally, you can add `openconnect` arguments after the `--` separator. This is called _"positional arguments"_. The
+solution of the previous errors is setting `--base-mtu` e.g.:
+
+```shell
+openconnect-sso --server vpn.server.com/group --user user@domain.com -- --base-mtu=1370
+#                                                          separator ^^|^^^^^^^^^^^^^^^ openconnect args
+```
+
+## Development
+
+`openconnect-sso` is developed using [Nix](https://nixos.org/nix/). Refer to the
+[Quick Start section of the Nix
+manual](https://nixos.org/nix/manual/#chap-quick-start) to see how to get it
+installed on your machine.
+
+To get dropped into a development environment, just type `nix-shell`:
+
+```shell
+$ nix-shell
+Sourcing python-catch-conflicts-hook.sh
+Sourcing python-remove-bin-bytecode-hook.sh
+Sourcing pip-build-hook
+Using pipBuildPhase
+Sourcing pip-install-hook
+Using pipInstallPhase
+Sourcing python-imports-check-hook.sh
+Using pythonImportsCheckPhase
+Run 'make help' for available commands
+
+[nix-shell]$
+```
+
+To try an installed version of the package, issue `nix-build`:
+
+```shell
+$ nix build
+[1 built, 0.0 MiB DL]
+
+$ result/bin/openconnect-sso --help
+```
 
+Alternatively you may just [get Poetry](https://python-poetry.org/docs/) and
+start developing by using the included `Makefile`. Type `make help` to see the
+possible make targets.
 
-setup(**setup_kwargs)
```

