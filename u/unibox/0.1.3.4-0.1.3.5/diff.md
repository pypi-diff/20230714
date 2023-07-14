# Comparing `tmp/unibox-0.1.3.4.tar.gz` & `tmp/unibox-0.1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unibox-0.1.3.4.tar", max compression
+gzip compressed data, was "unibox-0.1.3.5.tar", max compression
```

## Comparing `unibox-0.1.3.4.tar` & `unibox-0.1.3.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-07-10 23:45:04.957926 unibox-0.1.3.4/LICENSE
--rw-r--r--   0        0        0      546 2023-07-10 23:45:04.957926 unibox-0.1.3.4/README.md
--rw-r--r--   0        0        0      444 2023-07-10 23:45:04.957926 unibox-0.1.3.4/pyproject.toml
--rw-r--r--   0        0        0       76 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/__init__.py
--rw-r--r--   0        0        0     1586 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/cli.py
--rw-r--r--   0        0        0        0 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/processing/__init__.py
--rw-r--r--   0        0        0     5896 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/processing/image_resizer.py
--rw-r--r--   0        0        0        0 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/utils/__init__.py
--rw-r--r--   0        0        0     2743 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/utils/data_loader.py
--rw-r--r--   0        0        0     3423 2023-07-10 23:45:04.957926 unibox-0.1.3.4/unibox/utils/logger.py
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 unibox-0.1.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-14 01:40:44.793897 unibox-0.1.3.5/LICENSE
+-rw-r--r--   0        0        0      546 2023-07-14 01:40:44.793897 unibox-0.1.3.5/README.md
+-rw-r--r--   0        0        0      464 2023-07-14 01:40:44.793897 unibox-0.1.3.5/pyproject.toml
+-rw-r--r--   0        0        0       76 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/__init__.py
+-rw-r--r--   0        0        0     3095 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/cli.py
+-rw-r--r--   0        0        0        0 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/processing/__init__.py
+-rw-r--r--   0        0        0     2095 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/processing/file_mover.py
+-rw-r--r--   0        0        0     6268 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/processing/image_resizer.py
+-rw-r--r--   0        0        0        0 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/utils/__init__.py
+-rw-r--r--   0        0        0     2787 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/utils/data_loader.py
+-rw-r--r--   0        0        0     3759 2023-07-14 01:40:44.793897 unibox-0.1.3.5/unibox/utils/logger.py
+-rw-r--r--   0        0        0     1233 1970-01-01 00:00:00.000000 unibox-0.1.3.5/PKG-INFO
```

### Comparing `unibox-0.1.3.4/LICENSE` & `unibox-0.1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unibox-0.1.3.4/README.md` & `unibox-0.1.3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# unibox
+# Unibox
 
-unibox is a tool that aims to provide a unified interface for various common daily operations.
+Unibox is a tool that aims to provide a unified interface for various common daily operations.
 
 ## Features
 
 **CLI**:
 - `unibox resize <dir>`: resizes a directory of images using either `pillow` or `libvips`
 
 **utils**:
```

### Comparing `unibox-0.1.3.4/unibox/cli.py` & `unibox-0.1.3.5/unibox/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import click
 
 from .processing import image_resizer
+from .processing import file_mover
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -22,34 +23,62 @@
 
 @cli.command()
 @click.argument('src_dir')
 @click.option('--min_side', '-m', default=None, type=int, help='Minimum side length of the image.')
 @click.option('--dst_dir', '-d', default=None, help='Destination directory for the images.')
 @click.option('--format', '-f', default=None, help='Format of the image.')
 @click.option('--quality', '-q', default=None, type=int, help='Quality of the image.')
-def resize(src_dir, min_side, dst_dir, format, quality):
+@click.option('--exist_ok', '-e', default=None, type=bool, help='Keep existing images')
+def resize(src_dir, min_side, dst_dir, format, quality, exist_ok):
+
     # resize implementation
     print(f'Resizing directory: {src_dir}')
 
     if not min_side:
         min_side = click.prompt('- Minimum side length', type=int, default=768)
     if not format:
         format = click.prompt('- File format', default="webp")
     if not dst_dir:
         src_dir_name = os.path.basename(os.path.abspath(src_dir))
         dst_dir = click.prompt('- Destination', default=f"{src_dir_name}_{min_side}_{format}")
     if not quality:
         quality = click.prompt('- Image quality', type=int, default=95)
