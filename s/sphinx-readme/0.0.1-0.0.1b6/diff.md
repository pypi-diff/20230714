# Comparing `tmp/sphinx-readme-0.0.1.tar.gz` & `tmp/sphinx-readme-0.0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-readme-0.0.1.tar", last modified: Fri Jul 14 06:48:15 2023, max compression
+gzip compressed data, was "sphinx-readme-0.0.1b6.tar", last modified: Mon Jul 10 13:25:29 2023, max compression
```

## Comparing `sphinx-readme-0.0.1.tar` & `sphinx-readme-0.0.1b6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 06:48:15.666150 sphinx-readme-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     9259 2023-07-14 06:48:15.650527 sphinx-readme-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8470 2023-07-14 06:47:42.000000 sphinx-readme-0.0.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-14 06:48:15.666150 sphinx-readme-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1454 2023-07-14 06:37:22.000000 sphinx-readme-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:48:15.632814 sphinx-readme-0.0.1/sphinx_readme/
--rw-rw-rw-   0        0        0     1710 2023-07-14 06:47:42.000000 sphinx-readme-0.0.1/sphinx_readme/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:48:15.650527 sphinx-readme-0.0.1/sphinx_readme/config/
--rw-rw-rw-   0        0        0       57 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1/sphinx_readme/config/__init__.py
--rw-rw-rw-   0        0        0     8206 2023-07-14 06:00:41.000000 sphinx-readme-0.0.1/sphinx_readme/config/linkcode.py
--rw-rw-rw-   0        0        0    11635 2023-07-14 06:00:41.000000 sphinx-readme-0.0.1/sphinx_readme/config/main.py
--rw-rw-rw-   0        0        0    27832 2023-07-14 06:03:19.000000 sphinx-readme-0.0.1/sphinx_readme/parser.py
--rw-rw-rw-   0        0        0     5107 2023-07-14 06:00:41.000000 sphinx-readme-0.0.1/sphinx_readme/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:48:15.650527 sphinx-readme-0.0.1/sphinx_readme.egg-info/
--rw-rw-rw-   0        0        0     9259 2023-07-14 06:48:15.000000 sphinx-readme-0.0.1/sphinx_readme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-07-14 06:48:15.000000 sphinx-readme-0.0.1/sphinx_readme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 06:48:15.000000 sphinx-readme-0.0.1/sphinx_readme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-14 06:48:15.000000 sphinx-readme-0.0.1/sphinx_readme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-14 06:48:15.000000 sphinx-readme-0.0.1/sphinx_readme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 13:25:29.443000 sphinx-readme-0.0.1b6/
+-rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.0.1b6/LICENSE
+-rw-rw-rw-   0        0        0     9372 2023-07-10 13:25:29.443000 sphinx-readme-0.0.1b6/PKG-INFO
+-rw-rw-rw-   0        0        0     8581 2023-07-10 13:24:24.000000 sphinx-readme-0.0.1b6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-10 13:25:29.443000 sphinx-readme-0.0.1b6/setup.cfg
+-rw-rw-rw-   0        0        0     1454 2023-07-07 16:12:34.000000 sphinx-readme-0.0.1b6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:25:29.396136 sphinx-readme-0.0.1b6/sphinx_readme/
+-rw-rw-rw-   0        0        0     1712 2023-07-10 13:12:35.000000 sphinx-readme-0.0.1b6/sphinx_readme/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:25:29.443000 sphinx-readme-0.0.1b6/sphinx_readme/config/
+-rw-rw-rw-   0        0        0       57 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b6/sphinx_readme/config/__init__.py
+-rw-rw-rw-   0        0        0     7156 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b6/sphinx_readme/config/linkcode.py
+-rw-rw-rw-   0        0        0     9080 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b6/sphinx_readme/config/main.py
+-rw-rw-rw-   0        0        0    20713 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b6/sphinx_readme/parser.py
+-rw-rw-rw-   0        0        0     4878 2023-07-07 16:12:34.000000 sphinx-readme-0.0.1b6/sphinx_readme/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-10 13:25:29.427382 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/
+-rw-rw-rw-   0        0        0     9372 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-10 13:25:29.000000 sphinx-readme-0.0.1b6/sphinx_readme.egg-info/top_level.txt
```

### Comparing `sphinx-readme-0.0.1/LICENSE` & `sphinx-readme-0.0.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1/PKG-INFO` & `sphinx-readme-0.0.1b6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-readme
-Version: 0.0.1
+Version: 0.0.1b6
 Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 Home-page: https://github.com/tdkorn/sphinx-readme
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
 Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
