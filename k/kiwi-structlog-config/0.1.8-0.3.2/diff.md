# Comparing `tmp/kiwi-structlog-config-0.1.8.tar.gz` & `tmp/kiwi-structlog-config-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kiwi-structlog-config-0.1.8.tar", last modified: Wed Jan 15 14:54:58 2020, max compression
+gzip compressed data, was "dist/kiwi-structlog-config-0.3.2.tar", last modified: Thu Jul 13 22:01:46 2023, max compression
```

## Comparing `kiwi-structlog-config-0.1.8.tar` & `kiwi-structlog-config-0.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 pavel     (1000) pavel     (1000)        0 2020-01-15 14:54:58.000000 kiwi-structlog-config-0.1.8/
--rw-r--r--   0 pavel     (1000) pavel     (1000)       64 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/MANIFEST.in
--rw-r--r--   0 pavel     (1000) pavel     (1000)      473 2020-01-15 14:54:58.000000 kiwi-structlog-config-0.1.8/PKG-INFO
--rw-r--r--   0 pavel     (1000) pavel     (1000)      323 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/README.md
-drwxr-xr-x   0 pavel     (1000) pavel     (1000)        0 2020-01-15 14:54:58.000000 kiwi-structlog-config-0.1.8/docs/
--rw-r--r--   0 pavel     (1000) pavel     (1000)      610 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/docs/Makefile
--rw-r--r--   0 pavel     (1000) pavel     (1000)     4876 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/docs/conf.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)      457 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/docs/index.rst
-drwxr-xr-x   0 pavel     (1000) pavel     (1000)        0 2020-01-15 14:54:58.000000 kiwi-structlog-config-0.1.8/kiwi_structlog_config.egg-info/
--rw-r--r--   0 pavel     (1000) pavel     (1000)      473 2020-01-15 14:54:57.000000 kiwi-structlog-config-0.1.8/kiwi_structlog_config.egg-info/PKG-INFO
--rw-r--r--   0 pavel     (1000) pavel     (1000)      541 2020-01-15 14:54:58.000000 kiwi-structlog-config-0.1.8/kiwi_structlog_config.egg-info/SOURCES.txt
--rw-r--r--   0 pavel     (1000) pavel     (1000)        1 2020-01-15 14:54:57.000000 kiwi-structlog-config-0.1.8/kiwi_structlog_config.egg-info/dependency_links.txt
--rw-r--r--   0 pavel     (1000) pavel     (1000)       30 2020-01-15 14:54:57.000000 kiwi-structlog-config-0.1.8/kiwi_structlog_config.egg-info/requires.txt
--rw-r--r--   0 pavel     (1000) pavel     (1000)        8 2020-01-15 14:54:57.000000 kiwi-structlog-config-0.1.8/kiwi_structlog_config.egg-info/top_level.txt
-drwxr-xr-x   0 pavel     (1000) pavel     (1000)        0 2020-01-15 14:54:58.000000 kiwi-structlog-config-0.1.8/kw/
--rw-r--r--   0 pavel     (1000) pavel     (1000)       56 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/kw/__init__.py
-drwxr-xr-x   0 pavel     (1000) pavel     (1000)        0 2020-01-15 14:54:58.000000 kiwi-structlog-config-0.1.8/kw/structlog_config/
--rw-r--r--   0 pavel     (1000) pavel     (1000)      129 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/kw/structlog_config/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     3588 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/kw/structlog_config/config.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)     1991 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/kw/structlog_config/processors.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)       30 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/requirements.in
--rw-r--r--   0 pavel     (1000) pavel     (1000)       38 2020-01-15 14:54:58.000000 kiwi-structlog-config-0.1.8/setup.cfg
--rw-r--r--   0 pavel     (1000) pavel     (1000)      835 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/setup.py
-drwxr-xr-x   0 pavel     (1000) pavel     (1000)        0 2020-01-15 14:54:58.000000 kiwi-structlog-config-0.1.8/test/
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/test/__init__.py
-drwxr-xr-x   0 pavel     (1000) pavel     (1000)        0 2020-01-15 14:54:58.000000 kiwi-structlog-config-0.1.8/test/integration/
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/test/integration/__init__.py
-drwxr-xr-x   0 pavel     (1000) pavel     (1000)        0 2020-01-15 14:54:58.000000 kiwi-structlog-config-0.1.8/test/unit/
--rw-r--r--   0 pavel     (1000) pavel     (1000)        0 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/test/unit/__init__.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)      554 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/test/unit/test_processors.py
--rw-r--r--   0 pavel     (1000) pavel     (1000)       63 2020-01-15 14:52:53.000000 kiwi-structlog-config-0.1.8/test-requirements.in
+drwxr-xr-x   0 jurica     (501) staff       (20)        0 2023-07-13 22:01:46.620262 kiwi-structlog-config-0.3.2/
+-rw-r--r--   0 jurica     (501) staff       (20)       64 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/MANIFEST.in
+-rw-r--r--   0 jurica     (501) staff       (20)      433 2023-07-13 22:01:46.620091 kiwi-structlog-config-0.3.2/PKG-INFO
+-rw-r--r--   0 jurica     (501) staff       (20)      639 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/README.md
+drwxr-xr-x   0 jurica     (501) staff       (20)        0 2023-07-13 22:01:46.617946 kiwi-structlog-config-0.3.2/docs/
+-rw-r--r--   0 jurica     (501) staff       (20)      610 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/docs/Makefile
+-rw-r--r--   0 jurica     (501) staff       (20)     4948 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/docs/conf.py
+-rw-r--r--   0 jurica     (501) staff       (20)      457 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/docs/index.rst
+drwxr-xr-x   0 jurica     (501) staff       (20)        0 2023-07-13 22:01:46.618682 kiwi-structlog-config-0.3.2/kiwi_structlog_config.egg-info/
+-rw-r--r--   0 jurica     (501) staff       (20)      433 2023-07-13 22:01:46.000000 kiwi-structlog-config-0.3.2/kiwi_structlog_config.egg-info/PKG-INFO
+-rw-r--r--   0 jurica     (501) staff       (20)      541 2023-07-13 22:01:46.000000 kiwi-structlog-config-0.3.2/kiwi_structlog_config.egg-info/SOURCES.txt
+-rw-r--r--   0 jurica     (501) staff       (20)        1 2023-07-13 22:01:46.000000 kiwi-structlog-config-0.3.2/kiwi_structlog_config.egg-info/dependency_links.txt
+-rw-r--r--   0 jurica     (501) staff       (20)       30 2023-07-13 22:01:46.000000 kiwi-structlog-config-0.3.2/kiwi_structlog_config.egg-info/requires.txt
+-rw-r--r--   0 jurica     (501) staff       (20)        8 2023-07-13 22:01:46.000000 kiwi-structlog-config-0.3.2/kiwi_structlog_config.egg-info/top_level.txt
+drwxr-xr-x   0 jurica     (501) staff       (20)        0 2023-07-13 22:01:46.618887 kiwi-structlog-config-0.3.2/kw/
+-rw-r--r--   0 jurica     (501) staff       (20)        0 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/kw/__init__.py
+drwxr-xr-x   0 jurica     (501) staff       (20)        0 2023-07-13 22:01:46.619326 kiwi-structlog-config-0.3.2/kw/structlog_config/
+-rw-r--r--   0 jurica     (501) staff       (20)      168 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/kw/structlog_config/__init__.py
+-rw-r--r--   0 jurica     (501) staff       (20)     3940 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/kw/structlog_config/config.py
+-rw-r--r--   0 jurica     (501) staff       (20)     2679 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/kw/structlog_config/processors.py
+-rw-r--r--   0 jurica     (501) staff       (20)       30 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/requirements.in
+-rw-r--r--   0 jurica     (501) staff       (20)       38 2023-07-13 22:01:46.620315 kiwi-structlog-config-0.3.2/setup.cfg
+-rw-r--r--   0 jurica     (501) staff       (20)      884 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/setup.py
+drwxr-xr-x   0 jurica     (501) staff       (20)        0 2023-07-13 22:01:46.619491 kiwi-structlog-config-0.3.2/test/
+-rw-r--r--   0 jurica     (501) staff       (20)        0 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/test/__init__.py
+drwxr-xr-x   0 jurica     (501) staff       (20)        0 2023-07-13 22:01:46.619609 kiwi-structlog-config-0.3.2/test/integration/
+-rw-r--r--   0 jurica     (501) staff       (20)        0 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/test/integration/__init__.py
+drwxr-xr-x   0 jurica     (501) staff       (20)        0 2023-07-13 22:01:46.619837 kiwi-structlog-config-0.3.2/test/unit/
+-rw-r--r--   0 jurica     (501) staff       (20)        0 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/test/unit/__init__.py
+-rw-r--r--   0 jurica     (501) staff       (20)     1197 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/test/unit/test_processors.py
+-rw-r--r--   0 jurica     (501) staff       (20)       77 2023-03-23 09:29:56.000000 kiwi-structlog-config-0.3.2/test-requirements.in
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kiwi-structlog-config-0.1.8/docs/Makefile` & `kiwi-structlog-config-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kiwi-structlog-config-0.1.8/docs/conf.py` & `kiwi-structlog-config-0.3.2/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,132 +30,137 @@
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.viewcode',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.viewcode",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'structlog_config'
-copyright = u'2017, platform team'
-author = u'platform team'
+project = "structlog_config"
+copyright = "2017, platform team"
+author = "platform team"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = u''
+version = ""
 # The full version, including alpha/beta/rc tags.
