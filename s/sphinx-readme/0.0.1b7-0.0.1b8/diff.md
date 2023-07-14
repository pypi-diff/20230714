# Comparing `tmp/sphinx-readme-0.0.1b7.tar.gz` & `tmp/sphinx-readme-0.0.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-readme-0.0.1b7.tar", last modified: Fri Jul 14 06:11:55 2023, max compression
+gzip compressed data, was "sphinx-readme-0.0.1b8.tar", last modified: Fri Jul 14 06:38:14 2023, max compression
```

## Comparing `sphinx-readme-0.0.1b7.tar` & `sphinx-readme-0.0.1b8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 06:11:55.459147 sphinx-readme-0.0.1b7/
--rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.0.1b7/LICENSE
--rw-rw-rw-   0        0        0     9225 2023-07-14 06:11:55.459147 sphinx-readme-0.0.1b7/PKG-INFO
--rw-rw-rw-   0        0        0     8588 2023-07-14 06:10:36.000000 sphinx-readme-0.0.1b7/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-14 06:11:55.459147 sphinx-readme-0.0.1b7/setup.cfg
--rw-rw-rw-   0        0        0     1459 2023-07-14 06:11:30.000000 sphinx-readme-0.0.1b7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:11:55.427904 sphinx-readme-0.0.1b7/sphinx_readme/
--rw-rw-rw-   0        0        0     1712 2023-07-14 06:10:36.000000 sphinx-readme-0.0.1b7/sphinx_readme/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:11:55.459147 sphinx-readme-0.0.1b7/sphinx_readme/config/
--rw-rw-rw-   0        0        0       57 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b7/sphinx_readme/config/__init__.py
--rw-rw-rw-   0        0        0     8206 2023-07-14 06:00:41.000000 sphinx-readme-0.0.1b7/sphinx_readme/config/linkcode.py
--rw-rw-rw-   0        0        0    11635 2023-07-14 06:00:41.000000 sphinx-readme-0.0.1b7/sphinx_readme/config/main.py
--rw-rw-rw-   0        0        0    27832 2023-07-14 06:03:19.000000 sphinx-readme-0.0.1b7/sphinx_readme/parser.py
--rw-rw-rw-   0        0        0     5107 2023-07-14 06:00:41.000000 sphinx-readme-0.0.1b7/sphinx_readme/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-14 06:11:55.459147 sphinx-readme-0.0.1b7/sphinx_readme.egg-info/
--rw-rw-rw-   0        0        0     9225 2023-07-14 06:11:55.000000 sphinx-readme-0.0.1b7/sphinx_readme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2023-07-14 06:11:55.000000 sphinx-readme-0.0.1b7/sphinx_readme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 06:11:55.000000 sphinx-readme-0.0.1b7/sphinx_readme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-14 06:11:55.000000 sphinx-readme-0.0.1b7/sphinx_readme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-14 06:11:55.000000 sphinx-readme-0.0.1b7/sphinx_readme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 06:38:14.581791 sphinx-readme-0.0.1b8/
+-rw-rw-rw-   0        0        0     1084 2023-05-09 12:07:43.000000 sphinx-readme-0.0.1b8/LICENSE
+-rw-rw-rw-   0        0        0     9261 2023-07-14 06:38:14.581791 sphinx-readme-0.0.1b8/PKG-INFO
+-rw-rw-rw-   0        0        0     8470 2023-07-14 06:37:58.000000 sphinx-readme-0.0.1b8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-14 06:38:14.581791 sphinx-readme-0.0.1b8/setup.cfg
+-rw-rw-rw-   0        0        0     1454 2023-07-14 06:37:22.000000 sphinx-readme-0.0.1b8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:38:14.542387 sphinx-readme-0.0.1b8/sphinx_readme/
+-rw-rw-rw-   0        0        0     1712 2023-07-14 06:37:58.000000 sphinx-readme-0.0.1b8/sphinx_readme/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:38:14.581791 sphinx-readme-0.0.1b8/sphinx_readme/config/
+-rw-rw-rw-   0        0        0       57 2023-07-10 13:08:55.000000 sphinx-readme-0.0.1b8/sphinx_readme/config/__init__.py
+-rw-rw-rw-   0        0        0     8206 2023-07-14 06:00:41.000000 sphinx-readme-0.0.1b8/sphinx_readme/config/linkcode.py
+-rw-rw-rw-   0        0        0    11635 2023-07-14 06:00:41.000000 sphinx-readme-0.0.1b8/sphinx_readme/config/main.py
+-rw-rw-rw-   0        0        0    27832 2023-07-14 06:03:19.000000 sphinx-readme-0.0.1b8/sphinx_readme/parser.py
+-rw-rw-rw-   0        0        0     5107 2023-07-14 06:00:41.000000 sphinx-readme-0.0.1b8/sphinx_readme/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-14 06:38:14.581170 sphinx-readme-0.0.1b8/sphinx_readme.egg-info/
+-rw-rw-rw-   0        0        0     9261 2023-07-14 06:38:14.000000 sphinx-readme-0.0.1b8/sphinx_readme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-07-14 06:38:14.000000 sphinx-readme-0.0.1b8/sphinx_readme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 06:38:14.000000 sphinx-readme-0.0.1b8/sphinx_readme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-14 06:38:14.000000 sphinx-readme-0.0.1b8/sphinx_readme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-14 06:38:14.000000 sphinx-readme-0.0.1b8/sphinx_readme.egg-info/top_level.txt
```

### Comparing `sphinx-readme-0.0.1b7/LICENSE` & `sphinx-readme-0.0.1b8/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b7/PKG-INFO` & `sphinx-readme-0.0.1b8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-readme
-Version: 0.0.1b7
+Version: 0.0.1b8
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
 
-.. |.sphinx.ext.linkcode| replace:: sphinx.ext.linkcode
-.. _.sphinx.ext.linkcode: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
-.. |.sphinx.ext.autodoc| replace:: sphinx.ext.autodoc
-.. _.sphinx.ext.autodoc: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |.~.sphinx.ext.autodoc| replace:: autodoc
-.. _.~.sphinx.ext.autodoc: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |.~.parse_intersphinx_node| replace:: parse_intersphinx_node()
-.. _.~.parse_intersphinx_node: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b7/sphinx_readme/parser.py#L145-L159
+.. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1/sphinx_readme/parser.py#L145-L159
+.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
+.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
+.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
+.. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
 .. |attention| replace:: 🔔️
 .. |caution| replace:: ⚠️
 .. |danger| replace:: ☢️
 .. |error| replace:: ⛔
 .. |hint| replace:: 🧠
 .. |important| replace:: 📢
 .. |note| replace:: 📝
@@ -40,15 +40,15 @@
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/logo_transparent.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1/docs/source/_static/logo_transparent.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
 
@@ -89,29 +89,29 @@
    GitHub, PyPi, GitLab, and BitBucket."
 
 
 
 **With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
-as ``html`` builds, including |.sphinx.ext.autodoc|_ cross-references!
+as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 |
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
 
 ``sphinx_readme`` adds support for the following ``sphinx`` and ``docutils`` directives and features:
 
-* |.sphinx.ext.autodoc|_ cross-references (``:mod:``, ``:class:``, ``:meth:``, ``:func:``, and ``:attr:``)
+* |.`sphinx.ext.autodoc`|_ cross-references (``:mod:``, ``:class:``, ``:meth:``, ``:func:``, and ``:attr:``)
 * Standard cross-reference roles (``:doc:`` and ``:ref:``)
 * Generic and Specific Admonitions
 * Only directives
 * Toctrees
 * Rubrics
 * Images
 
@@ -185,23 +185,23 @@
 
 .. |readme_src_files| replace:: ``readme_src_files``
 .. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
 
 |
 
 |readme_docs_url_type|_
- The documentation source to link to when resolving |.~.sphinx.ext.autodoc|_ cross-references
+ The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
   Type: ``str``
 
  Must be either ``"code"`` or ``"html"``
 
- * ``"code"``: uses |.sphinx.ext.linkcode|_ to replace references with links to highlighted source code
+ * ``"code"``: uses |.`sphinx.ext.linkcode`|_ to replace references with links to highlighted source code
 
-   **Example**: |.~.parse_intersphinx_node|_
+   **Example**: |.`~.parse_intersphinx_node`|_
 
 
  * ``"html"``: replaces references with links to HTML documentation entries
 
    **Example**: |parse_intersphinx_node_html|_