@@ -12,22 +12,22 @@
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
+.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
+.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
+.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
 .. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
 .. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1/sphinx_readme/parser.py#L145-L159
-.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
-.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
-.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b6/sphinx_readme/parser.py#L124-L134
 .. |attention| replace:: 🔔️
 .. |caution| replace:: ⚠️
 .. |danger| replace:: ☢️
 .. |error| replace:: ⛔
 .. |hint| replace:: 🧠
 .. |important| replace:: 📢
 .. |note| replace:: 📝
@@ -37,31 +37,31 @@
 .. |about| replace:: 📚
 
 .. meta::
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
+
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1/docs/source/_static/logo_transparent.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/logo_readme.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
-A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
+A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
 .. |RTD| replace:: **Explore the docs »**
 .. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
 
 |RTD|_
 
-|
 
 .. image:: https://img.shields.io/pypi/v/sphinx-readme?color=eb5202
    :target: https://pypi.org/project/sphinx-readme
    :alt: PyPI Project for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 .. image:: https://img.shields.io/badge/GitHub-sphinx--readme-4f1abc
    :target: https://github.com/tdkorn/sphinx-readme
@@ -71,14 +71,15 @@
    :target: https://pepy.tech/project/sphinx-readme
    :alt: Downloads for Sphinx README
 
 .. image:: https://readthedocs.org/projects/sphinx-readme/badge/?version=latest
    :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
+
 |
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
 .. csv-table::
@@ -86,22 +87,22 @@
 
    "``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
    to generate ``rst`` files that render beautifully on
    GitHub, PyPi, GitLab, and BitBucket."
 
 
 
-**With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
+With ``sphinx_readme``, there's no need to rewrite your ``README.rst`` as a ``README.md`` file
+==============================================================================================
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
-|
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
 
@@ -155,25 +156,25 @@
  * At minimum, the username and repository name must be specified
  * Please see `HTML Context Settings <https://docs.readthedocs.io/en/stable/guides/edit-source-links-sphinx.html>`_
    to determine the correct dictionary keys for your hosting platform
 
 .. |html_context| replace:: ``html_context``
 .. _html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 
-|
+...
 
 |html_baseurl|_
  The base URL which points to the root of the HTML documentation
 
   Type: ``str``
 
 .. |html_baseurl| replace:: ``html_baseurl``
 .. _html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
 
-|
+...
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
 
   Type: ``Union[str, List]``
 
 
@@ -182,15 +183,15 @@
 
    "Filepaths should be specified relative to the source directory"
 
 
 .. |readme_src_files| replace:: ``readme_src_files``
 .. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
 
-|
+...
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
   Type: ``str``
 
  Must be either ``"code"`` or ``"html"``
@@ -250,16 +251,16 @@
 .. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
 
 
 
 .. csv-table::
    :header: |important| Important
 
-   "For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
-   be sure to disable |readme_raw_directive|_:
+   "If generating a ``README`` for a platform that doesn't support ``raw``
+   directives (PyPi, GitLab, and BitBucket), be sure to disable |readme_raw_directive|_:
 
    .. code-block:: python
 
       readme_raw_directive = False"
```

### Comparing `sphinx-readme-0.0.1/README.rst` & `sphinx-readme-0.0.1b6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
+.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
+.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
 .. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
 .. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1/sphinx_readme/parser.py#L145-L159
-.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
-.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
-.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b6/sphinx_readme/parser.py#L124-L134
 .. |attention| replace:: 🔔️
 .. |caution| replace:: ⚠️
 .. |danger| replace:: ☢️
 .. |error| replace:: ⛔
 .. |hint| replace:: 🧠
 .. |important| replace:: 📢
 .. |note| replace:: 📝
@@ -19,31 +19,31 @@
 .. |about| replace:: 📚
 
 .. meta::
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
+
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1/docs/source/_static/logo_transparent.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/logo_readme.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
-A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
+A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
 .. |RTD| replace:: **Explore the docs »**
 .. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
 
 |RTD|_
 