+    if not exist_ok:
+        exist_ok = click.prompt('- Keep existing images', type=bool, default=True)
 
     # Printing the command
     print("\nRunning Command:\n")
-    print(f"unibox resize {src_dir} --min_side {min_side} --dst_dir {dst_dir} --format {format} --quality {quality}\n")
+    print(f"unibox resize {src_dir} --min_side {min_side} --dst_dir {dst_dir} "
+          f"--format {format} --quality {quality} --exist_ok {exist_ok}\n")
 
-    resizer = image_resizer.ImageResizer(src_dir, dst_dir, min_side, format=format, quality=quality)
+    resizer = image_resizer.ImageResizer(src_dir, dst_dir, min_side, format=format, quality=quality, exist_ok=exist_ok)
     resizer.resize_images()
 
 
 
+@cli.command()
+@click.argument('src_dir')
+@click.argument('dst_dir')
+@click.option('--keep_structure', '-k', default=False, type=bool, help='Keep directory structure.')
+@click.option('--include', '-i', default=None, multiple=True, help='File extensions to include.')
+@click.option('--exclude', '-e', default=None, multiple=True, help='File extensions to exclude.')
+def move(src_dir, dst_dir, keep_structure, include, exclude):
+    mover = file_mover.DirMoverCopier(src_dir, dst_dir, keep_structure, include, exclude, 'move')
+    mover.process_files()
+    print(f'Moved files from {src_dir} to {dst_dir}')
+
+@cli.command()
+@click.argument('src_dir')
+@click.argument('dst_dir')
+@click.option('--keep_structure', '-k', default=False, type=bool, help='Keep directory structure.')
+@click.option('--include', '-i', default=None, multiple=True, help='File extensions to include.')
+@click.option('--exclude', '-e', default=None, multiple=True, help='File extensions to exclude.')
+def copy(src_dir, dst_dir, keep_structure, include, exclude):
+    copier = file_mover.DirMoverCopier(src_dir, dst_dir, keep_structure, include, exclude, 'copy')
+    copier.process_files()
+    print(f'Copied files from {src_dir} to {dst_dir}')
+
+
 cli.add_command(setup)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `unibox-0.1.3.4/unibox/processing/image_resizer.py` & `unibox-0.1.3.5/unibox/processing/image_resizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,24 +16,27 @@
     HAS_PYVIPS = False
 except pyvips.error.Error:
     HAS_PYVIPS = False
 
 SUPPORTED_FORMATS = {"jpg", "webp", "png"}
 
 
+# Updated ImageResizer class
+
 class ImageResizer:
-    def __init__(self, src_dir: str, dst_dir: str, min_side: int = 768, format: str = "webp", quality: int = 95):
+    def __init__(self, src_dir: str, dst_dir: str, min_side: int = 768, format: str = "webp", quality: int = 95, exist_ok: bool = False):
         """
         Initialize an instance of ImageResizer.
         """
         self.src_dir = Path(src_dir)
         self.dst_dir = Path(dst_dir)
         self.min_side = min_side
         self.format = self._validate_format(format)
         self.quality = quality
+        self.exist_ok = exist_ok
         self.num_processes = multiprocessing.cpu_count()
 
     def _validate_format(self, format: str) -> str:
         """
         Validate the provided image format.
         """
         if format not in SUPPORTED_FORMATS:
@@ -101,14 +104,15 @@
             return None
 
         scale = self.min_side / min_dim
         return image.resize(scale)
 
     def _task(self, file_path, relative_path):
         self._resize_image(file_path, relative_path)
+
     def _save_image(self, image, dst_path: Path):
         """
         Save an image in the specified format.
         """
         save_methods = {
             "jpg": {"pil": "JPEG", "pyvips": "jpegsave", "params": {"Q": self.quality}},
             "webp": {"pil": "WEBP", "pyvips": "webpsave", "params": {"Q": self.quality}},
@@ -120,15 +124,14 @@
             if HAS_PYVIPS:
                 getattr(image, method_map["pyvips"])(str(dst_path), **method_map["params"])
             else:
                 image.save(dst_path, method_map["pil"], **method_map["params"])
         except Exception as e:
             print(f"Error saving image {dst_path}. Skipping...\n{str(e)}")
 
-
     def _execute_resize(self, tasks):
         """
         Execute tasks using ProcessPoolExecutor
         """
         with concurrent.futures.ProcessPoolExecutor(max_workers=self.num_processes) as executor:
             futures = [executor.submit(task, *args) for task, *args in tasks]
             list(tqdm(concurrent.futures.as_completed(futures), total=len(tasks),
@@ -141,37 +144,42 @@
         tasks = []
 
         self._print_debug_string()
 
         for file_path in self.src_dir.rglob("*"):
             if file_path.is_file() and file_path.suffix[1:].lower() in SUPPORTED_FORMATS:
                 relative_path = file_path.relative_to(self.src_dir)
-                tasks.append((self._task, file_path, relative_path))
+                dst_path = self.dst_dir / relative_path.with_suffix(f".{self.format}")
+
+                # Check if the destination file exists and exist_ok is True
+                if not self.exist_ok or not dst_path.exists():
+                    tasks.append((self._task, file_path, relative_path))
 
         self._execute_resize(tasks)
 
     def _print_debug_string(self):
         """
         prints debug message once resize_images is called
         """
         debug_string = ""
         if HAS_PYVIPS:
             debug_string += "Resizing with libvips: "
         else:
             debug_string += "Resizing with PIL: "
         debug_string += f"num_processes = {self.num_processes}, src_dir={self.src_dir}, dst_dir={self.dst_dir}, " \
-                        f"min_side={self.min_side}, format={self.format}, quality={self.quality}"
+                        f"min_side={self.min_side}, format={self.format}, quality={self.quality}," \
+                        f"exist_ok={self.exist_ok}"
         print(debug_string)
 
 
 if __name__ == "__main__":
     # Define the source and destination directories and the minimum side length for resizing
     src_dir = input("dir path:")
 
     dst_dir = f"{src_dir}_768webp"
     min_side = 64
 
     # Create an instance of the ImageResizer class
     resizer = ImageResizer(src_dir, dst_dir, min_side)
 
     # Get a list of image files from the source directory
-    resizer.resize_images()
+    resizer.resize_images()
```