-release = u''
+release = ""
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'kw_structlogdoc'
+htmlhelp_basename = "kw_structlogdoc"
 
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'structlog_config.tex', u'structlog_config Documentation',
-     u'platform team', 'manual'),
+    (
+        master_doc,
+        "structlog_config.tex",
+        "structlog_config Documentation",
+        "platform team",
+        "manual",
+    ),
 ]
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'structlog_config', u'structlog_config Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "structlog_config", "structlog_config Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'structlog_config', u'structlog_config Documentation',
-     author, 'structlog_config', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "structlog_config",
+        "structlog_config Documentation",
+        author,
+        "structlog_config",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 # stop ignoring
```

### Comparing `kiwi-structlog-config-0.1.8/kiwi_structlog_config.egg-info/SOURCES.txt` & `kiwi-structlog-config-0.3.2/kiwi_structlog_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiwi-structlog-config-0.1.8/kw/structlog_config/config.py` & `kiwi-structlog-config-0.3.2/kw/structlog_config/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 import logging
 import logging.config
 
 import simplejson
 import structlog
 
 from .processors import (
-    add_structlog_context, drop_debug_logs, numeric_rounder, process_stdlib_logging, datadog_tracer_injection
+    add_structlog_context,
+    datadog_tracer_injection,
+    drop_debug_logs,
+    numeric_rounder,
+    process_stdlib_logging,
 )
 
 # structlog configuration
 PRODUCTION_PROCESSORS = [
     structlog.stdlib.add_log_level,
     drop_debug_logs,
     structlog.stdlib.PositionalArgumentsFormatter(),
@@ -22,40 +26,47 @@
     structlog.processors.UnicodeEncoder(),
 ]
 
 DEBUG_PROCESSORS = [
     structlog.stdlib.add_log_level,
     structlog.stdlib.PositionalArgumentsFormatter(),
     numeric_rounder,
-    structlog.processors.TimeStamper('iso'),
+    structlog.processors.TimeStamper("iso"),
     datadog_tracer_injection,
     structlog.processors.ExceptionPrettyPrinter(),
     structlog.processors.UnicodeDecoder(),
     structlog.dev.ConsoleRenderer(pad_event=25),
 ]
 
 