-|
 
 .. image:: https://img.shields.io/pypi/v/sphinx-readme?color=eb5202
    :target: https://pypi.org/project/sphinx-readme
    :alt: PyPI Project for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 .. image:: https://img.shields.io/badge/GitHub-sphinx--readme-4f1abc
    :target: https://github.com/tdkorn/sphinx-readme
@@ -53,14 +53,15 @@
    :target: https://pepy.tech/project/sphinx-readme
    :alt: Downloads for Sphinx README
 
 .. image:: https://readthedocs.org/projects/sphinx-readme/badge/?version=latest
    :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
+
 |
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
 .. csv-table::
@@ -68,22 +69,22 @@
 
    "``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
    to generate ``rst`` files that render beautifully on
    GitHub, PyPi, GitLab, and BitBucket."
 
 
 
-**With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
+With ``sphinx_readme``, there's no need to rewrite your ``README.rst`` as a ``README.md`` file
+==============================================================================================
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
-|
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
 
@@ -137,25 +138,25 @@
  * At minimum, the username and repository name must be specified
  * Please see `HTML Context Settings <https://docs.readthedocs.io/en/stable/guides/edit-source-links-sphinx.html>`_
    to determine the correct dictionary keys for your hosting platform
 
 .. |html_context| replace:: ``html_context``
 .. _html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 
-|
+...
 
 |html_baseurl|_
  The base URL which points to the root of the HTML documentation
 
   Type: ``str``
 
 .. |html_baseurl| replace:: ``html_baseurl``
 .. _html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
 
-|
+...
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
 
   Type: ``Union[str, List]``
 
 
@@ -164,15 +165,15 @@
 
    "Filepaths should be specified relative to the source directory"
 
 
 .. |readme_src_files| replace:: ``readme_src_files``
 .. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
 
-|
+...
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
   Type: ``str``
 
  Must be either ``"code"`` or ``"html"``
@@ -232,16 +233,16 @@
 .. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
 
 
 
 .. csv-table::
    :header: |important| Important
 
-   "For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
-   be sure to disable |readme_raw_directive|_:
+   "If generating a ``README`` for a platform that doesn't support ``raw``
+   directives (PyPi, GitLab, and BitBucket), be sure to disable |readme_raw_directive|_:
 
    .. code-block:: python
 
       readme_raw_directive = False"
```

### Comparing `sphinx-readme-0.0.1/setup.py` & `sphinx-readme-0.0.1b6/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1/sphinx_readme/__init__.py` & `sphinx-readme-0.0.1b6/sphinx_readme/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
 from sphinx_readme.utils import get_conf_val, set_conf_val
 from sphinx_readme.config import get_repo_dir
 from sphinx_readme.parser import READMEParser
 
 
-__version__ = "v0.0.1"
+__version__ = "v0.0.1b6"
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
     # Avoid setting up extension if building on ReadTheDocs
     if os.environ.get("READTHEDOCS") == "True":
         return {}
```

### Comparing `sphinx-readme-0.0.1/sphinx_readme/config/linkcode.py` & `sphinx-readme-0.0.1b6/sphinx_readme/config/linkcode.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,33 +6,22 @@
 import pkg_resources
 from pathlib import Path
 from typing import Dict, Optional, Callable
 from sphinx.errors import ExtensionError
 from sphinx_readme.utils import logger
 
 
-def get_linkcode_url(
-        blob_url: Optional[str] = None,
-        repo_url: Optional[str] = None,
-        context: Optional[Dict] = None,
-        blob: Optional[str] = None
-) -> str:
-    """Generates the template URL for linking to highlighted source code
-
-    Final links are generated from the template by a ``linkcode_resolve()`` function
-
-    .. note:: Only one of ``blob_url``, ``repo_url``, or ``context`` needs to be specified
-
-    :param blob_url: the base URL for a specific blob of a repository
-    :param repo_url: the base URL of a repository
-    :param context: the Sphinx :external+sphinx:confval:`html_context` dict
-    :param blob: the blob of the repository to generate the link for
-    :raises ExtensionError: if none of ``blob_url``, ``repo_url``, or ``context`` are provided
+def get_linkcode_url(blob_url: Optional[str] = None,
+                     repo_url: Optional[str] = None,
+                     context: Optional[Dict] = None,
+                     blob: Optional[str] = None) -> str:
+    """Get the template URL for linking to highlighted GitHub source code
+
+    Formatted into the final link by ``linkcode_resolve()``
     """
-    # """
     if blob_url is None:
         if repo_url is None:
             if context is None:
                 raise ExtensionError(
                     "``sphinx_readme:`` config value ``html_context`` is missing")
             else:
                 repo_url = get_repo_url(context)