### Comparing `unibox-0.1.3.4/unibox/utils/data_loader.py` & `unibox-0.1.3.5/unibox/utils/data_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,17 @@
     def load_toml(self, toml_path: Path, encoding="utf-8"):
         return self._load_data(toml_path, tomli.load, encoding)
 
     def load_yaml(self, yaml_path: Path, encoding="utf-8"):
         return self._load_data(yaml_path, lambda f: OmegaConf.load(f), encoding)
 
 
+
+# todo: implement unibox.loads() function
+
 if __name__ == "__main__":
     # Usage example
     logger = UniLogger("logs", file_suffix="data_loader")
     data_loader = UniLoader(logger)
     json_data = data_loader.load_json(Path("example.json"))
     txt_data = data_loader.load_txt(Path("example.txt"))
     csv_data = data_loader.load_csv(Path("example.csv"))
```

### Comparing `unibox-0.1.3.4/unibox/utils/logger.py` & `unibox-0.1.3.5/unibox/utils/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import logging
 import os
-from pathlib import Path
 import inspect
+import logging
+import colorlog
+
+from pathlib import Path
 from datetime import datetime
 
 NOTICE = 25  # Value between WARNING (30) and INFO (20)
 
 
 class UniLogger:
     """包含时间和 caller frame的 logger utils
@@ -24,55 +26,63 @@
         logging.basicConfig(level=logging.INFO,
                             format='%(asctime)s [%(levelname)s] %(message)s',
                             datefmt='%Y-%m-%d %H:%M:%S')
         self.logger = logging.getLogger(__name__)
     """
 
     def __init__(self, output_dir: str = "logs", file_suffix: str = "log", verbose: bool = True, logger_name: str = None):