-def get_structlog_processors(debug=False, json_kwargs=None, timestamp_format=None):
+def get_structlog_processors(debug=False, json_kwargs=None, timestamp_format=None, extra_processors=None):
     """Helper method to get debug/production processors list."""
     json_kwargs = {} if json_kwargs is None else json_kwargs
+    extra_processors = extra_processors or []
 
     if debug:
-        processors = DEBUG_PROCESSORS
+        processors = DEBUG_PROCESSORS + extra_processors
     else:
-        processors = PRODUCTION_PROCESSORS + [
-            structlog.processors.TimeStamper(fmt=timestamp_format), structlog.processors.JSONRenderer(
-                serializer=simplejson.dumps, **json_kwargs
-            )
-        ]
+        processors = (
+            PRODUCTION_PROCESSORS
+            + [
+                structlog.processors.TimeStamper(fmt=timestamp_format),
+            ]
+            + extra_processors
+            + [
+                structlog.processors.JSONRenderer(serializer=simplejson.dumps, **json_kwargs),
+            ]
+        )
+
     return processors
 
 
-def configure_structlog(debug=False, json_kwargs=None, timestamp_format=None):
-    """Configure proper log processors and settings for structlog with regards to debug setting."""
-    processors = get_structlog_processors(debug, json_kwargs, timestamp_format)
+def configure_structlog(debug=False, json_kwargs=None, timestamp_format=None, extra_processors=None):
+    """Configure proper log processors and settings for structlog in regard to debug setting."""
+    processors = get_structlog_processors(debug, json_kwargs, timestamp_format, extra_processors)
     structlog.configure_once(
         processors=processors,
         logger_factory=structlog.PrintLoggerFactory(),
         wrapper_class=structlog.stdlib.BoundLogger,
         context_class=structlog.threadlocal.wrap_dict(dict),
     )
 