@@ -40,21 +29,15 @@
 
     if 'bitbucket' in blob_url:
         return blob_url + "/{filepath}#lines-{linestart}:{linestop}"
     else:
         return blob_url + "/{filepath}#L{linestart}-L{linestop}"
 
 
-def get_repo_url(context: Dict) -> str:
-    """Parses the repository URL from the Sphinx :external+sphinx:confval:`html_context` dict
-
-    :param context: the ``html_context`` dict
-    :return: the base URL of the project's repository
-    :raises ExtensionError: if the repository URL cannot be parsed from ``html_context``
-    """
+def get_repo_url(context: Dict):
     for host in ('github', 'gitlab', 'bitbucket'):
         user = context.get(f"{host}_user")
         repo = context.get(f"{host}_repo")
 
         if not all((user, repo)):
             continue
 
@@ -66,73 +49,64 @@
         return f"https://{host}.{tld}/{user}/{repo}"
 
     raise ExtensionError(
         "``sphinx_readme``: unable to determine repo url")
 
 
 def get_blob_url(repo_url: str, blob: Optional[str] = None, context: Optional[Dict] = None) -> str:
-    """Generates the base URL for a specific blob of a repository
+    """Generate the url for a specific blob of a repository
 
-    :param repo_url: the base URL of the repository
-    :param blob: the blob of the repository to generate the link for
-    :param context: the Sphinx :external+sphinx:confval:`html_context` dict
+    If ``blob`` and ``context`` are not provided, the most recent commit hash will be used
     """
     if context:
         host = get_repo_host(repo_url)
         blob = context.get(f"{host}_version")
 
     if blob is not None:
         # Use blob from kwarg/html_context
-        blob = get_blob(blob)
+        blob = get_linkcode_revision(blob)
     else:
         # Use hash of the most recent commit
-        blob = get_blob('head')
+        blob = get_linkcode_revision('head')
 
     if "bitbucket" in repo_url:
         return repo_url.strip('/') + f"/src/{blob}"
     else:
         return repo_url.strip("/") + f"/blob/{blob}"
 
 
-def get_repo_host(repo_url: str) -> Optional[str]:
-    """Returns the hosting platform of a repository
-
-    >>> get_repo_host("https://github.com/TDKorn/sphinx-readme")
-    'github'
-
-    :param repo_url: the URL of the repository
-    """
-    if match := re.match(r"https?://(\w+)\.(?:com|org)", repo_url):
+def get_repo_host(url: str):
+    if match := re.match(r"https?://(\w+)\.(?:com|org)", url):
         return match.group(1)
     return None
 
 
-def get_blob(blob: str) -> str:
-    """Returns the git blob corresponding to ``blob``
+def get_linkcode_revision(blob: str) -> str:
+    """Get the blob to link to
+
+    .. note::
 
-    The value of ``blob`` can be any of ``"head"``, ``"last_tag"``, or ``"{blob}"``
+       The value of ``blob`` can be any of ``"head"``, ``"last_tag"``, or ``"{blob}"``
 
-    * ``"head"``: returns the hash of the most recent commit; if this commit is tagged, uses the tag instead
-    * ``"last_tag"``: returns the most recent commit tag; if no tags exist, uses ``"head"``
-    * ``"{blob}"``: returns the specified blob as is, for example ``"master"`` or ``"v2.0.1"``
+       * ``head`` (default): links to the most recent commit hash; if this commit is tagged, uses the tag instead
+       * ``last_tag``: links to the most recently tagged commit; if no tags exist, uses ``head``
+       * ``blob``: links to any blob you want, for example ``"master"`` or ``"v2.0.1"``
     """
     if blob == "head":
         return get_head()
     if blob == 'last_tag':
         return get_last_tag()
-    # Return the branch/tree/blob you provided
+    # Link to the branch/tree/blob you provided, ex. "master"
     return blob
 
 
