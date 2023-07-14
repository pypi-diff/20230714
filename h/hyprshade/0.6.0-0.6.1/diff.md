# Comparing `tmp/hyprshade-0.6.0.tar.gz` & `tmp/hyprshade-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprshade-0.6.0.tar", max compression
+gzip compressed data, was "hyprshade-0.6.1.tar", max compression
```

## Comparing `hyprshade-0.6.0.tar` & `hyprshade-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1065 2023-07-13 17:26:18.998108 hyprshade-0.6.0/LICENSE
--rw-r--r--   0        0        0     2440 2023-07-13 17:26:18.998108 hyprshade-0.6.0/README.md
--rw-r--r--   0        0        0      125 2023-07-13 17:26:18.998108 hyprshade-0.6.0/examples/config.toml
--rw-r--r--   0        0        0        0 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/__init__.py
--rw-r--r--   0        0        0       92 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/__main__.py
--rw-r--r--   0        0        0     2484 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/cli.py
--rw-r--r--   0        0        0     3709 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/config.py
--rw-r--r--   0        0        0      483 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/constants.py
--rw-r--r--   0        0        0      643 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/helpers.py
--rw-r--r--   0        0        0      803 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/hyprctl.py
--rw-r--r--   0        0        0      812 2023-07-13 17:26:18.998108 hyprshade-0.6.0/hyprshade/utils.py
--rw-r--r--   0        0        0     1036 2023-07-13 17:26:18.998108 hyprshade-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1986 2023-07-13 17:26:18.998108 hyprshade-0.6.0/shaders/blue-light-filter.glsl
--rw-r--r--   0        0        0     1276 2023-07-13 17:26:18.998108 hyprshade-0.6.0/shaders/vibrance.glsl
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 hyprshade-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-14 05:53:08.754014 hyprshade-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2440 2023-07-14 05:53:08.754014 hyprshade-0.6.1/README.md
+-rw-r--r--   0        0        0      125 2023-07-14 05:53:08.754014 hyprshade-0.6.1/examples/config.toml
+-rw-r--r--   0        0        0        0 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/__main__.py
+-rw-r--r--   0        0        0     2466 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/cli.py
+-rw-r--r--   0        0        0     3709 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/config.py
+-rw-r--r--   0        0        0      483 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/constants.py
+-rw-r--r--   0        0        0      643 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/helpers.py
+-rw-r--r--   0        0        0      803 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/hyprctl.py
+-rw-r--r--   0        0        0      812 2023-07-14 05:53:08.754014 hyprshade-0.6.1/hyprshade/utils.py
+-rw-r--r--   0        0        0     1036 2023-07-14 05:53:08.754014 hyprshade-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1986 2023-07-14 05:53:08.754014 hyprshade-0.6.1/shaders/blue-light-filter.glsl
+-rw-r--r--   0        0        0     1276 2023-07-14 05:53:08.754014 hyprshade-0.6.1/shaders/vibrance.glsl
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 hyprshade-0.6.1/PKG-INFO
```

### Comparing `hyprshade-0.6.0/LICENSE` & `hyprshade-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.0/README.md` & `hyprshade-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.0/hyprshade/cli.py` & `hyprshade-0.6.1/hyprshade/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,30 +41,30 @@
     return on(shader_name_or_path)
 
 
 @app.command()
 def auto() -> int:
     """Turn on/off screen shader based on schedule"""
 
-    from hyprshade.config import Config
+    from .config import Config
 
     t = datetime.now().time()
     schedule = Config().to_schedule()
     shade = schedule.find_shade(t)
 
     if shade is not None:
         return on(shade)
     return off()
 
 
 @app.command()
 def install() -> int:
     """Instal systemd user units"""
 
-    from hyprshade.config import Config
+    from .config import Config
 
     schedule = Config().to_schedule()
 
     with open(path.join(systemd_user_config_home(), "hyprshade.service"), "w") as f:
         f.write(
             """[Unit]
 Description=Apply screen filter
```

### Comparing `hyprshade-0.6.0/hyprshade/config.py` & `hyprshade-0.6.1/hyprshade/config.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.0/hyprshade/helpers.py` & `hyprshade-0.6.1/hyprshade/helpers.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.0/hyprshade/hyprctl.py` & `hyprshade-0.6.1/hyprshade/hyprctl.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 def get_screen_shader() -> str | None:
     try:
         o = json.load(os.popen("hyprctl -j getoption decoration:screen_shader"))
     except JSONDecodeError as e:
         raise RuntimeError("Failed to parse JSON returned by hyprctl") from e
 
     shader = str(o["str"]).strip()
+    if shader == EMPTY_STR:
+        return None
     if not path.isfile(shader):
         raise RuntimeError(f"Got shader {shader} from hyprctl, which does not exist")
 
-    if shader == EMPTY_STR:
-        return None
     return shader
```

### Comparing `hyprshade-0.6.0/hyprshade/utils.py` & `hyprshade-0.6.1/hyprshade/utils.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.0/pyproject.toml` & `hyprshade-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyprshade"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 authors = ["John Bernard <loqusion@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyprshade" }]
 include = ["examples", "shaders"]
```

### Comparing `hyprshade-0.6.0/shaders/blue-light-filter.glsl` & `hyprshade-0.6.1/shaders/blue-light-filter.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.0/shaders/vibrance.glsl` & `hyprshade-0.6.1/shaders/vibrance.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.0/PKG-INFO` & `hyprshade-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyprshade
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 License: MIT
 Author: John Bernard
 Author-email: loqusion@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