```

### Comparing `sphinx-readme-0.0.1b7/README.rst` & `sphinx-readme-0.0.1b8/sphinx_readme.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,537 +1,579 @@
-00000000: 2e2e 207c 2e60 7370 6869 6e78 2e65 7874  .. |.`sphinx.ext
-00000010: 2e6c 696e 6b63 6f64 6560 7c20 7265 706c  .linkcode`| repl
-00000020: 6163 653a 3a20 6060 7370 6869 6e78 2e65  ace:: ``sphinx.e
-00000030: 7874 2e6c 696e 6b63 6f64 6560 600d 0a2e  xt.linkcode``...
-00000040: 2e20 5f2e 6073 7068 696e 782e 6578 742e  . _.`sphinx.ext.
-00000050: 6c69 6e6b 636f 6465 603a 2068 7474 7073  linkcode`: https
-00000060: 3a2f 2f77 7777 2e73 7068 696e 782d 646f  ://www.sphinx-do
-00000070: 632e 6f72 672f 656e 2f6d 6173 7465 722f  c.org/en/master/
-00000080: 7573 6167 652f 6578 7465 6e73 696f 6e73  usage/extensions
-00000090: 2f6c 696e 6b63 6f64 652e 6874 6d6c 236d  /linkcode.html#m
-000000a0: 6f64 756c 652d 7370 6869 6e78 2e65 7874  odule-sphinx.ext
-000000b0: 2e6c 696e 6b63 6f64 650d 0a2e 2e20 7c2e  .linkcode.... |.
-000000c0: 607e 2e70 6172 7365 5f69 6e74 6572 7370  `~.parse_intersp
-000000d0: 6869 6e78 5f6e 6f64 6560 7c20 7265 706c  hinx_node`| repl
-000000e0: 6163 653a 3a20 6060 7061 7273 655f 696e  ace:: ``parse_in
-000000f0: 7465 7273 7068 696e 785f 6e6f 6465 2829  tersphinx_node()
-00000100: 6060 0d0a 2e2e 205f 2e60 7e2e 7061 7273  ``.... _.`~.pars
-00000110: 655f 696e 7465 7273 7068 696e 785f 6e6f  e_intersphinx_no
-00000120: 6465 603a 2068 7474 7073 3a2f 2f67 6974  de`: https://git
-00000130: 6875 622e 636f 6d2f 5444 4b6f 726e 2f73  hub.com/TDKorn/s
-00000140: 7068 696e 782d 7265 6164 6d65 2f62 6c6f  phinx-readme/blo
-00000150: 622f 7630 2e30 2e31 6237 2f73 7068 696e  b/v0.0.1b7/sphin
-00000160: 785f 7265 6164 6d65 2f70 6172 7365 722e  x_readme/parser.
-00000170: 7079 234c 3134 352d 4c31 3539 0d0a 2e2e  py#L145-L159....
-00000180: 207c 2e60 7370 6869 6e78 2e65 7874 2e61   |.`sphinx.ext.a
-00000190: 7574 6f64 6f63 607c 2072 6570 6c61 6365  utodoc`| replace
-000001a0: 3a3a 2060 6073 7068 696e 782e 6578 742e  :: ``sphinx.ext.
-000001b0: 6175 746f 646f 6360 600d 0a2e 2e20 5f2e  autodoc``.... _.
-000001c0: 6073 7068 696e 782e 6578 742e 6175 746f  `sphinx.ext.auto
-000001d0: 646f 6360 3a20 6874 7470 733a 2f2f 7777  doc`: https://ww
-000001e0: 772e 7370 6869 6e78 2d64 6f63 2e6f 7267  w.sphinx-doc.org
-000001f0: 2f65 6e2f 6d61 7374 6572 2f75 7361 6765  /en/master/usage
-00000200: 2f65 7874 656e 7369 6f6e 732f 6175 746f  /extensions/auto
-00000210: 646f 632e 6874 6d6c 236d 6f64 756c 652d  doc.html#module-
-00000220: 7370 6869 6e78 2e65 7874 2e61 7574 6f64  sphinx.ext.autod
-00000230: 6f63 0d0a 2e2e 207c 2e60 7e2e 7370 6869  oc.... |.`~.sphi
-00000240: 6e78 2e65 7874 2e61 7574 6f64 6f63 607c  nx.ext.autodoc`|
-00000250: 2072 6570 6c61 6365 3a3a 2060 6061 7574   replace:: ``aut
-00000260: 6f64 6f63 6060 0d0a 2e2e 205f 2e60 7e2e  odoc``.... _.`~.
-00000270: 7370 6869 6e78 2e65 7874 2e61 7574 6f64  sphinx.ext.autod
-00000280: 6f63 603a 2068 7474 7073 3a2f 2f77 7777  oc`: https://www
-00000290: 2e73 7068 696e 782d 646f 632e 6f72 672f  .sphinx-doc.org/
-000002a0: 656e 2f6d 6173 7465 722f 7573 6167 652f  en/master/usage/
-000002b0: 6578 7465 6e73 696f 6e73 2f61 7574 6f64  extensions/autod
-000002c0: 6f63 2e68 746d 6c23 6d6f 6475 6c65 2d73  oc.html#module-s
-000002d0: 7068 696e 782e 6578 742e 6175 746f 646f  phinx.ext.autodo
-000002e0: 630d 0a0d 0a2e 2e20 6d65 7461 3a3a 0d0a  c...... meta::..
-000002f0: 2020 203a 6175 7468 6f72 3a20 4164 616d     :author: Adam
-00000300: 204b 6f72 6e0d 0a20 2020 3a74 6974 6c65   Korn..   :title
-00000310: 3a20 5370 6869 6e78 2052 4541 444d 450d  : Sphinx README.
-00000320: 0a20 2020 3a64 6573 6372 6970 7469 6f6e  .   :description
-00000330: 3a20 5370 6869 6e78 2045 7874 656e 7369  : Sphinx Extensi
-00000340: 6f6e 2074 6f20 4765 6e65 7261 7465 2042  on to Generate B
-00000350: 6561 7574 6966 756c 2072 6553 7472 7563  eautiful reStruc
-00000360: 7475 7265 6454 6578 7420 5245 4144 4d45  turedText README
-00000370: 2e72 7374 2066 6f72 2047 6974 4875 622c  .rst for GitHub,
-00000380: 2050 7950 692c 2047 6974 4c61 622c 2042   PyPi, GitLab, B
-00000390: 6974 4275 636b 6574 0d0a 0d0a 0d0a 2e2e  itBucket........
-000003a0: 2072 6177 3a3a 2068 746d 6c0d 0a0d 0a20   raw:: html.... 
-000003b0: 2020 3c64 6976 2061 6c69 676e 3d22 6365    <div align="ce
-000003c0: 6e74 6572 223e 0d0a 0d0a 2e2e 2069 6d61  nter">...... ima
-000003d0: 6765 3a3a 2068 7474 7073 3a2f 2f72 6177  ge:: https://raw
-000003e0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-000003f0: 6e74 2e63 6f6d 2f54 444b 6f72 6e2f 7370  nt.com/TDKorn/sp
-00000400: 6869 6e78 2d72 6561 646d 652f 7630 2e30  hinx-readme/v0.0
-00000410: 2e31 6236 2f64 6f63 732f 736f 7572 6365  .1b6/docs/source
-00000420: 2f5f 7374 6174 6963 2f6c 6f67 6f5f 7265  /_static/logo_re
-00000430: 6164 6d65 2e70 6e67 0d0a 2020 203a 616c  adme.png..   :al
-00000440: 743a 2053 7068 696e 7820 5245 4144 4d45  t: Sphinx README
-00000450: 3a20 4765 6e65 7261 7465 2042 6561 7574  : Generate Beaut
-00000460: 6966 756c 2072 6553 7472 7563 7475 7265  iful reStructure
-00000470: 6454 6578 7420 5245 4144 4d45 2e72 7374  dText README.rst
-00000480: 2066 6f72 2047 6974 4875 622c 2050 7950   for GitHub, PyP
-00000490: 692c 2047 6974 4c61 622c 2042 6974 4275  i, GitLab, BitBu
-000004a0: 636b 6574 0d0a 2020 203a 616c 6967 6e3a  cket..   :align:
-000004b0: 2063 656e 7465 720d 0a20 2020 3a77 6964   center..   :wid
-000004c0: 7468 3a20 3235 250d 0a0d 0a0d 0a0d 0a2e  th: 25%.........
-000004d0: 2e20 7261 773a 3a20 6874 6d6c 0d0a 0d0a  . raw:: html....
-000004e0: 2020 203c 6831 3e53 7068 696e 7820 5245     <h1>Sphinx RE
-000004f0: 4144 4d45 3c2f 6831 3e0d 0a0d 0a0d 0a0d  ADME</h1>.......
-00000500: 0a0d 0a0d 0a41 2053 7068 696e 7820 6578  .....A Sphinx ex
-00000510: 7465 6e73 696f 6e20 746f 2067 656e 6572  tension to gener
-00000520: 6174 6520 6060 5245 4144 4d45 2e72 7374  ate ``README.rst
-00000530: 6060 2066 696c 6573 2074 6861 7420 7265  `` files that re
-00000540: 6e64 6572 2062 6561 7574 6966 756c 6c79  nder beautifully
-00000550: 206f 6e20 4769 7448 7562 2c20 5079 5069   on GitHub, PyPi
-00000560: 2c20 4769 744c 6162 2c20 4269 7442 7563  , GitLab, BitBuc
-00000570: 6b65 740d 0a0d 0a2e 2e20 7c52 5444 7c20  ket...... |RTD| 
-00000580: 7265 706c 6163 653a 3a20 2a2a 4578 706c  replace:: **Expl
-00000590: 6f72 6520 7468 6520 646f 6373 20c2 bb2a  ore the docs ..*
-000005a0: 2a0d 0a2e 2e20 5f52 5444 3a20 6874 7470  *.... _RTD: http
-000005b0: 733a 2f2f 7370 6869 6e78 2d72 6561 646d  s://sphinx-readm
-000005c0: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-000005d0: 2f65 6e2f 6c61 7465 7374 2f0d 0a0d 0a7c  /en/latest/....|
-000005e0: 5254 447c 5f0d 0a0d 0a0d 0a2e 2e20 696d  RTD|_........ im
-000005f0: 6167 653a 3a20 6874 7470 733a 2f2f 696d  age:: https://im
-00000600: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000610: 692f 762f 7370 6869 6e78 2d72 6561 646d  i/v/sphinx-readm
-00000620: 653f 636f 6c6f 723d 6562 3532 3032 0d0a  e?color=eb5202..
-00000630: 2020 203a 7461 7267 6574 3a20 6874 7470     :target: http
-00000640: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-00000650: 6a65 6374 2f73 7068 696e 782d 7265 6164  ject/sphinx-read
-00000660: 6d65 0d0a 2020 203a 616c 743a 2050 7950  me..   :alt: PyP
-00000670: 4920 5072 6f6a 6563 7420 666f 7220 5370  I Project for Sp
-00000680: 6869 6e78 2052 4541 444d 453a 2047 656e  hinx README: Gen
-00000690: 6572 6174 6520 4265 6175 7469 6675 6c20  erate Beautiful 
-000006a0: 7265 5374 7275 6374 7572 6564 5465 7874  reStructuredText
-000006b0: 2052 4541 444d 452e 7273 7420 666f 7220   README.rst for 
-000006c0: 4769 7448 7562 2c20 5079 5069 2c20 4769  GitHub, PyPi, Gi
-000006d0: 744c 6162 2c20 4269 7442 7563 6b65 740d  tLab, BitBucket.
-000006e0: 0a0d 0a2e 2e20 696d 6167 653a 3a20 6874  ..... image:: ht
-000006f0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000700: 732e 696f 2f62 6164 6765 2f47 6974 4875  s.io/badge/GitHu
-00000710: 622d 7370 6869 6e78 2d2d 7265 6164 6d65  b-sphinx--readme
-00000720: 2d34 6631 6162 630d 0a20 2020 3a74 6172  -4f1abc..   :tar
-00000730: 6765 743a 2068 7474 7073 3a2f 2f67 6974  get: https://git
-00000740: 6875 622e 636f 6d2f 7464 6b6f 726e 2f73  hub.com/tdkorn/s
-00000750: 7068 696e 782d 7265 6164 6d65 0d0a 2020  phinx-readme..  
-00000760: 203a 616c 743a 2047 6974 4875 6220 5265   :alt: GitHub Re
-00000770: 706f 7369 746f 7279 2066 6f72 2053 7068  pository for Sph
-00000780: 696e 7820 5245 4144 4d45 3a20 4765 6e65  inx README: Gene
-00000790: 7261 7465 2042 6561 7574 6966 756c 2072  rate Beautiful r
-000007a0: 6553 7472 7563 7475 7265 6454 6578 7420  eStructuredText 
-000007b0: 5245 4144 4d45 2e72 7374 2066 6f72 2047  README.rst for G
-000007c0: 6974 4875 622c 2050 7950 692c 2047 6974  itHub, PyPi, Git
-000007d0: 4c61 622c 2042 6974 4275 636b 6574 0d0a  Lab, BitBucket..
-000007e0: 0d0a 2e2e 2069 6d61 6765 3a3a 2068 7474  .... image:: htt
-000007f0: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
-00000800: 2e74 6563 682f 7065 7273 6f6e 616c 697a  .tech/personaliz
-00000810: 6564 2d62 6164 6765 2f73 7068 696e 782d  ed-badge/sphinx-
-00000820: 7265 6164 6d65 3f70 6572 696f 643d 746f  readme?period=to
-00000830: 7461 6c26 756e 6974 733d 6e6f 6e65 266c  tal&units=none&l
-00000840: 6566 745f 636f 6c6f 723d 6772 6579 2672  eft_color=grey&r
-00000850: 6967 6874 5f63 6f6c 6f72 3d62 6c75 6526  ight_color=blue&
-00000860: 6c65 6674 5f74 6578 743d 446f 776e 6c6f  left_text=Downlo
-00000870: 6164 730d 0a20 2020 3a74 6172 6765 743a  ads..   :target:
-00000880: 2068 7474 7073 3a2f 2f70 6570 792e 7465   https://pepy.te
-00000890: 6368 2f70 726f 6a65 6374 2f73 7068 696e  ch/project/sphin
-000008a0: 782d 7265 6164 6d65 0d0a 2020 203a 616c  x-readme..   :al
-000008b0: 743a 2044 6f77 6e6c 6f61 6473 2066 6f72  t: Downloads for
-000008c0: 2053 7068 696e 7820 5245 4144 4d45 0d0a   Sphinx README..
-000008d0: 0d0a 2e2e 2069 6d61 6765 3a3a 2068 7474  .... image:: htt
-000008e0: 7073 3a2f 2f72 6561 6474 6865 646f 6373  ps://readthedocs
-000008f0: 2e6f 7267 2f70 726f 6a65 6374 732f 7370  .org/projects/sp
-00000900: 6869 6e78 2d72 6561 646d 652f 6261 6467  hinx-readme/badg
-00000910: 652f 3f76 6572 7369 6f6e 3d6c 6174 6573  e/?version=lates
-00000920: 740d 0a20 2020 3a74 6172 6765 743a 2068  t..   :target: h
-00000930: 7474 7073 3a2f 2f73 7068 696e 782d 7265  ttps://sphinx-re
-00000940: 6164 6d65 2e72 6561 6474 6865 646f 6373  adme.readthedocs
-00000950: 2e69 6f2f 656e 2f6c 6174 6573 742f 3f62  .io/en/latest/?b
-00000960: 6164 6765 3d6c 6174 6573 740d 0a20 2020  adge=latest..   
-00000970: 3a61 6c74 3a20 446f 6375 6d65 6e74 6174  :alt: Documentat
-00000980: 696f 6e20 666f 7220 5370 6869 6e78 2052  ion for Sphinx R
-00000990: 4541 444d 453a 2047 656e 6572 6174 6520  EADME: Generate 
-000009a0: 4265 6175 7469 6675 6c20 7265 5374 7275  Beautiful reStru
-000009b0: 6374 7572 6564 5465 7874 2052 4541 444d  cturedText READM
-000009c0: 452e 7273 7420 666f 7220 4769 7448 7562  E.rst for GitHub
-000009d0: 2c20 5079 5069 2c20 4769 744c 6162 2c20  , PyPi, GitLab, 
-000009e0: 4269 7442 7563 6b65 740d 0a0d 0a0d 0a2e  BitBucket.......
-000009f0: 2e20 7261 773a 3a20 6874 6d6c 0d0a 0d0a  . raw:: html....
-00000a00: 2020 203c 2f64 6976 3e0d 0a0d 0a7c 0d0a     </div>....|..
-00000a10: 0d0a 4162 6f75 7420 5370 6869 6e78 2052  ..About Sphinx R
-00000a20: 4541 444d 450d 0a7e 7e7e 7e7e 7e7e 7e7e  EADME..~~~~~~~~~
-00000a30: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0d0a  ~~~~~~~~~~~~~~..
-00000a40: 0d0a 0d0a 2e2e 2072 6177 3a3a 2068 746d  ...... raw:: htm
-00000a50: 6c0d 0a0d 0a20 2020 3c74 6162 6c65 3e0d  l....   <table>.
-00000a60: 0a20 2020 2020 2020 3c74 7220 616c 6967  .       <tr alig
-00000a70: 6e3d 226c 6566 7422 3e0d 0a20 2020 2020  n="left">..     
-00000a80: 2020 2020 2020 3c74 683e 0d0a 0d0a f09f        <th>......
-00000a90: 939a 2057 6861 7427 7320 5370 6869 6e78  .. What's Sphinx
-00000aa0: 2052 4541 444d 453f 0d0a 0d0a 2e2e 2072   README?...... r
-00000ab0: 6177 3a3a 2068 746d 6c0d 0a0d 0a20 2020  aw:: html....   
-00000ac0: 3c2f 7468 3e0d 0a20 2020 3c74 723e 3c74  </th>..   <tr><t
-00000ad0: 643e 0d0a 0d0a 6060 7370 6869 6e78 5f72  d>....``sphinx_r
-00000ae0: 6561 646d 6560 6020 6973 2061 2060 6072  eadme`` is a ``r
-00000af0: 6553 7472 7563 7475 7265 6454 6578 7460  eStructuredText`
-00000b00: 6020 7061 7273 6572 2074 6861 7420 7573  ` parser that us
-00000b10: 6573 2053 7068 696e 780d 0a74 6f20 6765  es Sphinx..to ge
-00000b20: 6e65 7261 7465 2060 6072 7374 6060 2066  nerate ``rst`` f
-00000b30: 696c 6573 2074 6861 7420 7265 6e64 6572  iles that render
-00000b40: 2062 6561 7574 6966 756c 6c79 206f 6e0d   beautifully on.
-00000b50: 0a47 6974 4875 622c 2050 7950 692c 2047  .GitHub, PyPi, G
-00000b60: 6974 4c61 622c 2061 6e64 2042 6974 4275  itLab, and BitBu
-00000b70: 636b 6574 2e0d 0a0d 0a2e 2e20 7261 773a  cket....... raw:
-00000b80: 3a20 6874 6d6c 0d0a 0d0a 2020 203c 2f74  : html....   </t
-00000b90: 643e 3c2f 7472 3e0d 0a20 2020 3c2f 7461  d></tr>..   </ta
-00000ba0: 626c 653e 0d0a 0d0a 0d0a 0d0a 2a2a 5769  ble>........**Wi
-00000bb0: 7468 2a2a 2060 6073 7068 696e 785f 7265  th** ``sphinx_re
-00000bc0: 6164 6d65 6060 202a 2a2c 2074 6865 7265  adme`` **, there
-00000bd0: 2773 206e 6f20 6e65 6564 2074 6f20 7265  's no need to re
-00000be0: 7772 6974 6520 796f 7572 2a2a 2060 6052  write your** ``R
-00000bf0: 4541 444d 452e 7273 7460 6020 2a2a 6173  EADME.rst`` **as
-00000c00: 2061 2a2a 2060 6052 4541 444d 452e 6d64   a** ``README.md
-00000c10: 6060 202a 2a66 696c 652a 2a0d 0a0d 0a46  `` **file**....F
-00000c20: 696c 6573 2067 656e 6572 6174 6564 2062  iles generated b
-00000c30: 7920 6060 7370 6869 6e78 5f72 6561 646d  y ``sphinx_readm
-00000c40: 6560 6020 6861 7665 206e 6561 726c 7920  e`` have nearly 
-00000c50: 6964 656e 7469 6361 6c20 6170 7065 6172  identical appear
-00000c60: 616e 6365 2061 6e64 2066 756e 6374 696f  ance and functio
-00000c70: 6e61 6c69 7479 0d0a 6173 2060 6068 746d  nality..as ``htm
-00000c80: 6c60 6020 6275 696c 6473 2c20 696e 636c  l`` builds, incl
-00000c90: 7564 696e 6720 7c2e 6073 7068 696e 782e  uding |.`sphinx.
-00000ca0: 6578 742e 6175 746f 646f 6360 7c5f 2063  ext.autodoc`|_ c
-00000cb0: 726f 7373 2d72 6566 6572 656e 6365 7321  ross-references!
-00000cc0: 0d0a 0d0a 0d0a 2e2e 2069 6d61 6765 3a3a  ........ image::
-00000cd0: 2068 7474 7073 3a2f 2f72 6177 2e67 6974   https://raw.git
-00000ce0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000cf0: 6f6d 2f54 444b 6f72 6e2f 7370 6869 6e78  om/TDKorn/sphinx
-00000d00: 2d72 6561 646d 652f 7630 2e30 2e31 6236  -readme/v0.0.1b6
-00000d10: 2f64 6f63 732f 736f 7572 6365 2f5f 7374  /docs/source/_st
-00000d20: 6174 6963 2f64 656d 6f2f 6465 6d6f 2e67  atic/demo/demo.g
-00000d30: 6966 0d0a 2020 203a 616c 743a 2044 656d  if..   :alt: Dem
-00000d40: 6f6e 7374 7261 7469 6f6e 206f 6620 686f  onstration of ho
-00000d50: 7720 7265 5374 7275 6374 7572 6564 5465  w reStructuredTe
-00000d60: 7874 2052 4541 444d 452e 7273 7420 6669  xt README.rst fi
-00000d70: 6c65 7320 6765 6e65 7261 7465 6420 6279  les generated by
-00000d80: 2053 7068 696e 7820 5245 4144 4d45 2072   Sphinx README r
-00000d90: 656e 6465 7220 6f6e 2047 6974 4875 622c  ender on GitHub,
-00000da0: 2050 7950 692c 2047 6974 4c61 622c 2042   PyPi, GitLab, B
-00000db0: 6974 4275 636b 6574 0d0a 2020 203a 7769  itBucket..   :wi
-00000dc0: 6474 683a 2037 3525 0d0a 0d0a 0d0a 4665  dth: 75%......Fe
-00000dd0: 6174 7572 6573 0d0a 7e7e 7e7e 7e7e 7e7e  atures..~~~~~~~~
-00000de0: 7e7e 0d0a 0d0a 6060 7370 6869 6e78 5f72  ~~....``sphinx_r
-00000df0: 6561 646d 6560 6020 6164 6473 2073 7570  eadme`` adds sup
-00000e00: 706f 7274 2066 6f72 2074 6865 2066 6f6c  port for the fol
-00000e10: 6c6f 7769 6e67 2060 6073 7068 696e 7860  lowing ``sphinx`
-00000e20: 6020 616e 6420 6060 646f 6375 7469 6c73  ` and ``docutils
-00000e30: 6060 2064 6972 6563 7469 7665 7320 616e  `` directives an
-00000e40: 6420 6665 6174 7572 6573 3a0d 0a0d 0a2a  d features:....*
-00000e50: 207c 2e60 7370 6869 6e78 2e65 7874 2e61   |.`sphinx.ext.a
-00000e60: 7574 6f64 6f63 607c 5f20 6372 6f73 732d  utodoc`|_ cross-
-00000e70: 7265 6665 7265 6e63 6573 2028 6060 3a6d  references (``:m
-00000e80: 6f64 3a60 602c 2060 603a 636c 6173 733a  od:``, ``:class:
-00000e90: 6060 2c20 6060 3a6d 6574 683a 6060 2c20  ``, ``:meth:``, 
-00000ea0: 6060 3a66 756e 633a 6060 2c20 616e 6420  ``:func:``, and 
-00000eb0: 6060 3a61 7474 723a 6060 290d 0a2a 2053  ``:attr:``)..* S
-00000ec0: 7461 6e64 6172 6420 6372 6f73 732d 7265  tandard cross-re
-00000ed0: 6665 7265 6e63 6520 726f 6c65 7320 2860  ference roles (`
-00000ee0: 603a 646f 633a 6060 2061 6e64 2060 603a  `:doc:`` and ``:
-00000ef0: 7265 663a 6060 290d 0a2a 2047 656e 6572  ref:``)..* Gener
-00000f00: 6963 2061 6e64 2053 7065 6369 6669 6320  ic and Specific 
-00000f10: 4164 6d6f 6e69 7469 6f6e 730d 0a2a 204f  Admonitions..* O
-00000f20: 6e6c 7920 6469 7265 6374 6976 6573 0d0a  nly directives..
-00000f30: 2a20 546f 6374 7265 6573 0d0a 2a20 5275  * Toctrees..* Ru
-00000f40: 6272 6963 730d 0a2a 2049 6d61 6765 730d  brics..* Images.
-00000f50: 0a0d 0a0d 0a49 6e73 7461 6c6c 6174 696f  .....Installatio
-00000f60: 6e0d 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  n..~~~~~~~~~~~~~
-00000f70: 0d0a 0d0a 496e 7374 616c 6c20 7573 696e  ....Install usin
-00000f80: 6720 7069 703a 3a0d 0a0d 0a20 2020 7069  g pip::....   pi
-00000f90: 7020 696e 7374 616c 6c20 7370 6869 6e78  p install sphinx
-00000fa0: 2d72 6561 646d 650d 0a0d 0a0d 0a41 6464  -readme......Add
-00000fb0: 2074 6865 2065 7874 656e 7369 6f6e 2074   the extension t
-00000fc0: 6f20 796f 7572 2060 6063 6f6e 662e 7079  o your ``conf.py
-00000fd0: 6060 3a0d 0a0d 0a2e 2e20 636f 6465 2d62  ``:...... code-b
-00000fe0: 6c6f 636b 3a3a 2070 7974 686f 6e0d 0a0d  lock:: python...
-00000ff0: 0a20 2020 6578 7465 6e73 696f 6e73 203d  .   extensions =
-00001000: 205b 0d0a 2020 2020 2020 2773 7068 696e   [..      'sphin
-00001010: 785f 7265 6164 6d65 272c 0d0a 2020 205d  x_readme',..   ]
-00001020: 0d0a 0d0a 0d0a 0d0a 436f 6e66 6967 7572  ........Configur
-00001030: 6174 696f 6e0d 0a7e 7e7e 7e7e 7e7e 7e7e  ation..~~~~~~~~~
-00001040: 7e7e 7e7e 7e7e 0d0a 0d0a 0d0a 0d0a 0d0a  ~~~~~~..........
-00001050: 0d0a 506c 6561 7365 2073 6565 2060 4578  ..Please see `Ex
-00001060: 7465 6e73 696f 6e20 436f 6e66 6967 7572  tension Configur
-00001070: 6174 696f 6e20 3c68 7474 7073 3a2f 2f73  ation <https://s
-00001080: 7068 696e 782d 7265 6164 6d65 2e72 6561  phinx-readme.rea
-00001090: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-000010a0: 6174 6573 742f 636f 6e66 6967 7572 6174  atest/configurat
-000010b0: 696f 6e2f 636f 6e66 6967 7572 696e 672e  ion/configuring.
-000010c0: 6874 6d6c 3e60 5f20 666f 7220 6675 6c6c  html>`_ for full
-000010d0: 2064 6f63 756d 656e 7461 7469 6f6e 206f   documentation o
-000010e0: 6e20 636f 6e66 6967 7572 6174 696f 6e20  n configuration 
-000010f0: 7661 7269 6162 6c65 730d 0a0d 0a0d 0a4d  variables......M
-00001100: 616e 6461 746f 7279 2060 6063 6f6e 662e  andatory ``conf.
-00001110: 7079 6060 2056 616c 7565 730d 0a3d 3d3d  py`` Values..===
-00001120: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001130: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d  ===============.
-00001140: 0a0d 0a7c 6874 6d6c 5f63 6f6e 7465 7874  ...|html_context
-00001150: 7c5f 0d0a 2041 2064 6963 7469 6f6e 6172  |_.. A dictionar
-00001160: 7920 636f 6e74 6169 6e69 6e67 2069 6e66  y containing inf
-00001170: 6f20 6162 6f75 7420 796f 7572 2072 6570  o about your rep
-00001180: 6f73 6974 6f72 790d 0a0d 0a20 2054 7970  ository....  Typ
-00001190: 653a 2060 6064 6963 7460 600d 0a0d 0a20  e: ``dict``.... 
-000011a0: 2a20 4174 206d 696e 696d 756d 2c20 7468  * At minimum, th
-000011b0: 6520 7573 6572 6e61 6d65 2061 6e64 2072  e username and r
-000011c0: 6570 6f73 6974 6f72 7920 6e61 6d65 206d  epository name m
-000011d0: 7573 7420 6265 2073 7065 6369 6669 6564  ust be specified
-000011e0: 0d0a 202a 2050 6c65 6173 6520 7365 6520  .. * Please see 
-000011f0: 6048 544d 4c20 436f 6e74 6578 7420 5365  `HTML Context Se
-00001200: 7474 696e 6773 203c 6874 7470 733a 2f2f  ttings <https://
-00001210: 646f 6373 2e72 6561 6474 6865 646f 6373  docs.readthedocs
-00001220: 2e69 6f2f 656e 2f73 7461 626c 652f 6775  .io/en/stable/gu
-00001230: 6964 6573 2f65 6469 742d 736f 7572 6365  ides/edit-source
-00001240: 2d6c 696e 6b73 2d73 7068 696e 782e 6874  -links-sphinx.ht
-00001250: 6d6c 3e60 5f0d 0a20 2020 746f 2064 6574  ml>`_..   to det
-00001260: 6572 6d69 6e65 2074 6865 2063 6f72 7265  ermine the corre
-00001270: 6374 2064 6963 7469 6f6e 6172 7920 6b65  ct dictionary ke
-00001280: 7973 2066 6f72 2079 6f75 7220 686f 7374  ys for your host
-00001290: 696e 6720 706c 6174 666f 726d 0d0a 0d0a  ing platform....
-000012a0: 2e2e 207c 6874 6d6c 5f63 6f6e 7465 7874  .. |html_context
-000012b0: 7c20 7265 706c 6163 653a 3a20 6060 6874  | replace:: ``ht
-000012c0: 6d6c 5f63 6f6e 7465 7874 6060 0d0a 2e2e  ml_context``....
-000012d0: 205f 6874 6d6c 5f63 6f6e 7465 7874 3a20   _html_context: 
-000012e0: 6874 7470 733a 2f2f 7777 772e 7370 6869  https://www.sphi
-000012f0: 6e78 2d64 6f63 2e6f 7267 2f65 6e2f 6d61  nx-doc.org/en/ma
-00001300: 7374 6572 2f75 7361 6765 2f63 6f6e 6669  ster/usage/confi
-00001310: 6775 7261 7469 6f6e 2e68 746d 6c23 636f  guration.html#co
-00001320: 6e66 7661 6c2d 6874 6d6c 5f63 6f6e 7465  nfval-html_conte
-00001330: 7874 0d0a 0d0a 7c0d 0a0d 0a7c 6874 6d6c  xt....|....|html
-00001340: 5f62 6173 6575 726c 7c5f 0d0a 2054 6865  _baseurl|_.. The
-00001350: 2062 6173 6520 5552 4c20 7768 6963 6820   base URL which 
-00001360: 706f 696e 7473 2074 6f20 7468 6520 726f  points to the ro
-00001370: 6f74 206f 6620 7468 6520 4854 4d4c 2064  ot of the HTML d
-00001380: 6f63 756d 656e 7461 7469 6f6e 0d0a 0d0a  ocumentation....
-00001390: 2020 5479 7065 3a20 6060 7374 7260 600d    Type: ``str``.
-000013a0: 0a0d 0a2e 2e20 7c68 746d 6c5f 6261 7365  ..... |html_base
-000013b0: 7572 6c7c 2072 6570 6c61 6365 3a3a 2060  url| replace:: `
-000013c0: 6068 746d 6c5f 6261 7365 7572 6c60 600d  `html_baseurl``.
-000013d0: 0a2e 2e20 5f68 746d 6c5f 6261 7365 7572  ... _html_baseur
-000013e0: 6c3a 2068 7474 7073 3a2f 2f77 7777 2e73  l: https://www.s
-000013f0: 7068 696e 782d 646f 632e 6f72 672f 656e  phinx-doc.org/en
-00001400: 2f6d 6173 7465 722f 7573 6167 652f 636f  /master/usage/co
-00001410: 6e66 6967 7572 6174 696f 6e2e 6874 6d6c  nfiguration.html
-00001420: 2363 6f6e 6676 616c 2d68 746d 6c5f 6261  #confval-html_ba
-00001430: 7365 7572 6c0d 0a0d 0a7c 0d0a 0d0a 7c72  seurl....|....|r
-00001440: 6561 646d 655f 7372 635f 6669 6c65 737c  eadme_src_files|
-00001450: 5f0d 0a20 416e 2069 6e64 6976 6964 7561  _.. An individua
-00001460: 6c20 6f72 206c 6973 7420 6f66 2060 6072  l or list of ``r
-00001470: 7374 6060 2066 696c 6573 2074 6f20 7061  st`` files to pa
-00001480: 7273 650d 0a0d 0a20 2054 7970 653a 2060  rse....  Type: `
-00001490: 6055 6e69 6f6e 5b73 7472 2c20 4c69 7374  `Union[str, List
-000014a0: 5d60 600d 0a0d 0a0d 0a2e 2e20 7261 773a  ]``........ raw:
-000014b0: 3a20 6874 6d6c 0d0a 0d0a 2020 203c 7461  : html....   <ta
-000014c0: 626c 653e 0d0a 2020 2020 2020 203c 7472  ble>..       <tr
-000014d0: 2061 6c69 676e 3d22 6c65 6674 223e 0d0a   align="left">..
-000014e0: 2020 2020 2020 2020 2020 203c 7468 3e0d             <th>.
-000014f0: 0a0d 0af0 9f93 a220 496d 706f 7274 616e  ....... Importan
-00001500: 740d 0a0d 0a2e 2e20 7261 773a 3a20 6874  t...... raw:: ht
-00001510: 6d6c 0d0a 0d0a 2020 203c 2f74 683e 0d0a  ml....   </th>..
-00001520: 2020 203c 7472 3e3c 7464 3e0d 0a0d 0a46     <tr><td>....F
-00001530: 696c 6570 6174 6873 2073 686f 756c 6420  ilepaths should 
-00001540: 6265 2073 7065 6369 6669 6564 2072 656c  be specified rel
-00001550: 6174 6976 6520 746f 2074 6865 2073 6f75  ative to the sou
-00001560: 7263 6520 6469 7265 6374 6f72 790d 0a0d  rce directory...
-00001570: 0a2e 2e20 7261 773a 3a20 6874 6d6c 0d0a  ... raw:: html..
-00001580: 0d0a 2020 203c 2f74 643e 3c2f 7472 3e0d  ..   </td></tr>.
-00001590: 0a20 2020 3c2f 7461 626c 653e 0d0a 0d0a  .   </table>....
-000015a0: 0d0a 2e2e 207c 7265 6164 6d65 5f73 7263  .... |readme_src
-000015b0: 5f66 696c 6573 7c20 7265 706c 6163 653a  _files| replace:
-000015c0: 3a20 6060 7265 6164 6d65 5f73 7263 5f66  : ``readme_src_f
-000015d0: 696c 6573 6060 0d0a 2e2e 205f 7265 6164  iles``.... _read
-000015e0: 6d65 5f73 7263 5f66 696c 6573 3a20 6874  me_src_files: ht
-000015f0: 7470 733a 2f2f 7370 6869 6e78 2d72 6561  tps://sphinx-rea
-00001600: 646d 652e 7265 6164 7468 6564 6f63 732e  dme.readthedocs.
-00001610: 696f 2f65 6e2f 6c61 7465 7374 2f63 6f6e  io/en/latest/con
-00001620: 6669 6775 7261 7469 6f6e 2f63 6f6e 6669  figuration/confi
-00001630: 6775 7269 6e67 2e68 746d 6c23 636f 6e66  guring.html#conf
-00001640: 7661 6c2d 7265 6164 6d65 5f73 7263 5f66  val-readme_src_f
-00001650: 696c 6573 0d0a 0d0a 7c0d 0a0d 0a7c 7265  iles....|....|re
-00001660: 6164 6d65 5f64 6f63 735f 7572 6c5f 7479  adme_docs_url_ty
-00001670: 7065 7c5f 0d0a 2054 6865 2064 6f63 756d  pe|_.. The docum
-00001680: 656e 7461 7469 6f6e 2073 6f75 7263 6520  entation source 
-00001690: 746f 206c 696e 6b20 746f 2077 6865 6e20  to link to when 
-000016a0: 7265 736f 6c76 696e 6720 7c2e 607e 2e73  resolving |.`~.s
-000016b0: 7068 696e 782e 6578 742e 6175 746f 646f  phinx.ext.autodo
-000016c0: 6360 7c5f 2063 726f 7373 2d72 6566 6572  c`|_ cross-refer
-000016d0: 656e 6365 730d 0a0d 0a20 2054 7970 653a  ences....  Type:
-000016e0: 2060 6073 7472 6060 0d0a 0d0a 204d 7573   ``str``.... Mus
-000016f0: 7420 6265 2065 6974 6865 7220 6060 2263  t be either ``"c
-00001700: 6f64 6522 6060 206f 7220 6060 2268 746d  ode"`` or ``"htm
-00001710: 6c22 6060 0d0a 0d0a 202a 2060 6022 636f  l"``.... * ``"co
-00001720: 6465 2260 603a 2075 7365 7320 7c2e 6073  de"``: uses |.`s
-00001730: 7068 696e 782e 6578 742e 6c69 6e6b 636f  phinx.ext.linkco
-00001740: 6465 607c 5f20 746f 2072 6570 6c61 6365  de`|_ to replace
-00001750: 2072 6566 6572 656e 6365 7320 7769 7468   references with
-00001760: 206c 696e 6b73 2074 6f20 6869 6768 6c69   links to highli
-00001770: 6768 7465 6420 736f 7572 6365 2063 6f64  ghted source cod
-00001780: 650d 0a0d 0a20 2020 2a2a 4578 616d 706c  e....   **Exampl
-00001790: 652a 2a3a 207c 2e60 7e2e 7061 7273 655f  e**: |.`~.parse_
-000017a0: 696e 7465 7273 7068 696e 785f 6e6f 6465  intersphinx_node
-000017b0: 607c 5f0d 0a0d 0a0d 0a20 2a20 6060 2268  `|_...... * ``"h
-000017c0: 746d 6c22 6060 3a20 7265 706c 6163 6573  tml"``: replaces
-000017d0: 2072 6566 6572 656e 6365 7320 7769 7468   references with
-000017e0: 206c 696e 6b73 2074 6f20 4854 4d4c 2064   links to HTML d
-000017f0: 6f63 756d 656e 7461 7469 6f6e 2065 6e74  ocumentation ent
-00001800: 7269 6573 0d0a 0d0a 2020 202a 2a45 7861  ries....   **Exa
-00001810: 6d70 6c65 2a2a 3a20 7c70 6172 7365 5f69  mple**: |parse_i
-00001820: 6e74 6572 7370 6869 6e78 5f6e 6f64 655f  ntersphinx_node_
-00001830: 6874 6d6c 7c5f 0d0a 0d0a 0d0a 2e2e 2072  html|_........ r
-00001840: 6177 3a3a 2068 746d 6c0d 0a0d 0a20 2020  aw:: html....   
-00001850: 3c74 6162 6c65 3e0d 0a20 2020 2020 2020  <table>..       
-00001860: 3c74 7220 616c 6967 6e3d 226c 6566 7422  <tr align="left"
-00001870: 3e0d 0a20 2020 2020 2020 2020 2020 3c74  >..           <t
-00001880: 683e 0d0a 0d0a f09f 939d 204e 6f74 650d  h>........ Note.
-00001890: 0a0d 0a2e 2e20 7261 773a 3a20 6874 6d6c  ..... raw:: html
-000018a0: 0d0a 0d0a 2020 203c 2f74 683e 0d0a 2020  ....   </th>..  
-000018b0: 203c 7472 3e3c 7464 3e0d 0a0d 0a49 6620   <tr><td>....If 
-000018c0: 7365 7420 746f 2060 6063 6f64 6560 602c  set to ``code``,
-000018d0: 2074 6865 6e20 3a63 6f64 653a 603a 6174   then :code:`:at
-000018e0: 7472 3a60 2063 726f 7373 2d72 6566 6572  tr:` cross-refer
-000018f0: 656e 6365 7320 7769 6c6c 206e 6f74 2062  ences will not b
-00001900: 6520 7265 706c 6163 6564 2077 6974 6820  e replaced with 
-00001910: 6c69 6e6b 730d 0a0d 0a2a 2049 6e73 7465  links....* Inste
-00001920: 6164 2c20 7468 6579 276c 6c20 6265 2072  ad, they'll be r
-00001930: 6570 6c61 6365 6420 7769 7468 2060 6069  eplaced with ``i
-00001940: 6e6c 696e 6520 6c69 7465 7261 6c73 6060  nline literals``
-00001950: 206f 7220 6c65 6674 2061 7320 6973 0d0a   or left as is..
-00001960: 2a20 506c 6561 7365 2073 6565 207c 7265  * Please see |re
-00001970: 6164 6d65 5f72 6570 6c61 6365 5f61 7474  adme_replace_att
-00001980: 7273 7c5f 2061 6e64 207c 7265 6164 6d65  rs|_ and |readme
-00001990: 5f69 6e6c 696e 655f 6d61 726b 7570 7c5f  _inline_markup|_
-000019a0: 0d0a 0d0a 2e2e 2072 6177 3a3a 2068 746d  ...... raw:: htm
-000019b0: 6c0d 0a0d 0a20 2020 3c2f 7464 3e3c 2f74  l....   </td></t
-000019c0: 723e 0d0a 2020 203c 2f74 6162 6c65 3e0d  r>..   </table>.
-000019d0: 0a0d 0a0d 0a2e 2e20 7c72 6561 646d 655f  ....... |readme_
-000019e0: 646f 6373 5f75 726c 5f74 7970 657c 2072  docs_url_type| r
-000019f0: 6570 6c61 6365 3a3a 2060 6072 6561 646d  eplace:: ``readm
-00001a00: 655f 646f 6373 5f75 726c 5f74 7970 6560  e_docs_url_type`
-00001a10: 600d 0a2e 2e20 5f72 6561 646d 655f 646f  `.... _readme_do
-00001a20: 6373 5f75 726c 5f74 7970 653a 2068 7474  cs_url_type: htt
-00001a30: 7073 3a2f 2f73 7068 696e 782d 7265 6164  ps://sphinx-read
-00001a40: 6d65 2e72 6561 6474 6865 646f 6373 2e69  me.readthedocs.i
-00001a50: 6f2f 656e 2f6c 6174 6573 742f 636f 6e66  o/en/latest/conf
-00001a60: 6967 7572 6174 696f 6e2f 636f 6e66 6967  iguration/config
-00001a70: 7572 696e 672e 6874 6d6c 2363 6f6e 6676  uring.html#confv
-00001a80: 616c 2d72 6561 646d 655f 646f 6373 5f75  al-readme_docs_u
-00001a90: 726c 5f74 7970 650d 0a2e 2e20 7c70 6172  rl_type.... |par
-00001aa0: 7365 5f69 6e74 6572 7370 6869 6e78 5f6e  se_intersphinx_n
-00001ab0: 6f64 655f 6874 6d6c 7c20 7265 706c 6163  ode_html| replac
-00001ac0: 653a 3a20 6060 7061 7273 655f 696e 7465  e:: ``parse_inte
-00001ad0: 7273 7068 696e 785f 6e6f 6465 2829 6060  rsphinx_node()``
-00001ae0: 0d0a 2e2e 205f 7061 7273 655f 696e 7465  .... _parse_inte
-00001af0: 7273 7068 696e 785f 6e6f 6465 5f68 746d  rsphinx_node_htm
-00001b00: 6c3a 2068 7474 703a 2f2f 7370 6869 6e78  l: http://sphinx
-00001b10: 2d72 6561 646d 652e 7265 6164 7468 6564  -readme.readthed
-00001b20: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00001b30: 2f70 6172 7365 722e 6874 6d6c 2373 7068  /parser.html#sph
-00001b40: 696e 785f 7265 6164 6d65 2e70 6172 7365  inx_readme.parse
-00001b50: 722e 5245 4144 4d45 5061 7273 6572 2e70  r.READMEParser.p
-00001b60: 6172 7365 5f69 6e74 6572 7370 6869 6e78  arse_intersphinx
-00001b70: 5f6e 6f64 650d 0a2e 2e20 7c72 6561 646d  _node.... |readm
-00001b80: 655f 7265 706c 6163 655f 6174 7472 737c  e_replace_attrs|
-00001b90: 2072 6570 6c61 6365 3a3a 2060 6072 6561   replace:: ``rea
-00001ba0: 646d 655f 7265 706c 6163 655f 6174 7472  dme_replace_attr
-00001bb0: 7360 600d 0a2e 2e20 5f72 6561 646d 655f  s``.... _readme_
-00001bc0: 7265 706c 6163 655f 6174 7472 733a 2068  replace_attrs: h
-00001bd0: 7474 7073 3a2f 2f73 7068 696e 782d 7265  ttps://sphinx-re
-00001be0: 6164 6d65 2e72 6561 6474 6865 646f 6373  adme.readthedocs
-00001bf0: 2e69 6f2f 656e 2f6c 6174 6573 742f 636f  .io/en/latest/co
-00001c00: 6e66 6967 7572 6174 696f 6e2f 636f 6e66  nfiguration/conf
-00001c10: 6967 7572 696e 672e 6874 6d6c 2363 6f6e  iguring.html#con
-00001c20: 6676 616c 2d72 6561 646d 655f 7265 706c  fval-readme_repl
-00001c30: 6163 655f 6174 7472 730d 0a2e 2e20 7c72  ace_attrs.... |r
-00001c40: 6561 646d 655f 696e 6c69 6e65 5f6d 6172  eadme_inline_mar
-00001c50: 6b75 707c 2072 6570 6c61 6365 3a3a 2060  kup| replace:: `
-00001c60: 6072 6561 646d 655f 696e 6c69 6e65 5f6d  `readme_inline_m
-00001c70: 6172 6b75 7060 600d 0a2e 2e20 5f72 6561  arkup``.... _rea
-00001c80: 646d 655f 696e 6c69 6e65 5f6d 6172 6b75  dme_inline_marku
-00001c90: 703a 2068 7474 7073 3a2f 2f73 7068 696e  p: https://sphin
-00001ca0: 782d 7265 6164 6d65 2e72 6561 6474 6865  x-readme.readthe
-00001cb0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00001cc0: 742f 636f 6e66 6967 7572 6174 696f 6e2f  t/configuration/
-00001cd0: 636f 6e66 6967 7572 696e 672e 6874 6d6c  configuring.html
-00001ce0: 2363 6f6e 6676 616c 2d72 6561 646d 655f  #confval-readme_
-00001cf0: 696e 6c69 6e65 5f6d 6172 6b75 700d 0a0d  inline_markup...
-00001d00: 0a0d 0a53 616d 706c 6520 6060 636f 6e66  ...Sample ``conf
-00001d10: 2e70 7960 600d 0a7e 7e7e 7e7e 7e7e 7e7e  .py``..~~~~~~~~~
-00001d20: 7e7e 7e7e 7e7e 7e7e 7e7e 0d0a 0d0a 2e2e  ~~~~~~~~~~......
-00001d30: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
-00001d40: 7468 6f6e 0d0a 0d0a 2020 2065 7874 656e  thon....   exten
-00001d50: 7369 6f6e 7320 3d20 5b0d 0a20 2020 2020  sions = [..     
-00001d60: 2022 7370 6869 6e78 5f72 6561 646d 6522   "sphinx_readme"
-00001d70: 2c0d 0a20 2020 5d0d 0a0d 0a20 2020 6874  ,..   ]....   ht
-00001d80: 6d6c 5f63 6f6e 7465 7874 203d 207b 0d0a  ml_context = {..
-00001d90: 2020 2020 2020 2764 6973 706c 6179 5f67        'display_g
-00001da0: 6974 6875 6227 3a20 5472 7565 2c0d 0a20  ithub': True,.. 
-00001db0: 2020 2020 2027 6769 7468 7562 5f75 7365       'github_use
-00001dc0: 7227 3a20 2754 444b 6f72 6e27 2c0d 0a20  r': 'TDKorn',.. 
-00001dd0: 2020 2020 2027 6769 7468 7562 5f72 6570       'github_rep
-00001de0: 6f27 3a20 2773 7068 696e 782d 7265 6164  o': 'sphinx-read
-00001df0: 6d65 272c 0d0a 2020 207d 0d0a 0d0a 2020  me',..   }....  
-00001e00: 2068 746d 6c5f 6261 7365 7572 6c20 3d20   html_baseurl = 
-00001e10: 2268 7474 7073 3a2f 2f73 7068 696e 782d  "https://sphinx-
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310d 0a4e 616d 653a 2073 7068  : 2.1..Name: sph
+00000020: 696e 782d 7265 6164 6d65 0d0a 5665 7273  inx-readme..Vers
+00000030: 696f 6e3a 2030 2e30 2e31 6238 0d0a 5375  ion: 0.0.1b8..Su
+00000040: 6d6d 6172 793a 2047 656e 6572 6174 6520  mmary: Generate 
+00000050: 4265 6175 7469 6675 6c20 7265 5374 7275  Beautiful reStru
+00000060: 6374 7572 6564 5465 7874 2052 4541 444d  cturedText READM
+00000070: 452e 7273 7420 666f 7220 4769 7448 7562  E.rst for GitHub
+00000080: 2c20 5079 5069 2c20 4769 744c 6162 2c20  , PyPi, GitLab, 
+00000090: 4269 7442 7563 6b65 740d 0a48 6f6d 652d  BitBucket..Home-
+000000a0: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
+000000b0: 7468 7562 2e63 6f6d 2f74 646b 6f72 6e2f  thub.com/tdkorn/
+000000c0: 7370 6869 6e78 2d72 6561 646d 650d 0a41  sphinx-readme..A
+000000d0: 7574 686f 723a 2041 6461 6d20 4b6f 726e  uthor: Adam Korn
+000000e0: 0d0a 4175 7468 6f72 2d65 6d61 696c 3a20  ..Author-email: 
+000000f0: 6865 6c6c 6f40 6461 696c 796b 6974 7465  hello@dailykitte
+00000100: 6e2e 6e65 740d 0a4c 6963 656e 7365 3a20  n.net..License: 
+00000110: 4d49 5420 4c69 6365 6e73 650d 0a44 6f77  MIT License..Dow
+00000120: 6e6c 6f61 642d 5552 4c3a 2068 7474 7073  nload-URL: https
+00000130: 3a2f 2f67 6974 6875 622e 636f 6d2f 5444  ://github.com/TD
+00000140: 4b6f 726e 2f73 7068 696e 782d 7265 6164  Korn/sphinx-read
+00000150: 6d65 2f74 6172 6261 6c6c 2f6d 6169 6e0d  me/tarball/main.
+00000160: 0a4b 6579 776f 7264 733a 2073 7068 696e  .Keywords: sphin
+00000170: 782c 646f 6375 7469 6c73 2c73 7068 696e  x,docutils,sphin
+00000180: 782d 6578 7465 6e73 696f 6e2c 7370 6869  x-extension,sphi
+00000190: 6e78 2d63 6f6e 7472 6962 2c72 6553 7472  nx-contrib,reStr
+000001a0: 7563 7475 7265 6454 6578 742c 7273 742c  ucturedText,rst,
+000001b0: 7265 5354 2c70 6172 7365 722c 7273 742d  reST,parser,rst-
+000001c0: 7061 7273 6572 2c52 4541 444d 452e 7273  parser,README.rs
+000001d0: 742c 5245 4144 4d45 2c61 7574 6f64 6f63  t,README,autodoc
+000001e0: 2c6c 696e 6b63 6f64 650d 0a50 6c61 7466  ,linkcode..Platf
+000001f0: 6f72 6d3a 2055 4e4b 4e4f 574e 0d0a 436c  orm: UNKNOWN..Cl
+00000200: 6173 7369 6669 6572 3a20 4672 616d 6577  assifier: Framew
+00000210: 6f72 6b20 3a3a 2053 7068 696e 7820 3a3a  ork :: Sphinx ::
+00000220: 2045 7874 656e 7369 6f6e 0d0a 436c 6173   Extension..Clas
+00000230: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
+00000240: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000250: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
+00000260: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000270: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000280: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
+00000290: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000002a0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000002b0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000002c0: 2e31 300d 0a44 6573 6372 6970 7469 6f6e  .10..Description
+000002d0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000002e0: 6578 742f 782d 7273 743b 2063 6861 7273  ext/x-rst; chars
+000002f0: 6574 3d55 5446 2d38 0d0a 4c69 6365 6e73  et=UTF-8..Licens
+00000300: 652d 4669 6c65 3a20 4c49 4345 4e53 450d  e-File: LICENSE.
+00000310: 0a0d 0a2e 2e20 7c2e 607e 2e70 6172 7365  ..... |.`~.parse
+00000320: 5f69 6e74 6572 7370 6869 6e78 5f6e 6f64  _intersphinx_nod
+00000330: 6560 7c20 7265 706c 6163 653a 3a20 6060  e`| replace:: ``
+00000340: 7061 7273 655f 696e 7465 7273 7068 696e  parse_intersphin
+00000350: 785f 6e6f 6465 2829 6060 0d0a 2e2e 205f  x_node()``.... _
+00000360: 2e60 7e2e 7061 7273 655f 696e 7465 7273  .`~.parse_inters
+00000370: 7068 696e 785f 6e6f 6465 603a 2068 7474  phinx_node`: htt
+00000380: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000390: 5444 4b6f 726e 2f73 7068 696e 782d 7265  TDKorn/sphinx-re
+000003a0: 6164 6d65 2f62 6c6f 622f 7630 2e30 2e31  adme/blob/v0.0.1
+000003b0: 2f73 7068 696e 785f 7265 6164 6d65 2f70  /sphinx_readme/p
+000003c0: 6172 7365 722e 7079 234c 3134 352d 4c31  arser.py#L145-L1
+000003d0: 3539 0d0a 2e2e 207c 2e60 7e2e 7370 6869  59.... |.`~.sphi
+000003e0: 6e78 2e65 7874 2e61 7574 6f64 6f63 607c  nx.ext.autodoc`|
+000003f0: 2072 6570 6c61 6365 3a3a 2060 6061 7574   replace:: ``aut
+00000400: 6f64 6f63 6060 0d0a 2e2e 205f 2e60 7e2e  odoc``.... _.`~.
+00000410: 7370 6869 6e78 2e65 7874 2e61 7574 6f64  sphinx.ext.autod
+00000420: 6f63 603a 2068 7474 7073 3a2f 2f77 7777  oc`: https://www
+00000430: 2e73 7068 696e 782d 646f 632e 6f72 672f  .sphinx-doc.org/
+00000440: 656e 2f6d 6173 7465 722f 7573 6167 652f  en/master/usage/
+00000450: 6578 7465 6e73 696f 6e73 2f61 7574 6f64  extensions/autod
+00000460: 6f63 2e68 746d 6c23 6d6f 6475 6c65 2d73  oc.html#module-s
+00000470: 7068 696e 782e 6578 742e 6175 746f 646f  phinx.ext.autodo
+00000480: 630d 0a2e 2e20 7c2e 6073 7068 696e 782e  c.... |.`sphinx.
+00000490: 6578 742e 6175 746f 646f 6360 7c20 7265  ext.autodoc`| re
+000004a0: 706c 6163 653a 3a20 6060 7370 6869 6e78  place:: ``sphinx
+000004b0: 2e65 7874 2e61 7574 6f64 6f63 6060 0d0a  .ext.autodoc``..
+000004c0: 2e2e 205f 2e60 7370 6869 6e78 2e65 7874  .. _.`sphinx.ext
+000004d0: 2e61 7574 6f64 6f63 603a 2068 7474 7073  .autodoc`: https
+000004e0: 3a2f 2f77 7777 2e73 7068 696e 782d 646f  ://www.sphinx-do
+000004f0: 632e 6f72 672f 656e 2f6d 6173 7465 722f  c.org/en/master/
+00000500: 7573 6167 652f 6578 7465 6e73 696f 6e73  usage/extensions
+00000510: 2f61 7574 6f64 6f63 2e68 746d 6c23 6d6f  /autodoc.html#mo
+00000520: 6475 6c65 2d73 7068 696e 782e 6578 742e  dule-sphinx.ext.
+00000530: 6175 746f 646f 630d 0a2e 2e20 7c2e 6073  autodoc.... |.`s
+00000540: 7068 696e 782e 6578 742e 6c69 6e6b 636f  phinx.ext.linkco
+00000550: 6465 607c 2072 6570 6c61 6365 3a3a 2060  de`| replace:: `
+00000560: 6073 7068 696e 782e 6578 742e 6c69 6e6b  `sphinx.ext.link
+00000570: 636f 6465 6060 0d0a 2e2e 205f 2e60 7370  code``.... _.`sp
+00000580: 6869 6e78 2e65 7874 2e6c 696e 6b63 6f64  hinx.ext.linkcod
+00000590: 6560 3a20 6874 7470 733a 2f2f 7777 772e  e`: https://www.
+000005a0: 7370 6869 6e78 2d64 6f63 2e6f 7267 2f65  sphinx-doc.org/e
+000005b0: 6e2f 6d61 7374 6572 2f75 7361 6765 2f65  n/master/usage/e
+000005c0: 7874 656e 7369 6f6e 732f 6c69 6e6b 636f  xtensions/linkco
+000005d0: 6465 2e68 746d 6c23 6d6f 6475 6c65 2d73  de.html#module-s
+000005e0: 7068 696e 782e 6578 742e 6c69 6e6b 636f  phinx.ext.linkco
+000005f0: 6465 0d0a 2e2e 207c 6174 7465 6e74 696f  de.... |attentio
+00000600: 6e7c 2072 6570 6c61 6365 3a3a 20f0 9f94  n| replace:: ...
+00000610: 94ef b88f 0d0a 2e2e 207c 6361 7574 696f  ........ |cautio
+00000620: 6e7c 2072 6570 6c61 6365 3a3a 20e2 9aa0  n| replace:: ...
+00000630: efb8 8f0d 0a2e 2e20 7c64 616e 6765 727c  ....... |danger|
+00000640: 2072 6570 6c61 6365 3a3a 20e2 98a2 efb8   replace:: .....
+00000650: 8f0d 0a2e 2e20 7c65 7272 6f72 7c20 7265  ..... |error| re
+00000660: 706c 6163 653a 3a20 e29b 940d 0a2e 2e20  place:: ....... 
+00000670: 7c68 696e 747c 2072 6570 6c61 6365 3a3a  |hint| replace::
+00000680: 20f0 9fa7 a00d 0a2e 2e20 7c69 6d70 6f72   ........ |impor
+00000690: 7461 6e74 7c20 7265 706c 6163 653a 3a20  tant| replace:: 
+000006a0: f09f 93a2 0d0a 2e2e 207c 6e6f 7465 7c20  ........ |note| 
+000006b0: 7265 706c 6163 653a 3a20 f09f 939d 0d0a  replace:: ......
+000006c0: 2e2e 207c 7469 707c 2072 6570 6c61 6365  .. |tip| replace
+000006d0: 3a3a 20f0 9f92 a10d 0a2e 2e20 7c77 6172  :: ........ |war
+000006e0: 6e69 6e67 7c20 7265 706c 6163 653a 3a20  ning| replace:: 
+000006f0: f09f 9aa9 0d0a 2e2e 207c 6465 6661 756c  ........ |defaul
+00000700: 747c 2072 6570 6c61 6365 3a3a 20f0 9f93  t| replace:: ...
+00000710: 840d 0a2e 2e20 7c61 626f 7574 7c20 7265  ..... |about| re
+00000720: 706c 6163 653a 3a20 f09f 939a 0d0a 0d0a  place:: ........
+00000730: 2e2e 206d 6574 613a 3a0d 0a20 2020 3a61  .. meta::..   :a
+00000740: 7574 686f 723a 2041 6461 6d20 4b6f 726e  uthor: Adam Korn
+00000750: 0d0a 2020 203a 7469 746c 653a 2053 7068  ..   :title: Sph
+00000760: 696e 7820 5245 4144 4d45 0d0a 2020 203a  inx README..   :
+00000770: 6465 7363 7269 7074 696f 6e3a 2053 7068  description: Sph
+00000780: 696e 7820 4578 7465 6e73 696f 6e20 746f  inx Extension to
+00000790: 2047 656e 6572 6174 6520 4265 6175 7469   Generate Beauti
+000007a0: 6675 6c20 7265 5374 7275 6374 7572 6564  ful reStructured
+000007b0: 5465 7874 2052 4541 444d 452e 7273 7420  Text README.rst 
+000007c0: 666f 7220 4769 7448 7562 2c20 5079 5069  for GitHub, PyPi
+000007d0: 2c20 4769 744c 6162 2c20 4269 7442 7563  , GitLab, BitBuc
+000007e0: 6b65 740d 0a0d 0a53 7068 696e 7820 5245  ket....Sphinx RE
+000007f0: 4144 4d45 202d 2047 656e 6572 6174 6520  ADME - Generate 
+00000800: 4265 6175 7469 6675 6c20 6060 5245 4144  Beautiful ``READ
+00000810: 4d45 2e72 7374 6060 2066 6f72 2047 6974  ME.rst`` for Git
+00000820: 4875 622c 2050 7950 692c 2047 6974 4c61  Hub, PyPi, GitLa
+00000830: 622c 2042 6974 4275 636b 6574 0d0a 2d2d  b, BitBucket..--
+00000840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000890: 2d2d 2d2d 0d0a 0d0a 2e2e 2069 6d61 6765  ----...... image
+000008a0: 3a3a 2068 7474 7073 3a2f 2f72 6177 2e67  :: https://raw.g
+000008b0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+000008c0: 2e63 6f6d 2f54 444b 6f72 6e2f 7370 6869  .com/TDKorn/sphi
+000008d0: 6e78 2d72 6561 646d 652f 7630 2e30 2e31  nx-readme/v0.0.1
+000008e0: 2f64 6f63 732f 736f 7572 6365 2f5f 7374  /docs/source/_st
+000008f0: 6174 6963 2f6c 6f67 6f5f 7472 616e 7370  atic/logo_transp
+00000900: 6172 656e 742e 706e 670d 0a20 2020 3a61  arent.png..   :a
+00000910: 6c74 3a20 5370 6869 6e78 2052 4541 444d  lt: Sphinx READM
+00000920: 453a 2047 656e 6572 6174 6520 4265 6175  E: Generate Beau
+00000930: 7469 6675 6c20 7265 5374 7275 6374 7572  tiful reStructur
+00000940: 6564 5465 7874 2052 4541 444d 452e 7273  edText README.rs
+00000950: 7420 666f 7220 4769 7448 7562 2c20 5079  t for GitHub, Py
+00000960: 5069 2c20 4769 744c 6162 2c20 4269 7442  Pi, GitLab, BitB
+00000970: 7563 6b65 740d 0a20 2020 3a61 6c69 676e  ucket..   :align
+00000980: 3a20 6365 6e74 6572 0d0a 2020 203a 7769  : center..   :wi
+00000990: 6474 683a 2032 3525 0d0a 0d0a 4120 5370  dth: 25%....A Sp
+000009a0: 6869 6e78 2065 7874 656e 7369 6f6e 2074  hinx extension t
+000009b0: 6f20 6765 6e65 7261 7465 2060 6052 4541  o generate ``REA
+000009c0: 444d 452e 7273 7460 6020 6669 6c65 7320  DME.rst`` files 
+000009d0: 7468 6174 2072 656e 6465 7220 6265 6175  that render beau
+000009e0: 7469 6675 6c6c 7920 6f6e 2047 6974 4875  tifully on GitHu
+000009f0: 622c 2050 7950 692c 2047 6974 4c61 622c  b, PyPi, GitLab,
+00000a00: 2042 6974 4275 636b 6574 0d0a 0d0a 0d0a   BitBucket......
+00000a10: 2e2e 207c 5254 447c 2072 6570 6c61 6365  .. |RTD| replace
+00000a20: 3a3a 202a 2a45 7870 6c6f 7265 2074 6865  :: **Explore the
+00000a30: 2064 6f63 7320 c2bb 2a2a 0d0a 2e2e 205f   docs ..**.... _
+00000a40: 5254 443a 2068 7474 7073 3a2f 2f73 7068  RTD: https://sph
+00000a50: 696e 782d 7265 6164 6d65 2e72 6561 6474  inx-readme.readt
+00000a60: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00000a70: 6573 742f 0d0a 0d0a 7c52 5444 7c5f 0d0a  est/....|RTD|_..
+00000a80: 0d0a 7c0d 0a0d 0a2e 2e20 696d 6167 653a  ..|...... image:
+00000a90: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
+00000aa0: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000ab0: 7370 6869 6e78 2d72 6561 646d 653f 636f  sphinx-readme?co
+00000ac0: 6c6f 723d 6562 3532 3032 0d0a 2020 203a  lor=eb5202..   :
+00000ad0: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
+00000ae0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000af0: 2f73 7068 696e 782d 7265 6164 6d65 0d0a  /sphinx-readme..
+00000b00: 2020 203a 616c 743a 2050 7950 4920 5072     :alt: PyPI Pr
+00000b10: 6f6a 6563 7420 666f 7220 5370 6869 6e78  oject for Sphinx
+00000b20: 2052 4541 444d 453a 2047 656e 6572 6174   README: Generat
+00000b30: 6520 4265 6175 7469 6675 6c20 7265 5374  e Beautiful reSt
+00000b40: 7275 6374 7572 6564 5465 7874 2052 4541  ructuredText REA
+00000b50: 444d 452e 7273 7420 666f 7220 4769 7448  DME.rst for GitH
+00000b60: 7562 2c20 5079 5069 2c20 4769 744c 6162  ub, PyPi, GitLab
+00000b70: 2c20 4269 7442 7563 6b65 740d 0a0d 0a2e  , BitBucket.....
+00000b80: 2e20 696d 6167 653a 3a20 6874 7470 733a  . image:: https:
+00000b90: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000ba0: 2f62 6164 6765 2f47 6974 4875 622d 7370  /badge/GitHub-sp
+00000bb0: 6869 6e78 2d2d 7265 6164 6d65 2d34 6631  hinx--readme-4f1
+00000bc0: 6162 630d 0a20 2020 3a74 6172 6765 743a  abc..   :target:
+00000bd0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000be0: 636f 6d2f 7464 6b6f 726e 2f73 7068 696e  com/tdkorn/sphin
+00000bf0: 782d 7265 6164 6d65 0d0a 2020 203a 616c  x-readme..   :al
+00000c00: 743a 2047 6974 4875 6220 5265 706f 7369  t: GitHub Reposi
+00000c10: 746f 7279 2066 6f72 2053 7068 696e 7820  tory for Sphinx 
+00000c20: 5245 4144 4d45 3a20 4765 6e65 7261 7465  README: Generate
+00000c30: 2042 6561 7574 6966 756c 2072 6553 7472   Beautiful reStr
+00000c40: 7563 7475 7265 6454 6578 7420 5245 4144  ucturedText READ
+00000c50: 4d45 2e72 7374 2066 6f72 2047 6974 4875  ME.rst for GitHu
+00000c60: 622c 2050 7950 692c 2047 6974 4c61 622c  b, PyPi, GitLab,
+00000c70: 2042 6974 4275 636b 6574 0d0a 0d0a 2e2e   BitBucket......
+00000c80: 2069 6d61 6765 3a3a 2068 7474 7073 3a2f   image:: https:/
+00000c90: 2f73 7461 7469 632e 7065 7079 2e74 6563  /static.pepy.tec
+00000ca0: 682f 7065 7273 6f6e 616c 697a 6564 2d62  h/personalized-b
+00000cb0: 6164 6765 2f73 7068 696e 782d 7265 6164  adge/sphinx-read
+00000cc0: 6d65 3f70 6572 696f 643d 746f 7461 6c26  me?period=total&
+00000cd0: 756e 6974 733d 6e6f 6e65 266c 6566 745f  units=none&left_
+00000ce0: 636f 6c6f 723d 6772 6579 2672 6967 6874  color=grey&right
+00000cf0: 5f63 6f6c 6f72 3d62 6c75 6526 6c65 6674  _color=blue&left
+00000d00: 5f74 6578 743d 446f 776e 6c6f 6164 730d  _text=Downloads.
+00000d10: 0a20 2020 3a74 6172 6765 743a 2068 7474  .   :target: htt
+00000d20: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
+00000d30: 726f 6a65 6374 2f73 7068 696e 782d 7265  roject/sphinx-re
+00000d40: 6164 6d65 0d0a 2020 203a 616c 743a 2044  adme..   :alt: D
+00000d50: 6f77 6e6c 6f61 6473 2066 6f72 2053 7068  ownloads for Sph
+00000d60: 696e 7820 5245 4144 4d45 0d0a 0d0a 2e2e  inx README......
+00000d70: 2069 6d61 6765 3a3a 2068 7474 7073 3a2f   image:: https:/
+00000d80: 2f72 6561 6474 6865 646f 6373 2e6f 7267  /readthedocs.org
+00000d90: 2f70 726f 6a65 6374 732f 7370 6869 6e78  /projects/sphinx
+00000da0: 2d72 6561 646d 652f 6261 6467 652f 3f76  -readme/badge/?v
+00000db0: 6572 7369 6f6e 3d6c 6174 6573 740d 0a20  ersion=latest.. 
+00000dc0: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
+00000dd0: 3a2f 2f73 7068 696e 782d 7265 6164 6d65  ://sphinx-readme
+00000de0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00000df0: 656e 2f6c 6174 6573 742f 3f62 6164 6765  en/latest/?badge
+00000e00: 3d6c 6174 6573 740d 0a20 2020 3a61 6c74  =latest..   :alt
+00000e10: 3a20 446f 6375 6d65 6e74 6174 696f 6e20  : Documentation 
+00000e20: 666f 7220 5370 6869 6e78 2052 4541 444d  for Sphinx READM
+00000e30: 453a 2047 656e 6572 6174 6520 4265 6175  E: Generate Beau
+00000e40: 7469 6675 6c20 7265 5374 7275 6374 7572  tiful reStructur
+00000e50: 6564 5465 7874 2052 4541 444d 452e 7273  edText README.rs
+00000e60: 7420 666f 7220 4769 7448 7562 2c20 5079  t for GitHub, Py
+00000e70: 5069 2c20 4769 744c 6162 2c20 4269 7442  Pi, GitLab, BitB
+00000e80: 7563 6b65 740d 0a0d 0a7c 0d0a 0d0a 4162  ucket....|....Ab
+00000e90: 6f75 7420 5370 6869 6e78 2052 4541 444d  out Sphinx READM
+00000ea0: 450d 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  E..~~~~~~~~~~~~~
+00000eb0: 7e7e 7e7e 7e7e 7e7e 7e7e 0d0a 0d0a 0d0a  ~~~~~~~~~~......
+00000ec0: 2e2e 2063 7376 2d74 6162 6c65 3a3a 0d0a  .. csv-table::..
+00000ed0: 2020 203a 6865 6164 6572 3a20 7c61 626f     :header: |abo
+00000ee0: 7574 7c20 5768 6174 2773 2053 7068 696e  ut| What's Sphin
+00000ef0: 7820 5245 4144 4d45 3f0d 0a0d 0a20 2020  x README?....   
+00000f00: 2260 6073 7068 696e 785f 7265 6164 6d65  "``sphinx_readme
+00000f10: 6060 2069 7320 6120 6060 7265 5374 7275  `` is a ``reStru
+00000f20: 6374 7572 6564 5465 7874 6060 2070 6172  cturedText`` par
+00000f30: 7365 7220 7468 6174 2075 7365 7320 5370  ser that uses Sp
+00000f40: 6869 6e78 0d0a 2020 2074 6f20 6765 6e65  hinx..   to gene
+00000f50: 7261 7465 2060 6072 7374 6060 2066 696c  rate ``rst`` fil
+00000f60: 6573 2074 6861 7420 7265 6e64 6572 2062  es that render b
+00000f70: 6561 7574 6966 756c 6c79 206f 6e0d 0a20  eautifully on.. 
+00000f80: 2020 4769 7448 7562 2c20 5079 5069 2c20    GitHub, PyPi, 
+00000f90: 4769 744c 6162 2c20 616e 6420 4269 7442  GitLab, and BitB
+00000fa0: 7563 6b65 742e 220d 0a0d 0a0d 0a0d 0a2a  ucket."........*
+00000fb0: 2a57 6974 682a 2a20 6060 7370 6869 6e78  *With** ``sphinx
+00000fc0: 5f72 6561 646d 6560 6020 2a2a 2c20 7468  _readme`` **, th
+00000fd0: 6572 6527 7320 6e6f 206e 6565 6420 746f  ere's no need to
+00000fe0: 2072 6577 7269 7465 2079 6f75 722a 2a20   rewrite your** 
+00000ff0: 6060 5245 4144 4d45 2e72 7374 6060 202a  ``README.rst`` *
+00001000: 2a61 7320 612a 2a20 6060 5245 4144 4d45  *as a** ``README
+00001010: 2e6d 6460 6020 2a2a 6669 6c65 2a2a 0d0a  .md`` **file**..
+00001020: 0d0a 4669 6c65 7320 6765 6e65 7261 7465  ..Files generate
+00001030: 6420 6279 2060 6073 7068 696e 785f 7265  d by ``sphinx_re
+00001040: 6164 6d65 6060 2068 6176 6520 6e65 6172  adme`` have near
+00001050: 6c79 2069 6465 6e74 6963 616c 2061 7070  ly identical app
+00001060: 6561 7261 6e63 6520 616e 6420 6675 6e63  earance and func
+00001070: 7469 6f6e 616c 6974 790d 0a61 7320 6060  tionality..as ``
+00001080: 6874 6d6c 6060 2062 7569 6c64 732c 2069  html`` builds, i
+00001090: 6e63 6c75 6469 6e67 207c 2e60 7370 6869  ncluding |.`sphi
+000010a0: 6e78 2e65 7874 2e61 7574 6f64 6f63 607c  nx.ext.autodoc`|
+000010b0: 5f20 6372 6f73 732d 7265 6665 7265 6e63  _ cross-referenc
+000010c0: 6573 210d 0a0d 0a7c 0d0a 0d0a 2e2e 2069  es!....|...... i
+000010d0: 6d61 6765 3a3a 2068 7474 7073 3a2f 2f72  mage:: https://r
+000010e0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+000010f0: 7465 6e74 2e63 6f6d 2f54 444b 6f72 6e2f  tent.com/TDKorn/
+00001100: 7370 6869 6e78 2d72 6561 646d 652f 7630  sphinx-readme/v0
+00001110: 2e30 2e31 2f64 6f63 732f 736f 7572 6365  .0.1/docs/source
+00001120: 2f5f 7374 6174 6963 2f64 656d 6f2f 6465  /_static/demo/de
+00001130: 6d6f 2e67 6966 0d0a 2020 203a 616c 743a  mo.gif..   :alt:
+00001140: 2044 656d 6f6e 7374 7261 7469 6f6e 206f   Demonstration o
+00001150: 6620 686f 7720 7265 5374 7275 6374 7572  f how reStructur
+00001160: 6564 5465 7874 2052 4541 444d 452e 7273  edText README.rs
+00001170: 7420 6669 6c65 7320 6765 6e65 7261 7465  t files generate
+00001180: 6420 6279 2053 7068 696e 7820 5245 4144  d by Sphinx READ
+00001190: 4d45 2072 656e 6465 7220 6f6e 2047 6974  ME render on Git
+000011a0: 4875 622c 2050 7950 692c 2047 6974 4c61  Hub, PyPi, GitLa
+000011b0: 622c 2042 6974 4275 636b 6574 0d0a 2020  b, BitBucket..  
+000011c0: 203a 7769 6474 683a 2037 3525 0d0a 0d0a   :width: 75%....
+000011d0: 0d0a 4665 6174 7572 6573 0d0a 7e7e 7e7e  ..Features..~~~~
+000011e0: 7e7e 7e7e 7e7e 0d0a 0d0a 6060 7370 6869  ~~~~~~....``sphi
+000011f0: 6e78 5f72 6561 646d 6560 6020 6164 6473  nx_readme`` adds
+00001200: 2073 7570 706f 7274 2066 6f72 2074 6865   support for the
+00001210: 2066 6f6c 6c6f 7769 6e67 2060 6073 7068   following ``sph
+00001220: 696e 7860 6020 616e 6420 6060 646f 6375  inx`` and ``docu
+00001230: 7469 6c73 6060 2064 6972 6563 7469 7665  tils`` directive
+00001240: 7320 616e 6420 6665 6174 7572 6573 3a0d  s and features:.
+00001250: 0a0d 0a2a 207c 2e60 7370 6869 6e78 2e65  ...* |.`sphinx.e
+00001260: 7874 2e61 7574 6f64 6f63 607c 5f20 6372  xt.autodoc`|_ cr
+00001270: 6f73 732d 7265 6665 7265 6e63 6573 2028  oss-references (
+00001280: 6060 3a6d 6f64 3a60 602c 2060 603a 636c  ``:mod:``, ``:cl
+00001290: 6173 733a 6060 2c20 6060 3a6d 6574 683a  ass:``, ``:meth:
+000012a0: 6060 2c20 6060 3a66 756e 633a 6060 2c20  ``, ``:func:``, 
+000012b0: 616e 6420 6060 3a61 7474 723a 6060 290d  and ``:attr:``).
+000012c0: 0a2a 2053 7461 6e64 6172 6420 6372 6f73  .* Standard cros
+000012d0: 732d 7265 6665 7265 6e63 6520 726f 6c65  s-reference role
+000012e0: 7320 2860 603a 646f 633a 6060 2061 6e64  s (``:doc:`` and
+000012f0: 2060 603a 7265 663a 6060 290d 0a2a 2047   ``:ref:``)..* G
+00001300: 656e 6572 6963 2061 6e64 2053 7065 6369  eneric and Speci
+00001310: 6669 6320 4164 6d6f 6e69 7469 6f6e 730d  fic Admonitions.
+00001320: 0a2a 204f 6e6c 7920 6469 7265 6374 6976  .* Only directiv
+00001330: 6573 0d0a 2a20 546f 6374 7265 6573 0d0a  es..* Toctrees..
+00001340: 2a20 5275 6272 6963 730d 0a2a 2049 6d61  * Rubrics..* Ima
+00001350: 6765 730d 0a0d 0a0d 0a49 6e73 7461 6c6c  ges......Install
+00001360: 6174 696f 6e0d 0a7e 7e7e 7e7e 7e7e 7e7e  ation..~~~~~~~~~
+00001370: 7e7e 7e7e 0d0a 0d0a 496e 7374 616c 6c20  ~~~~....Install 
+00001380: 7573 696e 6720 7069 703a 3a0d 0a0d 0a20  using pip::.... 
+00001390: 2020 7069 7020 696e 7374 616c 6c20 7370    pip install sp
+000013a0: 6869 6e78 2d72 6561 646d 650d 0a0d 0a0d  hinx-readme.....
+000013b0: 0a41 6464 2074 6865 2065 7874 656e 7369  .Add the extensi
+000013c0: 6f6e 2074 6f20 796f 7572 2060 6063 6f6e  on to your ``con
+000013d0: 662e 7079 6060 3a0d 0a0d 0a2e 2e20 636f  f.py``:...... co
+000013e0: 6465 2d62 6c6f 636b 3a3a 2070 7974 686f  de-block:: pytho
+000013f0: 6e0d 0a0d 0a20 2020 6578 7465 6e73 696f  n....   extensio
+00001400: 6e73 203d 205b 0d0a 2020 2020 2020 2773  ns = [..      's
+00001410: 7068 696e 785f 7265 6164 6d65 272c 0d0a  phinx_readme',..
+00001420: 2020 205d 0d0a 0d0a 0d0a 0d0a 436f 6e66     ]........Conf
+00001430: 6967 7572 6174 696f 6e0d 0a7e 7e7e 7e7e  iguration..~~~~~
+00001440: 7e7e 7e7e 7e7e 7e7e 7e7e 0d0a 0d0a 0d0a  ~~~~~~~~~~......
+00001450: 0d0a 0d0a 0d0a 506c 6561 7365 2073 6565  ......Please see
+00001460: 2060 4578 7465 6e73 696f 6e20 436f 6e66   `Extension Conf
+00001470: 6967 7572 6174 696f 6e20 3c68 7474 7073  iguration <https
+00001480: 3a2f 2f73 7068 696e 782d 7265 6164 6d65  ://sphinx-readme
+00001490: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+000014a0: 656e 2f6c 6174 6573 742f 636f 6e66 6967  en/latest/config
+000014b0: 7572 6174 696f 6e2f 636f 6e66 6967 7572  uration/configur
+000014c0: 696e 672e 6874 6d6c 3e60 5f20 666f 7220  ing.html>`_ for 
+000014d0: 6675 6c6c 2064 6f63 756d 656e 7461 7469  full documentati
+000014e0: 6f6e 206f 6e20 636f 6e66 6967 7572 6174  on on configurat
+000014f0: 696f 6e20 7661 7269 6162 6c65 730d 0a0d  ion variables...
+00001500: 0a0d 0a4d 616e 6461 746f 7279 2060 6063  ...Mandatory ``c
+00001510: 6f6e 662e 7079 6060 2056 616c 7565 730d  onf.py`` Values.
+00001520: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .===============
+00001530: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001540: 3d3d 3d0d 0a0d 0a7c 6874 6d6c 5f63 6f6e  ===....|html_con
+00001550: 7465 7874 7c5f 0d0a 2041 2064 6963 7469  text|_.. A dicti
+00001560: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+00001570: 2069 6e66 6f20 6162 6f75 7420 796f 7572   info about your
+00001580: 2072 6570 6f73 6974 6f72 790d 0a0d 0a20   repository.... 
+00001590: 2054 7970 653a 2060 6064 6963 7460 600d   Type: ``dict``.
+000015a0: 0a0d 0a20 2a20 4174 206d 696e 696d 756d  ... * At minimum
+000015b0: 2c20 7468 6520 7573 6572 6e61 6d65 2061  , the username a
+000015c0: 6e64 2072 6570 6f73 6974 6f72 7920 6e61  nd repository na
+000015d0: 6d65 206d 7573 7420 6265 2073 7065 6369  me must be speci
+000015e0: 6669 6564 0d0a 202a 2050 6c65 6173 6520  fied.. * Please 
+000015f0: 7365 6520 6048 544d 4c20 436f 6e74 6578  see `HTML Contex
+00001600: 7420 5365 7474 696e 6773 203c 6874 7470  t Settings <http
+00001610: 733a 2f2f 646f 6373 2e72 6561 6474 6865  s://docs.readthe
+00001620: 646f 6373 2e69 6f2f 656e 2f73 7461 626c  docs.io/en/stabl
+00001630: 652f 6775 6964 6573 2f65 6469 742d 736f  e/guides/edit-so
+00001640: 7572 6365 2d6c 696e 6b73 2d73 7068 696e  urce-links-sphin
+00001650: 782e 6874 6d6c 3e60 5f0d 0a20 2020 746f  x.html>`_..   to
+00001660: 2064 6574 6572 6d69 6e65 2074 6865 2063   determine the c
+00001670: 6f72 7265 6374 2064 6963 7469 6f6e 6172  orrect dictionar
+00001680: 7920 6b65 7973 2066 6f72 2079 6f75 7220  y keys for your 
+00001690: 686f 7374 696e 6720 706c 6174 666f 726d  hosting platform
+000016a0: 0d0a 0d0a 2e2e 207c 6874 6d6c 5f63 6f6e  ...... |html_con
+000016b0: 7465 7874 7c20 7265 706c 6163 653a 3a20  text| replace:: 
+000016c0: 6060 6874 6d6c 5f63 6f6e 7465 7874 6060  ``html_context``
+000016d0: 0d0a 2e2e 205f 6874 6d6c 5f63 6f6e 7465  .... _html_conte
+000016e0: 7874 3a20 6874 7470 733a 2f2f 7777 772e  xt: https://www.
+000016f0: 7370 6869 6e78 2d64 6f63 2e6f 7267 2f65  sphinx-doc.org/e
+00001700: 6e2f 6d61 7374 6572 2f75 7361 6765 2f63  n/master/usage/c
+00001710: 6f6e 6669 6775 7261 7469 6f6e 2e68 746d  onfiguration.htm
+00001720: 6c23 636f 6e66 7661 6c2d 6874 6d6c 5f63  l#confval-html_c
+00001730: 6f6e 7465 7874 0d0a 0d0a 7c0d 0a0d 0a7c  ontext....|....|
+00001740: 6874 6d6c 5f62 6173 6575 726c 7c5f 0d0a  html_baseurl|_..
+00001750: 2054 6865 2062 6173 6520 5552 4c20 7768   The base URL wh
+00001760: 6963 6820 706f 696e 7473 2074 6f20 7468  ich points to th
+00001770: 6520 726f 6f74 206f 6620 7468 6520 4854  e root of the HT
+00001780: 4d4c 2064 6f63 756d 656e 7461 7469 6f6e  ML documentation
+00001790: 0d0a 0d0a 2020 5479 7065 3a20 6060 7374  ....  Type: ``st
+000017a0: 7260 600d 0a0d 0a2e 2e20 7c68 746d 6c5f  r``...... |html_
+000017b0: 6261 7365 7572 6c7c 2072 6570 6c61 6365  baseurl| replace
+000017c0: 3a3a 2060 6068 746d 6c5f 6261 7365 7572  :: ``html_baseur
+000017d0: 6c60 600d 0a2e 2e20 5f68 746d 6c5f 6261  l``.... _html_ba
+000017e0: 7365 7572 6c3a 2068 7474 7073 3a2f 2f77  seurl: https://w
+000017f0: 7777 2e73 7068 696e 782d 646f 632e 6f72  ww.sphinx-doc.or
+00001800: 672f 656e 2f6d 6173 7465 722f 7573 6167  g/en/master/usag
+00001810: 652f 636f 6e66 6967 7572 6174 696f 6e2e  e/configuration.
+00001820: 6874 6d6c 2363 6f6e 6676 616c 2d68 746d  html#confval-htm
+00001830: 6c5f 6261 7365 7572 6c0d 0a0d 0a7c 0d0a  l_baseurl....|..
+00001840: 0d0a 7c72 6561 646d 655f 7372 635f 6669  ..|readme_src_fi
+00001850: 6c65 737c 5f0d 0a20 416e 2069 6e64 6976  les|_.. An indiv
+00001860: 6964 7561 6c20 6f72 206c 6973 7420 6f66  idual or list of
+00001870: 2060 6072 7374 6060 2066 696c 6573 2074   ``rst`` files t
+00001880: 6f20 7061 7273 650d 0a0d 0a20 2054 7970  o parse....  Typ
+00001890: 653a 2060 6055 6e69 6f6e 5b73 7472 2c20  e: ``Union[str, 
+000018a0: 4c69 7374 5d60 600d 0a0d 0a0d 0a2e 2e20  List]``........ 
+000018b0: 6373 762d 7461 626c 653a 3a0d 0a20 2020  csv-table::..   
+000018c0: 3a68 6561 6465 723a 207c 696d 706f 7274  :header: |import
+000018d0: 616e 747c 2049 6d70 6f72 7461 6e74 0d0a  ant| Important..
+000018e0: 0d0a 2020 2022 4669 6c65 7061 7468 7320  ..   "Filepaths 
+000018f0: 7368 6f75 6c64 2062 6520 7370 6563 6966  should be specif
+00001900: 6965 6420 7265 6c61 7469 7665 2074 6f20  ied relative to 
+00001910: 7468 6520 736f 7572 6365 2064 6972 6563  the source direc
+00001920: 746f 7279 220d 0a0d 0a0d 0a2e 2e20 7c72  tory"........ |r
+00001930: 6561 646d 655f 7372 635f 6669 6c65 737c  eadme_src_files|
+00001940: 2072 6570 6c61 6365 3a3a 2060 6072 6561   replace:: ``rea
+00001950: 646d 655f 7372 635f 6669 6c65 7360 600d  dme_src_files``.
+00001960: 0a2e 2e20 5f72 6561 646d 655f 7372 635f  ... _readme_src_
+00001970: 6669 6c65 733a 2068 7474 7073 3a2f 2f73  files: https://s
+00001980: 7068 696e 782d 7265 6164 6d65 2e72 6561  phinx-readme.rea
+00001990: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000019a0: 6174 6573 742f 636f 6e66 6967 7572 6174  atest/configurat
+000019b0: 696f 6e2f 636f 6e66 6967 7572 696e 672e  ion/configuring.
+000019c0: 6874 6d6c 2363 6f6e 6676 616c 2d72 6561  html#confval-rea
+000019d0: 646d 655f 7372 635f 6669 6c65 730d 0a0d  dme_src_files...
+000019e0: 0a7c 0d0a 0d0a 7c72 6561 646d 655f 646f  .|....|readme_do
+000019f0: 6373 5f75 726c 5f74 7970 657c 5f0d 0a20  cs_url_type|_.. 
+00001a00: 5468 6520 646f 6375 6d65 6e74 6174 696f  The documentatio
+00001a10: 6e20 736f 7572 6365 2074 6f20 6c69 6e6b  n source to link
+00001a20: 2074 6f20 7768 656e 2072 6573 6f6c 7669   to when resolvi
+00001a30: 6e67 207c 2e60 7e2e 7370 6869 6e78 2e65  ng |.`~.sphinx.e
+00001a40: 7874 2e61 7574 6f64 6f63 607c 5f20 6372  xt.autodoc`|_ cr
+00001a50: 6f73 732d 7265 6665 7265 6e63 6573 0d0a  oss-references..
+00001a60: 0d0a 2020 5479 7065 3a20 6060 7374 7260  ..  Type: ``str`
+00001a70: 600d 0a0d 0a20 4d75 7374 2062 6520 6569  `.... Must be ei
+00001a80: 7468 6572 2060 6022 636f 6465 2260 6020  ther ``"code"`` 
+00001a90: 6f72 2060 6022 6874 6d6c 2260 600d 0a0d  or ``"html"``...
+00001aa0: 0a20 2a20 6060 2263 6f64 6522 6060 3a20  . * ``"code"``: 
+00001ab0: 7573 6573 207c 2e60 7370 6869 6e78 2e65  uses |.`sphinx.e
+00001ac0: 7874 2e6c 696e 6b63 6f64 6560 7c5f 2074  xt.linkcode`|_ t
+00001ad0: 6f20 7265 706c 6163 6520 7265 6665 7265  o replace refere
+00001ae0: 6e63 6573 2077 6974 6820 6c69 6e6b 7320  nces with links 
+00001af0: 746f 2068 6967 686c 6967 6874 6564 2073  to highlighted s
+00001b00: 6f75 7263 6520 636f 6465 0d0a 0d0a 2020  ource code....  
+00001b10: 202a 2a45 7861 6d70 6c65 2a2a 3a20 7c2e   **Example**: |.
+00001b20: 607e 2e70 6172 7365 5f69 6e74 6572 7370  `~.parse_intersp
+00001b30: 6869 6e78 5f6e 6f64 6560 7c5f 0d0a 0d0a  hinx_node`|_....
+00001b40: 0d0a 202a 2060 6022 6874 6d6c 2260 603a  .. * ``"html"``:
+00001b50: 2072 6570 6c61 6365 7320 7265 6665 7265   replaces refere
+00001b60: 6e63 6573 2077 6974 6820 6c69 6e6b 7320  nces with links 
+00001b70: 746f 2048 544d 4c20 646f 6375 6d65 6e74  to HTML document
+00001b80: 6174 696f 6e20 656e 7472 6965 730d 0a0d  ation entries...
+00001b90: 0a20 2020 2a2a 4578 616d 706c 652a 2a3a  .   **Example**:
+00001ba0: 207c 7061 7273 655f 696e 7465 7273 7068   |parse_intersph
+00001bb0: 696e 785f 6e6f 6465 5f68 746d 6c7c 5f0d  inx_node_html|_.
+00001bc0: 0a0d 0a0d 0a2e 2e20 6373 762d 7461 626c  ....... csv-tabl
+00001bd0: 653a 3a0d 0a20 2020 3a68 6561 6465 723a  e::..   :header:
+00001be0: 207c 6e6f 7465 7c20 4e6f 7465 0d0a 0d0a   |note| Note....
+00001bf0: 2020 2022 4966 2073 6574 2074 6f20 6060     "If set to ``
+00001c00: 636f 6465 6060 2c20 7468 656e 203a 636f  code``, then :co
+00001c10: 6465 3a60 3a61 7474 723a 6020 6372 6f73  de:`:attr:` cros
+00001c20: 732d 7265 6665 7265 6e63 6573 2077 696c  s-references wil
+00001c30: 6c20 6e6f 7420 6265 2072 6570 6c61 6365  l not be replace
+00001c40: 6420 7769 7468 206c 696e 6b73 0d0a 0d0a  d with links....
+00001c50: 2020 202a 2049 6e73 7465 6164 2c20 7468     * Instead, th
+00001c60: 6579 276c 6c20 6265 2072 6570 6c61 6365  ey'll be replace
+00001c70: 6420 7769 7468 2060 6069 6e6c 696e 6520  d with ``inline 
+00001c80: 6c69 7465 7261 6c73 6060 206f 7220 6c65  literals`` or le
+00001c90: 6674 2061 7320 6973 0d0a 2020 202a 2050  ft as is..   * P
+00001ca0: 6c65 6173 6520 7365 6520 7c72 6561 646d  lease see |readm
+00001cb0: 655f 7265 706c 6163 655f 6174 7472 737c  e_replace_attrs|
+00001cc0: 5f20 616e 6420 7c72 6561 646d 655f 696e  _ and |readme_in
+00001cd0: 6c69 6e65 5f6d 6172 6b75 707c 5f22 0d0a  line_markup|_"..
+00001ce0: 0d0a 0d0a 2e2e 207c 7265 6164 6d65 5f64  ...... |readme_d
+00001cf0: 6f63 735f 7572 6c5f 7479 7065 7c20 7265  ocs_url_type| re
+00001d00: 706c 6163 653a 3a20 6060 7265 6164 6d65  place:: ``readme
+00001d10: 5f64 6f63 735f 7572 6c5f 7479 7065 6060  _docs_url_type``
+00001d20: 0d0a 2e2e 205f 7265 6164 6d65 5f64 6f63  .... _readme_doc
+00001d30: 735f 7572 6c5f 7479 7065 3a20 6874 7470  s_url_type: http
+00001d40: 733a 2f2f 7370 6869 6e78 2d72 6561 646d  s://sphinx-readm
+00001d50: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
+00001d60: 2f65 6e2f 6c61 7465 7374 2f63 6f6e 6669  /en/latest/confi
+00001d70: 6775 7261 7469 6f6e 2f63 6f6e 6669 6775  guration/configu
+00001d80: 7269 6e67 2e68 746d 6c23 636f 6e66 7661  ring.html#confva
+00001d90: 6c2d 7265 6164 6d65 5f64 6f63 735f 7572  l-readme_docs_ur
+00001da0: 6c5f 7479 7065 0d0a 2e2e 207c 7061 7273  l_type.... |pars
+00001db0: 655f 696e 7465 7273 7068 696e 785f 6e6f  e_intersphinx_no
+00001dc0: 6465 5f68 746d 6c7c 2072 6570 6c61 6365  de_html| replace
+00001dd0: 3a3a 2060 6070 6172 7365 5f69 6e74 6572  :: ``parse_inter
+00001de0: 7370 6869 6e78 5f6e 6f64 6528 2960 600d  sphinx_node()``.
+00001df0: 0a2e 2e20 5f70 6172 7365 5f69 6e74 6572  ... _parse_inter
+00001e00: 7370 6869 6e78 5f6e 6f64 655f 6874 6d6c  sphinx_node_html
+00001e10: 3a20 6874 7470 3a2f 2f73 7068 696e 782d  : http://sphinx-
 00001e20: 7265 6164 6d65 2e72 6561 6474 6865 646f  readme.readthedo
-00001e30: 6373 2e69 6f2f 656e 2f6c 6174 6573 7422  cs.io/en/latest"
-00001e40: 0d0a 0d0a 2020 2072 6561 646d 655f 7372  ....   readme_sr
-00001e50: 635f 6669 6c65 7320 3d20 2252 4541 444d  c_files = "READM
-00001e60: 452e 7273 7422 0d0a 0d0a 2020 2072 6561  E.rst"....   rea
-00001e70: 646d 655f 646f 6373 5f75 726c 5f74 7970  dme_docs_url_typ
-00001e80: 6520 3d20 2263 6f64 6522 0d0a 0d0a 0d0a  e = "code"......
-00001e90: 2e2e 207c 7265 6164 6d65 5f72 6177 5f64  .. |readme_raw_d
-00001ea0: 6972 6563 7469 7665 7c20 7265 706c 6163  irective| replac
-00001eb0: 653a 3a20 6060 7265 6164 6d65 5f72 6177  e:: ``readme_raw
-00001ec0: 5f64 6972 6563 7469 7665 6060 0d0a 2e2e  _directive``....
-00001ed0: 205f 7265 6164 6d65 5f72 6177 5f64 6972   _readme_raw_dir
-00001ee0: 6563 7469 7665 3a20 6874 7470 733a 2f2f  ective: https://
-00001ef0: 7370 6869 6e78 2d72 6561 646d 652e 7265  sphinx-readme.re
-00001f00: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00001f10: 6c61 7465 7374 2f63 6f6e 6669 6775 7261  latest/configura
-00001f20: 7469 6f6e 2f63 6f6e 6669 6775 7269 6e67  tion/configuring
-00001f30: 2e68 746d 6c23 636f 6e66 7661 6c2d 7265  .html#confval-re
-00001f40: 6164 6d65 5f72 6177 5f64 6972 6563 7469  adme_raw_directi
-00001f50: 7665 0d0a 0d0a 0d0a 0d0a 2e2e 2072 6177  ve.......... raw
-00001f60: 3a3a 2068 746d 6c0d 0a0d 0a20 2020 3c74  :: html....   <t
-00001f70: 6162 6c65 3e0d 0a20 2020 2020 2020 3c74  able>..       <t
-00001f80: 7220 616c 6967 6e3d 226c 6566 7422 3e0d  r align="left">.
-00001f90: 0a20 2020 2020 2020 2020 2020 3c74 683e  .           <th>
-00001fa0: 0d0a 0d0a f09f 93a2 2049 6d70 6f72 7461  ........ Importa
-00001fb0: 6e74 0d0a 0d0a 2e2e 2072 6177 3a3a 2068  nt...... raw:: h
-00001fc0: 746d 6c0d 0a0d 0a20 2020 3c2f 7468 3e0d  tml....   </th>.
-00001fd0: 0a20 2020 3c74 723e 3c74 643e 0d0a 0d0a  .   <tr><td>....
-00001fe0: 466f 7220 706c 6174 666f 726d 7320 7468  For platforms th
-00001ff0: 6174 2064 6f6e 2774 2073 7570 706f 7274  at don't support
-00002000: 2074 6865 2060 6072 6177 6060 2064 6972   the ``raw`` dir
-00002010: 6563 7469 7665 2028 5079 5069 2c20 4769  ective (PyPi, Gi
-00002020: 744c 6162 2c20 616e 6420 4269 7442 7563  tLab, and BitBuc
-00002030: 6b65 7429 2c0d 0a62 6520 7375 7265 2074  ket),..be sure t
-00002040: 6f20 6469 7361 626c 6520 7c72 6561 646d  o disable |readm
-00002050: 655f 7261 775f 6469 7265 6374 6976 657c  e_raw_directive|
-00002060: 5f3a 0d0a 0d0a 2e2e 2063 6f64 652d 626c  _:...... code-bl
-00002070: 6f63 6b3a 3a20 7079 7468 6f6e 0d0a 0d0a  ock:: python....
-00002080: 2020 2072 6561 646d 655f 7261 775f 6469     readme_raw_di
-00002090: 7265 6374 6976 6520 3d20 4661 6c73 650d  rective = False.
-000020a0: 0a0d 0a2e 2e20 7261 773a 3a20 6874 6d6c  ..... raw:: html
-000020b0: 0d0a 0d0a 2020 203c 2f74 643e 3c2f 7472  ....   </td></tr
-000020c0: 3e0d 0a20 2020 3c2f 7461 626c 653e 0d0a  >..   </table>..
-000020d0: 0d0a 0d0a 0d0a 0d0a 0d0a 446f 6375 6d65  ..........Docume
-000020e0: 6e74 6174 696f 6e0d 0a7e 7e7e 7e7e 7e7e  ntation..~~~~~~~
-000020f0: 7e7e 7e7e 7e7e 7e7e 7e0d 0a0d 0a46 756c  ~~~~~~~~~....Ful
-00002100: 6c20 646f 6375 6d65 6e74 6174 696f 6e20  l documentation 
-00002110: 6361 6e20 6265 2066 6f75 6e64 206f 6e20  can be found on 
-00002120: 7c64 6f63 737c 5f0d 0a0d 0a0d 0a2e 2e20  |docs|_........ 
-00002130: 7c64 6f63 737c 2072 6570 6c61 6365 3a3a  |docs| replace::
-00002140: 2060 6052 6561 6454 6865 446f 6373 6060   ``ReadTheDocs``
-00002150: 0d0a 2e2e 205f 646f 6373 3a20 6874 7470  .... _docs: http
-00002160: 733a 2f2f 7370 6869 6e78 2d72 6561 646d  s://sphinx-readm
-00002170: 652e 7265 6164 7468 6564 6f63 732e 696f  e.readthedocs.io
-00002180: 2f65 6e2f 6c61 7465 7374 0d0a            /en/latest..
+00001e30: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00001e40: 7061 7273 6572 2e68 746d 6c23 7370 6869  parser.html#sphi
+00001e50: 6e78 5f72 6561 646d 652e 7061 7273 6572  nx_readme.parser
+00001e60: 2e52 4541 444d 4550 6172 7365 722e 7061  .READMEParser.pa
+00001e70: 7273 655f 696e 7465 7273 7068 696e 785f  rse_intersphinx_
+00001e80: 6e6f 6465 0d0a 2e2e 207c 7265 6164 6d65  node.... |readme
+00001e90: 5f72 6570 6c61 6365 5f61 7474 7273 7c20  _replace_attrs| 
+00001ea0: 7265 706c 6163 653a 3a20 6060 7265 6164  replace:: ``read
+00001eb0: 6d65 5f72 6570 6c61 6365 5f61 7474 7273  me_replace_attrs
+00001ec0: 6060 0d0a 2e2e 205f 7265 6164 6d65 5f72  ``.... _readme_r
+00001ed0: 6570 6c61 6365 5f61 7474 7273 3a20 6874  eplace_attrs: ht
+00001ee0: 7470 733a 2f2f 7370 6869 6e78 2d72 6561  tps://sphinx-rea
+00001ef0: 646d 652e 7265 6164 7468 6564 6f63 732e  dme.readthedocs.
+00001f00: 696f 2f65 6e2f 6c61 7465 7374 2f63 6f6e  io/en/latest/con
+00001f10: 6669 6775 7261 7469 6f6e 2f63 6f6e 6669  figuration/confi
+00001f20: 6775 7269 6e67 2e68 746d 6c23 636f 6e66  guring.html#conf
+00001f30: 7661 6c2d 7265 6164 6d65 5f72 6570 6c61  val-readme_repla
+00001f40: 6365 5f61 7474 7273 0d0a 2e2e 207c 7265  ce_attrs.... |re
+00001f50: 6164 6d65 5f69 6e6c 696e 655f 6d61 726b  adme_inline_mark
+00001f60: 7570 7c20 7265 706c 6163 653a 3a20 6060  up| replace:: ``
+00001f70: 7265 6164 6d65 5f69 6e6c 696e 655f 6d61  readme_inline_ma
+00001f80: 726b 7570 6060 0d0a 2e2e 205f 7265 6164  rkup``.... _read
+00001f90: 6d65 5f69 6e6c 696e 655f 6d61 726b 7570  me_inline_markup
+00001fa0: 3a20 6874 7470 733a 2f2f 7370 6869 6e78  : https://sphinx
+00001fb0: 2d72 6561 646d 652e 7265 6164 7468 6564  -readme.readthed
+00001fc0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00001fd0: 2f63 6f6e 6669 6775 7261 7469 6f6e 2f63  /configuration/c
+00001fe0: 6f6e 6669 6775 7269 6e67 2e68 746d 6c23  onfiguring.html#
+00001ff0: 636f 6e66 7661 6c2d 7265 6164 6d65 5f69  confval-readme_i
+00002000: 6e6c 696e 655f 6d61 726b 7570 0d0a 0d0a  nline_markup....
+00002010: 0d0a 5361 6d70 6c65 2060 6063 6f6e 662e  ..Sample ``conf.
+00002020: 7079 6060 0d0a 7e7e 7e7e 7e7e 7e7e 7e7e  py``..~~~~~~~~~~
+00002030: 7e7e 7e7e 7e7e 7e7e 7e0d 0a0d 0a2e 2e20  ~~~~~~~~~...... 
+00002040: 636f 6465 2d62 6c6f 636b 3a3a 2070 7974  code-block:: pyt
+00002050: 686f 6e0d 0a0d 0a20 2020 6578 7465 6e73  hon....   extens
+00002060: 696f 6e73 203d 205b 0d0a 2020 2020 2020  ions = [..      
+00002070: 2273 7068 696e 785f 7265 6164 6d65 222c  "sphinx_readme",
+00002080: 0d0a 2020 205d 0d0a 0d0a 2020 2068 746d  ..   ]....   htm
+00002090: 6c5f 636f 6e74 6578 7420 3d20 7b0d 0a20  l_context = {.. 
+000020a0: 2020 2020 2027 6469 7370 6c61 795f 6769       'display_gi
+000020b0: 7468 7562 273a 2054 7275 652c 0d0a 2020  thub': True,..  
+000020c0: 2020 2020 2767 6974 6875 625f 7573 6572      'github_user
+000020d0: 273a 2027 5444 4b6f 726e 272c 0d0a 2020  ': 'TDKorn',..  
+000020e0: 2020 2020 2767 6974 6875 625f 7265 706f      'github_repo
+000020f0: 273a 2027 7370 6869 6e78 2d72 6561 646d  ': 'sphinx-readm
+00002100: 6527 2c0d 0a20 2020 7d0d 0a0d 0a20 2020  e',..   }....   
+00002110: 6874 6d6c 5f62 6173 6575 726c 203d 2022  html_baseurl = "
+00002120: 6874 7470 733a 2f2f 7370 6869 6e78 2d72  https://sphinx-r
+00002130: 6561 646d 652e 7265 6164 7468 6564 6f63  eadme.readthedoc
+00002140: 732e 696f 2f65 6e2f 6c61 7465 7374 220d  s.io/en/latest".
+00002150: 0a0d 0a20 2020 7265 6164 6d65 5f73 7263  ...   readme_src
+00002160: 5f66 696c 6573 203d 2022 5245 4144 4d45  _files = "README
+00002170: 2e72 7374 220d 0a0d 0a20 2020 7265 6164  .rst"....   read
+00002180: 6d65 5f64 6f63 735f 7572 6c5f 7479 7065  me_docs_url_type
+00002190: 203d 2022 636f 6465 220d 0a0d 0a0d 0a2e   = "code".......
+000021a0: 2e20 7c72 6561 646d 655f 7261 775f 6469  . |readme_raw_di
+000021b0: 7265 6374 6976 657c 2072 6570 6c61 6365  rective| replace
+000021c0: 3a3a 2060 6072 6561 646d 655f 7261 775f  :: ``readme_raw_
+000021d0: 6469 7265 6374 6976 6560 600d 0a2e 2e20  directive``.... 
+000021e0: 5f72 6561 646d 655f 7261 775f 6469 7265  _readme_raw_dire
+000021f0: 6374 6976 653a 2068 7474 7073 3a2f 2f73  ctive: https://s
+00002200: 7068 696e 782d 7265 6164 6d65 2e72 6561  phinx-readme.rea
+00002210: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00002220: 6174 6573 742f 636f 6e66 6967 7572 6174  atest/configurat
+00002230: 696f 6e2f 636f 6e66 6967 7572 696e 672e  ion/configuring.
+00002240: 6874 6d6c 2363 6f6e 6676 616c 2d72 6561  html#confval-rea
+00002250: 646d 655f 7261 775f 6469 7265 6374 6976  dme_raw_directiv
+00002260: 650d 0a0d 0a0d 0a0d 0a2e 2e20 6373 762d  e.......... csv-
+00002270: 7461 626c 653a 3a0d 0a20 2020 3a68 6561  table::..   :hea
+00002280: 6465 723a 207c 696d 706f 7274 616e 747c  der: |important|
+00002290: 2049 6d70 6f72 7461 6e74 0d0a 0d0a 2020   Important....  
+000022a0: 2022 466f 7220 706c 6174 666f 726d 7320   "For platforms 
+000022b0: 7468 6174 2064 6f6e 2774 2073 7570 706f  that don't suppo
+000022c0: 7274 2074 6865 2060 6072 6177 6060 2064  rt the ``raw`` d
+000022d0: 6972 6563 7469 7665 2028 5079 5069 2c20  irective (PyPi, 
+000022e0: 4769 744c 6162 2c20 616e 6420 4269 7442  GitLab, and BitB
+000022f0: 7563 6b65 7429 2c0d 0a20 2020 6265 2073  ucket),..   be s
+00002300: 7572 6520 746f 2064 6973 6162 6c65 207c  ure to disable |
+00002310: 7265 6164 6d65 5f72 6177 5f64 6972 6563  readme_raw_direc
+00002320: 7469 7665 7c5f 3a0d 0a0d 0a20 2020 2e2e  tive|_:....   ..
+00002330: 2063 6f64 652d 626c 6f63 6b3a 3a20 7079   code-block:: py
+00002340: 7468 6f6e 0d0a 0d0a 2020 2020 2020 7265  thon....      re
+00002350: 6164 6d65 5f72 6177 5f64 6972 6563 7469  adme_raw_directi
+00002360: 7665 203d 2046 616c 7365 220d 0a0d 0a0d  ve = False".....
+00002370: 0a0d 0a0d 0a0d 0a44 6f63 756d 656e 7461  .......Documenta
+00002380: 7469 6f6e 0d0a 7e7e 7e7e 7e7e 7e7e 7e7e  tion..~~~~~~~~~~
+00002390: 7e7e 7e7e 7e7e 0d0a 0d0a 4675 6c6c 2064  ~~~~~~....Full d
+000023a0: 6f63 756d 656e 7461 7469 6f6e 2063 616e  ocumentation can
+000023b0: 2062 6520 666f 756e 6420 6f6e 207c 646f   be found on |do
+000023c0: 6373 7c5f 0d0a 0d0a 0d0a 2e2e 207c 646f  cs|_........ |do
+000023d0: 6373 7c20 7265 706c 6163 653a 3a20 6060  cs| replace:: ``
+000023e0: 5265 6164 5468 6544 6f63 7360 600d 0a2e  ReadTheDocs``...
+000023f0: 2e20 5f64 6f63 733a 2068 7474 7073 3a2f  . _docs: https:/
+00002400: 2f73 7068 696e 782d 7265 6164 6d65 2e72  /sphinx-readme.r
+00002410: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00002420: 2f6c 6174 6573 740d 0a0d 0a0d 0a         /latest......
```

### Comparing `sphinx-readme-0.0.1b7/setup.py` & `sphinx-readme-0.0.1b8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup, find_packages
 
-LONG_DESCRIPTION_SRC = 'README_PyPi.rst'
+LONG_DESCRIPTION_SRC = 'README.rst'
 
 
 def read(file):
     with open(os.path.abspath(file), 'r', encoding='utf-8') as f:
         return f.read()
```

### Comparing `sphinx-readme-0.0.1b7/sphinx_readme/__init__.py` & `sphinx-readme-0.0.1b8/sphinx_readme/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
 from sphinx_readme.utils import get_conf_val, set_conf_val
 from sphinx_readme.config import get_repo_dir
 from sphinx_readme.parser import READMEParser
 
 
-__version__ = "v0.0.1b7"
+__version__ = "v0.0.1b8"
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
     # Avoid setting up extension if building on ReadTheDocs
     if os.environ.get("READTHEDOCS") == "True":
         return {}
```

### Comparing `sphinx-readme-0.0.1b7/sphinx_readme/config/linkcode.py` & `sphinx-readme-0.0.1b8/sphinx_readme/config/linkcode.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b7/sphinx_readme/config/main.py` & `sphinx-readme-0.0.1b8/sphinx_readme/config/main.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b7/sphinx_readme/parser.py` & `sphinx-readme-0.0.1b8/sphinx_readme/parser.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b7/sphinx_readme/utils.py` & `sphinx-readme-0.0.1b8/sphinx_readme/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx-readme-0.0.1b7/sphinx_readme.egg-info/PKG-INFO` & `sphinx-readme-0.0.1b8/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,15 @@
-Metadata-Version: 2.1
-Name: sphinx-readme
-Version: 0.0.1b7
-Summary: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
-Home-page: https://github.com/tdkorn/sphinx-readme
-Author: Adam Korn
-Author-email: hello@dailykitten.net
-License: MIT License
-Download-URL: https://github.com/TDKorn/sphinx-readme/tarball/main
-Keywords: sphinx,docutils,sphinx-extension,sphinx-contrib,reStructuredText,rst,reST,parser,rst-parser,README.rst,README,autodoc,linkcode
-Platform: UNKNOWN
-Classifier: Framework :: Sphinx :: Extension
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/x-rst; charset=UTF-8
-License-File: LICENSE
-
-.. |.sphinx.ext.linkcode| replace:: sphinx.ext.linkcode
-.. _.sphinx.ext.linkcode: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
-.. |.sphinx.ext.autodoc| replace:: sphinx.ext.autodoc
-.. _.sphinx.ext.autodoc: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |.~.sphinx.ext.autodoc| replace:: autodoc
-.. _.~.sphinx.ext.autodoc: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
-.. |.~.parse_intersphinx_node| replace:: parse_intersphinx_node()
-.. _.~.parse_intersphinx_node: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1b7/sphinx_readme/parser.py#L145-L159
+.. |.`~.parse_intersphinx_node`| replace:: ``parse_intersphinx_node()``
+.. _.`~.parse_intersphinx_node`: https://github.com/TDKorn/sphinx-readme/blob/v0.0.1/sphinx_readme/parser.py#L145-L159
+.. |.`~.sphinx.ext.autodoc`| replace:: ``autodoc``
+.. _.`~.sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. |.`sphinx.ext.autodoc`| replace:: ``sphinx.ext.autodoc``
+.. _.`sphinx.ext.autodoc`: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#module-sphinx.ext.autodoc
+.. |.`sphinx.ext.linkcode`| replace:: ``sphinx.ext.linkcode``
+.. _.`sphinx.ext.linkcode`: https://www.sphinx-doc.org/en/master/usage/extensions/linkcode.html#module-sphinx.ext.linkcode
 .. |attention| replace:: 🔔️
 .. |caution| replace:: ⚠️
 .. |danger| replace:: ☢️
 .. |error| replace:: ⛔
 .. |hint| replace:: 🧠
 .. |important| replace:: 📢
 .. |note| replace:: 📝
@@ -40,15 +22,15 @@
    :author: Adam Korn
    :title: Sphinx README
    :description: Sphinx Extension to Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
 
 Sphinx README - Generate Beautiful ``README.rst`` for GitHub, PyPi, GitLab, BitBucket
 --------------------------------------------------------------------------------------
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/logo_transparent.png
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1/docs/source/_static/logo_transparent.png
    :alt: Sphinx README: Generate Beautiful reStructuredText README.rst for GitHub, PyPi, GitLab, BitBucket
    :align: center
    :width: 25%
 
 A Sphinx extension to generate ``README.rst`` files that render beautifully on GitHub, PyPi, GitLab, BitBucket
 
 
@@ -89,29 +71,29 @@
    GitHub, PyPi, GitLab, and BitBucket."
 
 
 
 **With** ``sphinx_readme`` **, there's no need to rewrite your** ``README.rst`` **as a** ``README.md`` **file**
 
 Files generated by ``sphinx_readme`` have nearly identical appearance and functionality
-as ``html`` builds, including |.sphinx.ext.autodoc|_ cross-references!
+as ``html`` builds, including |.`sphinx.ext.autodoc`|_ cross-references!
 
 |
 
-.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1b6/docs/source/_static/demo/demo.gif
+.. image:: https://raw.githubusercontent.com/TDKorn/sphinx-readme/v0.0.1/docs/source/_static/demo/demo.gif
    :alt: Demonstration of how reStructuredText README.rst files generated by Sphinx README render on GitHub, PyPi, GitLab, BitBucket
    :width: 75%
 
 
 Features
 ~~~~~~~~~~
 
 ``sphinx_readme`` adds support for the following ``sphinx`` and ``docutils`` directives and features:
 
-* |.sphinx.ext.autodoc|_ cross-references (``:mod:``, ``:class:``, ``:meth:``, ``:func:``, and ``:attr:``)
+* |.`sphinx.ext.autodoc`|_ cross-references (``:mod:``, ``:class:``, ``:meth:``, ``:func:``, and ``:attr:``)
 * Standard cross-reference roles (``:doc:`` and ``:ref:``)
 * Generic and Specific Admonitions
 * Only directives
 * Toctrees
 * Rubrics
 * Images
 
@@ -185,23 +167,23 @@
 
 .. |readme_src_files| replace:: ``readme_src_files``
 .. _readme_src_files: https://sphinx-readme.readthedocs.io/en/latest/configuration/configuring.html#confval-readme_src_files
 
 |
 
 |readme_docs_url_type|_
- The documentation source to link to when resolving |.~.sphinx.ext.autodoc|_ cross-references
+ The documentation source to link to when resolving |.`~.sphinx.ext.autodoc`|_ cross-references
 
   Type: ``str``
 
  Must be either ``"code"`` or ``"html"``
 
- * ``"code"``: uses |.sphinx.ext.linkcode|_ to replace references with links to highlighted source code
+ * ``"code"``: uses |.`sphinx.ext.linkcode`|_ to replace references with links to highlighted source code
 
-   **Example**: |.~.parse_intersphinx_node|_
+   **Example**: |.`~.parse_intersphinx_node`|_
 
 
  * ``"html"``: replaces references with links to HTML documentation entries
 
    **Example**: |parse_intersphinx_node_html|_
 
 
@@ -269,9 +251,7 @@
 ~~~~~~~~~~~~~~~~
 
 Full documentation can be found on |docs|_
 
 
 .. |docs| replace:: ``ReadTheDocs``
 .. _docs: https://sphinx-readme.readthedocs.io/en/latest
-
-
```