-def get_head() -> str:
-    """Returns the hash of the most recent commit
-
-    If the most recent commit is tagged, the tag is returned instead
+def get_head(errors: bool = False) -> Optional[str]:
+    """Gets the most recent commit hash or tag
 
-    :raises RuntimeError: if the most recent commit can't be found
+    :raises subprocess.CalledProcessError: if the commit can't be found and ``errors`` is ``True``
     """
     cmd = "git log -n1 --pretty=%H"
     try:
         # get most recent commit hash
         head = subprocess.check_output(cmd.split()).strip().decode('utf-8')
 
         # if head is a tag, use tag as reference
@@ -141,32 +115,35 @@
             tag = subprocess.check_output(cmd.split(" ")).strip().decode('utf-8')
             return tag
 
         except subprocess.CalledProcessError:
             return head
 
     except subprocess.CalledProcessError as e:
-        raise RuntimeError("Failed to get head") from e  # so no head?
+        if errors:
+            raise e
+        else:
+            return logger.error("Failed to get head")  # so no head?
 
 
 def get_last_tag() -> str:
-    """Returns the most recent commit tag
+    """Get the most recent commit tag
 
     :raises RuntimeError: if there are no tagged commits
     """
     try:
         cmd = "git describe --tags --abbrev=0"
         return subprocess.check_output(cmd.split(" ")).strip().decode('utf-8')
 
     except subprocess.CalledProcessError as e:
         raise RuntimeError("No tags exist for the repo") from e
 
 
 def get_repo_dir() -> Path:
-    """Returns the root directory of the repository
+    """Get the root directory of the repository
 
     :raises RuntimeError: if the directory can't be determined
     """
     try:
         cmd = "git rev-parse --show-toplevel"
         repo_dir = Path(subprocess.check_output(cmd.split(" ")).strip().decode('utf-8'))
 
@@ -177,18 +154,19 @@
     if repo_dir.parent == "checkouts":
         return repo_dir.parent.parent
     else:
         return repo_dir
 
 
 def get_linkcode_resolve(linkcode_url: str) -> Callable:
-    """Defines and returns a ``linkcode_resolve()`` function for your package
+    """Defines and returns a ``linkcode_resolve`` function for your package
 
-    :param linkcode_url: the template URL for linking to source code (see :meth:`~get_linkcode_url`)
+    Used by default if ``linkcode_resolve`` isn't defined in ``conf.py``
     """
+
     repo_dir = get_repo_dir()
     pkg = pkg_resources.require(repo_dir.name)[0]
     top_level = pkg.get_metadata('top_level.txt').strip()
 
     def linkcode_resolve(domain, info):
         """Returns a link to the source code on GitHub, with appropriate lines highlighted
```

### Comparing `sphinx-readme-0.0.1/sphinx_readme/utils.py` & `sphinx-readme-0.0.1b6/sphinx_readme/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,21 +36,18 @@
 
 
 def format_rst(inline_markup: str, rst: str) -> str:
     """Formats text with the specified type of inline markup
 
     Preserves any ``inline literals`` within the text
 
-    **Example:**
+    :Example::
 
-    >>> format_rst("bold", "This is part of the ``sphinx_readme.utils`` module")
-    "**This is part of the** ``sphinx_readme.utils`` **module**"
-
-
-    **This is part of the** ``sphinx_readme.utils`` **module**
+        >>> format_rst("bold", "This is part of the ``sphinx_readme.utils`` module")
+        "**This is part of the** ``sphinx_readme.utils`` **module**"
 
     :param inline_markup: either "bold" or "italic"
     :param rst: the rst content to format
     """
     if inline_markup == "bold":
         markup = "**"
     elif inline_markup == "italic":
@@ -67,20 +64,20 @@
         else:
             parts.append(f"{markup}{part}{markup}")
 
     return " ".join(parts)
 
 
 def replace_only_directives(rst: str) -> str:
-    """Replaces and removes :rst:dir:`only` directives.
+    """Replaces and removes ``only`` directives
 
     If ``"readme"`` is in the ``<expression>`` part of the
-    directive, the content of the directive will be used.
+    ``only`` directive, the content will be used.
 
-    Otherwise, the directive will be removed.
+    Otherwise, the directive will be removed
 
     :param rst: the content of an ``rst`` file
     """
     # Match all ``only`` directives
     pattern = r"\.\. only::\s+(\S.*?)\n+?((?:^[ ]+.+?$|^\s*$)+?)(?=\n*\S+|\Z)"
     directives = re.findall(pattern, rst, re.M | re.DOTALL)
 