-
+        """
+        The rest of your __init__ method...
+        """
         self.output_dir = Path(output_dir)
         self.log_file_suffix = file_suffix
         self.verbose = verbose
 
         self.output_dir.mkdir(parents=True, exist_ok=True)
         self.log_file = (
                 self.output_dir
                 / f"{self.log_file_suffix}_{datetime.now().strftime('%Y%m%d')}.log"
         )
 
-        handlers = [logging.FileHandler(self.log_file, mode="a", encoding="utf-8")]
+        # Create a color handler
+        color_handler = colorlog.StreamHandler()
+        color_handler.setFormatter(
+            colorlog.ColoredFormatter(
+                fmt='%(log_color)s%(asctime)s [%(levelname)s] %(name)s: %(message)s',
+                datefmt='%Y-%m-%d %H:%M:%S',
+                log_colors={
+                    'DEBUG': 'cyan',
+                    'INFO': 'green',
+                    'WARNING': 'yellow',
+                    'ERROR': 'red',
+                    'CRITICAL': 'red,bg_white',
+                },
+            )
+        )
+
+        handlers = [logging.FileHandler(self.log_file, mode="a", encoding="utf-8"), color_handler]
 
         if verbose:
-            handlers.append(logging.StreamHandler())
             log_level = logging.DEBUG
         else:
             log_level = logging.INFO
 
         self.logger = logging.getLogger(logger_name if logger_name else self.__class__.__name__)
         self.logger.setLevel(log_level)
 
         # Check if handlers already exist before adding them; prevents duplicate handlers in Jupyter notebooks
-        if not self.logger.handlers:
-            handlers = [logging.FileHandler(self.log_file, mode="a", encoding="utf-8")]
-
-            if verbose:
-                handlers.append(logging.StreamHandler())
-
+        if not self.logger.hasHandlers():
             formatter = logging.Formatter("%(asctime)s [%(levelname)s] %(name)s: %(message)s")
             for handler in handlers:
                 handler.setFormatter(formatter)
                 self.logger.addHandler(handler)
 
-        formatter = logging.Formatter("%(asctime)s [%(levelname)s] %(name)s: %(message)s")
-        for handler in handlers:
-            handler.setFormatter(formatter)
-            self.logger.addHandler(handler)
-
         logging.addLevelName(NOTICE, "NOTICE")
 
+
     def log(self, log_level: str, message: str):
         level = getattr(logging, log_level.upper(), logging.INFO)
 
         # Get the caller function information
         caller_frame = inspect.currentframe().f_back.f_back  # Skip 'log' function frame
         caller_func_name = caller_frame.f_code.co_name
 
@@ -87,18 +97,21 @@
             full_message = f"{caller_class_name}.{caller_func_name}: {message}"
         else:
             full_message = f"{caller_func_name}: {message}"
 
         self.logger.log(level, full_message)
 
     def notice(self, message: str):
-        self.log("NOTICE", message)
+        """
+        using INFO log level but with a checkmark √
+        """
+        self.log("NOTICE", "✅ " + message)
 
     def warning(self, message: str):
-        self.log("WARNING", message)
+        self.log("WARNING", "⚠️ " + message)
 
     def error(self, message: str):
-        self.log("ERROR", message)
+        self.log("ERROR", "❌ " + message)
 
     def info(self, message: str):
         self.log("INFO", message)
```

### Comparing `unibox-0.1.3.4/PKG-INFO` & `unibox-0.1.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: unibox
-Version: 0.1.3.4
+Version: 0.1.3.5
 Summary: one toolbox to rule'em all
 License: GPL-3.0
 Author: yada
 Author-email: trojblue@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.4,<9.0.0)
+Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
-# unibox
+# Unibox
 
-unibox is a tool that aims to provide a unified interface for various common daily operations.
+Unibox is a tool that aims to provide a unified interface for various common daily operations.
 
 ## Features
 
 **CLI**:
 - `unibox resize <dir>`: resizes a directory of images using either `pillow` or `libvips`
 
 **utils**:
```