@@ -63,46 +74,48 @@
 def configure_stdlib_logging(debug=False, json_kwargs=None, timestamp_format=None, level=None):
     """Configure standard logging to log using the same processors as structlog."""
 
     # Specific processors for stdlib logging
     stdlib_processors = [
         add_structlog_context,  # fill structlog logger attributes (e.g. provided to bind())
         structlog.stdlib.add_logger_name,  # fill `logger` attribute
-        process_stdlib_logging  # fill `message` attribute, set `event`
+        process_stdlib_logging,  # fill `message` attribute, set `event`
     ]
 
     if level is None:
         level = "DEBUG" if debug else "INFO"
 
     # Append structlog processors to chain
     processors = get_structlog_processors(debug, json_kwargs, timestamp_format)
     stdlib_processors.extend(processors)
 
     # The last processor needs to be passed separately
     stdlib_renderer = stdlib_processors.pop(-1)
 
-    logging.config.dictConfig({
-        "version": 1,
-        "disable_existing_loggers": False,
-        "formatters": {
-            "plain": {
-                "()": structlog.stdlib.ProcessorFormatter,
-                "processor": stdlib_renderer,
-                "foreign_pre_chain": stdlib_processors,
+    logging.config.dictConfig(
+        {
+            "version": 1,
+            "disable_existing_loggers": False,
+            "formatters": {
+                "plain": {
+                    "()": structlog.stdlib.ProcessorFormatter,
+                    "processor": stdlib_renderer,
+                    "foreign_pre_chain": stdlib_processors,
+                },
             },
-        },
-        "handlers": {
-            "default": {
-                "level": level,
-                "class": "logging.StreamHandler",
-                "formatter": "plain",
-                "stream": "ext://sys.stdout",
+            "handlers": {
+                "default": {
+                    "level": level,
+                    "class": "logging.StreamHandler",
+                    "formatter": "plain",
+                    "stream": "ext://sys.stdout",
+                },
             },
-        },
-        "loggers": {
-            "": {
-                "handlers": ["default"],
-                "level": level,
-                "propagate": True,
+            "loggers": {
+                "": {
+                    "handlers": ["default"],
+                    "level": level,
+                    "propagate": True,
+                },
             },
         }
-    })
+    )
```

### Comparing `kiwi-structlog-config-0.1.8/kw/structlog_config/processors.py` & `kiwi-structlog-config-0.3.2/kw/structlog_config/processors.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,91 @@
 """Contains ``structlog`` event processors."""
 from __future__ import absolute_import, print_function
 
+import re
 from decimal import Decimal
 from time import time
 
 import structlog
 
 try:
-    from ddtrace.helpers import get_correlation_ids
+    import ddtrace
 except ImportError:
-    get_correlation_ids = None
+    ddtrace = None
 
 
 def numeric_rounder(_, __, event_dict):
     """Round any floats in ``event_dict`` to 3 decimal places."""
     for key, value in event_dict.items():
         if isinstance(value, (float, Decimal)):
             event_dict[key] = round(value, 3)
     return event_dict
 
 
 def drop_debug_logs(_, __, event_dict):
     """Drop event with ``debug`` log level."""
-    if event_dict['level'] == 'debug':
+    if event_dict["level"] == "debug":
         raise structlog.DropEvent
     return event_dict
 
 
 def unix_timestamper(_, __, event_dict):
     """Add curent timestamp to event."""
-    event_dict['timestamp'] = time()
+    event_dict["timestamp"] = time()
     return event_dict
 
 
 def process_stdlib_logging(_, __, event_dict):
     """Move standard logging message to ``message`` field and change ``event`` to desired event name."""
-    event_dict['message'] = event_dict['event']
-    event_dict['event'] = 'stdlib_log'
+    event_dict["message"] = event_dict["event"]
+    event_dict["event"] = "stdlib_log"
     return event_dict
 
 
 def add_structlog_context(_, __, event_dict):
     """Update ``event_dict`` with context of the ``structlog`` logger."""
     event_dict.update(structlog.get_logger()._context._dict)
     return event_dict
 
 
 def datadog_tracer_injection(_, __, event_dict):
     """Propagate trace ids for Datadog."""
-    if get_correlation_ids is None:
-        # Do nothing if ddtrace module is not available.
+    if not ddtrace:
         return event_dict
 
-    # Hack to prevent infinite loop in asyncio event loop creation in debug log-level
-    # https://github.com/DataDog/dd-trace-py/issues/1003
-    if event_dict["level"] == "debug" and event_dict.get('logger') == 'asyncio':
-        return event_dict
+    context = ddtrace.tracer.get_log_correlation_context()
+
+    event_dict["dd.trace_id"] = context["trace_id"]
+    event_dict["dd.span_id"] = context["span_id"]
+    event_dict["dd.env"] = context["env"]
+    event_dict["dd.service"] = context["service"]
+    event_dict["dd.version"] = context["version"]
 
-    trace_id, span_id = get_correlation_ids()
-    if trace_id and span_id:
-        event_dict['dd.trace_id'] = trace_id
-        event_dict['dd.span_id'] = span_id
     return event_dict
+
+
+class Anonymize:
+    r"""Anonymize personal data.
+
+    anonymize = Anonymize(patterns=[
+        ({"visa", "amex"}, r"\d+(\d{4})", "*"*12 + r"\1"),
+        ({"passenger_name"}, r"(\w)\w*", r"\1***"),
+    ])
+    """
+
+    def __init__(self, patterns):
+        self.patterns = self.build_mapping(patterns)
+
+    @classmethod
+    def build_mapping(cls, patterns):
+        """Flatten input in a dict and compile regex patterns."""
+        mapping = {}
+        for keys, pattern, replacement in patterns:
+            regex = re.compile(pattern)
+            mapping.update({key: (regex, replacement) for key in keys})
+        return mapping
+
+    def __call__(self, logger, method_name, event_dict):
+        for key in set(event_dict) & set(self.patterns):
+            pattern, replacement = self.patterns[key]
+            event_dict[key] = re.sub(pattern, replacement, event_dict[key])
+        return event_dict
```

### Comparing `kiwi-structlog-config-0.1.8/setup.py` & `kiwi-structlog-config-0.3.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+from pathlib import Path
 from setuptools import find_packages, setup
 
-with open('requirements.in') as f:
-    REQUIREMENTS = [line for line in f if line and line[0] not in '#-']
+with open("requirements.in") as f:
+    REQUIREMENTS = [line for line in f if line and line[0] not in "#-"]
 
-with open('test-requirements.in') as f:
-    TEST_REQUIREMENTS = [line for line in f if line and line[0] not in '#-']
+with open("test-requirements.in") as f:
+    TEST_REQUIREMENTS = [line for line in f if line and line[0] not in "#-"]
+
+version = Path("VERSION").read_text(encoding="utf-8").strip()
 
 setup(
-    name='kiwi-structlog-config',
-    version='0.1.8',
-    url='https://github.com/kiwicom/kiwi-structlog-config',
-    author='Platform Team',
-    author_email='platform@kiwi.com',
+    name="kiwi-structlog-config",
+    version=version,
+    url="https://github.com/kiwicom/kiwi-structlog-config",
+    author="Booking Backend team",
+    author_email="bookingbe@kiwi.com",
     packages=find_packages(),
     install_requires=REQUIREMENTS,
     tests_require=TEST_REQUIREMENTS,
     include_package_data=True,
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Environment :: Console',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 3',
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
     ],
 )
```