@@ -99,52 +96,46 @@
             # Remove directive
             rst = re.sub(pattern, '', rst)
 
     return rst
 
 
 def remove_raw_directives(rst: str) -> str:
-    """Removes all ``raw`` directives from ``rst``
-
-    :param rst: the rst to remove ``raw`` directives from
-    """
     return re.sub(
         pattern=r"(\.\. raw::\s+\S.*?\n+?(?:^[ ]+.+?$|^\s*$)+?)(?=\n*\S+|\Z)",
         repl='', string=rst, flags=re.M | re.DOTALL
     )
 
 
-def get_xref_variants(target: str) -> List[str]:
-    """Returns a list of ways to make a cross-reference to ``target``
-
-    **Example:**
-
-    >>> get_xref_variants('mod.Class.meth')
-    ['mod.Class.meth', '.mod.Class.meth', '~mod.Class.meth', '~.mod.Class.meth']
+def get_variants(obj: str):
+    """
 
-    :param target: the object to generate cross-reference syntax for
+    >>> get_variants('mod.Class.meth')
+    >>> ['mod.Class.meth', '.mod.Class.meth', '~mod.Class.meth', '~.mod.Class.meth']
     """
-    return [prefix + target for prefix in ('', '.', '~', '~.')]
+    return [prefix + obj for prefix in ('', '.', '~', '~.')]
 
 
-def get_all_xref_variants(fully_qualified_name: str) -> List[str]:
-    """Generates a list of all possible ways to cross-reference an object
+def get_all_variants(fully_qualified_name: str) -> List[str]:
+    """Generates a list of all possible ways to cross-reference a class/method/function
 
-    **Example:**
+    >>> get_all_variants("sphinx_github_style.meth_lexer.TDKMethLexer.get_pkg_lexer")
 
-    >>> get_all_xref_variants("sphinx_readme.utils.get_all_xref_variants") # doctest: +NORMALIZE_WHITESPACE
-    ['get_all_xref_variants', '.get_all_xref_variants', '~get_all_xref_variants',
-    '~.get_all_xref_variants', 'utils.get_all_xref_variants', '.utils.get_all_xref_variants',
-    '~utils.get_all_xref_variants', '~.utils.get_all_xref_variants',
-    'sphinx_readme.utils.get_all_xref_variants', '.sphinx_readme.utils.get_all_xref_variants',
-    '~sphinx_readme.utils.get_all_xref_variants', '~.sphinx_readme.utils.get_all_xref_variants']
+    ['get_pkg_lexer', '.get_pkg_lexer', '~get_pkg_lexer', '~.get_pkg_lexer', 'TDKMethLexer.get_pkg_lexer',
+    '.TDKMethLexer.get_pkg_lexer', '~TDKMethLexer.get_pkg_lexer', '~.TDKMethLexer.get_pkg_lexer',
+    'meth_lexer.TDKMethLexer.get_pkg_lexer', '.meth_lexer.TDKMethLexer.get_pkg_lexer',
+    '~meth_lexer.TDKMethLexer.get_pkg_lexer', '~.meth_lexer.TDKMethLexer.get_pkg_lexer',
+    'sphinx_github_style.meth_lexer.TDKMethLexer.get_pkg_lexer',
+     '.sphinx_github_style.meth_lexer.TDKMethLexer.get_pkg_lexer',
+     '~sphinx_github_style.meth_lexer.TDKMethLexer.get_pkg_lexer',
+      '~.sphinx_github_style.meth_lexer.TDKMethLexer.get_pkg_lexer']
 
-    :param fully_qualified_name: the fully qualified name of the target (ex. ``pkg.module.class.method``)
+    :param fully_qualified_name: the fully qualified name (pkg.module.class.method)
     """
     parts = fully_qualified_name.split(".")[::-1]  # => ['meth', 'Class', 'mod', "pkg"]
     variants = []
 
     for i, part in enumerate(parts):
-        target = '.'.join(parts[i::-1])  # 'meth', 'Class.meth', 'mod.class.meth', 'pkg.mod.class.meth'
-        variants.extend(get_xref_variants(target))
+        ref = '.'.join(parts[i::-1])  # 'meth', 'Class.meth', 'mod.class.meth', 'pkg.mod.class.meth'
+        variants.extend(get_variants(ref))
 
     return variants
```

### Comparing `sphinx-readme-0.0.1/sphinx_readme.egg-info/PKG-INFO` & `sphinx-readme-0.0.1b6/sphinx_readme.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-readme
-Version: 0.0.1
+Version: 0.0.1b6
 Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 Home-page: https://github.com/tdkorn/sphinx-readme
 Author: Adam Korn
 Author-email: hello@dailykitten.net
 License: MIT License
 Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
 Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
@@ -12,22 +12,22 @@
 Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
+.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
+.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
+.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
 .. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
 .. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
 .. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
-.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1/sphinx_readme/parser.py#L145-L159
-.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
-.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
-.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b6/sphinx_readme/parser.py#L124-L134
 .. |attention| replace:: 🔔️
 .. |caution| replace:: ⚠️
 .. |danger| replace:: ☢️
 .. |error| replace:: ⛔
 .. |hint| replace:: 🧠
 .. |important| replace:: 📢
 .. |note| replace:: 📝
@@ -37,31 +37,31 @@
 .. |about| replace:: 📚
 
 .. meta::
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
+
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1/docs/source/_static/logo_transparent.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/logo_readme.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
-A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
+A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
 .. |RTD| replace:: **Explore the docs »**
 .. _RTD: https://sphinx-readme.readthedocs.io/en/latest/
 
 |RTD|_
 
-|
 
 .. image:: https://img.shields.io/pypi/v/sphinx-readme?color=eb5202
    :target: https://pypi.org/project/sphinx-readme
    :alt: PyPI Project for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 .. image:: https://img.shields.io/badge/GitHub-sphinx--readme-4f1abc
    :target: https://github.com/tdkorn/sphinx-readme
@@ -71,14 +71,15 @@
    :target: https://pepy.tech/project/sphinx-readme
    :alt: Downloads for Sphinx README
 
 .. image:: https://readthedocs.org/projects/sphinx-readme/badge/?version=latest
    :target: https://sphinx-readme.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation for Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
+
 |
 
 About Sphinx README
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 
 .. csv-table::
@@ -86,22 +87,22 @@
 
    "``sphinx_readme`` is a ``reStructuredText`` parser that uses Sphinx
    to generate ``rst`` files that render beautifully on
    GitHub, PyPi, GitLab, and BitBucket."
 
 
 
-**With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
+With ``sphinx_readme``, there's no need to rewrite your ``README.rst`` as a ``README.md`` file
+==============================================================================================
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
 as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
-|
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
 
@@ -155,25 +156,25 @@
  * At minimum, the username and repository name must be specified
  * Please see `HTML Context Settings <https://docs.readthedocs.io/en/stable/guides/edit-source-links-sphinx.html>`_
    to determine the correct dictionary keys for your hosting platform
 
 .. |html_context| replace:: ``html_context``
 .. _html_context: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_context
 
-|
+...
 
 |html_baseurl|_
  The base URL which points to the root of the HTML documentation
 
   Type: ``str``
 
 .. |html_baseurl| replace:: ``html_baseurl``
 .. _html_baseurl: https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_baseurl
 
-|
+...
 
 |readme_src_files|_
  An individual or list of ``rst`` files to parse
 
   Type: ``Union[str, List]``
 
 
@@ -182,15 +183,15 @@
 
    "Filepaths should be specified relative to the source directory"
 
 
 .. |readme_src_files| replace:: ``readme_src_files``
 .. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
 
-|
+...
 
 |readme_docs_url_type|_
  The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
   Type: ``str``
 
  Must be either ``"code"`` or ``"html"``
@@ -250,16 +251,16 @@
 .. _readme_raw_directive: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_raw_directive
 
 
 
 .. csv-table::
    :header: |important| Important
 
-   "For platforms that don't support the ``raw`` directive (PyPi, GitLab, and BitBucket),
-   be sure to disable |readme_raw_directive|_:
+   "If generating a ``README`` for a platform that doesn't support ``raw``
+   directives (PyPi, GitLab, and BitBucket), be sure to disable |readme_raw_directive|_:
 
    .. code-block:: python
 
       readme_raw_directive = False"
```

