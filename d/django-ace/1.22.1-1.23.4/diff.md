# Comparing `tmp/django-ace-1.22.1.tar.gz` & `tmp/django-ace-1.23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ace-1.22.1.tar", last modified: Mon Jun 12 09:21:54 2023, max compression
+gzip compressed data, was "django-ace-1.23.4.tar", last modified: Fri Jul 14 13:16:27 2023, max compression
```

## Comparing `django-ace-1.22.1.tar` & `django-ace-1.23.4.tar`

### file list

```diff
@@ -1,476 +1,476 @@
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-06-12 09:21:54.795644 django-ace-1.22.1/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     5388 2020-10-04 15:07:59.000000 django-ace-1.22.1/LICENCE
--rw-r--r--   0 mdk       (1000) mdk       (1000)       65 2019-12-04 21:51:14.000000 django-ace-1.22.1/MANIFEST.in
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3942 2023-06-12 09:21:54.799644 django-ace-1.22.1/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3342 2023-06-12 09:21:20.000000 django-ace-1.22.1/README.rst
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-06-12 09:21:54.691649 django-ace-1.22.1/django_ace/
--rw-r--r--   0 mdk       (1000) mdk       (1000)       75 2023-06-12 09:21:32.000000 django-ace-1.22.1/django_ace/__init__.py
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-06-12 09:21:54.691649 django-ace-1.22.1/django_ace/static/
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-06-12 09:21:54.703648 django-ace-1.22.1/django_ace/static/django_ace/
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-06-12 09:21:54.771645 django-ace-1.22.1/django_ace/static/django_ace/ace/
--rw-r--r--   0 mdk       (1000) mdk       (1000)   842898 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ace.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13362 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-beautify.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     8185 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-code_lens.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    21729 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-command_bar.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     9282 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-elastic_tabstops_lite.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    51049 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-emmet.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-error_marker.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4368 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-hardwrap.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   128756 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-inline_autocomplete.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     6741 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-keybinding_menu.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    93620 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-language_tools.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2007 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-linking.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     7041 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-modelist.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    26335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-options.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   114091 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-prompt.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4640 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-rtl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    18380 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-searchbox.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    27248 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-settings_menu.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2521 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-spellcheck.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     6546 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-split.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     7487 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-static_highlight.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1966 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-statusbar.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13022 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-textarea.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2480 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-themelist.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     6755 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/ext-whitespace.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    43079 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/keybinding-emacs.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    12833 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/keybinding-sublime.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   251788 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/keybinding-vim.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     9188 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/keybinding-vscode.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     9492 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-abap.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     9449 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-abc.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    25355 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-actionscript.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4323 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ada.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    10523 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-alda.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    19937 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-apache_conf.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    15658 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-apex.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     9813 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-applescript.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     5601 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-aql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    14224 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-asciidoc.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    14861 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-asl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    12287 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-assembly_x86.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    67779 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-autohotkey.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     8835 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-batchfile.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    11316 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-bibtex.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     9836 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-c9search.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    19561 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-c_cpp.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     6577 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-cirru.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    14162 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-clojure.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3775 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-cobol.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13889 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-coffee.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   108172 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-coldfusion.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    24006 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-crystal.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    16373 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-csharp.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   132801 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-csound_document.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    77245 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-csound_orchestra.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13998 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-csound_score.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2441 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-csp.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    32843 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-css.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   106237 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-curly.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    17075 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-d.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    26316 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-dart.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4735 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-diff.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   107179 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-django.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    17052 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-dockerfile.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13922 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-dot.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    19064 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-drools.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     5027 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-edifact.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     5062 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-eiffel.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   144552 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ejs.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    24911 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-elixir.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    10122 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-elm.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    49008 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-erlang.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    11968 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-forth.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    15322 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-fortran.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    10632 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-fsharp.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     9080 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-fsl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    58601 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ftl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2845 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-gcode.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     5201 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-gherkin.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1774 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-gitignore.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    22490 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-glsl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    51759 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-gobstones.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13323 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-golang.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     6912 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-graphqlschema.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    46189 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-groovy.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    85577 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-haml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   108056 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-handlebars.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    18131 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-haskell.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     5092 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-haskell_cabal.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    12186 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-haxe.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    12204 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-hjson.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   104651 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-html.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   131706 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-html_elixir.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   145130 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-html_ruby.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     5379 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ini.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     9524 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-io.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    16625 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ion.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    11047 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jack.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    88275 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jade.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    48080 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-java.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    37910 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-javascript.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    10095 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jexl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    10252 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-json.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    11437 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-json5.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   328142 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jsoniq.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    67999 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jsp.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    11431 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jssm.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13267 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jsx.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    12518 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-julia.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    16677 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-kotlin.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     9892 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-latex.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   111551 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-latte.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    36880 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-less.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   118491 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-liquid.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4065 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-lisp.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     9177 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-livescript.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    11080 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-logiql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    16647 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-logtalk.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    31691 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-lsl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    15676 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-lua.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   122028 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-luapage.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4917 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-lucene.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    14529 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-makefile.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   127937 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-markdown.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    78177 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mask.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    24470 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-matlab.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     9740 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-maze.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    22557 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mediawiki.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    29186 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mel.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     9748 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mips.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     5472 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mixal.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    16070 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mushcode.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    10613 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mysql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    20951 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-nginx.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13095 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-nim.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    24023 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-nix.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    15795 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-nsis.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   111224 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-nunjucks.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    78897 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-objectivec.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    21592 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ocaml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    15971 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-odin.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    26397 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-partiql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     8144 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-pascal.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13146 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-perl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    94248 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-pgsql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   637226 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-php.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   645311 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-php_laravel_blade.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    11799 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-pig.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1082 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-plain_text.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13191 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-plsql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    38871 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-powershell.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    17683 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-praat.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    17158 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-prisma.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    14894 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-prolog.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2359 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-properties.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    22506 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-protobuf.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    12836 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-puppet.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    16490 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-python.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    22356 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-qml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    15166 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-r.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    26335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-raku.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   118212 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-razor.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    11825 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-rdoc.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    20438 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-red.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13303 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-redshift.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   120988 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-rhtml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     7382 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-robot.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     7279 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-rst.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    39461 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ruby.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    16234 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-rust.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13123 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sac.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    24789 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sass.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    12768 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-scad.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    46231 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-scala.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     7813 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-scheme.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    12947 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-scrypt.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    38506 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-scss.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    15408 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sh.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    43886 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sjs.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   204703 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-slim.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   109900 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-smarty.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    17347 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-smithy.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     7382 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-snippets.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   118856 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-soy_template.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     5075 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-space.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13232 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sparql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     8538 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    24027 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sqlserver.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    22581 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-stylus.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    60659 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-svg.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13433 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-swift.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    12296 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-tcl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    13146 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-terraform.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     8823 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-tex.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      329 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-text.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4301 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-textile.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4417 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-toml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    41146 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-tsx.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    10037 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-turtle.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   110572 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-twig.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    40662 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-typescript.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    28600 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-vala.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    25160 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-vbscript.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   113544 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-velocity.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4672 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-verilog.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3870 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-vhdl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   109005 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-visualforce.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    42983 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-wollok.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    19613 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-xml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   325349 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-xquery.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    11025 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-yaml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    17787 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/mode-zeek.js
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-06-12 09:21:54.795644 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/abap.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1552 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/abc.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3830 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/actionscript.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/ada.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/alda.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      340 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/apache_conf.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/apex.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      340 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/applescript.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/aql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/asciidoc.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/asl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      341 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/assembly_x86.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/autohotkey.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      338 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/batchfile.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/bibtex.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/c9search.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3282 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/c_cpp.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/cirru.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2674 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/clojure.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/cobol.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2874 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/coffee.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/coldfusion.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/crystal.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/csharp.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      906 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/csound_document.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1713 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/csound_orchestra.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      341 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/csound_score.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/csp.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    20689 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/css.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/curly.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      330 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/d.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1928 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/dart.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1113 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/diff.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4645 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/django.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/dockerfile.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/dot.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      949 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/drools.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     5032 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/edifact.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/eiffel.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/ejs.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/elixir.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/elm.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4232 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/erlang.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/forth.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/fortran.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/fsharp.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      907 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/fsl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/ftl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/gcode.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/gherkin.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      338 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/gitignore.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/glsl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    40397 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/gobstones.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/golang.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1267 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/graphqlschema.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/groovy.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1030 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/haml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/handlebars.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2603 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/haskell.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      342 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/haskell_cabal.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/haxe.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/hjson.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    21108 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/html.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      340 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/html_elixir.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      338 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/html_ruby.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/ini.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2194 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/io.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/ion.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/jack.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/jade.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     5025 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/java.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4580 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/javascript.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/jexl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/json.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/json5.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2473 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/jsoniq.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3487 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/jsp.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/jssm.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/jsx.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/julia.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/kotlin.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/latex.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/latte.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/less.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    21495 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/liquid.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/lisp.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/livescript.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/logiql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/logtalk.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    36757 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/lsl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1073 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/lua.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/luapage.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/lucene.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      770 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/makefile.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2601 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/markdown.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/mask.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/matlab.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      824 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/maze.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      338 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/mediawiki.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/mel.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/mips.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/mixal.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/mushcode.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/mysql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/nginx.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/nim.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/nix.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/nsis.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/nunjucks.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/objectivec.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/ocaml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/odin.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/partiql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/pascal.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     6267 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/perl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/pgsql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     7825 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/php.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      346 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/php_laravel_blade.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/pig.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/plain_text.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/plsql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/powershell.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/praat.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/prisma.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/prolog.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/properties.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/protobuf.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/puppet.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4409 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/python.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/qml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3232 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/r.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/raku.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      721 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/razor.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/rdoc.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/red.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/redshift.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/rhtml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2186 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/robot.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1003 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/rst.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    22700 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/ruby.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/rust.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/sac.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/sass.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/scad.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/scala.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/scheme.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/scrypt.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/scss.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2688 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/sh.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/sjs.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/slim.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/smarty.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/smithy.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      872 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/snippets.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      341 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/soy_template.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/space.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/sparql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1517 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/sql.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2777 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/sqlserver.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/stylus.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/svg.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/swift.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2310 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/tcl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      338 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/terraform.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4308 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/tex.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/text.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1118 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/textile.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/toml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/tsx.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/turtle.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/twig.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/typescript.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     5346 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/vala.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/vbscript.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1253 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/velocity.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/verilog.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/vhdl.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      340 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/visualforce.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1871 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/wollok.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/xml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2473 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/xquery.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/yaml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/zeek.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    28832 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-ambiance.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3974 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-chaos.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3997 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-chrome.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4298 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-cloud9_day.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4401 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-cloud9_night.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4422 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-cloud9_night_low_color.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3251 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-clouds.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3547 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-clouds_midnight.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3479 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-cobalt.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4110 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-crimson_editor.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3446 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-dawn.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4954 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-dracula.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4509 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-dreamweaver.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3311 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-eclipse.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3640 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-github.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3927 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-github_dark.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3484 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-gob.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2702 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-gruvbox.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4176 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-gruvbox_dark_hard.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4533 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-gruvbox_light_hard.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3352 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-idle_fingers.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     7739 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-iplastic.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4697 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-katzenmilch.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3406 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-kr_theme.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3418 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-kuroir.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3313 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-merbivore.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3552 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-merbivore_soft.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3940 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-mono_industrial.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3474 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-monokai.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3045 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-nord_dark.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3972 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-one_dark.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3787 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-pastel_on_dark.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3390 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-solarized_dark.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3557 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-solarized_light.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4321 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-sqlserver.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4043 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-terminal.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)      714 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-textmate.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3764 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-tomorrow.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3956 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-tomorrow_night.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4184 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-tomorrow_night_blue.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4713 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-tomorrow_night_bright.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     4402 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-tomorrow_night_eighties.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3589 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-twilight.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3293 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-vibrant_ink.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3154 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/theme-xcode.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    44394 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/worker-base.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   350558 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/worker-coffee.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   315610 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/worker-css.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   317658 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/worker-html.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   732435 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/worker-javascript.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    52132 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/worker-json.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   105288 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/worker-lua.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   131952 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/worker-php.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)    92081 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/worker-xml.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)  3502484 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/worker-xquery.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)   166118 2023-06-12 09:19:14.000000 django-ace-1.22.1/django_ace/static/django_ace/ace/worker-yaml.js
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-06-12 09:21:54.795644 django-ace-1.22.1/django_ace/static/django_ace/img/
--rw-r--r--   0 mdk       (1000) mdk       (1000)      304 2019-12-04 21:51:14.000000 django-ace-1.22.1/django_ace/static/django_ace/img/contract.png
--rw-r--r--   0 mdk       (1000) mdk       (1000)      284 2019-12-04 21:51:14.000000 django-ace-1.22.1/django_ace/static/django_ace/img/expand.png
--rw-r--r--   0 mdk       (1000) mdk       (1000)     1147 2023-04-06 09:26:26.000000 django-ace-1.22.1/django_ace/static/django_ace/widget.css
--rw-r--r--   0 mdk       (1000) mdk       (1000)     7593 2022-05-12 21:24:24.000000 django-ace-1.22.1/django_ace/static/django_ace/widget.js
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3504 2020-11-10 10:17:21.000000 django-ace-1.22.1/django_ace/widgets.py
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-06-12 09:21:54.695649 django-ace-1.22.1/django_ace.egg-info/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3942 2023-06-12 09:21:54.000000 django-ace-1.22.1/django_ace.egg-info/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)    23103 2023-06-12 09:21:54.000000 django-ace-1.22.1/django_ace.egg-info/SOURCES.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-06-12 09:21:54.000000 django-ace-1.22.1/django_ace.egg-info/dependency_links.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       12 2023-06-12 09:21:54.000000 django-ace-1.22.1/django_ace.egg-info/requires.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       11 2023-06-12 09:21:54.000000 django-ace-1.22.1/django_ace.egg-info/top_level.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       90 2022-05-12 21:24:24.000000 django-ace-1.22.1/pyproject.toml
--rw-r--r--   0 mdk       (1000) mdk       (1000)      749 2023-06-12 09:21:54.799644 django-ace-1.22.1/setup.cfg
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-14 13:16:27.091855 django-ace-1.23.4/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     5388 2020-10-04 15:07:59.000000 django-ace-1.23.4/LICENCE
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       65 2019-12-04 21:51:14.000000 django-ace-1.23.4/MANIFEST.in
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4000 2023-07-14 13:16:27.091855 django-ace-1.23.4/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3400 2023-07-14 13:15:46.000000 django-ace-1.23.4/README.rst
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-14 13:16:27.003855 django-ace-1.23.4/django_ace/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       75 2023-07-14 13:15:50.000000 django-ace-1.23.4/django_ace/__init__.py
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-14 13:16:26.999855 django-ace-1.23.4/django_ace/static/
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-14 13:16:27.003855 django-ace-1.23.4/django_ace/static/django_ace/
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-14 13:16:27.067855 django-ace-1.23.4/django_ace/static/django_ace/ace/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   844902 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ace.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13362 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-beautify.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     8185 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-code_lens.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    21729 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-command_bar.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     9282 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-elastic_tabstops_lite.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    51049 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-emmet.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-error_marker.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4368 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-hardwrap.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   131261 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-inline_autocomplete.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     6741 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-keybinding_menu.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    96125 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-language_tools.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2007 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-linking.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     7041 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-modelist.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    26460 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-options.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   115971 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-prompt.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4640 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-rtl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    18380 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-searchbox.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    27373 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-settings_menu.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2521 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-spellcheck.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     6546 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-split.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     7487 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-static_highlight.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1966 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-statusbar.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    12776 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-textarea.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2480 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-themelist.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     6755 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/ext-whitespace.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    43079 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/keybinding-emacs.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    12833 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/keybinding-sublime.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   251788 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/keybinding-vim.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     9188 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/keybinding-vscode.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     9492 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-abap.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     9449 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-abc.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    25355 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-actionscript.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4323 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ada.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    10523 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-alda.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    19937 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-apache_conf.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    15658 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-apex.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     9813 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-applescript.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     5601 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-aql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    14224 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-asciidoc.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    14861 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-asl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    12287 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-assembly_x86.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    67779 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-autohotkey.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     8835 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-batchfile.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    11316 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-bibtex.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     9836 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-c9search.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    19561 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-c_cpp.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     6577 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-cirru.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    14162 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-clojure.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3775 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-cobol.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13889 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-coffee.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   108172 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-coldfusion.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    24006 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-crystal.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    16373 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-csharp.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   132801 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-csound_document.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    77245 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-csound_orchestra.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13998 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-csound_score.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2441 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-csp.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    32843 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-css.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   106237 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-curly.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    17075 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-d.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    26316 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-dart.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4735 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-diff.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   107179 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-django.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    17052 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-dockerfile.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13922 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-dot.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    19064 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-drools.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     5027 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-edifact.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     5062 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-eiffel.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   144552 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ejs.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    24911 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-elixir.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    10122 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-elm.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    49008 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-erlang.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    11968 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-forth.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    15322 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-fortran.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    10632 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-fsharp.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     9080 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-fsl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    58601 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ftl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2845 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-gcode.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     5201 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-gherkin.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1774 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-gitignore.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    22490 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-glsl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    51759 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-gobstones.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13323 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-golang.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     6912 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-graphqlschema.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    46189 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-groovy.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    85577 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-haml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   108056 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-handlebars.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    18131 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-haskell.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     5092 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-haskell_cabal.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    12186 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-haxe.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    12204 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-hjson.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   104651 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-html.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   131706 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-html_elixir.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   145130 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-html_ruby.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     5379 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ini.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     9524 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-io.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    16625 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ion.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    11047 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jack.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    88275 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jade.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    48080 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-java.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    37910 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-javascript.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    10095 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jexl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    10252 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-json.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    11437 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-json5.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   328142 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jsoniq.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    67999 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jsp.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    11431 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jssm.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13267 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jsx.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    12518 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-julia.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    16677 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-kotlin.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     9892 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-latex.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   111551 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-latte.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    36880 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-less.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   118491 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-liquid.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4065 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-lisp.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     9177 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-livescript.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    11080 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-logiql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    16647 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-logtalk.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    31691 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-lsl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    15676 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-lua.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   122028 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-luapage.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4917 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-lucene.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    14529 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-makefile.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   127937 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-markdown.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    78177 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mask.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    24470 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-matlab.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     9740 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-maze.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    22557 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mediawiki.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    29186 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mel.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     9748 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mips.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     5472 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mixal.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    16070 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mushcode.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    10613 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mysql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    20951 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-nginx.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13095 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-nim.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    24023 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-nix.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    15802 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-nsis.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   111224 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-nunjucks.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    78897 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-objectivec.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    21592 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ocaml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    15971 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-odin.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    26397 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-partiql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     8144 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-pascal.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13146 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-perl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    94248 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-pgsql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   637226 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-php.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   645311 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-php_laravel_blade.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    11799 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-pig.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1082 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-plain_text.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13191 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-plsql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    38871 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-powershell.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    17683 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-praat.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    17158 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-prisma.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    14894 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-prolog.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2359 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-properties.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    22506 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-protobuf.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    12836 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-puppet.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    16490 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-python.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    22356 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-qml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    15166 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-r.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    26335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-raku.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   118212 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-razor.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    11825 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-rdoc.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    20438 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-red.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13303 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-redshift.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   120988 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-rhtml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     7382 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-robot.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     7279 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-rst.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    39461 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ruby.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    16234 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-rust.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13123 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sac.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    24789 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sass.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    12768 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-scad.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    46231 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-scala.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     7813 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-scheme.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    12947 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-scrypt.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    38506 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-scss.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    15408 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sh.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    43886 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sjs.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   204703 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-slim.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   109900 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-smarty.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    17347 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-smithy.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     7382 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-snippets.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   118856 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-soy_template.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     5075 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-space.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13232 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sparql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     8538 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    24027 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sqlserver.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    22581 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-stylus.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    60659 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-svg.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13433 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-swift.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    12296 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-tcl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    13146 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-terraform.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     8823 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-tex.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      329 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-text.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4301 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-textile.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4417 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-toml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    41146 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-tsx.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    10037 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-turtle.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   110572 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-twig.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    40662 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-typescript.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    28600 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-vala.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    25160 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-vbscript.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   113544 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-velocity.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4672 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-verilog.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3870 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-vhdl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   109005 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-visualforce.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    42983 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-wollok.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    19613 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-xml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   325349 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-xquery.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    11025 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-yaml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    17787 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/mode-zeek.js
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-14 13:16:27.091855 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/abap.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1552 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/abc.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3830 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/actionscript.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/ada.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/alda.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      340 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/apache_conf.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/apex.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      340 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/applescript.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/aql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/asciidoc.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/asl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      341 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/assembly_x86.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/autohotkey.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      338 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/batchfile.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/bibtex.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/c9search.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3282 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/c_cpp.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/cirru.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2674 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/clojure.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/cobol.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2874 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/coffee.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/coldfusion.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/crystal.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/csharp.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      906 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/csound_document.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1713 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/csound_orchestra.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      341 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/csound_score.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/csp.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    20689 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/css.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/curly.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      330 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/d.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1928 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/dart.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1113 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/diff.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4645 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/django.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/dockerfile.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/dot.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      949 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/drools.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     5032 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/edifact.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/eiffel.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/ejs.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/elixir.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/elm.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4232 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/erlang.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/forth.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/fortran.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/fsharp.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      907 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/fsl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/ftl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/gcode.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/gherkin.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      338 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/gitignore.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/glsl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    40397 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/gobstones.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/golang.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1267 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/graphqlschema.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/groovy.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1030 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/haml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/handlebars.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2603 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/haskell.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      342 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/haskell_cabal.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/haxe.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/hjson.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    21108 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/html.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      340 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/html_elixir.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      338 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/html_ruby.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/ini.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2194 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/io.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/ion.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/jack.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/jade.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     5025 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/java.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4580 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/javascript.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/jexl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/json.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/json5.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2473 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/jsoniq.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3487 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/jsp.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/jssm.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/jsx.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/julia.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/kotlin.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/latex.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/latte.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/less.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    21495 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/liquid.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/lisp.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/livescript.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/logiql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/logtalk.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    36757 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/lsl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1073 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/lua.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/luapage.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/lucene.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      770 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/makefile.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2601 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/markdown.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/mask.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/matlab.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      824 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/maze.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      338 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/mediawiki.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/mel.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/mips.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/mixal.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/mushcode.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/mysql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/nginx.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/nim.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/nix.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/nsis.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/nunjucks.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/objectivec.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/ocaml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/odin.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/partiql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/pascal.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     6267 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/perl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/pgsql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     7825 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/php.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      346 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/php_laravel_blade.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/pig.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/plain_text.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/plsql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/powershell.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/praat.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/prisma.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/prolog.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/properties.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/protobuf.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/puppet.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4409 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/python.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/qml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3232 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/r.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/raku.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      721 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/razor.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/rdoc.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/red.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/redshift.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/rhtml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2186 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/robot.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1003 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/rst.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    22700 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/ruby.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/rust.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/sac.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/sass.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/scad.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/scala.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/scheme.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/scrypt.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/scss.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2688 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/sh.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/sjs.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/slim.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/smarty.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/smithy.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      872 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/snippets.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      341 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/soy_template.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/space.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/sparql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1517 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/sql.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2777 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/sqlserver.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/stylus.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/svg.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      334 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/swift.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2310 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/tcl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      338 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/terraform.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4308 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/tex.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/text.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1118 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/textile.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/toml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/tsx.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      335 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/turtle.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/twig.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      339 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/typescript.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     5346 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/vala.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      337 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/vbscript.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1253 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/velocity.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      336 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/verilog.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/vhdl.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      340 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/visualforce.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1871 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/wollok.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      332 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/xml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2473 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/xquery.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/yaml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      333 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/zeek.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    28832 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-ambiance.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3974 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-chaos.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3997 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-chrome.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4298 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-cloud9_day.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4401 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-cloud9_night.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4422 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-cloud9_night_low_color.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3251 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-clouds.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3547 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-clouds_midnight.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3479 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-cobalt.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4110 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-crimson_editor.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3446 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-dawn.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4954 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-dracula.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4509 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-dreamweaver.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3311 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-eclipse.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3640 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-github.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3927 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-github_dark.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3484 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-gob.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2702 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-gruvbox.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4176 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-gruvbox_dark_hard.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4533 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-gruvbox_light_hard.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3352 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-idle_fingers.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     7739 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-iplastic.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4697 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-katzenmilch.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3406 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-kr_theme.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3418 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-kuroir.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3313 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-merbivore.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3552 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-merbivore_soft.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3940 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-mono_industrial.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3474 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-monokai.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3045 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-nord_dark.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3972 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-one_dark.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3787 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-pastel_on_dark.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3390 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-solarized_dark.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3557 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-solarized_light.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4321 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-sqlserver.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4043 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-terminal.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      714 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-textmate.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3764 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-tomorrow.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3956 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-tomorrow_night.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4184 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-tomorrow_night_blue.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4713 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-tomorrow_night_bright.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4402 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-tomorrow_night_eighties.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3589 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-twilight.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3293 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-vibrant_ink.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3154 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/theme-xcode.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    44394 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/worker-base.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   350558 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/worker-coffee.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   315610 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/worker-css.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   317658 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/worker-html.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   732433 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/worker-javascript.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    52132 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/worker-json.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   105288 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/worker-lua.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   131952 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/worker-php.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    92081 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/worker-xml.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)  3502484 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/worker-xquery.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)   166118 2023-07-14 13:12:34.000000 django-ace-1.23.4/django_ace/static/django_ace/ace/worker-yaml.js
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-14 13:16:27.091855 django-ace-1.23.4/django_ace/static/django_ace/img/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      304 2019-12-04 21:51:14.000000 django-ace-1.23.4/django_ace/static/django_ace/img/contract.png
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      284 2019-12-04 21:51:14.000000 django-ace-1.23.4/django_ace/static/django_ace/img/expand.png
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     1147 2023-04-06 09:26:26.000000 django-ace-1.23.4/django_ace/static/django_ace/widget.css
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     7593 2022-05-12 21:24:24.000000 django-ace-1.23.4/django_ace/static/django_ace/widget.js
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3504 2020-11-10 10:17:21.000000 django-ace-1.23.4/django_ace/widgets.py
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-07-14 13:16:27.003855 django-ace-1.23.4/django_ace.egg-info/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     4000 2023-07-14 13:16:26.000000 django-ace-1.23.4/django_ace.egg-info/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    23103 2023-07-14 13:16:26.000000 django-ace-1.23.4/django_ace.egg-info/SOURCES.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-07-14 13:16:26.000000 django-ace-1.23.4/django_ace.egg-info/dependency_links.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       12 2023-07-14 13:16:26.000000 django-ace-1.23.4/django_ace.egg-info/requires.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       11 2023-07-14 13:16:26.000000 django-ace-1.23.4/django_ace.egg-info/top_level.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       90 2022-05-12 21:24:24.000000 django-ace-1.23.4/pyproject.toml
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      749 2023-07-14 13:16:27.091855 django-ace-1.23.4/setup.cfg
```

### Comparing `django-ace-1.22.1/LICENCE` & `django-ace-1.23.4/LICENCE`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/PKG-INFO` & `django-ace-1.23.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ace
-Version: 1.22.1
+Version: 1.23.4
 Summary: django-ace provides integration for ajax.org ACE with Django
 Home-page: https://github.com/django-ace/django-ace
 Author: Bradley Ayers
 Author-email: bradley.ayers@gmail.com
 License: Simplified BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -95,14 +95,19 @@
 
 Then browser to ``http://localhost:8000``.
 
 
 Change log
 ==========
 
+v1.23.4
+-------
+
+- Update ACE editor to version v1.23.4.
+
 v1.22.1
 -------
 
 - Update ACE editor to version v1.22.1.
 
 v1.19.0
 -------
```

### Comparing `django-ace-1.22.1/README.rst` & `django-ace-1.23.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,19 @@
 
 Then browser to ``http://localhost:8000``.
 
 
 Change log
 ==========
 
+v1.23.4
+-------
+
+- Update ACE editor to version v1.23.4.
+
 v1.22.1
 -------
 
 - Update ACE editor to version v1.22.1.
 
 v1.19.0
 -------
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ace.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ace.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1064,14 +1064,17 @@
                 this.setDefaultValue(path, key, optionHash[key]);
             }, this);
         };
         AppConfig.prototype.setMessages = function(value) {
             messages = value;
         };
         AppConfig.prototype.nls = function(string, params) {
+            if (messages && !messages[string]) {
+                warn("No message found for '" + string + "' in the provided messages, falling back to default English message.");
+            }
             var translated = messages && messages[string] || string;
             if (params) {
                 translated = translated.replace(/\$(\$|[\d]+)/g, function(_, name) {
                     if (name == "$")
                         return "$";
                     return params[name];
                 });
@@ -1083,24 +1086,24 @@
     AppConfig.prototype.warn = warn;
     AppConfig.prototype.reportError = reportError;
     oop.implement(AppConfig.prototype, EventEmitter);
     exports.AppConfig = AppConfig;
 
 });
 
-define("ace/theme/textmate.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/textmate-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-tm .ace_gutter {\n  background: #f0f0f0;\n  color: #333;\n}\n\n.ace-tm .ace_print-margin {\n  width: 1px;\n  background: #e8e8e8;\n}\n\n.ace-tm .ace_fold {\n    background-color: #6B72E6;\n}\n\n.ace-tm {\n  background-color: #FFFFFF;\n  color: black;\n}\n\n.ace-tm .ace_cursor {\n  color: black;\n}\n        \n.ace-tm .ace_invisible {\n  color: rgb(191, 191, 191);\n}\n\n.ace-tm .ace_storage,\n.ace-tm .ace_keyword {\n  color: blue;\n}\n\n.ace-tm .ace_constant {\n  color: rgb(197, 6, 11);\n}\n\n.ace-tm .ace_constant.ace_buildin {\n  color: rgb(88, 72, 246);\n}\n\n.ace-tm .ace_constant.ace_language {\n  color: rgb(88, 92, 246);\n}\n\n.ace-tm .ace_constant.ace_library {\n  color: rgb(6, 150, 14);\n}\n\n.ace-tm .ace_invalid {\n  background-color: rgba(255, 0, 0, 0.1);\n  color: red;\n}\n\n.ace-tm .ace_support.ace_function {\n  color: rgb(60, 76, 114);\n}\n\n.ace-tm .ace_support.ace_constant {\n  color: rgb(6, 150, 14);\n}\n\n.ace-tm .ace_support.ace_type,\n.ace-tm .ace_support.ace_class {\n  color: rgb(109, 121, 222);\n}\n\n.ace-tm .ace_keyword.ace_operator {\n  color: rgb(104, 118, 135);\n}\n\n.ace-tm .ace_string {\n  color: rgb(3, 106, 7);\n}\n\n.ace-tm .ace_comment {\n  color: rgb(76, 136, 107);\n}\n\n.ace-tm .ace_comment.ace_doc {\n  color: rgb(0, 102, 255);\n}\n\n.ace-tm .ace_comment.ace_doc.ace_tag {\n  color: rgb(128, 159, 191);\n}\n\n.ace-tm .ace_constant.ace_numeric {\n  color: rgb(0, 0, 205);\n}\n\n.ace-tm .ace_variable {\n  color: rgb(49, 132, 149);\n}\n\n.ace-tm .ace_xml-pe {\n  color: rgb(104, 104, 91);\n}\n\n.ace-tm .ace_entity.ace_name.ace_function {\n  color: #0000A2;\n}\n\n\n.ace-tm .ace_heading {\n  color: rgb(12, 7, 255);\n}\n\n.ace-tm .ace_list {\n  color:rgb(185, 6, 144);\n}\n\n.ace-tm .ace_meta.ace_tag {\n  color:rgb(0, 22, 142);\n}\n\n.ace-tm .ace_string.ace_regex {\n  color: rgb(255, 0, 0)\n}\n\n.ace-tm .ace_marker-layer .ace_selection {\n  background: rgb(181, 213, 255);\n}\n.ace-tm.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px white;\n}\n.ace-tm .ace_marker-layer .ace_step {\n  background: rgb(252, 255, 0);\n}\n\n.ace-tm .ace_marker-layer .ace_stack {\n  background: rgb(164, 229, 101);\n}\n\n.ace-tm .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgb(192, 192, 192);\n}\n\n.ace-tm .ace_marker-layer .ace_active-line {\n  background: rgba(0, 0, 0, 0.07);\n}\n\n.ace-tm .ace_gutter-active-line {\n    background-color : #dcdcdc;\n}\n\n.ace-tm .ace_marker-layer .ace_selected-word {\n  background: rgb(250, 250, 255);\n  border: 1px solid rgb(200, 200, 250);\n}\n\n.ace-tm .ace_indent-guide {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bLly//BwAmVgd1/w11/gAAAABJRU5ErkJggg==\") right repeat-y;\n}\n\n.ace-tm .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/textmate", ["require", "exports", "module", "ace/theme/textmate.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/textmate", ["require", "exports", "module", "ace/theme/textmate-css", "ace/lib/dom"], function(require, exports, module) {
     "use strict";
     exports.isDark = false;
     exports.cssClass = "ace-tm";
-    exports.cssText = require("./textmate.css");
+    exports.cssText = require("./textmate-css");
     exports.$id = "ace/theme/textmate";
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 
 define("ace/config", ["require", "exports", "module", "ace/lib/lang", "ace/lib/net", "ace/lib/dom", "ace/lib/app_config", "ace/theme/textmate"], function(require, exports, module) {
@@ -1164,37 +1167,43 @@
     };
     exports.setModuleUrl = function(name, subst) {
         return options.$moduleUrls[name] = subst;
     };
     var loader = function(moduleName, cb) {
         if (moduleName === "ace/theme/textmate" || moduleName === "./theme/textmate")
             return cb(null, require("./theme/textmate"));
-        return console.error("loader is not configured");
+        if (customLoader)
+            return customLoader(moduleName, cb);
+        console.error("loader is not configured");
     };
+    var customLoader;
     exports.setLoader = function(cb) {
-        loader = cb;
+        customLoader = cb;
     };
     exports.dynamicModules = Object.create(null);
     exports.$loading = {};
+    exports.$loaded = {};
     exports.loadModule = function(moduleName, onLoad) {
-        var module, moduleType;
+        var loadedModule, moduleType;
         if (Array.isArray(moduleName)) {
             moduleType = moduleName[0];
             moduleName = moduleName[1];
         }
         var load = function(module) {
             if (module && !exports.$loading[moduleName])
                 return onLoad && onLoad(module);
             if (!exports.$loading[moduleName])
                 exports.$loading[moduleName] = [];
             exports.$loading[moduleName].push(onLoad);
             if (exports.$loading[moduleName].length > 1)
                 return;
             var afterLoad = function() {
                 loader(moduleName, function(err, module) {
+                    if (module)
+                        exports.$loaded[moduleName] = module;
                     exports._emit("load.module", {
                         name: moduleName,
                         module: module
                     });
                     var listeners = exports.$loading[moduleName];
                     exports.$loading[moduleName] = null;
                     listeners.forEach(function(onLoad) {
@@ -1213,31 +1222,37 @@
                     load(module.default);
                 } else {
                     load(module);
                 }
             });
         } else {
             try {
-                module = require(moduleName);
+                loadedModule = this.$require(moduleName);
             } catch (e) {}
-            load(module);
+            load(loadedModule || exports.$loaded[moduleName]);
+        }
+    };
+    exports.$require = function(moduleName) {
+        if (typeof module.require == "function") {
+            var req = "require";
+            return module[req](moduleName);
         }
     };
     exports.setModuleLoader = function(moduleName, onLoad) {
         exports.dynamicModules[moduleName] = onLoad;
     };
     var reportErrorIfPathIsNotConfigured = function() {
         if (!options.basePath && !options.workerPath &&
             !options.modePath && !options.themePath &&
             !Object.keys(options.$moduleUrls).length) {
             console.error("Unable to infer path to ace from script src,", "use ace.config.set('basePath', 'path') to enable dynamic loading of modes and themes", "or with webpack use ace/webpack-resolver");
             reportErrorIfPathIsNotConfigured = function() {};
         }
     };
-    exports.version = "1.22.1";
+    exports.version = "1.23.4";
 
 });
 
 define("ace/loader_build", ["require", "exports", "module", "ace/lib/fixoldbrowsers", "ace/config"], function(require, exports, module) {
     "use strict";
 
     require("./lib/fixoldbrowsers");
@@ -1250,14 +1265,15 @@
 
     var global = (function() {
         return this || typeof window != "undefined" && window;
     })();
 
     module.exports = function(ace) {
         config.init = init;
+        config.$require = require;
         ace.require = require;
 
         if (typeof define === "function")
             ace.define = define;
     };
     init(true);
 
@@ -1739,14 +1755,15 @@
             }
         })();
         ret.KEY_MODS[0] = "";
         ret.KEY_MODS[-1] = "input-";
         return ret;
     })();
     oop.mixin(exports, Keys);
+    exports.default = exports;
     exports.keyCodeToString = function(keyCode) {
         var keyString = Keys[keyCode];
         if (typeof keyString != "string")
             keyString = String.fromCharCode(keyCode);
         return keyString.toLowerCase();
     };
 
@@ -2127,16 +2144,14 @@
         });
         this.setAriaLabel();
         event.addListener(text, "blur", function(e) {
             if (ignoreFocusEvents)
                 return;
             host.onBlur(e);
             isFocused = false;
-            if (isMobile && !isIOS)
-                document.removeEventListener("selectionchange", detectSelectionChange);
         }, host);
         event.addListener(text, "focus", function(e) {
             if (ignoreFocusEvents)
                 return;
             isFocused = true;
             if (useragent.isEdge) {
                 try {
@@ -2145,16 +2160,14 @@
                 } catch (e) {}
             }
             host.onFocus(e);
             if (useragent.isEdge)
                 setTimeout(resetSelection);
             else
                 resetSelection();
-            if (isMobile && !isIOS)
-                document.addEventListener("selectionchange", detectSelectionChange);
         }, host);
         this.$focusScroll = false;
         this.focus = function() {
             this.setAriaLabel();
             if (tempStyle || HAS_FOCUS_ARGS || this.$focusScroll == "browser")
                 return text.focus({
                     preventScroll: true
@@ -2310,35 +2323,14 @@
             } else if (isAllSelected(text)) {
                 host.selectAll();
                 resetSelection();
             } else if (isMobile && text.selectionStart != lastSelectionStart) {
                 resetSelection();
             }
         };
-
-        function detectSelectionChange(e) {
-            if (!text || !text.parentNode)
-                document.removeEventListener("selectionchange", detectSelectionChange);
-            if (inComposition)
-                return;
-            if (text.selectionStart !== text.selectionEnd)
-                return;
-            var startDiff = text.selectionStart - lastSelectionStart;
-            var oldLenght = lastSelectionEnd - lastSelectionStart;
-            if (startDiff > 0) {
-                startDiff = Math.max(startDiff - oldLenght, 1);
-            } else if (startDiff === 0 && oldLenght) {
-                startDiff = -1;
-            }
-            var repeat = Math.abs(startDiff);
-            var key = startDiff > 0 ? KEYS.right : KEYS.left;
-            for (var i = 0; i < repeat; i++) {
-                host.onCommandKey({}, 0, key);
-            }
-        }
         var inputHandler = null;
         this.setInputHandler = function(cb) {
             inputHandler = cb;
         };
         this.getInputHandler = function() {
             return inputHandler;
         };
@@ -3442,28 +3434,33 @@
             tooltip.showTooltip(row);
             if (!tooltip.isOpen)
                 return;
             editor.on("mousewheel", hideTooltip);
             if (mouseHandler.$tooltipFollowsMouse) {
                 moveTooltip(mouseEvent);
             } else {
-                var gutterElement = gutter.$lines.cells[row].element.querySelector("[class*=ace_icon]");
-                var rect = gutterElement.getBoundingClientRect();
-                var style = tooltip.getElement().style;
-                style.left = rect.right + "px";
-                style.top = rect.bottom + "px";
+                var gutterRow = mouseEvent.getGutterRow();
+                var gutterCell = gutter.$lines.get(gutterRow);
+                if (gutterCell) {
+                    var gutterElement = gutterCell.element.querySelector(".ace_gutter_annotation");
+                    var rect = gutterElement.getBoundingClientRect();
+                    var style = tooltip.getElement().style;
+                    style.left = rect.right + "px";
+                    style.top = rect.bottom + "px";
+                } else {
+                    moveTooltip(mouseEvent);
+                }
             }
         }
 
         function hideTooltip() {
             if (tooltipTimeout)
                 tooltipTimeout = clearTimeout(tooltipTimeout);
             if (tooltip.isOpen) {
-                tooltip.hide();
-                editor._signal("hideGutterTooltip", tooltip);
+                tooltip.hideTooltip();
                 editor.off("mousewheel", hideTooltip);
             }
         }
 
         function moveTooltip(e) {
             tooltip.setPosition(e.x, e.y);
         }
@@ -3594,21 +3591,26 @@
             var iconClassName = gutter.$useSvgGutterIcons ? "ace_icon_svg" : "ace_icon";
             for (var i = 0; i < annotation.text.length; i++) {
                 var line = "<span class='ace_".concat(annotation.type[i], " ").concat(iconClassName, "' aria-label='").concat(GutterTooltip.annotationLabels[annotation.type[i].replace("_fold", "")].singular, "' role=img> </span> ").concat(annotation.text[i]);
                 annotationMessages[annotation.type[i].replace("_fold", "")].push(line);
             }
             var tooltipContent = [].concat(annotationMessages.error, annotationMessages.warning, annotationMessages.info).join("<br>");
             this.setHtml(tooltipContent);
-            this.setClassName("ace_gutter-tooltip");
             this.$element.setAttribute("aria-live", "polite");
             if (!this.isOpen) {
                 this.setTheme(this.editor.renderer.theme);
+                this.setClassName("ace_gutter-tooltip");
             }
-            this.editor._signal("showGutterTooltip", this);
             this.show();
+            this.editor._signal("showGutterTooltip", this);
+        };
+        GutterTooltip.prototype.hideTooltip = function() {
+            this.$element.removeAttribute("aria-live");
+            this.hide();
+            this.editor._signal("hideGutterTooltip", this);
         };
         GutterTooltip.annotationsToSummaryString = function(annotations) {
             var e_1, _a;
             var summary = [];
             var annotationTypes = ['error', 'warning', 'info'];
             try {
                 for (var annotationTypes_1 = __values(annotationTypes), annotationTypes_1_1 = annotationTypes_1.next(); !annotationTypes_1_1.done; annotationTypes_1_1 = annotationTypes_1.next()) {
@@ -3666,14 +3668,20 @@
         };
         MouseEvent.prototype.getDocumentPosition = function() {
             if (this.$pos)
                 return this.$pos;
             this.$pos = this.editor.renderer.screenToTextCoordinates(this.clientX, this.clientY);
             return this.$pos;
         };
+        MouseEvent.prototype.getGutterRow = function() {
+            var documentRow = this.getDocumentPosition().row;
+            var screenRow = this.editor.session.documentToScreenRow(documentRow, 0);
+            var screenTopRow = this.editor.session.documentToScreenRow(this.editor.renderer.$gutterLayer.$lines.get(0).row, 0);
+            return screenRow - screenTopRow;
+        };
         MouseEvent.prototype.inSelection = function() {
             if (this.$inSelection !== null)
                 return this.$inSelection;
             var editor = this.editor;
             var selectionRange = editor.getSelectionRange();
             if (selectionRange.isEmpty())
                 this.$inSelection = false;
@@ -13233,15 +13241,15 @@
             this.element.removeEventListener("focusout", this.$blurGutter.bind(this));
             this.editor.off("mousewheel", this.$blurGutter.bind(this));
         };
         GutterKeyboardHandler.prototype.$onGutterKeyDown = function(e) {
             if (this.annotationTooltip.isOpen) {
                 e.preventDefault();
                 if (e.keyCode === keys["escape"])
-                    this.annotationTooltip.hide();
+                    this.annotationTooltip.hideTooltip();
                 return;
             }
             if (e.target === this.element) {
                 if (e.keyCode != keys["enter"]) {
                     return;
                 }
                 e.preventDefault();
@@ -13276,14 +13284,20 @@
                         this.activeLane = "fold";
                         this.$focusFoldWidget(this.activeRowIndex);
                         return;
                     }
                 }.bind(this), 10);
                 return;
             }
+            this.$handleGutterKeyboardInteraction(e);
+            setTimeout(function() {
+                this.editor._signal("gutterkeydown", new GutterKeyboardEvent(e, this));
+            }.bind(this), 10);
+        };
+        GutterKeyboardHandler.prototype.$handleGutterKeyboardInteraction = function(e) {
             if (e.keyCode === keys["tab"]) {
                 e.preventDefault();
                 return;
             }
             if (e.keyCode === keys["escape"]) {
                 e.preventDefault();
                 this.$blurGutter();
@@ -13314,18 +13328,20 @@
                         break;
                 }
                 return;
             }
             if (e.keyCode === keys["left"]) {
                 e.preventDefault();
                 this.$switchLane("annotation");
+                return;
             }
             if (e.keyCode === keys["right"]) {
                 e.preventDefault();
                 this.$switchLane("fold");
+                return;
             }
             if (e.keyCode === keys["enter"] || e.keyCode === keys["space"]) {
                 e.preventDefault();
                 switch (this.activeLane) {
                     case "fold":
                         if (this.gutterLayer.session.foldWidgets[this.$rowIndexToRow(this.activeRowIndex)] === 'start') {
                             var rowFoldingWidget = this.$rowIndexToRow(this.activeRowIndex);
@@ -13362,15 +13378,15 @@
                         break;
                     case "annotation":
                         this.$blurAnnotation(this.activeRowIndex);
                         break;
                 }
             }
             if (this.annotationTooltip.isOpen)
-                this.annotationTooltip.hide();
+                this.annotationTooltip.hideTooltip();
             return;
         };
         GutterKeyboardHandler.prototype.$isFoldWidgetVisible = function(index) {
             var isRowFullyVisible = this.editor.isRowFullyVisible(this.$rowIndexToRow(index));
             var isIconVisible = this.$getFoldWidget(index).style.display !== "none";
             return isRowFullyVisible && isIconVisible;
         };
@@ -13423,26 +13439,24 @@
             foldWidget.focus();
         };
         GutterKeyboardHandler.prototype.$focusAnnotation = function(index) {
             if (index == null)
                 return;
             var annotation = this.$getAnnotation(index);
             annotation.classList.add(this.editor.renderer.keyboardFocusClassName);
-            annotation.setAttribute("role", "button");
             annotation.focus();
         };
         GutterKeyboardHandler.prototype.$blurFoldWidget = function(index) {
             var foldWidget = this.$getFoldWidget(index);
             foldWidget.classList.remove(this.editor.renderer.keyboardFocusClassName);
             foldWidget.blur();
         };
         GutterKeyboardHandler.prototype.$blurAnnotation = function(index) {
             var annotation = this.$getAnnotation(index);
             annotation.classList.remove(this.editor.renderer.keyboardFocusClassName);
-            annotation.removeAttribute("role");
             annotation.blur();
         };
         GutterKeyboardHandler.prototype.$moveFoldWidgetUp = function() {
             var index = this.activeRowIndex;
             while (index > 0) {
                 index--;
                 if (this.$isFoldWidgetVisible(index)) {
@@ -13537,14 +13551,34 @@
                     return i;
             }
             return null;
         };
         return GutterKeyboardHandler;
     }());
     exports.GutterKeyboardHandler = GutterKeyboardHandler;
+    var GutterKeyboardEvent = /** @class */ (function() {
+        function GutterKeyboardEvent(domEvent, gutterKeyboardHandler) {
+            this.gutterKeyboardHandler = gutterKeyboardHandler;
+            this.domEvent = domEvent;
+        }
+        GutterKeyboardEvent.prototype.getKey = function() {
+            return keys.keyCodeToString(this.domEvent.keyCode);
+        };
+        GutterKeyboardEvent.prototype.getRow = function() {
+            return this.gutterKeyboardHandler.$rowIndexToRow(this.gutterKeyboardHandler.activeRowIndex);
+        };
+        GutterKeyboardEvent.prototype.isInAnnotationLane = function() {
+            return this.gutterKeyboardHandler.activeLane === "annotation";
+        };
+        GutterKeyboardEvent.prototype.isInFoldLane = function() {
+            return this.gutterKeyboardHandler.activeLane === "fold";
+        };
+        return GutterKeyboardEvent;
+    }());
+    exports.GutterKeyboardEvent = GutterKeyboardEvent;
 
 });
 
 define("ace/editor", ["require", "exports", "module", "ace/lib/oop", "ace/lib/dom", "ace/lib/lang", "ace/lib/useragent", "ace/keyboard/textinput", "ace/mouse/mouse_handler", "ace/mouse/fold_handler", "ace/keyboard/keybinding", "ace/edit_session", "ace/search", "ace/range", "ace/lib/event_emitter", "ace/commands/command_manager", "ace/commands/default_commands", "ace/config", "ace/token_iterator", "ace/line_widgets", "ace/keyboard/gutter_handler", "ace/config", "ace/clipboard", "ace/lib/keys"], function(require, exports, module) {
     "use strict";
     var __values = (this && this.__values) || function(o) {
         var s = typeof Symbol === "function" && Symbol.iterator,
@@ -16440,26 +16474,25 @@
             }
             if (breakpoints[row])
                 className += breakpoints[row];
             if (decorations[row])
                 className += decorations[row];
             if (this.$annotations[row] && row !== foldStart)
                 className += this.$annotations[row].className;
-            if (element.className != className)
-                element.className = className;
             if (foldWidgets) {
                 var c = foldWidgets[row];
                 if (c == null)
                     c = foldWidgets[row] = session.getFoldWidget(row);
             }
             if (c) {
-                var className = "ace_fold-widget ace_" + c;
-                if (c == "start" && row == foldStart && row < fold.end.row) {
-                    className += " ace_closed";
-                    var foldAnnotationClass;
+                var foldClass = "ace_fold-widget ace_" + c;
+                var isClosedFold = c == "start" && row == foldStart && row < fold.end.row;
+                if (isClosedFold) {
+                    foldClass += " ace_closed";
+                    var foldAnnotationClass = '';
                     var annotationInFold = false;
                     for (var i = row + 1; i <= fold.end.row; i++) {
                         if (!this.$annotations[i])
                             continue;
                         if (this.$annotations[i].className === " ace_error") {
                             annotationInFold = true;
                             foldAnnotationClass = " ace_error_fold";
@@ -16467,29 +16500,37 @@
                         }
                         if (this.$annotations[i].className === " ace_warning") {
                             annotationInFold = true;
                             foldAnnotationClass = " ace_warning_fold";
                             continue;
                         }
                     }
-                    element.className += foldAnnotationClass;
+                    className += foldAnnotationClass;
                 } else
-                    className += " ace_open";
-                if (foldWidget.className != className)
-                    foldWidget.className = className;
+                    foldClass += " ace_open";
+                if (foldWidget.className != foldClass)
+                    foldWidget.className = foldClass;
                 dom.setStyle(foldWidget.style, "height", lineHeight);
                 dom.setStyle(foldWidget.style, "display", "inline-block");
                 foldWidget.setAttribute("role", "button");
                 foldWidget.setAttribute("tabindex", "-1");
-                var fold = session.getFoldLine(rowText - 1);
-                if (fold) {
-                    foldWidget.setAttribute("aria-label", nls("Unfold rows $0 to $1", [rowText, fold.end.row + 1]));
+                var foldRange = session.getFoldWidgetRange(row);
+                if (foldRange)
+                    foldWidget.setAttribute("aria-label", nls("Toggle code folding, rows $0 through $1", [foldRange.start.row + 1, foldRange.end.row + 1]));
+                else {
+                    if (fold)
+                        foldWidget.setAttribute("aria-label", nls("Toggle code folding, rows $0 through $1", [fold.start.row + 1, fold.end.row + 1]));
+                    else
+                        foldWidget.setAttribute("aria-label", nls("Toggle code folding, row $0", [row + 1]));
+                }
+                if (isClosedFold) {
+                    foldWidget.setAttribute("aria-expanded", "false");
                     foldWidget.setAttribute("title", nls("Unfold code"));
                 } else {
-                    foldWidget.setAttribute("aria-label", nls("Fold at row $0", [rowText]));
+                    foldWidget.setAttribute("aria-expanded", "true");
                     foldWidget.setAttribute("title", nls("Fold code"));
                 }
             } else {
                 if (foldWidget) {
                     dom.setStyle(foldWidget.style, "display", "none");
                     foldWidget.setAttribute("tabindex", "0");
                     foldWidget.removeAttribute("role");
@@ -16524,14 +16565,16 @@
                 annotationNode.removeAttribute("aria-label");
                 annotationNode.removeAttribute("role");
                 annotationNode.setAttribute("tabindex", "0");
             }
             if (rowText !== textNode.data) {
                 textNode.data = rowText;
             }
+            if (element.className != className)
+                element.className = className;
             dom.setStyle(cell.element.style, "height", this.$lines.computeLineHeight(row, config, session) + "px");
             dom.setStyle(cell.element.style, "top", this.$lines.computeLineTop(row, config, session) + "px");
             cell.text = rowText;
             if (annotationNode.style.display === "none" && foldWidget.style.display === "none")
                 cell.element.setAttribute("aria-hidden", true);
             else
                 cell.element.setAttribute("aria-hidden", false);
@@ -18264,15 +18307,15 @@
         height: 0
     };
     oop.implement(FontMetrics.prototype, EventEmitter);
     exports.FontMetrics = FontMetrics;
 
 });
 
-define("ace/css/editor.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/css/editor-css", ["require", "exports", "module"], function(require, exports, module) {
     /*
     styles = []
     for (var i = 1; i < 16; i++) {
         styles.push(".ace_br" + i + "{" + (
             ["top-left", "top-right", "bottom-right", "bottom-left"]
         ).map(function(x, j) {
             return i & (1<<j) ? "border-" + x + "-radius: 3px;" : ""
@@ -18400,15 +18443,15 @@
         return Decorator;
     }());
     oop.implement(Decorator.prototype, EventEmitter);
     exports.Decorator = Decorator;
 
 });
 
-define("ace/virtual_renderer", ["require", "exports", "module", "ace/lib/oop", "ace/lib/dom", "ace/lib/lang", "ace/config", "ace/layer/gutter", "ace/layer/marker", "ace/layer/text", "ace/layer/cursor", "ace/scrollbar", "ace/scrollbar", "ace/scrollbar_custom", "ace/scrollbar_custom", "ace/renderloop", "ace/layer/font_metrics", "ace/lib/event_emitter", "ace/css/editor.css", "ace/layer/decorators", "ace/lib/useragent"], function(require, exports, module) {
+define("ace/virtual_renderer", ["require", "exports", "module", "ace/lib/oop", "ace/lib/dom", "ace/lib/lang", "ace/config", "ace/layer/gutter", "ace/layer/marker", "ace/layer/text", "ace/layer/cursor", "ace/scrollbar", "ace/scrollbar", "ace/scrollbar_custom", "ace/scrollbar_custom", "ace/renderloop", "ace/layer/font_metrics", "ace/lib/event_emitter", "ace/css/editor-css", "ace/layer/decorators", "ace/lib/useragent"], function(require, exports, module) {
     "use strict";
     var oop = require("./lib/oop");
     var dom = require("./lib/dom");
     var lang = require("./lib/lang");
     var config = require("./config");
     var GutterLayer = require("./layer/gutter").Gutter;
     var MarkerLayer = require("./layer/marker").Marker;
@@ -18417,15 +18460,15 @@
     var HScrollBar = require("./scrollbar").HScrollBar;
     var VScrollBar = require("./scrollbar").VScrollBar;
     var HScrollBarCustom = require("./scrollbar_custom").HScrollBar;
     var VScrollBarCustom = require("./scrollbar_custom").VScrollBar;
     var RenderLoop = require("./renderloop").RenderLoop;
     var FontMetrics = require("./layer/font_metrics").FontMetrics;
     var EventEmitter = require("./lib/event_emitter").EventEmitter;
-    var editorCss = require("./css/editor.css");
+    var editorCss = require("./css/editor-css");
     var Decorator = require("./layer/decorators").Decorator;
     var useragent = require("./lib/useragent");
     dom.importCssString(editorCss, "ace_editor.css", false);
     var VirtualRenderer = /** @class */ (function() {
         function VirtualRenderer(container, theme) {
             var _self = this;
             this.container = container || dom.createElement("div");
@@ -18707,15 +18750,15 @@
         VirtualRenderer.prototype.setShowInvisibles = function(showInvisibles) {
             this.setOption("showInvisibles", showInvisibles);
             this.session.$bidiHandler.setShowInvisibles(showInvisibles);
         };
         VirtualRenderer.prototype.getShowInvisibles = function() {
             return this.getOption("showInvisibles");
         };
-        VirtualRenderer.prototype.getDisplayIndentGuide = function() {
+        VirtualRenderer.prototype.getDisplayIndentGuides = function() {
             return this.getOption("displayIndentGuides");
         };
         VirtualRenderer.prototype.setDisplayIndentGuides = function(display) {
             this.setOption("displayIndentGuides", display);
         };
         VirtualRenderer.prototype.getHighlightIndentGuides = function() {
             return this.getOption("highlightIndentGuides");
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-beautify.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-beautify.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-code_lens.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-code_lens.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-command_bar.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-command_bar.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-elastic_tabstops_lite.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-elastic_tabstops_lite.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-emmet.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-emmet.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-hardwrap.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-hardwrap.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-inline_autocomplete.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-inline_autocomplete.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1157,16 +1157,17 @@
             var popup = new $singleLineEditor(el);
             if (parentNode) {
                 parentNode.appendChild(el);
             }
             el.style.display = "none";
             popup.renderer.content.style.cursor = "default";
             popup.renderer.setStyle("ace_autocomplete");
-            popup.renderer.container.setAttribute("role", "listbox");
-            popup.renderer.container.setAttribute("aria-label", nls("Autocomplete suggestions"));
+            popup.renderer.$textLayer.element.setAttribute("role", "listbox");
+            popup.renderer.$textLayer.element.setAttribute("aria-label", nls("Autocomplete suggestions"));
+            popup.renderer.textarea.setAttribute("aria-hidden", "true");
             popup.setOption("displayIndentGuides", false);
             popup.setOption("dragDelay", 150);
             var noop = function() {};
             popup.focus = noop;
             popup.$isFocused = true;
             popup.renderer.$cursorLayer.restartTimer = noop;
             popup.renderer.$cursorLayer.element.style.opacity = 0;
@@ -1231,20 +1232,20 @@
                     t.selectedNode.removeAttribute("id");
                 }
                 t.selectedNode = selected;
                 if (selected) {
                     dom.addCssClass(selected, "ace_selected");
                     var ariaId = getAriaId(row);
                     selected.id = ariaId;
-                    popup.renderer.container.setAttribute("aria-activedescendant", ariaId);
+                    t.element.setAttribute("aria-activedescendant", ariaId);
                     el.setAttribute("aria-activedescendant", ariaId);
                     selected.setAttribute("role", "option");
                     selected.setAttribute("aria-label", popup.getData(row).value);
                     selected.setAttribute("aria-setsize", popup.data.length);
-                    selected.setAttribute("aria-posinset", row);
+                    selected.setAttribute("aria-posinset", row + 1);
                     selected.setAttribute("aria-describedby", "doc-tooltip");
                 }
             });
             var hideHoverMarker = function() {
                 setHoverMarker(-1);
             };
             var setHoverMarker = function(row, suppressRedraw) {
@@ -1464,15 +1465,15 @@
             };
             popup.$imageSize = 0;
             popup.$borderSize = 1;
             return popup;
         }
         return AcePopup;
     }());
-    dom.importCssString("\n.ace_editor.ace_autocomplete .ace_marker-layer .ace_active-line {\n    background-color: #CAD6FA;\n    z-index: 1;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_marker-layer .ace_active-line {\n    background-color: #3a674e;\n}\n.ace_editor.ace_autocomplete .ace_line-hover {\n    border: 1px solid #abbffe;\n    margin-top: -1px;\n    background: rgba(233,233,253,0.4);\n    position: absolute;\n    z-index: 2;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_line-hover {\n    border: 1px solid rgba(109, 150, 13, 0.8);\n    background: rgba(58, 103, 78, 0.62);\n}\n.ace_completion-meta {\n    opacity: 0.5;\n    margin: 0 0.9em;\n}\n.ace_completion-message {\n    color: blue;\n}\n.ace_editor.ace_autocomplete .ace_completion-highlight{\n    color: #2d69c7;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_completion-highlight{\n    color: #93ca12;\n}\n.ace_editor.ace_autocomplete {\n    width: 300px;\n    z-index: 200000;\n    border: 1px lightgray solid;\n    position: fixed;\n    box-shadow: 2px 3px 5px rgba(0,0,0,.2);\n    line-height: 1.4;\n    background: #fefefe;\n    color: #111;\n}\n.ace_dark.ace_editor.ace_autocomplete {\n    border: 1px #484747 solid;\n    box-shadow: 2px 3px 5px rgba(0, 0, 0, 0.51);\n    line-height: 1.4;\n    background: #25282c;\n    color: #c1c1c1;\n}\n.ace_autocomplete_right .ace_text-layer  {\n    width: calc(100% - 8px);\n}\n.ace_autocomplete_right .ace_line {\n    display: flex;\n}\n.ace_autocomplete_right .ace_completion-spacer {\n    flex: 1;\n}\n", "autocompletion.css", false);
+    dom.importCssString("\n.ace_editor.ace_autocomplete .ace_marker-layer .ace_active-line {\n    background-color: #CAD6FA;\n    z-index: 1;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_marker-layer .ace_active-line {\n    background-color: #3a674e;\n}\n.ace_editor.ace_autocomplete .ace_line-hover {\n    border: 1px solid #abbffe;\n    margin-top: -1px;\n    background: rgba(233,233,253,0.4);\n    position: absolute;\n    z-index: 2;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_line-hover {\n    border: 1px solid rgba(109, 150, 13, 0.8);\n    background: rgba(58, 103, 78, 0.62);\n}\n.ace_completion-meta {\n    opacity: 0.5;\n    margin-left: 0.9em;\n}\n.ace_completion-message {\n    color: blue;\n}\n.ace_editor.ace_autocomplete .ace_completion-highlight{\n    color: #2d69c7;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_completion-highlight{\n    color: #93ca12;\n}\n.ace_editor.ace_autocomplete {\n    width: 300px;\n    z-index: 200000;\n    border: 1px lightgray solid;\n    position: fixed;\n    box-shadow: 2px 3px 5px rgba(0,0,0,.2);\n    line-height: 1.4;\n    background: #fefefe;\n    color: #111;\n}\n.ace_dark.ace_editor.ace_autocomplete {\n    border: 1px #484747 solid;\n    box-shadow: 2px 3px 5px rgba(0, 0, 0, 0.51);\n    line-height: 1.4;\n    background: #25282c;\n    color: #c1c1c1;\n}\n.ace_autocomplete .ace_text-layer  {\n    width: calc(100% - 8px);\n}\n.ace_autocomplete .ace_line {\n    display: flex;\n    align-items: center;\n}\n.ace_autocomplete .ace_line > * {\n    min-width: 0;\n    flex: 0 0 auto;\n}\n.ace_autocomplete .ace_line .ace_ {\n    flex: 0 1 auto;\n    overflow: hidden;\n    white-space: nowrap;\n    text-overflow: ellipsis;\n}\n.ace_autocomplete .ace_completion-spacer {\n    flex: 1;\n}\n", "autocompletion.css", false);
     exports.AcePopup = AcePopup;
     exports.$singleLineEditor = $singleLineEditor;
     exports.getAriaId = getAriaId;
 
 });
 
 define("ace/autocomplete/util", ["require", "exports", "module"], function(require, exports, module) {
@@ -1565,14 +1566,15 @@
             this.keyboardHandler = new HashHandler();
             this.keyboardHandler.bindKeys(this.commands);
             this.parentNode = null;
             this.blurListener = this.blurListener.bind(this);
             this.changeListener = this.changeListener.bind(this);
             this.mousedownListener = this.mousedownListener.bind(this);
             this.mousewheelListener = this.mousewheelListener.bind(this);
+            this.onLayoutChange = this.onLayoutChange.bind(this);
             this.changeTimer = lang.delayedCall(function() {
                 this.updateCompletions(true);
             }.bind(this));
             this.tooltipTimer = lang.delayedCall(this.updateDocTooltip.bind(this), 50);
         }
         Autocomplete.prototype.$init = function() {
             this.popup = new AcePopup(this.parentNode || document.body || document.documentElement);
@@ -1609,14 +1611,51 @@
                 if (!this.inlineRenderer.show(this.editor, completion, prefix)) {
                     this.inlineRenderer.hide();
                 }
                 this.$updatePopupPosition();
             }
             this.tooltipTimer.call(null, null);
         };
+        Autocomplete.prototype.observeLayoutChanges = function() {
+            if (this.$elements || !this.editor)
+                return;
+            window.addEventListener("resize", this.onLayoutChange, {
+                passive: true
+            });
+            window.addEventListener("wheel", this.mousewheelListener);
+            var el = this.editor.container.parentNode;
+            var elements = [];
+            while (el) {
+                elements.push(el);
+                el.addEventListener("scroll", this.onLayoutChange, {
+                    passive: true
+                });
+                el = el.parentNode;
+            }
+            this.$elements = elements;
+        };
+        Autocomplete.prototype.unObserveLayoutChanges = function() {
+            var _this = this;
+            window.removeEventListener("resize", this.onLayoutChange, {
+                passive: true
+            });
+            window.removeEventListener("wheel", this.mousewheelListener);
+            this.$elements && this.$elements.forEach(function(el) {
+                el.removeEventListener("scroll", _this.onLayoutChange, {
+                    passive: true
+                });
+            });
+            this.$elements = null;
+        };
+        Autocomplete.prototype.onLayoutChange = function() {
+            if (!this.popup.isOpen)
+                return this.unObserveLayoutChanges();
+            this.$updatePopupPosition();
+            this.updateDocTooltip();
+        };
         Autocomplete.prototype.$updatePopupPosition = function() {
             var editor = this.editor;
             var renderer = editor.renderer;
             var lineHeight = renderer.layerConfig.lineHeight;
             var pos = renderer.$cursorLayer.getPixelPosition(this.base, true);
             pos.left -= this.popup.getTextLeftOffset();
             var rect = editor.container.getBoundingClientRect();
@@ -1662,14 +1701,15 @@
                 if (this.tooltipNode) {
                     this.updateDocTooltip();
                 }
             } else if (keepPopupPosition && !prefix) {
                 this.detach();
             }
             this.changeTimer.cancel();
+            this.observeLayoutChanges();
         };
         Autocomplete.prototype.detach = function() {
             if (this.editor) {
                 this.editor.keyBinding.removeKeyboardHandler(this.keyboardHandler);
                 this.editor.off("changeSelection", this.changeListener);
                 this.editor.off("blur", this.blurListener);
                 this.editor.off("mousedown", this.mousedownListener);
@@ -1682,14 +1722,15 @@
             }
             if (this.popup && this.popup.isOpen)
                 this.popup.hide();
             if (this.base)
                 this.base.detach();
             this.activated = false;
             this.completionProvider = this.completions = this.base = null;
+            this.unObserveLayoutChanges();
         };
         Autocomplete.prototype.changeListener = function(e) {
             var cursor = this.editor.selection.lead;
             if (cursor.row != this.base.row || cursor.column < this.base.column) {
                 this.detach();
             }
             if (this.activated)
@@ -2017,15 +2058,15 @@
                 }
             });
             if (data.completer && data.completer.insertMatch) {
                 data.completer.insertMatch(editor, data);
             } else {
                 if (!this.completions)
                     return false;
-                if (this.completions.filterText) {
+                if (this.completions.filterText && !data.range) {
                     var ranges;
                     if (editor.selection.getAllRanges) {
                         ranges = editor.selection.getAllRanges();
                     } else {
                         ranges = [editor.getSelectionRange()];
                     }
                     for (var i = 0, range; range = ranges[i]; i++) {
@@ -2068,14 +2109,15 @@
             }
         };
         CompletionProvider.prototype.gatherCompletions = function(editor, callback) {
             var session = editor.getSession();
             var pos = editor.getCursorPosition();
             var prefix = util.getCompletionPrefix(editor);
             var matches = [];
+            this.completers = editor.completers;
             var total = editor.completers.length;
             editor.completers.forEach(function(completer, i) {
                 completer.getCompletions(editor, session, pos, prefix, function(err, results) {
                     if (!err && results)
                         matches = matches.concat(results);
                     callback(null, {
                         prefix: util.getCompletionPrefix(editor),
@@ -2123,14 +2165,19 @@
                 var results = immediateResults;
                 immediateResults = null;
                 processResults(results);
             }
         };
         CompletionProvider.prototype.detach = function() {
             this.active = false;
+            this.completers && this.completers.forEach(function(completer) {
+                if (typeof completer.cancel === "function") {
+                    completer.cancel();
+                }
+            });
         };
         return CompletionProvider;
     }());
     var FilteredList = /** @class */ (function() {
         function FilteredList(array, filterText) {
             this.all = array;
             this.filtered = array;
@@ -2845,24 +2892,38 @@
     };
     var doLiveAutocomplete = function(e) {
         var editor = e.editor;
         var hasCompleter = editor.completer && editor.completer.activated;
         if (e.command.name === "backspace") {
             if (hasCompleter && !util.getCompletionPrefix(editor))
                 editor.completer.detach();
-        } else if (e.command.name === "insertstring") {
-            var prefix = util.getCompletionPrefix(editor);
-            var triggerAutocomplete = util.triggerAutocomplete(editor);
-            if ((prefix || triggerAutocomplete) && !hasCompleter) {
-                var completer = Autocomplete.for(editor);
-                completer.autoShown = true;
-                completer.showPopup(editor);
+        } else if (e.command.name === "insertstring" && !hasCompleter) {
+            lastExecEvent = e;
+            var delay = e.editor.$liveAutocompletionDelay;
+            if (delay) {
+                liveAutocompleteTimer.delay(delay);
+            } else {
+                showLiveAutocomplete(e);
             }
         }
     };
+    var lastExecEvent;
+    var liveAutocompleteTimer = lang.delayedCall(function() {
+        showLiveAutocomplete(lastExecEvent);
+    }, 0);
+    var showLiveAutocomplete = function(e) {
+        var editor = e.editor;
+        var prefix = util.getCompletionPrefix(editor);
+        var triggerAutocomplete = util.triggerAutocomplete(editor);
+        if ((prefix || triggerAutocomplete) && prefix.length >= editor.$liveAutocompletionThreshold) {
+            var completer = Autocomplete.for(editor);
+            completer.autoShown = true;
+            completer.showPopup(editor);
+        }
+    };
     var Editor = require("../editor").Editor;
     require("../config").defineOptions(Editor.prototype, "editor", {
         enableBasicAutocompletion: {
             set: function(val) {
                 if (val) {
                     if (!this.completers)
                         this.completers = Array.isArray(val) ? val : completers;
@@ -2876,19 +2937,25 @@
         enableLiveAutocompletion: {
             set: function(val) {
                 if (val) {
                     if (!this.completers)
                         this.completers = Array.isArray(val) ? val : completers;
                     this.commands.on('afterExec', doLiveAutocomplete);
                 } else {
-                    this.commands.removeListener('afterExec', doLiveAutocomplete);
+                    this.commands.off('afterExec', doLiveAutocomplete);
                 }
             },
             value: false
         },
+        liveAutocompletionDelay: {
+            initialValue: 0
+        },
+        liveAutocompletionThreshold: {
+            initialValue: 0
+        },
         enableSnippets: {
             set: function(val) {
                 if (val) {
                     this.commands.addCommand(expandSnippet);
                     this.on("changeMode", onChangeMode);
                     onChangeMode(null, this);
                 } else {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-keybinding_menu.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-keybinding_menu.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-language_tools.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-language_tools.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1105,16 +1105,17 @@
             var popup = new $singleLineEditor(el);
             if (parentNode) {
                 parentNode.appendChild(el);
             }
             el.style.display = "none";
             popup.renderer.content.style.cursor = "default";
             popup.renderer.setStyle("ace_autocomplete");
-            popup.renderer.container.setAttribute("role", "listbox");
-            popup.renderer.container.setAttribute("aria-label", nls("Autocomplete suggestions"));
+            popup.renderer.$textLayer.element.setAttribute("role", "listbox");
+            popup.renderer.$textLayer.element.setAttribute("aria-label", nls("Autocomplete suggestions"));
+            popup.renderer.textarea.setAttribute("aria-hidden", "true");
             popup.setOption("displayIndentGuides", false);
             popup.setOption("dragDelay", 150);
             var noop = function() {};
             popup.focus = noop;
             popup.$isFocused = true;
             popup.renderer.$cursorLayer.restartTimer = noop;
             popup.renderer.$cursorLayer.element.style.opacity = 0;
@@ -1179,20 +1180,20 @@
                     t.selectedNode.removeAttribute("id");
                 }
                 t.selectedNode = selected;
                 if (selected) {
                     dom.addCssClass(selected, "ace_selected");
                     var ariaId = getAriaId(row);
                     selected.id = ariaId;
-                    popup.renderer.container.setAttribute("aria-activedescendant", ariaId);
+                    t.element.setAttribute("aria-activedescendant", ariaId);
                     el.setAttribute("aria-activedescendant", ariaId);
                     selected.setAttribute("role", "option");
                     selected.setAttribute("aria-label", popup.getData(row).value);
                     selected.setAttribute("aria-setsize", popup.data.length);
-                    selected.setAttribute("aria-posinset", row);
+                    selected.setAttribute("aria-posinset", row + 1);
                     selected.setAttribute("aria-describedby", "doc-tooltip");
                 }
             });
             var hideHoverMarker = function() {
                 setHoverMarker(-1);
             };
             var setHoverMarker = function(row, suppressRedraw) {
@@ -1412,15 +1413,15 @@
             };
             popup.$imageSize = 0;
             popup.$borderSize = 1;
             return popup;
         }
         return AcePopup;
     }());
-    dom.importCssString("\n.ace_editor.ace_autocomplete .ace_marker-layer .ace_active-line {\n    background-color: #CAD6FA;\n    z-index: 1;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_marker-layer .ace_active-line {\n    background-color: #3a674e;\n}\n.ace_editor.ace_autocomplete .ace_line-hover {\n    border: 1px solid #abbffe;\n    margin-top: -1px;\n    background: rgba(233,233,253,0.4);\n    position: absolute;\n    z-index: 2;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_line-hover {\n    border: 1px solid rgba(109, 150, 13, 0.8);\n    background: rgba(58, 103, 78, 0.62);\n}\n.ace_completion-meta {\n    opacity: 0.5;\n    margin: 0 0.9em;\n}\n.ace_completion-message {\n    color: blue;\n}\n.ace_editor.ace_autocomplete .ace_completion-highlight{\n    color: #2d69c7;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_completion-highlight{\n    color: #93ca12;\n}\n.ace_editor.ace_autocomplete {\n    width: 300px;\n    z-index: 200000;\n    border: 1px lightgray solid;\n    position: fixed;\n    box-shadow: 2px 3px 5px rgba(0,0,0,.2);\n    line-height: 1.4;\n    background: #fefefe;\n    color: #111;\n}\n.ace_dark.ace_editor.ace_autocomplete {\n    border: 1px #484747 solid;\n    box-shadow: 2px 3px 5px rgba(0, 0, 0, 0.51);\n    line-height: 1.4;\n    background: #25282c;\n    color: #c1c1c1;\n}\n.ace_autocomplete_right .ace_text-layer  {\n    width: calc(100% - 8px);\n}\n.ace_autocomplete_right .ace_line {\n    display: flex;\n}\n.ace_autocomplete_right .ace_completion-spacer {\n    flex: 1;\n}\n", "autocompletion.css", false);
+    dom.importCssString("\n.ace_editor.ace_autocomplete .ace_marker-layer .ace_active-line {\n    background-color: #CAD6FA;\n    z-index: 1;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_marker-layer .ace_active-line {\n    background-color: #3a674e;\n}\n.ace_editor.ace_autocomplete .ace_line-hover {\n    border: 1px solid #abbffe;\n    margin-top: -1px;\n    background: rgba(233,233,253,0.4);\n    position: absolute;\n    z-index: 2;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_line-hover {\n    border: 1px solid rgba(109, 150, 13, 0.8);\n    background: rgba(58, 103, 78, 0.62);\n}\n.ace_completion-meta {\n    opacity: 0.5;\n    margin-left: 0.9em;\n}\n.ace_completion-message {\n    color: blue;\n}\n.ace_editor.ace_autocomplete .ace_completion-highlight{\n    color: #2d69c7;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_completion-highlight{\n    color: #93ca12;\n}\n.ace_editor.ace_autocomplete {\n    width: 300px;\n    z-index: 200000;\n    border: 1px lightgray solid;\n    position: fixed;\n    box-shadow: 2px 3px 5px rgba(0,0,0,.2);\n    line-height: 1.4;\n    background: #fefefe;\n    color: #111;\n}\n.ace_dark.ace_editor.ace_autocomplete {\n    border: 1px #484747 solid;\n    box-shadow: 2px 3px 5px rgba(0, 0, 0, 0.51);\n    line-height: 1.4;\n    background: #25282c;\n    color: #c1c1c1;\n}\n.ace_autocomplete .ace_text-layer  {\n    width: calc(100% - 8px);\n}\n.ace_autocomplete .ace_line {\n    display: flex;\n    align-items: center;\n}\n.ace_autocomplete .ace_line > * {\n    min-width: 0;\n    flex: 0 0 auto;\n}\n.ace_autocomplete .ace_line .ace_ {\n    flex: 0 1 auto;\n    overflow: hidden;\n    white-space: nowrap;\n    text-overflow: ellipsis;\n}\n.ace_autocomplete .ace_completion-spacer {\n    flex: 1;\n}\n", "autocompletion.css", false);
     exports.AcePopup = AcePopup;
     exports.$singleLineEditor = $singleLineEditor;
     exports.getAriaId = getAriaId;
 
 });
 
 define("ace/autocomplete/inline", ["require", "exports", "module", "ace/snippets"], function(require, exports, module) {
@@ -1565,14 +1566,15 @@
             this.keyboardHandler = new HashHandler();
             this.keyboardHandler.bindKeys(this.commands);
             this.parentNode = null;
             this.blurListener = this.blurListener.bind(this);
             this.changeListener = this.changeListener.bind(this);
             this.mousedownListener = this.mousedownListener.bind(this);
             this.mousewheelListener = this.mousewheelListener.bind(this);
+            this.onLayoutChange = this.onLayoutChange.bind(this);
             this.changeTimer = lang.delayedCall(function() {
                 this.updateCompletions(true);
             }.bind(this));
             this.tooltipTimer = lang.delayedCall(this.updateDocTooltip.bind(this), 50);
         }
         Autocomplete.prototype.$init = function() {
             this.popup = new AcePopup(this.parentNode || document.body || document.documentElement);
@@ -1609,14 +1611,51 @@
                 if (!this.inlineRenderer.show(this.editor, completion, prefix)) {
                     this.inlineRenderer.hide();
                 }
                 this.$updatePopupPosition();
             }
             this.tooltipTimer.call(null, null);
         };
+        Autocomplete.prototype.observeLayoutChanges = function() {
+            if (this.$elements || !this.editor)
+                return;
+            window.addEventListener("resize", this.onLayoutChange, {
+                passive: true
+            });
+            window.addEventListener("wheel", this.mousewheelListener);
+            var el = this.editor.container.parentNode;
+            var elements = [];
+            while (el) {
+                elements.push(el);
+                el.addEventListener("scroll", this.onLayoutChange, {
+                    passive: true
+                });
+                el = el.parentNode;
+            }
+            this.$elements = elements;
+        };
+        Autocomplete.prototype.unObserveLayoutChanges = function() {
+            var _this = this;
+            window.removeEventListener("resize", this.onLayoutChange, {
+                passive: true
+            });
+            window.removeEventListener("wheel", this.mousewheelListener);
+            this.$elements && this.$elements.forEach(function(el) {
+                el.removeEventListener("scroll", _this.onLayoutChange, {
+                    passive: true
+                });
+            });
+            this.$elements = null;
+        };
+        Autocomplete.prototype.onLayoutChange = function() {
+            if (!this.popup.isOpen)
+                return this.unObserveLayoutChanges();
+            this.$updatePopupPosition();
+            this.updateDocTooltip();
+        };
         Autocomplete.prototype.$updatePopupPosition = function() {
             var editor = this.editor;
             var renderer = editor.renderer;
             var lineHeight = renderer.layerConfig.lineHeight;
             var pos = renderer.$cursorLayer.getPixelPosition(this.base, true);
             pos.left -= this.popup.getTextLeftOffset();
             var rect = editor.container.getBoundingClientRect();
@@ -1662,14 +1701,15 @@
                 if (this.tooltipNode) {
                     this.updateDocTooltip();
                 }
             } else if (keepPopupPosition && !prefix) {
                 this.detach();
             }
             this.changeTimer.cancel();
+            this.observeLayoutChanges();
         };
         Autocomplete.prototype.detach = function() {
             if (this.editor) {
                 this.editor.keyBinding.removeKeyboardHandler(this.keyboardHandler);
                 this.editor.off("changeSelection", this.changeListener);
                 this.editor.off("blur", this.blurListener);
                 this.editor.off("mousedown", this.mousedownListener);
@@ -1682,14 +1722,15 @@
             }
             if (this.popup && this.popup.isOpen)
                 this.popup.hide();
             if (this.base)
                 this.base.detach();
             this.activated = false;
             this.completionProvider = this.completions = this.base = null;
+            this.unObserveLayoutChanges();
         };
         Autocomplete.prototype.changeListener = function(e) {
             var cursor = this.editor.selection.lead;
             if (cursor.row != this.base.row || cursor.column < this.base.column) {
                 this.detach();
             }
             if (this.activated)
@@ -2017,15 +2058,15 @@
                 }
             });
             if (data.completer && data.completer.insertMatch) {
                 data.completer.insertMatch(editor, data);
             } else {
                 if (!this.completions)
                     return false;
-                if (this.completions.filterText) {
+                if (this.completions.filterText && !data.range) {
                     var ranges;
                     if (editor.selection.getAllRanges) {
                         ranges = editor.selection.getAllRanges();
                     } else {
                         ranges = [editor.getSelectionRange()];
                     }
                     for (var i = 0, range; range = ranges[i]; i++) {
@@ -2068,14 +2109,15 @@
             }
         };
         CompletionProvider.prototype.gatherCompletions = function(editor, callback) {
             var session = editor.getSession();
             var pos = editor.getCursorPosition();
             var prefix = util.getCompletionPrefix(editor);
             var matches = [];
+            this.completers = editor.completers;
             var total = editor.completers.length;
             editor.completers.forEach(function(completer, i) {
                 completer.getCompletions(editor, session, pos, prefix, function(err, results) {
                     if (!err && results)
                         matches = matches.concat(results);
                     callback(null, {
                         prefix: util.getCompletionPrefix(editor),
@@ -2123,14 +2165,19 @@
                 var results = immediateResults;
                 immediateResults = null;
                 processResults(results);
             }
         };
         CompletionProvider.prototype.detach = function() {
             this.active = false;
+            this.completers && this.completers.forEach(function(completer) {
+                if (typeof completer.cancel === "function") {
+                    completer.cancel();
+                }
+            });
         };
         return CompletionProvider;
     }());
     var FilteredList = /** @class */ (function() {
         function FilteredList(array, filterText) {
             this.all = array;
             this.filtered = array;
@@ -2378,24 +2425,38 @@
     };
     var doLiveAutocomplete = function(e) {
         var editor = e.editor;
         var hasCompleter = editor.completer && editor.completer.activated;
         if (e.command.name === "backspace") {
             if (hasCompleter && !util.getCompletionPrefix(editor))
                 editor.completer.detach();
-        } else if (e.command.name === "insertstring") {
-            var prefix = util.getCompletionPrefix(editor);
-            var triggerAutocomplete = util.triggerAutocomplete(editor);
-            if ((prefix || triggerAutocomplete) && !hasCompleter) {
-                var completer = Autocomplete.for(editor);
-                completer.autoShown = true;
-                completer.showPopup(editor);
+        } else if (e.command.name === "insertstring" && !hasCompleter) {
+            lastExecEvent = e;
+            var delay = e.editor.$liveAutocompletionDelay;
+            if (delay) {
+                liveAutocompleteTimer.delay(delay);
+            } else {
+                showLiveAutocomplete(e);
             }
         }
     };
+    var lastExecEvent;
+    var liveAutocompleteTimer = lang.delayedCall(function() {
+        showLiveAutocomplete(lastExecEvent);
+    }, 0);
+    var showLiveAutocomplete = function(e) {
+        var editor = e.editor;
+        var prefix = util.getCompletionPrefix(editor);
+        var triggerAutocomplete = util.triggerAutocomplete(editor);
+        if ((prefix || triggerAutocomplete) && prefix.length >= editor.$liveAutocompletionThreshold) {
+            var completer = Autocomplete.for(editor);
+            completer.autoShown = true;
+            completer.showPopup(editor);
+        }
+    };
     var Editor = require("../editor").Editor;
     require("../config").defineOptions(Editor.prototype, "editor", {
         enableBasicAutocompletion: {
             set: function(val) {
                 if (val) {
                     if (!this.completers)
                         this.completers = Array.isArray(val) ? val : completers;
@@ -2409,19 +2470,25 @@
         enableLiveAutocompletion: {
             set: function(val) {
                 if (val) {
                     if (!this.completers)
                         this.completers = Array.isArray(val) ? val : completers;
                     this.commands.on('afterExec', doLiveAutocomplete);
                 } else {
-                    this.commands.removeListener('afterExec', doLiveAutocomplete);
+                    this.commands.off('afterExec', doLiveAutocomplete);
                 }
             },
             value: false
         },
+        liveAutocompletionDelay: {
+            initialValue: 0
+        },
+        liveAutocompletionThreshold: {
+            initialValue: 0
+        },
         enableSnippets: {
             set: function(val) {
                 if (val) {
                     this.commands.addCommand(expandSnippet);
                     this.on("changeMode", onChangeMode);
                     onChangeMode(null, this);
                 } else {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-linking.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-linking.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-modelist.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-modelist.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-options.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-options.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -628,14 +628,18 @@
                 path: "useSvgGutterIcons"
             },
             "Annotations for folded lines": {
                 path: "showFoldedAnnotations"
             },
             "Keyboard Accessibility Mode": {
                 path: "enableKeyboardAccessibility"
+            },
+            "Gutter tooltip follows mouse": {
+                path: "tooltipFollowsMouse",
+                defaultValue: true
             }
         }
     };
     var OptionPanel = /** @class */ (function() {
         function OptionPanel(editor, element) {
             this.editor = editor;
             this.container = element || document.createElement("div");
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-prompt.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-prompt.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -28,16 +28,17 @@
             var popup = new $singleLineEditor(el);
             if (parentNode) {
                 parentNode.appendChild(el);
             }
             el.style.display = "none";
             popup.renderer.content.style.cursor = "default";
             popup.renderer.setStyle("ace_autocomplete");
-            popup.renderer.container.setAttribute("role", "listbox");
-            popup.renderer.container.setAttribute("aria-label", nls("Autocomplete suggestions"));
+            popup.renderer.$textLayer.element.setAttribute("role", "listbox");
+            popup.renderer.$textLayer.element.setAttribute("aria-label", nls("Autocomplete suggestions"));
+            popup.renderer.textarea.setAttribute("aria-hidden", "true");
             popup.setOption("displayIndentGuides", false);
             popup.setOption("dragDelay", 150);
             var noop = function() {};
             popup.focus = noop;
             popup.$isFocused = true;
             popup.renderer.$cursorLayer.restartTimer = noop;
             popup.renderer.$cursorLayer.element.style.opacity = 0;
@@ -102,20 +103,20 @@
                     t.selectedNode.removeAttribute("id");
                 }
                 t.selectedNode = selected;
                 if (selected) {
                     dom.addCssClass(selected, "ace_selected");
                     var ariaId = getAriaId(row);
                     selected.id = ariaId;
-                    popup.renderer.container.setAttribute("aria-activedescendant", ariaId);
+                    t.element.setAttribute("aria-activedescendant", ariaId);
                     el.setAttribute("aria-activedescendant", ariaId);
                     selected.setAttribute("role", "option");
                     selected.setAttribute("aria-label", popup.getData(row).value);
                     selected.setAttribute("aria-setsize", popup.data.length);
-                    selected.setAttribute("aria-posinset", row);
+                    selected.setAttribute("aria-posinset", row + 1);
                     selected.setAttribute("aria-describedby", "doc-tooltip");
                 }
             });
             var hideHoverMarker = function() {
                 setHoverMarker(-1);
             };
             var setHoverMarker = function(row, suppressRedraw) {
@@ -335,15 +336,15 @@
             };
             popup.$imageSize = 0;
             popup.$borderSize = 1;
             return popup;
         }
         return AcePopup;
     }());
-    dom.importCssString("\n.ace_editor.ace_autocomplete .ace_marker-layer .ace_active-line {\n    background-color: #CAD6FA;\n    z-index: 1;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_marker-layer .ace_active-line {\n    background-color: #3a674e;\n}\n.ace_editor.ace_autocomplete .ace_line-hover {\n    border: 1px solid #abbffe;\n    margin-top: -1px;\n    background: rgba(233,233,253,0.4);\n    position: absolute;\n    z-index: 2;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_line-hover {\n    border: 1px solid rgba(109, 150, 13, 0.8);\n    background: rgba(58, 103, 78, 0.62);\n}\n.ace_completion-meta {\n    opacity: 0.5;\n    margin: 0 0.9em;\n}\n.ace_completion-message {\n    color: blue;\n}\n.ace_editor.ace_autocomplete .ace_completion-highlight{\n    color: #2d69c7;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_completion-highlight{\n    color: #93ca12;\n}\n.ace_editor.ace_autocomplete {\n    width: 300px;\n    z-index: 200000;\n    border: 1px lightgray solid;\n    position: fixed;\n    box-shadow: 2px 3px 5px rgba(0,0,0,.2);\n    line-height: 1.4;\n    background: #fefefe;\n    color: #111;\n}\n.ace_dark.ace_editor.ace_autocomplete {\n    border: 1px #484747 solid;\n    box-shadow: 2px 3px 5px rgba(0, 0, 0, 0.51);\n    line-height: 1.4;\n    background: #25282c;\n    color: #c1c1c1;\n}\n.ace_autocomplete_right .ace_text-layer  {\n    width: calc(100% - 8px);\n}\n.ace_autocomplete_right .ace_line {\n    display: flex;\n}\n.ace_autocomplete_right .ace_completion-spacer {\n    flex: 1;\n}\n", "autocompletion.css", false);
+    dom.importCssString("\n.ace_editor.ace_autocomplete .ace_marker-layer .ace_active-line {\n    background-color: #CAD6FA;\n    z-index: 1;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_marker-layer .ace_active-line {\n    background-color: #3a674e;\n}\n.ace_editor.ace_autocomplete .ace_line-hover {\n    border: 1px solid #abbffe;\n    margin-top: -1px;\n    background: rgba(233,233,253,0.4);\n    position: absolute;\n    z-index: 2;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_line-hover {\n    border: 1px solid rgba(109, 150, 13, 0.8);\n    background: rgba(58, 103, 78, 0.62);\n}\n.ace_completion-meta {\n    opacity: 0.5;\n    margin-left: 0.9em;\n}\n.ace_completion-message {\n    color: blue;\n}\n.ace_editor.ace_autocomplete .ace_completion-highlight{\n    color: #2d69c7;\n}\n.ace_dark.ace_editor.ace_autocomplete .ace_completion-highlight{\n    color: #93ca12;\n}\n.ace_editor.ace_autocomplete {\n    width: 300px;\n    z-index: 200000;\n    border: 1px lightgray solid;\n    position: fixed;\n    box-shadow: 2px 3px 5px rgba(0,0,0,.2);\n    line-height: 1.4;\n    background: #fefefe;\n    color: #111;\n}\n.ace_dark.ace_editor.ace_autocomplete {\n    border: 1px #484747 solid;\n    box-shadow: 2px 3px 5px rgba(0, 0, 0, 0.51);\n    line-height: 1.4;\n    background: #25282c;\n    color: #c1c1c1;\n}\n.ace_autocomplete .ace_text-layer  {\n    width: calc(100% - 8px);\n}\n.ace_autocomplete .ace_line {\n    display: flex;\n    align-items: center;\n}\n.ace_autocomplete .ace_line > * {\n    min-width: 0;\n    flex: 0 0 auto;\n}\n.ace_autocomplete .ace_line .ace_ {\n    flex: 0 1 auto;\n    overflow: hidden;\n    white-space: nowrap;\n    text-overflow: ellipsis;\n}\n.ace_autocomplete .ace_completion-spacer {\n    flex: 1;\n}\n", "autocompletion.css", false);
     exports.AcePopup = AcePopup;
     exports.$singleLineEditor = $singleLineEditor;
     exports.getAriaId = getAriaId;
 
 });
 
 define("ace/snippets", ["require", "exports", "module", "ace/lib/dom", "ace/lib/oop", "ace/lib/event_emitter", "ace/lib/lang", "ace/range", "ace/range_list", "ace/keyboard/hash_handler", "ace/tokenizer", "ace/clipboard", "ace/editor"], function(require, exports, module) {
@@ -1565,14 +1566,15 @@
             this.keyboardHandler = new HashHandler();
             this.keyboardHandler.bindKeys(this.commands);
             this.parentNode = null;
             this.blurListener = this.blurListener.bind(this);
             this.changeListener = this.changeListener.bind(this);
             this.mousedownListener = this.mousedownListener.bind(this);
             this.mousewheelListener = this.mousewheelListener.bind(this);
+            this.onLayoutChange = this.onLayoutChange.bind(this);
             this.changeTimer = lang.delayedCall(function() {
                 this.updateCompletions(true);
             }.bind(this));
             this.tooltipTimer = lang.delayedCall(this.updateDocTooltip.bind(this), 50);
         }
         Autocomplete.prototype.$init = function() {
             this.popup = new AcePopup(this.parentNode || document.body || document.documentElement);
@@ -1609,14 +1611,51 @@
                 if (!this.inlineRenderer.show(this.editor, completion, prefix)) {
                     this.inlineRenderer.hide();
                 }
                 this.$updatePopupPosition();
             }
             this.tooltipTimer.call(null, null);
         };
+        Autocomplete.prototype.observeLayoutChanges = function() {
+            if (this.$elements || !this.editor)
+                return;
+            window.addEventListener("resize", this.onLayoutChange, {
+                passive: true
+            });
+            window.addEventListener("wheel", this.mousewheelListener);
+            var el = this.editor.container.parentNode;
+            var elements = [];
+            while (el) {
+                elements.push(el);
+                el.addEventListener("scroll", this.onLayoutChange, {
+                    passive: true
+                });
+                el = el.parentNode;
+            }
+            this.$elements = elements;
+        };
+        Autocomplete.prototype.unObserveLayoutChanges = function() {
+            var _this = this;
+            window.removeEventListener("resize", this.onLayoutChange, {
+                passive: true
+            });
+            window.removeEventListener("wheel", this.mousewheelListener);
+            this.$elements && this.$elements.forEach(function(el) {
+                el.removeEventListener("scroll", _this.onLayoutChange, {
+                    passive: true
+                });
+            });
+            this.$elements = null;
+        };
+        Autocomplete.prototype.onLayoutChange = function() {
+            if (!this.popup.isOpen)
+                return this.unObserveLayoutChanges();
+            this.$updatePopupPosition();
+            this.updateDocTooltip();
+        };
         Autocomplete.prototype.$updatePopupPosition = function() {
             var editor = this.editor;
             var renderer = editor.renderer;
             var lineHeight = renderer.layerConfig.lineHeight;
             var pos = renderer.$cursorLayer.getPixelPosition(this.base, true);
             pos.left -= this.popup.getTextLeftOffset();
             var rect = editor.container.getBoundingClientRect();
@@ -1662,14 +1701,15 @@
                 if (this.tooltipNode) {
                     this.updateDocTooltip();
                 }
             } else if (keepPopupPosition && !prefix) {
                 this.detach();
             }
             this.changeTimer.cancel();
+            this.observeLayoutChanges();
         };
         Autocomplete.prototype.detach = function() {
             if (this.editor) {
                 this.editor.keyBinding.removeKeyboardHandler(this.keyboardHandler);
                 this.editor.off("changeSelection", this.changeListener);
                 this.editor.off("blur", this.blurListener);
                 this.editor.off("mousedown", this.mousedownListener);
@@ -1682,14 +1722,15 @@
             }
             if (this.popup && this.popup.isOpen)
                 this.popup.hide();
             if (this.base)
                 this.base.detach();
             this.activated = false;
             this.completionProvider = this.completions = this.base = null;
+            this.unObserveLayoutChanges();
         };
         Autocomplete.prototype.changeListener = function(e) {
             var cursor = this.editor.selection.lead;
             if (cursor.row != this.base.row || cursor.column < this.base.column) {
                 this.detach();
             }
             if (this.activated)
@@ -2017,15 +2058,15 @@
                 }
             });
             if (data.completer && data.completer.insertMatch) {
                 data.completer.insertMatch(editor, data);
             } else {
                 if (!this.completions)
                     return false;
-                if (this.completions.filterText) {
+                if (this.completions.filterText && !data.range) {
                     var ranges;
                     if (editor.selection.getAllRanges) {
                         ranges = editor.selection.getAllRanges();
                     } else {
                         ranges = [editor.getSelectionRange()];
                     }
                     for (var i = 0, range; range = ranges[i]; i++) {
@@ -2068,14 +2109,15 @@
             }
         };
         CompletionProvider.prototype.gatherCompletions = function(editor, callback) {
             var session = editor.getSession();
             var pos = editor.getCursorPosition();
             var prefix = util.getCompletionPrefix(editor);
             var matches = [];
+            this.completers = editor.completers;
             var total = editor.completers.length;
             editor.completers.forEach(function(completer, i) {
                 completer.getCompletions(editor, session, pos, prefix, function(err, results) {
                     if (!err && results)
                         matches = matches.concat(results);
                     callback(null, {
                         prefix: util.getCompletionPrefix(editor),
@@ -2123,14 +2165,19 @@
                 var results = immediateResults;
                 immediateResults = null;
                 processResults(results);
             }
         };
         CompletionProvider.prototype.detach = function() {
             this.active = false;
+            this.completers && this.completers.forEach(function(completer) {
+                if (typeof completer.cancel === "function") {
+                    completer.cancel();
+                }
+            });
         };
         return CompletionProvider;
     }());
     var FilteredList = /** @class */ (function() {
         function FilteredList(array, filterText) {
             this.all = array;
             this.filtered = array;
@@ -2595,15 +2642,14 @@
                 start: cmdLine.session.doc.indexToPosition(options.selection[0]),
                 end: cmdLine.session.doc.indexToPosition(options.selection[1])
             });
         }
         if (options.getCompletions) {
             var popup = new AcePopup();
             popup.renderer.setStyle("ace_autocomplete_inline");
-            popup.renderer.setStyle("ace_autocomplete_right");
             popup.container.style.display = "block";
             popup.container.style.maxWidth = "600px";
             popup.container.style.width = "100%";
             popup.container.style.marginTop = "3px";
             popup.renderer.setScrollMargin(2, 2, 0, 0);
             popup.autoSelect = false;
             popup.renderer.$maxLines = 15;
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-rtl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-rtl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-searchbox.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-searchbox.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
-define("ace/ext/searchbox.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/ext/searchbox-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = "\n\n/* ------------------------------------------------------------------------------------------\n * Editor Search Form\n * --------------------------------------------------------------------------------------- */\n.ace_search {\n    background-color: #ddd;\n    color: #666;\n    border: 1px solid #cbcbcb;\n    border-top: 0 none;\n    overflow: hidden;\n    margin: 0;\n    padding: 4px 6px 0 4px;\n    position: absolute;\n    top: 0;\n    z-index: 99;\n    white-space: normal;\n}\n.ace_search.left {\n    border-left: 0 none;\n    border-radius: 0px 0px 5px 0px;\n    left: 0;\n}\n.ace_search.right {\n    border-radius: 0px 0px 0px 5px;\n    border-right: 0 none;\n    right: 0;\n}\n\n.ace_search_form, .ace_replace_form {\n    margin: 0 20px 4px 0;\n    overflow: hidden;\n    line-height: 1.9;\n}\n.ace_replace_form {\n    margin-right: 0;\n}\n.ace_search_form.ace_nomatch {\n    outline: 1px solid red;\n}\n\n.ace_search_field {\n    border-radius: 3px 0 0 3px;\n    background-color: white;\n    color: black;\n    border: 1px solid #cbcbcb;\n    border-right: 0 none;\n    outline: 0;\n    padding: 0;\n    font-size: inherit;\n    margin: 0;\n    line-height: inherit;\n    padding: 0 6px;\n    min-width: 17em;\n    vertical-align: top;\n    min-height: 1.8em;\n    box-sizing: content-box;\n}\n.ace_searchbtn {\n    border: 1px solid #cbcbcb;\n    line-height: inherit;\n    display: inline-block;\n    padding: 0 6px;\n    background: #fff;\n    border-right: 0 none;\n    border-left: 1px solid #dcdcdc;\n    cursor: pointer;\n    margin: 0;\n    position: relative;\n    color: #666;\n}\n.ace_searchbtn:last-child {\n    border-radius: 0 3px 3px 0;\n    border-right: 1px solid #cbcbcb;\n}\n.ace_searchbtn:disabled {\n    background: none;\n    cursor: default;\n}\n.ace_searchbtn:hover {\n    background-color: #eef1f6;\n}\n.ace_searchbtn.prev, .ace_searchbtn.next {\n     padding: 0px 0.7em\n}\n.ace_searchbtn.prev:after, .ace_searchbtn.next:after {\n     content: \"\";\n     border: solid 2px #888;\n     width: 0.5em;\n     height: 0.5em;\n     border-width:  2px 0 0 2px;\n     display:inline-block;\n     transform: rotate(-45deg);\n}\n.ace_searchbtn.next:after {\n     border-width: 0 2px 2px 0 ;\n}\n.ace_searchbtn_close {\n    background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAcCAYAAABRVo5BAAAAZ0lEQVR42u2SUQrAMAhDvazn8OjZBilCkYVVxiis8H4CT0VrAJb4WHT3C5xU2a2IQZXJjiQIRMdkEoJ5Q2yMqpfDIo+XY4k6h+YXOyKqTIj5REaxloNAd0xiKmAtsTHqW8sR2W5f7gCu5nWFUpVjZwAAAABJRU5ErkJggg==) no-repeat 50% 0;\n    border-radius: 50%;\n    border: 0 none;\n    color: #656565;\n    cursor: pointer;\n    font: 16px/16px Arial;\n    padding: 0;\n    height: 14px;\n    width: 14px;\n    top: 9px;\n    right: 7px;\n    position: absolute;\n}\n.ace_searchbtn_close:hover {\n    background-color: #656565;\n    background-position: 50% 100%;\n    color: white;\n}\n\n.ace_button {\n    margin-left: 2px;\n    cursor: pointer;\n    -webkit-user-select: none;\n    -moz-user-select: none;\n    -o-user-select: none;\n    -ms-user-select: none;\n    user-select: none;\n    overflow: hidden;\n    opacity: 0.7;\n    border: 1px solid rgba(100,100,100,0.23);\n    padding: 1px;\n    box-sizing:    border-box!important;\n    color: black;\n}\n\n.ace_button:hover {\n    background-color: #eee;\n    opacity:1;\n}\n.ace_button:active {\n    background-color: #ddd;\n}\n\n.ace_button.checked {\n    border-color: #3399ff;\n    opacity:1;\n}\n\n.ace_search_options{\n    margin-bottom: 3px;\n    text-align: right;\n    -webkit-user-select: none;\n    -moz-user-select: none;\n    -o-user-select: none;\n    -ms-user-select: none;\n    user-select: none;\n    clear: both;\n}\n\n.ace_search_counter {\n    float: left;\n    font-family: arial;\n    padding: 0 8px;\n}";
 
 });
 
-define("ace/ext/searchbox", ["require", "exports", "module", "ace/lib/dom", "ace/lib/lang", "ace/lib/event", "ace/ext/searchbox.css", "ace/keyboard/hash_handler", "ace/lib/keys", "ace/config"], function(require, exports, module) {
+define("ace/ext/searchbox", ["require", "exports", "module", "ace/lib/dom", "ace/lib/lang", "ace/lib/event", "ace/ext/searchbox-css", "ace/keyboard/hash_handler", "ace/lib/keys", "ace/config"], function(require, exports, module) {
     "use strict";
     var dom = require("../lib/dom");
     var lang = require("../lib/lang");
     var event = require("../lib/event");
-    var searchboxCss = require("./searchbox.css");
+    var searchboxCss = require("./searchbox-css");
     var HashHandler = require("../keyboard/hash_handler").HashHandler;
     var keyUtil = require("../lib/keys");
     var nls = require("../config").nls;
     var MAX_COUNT = 999;
     dom.importCssString(searchboxCss, "ace_searchbox", false);
     var SearchBox = /** @class */ (function() {
         function SearchBox(editor, range, showReplaceForm) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-settings_menu.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-settings_menu.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -628,14 +628,18 @@
                 path: "useSvgGutterIcons"
             },
             "Annotations for folded lines": {
                 path: "showFoldedAnnotations"
             },
             "Keyboard Accessibility Mode": {
                 path: "enableKeyboardAccessibility"
+            },
+            "Gutter tooltip follows mouse": {
+                path: "tooltipFollowsMouse",
+                defaultValue: true
             }
         }
     };
     var OptionPanel = /** @class */ (function() {
         function OptionPanel(editor, element) {
             this.editor = editor;
             this.container = element || document.createElement("div");
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-spellcheck.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-spellcheck.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-split.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-split.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-static_highlight.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-static_highlight.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
-define("ace/ext/static.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/ext/static-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace_static_highlight {\n    font-family: 'Monaco', 'Menlo', 'Ubuntu Mono', 'Consolas', 'Source Code Pro', 'source-code-pro', 'Droid Sans Mono', monospace;\n    font-size: 12px;\n    white-space: pre-wrap\n}\n\n.ace_static_highlight .ace_gutter {\n    width: 2em;\n    text-align: right;\n    padding: 0 3px 0 0;\n    margin-right: 3px;\n    contain: none;\n}\n\n.ace_static_highlight.ace_show_gutter .ace_line {\n    padding-left: 2.6em;\n}\n\n.ace_static_highlight .ace_line { position: relative; }\n\n.ace_static_highlight .ace_gutter-cell {\n    -moz-user-select: -moz-none;\n    -khtml-user-select: none;\n    -webkit-user-select: none;\n    user-select: none;\n    top: 0;\n    bottom: 0;\n    left: 0;\n    position: absolute;\n}\n\n\n.ace_static_highlight .ace_gutter-cell:before {\n    content: counter(ace_line, decimal);\n    counter-increment: ace_line;\n}\n.ace_static_highlight {\n    counter-reset: ace_line;\n}\n";
 
 });
 
-define("ace/ext/static_highlight", ["require", "exports", "module", "ace/edit_session", "ace/layer/text", "ace/ext/static.css", "ace/config", "ace/lib/dom", "ace/lib/lang"], function(require, exports, module) {
+define("ace/ext/static_highlight", ["require", "exports", "module", "ace/edit_session", "ace/layer/text", "ace/ext/static-css", "ace/config", "ace/lib/dom", "ace/lib/lang"], function(require, exports, module) {
     "use strict";
     var EditSession = require("../edit_session").EditSession;
     var TextLayer = require("../layer/text").Text;
-    var baseStyles = require("./static.css");
+    var baseStyles = require("./static-css");
     var config = require("../config");
     var dom = require("../lib/dom");
     var escapeHTML = require("../lib/lang").escapeHTML;
     var Element = /** @class */ (function() {
         function Element(type) {
             this.type = type;
             this.style = {};
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-statusbar.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-statusbar.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-textarea.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-textarea.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,11 @@
-define("ace/ext/textarea", ["require", "exports", "module", "ace/lib/event", "ace/lib/useragent", "ace/lib/net", "ace/ace"], function(require, exports, module) {
+define("ace/ext/textarea", ["require", "exports", "module", "ace/lib/event", "ace/lib/useragent", "ace/ace"], function(require, exports, module) {
     "use strict";
     var event = require("../lib/event");
     var UA = require("../lib/useragent");
-    var net = require("../lib/net");
     var ace = require("../ace");
     module.exports = exports = ace;
     var getCSSProperty = function(element, container, property) {
         var ret = element.style[property];
         if (!ret) {
             if (window.getComputedStyle) {
                 ret = window.getComputedStyle(element, '').getPropertyValue(property);
@@ -151,24 +150,15 @@
                 container.style.height = e.clientY - rect.top + startY + "px";
                 editor.resize();
             }, function() {});
         });
         return editor;
     };
 
-    function load(url, module, callback) {
-        net.loadScript(url, function() {
-            require([module], callback);
-        });
-    }
-
     function setupApi(editor, editorDiv, settingDiv, ace, options) {
-        var session = editor.getSession();
-        var renderer = editor.renderer;
-
         function toBool(value) {
             return value === "true" || value == true;
         }
         editor.setDisplaySettings = function(display) {
             if (display == null)
                 display = settingDiv.style.display == "none";
             if (display) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-themelist.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-themelist.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/ext-whitespace.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/ext-whitespace.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/keybinding-emacs.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/keybinding-emacs.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/keybinding-sublime.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/keybinding-sublime.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/keybinding-vim.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/keybinding-vim.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/keybinding-vscode.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/keybinding-vscode.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-abap.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-abap.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-abc.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-abc.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-actionscript.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-actionscript.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ada.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ada.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-alda.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-alda.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-apache_conf.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-apache_conf.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-apex.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-apex.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-applescript.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-applescript.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-aql.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-aql.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-asciidoc.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-asciidoc.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-asl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-asl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-assembly_x86.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-assembly_x86.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-autohotkey.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-autohotkey.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-batchfile.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-batchfile.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-bibtex.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-bibtex.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-c9search.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-c9search.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-c_cpp.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-c_cpp.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-cirru.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-cirru.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-clojure.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-clojure.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-cobol.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-cobol.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-coffee.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-coffee.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-coldfusion.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-coldfusion.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-crystal.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-crystal.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-csharp.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-csharp.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-csound_document.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-csound_document.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-csound_orchestra.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-csound_orchestra.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-csound_score.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-csound_score.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-csp.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-csp.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-css.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-css.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-curly.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-curly.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-d.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-d.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-dart.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-dart.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-diff.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-diff.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-django.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-django.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-dockerfile.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-dockerfile.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-dot.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-dot.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-drools.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-drools.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-edifact.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-edifact.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-eiffel.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-eiffel.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ejs.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ejs.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-elixir.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-elixir.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-elm.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-elm.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-erlang.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-erlang.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-forth.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-forth.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-fortran.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-fortran.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-fsharp.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-fsharp.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-fsl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-fsl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ftl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ftl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-gcode.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-gcode.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-gherkin.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-gherkin.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-gitignore.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-gitignore.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-glsl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-glsl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-gobstones.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-gobstones.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-golang.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-golang.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-graphqlschema.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-graphqlschema.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-groovy.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-groovy.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-haml.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-haml.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-handlebars.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-handlebars.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-haskell.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-haskell.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-haskell_cabal.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-haskell_cabal.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-haxe.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-haxe.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-hjson.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-hjson.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-html.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-html.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-html_elixir.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-html_elixir.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-html_ruby.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-html_ruby.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ini.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ini.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-io.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-io.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ion.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ion.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jack.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jack.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jade.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jade.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-java.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-java.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-javascript.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-javascript.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jexl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jexl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-json.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-json.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-json5.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-json5.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jsoniq.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jsoniq.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jsp.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jsp.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jssm.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jssm.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-jsx.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-jsx.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-julia.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-julia.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-kotlin.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-kotlin.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-latex.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-latex.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-latte.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-latte.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-less.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-less.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-liquid.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-liquid.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-lisp.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-lisp.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-livescript.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-livescript.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-logiql.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-logiql.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-logtalk.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-logtalk.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-lsl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-lsl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-lua.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-lua.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-luapage.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-luapage.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-lucene.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-lucene.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-makefile.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-makefile.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-markdown.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-markdown.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mask.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mask.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-matlab.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-matlab.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-maze.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-maze.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mediawiki.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mediawiki.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mel.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mel.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mips.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mips.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mixal.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mixal.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mushcode.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mushcode.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-mysql.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-mysql.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-nginx.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-nginx.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-nim.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-nim.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-nix.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-nix.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-nsis.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-nsis.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
     "use strict";
     var oop = require("../lib/oop");
     var TextHighlightRules = require("./text_highlight_rules").TextHighlightRules;
     var NSISHighlightRules = function() {
         this.$rules = {
             start: [{
                 token: "keyword.compiler.nsis",
-                regex: /^\s*!(?:include|addincludedir|addplugindir|appendfile|cd|delfile|echo|error|execute|packhdr|pragma|finalize|getdllversion|gettlbversion|system|tempfile|warning|verbose|define|undef|insertmacro|macro|macroend|makensis|searchparse|searchreplace|uninstfinalize)\b/,
+                regex: /^\s*!(?:include|addincludedir|addplugindir|appendfile|assert|cd|delfile|echo|error|execute|packhdr|pragma|finalize|getdllversion|gettlbversion|system|tempfile|warning|verbose|define|undef|insertmacro|macro|macroend|makensis|searchparse|searchreplace|uninstfinalize)\b/,
                 caseInsensitive: true
             }, {
                 token: "keyword.command.nsis",
                 regex: /^\s*(?:Abort|AddBrandingImage|AddSize|AllowRootDirInstall|AllowSkipFiles|AutoCloseWindow|BGFont|BGGradient|BrandingText|BringToFront|Call|CallInstDLL|Caption|ChangeUI|CheckBitmap|ClearErrors|CompletedText|ComponentText|CopyFiles|CRCCheck|CreateDirectory|CreateFont|CreateShortCut|Delete|DeleteINISec|DeleteINIStr|DeleteRegKey|DeleteRegValue|DetailPrint|DetailsButtonText|DirText|DirVar|DirVerify|EnableWindow|EnumRegKey|EnumRegValue|Exch|Exec|ExecShell|ExecShellWait|ExecWait|ExpandEnvStrings|File|FileBufSize|FileClose|FileErrorText|FileOpen|FileRead|FileReadByte|FileReadUTF16LE|FileReadWord|FileWriteUTF16LE|FileSeek|FileWrite|FileWriteByte|FileWriteWord|FindClose|FindFirst|FindNext|FindWindow|FlushINI|GetCurInstType|GetCurrentAddress|GetDlgItem|GetDLLVersion|GetDLLVersionLocal|GetErrorLevel|GetFileTime|GetFileTimeLocal|GetFullPathName|GetFunctionAddress|GetInstDirError|GetKnownFolderPath|GetLabelAddress|GetTempFileName|GetWinVer|Goto|HideWindow|Icon|IfAbort|IfErrors|IfFileExists|IfRebootFlag|IfRtlLanguage|IfShellVarContextAll|IfSilent|InitPluginsDir|InstallButtonText|InstallColors|InstallDir|InstallDirRegKey|InstProgressFlags|InstType|InstTypeGetText|InstTypeSetText|Int64Cmp|Int64CmpU|Int64Fmt|IntCmp|IntCmpU|IntFmt|IntOp|IntPtrCmp|IntPtrCmpU|IntPtrOp|IsWindow|LangString|LicenseBkColor|LicenseData|LicenseForceSelection|LicenseLangString|LicenseText|LoadAndSetImage|LoadLanguageFile|LockWindow|LogSet|LogText|ManifestDPIAware|ManifestLongPathAware|ManifestMaxVersionTested|ManifestSupportedOS|MessageBox|MiscButtonText|Name|Nop|OutFile|Page|PageCallbacks|PEAddResource|PEDllCharacteristics|PERemoveResource|PESubsysVer|Pop|Push|Quit|ReadEnvStr|ReadINIStr|ReadRegDWORD|ReadRegStr|Reboot|RegDLL|Rename|RequestExecutionLevel|ReserveFile|Return|RMDir|SearchPath|SectionGetFlags|SectionGetInstTypes|SectionGetSize|SectionGetText|SectionIn|SectionSetFlags|SectionSetInstTypes|SectionSetSize|SectionSetText|SendMessage|SetAutoClose|SetBrandingImage|SetCompress|SetCompressor|SetCompressorDictSize|SetCtlColors|SetCurInstType|SetDatablockOptimize|SetDateSave|SetDetailsPrint|SetDetailsView|SetErrorLevel|SetErrors|SetFileAttributes|SetFont|SetOutPath|SetOverwrite|SetRebootFlag|SetRegView|SetShellVarContext|SetSilent|ShowInstDetails|ShowUninstDetails|ShowWindow|SilentInstall|SilentUnInstall|Sleep|SpaceTexts|StrCmp|StrCmpS|StrCpy|StrLen|SubCaption|Unicode|UninstallButtonText|UninstallCaption|UninstallIcon|UninstallSubCaption|UninstallText|UninstPage|UnRegDLL|Var|VIAddVersionKey|VIFileVersion|VIProductVersion|WindowIcon|WriteINIStr|WriteRegBin|WriteRegDWORD|WriteRegExpandStr|WriteRegMultiStr|WriteRegNone|WriteRegStr|WriteUninstaller|XPStyle)\b/,
                 caseInsensitive: true
             }, {
                 token: "keyword.control.nsis",
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-nunjucks.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-nunjucks.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-objectivec.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-objectivec.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ocaml.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ocaml.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-odin.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-odin.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-partiql.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-partiql.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-pascal.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-pascal.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-perl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-perl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-pgsql.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-pgsql.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-php.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-php.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-php_laravel_blade.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-php_laravel_blade.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-pig.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-pig.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-plain_text.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-plain_text.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-plsql.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-plsql.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-powershell.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-powershell.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-praat.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-praat.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-prisma.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-prisma.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-prolog.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-prolog.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-properties.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-properties.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-protobuf.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-protobuf.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-puppet.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-puppet.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-python.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-python.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-qml.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-qml.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-r.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-r.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-raku.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-raku.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-razor.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-razor.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-rdoc.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-rdoc.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-red.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-red.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-redshift.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-redshift.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-rhtml.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-rhtml.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-robot.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-robot.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-rst.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-rst.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-ruby.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-ruby.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-rust.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-rust.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sac.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sac.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sass.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sass.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-scad.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-scad.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-scala.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-scala.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-scheme.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-scheme.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-scrypt.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-scrypt.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-scss.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-scss.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sh.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sh.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sjs.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sjs.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-slim.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-slim.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-smarty.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-smarty.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-smithy.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-smithy.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-snippets.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-snippets.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-soy_template.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-soy_template.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-space.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-space.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sparql.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sparql.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sql.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sql.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-sqlserver.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-sqlserver.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-stylus.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-stylus.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-svg.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-svg.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-swift.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-swift.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-tcl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-tcl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-terraform.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-terraform.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-tex.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-tex.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-textile.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-textile.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-toml.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-toml.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-tsx.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-tsx.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-turtle.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-turtle.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-twig.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-twig.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-typescript.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-typescript.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-vala.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-vala.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-vbscript.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-vbscript.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-velocity.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-velocity.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-verilog.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-verilog.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-vhdl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-vhdl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-visualforce.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-visualforce.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-wollok.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-wollok.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-xml.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-xml.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-xquery.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-xquery.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-yaml.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-yaml.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/mode-zeek.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/mode-zeek.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/abc.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/abc.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/actionscript.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/actionscript.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/c_cpp.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/c_cpp.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/clojure.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/clojure.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/coffee.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/coffee.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/csound_document.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/csound_document.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/csound_orchestra.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/csound_orchestra.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/css.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/css.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/dart.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/dart.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/diff.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/diff.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/django.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/django.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/drools.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/drools.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/edifact.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/edifact.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/erlang.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/erlang.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/fsl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/fsl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/gobstones.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/gobstones.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/graphqlschema.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/graphqlschema.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/haml.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/haml.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/haskell.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/haskell.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/html.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/html.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/io.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/io.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/java.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/java.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/javascript.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/javascript.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/jsoniq.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/jsoniq.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/jsp.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/jsp.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/liquid.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/liquid.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/lsl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/lsl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/lua.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/lua.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/makefile.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/makefile.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/markdown.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/markdown.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/maze.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/maze.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/perl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/perl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/php.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/php.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/python.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/python.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/r.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/r.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/razor.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/razor.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/robot.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/robot.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/rst.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/rst.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/ruby.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/ruby.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/sh.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/sh.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/snippets.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/snippets.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/sql.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/sql.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/sqlserver.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/sqlserver.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/tcl.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/tcl.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/tex.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/tex.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/textile.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/textile.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/vala.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/vala.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/velocity.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/velocity.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/wollok.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/wollok.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/snippets/xquery.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/snippets/xquery.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-ambiance.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-ambiance.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/ambiance.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/ambiance-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-ambiance .ace_gutter {\n  background-color: #3d3d3d;\n  background-image: linear-gradient(left, #3D3D3D, #333);\n  background-repeat: repeat-x;\n  border-right: 1px solid #4d4d4d;\n  text-shadow: 0px 1px 1px #4d4d4d;\n  color: #222;\n}\n\n.ace-ambiance .ace_gutter-layer {\n  background: repeat left top;\n}\n\n.ace-ambiance .ace_gutter-active-line {\n  background-color: #3F3F3F;\n}\n\n.ace-ambiance .ace_fold-widget {\n  text-align: center;\n}\n\n.ace-ambiance .ace_fold-widget:hover {\n  color: #777;\n}\n\n.ace-ambiance .ace_fold-widget.ace_start,\n.ace-ambiance .ace_fold-widget.ace_end,\n.ace-ambiance .ace_fold-widget.ace_closed{\n  background: none !important;\n  border: none;\n  box-shadow: none;\n}\n\n.ace-ambiance .ace_fold-widget.ace_start:after {\n  content: '\u25BE'\n}\n\n.ace-ambiance .ace_fold-widget.ace_end:after {\n  content: '\u25B4'\n}\n\n.ace-ambiance .ace_fold-widget.ace_closed:after {\n  content: '\u2023'\n}\n\n.ace-ambiance .ace_print-margin {\n  border-left: 1px dotted #2D2D2D;\n  right: 0;\n  background: #262626;\n}\n\n.ace-ambiance .ace_scroller {\n  -webkit-box-shadow: inset 0 0 10px black;\n  -moz-box-shadow: inset 0 0 10px black;\n  -o-box-shadow: inset 0 0 10px black;\n  box-shadow: inset 0 0 10px black;\n}\n\n.ace-ambiance {\n  color: #E6E1DC;\n  background-color: #202020;\n}\n\n.ace-ambiance .ace_cursor {\n  border-left: 1px solid #7991E8;\n}\n\n.ace-ambiance .ace_overwrite-cursors .ace_cursor {\n  border: 1px solid #FFE300;\n  background: #766B13;\n}\n\n.ace-ambiance.normal-mode .ace_cursor-layer {\n  z-index: 0;\n}\n \n.ace-ambiance .ace_marker-layer .ace_selection {\n  background: rgba(221, 240, 255, 0.20);\n}\n\n.ace-ambiance .ace_marker-layer .ace_selected-word {\n  border-radius: 4px;\n  border: 8px solid #3f475d;\n  box-shadow: 0 0 4px black;\n}\n\n.ace-ambiance .ace_marker-layer .ace_step {\n  background: rgb(198, 219, 174);\n}\n\n.ace-ambiance .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(255, 255, 255, 0.25);\n}\n\n.ace-ambiance .ace_marker-layer .ace_active-line {\n  background: rgba(255, 255, 255, 0.031);\n}\n\n.ace-ambiance .ace_invisible {\n  color: #333;\n}\n\n.ace-ambiance .ace_paren {\n  color: #24C2C7;\n}\n\n.ace-ambiance .ace_keyword {\n  color: #cda869;\n}\n\n.ace-ambiance .ace_keyword.ace_operator {\n  color: #fa8d6a;\n}\n\n.ace-ambiance .ace_punctuation.ace_operator {\n  color: #fa8d6a;\n}\n\n.ace-ambiance .ace_identifier {\n}\n\n.ace-ambiance .ace-statement {\n  color: #cda869;\n}\n\n.ace-ambiance .ace_constant {\n  color: #CF7EA9;\n}\n\n.ace-ambiance .ace_constant.ace_language {\n  color: #CF7EA9;\n}\n\n.ace-ambiance .ace_constant.ace_library {\n  \n}\n\n.ace-ambiance .ace_constant.ace_numeric {\n  color: #78CF8A;\n}\n\n.ace-ambiance .ace_invalid {\n  text-decoration: underline;\n}\n\n.ace-ambiance .ace_invalid.ace_illegal {\n  color:#F8F8F8;\n  background-color: rgba(86, 45, 86, 0.75);\n}\n\n.ace-ambiance .ace_invalid,\n.ace-ambiance .ace_deprecated {\n  text-decoration: underline;\n  font-style: italic;\n  color: #D2A8A1;\n}\n\n.ace-ambiance .ace_support {\n  color: #9B859D;\n}\n\n.ace-ambiance .ace_support.ace_function {\n  color: #DAD085;\n}\n\n.ace-ambiance .ace_function.ace_buildin {\n  color: #9b859d;\n}\n\n.ace-ambiance .ace_string {\n  color: #8f9d6a;\n}\n\n.ace-ambiance .ace_string.ace_regexp {\n  color: #DAD085;\n}\n\n.ace-ambiance .ace_comment {\n  font-style: italic;\n  color: #555;\n}\n\n.ace-ambiance .ace_comment.ace_doc {\n}\n\n.ace-ambiance .ace_comment.ace_doc.ace_tag {\n  color: #666;\n  font-style: normal;\n}\n\n.ace-ambiance .ace_definition,\n.ace-ambiance .ace_type {\n  color: #aac6e3;\n}\n\n.ace-ambiance .ace_variable {\n  color: #9999cc;\n}\n\n.ace-ambiance .ace_variable.ace_language {\n  color: #9b859d;\n}\n\n.ace-ambiance .ace_xml-pe {\n  color: #494949;\n}\n\n.ace-ambiance .ace_gutter-layer,\n.ace-ambiance .ace_text-layer {\n  background-image: url(\"data:image/png;base64,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\");\n}\n\n.ace-ambiance .ace_indent-guide {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNQUFD4z6Crq/sfAAuYAuYl+7lfAAAAAElFTkSuQmCC\") right repeat-y;\n}\n\n.ace-ambiance .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/ambiance", ["require", "exports", "module", "ace/theme/ambiance.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/ambiance", ["require", "exports", "module", "ace/theme/ambiance-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-ambiance";
-    exports.cssText = require("./ambiance.css");
+    exports.cssText = require("./ambiance-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/ambiance"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-chaos.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-chaos.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/chaos.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/chaos-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-chaos .ace_gutter {\n  background: #141414;\n  color: #595959;\n  border-right: 1px solid #282828;\n}\n.ace-chaos .ace_gutter-cell.ace_warning {\n  background-image: none;\n  background: #FC0;\n  border-left: none;\n  padding-left: 0;\n  color: #000;\n}\n.ace-chaos .ace_gutter-cell.ace_error {\n  background-position: -6px center;\n  background-image: none;\n  background: #F10;\n  border-left: none;\n  padding-left: 0;\n  color: #000;\n}\n.ace-chaos .ace_print-margin {\n  border-left: 1px solid #555;\n  right: 0;\n  background: #1D1D1D;\n}\n.ace-chaos {\n  background-color: #161616;\n  color: #E6E1DC;\n}\n\n.ace-chaos .ace_cursor {\n  border-left: 2px solid #FFFFFF;\n}\n.ace-chaos .ace_cursor.ace_overwrite {\n  border-left: 0px;\n  border-bottom: 1px solid #FFFFFF;\n}\n.ace-chaos .ace_marker-layer .ace_selection {\n  background: #494836;\n}\n.ace-chaos .ace_marker-layer .ace_step {\n  background: rgb(198, 219, 174);\n}\n.ace-chaos .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #FCE94F;\n}\n.ace-chaos .ace_marker-layer .ace_active-line {\n  background: #333;\n}\n.ace-chaos .ace_gutter-active-line {\n  background-color: #222;\n}\n.ace-chaos .ace_invisible {\n  color: #404040;\n}\n.ace-chaos .ace_keyword {\n  color:#00698F;\n}\n.ace-chaos .ace_keyword.ace_operator {\n  color:#FF308F;\n}\n.ace-chaos .ace_constant {\n  color:#1EDAFB;\n}\n.ace-chaos .ace_constant.ace_language {\n  color:#FDC251;\n}\n.ace-chaos .ace_constant.ace_library {\n  color:#8DFF0A;\n}\n.ace-chaos .ace_constant.ace_numeric {\n  color:#58C554;\n}\n.ace-chaos .ace_invalid {\n  color:#FFFFFF;\n  background-color:#990000;\n}\n.ace-chaos .ace_invalid.ace_deprecated {\n  color:#FFFFFF;\n  background-color:#990000;\n}\n.ace-chaos .ace_support {\n  color: #999;\n}\n.ace-chaos .ace_support.ace_function {\n  color:#00AEEF;\n}\n.ace-chaos .ace_function {\n  color:#00AEEF;\n}\n.ace-chaos .ace_string {\n  color:#58C554;\n}\n.ace-chaos .ace_comment {\n  color:#555;\n  font-style:italic;\n  padding-bottom: 0px;\n}\n.ace-chaos .ace_variable {\n  color:#997744;\n}\n.ace-chaos .ace_meta.ace_tag {\n  color:#BE53E6;\n}\n.ace-chaos .ace_entity.ace_other.ace_attribute-name {\n  color:#FFFF89;\n}\n.ace-chaos .ace_markup.ace_underline {\n  text-decoration: underline;\n}\n.ace-chaos .ace_fold-widget {\n  text-align: center;\n}\n\n.ace-chaos .ace_fold-widget:hover {\n  color: #777;\n}\n\n.ace-chaos .ace_fold-widget.ace_start,\n.ace-chaos .ace_fold-widget.ace_end,\n.ace-chaos .ace_fold-widget.ace_closed{\n  background: none !important;\n  border: none;\n  box-shadow: none;\n}\n\n.ace-chaos .ace_fold-widget.ace_start:after {\n  content: '\u25BE'\n}\n\n.ace-chaos .ace_fold-widget.ace_end:after {\n  content: '\u25B4'\n}\n\n.ace-chaos .ace_fold-widget.ace_closed:after {\n  content: '\u2023'\n}\n\n.ace-chaos .ace_indent-guide {\n  border-right:1px dotted #333333;\n  margin-right:-1px;\n}\n\n.ace-chaos .ace_indent-guide-active {\n  border-right:1px dotted #afafaf;\n  margin-right:-1px;\n}\n\n.ace-chaos .ace_fold { \n  background: #222; \n  border-radius: 3px; \n  color: #7AF; \n  border: none; \n}\n.ace-chaos .ace_fold:hover {\n  background: #CCC; \n  color: #000;\n}\n";
 
 });
 
-define("ace/theme/chaos", ["require", "exports", "module", "ace/theme/chaos.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/chaos", ["require", "exports", "module", "ace/theme/chaos-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-chaos";
-    exports.cssText = require("./chaos.css");
+    exports.cssText = require("./chaos-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/chaos"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-chrome.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-chrome.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/chrome.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/chrome-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-chrome .ace_gutter {\n  background: #ebebeb;\n  color: #333;\n  overflow : hidden;\n}\n\n.ace-chrome .ace_print-margin {\n  width: 1px;\n  background: #e8e8e8;\n}\n\n.ace-chrome {\n  background-color: #FFFFFF;\n  color: black;\n}\n\n.ace-chrome .ace_cursor {\n  color: black;\n}\n\n.ace-chrome .ace_invisible {\n  color: rgb(191, 191, 191);\n}\n\n.ace-chrome .ace_constant.ace_buildin {\n  color: rgb(88, 72, 246);\n}\n\n.ace-chrome .ace_constant.ace_language {\n  color: rgb(88, 92, 246);\n}\n\n.ace-chrome .ace_constant.ace_library {\n  color: rgb(6, 150, 14);\n}\n\n.ace-chrome .ace_invalid {\n  background-color: rgb(153, 0, 0);\n  color: white;\n}\n\n.ace-chrome .ace_fold {\n}\n\n.ace-chrome .ace_support.ace_function {\n  color: rgb(60, 76, 114);\n}\n\n.ace-chrome .ace_support.ace_constant {\n  color: rgb(6, 150, 14);\n}\n\n.ace-chrome .ace_support.ace_type,\n.ace-chrome .ace_support.ace_class\n.ace-chrome .ace_support.ace_other {\n  color: rgb(109, 121, 222);\n}\n\n.ace-chrome .ace_variable.ace_parameter {\n  font-style:italic;\n  color:#FD971F;\n}\n.ace-chrome .ace_keyword.ace_operator {\n  color: rgb(104, 118, 135);\n}\n\n.ace-chrome .ace_comment {\n  color: #236e24;\n}\n\n.ace-chrome .ace_comment.ace_doc {\n  color: #236e24;\n}\n\n.ace-chrome .ace_comment.ace_doc.ace_tag {\n  color: #236e24;\n}\n\n.ace-chrome .ace_constant.ace_numeric {\n  color: rgb(0, 0, 205);\n}\n\n.ace-chrome .ace_variable {\n  color: rgb(49, 132, 149);\n}\n\n.ace-chrome .ace_xml-pe {\n  color: rgb(104, 104, 91);\n}\n\n.ace-chrome .ace_entity.ace_name.ace_function {\n  color: #0000A2;\n}\n\n\n.ace-chrome .ace_heading {\n  color: rgb(12, 7, 255);\n}\n\n.ace-chrome .ace_list {\n  color:rgb(185, 6, 144);\n}\n\n.ace-chrome .ace_marker-layer .ace_selection {\n  background: rgb(181, 213, 255);\n}\n\n.ace-chrome .ace_marker-layer .ace_step {\n  background: rgb(252, 255, 0);\n}\n\n.ace-chrome .ace_marker-layer .ace_stack {\n  background: rgb(164, 229, 101);\n}\n\n.ace-chrome .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgb(192, 192, 192);\n}\n\n.ace-chrome .ace_marker-layer .ace_active-line {\n  background: rgba(0, 0, 0, 0.07);\n}\n\n.ace-chrome .ace_gutter-active-line {\n    background-color : #dcdcdc;\n}\n\n.ace-chrome .ace_marker-layer .ace_selected-word {\n  background: rgb(250, 250, 255);\n  border: 1px solid rgb(200, 200, 250);\n}\n\n.ace-chrome .ace_storage,\n.ace-chrome .ace_keyword,\n.ace-chrome .ace_meta.ace_tag {\n  color: rgb(147, 15, 128);\n}\n\n.ace-chrome .ace_string.ace_regex {\n  color: rgb(255, 0, 0)\n}\n\n.ace-chrome .ace_string {\n  color: #1A1AA6;\n}\n\n.ace-chrome .ace_entity.ace_other.ace_attribute-name {\n  color: #994409;\n}\n\n.ace-chrome .ace_indent-guide {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bLly//BwAmVgd1/w11/gAAAABJRU5ErkJggg==\") right repeat-y;\n}\n  \n.ace-chrome .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/chrome", ["require", "exports", "module", "ace/theme/chrome.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/chrome", ["require", "exports", "module", "ace/theme/chrome-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
     exports.cssClass = "ace-chrome";
-    exports.cssText = require("./chrome.css");
+    exports.cssText = require("./chrome-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/chrome"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-cloud9_day.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-cloud9_day.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
-define("ace/theme/cloud9_day.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/cloud9_day-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-cloud9-day .ace_gutter {\n    background: #ECECEC;\n    color: #333;\n}\n\n.ace-cloud9-day .ace_print-margin {\n    width: 1px;\n    background: #e8e8e8;\n}\n\n.ace-cloud9-day .ace_fold {\n    background-color: #6B72E6;\n}\n\n.ace-cloud9-day {\n    background-color: #FBFBFB;\n    color: black;\n}\n\n.ace-cloud9-day .ace_cursor {\n    color: black;\n}\n\n.ace-cloud9-day .ace_invisible {\n    color: rgb(191, 191, 191);\n}\n\n.ace-cloud9-day .ace_storage,\n.ace-cloud9-day .ace_keyword {\n    color: rgb(24, 122, 234);\n}\n\n.ace-cloud9-day .ace_constant {\n    color: rgb(197, 6, 11);\n}\n\n.ace-cloud9-day .ace_constant.ace_buildin {\n    color: rgb(88, 72, 246);\n}\n\n.ace-cloud9-day .ace_constant.ace_language {\n    color: rgb(88, 92, 246);\n}\n\n.ace-cloud9-day .ace_constant.ace_library {\n    color: rgb(6, 150, 14);\n}\n\n.ace-cloud9-day .ace_invalid {\n    background-color: rgba(255, 0, 0, 0.1);\n    color: red;\n}\n\n.ace-cloud9-day .ace_support.ace_function {\n    color: rgb(60, 76, 114);\n}\n\n.ace-cloud9-day .ace_support.ace_constant {\n    color: rgb(6, 150, 14);\n}\n\n.ace-cloud9-day .ace_support.ace_type,\n.ace-cloud9-day .ace_support.ace_class {\n    color: rgb(109, 121, 222);\n}\n\n.ace-cloud9-day .ace_keyword.ace_operator {\n    color: rgb(104, 118, 135);\n}\n\n.ace-cloud9-day .ace_string {\n    color: rgb(3, 106, 7);\n}\n\n.ace-cloud9-day .ace_comment {\n    color: rgb(76, 136, 107);\n}\n\n.ace-cloud9-day .ace_comment.ace_doc {\n    color: rgb(0, 102, 255);\n}\n\n.ace-cloud9-day .ace_comment.ace_doc.ace_tag {\n    color: rgb(128, 159, 191);\n}\n\n.ace-cloud9-day .ace_constant.ace_numeric {\n    color: rgb(0, 0, 205);\n}\n\n.ace-cloud9-day .ace_variable {\n    color: rgb(49, 132, 149);\n}\n\n.ace-cloud9-day .ace_xml-pe {\n    color: rgb(104, 104, 91);\n}\n\n.ace-cloud9-day .ace_entity.ace_name.ace_function {\n    color: #0000A2;\n}\n\n\n.ace-cloud9-day .ace_heading {\n    color: rgb(12, 7, 255);\n}\n\n.ace-cloud9-day .ace_list {\n    color: rgb(185, 6, 144);\n}\n\n.ace-cloud9-day .ace_meta.ace_tag {\n    color: rgb(0, 22, 142);\n}\n\n.ace-cloud9-day .ace_string.ace_regex {\n    color: rgb(255, 0, 0)\n}\n\n.ace-cloud9-day .ace_marker-layer .ace_selection {\n    background: rgb(181, 213, 255);\n}\n\n.ace-cloud9-day.ace_multiselect .ace_selection.ace_start {\n    box-shadow: 0 0 3px 0px white;\n}\n\n.ace-cloud9-day .ace_marker-layer .ace_step {\n    background: rgb(247, 237, 137);\n}\n\n.ace-cloud9-day .ace_marker-layer .ace_stack {\n    background: #BAE0A0;\n}\n\n.ace-cloud9-day .ace_marker-layer .ace_bracket {\n    margin: -1px 0 0 -1px;\n    border: 1px solid rgb(192, 192, 192);\n}\n\n.ace-cloud9-day .ace_marker-layer .ace_active-line {\n    background: rgba(0, 0, 0, 0.07);\n}\n\n.ace-cloud9-day .ace_gutter-active-line {\n    background-color: #E5E5E5;\n}\n\n.ace-cloud9-day .ace_marker-layer .ace_selected-word {\n    background: rgb(250, 250, 255);\n    border: 1px solid rgb(200, 200, 250);\n}\n\n.ace-cloud9-day .ace_indent-guide {\n    background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bLly//BwAmVgd1/w11/gAAAABJRU5ErkJggg==\") right repeat-y;\n}\n\n.ace-cloud9-day .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n} \n";
 
 });
 
-define("ace/theme/cloud9_day", ["require", "exports", "module", "ace/theme/cloud9_day.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/cloud9_day", ["require", "exports", "module", "ace/theme/cloud9_day-css", "ace/lib/dom"], function(require, exports, module) {
     "use strict";
     exports.isDark = false;
     exports.cssClass = "ace-cloud9-day";
-    exports.cssText = require("./cloud9_day.css");
+    exports.cssText = require("./cloud9_day-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass);
 
 });
 (function() {
     window.require(["ace/theme/cloud9_day"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-cloud9_night.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-cloud9_night.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/cloud9_night.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/cloud9_night-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-cloud9-night .ace_gutter {\n    background: #303130;\n    color: #eee\n}\n\n.ace-cloud9-night .ace_print-margin {\n    width: 1px;\n    background: #222\n}\n\n.ace-cloud9-night {\n    background-color: #181818;\n    color: #EBEBEB\n}\n\n.ace-cloud9-night .ace_cursor {\n    color: #9F9F9F\n}\n\n.ace-cloud9-night .ace_marker-layer .ace_selection {\n    background: #424242\n}\n\n.ace-cloud9-night.ace_multiselect .ace_selection.ace_start {\n    box-shadow: 0 0 3px 0px #000000;\n    border-radius: 2px\n}\n\n.ace-cloud9-night .ace_marker-layer .ace_step {\n    background: rgb(102, 82, 0)\n}\n\n.ace-cloud9-night .ace_marker-layer .ace_bracket {\n    margin: -1px 0 0 -1px;\n    border: 1px solid #888888\n}\n\n.ace-cloud9-night .ace_marker-layer .ace_highlight {\n    border: 1px solid rgb(110, 119, 0);\n    border-bottom: 0;\n    box-shadow: inset 0 -1px rgb(110, 119, 0);\n    margin: -1px 0 0 -1px;\n    background: rgba(255, 235, 0, 0.1);\n}\n\n.ace-cloud9-night .ace_marker-layer .ace_active-line {\n    background: #292929\n}\n\n.ace-cloud9-night .ace_gutter-active-line {\n    background-color: #3D3D3D\n}\n\n.ace-cloud9-night .ace_stack {\n    background-color: rgb(66, 90, 44)\n}\n\n.ace-cloud9-night .ace_marker-layer .ace_selected-word {\n    border: 1px solid #888888\n}\n\n.ace-cloud9-night .ace_invisible {\n    color: #343434\n}\n\n.ace-cloud9-night .ace_keyword,\n.ace-cloud9-night .ace_meta,\n.ace-cloud9-night .ace_storage,\n.ace-cloud9-night .ace_storage.ace_type,\n.ace-cloud9-night .ace_support.ace_type {\n    color: #C397D8\n}\n\n.ace-cloud9-night .ace_keyword.ace_operator {\n    color: #70C0B1\n}\n\n.ace-cloud9-night .ace_constant.ace_character,\n.ace-cloud9-night .ace_constant.ace_language,\n.ace-cloud9-night .ace_constant.ace_numeric,\n.ace-cloud9-night .ace_keyword.ace_other.ace_unit,\n.ace-cloud9-night .ace_support.ace_constant,\n.ace-cloud9-night .ace_variable.ace_parameter {\n    color: #E78C45\n}\n\n.ace-cloud9-night .ace_constant.ace_other {\n    color: #EEEEEE\n}\n\n.ace-cloud9-night .ace_invalid {\n    color: #CED2CF;\n    background-color: #DF5F5F\n}\n\n.ace-cloud9-night .ace_invalid.ace_deprecated {\n    color: #CED2CF;\n    background-color: #B798BF\n}\n\n.ace-cloud9-night .ace_fold {\n    background-color: #7AA6DA;\n    border-color: #DEDEDE\n}\n\n.ace-cloud9-night .ace_entity.ace_name.ace_function,\n.ace-cloud9-night .ace_support.ace_function,\n.ace-cloud9-night .ace_variable:not(.ace_parameter),\n.ace-cloud9-night .ace_constant:not(.ace_numeric) {\n    color: #7AA6DA\n}\n\n.ace-cloud9-night .ace_support.ace_class,\n.ace-cloud9-night .ace_support.ace_type {\n    color: #E7C547\n}\n\n.ace-cloud9-night .ace_heading,\n.ace-cloud9-night .ace_markup.ace_heading,\n.ace-cloud9-night .ace_string {\n    color: #B9CA4A\n}\n\n.ace-cloud9-night .ace_entity.ace_name.ace_tag,\n.ace-cloud9-night .ace_entity.ace_other.ace_attribute-name,\n.ace-cloud9-night .ace_meta.ace_tag,\n.ace-cloud9-night .ace_string.ace_regexp,\n.ace-cloud9-night .ace_variable {\n    color: #D54E53\n}\n\n.ace-cloud9-night .ace_comment {\n    color: #969896\n}\n\n.ace-cloud9-night .ace_c9searchresults.ace_keyword {\n    color: #C2C280;\n}\n\n.ace-cloud9-night .ace_indent-guide {\n    background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYFBXV/8PAAJoAXX4kT2EAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-cloud9-night .ace_indent-guide-active {\n    background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/cloud9_night", ["require", "exports", "module", "ace/theme/cloud9_night.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/cloud9_night", ["require", "exports", "module", "ace/theme/cloud9_night-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-cloud9-night";
-    exports.cssText = require("./cloud9_night.css");
+    exports.cssText = require("./cloud9_night-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass);
 
 });
 (function() {
     window.require(["ace/theme/cloud9_night"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-cloud9_night_low_color.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-cloud9_night_low_color.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/cloud9_night_low_color.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/cloud9_night_low_color-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-cloud9-night-low-color .ace_gutter {\n    background: #303130;\n    color: #eee\n}\n\n.ace-cloud9-night-low-color .ace_print-margin {\n    width: 1px;\n    background: #222\n}\n\n.ace-cloud9-night-low-color {\n    background-color: #181818;\n    color: #EBEBEB\n}\n\n.ace-cloud9-night-low-color .ace_cursor {\n    color: #9F9F9F\n}\n\n.ace-cloud9-night-low-color .ace_marker-layer .ace_selection {\n    background: #424242\n}\n\n.ace-cloud9-night-low-color.ace_multiselect .ace_selection.ace_start {\n    box-shadow: 0 0 3px 0px #000000;\n    border-radius: 2px\n}\n\n.ace-cloud9-night-low-color .ace_marker-layer .ace_step {\n    background: rgb(102, 82, 0)\n}\n\n.ace-cloud9-night-low-color .ace_marker-layer .ace_bracket {\n    margin: -1px 0 0 -1px;\n    border: 1px solid #888888\n}\n\n.ace-cloud9-night-low-color .ace_marker-layer .ace_highlight {\n    border: 1px solid rgb(110, 119, 0);\n    border-bottom: 0;\n    box-shadow: inset 0 -1px rgb(110, 119, 0);\n    margin: -1px 0 0 -1px;\n    background: rgba(255, 235, 0, 0.1);\n}\n\n.ace-cloud9-night-low-color .ace_marker-layer .ace_active-line {\n    background: #292929\n}\n\n.ace-cloud9-night-low-color .ace_gutter-active-line {\n    background-color: #3D3D3D\n}\n\n.ace-cloud9-night-low-color .ace_stack {\n    background-color: rgb(66, 90, 44)\n}\n\n.ace-cloud9-night-low-color .ace_marker-layer .ace_selected-word {\n    border: 1px solid #888888\n}\n\n.ace-cloud9-night-low-color .ace_invisible {\n    color: #343434\n}\n\n.ace-cloud9-night-low-color .ace_keyword,\n.ace-cloud9-night-low-color .ace_meta,\n.ace-cloud9-night-low-color .ace_storage {\n    color: #C397D8\n}\n\n.ace-cloud9-night-low-color .ace_keyword.ace_operator {\n    color: #70C0B1\n}\n\n.ace-cloud9-night-low-color .ace_constant.ace_character,\n.ace-cloud9-night-low-color .ace_constant.ace_language,\n.ace-cloud9-night-low-color .ace_constant.ace_numeric,\n.ace-cloud9-night-low-color .ace_keyword.ace_other.ace_unit {\n    color: #DAA637\n}\n\n.ace-cloud9-night-low-color .ace_constant.ace_other {\n    color: #EEEEEE\n}\n\n.ace-cloud9-night-low-color .ace_invalid {\n    color: #CED2CF;\n    background-color: #DF5F5F\n}\n\n.ace-cloud9-night-low-color .ace_invalid.ace_deprecated {\n    color: #CED2CF;\n    background-color: #B798BF\n}\n\n.ace-cloud9-night-low-color .ace_fold {\n    background-color: #7AA6DA;\n    border-color: #DEDEDE\n}\n\n.ace-cloud9-night-low-color .ace_entity.ace_name.ace_function,\n.ace-cloud9-night-low-color .ace_support.ace_function,\n.ace-cloud9-night-low-color .ace_variable:not(.ace_parameter),\n.ace-cloud9-night-low-color .ace_constant:not(.ace_numeric) {\n    color: #7AA6DA\n}\n\n.ace-cloud9-night-low-color .ace_support.ace_class,\n.ace-cloud9-night-low-color .ace_support.ace_type {\n    color: #E7C547\n}\n\n.ace-cloud9-night-low-color .ace_heading,\n.ace-cloud9-night-low-color .ace_markup.ace_heading,\n.ace-cloud9-night-low-color .ace_string {\n    color: #B9CA4A\n}\n\n.ace-cloud9-night-low-color .ace_comment {\n    color: #969896\n}\n\n.ace-cloud9-night-low-color .ace_c9searchresults.ace_keyword {\n    color: #C2C280;\n}\n\n.ace-cloud9-night-low-color .ace_indent-guide {\n    background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYFBXV/8PAAJoAXX4kT2EAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-cloud9-night-low-color .ace_indent-guide-active {\n    background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/cloud9_night_low_color", ["require", "exports", "module", "ace/theme/cloud9_night_low_color.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/cloud9_night_low_color", ["require", "exports", "module", "ace/theme/cloud9_night_low_color-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-cloud9-night-low-color";
-    exports.cssText = require("./cloud9_night_low_color.css");
+    exports.cssText = require("./cloud9_night_low_color-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass);
 
 });
 (function() {
     window.require(["ace/theme/cloud9_night_low_color"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-clouds.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-clouds.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/clouds.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/clouds-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-clouds .ace_gutter {\n  background: #ebebeb;\n  color: #333\n}\n\n.ace-clouds .ace_print-margin {\n  width: 1px;\n  background: #e8e8e8\n}\n\n.ace-clouds {\n  background-color: #FFFFFF;\n  color: #000000\n}\n\n.ace-clouds .ace_cursor {\n  color: #000000\n}\n\n.ace-clouds .ace_marker-layer .ace_selection {\n  background: #BDD5FC\n}\n\n.ace-clouds.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #FFFFFF;\n}\n\n.ace-clouds .ace_marker-layer .ace_step {\n  background: rgb(255, 255, 0)\n}\n\n.ace-clouds .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #BFBFBF\n}\n\n.ace-clouds .ace_marker-layer .ace_active-line {\n  background: #FFFBD1\n}\n\n.ace-clouds .ace_gutter-active-line {\n  background-color : #dcdcdc\n}\n\n.ace-clouds .ace_marker-layer .ace_selected-word {\n  border: 1px solid #BDD5FC\n}\n\n.ace-clouds .ace_invisible {\n  color: #BFBFBF\n}\n\n.ace-clouds .ace_keyword,\n.ace-clouds .ace_meta,\n.ace-clouds .ace_support.ace_constant.ace_property-value {\n  color: #AF956F\n}\n\n.ace-clouds .ace_keyword.ace_operator {\n  color: #484848\n}\n\n.ace-clouds .ace_keyword.ace_other.ace_unit {\n  color: #96DC5F\n}\n\n.ace-clouds .ace_constant.ace_language {\n  color: #39946A\n}\n\n.ace-clouds .ace_constant.ace_numeric {\n  color: #46A609\n}\n\n.ace-clouds .ace_constant.ace_character.ace_entity {\n  color: #BF78CC\n}\n\n.ace-clouds .ace_invalid {\n  background-color: #FF002A\n}\n\n.ace-clouds .ace_fold {\n  background-color: #AF956F;\n  border-color: #000000\n}\n\n.ace-clouds .ace_storage,\n.ace-clouds .ace_support.ace_class,\n.ace-clouds .ace_support.ace_function,\n.ace-clouds .ace_support.ace_other,\n.ace-clouds .ace_support.ace_type {\n  color: #C52727\n}\n\n.ace-clouds .ace_string {\n  color: #5D90CD\n}\n\n.ace-clouds .ace_comment {\n  color: #BCC8BA\n}\n\n.ace-clouds .ace_entity.ace_name.ace_tag,\n.ace-clouds .ace_entity.ace_other.ace_attribute-name {\n  color: #606060\n}\n\n.ace-clouds .ace_indent-guide {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bLly//BwAmVgd1/w11/gAAAABJRU5ErkJggg==\") right repeat-y\n}\n\n.ace-clouds .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n} \n";
 
 });
 
-define("ace/theme/clouds", ["require", "exports", "module", "ace/theme/clouds.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/clouds", ["require", "exports", "module", "ace/theme/clouds-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
     exports.cssClass = "ace-clouds";
-    exports.cssText = require("./clouds.css");
+    exports.cssText = require("./clouds-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/clouds"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-clouds_midnight.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-clouds_midnight.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/clouds_midnight.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/clouds_midnight-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-clouds-midnight .ace_gutter {\n  background: #232323;\n  color: #929292\n}\n\n.ace-clouds-midnight .ace_print-margin {\n  width: 1px;\n  background: #232323\n}\n\n.ace-clouds-midnight {\n  background-color: #191919;\n  color: #929292\n}\n\n.ace-clouds-midnight .ace_cursor {\n  color: #7DA5DC\n}\n\n.ace-clouds-midnight .ace_marker-layer .ace_selection {\n  background: #000000\n}\n\n.ace-clouds-midnight.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #191919;\n}\n\n.ace-clouds-midnight .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-clouds-midnight .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #BFBFBF\n}\n\n.ace-clouds-midnight .ace_marker-layer .ace_active-line {\n  background: rgba(215, 215, 215, 0.031)\n}\n\n.ace-clouds-midnight .ace_gutter-active-line {\n  background-color: rgba(215, 215, 215, 0.031)\n}\n\n.ace-clouds-midnight .ace_marker-layer .ace_selected-word {\n  border: 1px solid #000000\n}\n\n.ace-clouds-midnight .ace_invisible {\n  color: #666\n}\n\n.ace-clouds-midnight .ace_keyword,\n.ace-clouds-midnight .ace_meta,\n.ace-clouds-midnight .ace_support.ace_constant.ace_property-value {\n  color: #927C5D\n}\n\n.ace-clouds-midnight .ace_keyword.ace_operator {\n  color: #4B4B4B\n}\n\n.ace-clouds-midnight .ace_keyword.ace_other.ace_unit {\n  color: #366F1A\n}\n\n.ace-clouds-midnight .ace_constant.ace_language {\n  color: #39946A\n}\n\n.ace-clouds-midnight .ace_constant.ace_numeric {\n  color: #46A609\n}\n\n.ace-clouds-midnight .ace_constant.ace_character.ace_entity {\n  color: #A165AC\n}\n\n.ace-clouds-midnight .ace_invalid {\n  color: #FFFFFF;\n  background-color: #E92E2E\n}\n\n.ace-clouds-midnight .ace_fold {\n  background-color: #927C5D;\n  border-color: #929292\n}\n\n.ace-clouds-midnight .ace_storage,\n.ace-clouds-midnight .ace_support.ace_class,\n.ace-clouds-midnight .ace_support.ace_function,\n.ace-clouds-midnight .ace_support.ace_other,\n.ace-clouds-midnight .ace_support.ace_type {\n  color: #E92E2E\n}\n\n.ace-clouds-midnight .ace_string {\n  color: #5D90CD\n}\n\n.ace-clouds-midnight .ace_comment {\n  color: #3C403B\n}\n\n.ace-clouds-midnight .ace_entity.ace_name.ace_tag,\n.ace-clouds-midnight .ace_entity.ace_other.ace_attribute-name {\n  color: #606060\n}\n\n.ace-clouds-midnight .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYHB3d/8PAAOIAdULw8qMAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-clouds-midnight .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/clouds_midnight", ["require", "exports", "module", "ace/theme/clouds_midnight.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/clouds_midnight", ["require", "exports", "module", "ace/theme/clouds_midnight-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-clouds-midnight";
-    exports.cssText = require("./clouds_midnight.css");
+    exports.cssText = require("./clouds_midnight-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/clouds_midnight"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-cobalt.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-cobalt.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/cobalt.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/cobalt-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-cobalt .ace_gutter {\n  background: #011e3a;\n  color: rgb(128,145,160)\n}\n\n.ace-cobalt .ace_print-margin {\n  width: 1px;\n  background: #555555\n}\n\n.ace-cobalt {\n  background-color: #002240;\n  color: #FFFFFF\n}\n\n.ace-cobalt .ace_cursor {\n  color: #FFFFFF\n}\n\n.ace-cobalt .ace_marker-layer .ace_selection {\n  background: rgba(179, 101, 57, 0.75)\n}\n\n.ace-cobalt.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #002240;\n}\n\n.ace-cobalt .ace_marker-layer .ace_step {\n  background: rgb(127, 111, 19)\n}\n\n.ace-cobalt .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(255, 255, 255, 0.15)\n}\n\n.ace-cobalt .ace_marker-layer .ace_active-line {\n  background: rgba(0, 0, 0, 0.35)\n}\n\n.ace-cobalt .ace_gutter-active-line {\n  background-color: rgba(0, 0, 0, 0.35)\n}\n\n.ace-cobalt .ace_marker-layer .ace_selected-word {\n  border: 1px solid rgba(179, 101, 57, 0.75)\n}\n\n.ace-cobalt .ace_invisible {\n  color: rgba(255, 255, 255, 0.15)\n}\n\n.ace-cobalt .ace_keyword,\n.ace-cobalt .ace_meta {\n  color: #FF9D00\n}\n\n.ace-cobalt .ace_constant,\n.ace-cobalt .ace_constant.ace_character,\n.ace-cobalt .ace_constant.ace_character.ace_escape,\n.ace-cobalt .ace_constant.ace_other {\n  color: #FF628C\n}\n\n.ace-cobalt .ace_invalid {\n  color: #F8F8F8;\n  background-color: #800F00\n}\n\n.ace-cobalt .ace_support {\n  color: #80FFBB\n}\n\n.ace-cobalt .ace_support.ace_constant {\n  color: #EB939A\n}\n\n.ace-cobalt .ace_fold {\n  background-color: #FF9D00;\n  border-color: #FFFFFF\n}\n\n.ace-cobalt .ace_support.ace_function {\n  color: #FFB054\n}\n\n.ace-cobalt .ace_storage {\n  color: #FFEE80\n}\n\n.ace-cobalt .ace_entity {\n  color: #FFDD00\n}\n\n.ace-cobalt .ace_string {\n  color: #3AD900\n}\n\n.ace-cobalt .ace_string.ace_regexp {\n  color: #80FFC2\n}\n\n.ace-cobalt .ace_comment {\n  font-style: italic;\n  color: #0088FF\n}\n\n.ace-cobalt .ace_heading,\n.ace-cobalt .ace_markup.ace_heading {\n  color: #C8E4FD;\n  background-color: #001221\n}\n\n.ace-cobalt .ace_list,\n.ace-cobalt .ace_markup.ace_list {\n  background-color: #130D26\n}\n\n.ace-cobalt .ace_variable {\n  color: #CCCCCC\n}\n\n.ace-cobalt .ace_variable.ace_language {\n  color: #FF80E1\n}\n\n.ace-cobalt .ace_meta.ace_tag {\n  color: #9EFFFF\n}\n\n.ace-cobalt .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYHCLSvkPAAP3AgSDTRd4AAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-cobalt .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/cobalt", ["require", "exports", "module", "ace/theme/cobalt.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/cobalt", ["require", "exports", "module", "ace/theme/cobalt-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-cobalt";
-    exports.cssText = require("./cobalt.css");
+    exports.cssText = require("./cobalt-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/cobalt"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-crimson_editor.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-crimson_editor.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
-define("ace/theme/crimson_editor.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/crimson_editor-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-crimson-editor .ace_gutter {\n  background: #ebebeb;\n  color: #333;\n  overflow : hidden;\n}\n\n.ace-crimson-editor .ace_gutter-layer {\n  width: 100%;\n  text-align: right;\n}\n\n.ace-crimson-editor .ace_print-margin {\n  width: 1px;\n  background: #e8e8e8;\n}\n\n.ace-crimson-editor {\n  background-color: #FFFFFF;\n  color: rgb(64, 64, 64);\n}\n\n.ace-crimson-editor .ace_cursor {\n  color: black;\n}\n\n.ace-crimson-editor .ace_invisible {\n  color: rgb(191, 191, 191);\n}\n\n.ace-crimson-editor .ace_identifier {\n  color: black;\n}\n\n.ace-crimson-editor .ace_keyword {\n  color: blue;\n}\n\n.ace-crimson-editor .ace_constant.ace_buildin {\n  color: rgb(88, 72, 246);\n}\n\n.ace-crimson-editor .ace_constant.ace_language {\n  color: rgb(255, 156, 0);\n}\n\n.ace-crimson-editor .ace_constant.ace_library {\n  color: rgb(6, 150, 14);\n}\n\n.ace-crimson-editor .ace_invalid {\n  text-decoration: line-through;\n  color: rgb(224, 0, 0);\n}\n\n.ace-crimson-editor .ace_fold {\n}\n\n.ace-crimson-editor .ace_support.ace_function {\n  color: rgb(192, 0, 0);\n}\n\n.ace-crimson-editor .ace_support.ace_constant {\n  color: rgb(6, 150, 14);\n}\n\n.ace-crimson-editor .ace_support.ace_type,\n.ace-crimson-editor .ace_support.ace_class {\n  color: rgb(109, 121, 222);\n}\n\n.ace-crimson-editor .ace_keyword.ace_operator {\n  color: rgb(49, 132, 149);\n}\n\n.ace-crimson-editor .ace_string {\n  color: rgb(128, 0, 128);\n}\n\n.ace-crimson-editor .ace_comment {\n  color: rgb(76, 136, 107);\n}\n\n.ace-crimson-editor .ace_comment.ace_doc {\n  color: rgb(0, 102, 255);\n}\n\n.ace-crimson-editor .ace_comment.ace_doc.ace_tag {\n  color: rgb(128, 159, 191);\n}\n\n.ace-crimson-editor .ace_constant.ace_numeric {\n  color: rgb(0, 0, 64);\n}\n\n.ace-crimson-editor .ace_variable {\n  color: rgb(0, 64, 128);\n}\n\n.ace-crimson-editor .ace_xml-pe {\n  color: rgb(104, 104, 91);\n}\n\n.ace-crimson-editor .ace_marker-layer .ace_selection {\n  background: rgb(181, 213, 255);\n}\n\n.ace-crimson-editor .ace_marker-layer .ace_step {\n  background: rgb(252, 255, 0);\n}\n\n.ace-crimson-editor .ace_marker-layer .ace_stack {\n  background: rgb(164, 229, 101);\n}\n\n.ace-crimson-editor .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgb(192, 192, 192);\n}\n\n.ace-crimson-editor .ace_marker-layer .ace_active-line {\n  background: rgb(232, 242, 254);\n}\n\n.ace-crimson-editor .ace_gutter-active-line {\n    background-color : #dcdcdc;\n}\n\n.ace-crimson-editor .ace_meta.ace_tag {\n  color:rgb(28, 2, 255);\n}\n\n.ace-crimson-editor .ace_marker-layer .ace_selected-word {\n  background: rgb(250, 250, 255);\n  border: 1px solid rgb(200, 200, 250);\n}\n\n.ace-crimson-editor .ace_string.ace_regex {\n  color: rgb(192, 0, 192);\n}\n\n.ace-crimson-editor .ace_indent-guide {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bLly//BwAmVgd1/w11/gAAAABJRU5ErkJggg==\") right repeat-y;\n}\n\n.ace-crimson-editor .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n} \n";
 
 });
 
-define("ace/theme/crimson_editor", ["require", "exports", "module", "ace/theme/crimson_editor.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/crimson_editor", ["require", "exports", "module", "ace/theme/crimson_editor-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
-    exports.cssText = require("./crimson_editor.css");
+    exports.cssText = require("./crimson_editor-css");
     exports.cssClass = "ace-crimson-editor";
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/crimson_editor"], function(m) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-dawn.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-dawn.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/dawn.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/dawn-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-dawn .ace_gutter {\n  background: #ebebeb;\n  color: #333\n}\n\n.ace-dawn .ace_print-margin {\n  width: 1px;\n  background: #e8e8e8\n}\n\n.ace-dawn {\n  background-color: #F9F9F9;\n  color: #080808\n}\n\n.ace-dawn .ace_cursor {\n  color: #000000\n}\n\n.ace-dawn .ace_marker-layer .ace_selection {\n  background: rgba(39, 95, 255, 0.30)\n}\n\n.ace-dawn.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #F9F9F9;\n}\n\n.ace-dawn .ace_marker-layer .ace_step {\n  background: rgb(255, 255, 0)\n}\n\n.ace-dawn .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(75, 75, 126, 0.50)\n}\n\n.ace-dawn .ace_marker-layer .ace_active-line {\n  background: rgba(36, 99, 180, 0.12)\n}\n\n.ace-dawn .ace_gutter-active-line {\n  background-color : #dcdcdc\n}\n\n.ace-dawn .ace_marker-layer .ace_selected-word {\n  border: 1px solid rgba(39, 95, 255, 0.30)\n}\n\n.ace-dawn .ace_invisible {\n  color: rgba(75, 75, 126, 0.50)\n}\n\n.ace-dawn .ace_keyword,\n.ace-dawn .ace_meta {\n  color: #794938\n}\n\n.ace-dawn .ace_constant,\n.ace-dawn .ace_constant.ace_character,\n.ace-dawn .ace_constant.ace_character.ace_escape,\n.ace-dawn .ace_constant.ace_other {\n  color: #811F24\n}\n\n.ace-dawn .ace_invalid.ace_illegal {\n  text-decoration: underline;\n  font-style: italic;\n  color: #F8F8F8;\n  background-color: #B52A1D\n}\n\n.ace-dawn .ace_invalid.ace_deprecated {\n  text-decoration: underline;\n  font-style: italic;\n  color: #B52A1D\n}\n\n.ace-dawn .ace_support {\n  color: #691C97\n}\n\n.ace-dawn .ace_support.ace_constant {\n  color: #B4371F\n}\n\n.ace-dawn .ace_fold {\n  background-color: #794938;\n  border-color: #080808\n}\n\n.ace-dawn .ace_list,\n.ace-dawn .ace_markup.ace_list,\n.ace-dawn .ace_support.ace_function {\n  color: #693A17\n}\n\n.ace-dawn .ace_storage {\n  font-style: italic;\n  color: #A71D5D\n}\n\n.ace-dawn .ace_string {\n  color: #0B6125\n}\n\n.ace-dawn .ace_string.ace_regexp {\n  color: #CF5628\n}\n\n.ace-dawn .ace_comment {\n  font-style: italic;\n  color: #5A525F\n}\n\n.ace-dawn .ace_heading,\n.ace-dawn .ace_markup.ace_heading {\n  color: #19356D\n}\n\n.ace-dawn .ace_variable {\n  color: #234A97\n}\n\n.ace-dawn .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYLh/5+x/AAizA4hxNNsZAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-dawn .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n} \n";
 
 });
 
-define("ace/theme/dawn", ["require", "exports", "module", "ace/theme/dawn.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/dawn", ["require", "exports", "module", "ace/theme/dawn-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
     exports.cssClass = "ace-dawn";
-    exports.cssText = require("./dawn.css");
+    exports.cssText = require("./dawn-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/dawn"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-dracula.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-dracula.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/dracula.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/dracula-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = "/*\n * Copyright \u00A9 2017 Zeno Rocha <hi@zenorocha.com>\n *\n * Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the \u201CSoftware\u201D), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n *\n * The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n *\n * THE SOFTWARE IS PROVIDED \u201CAS IS\u201D, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n */\n\n.ace-dracula .ace_gutter {\n  background: #282a36;\n  color: rgb(144,145,148)\n}\n\n.ace-dracula .ace_print-margin {\n  width: 1px;\n  background: #44475a\n}\n\n.ace-dracula {\n  background-color: #282a36;\n  color: #f8f8f2\n}\n\n.ace-dracula .ace_cursor {\n  color: #f8f8f0\n}\n\n.ace-dracula .ace_marker-layer .ace_selection {\n  background: #44475a\n}\n\n.ace-dracula.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #282a36;\n  border-radius: 2px\n}\n\n.ace-dracula .ace_marker-layer .ace_step {\n  background: rgb(198, 219, 174)\n}\n\n.ace-dracula .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #a29709\n}\n\n.ace-dracula .ace_marker-layer .ace_active-line {\n  background: #44475a\n}\n\n.ace-dracula .ace_gutter-active-line {\n  background-color: #44475a\n}\n\n.ace-dracula .ace_marker-layer .ace_selected-word {\n  box-shadow: 0px 0px 0px 1px #a29709;\n  border-radius: 3px;\n}\n\n.ace-dracula .ace_fold {\n  background-color: #50fa7b;\n  border-color: #f8f8f2\n}\n\n.ace-dracula .ace_keyword {\n  color: #ff79c6\n}\n\n.ace-dracula .ace_constant.ace_language {\n  color: #bd93f9\n}\n\n.ace-dracula .ace_constant.ace_numeric {\n  color: #bd93f9\n}\n\n.ace-dracula .ace_constant.ace_character {\n  color: #bd93f9\n}\n\n.ace-dracula .ace_constant.ace_character.ace_escape {\n  color: #ff79c6\n}\n\n.ace-dracula .ace_constant.ace_other {\n  color: #bd93f9\n}\n\n.ace-dracula .ace_support.ace_function {\n  color: #8be9fd\n}\n\n.ace-dracula .ace_support.ace_constant {\n  color: #6be5fd\n}\n\n.ace-dracula .ace_support.ace_class {\n  font-style: italic;\n  color: #66d9ef\n}\n\n.ace-dracula .ace_support.ace_type {\n  font-style: italic;\n  color: #66d9ef\n}\n\n.ace-dracula .ace_storage {\n  color: #ff79c6\n}\n\n.ace-dracula .ace_storage.ace_type {\n  font-style: italic;\n  color: #8be9fd\n}\n\n.ace-dracula .ace_invalid {\n  color: #F8F8F0;\n  background-color: #ff79c6\n}\n\n.ace-dracula .ace_invalid.ace_deprecated {\n  color: #F8F8F0;\n  background-color: #bd93f9\n}\n\n.ace-dracula .ace_string {\n  color: #f1fa8c\n}\n\n.ace-dracula .ace_comment {\n  color: #6272a4\n}\n\n.ace-dracula .ace_variable {\n  color: #50fa7b\n}\n\n.ace-dracula .ace_variable.ace_parameter {\n  font-style: italic;\n  color: #ffb86c\n}\n\n.ace-dracula .ace_entity.ace_other.ace_attribute-name {\n  color: #50fa7b\n}\n\n.ace-dracula .ace_entity.ace_name.ace_function {\n  color: #50fa7b\n}\n\n.ace-dracula .ace_entity.ace_name.ace_tag {\n  color: #ff79c6\n}\n.ace-dracula .ace_invisible {\n  color: #626680;\n}\n\n.ace-dracula .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYHB3d/8PAAOIAdULw8qMAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-dracula .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACAQMAAACjTyRkAAAABlBMVEUAAADCwsK76u2xAAAAAXRSTlMAQObYZgAAAAxJREFUCNdjYGBoAAAAhACBGFbxzQAAAABJRU5ErkJggg==\") right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/dracula", ["require", "exports", "module", "ace/theme/dracula.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/dracula", ["require", "exports", "module", "ace/theme/dracula-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-dracula";
-    exports.cssText = require("./dracula.css");
+    exports.cssText = require("./dracula-css");
     exports.$selectionColorConflict = true;
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/dracula"], function(m) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-dreamweaver.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-dreamweaver.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/dreamweaver.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/dreamweaver-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-dreamweaver .ace_gutter {\n  background: #e8e8e8;\n  color: #333;\n}\n\n.ace-dreamweaver .ace_print-margin {\n  width: 1px;\n  background: #e8e8e8;\n}\n\n.ace-dreamweaver {\n  background-color: #FFFFFF;\n  color: black;\n}\n\n.ace-dreamweaver .ace_fold {\n    background-color: #757AD8;\n}\n\n.ace-dreamweaver .ace_cursor {\n  color: black;\n}\n        \n.ace-dreamweaver .ace_invisible {\n  color: rgb(191, 191, 191);\n}\n\n.ace-dreamweaver .ace_storage,\n.ace-dreamweaver .ace_keyword {\n  color: blue;\n}\n\n.ace-dreamweaver .ace_constant.ace_buildin {\n  color: rgb(88, 72, 246);\n}\n\n.ace-dreamweaver .ace_constant.ace_language {\n  color: rgb(88, 92, 246);\n}\n\n.ace-dreamweaver .ace_constant.ace_library {\n  color: rgb(6, 150, 14);\n}\n\n.ace-dreamweaver .ace_invalid {\n  background-color: rgb(153, 0, 0);\n  color: white;\n}\n\n.ace-dreamweaver .ace_support.ace_function {\n  color: rgb(60, 76, 114);\n}\n\n.ace-dreamweaver .ace_support.ace_constant {\n  color: rgb(6, 150, 14);\n}\n\n.ace-dreamweaver .ace_support.ace_type,\n.ace-dreamweaver .ace_support.ace_class {\n  color: #009;\n}\n\n.ace-dreamweaver .ace_support.ace_php_tag {\n  color: #f00;\n}\n\n.ace-dreamweaver .ace_keyword.ace_operator {\n  color: rgb(104, 118, 135);\n}\n\n.ace-dreamweaver .ace_string {\n  color: #00F;\n}\n\n.ace-dreamweaver .ace_comment {\n  color: rgb(76, 136, 107);\n}\n\n.ace-dreamweaver .ace_comment.ace_doc {\n  color: rgb(0, 102, 255);\n}\n\n.ace-dreamweaver .ace_comment.ace_doc.ace_tag {\n  color: rgb(128, 159, 191);\n}\n\n.ace-dreamweaver .ace_constant.ace_numeric {\n  color: rgb(0, 0, 205);\n}\n\n.ace-dreamweaver .ace_variable {\n  color: #06F\n}\n\n.ace-dreamweaver .ace_xml-pe {\n  color: rgb(104, 104, 91);\n}\n\n.ace-dreamweaver .ace_entity.ace_name.ace_function {\n  color: #00F;\n}\n\n\n.ace-dreamweaver .ace_heading {\n  color: rgb(12, 7, 255);\n}\n\n.ace-dreamweaver .ace_list {\n  color:rgb(185, 6, 144);\n}\n\n.ace-dreamweaver .ace_marker-layer .ace_selection {\n  background: rgb(181, 213, 255);\n}\n\n.ace-dreamweaver .ace_marker-layer .ace_step {\n  background: rgb(252, 255, 0);\n}\n\n.ace-dreamweaver .ace_marker-layer .ace_stack {\n  background: rgb(164, 229, 101);\n}\n\n.ace-dreamweaver .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgb(192, 192, 192);\n}\n\n.ace-dreamweaver .ace_marker-layer .ace_active-line {\n  background: rgba(0, 0, 0, 0.07);\n}\n\n.ace-dreamweaver .ace_gutter-active-line {\n  background-color : #DCDCDC;\n}\n\n.ace-dreamweaver .ace_marker-layer .ace_selected-word {\n  background: rgb(250, 250, 255);\n  border: 1px solid rgb(200, 200, 250);\n}\n\n.ace-dreamweaver .ace_meta.ace_tag {\n  color:#009;\n}\n\n.ace-dreamweaver .ace_meta.ace_tag.ace_anchor {\n  color:#060;\n}\n\n.ace-dreamweaver .ace_meta.ace_tag.ace_form {\n  color:#F90;\n}\n\n.ace-dreamweaver .ace_meta.ace_tag.ace_image {\n  color:#909;\n}\n\n.ace-dreamweaver .ace_meta.ace_tag.ace_script {\n  color:#900;\n}\n\n.ace-dreamweaver .ace_meta.ace_tag.ace_style {\n  color:#909;\n}\n\n.ace-dreamweaver .ace_meta.ace_tag.ace_table {\n  color:#099;\n}\n\n.ace-dreamweaver .ace_string.ace_regex {\n  color: rgb(255, 0, 0)\n}\n\n.ace-dreamweaver .ace_indent-guide {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bLly//BwAmVgd1/w11/gAAAABJRU5ErkJggg==\") right repeat-y;\n}\n\n.ace-dreamweaver .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n} \n";
 
 });
 
-define("ace/theme/dreamweaver", ["require", "exports", "module", "ace/theme/dreamweaver.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/dreamweaver", ["require", "exports", "module", "ace/theme/dreamweaver-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
     exports.cssClass = "ace-dreamweaver";
-    exports.cssText = require("./dreamweaver.css");
+    exports.cssText = require("./dreamweaver-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/dreamweaver"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-eclipse.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-eclipse.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/eclipse.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/eclipse-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-eclipse .ace_gutter {\n  background: #ebebeb;\n  border-right: 1px solid rgb(159, 159, 159);\n  color: rgb(136, 136, 136);\n}\n\n.ace-eclipse .ace_print-margin {\n  width: 1px;\n  background: #ebebeb;\n}\n\n.ace-eclipse {\n  background-color: #FFFFFF;\n  color: black;\n}\n\n.ace-eclipse .ace_fold {\n    background-color: rgb(60, 76, 114);\n}\n\n.ace-eclipse .ace_cursor {\n  color: black;\n}\n\n.ace-eclipse .ace_storage,\n.ace-eclipse .ace_keyword,\n.ace-eclipse .ace_variable {\n  color: rgb(127, 0, 85);\n}\n\n.ace-eclipse .ace_constant.ace_buildin {\n  color: rgb(88, 72, 246);\n}\n\n.ace-eclipse .ace_constant.ace_library {\n  color: rgb(6, 150, 14);\n}\n\n.ace-eclipse .ace_function {\n  color: rgb(60, 76, 114);\n}\n\n.ace-eclipse .ace_string {\n  color: rgb(42, 0, 255);\n}\n\n.ace-eclipse .ace_comment {\n  color: rgb(113, 150, 130);\n}\n\n.ace-eclipse .ace_comment.ace_doc {\n  color: rgb(63, 95, 191);\n}\n\n.ace-eclipse .ace_comment.ace_doc.ace_tag {\n  color: rgb(127, 159, 191);\n}\n\n.ace-eclipse .ace_constant.ace_numeric {\n  color: darkblue;\n}\n\n.ace-eclipse .ace_tag {\n  color: rgb(25, 118, 116);\n}\n\n.ace-eclipse .ace_type {\n  color: rgb(127, 0, 127);\n}\n\n.ace-eclipse .ace_xml-pe {\n  color: rgb(104, 104, 91);\n}\n\n.ace-eclipse .ace_marker-layer .ace_selection {\n  background: rgb(181, 213, 255);\n}\n\n.ace-eclipse .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgb(192, 192, 192);\n}\n\n.ace-eclipse .ace_meta.ace_tag {\n  color:rgb(25, 118, 116);\n}\n\n.ace-eclipse .ace_invisible {\n  color: #ddd;\n}\n\n.ace-eclipse .ace_entity.ace_other.ace_attribute-name {\n  color:rgb(127, 0, 127);\n}\n.ace-eclipse .ace_marker-layer .ace_step {\n  background: rgb(255, 255, 0);\n}\n\n.ace-eclipse .ace_active-line {\n  background: rgb(232, 242, 254);\n}\n\n.ace-eclipse .ace_gutter-active-line {\n  background-color : #DADADA;\n}\n\n.ace-eclipse .ace_marker-layer .ace_selected-word {\n  border: 1px solid rgb(181, 213, 255);\n}\n\n.ace-eclipse .ace_indent-guide {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bLly//BwAmVgd1/w11/gAAAABJRU5ErkJggg==\") right repeat-y;\n}\n\n.ace-eclipse .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n} \n";
 
 });
 
-define("ace/theme/eclipse", ["require", "exports", "module", "ace/theme/eclipse.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/eclipse", ["require", "exports", "module", "ace/theme/eclipse-css", "ace/lib/dom"], function(require, exports, module) {
     "use strict";
     exports.isDark = false;
-    exports.cssText = require("./eclipse.css");
+    exports.cssText = require("./eclipse-css");
     exports.cssClass = "ace-eclipse";
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/eclipse"], function(m) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-github.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-github.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/github.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/github-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = "/* CSS style content from github's default pygments highlighter template.\n   Cursor and selection styles from textmate.css. */\n.ace-github .ace_gutter {\n  background: #e8e8e8;\n  color: #AAA;\n}\n\n.ace-github  {\n  background: #fff;\n  color: #000;\n}\n\n.ace-github .ace_keyword {\n  font-weight: bold;\n}\n\n.ace-github .ace_string {\n  color: #D14;\n}\n\n.ace-github .ace_variable.ace_class {\n  color: teal;\n}\n\n.ace-github .ace_constant.ace_numeric {\n  color: #099;\n}\n\n.ace-github .ace_constant.ace_buildin {\n  color: #0086B3;\n}\n\n.ace-github .ace_support.ace_function {\n  color: #0086B3;\n}\n\n.ace-github .ace_comment {\n  color: #998;\n  font-style: italic;\n}\n\n.ace-github .ace_variable.ace_language  {\n  color: #0086B3;\n}\n\n.ace-github .ace_paren {\n  font-weight: bold;\n}\n\n.ace-github .ace_boolean {\n  font-weight: bold;\n}\n\n.ace-github .ace_string.ace_regexp {\n  color: #009926;\n  font-weight: normal;\n}\n\n.ace-github .ace_variable.ace_instance {\n  color: teal;\n}\n\n.ace-github .ace_constant.ace_language {\n  font-weight: bold;\n}\n\n.ace-github .ace_cursor {\n  color: black;\n}\n\n.ace-github.ace_focus .ace_marker-layer .ace_active-line {\n  background: rgb(255, 255, 204);\n}\n.ace-github .ace_marker-layer .ace_active-line {\n  background: rgb(245, 245, 245);\n}\n\n.ace-github .ace_marker-layer .ace_selection {\n  background: rgb(181, 213, 255);\n}\n\n.ace-github.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px white;\n}\n/* bold keywords cause cursor issues for some fonts */\n/* this disables bold style for editor and keeps for static highlighter */\n.ace-github.ace_nobold .ace_line > span {\n    font-weight: normal !important;\n}\n\n.ace-github .ace_marker-layer .ace_step {\n  background: rgb(252, 255, 0);\n}\n\n.ace-github .ace_marker-layer .ace_stack {\n  background: rgb(164, 229, 101);\n}\n\n.ace-github .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgb(192, 192, 192);\n}\n\n.ace-github .ace_gutter-active-line {\n    background-color : rgba(0, 0, 0, 0.07);\n}\n\n.ace-github .ace_marker-layer .ace_selected-word {\n  background: rgb(250, 250, 255);\n  border: 1px solid rgb(200, 200, 250);\n}\n\n.ace-github .ace_invisible {\n  color: #BFBFBF\n}\n\n.ace-github .ace_print-margin {\n  width: 1px;\n  background: #e8e8e8;\n}\n\n.ace-github .ace_indent-guide {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bLly//BwAmVgd1/w11/gAAAABJRU5ErkJggg==\") right repeat-y;\n}\n\n.ace-github .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/github", ["require", "exports", "module", "ace/theme/github.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/github", ["require", "exports", "module", "ace/theme/github-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
     exports.cssClass = "ace-github";
-    exports.cssText = require("./github.css");
+    exports.cssText = require("./github-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/github"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-github_dark.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-github_dark.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/github_dark.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/github_dark-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-github-dark .ace_gutter {\n  background: #24292e;\n  color: #7388b5\n}\n\n.ace-github-dark .ace_print-margin {\n  width: 1px;\n  background: #00204b\n}\n\n.ace-github-dark {\n  background-color: #24292e;\n  color: #FFFFFF\n}\n\n.ace-github-dark .ace_constant.ace_other,\n.ace-github-dark .ace_cursor {\n  color: #FFFFFF\n}\n\n.ace-github-dark .ace_marker-layer .ace_selection {\n  background: #003F8E\n}\n\n.ace-github-dark.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #24292e;\n}\n\n.ace-github-dark .ace_marker-layer .ace_step {\n  background: rgb(127, 111, 19)\n}\n\n.ace-github-dark .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #404F7D\n}\n\n.ace-github-dark .ace_marker-layer .ace_active-line {\n  background: #00346E\n}\n\n.ace-github-dark .ace_gutter-active-line {\n  background-color: #24292e\n}\n\n.ace-github-dark .ace_marker-layer .ace_selected-word {\n  border: 1px solid #003F8E\n}\n\n.ace-github-dark .ace_invisible {\n  color: #404F7D\n}\n\n.ace-github-dark .ace_keyword,\n.ace-github-dark .ace_meta,\n.ace-github-dark .ace_storage,\n.ace-github-dark .ace_storage.ace_type,\n.ace-github-dark .ace_support.ace_type {\n  color: #ff7b72\n}\n\n.ace-github-dark .ace_keyword.ace_operator {\n  color: #79c0ff\n}\n\n.ace-github-dark .ace_constant.ace_character,\n.ace-github-dark .ace_constant.ace_language,\n.ace-github-dark .ace_constant.ace_numeric,\n.ace-github-dark .ace_keyword.ace_other.ace_unit,\n.ace-github-dark .ace_support.ace_constant,\n.ace-github-dark .ace_variable.ace_parameter {\n  color: #FFC58F\n}\n\n.ace-github-dark .ace_invalid {\n  color: #FFFFFF;\n  background-color: #F99DA5\n}\n\n.ace-github-dark .ace_invalid.ace_deprecated {\n  color: #FFFFFF;\n  background-color: #ff7b72\n}\n\n.ace-github-dark .ace_fold {\n  background-color: #BBDAFF;\n  border-color: #FFFFFF\n}\n\n.ace-github-dark .ace_entity.ace_name.ace_function,\n.ace-github-dark .ace_support.ace_function,\n.ace-github-dark .ace_variable {\n  color: #BBDAFF\n}\n\n.ace-github-dark .ace_support.ace_class,\n.ace-github-dark .ace_support.ace_type {\n  color: #FFEEAD\n}\n\n.ace-github-dark .ace_heading,\n.ace-github-dark .ace_markup.ace_heading,\n.ace-github-dark .ace_string {\n  color: #9fcef6\n}\n\n.ace-github-dark .ace_entity.ace_name.ace_tag,\n.ace-github-dark .ace_entity.ace_other.ace_attribute-name,\n.ace-github-dark .ace_meta.ace_tag,\n.ace-github-dark .ace_string.ace_regexp,\n.ace-github-dark .ace_variable {\n  color: #FF9DA4\n}\n\n.ace-github-dark .ace_comment {\n  color: #7285B7\n}\n\n.ace-github-dark .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYJDzqfwPAANXAeNsiA+ZAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-github-dark .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n\n.ace-github-dark .ace_constant.ace_buildin {\n  color: #0086B3;\n}\n\n.ace-github-dark .ace_variable.ace_language {\n  color: #ffffff;\n}\n  ";
 
 });
 
-define("ace/theme/github_dark", ["require", "exports", "module", "ace/theme/github_dark.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/github_dark", ["require", "exports", "module", "ace/theme/github_dark-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-github-dark";
-    exports.cssText = require("./github_dark.css");
+    exports.cssText = require("./github_dark-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/github_dark"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-gob.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-gob.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/gob.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/gob-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-gob .ace_gutter {\n  background: #0B1818;\n  color: #03EE03\n}\n\n.ace-gob .ace_print-margin {\n  width: 1px;\n  background: #131313\n}\n\n.ace-gob {\n  background-color: #0B0B0B;\n  color: #00FF00\n}\n\n.ace-gob .ace_cursor {\n  border-color: rgba(16, 248, 255, 0.90);\n  background-color: rgba(16, 240, 248, 0.70);\n  opacity: 0.4;\n}\n\n.ace-gob .ace_marker-layer .ace_selection {\n  background: rgba(221, 240, 255, 0.20)\n}\n\n.ace-gob.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #141414;\n}\n\n.ace-gob .ace_marker-layer .ace_step {\n  background: rgb(16, 128, 0)\n}\n\n.ace-gob .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(64, 255, 255, 0.25)\n}\n\n.ace-gob .ace_marker-layer .ace_active-line {\n  background: rgba(255, 255, 255, 0.04)\n}\n\n.ace-gob .ace_gutter-active-line {\n  background-color: rgba(255, 255, 255, 0.04)\n}\n\n.ace-gob .ace_marker-layer .ace_selected-word {\n  border: 1px solid rgba(192, 240, 255, 0.20)\n}\n\n.ace-gob .ace_invisible {\n  color: rgba(255, 255, 255, 0.25)\n}\n\n.ace-gob .ace_keyword,\n.ace-gob .ace_meta {\n  color: #10D8E8\n}\n\n.ace-gob .ace_constant,\n.ace-gob .ace_constant.ace_character,\n.ace-gob .ace_constant.ace_character.ace_escape,\n.ace-gob .ace_constant.ace_other,\n.ace-gob .ace_heading,\n.ace-gob .ace_markup.ace_heading,\n.ace-gob .ace_support.ace_constant {\n  color: #10F0A0\n}\n\n.ace-gob .ace_invalid.ace_illegal {\n  color: #F8F8F8;\n  background-color: rgba(86, 45, 86, 0.75)\n}\n\n.ace-gob .ace_invalid.ace_deprecated {\n  text-decoration: underline;\n  font-style: italic;\n  color: #20F8C0\n}\n\n.ace-gob .ace_support {\n  color: #20E8B0\n}\n\n.ace-gob .ace_fold {\n  background-color: #50B8B8;\n  border-color: #70F8F8\n}\n\n.ace-gob .ace_support.ace_function {\n  color: #00F800\n}\n\n.ace-gob .ace_list,\n.ace-gob .ace_markup.ace_list,\n.ace-gob .ace_storage {\n  color: #10FF98\n}\n\n.ace-gob .ace_entity.ace_name.ace_function,\n.ace-gob .ace_meta.ace_tag,\n.ace-gob .ace_variable {\n  color: #00F868\n}\n\n.ace-gob .ace_string {\n  color: #10F060\n}\n\n.ace-gob .ace_string.ace_regexp {\n  color: #20F090;\n}\n\n.ace-gob .ace_comment {\n  font-style: italic;\n  color: #00E060;\n}\n\n.ace-gob .ace_variable {\n  color: #00F888;\n}\n\n.ace-gob .ace_xml-pe {\n  color: #488858;\n}\n\n.ace-gob .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWMQERFpYLC1tf0PAAgOAnPnhxyiAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-gob .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/gob", ["require", "exports", "module", "ace/theme/gob.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/gob", ["require", "exports", "module", "ace/theme/gob-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-gob";
-    exports.cssText = require("./gob.css");
+    exports.cssText = require("./gob-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/gob"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-gruvbox.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-gruvbox.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/gruvbox.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/gruvbox-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-gruvbox .ace_gutter-active-line {\n  background-color: #3C3836;\n}\n\n.ace-gruvbox {\n  color: #EBDAB4;\n  background-color: #1D2021;\n}\n\n.ace-gruvbox .ace_invisible {\n  color: #504945;\n}\n\n.ace-gruvbox .ace_marker-layer .ace_selection {\n  background: rgba(179, 101, 57, 0.75)\n}\n\n.ace-gruvbox.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #002240;\n}\n\n.ace-gruvbox .ace_keyword {\n  color: #8ec07c;\n}\n\n.ace-gruvbox .ace_comment {\n  font-style: italic;\n  color: #928375;\n}\n\n.ace-gruvbox .ace-statement {\n  color: red;\n}\n\n.ace-gruvbox .ace_variable {\n  color: #84A598;\n}\n\n.ace-gruvbox .ace_variable.ace_language {\n  color: #D2879B;\n}\n\n.ace-gruvbox .ace_constant {\n  color: #C2859A;\n}\n\n.ace-gruvbox .ace_constant.ace_language {\n  color: #C2859A;\n}\n\n.ace-gruvbox .ace_constant.ace_numeric {\n  color: #C2859A;\n}\n\n.ace-gruvbox .ace_string {\n  color: #B8BA37;\n}\n\n.ace-gruvbox .ace_support {\n  color: #F9BC41;\n}\n\n.ace-gruvbox .ace_support.ace_function {\n  color: #F84B3C;\n}\n\n.ace-gruvbox .ace_storage {\n  color: #8FBF7F;\n}\n\n.ace-gruvbox .ace_keyword.ace_operator {\n  color: #EBDAB4;\n}\n\n.ace-gruvbox .ace_punctuation.ace_operator {\n  color: yellow;\n}\n\n.ace-gruvbox .ace_marker-layer .ace_active-line {\n  background: #3C3836;\n}\n\n.ace-gruvbox .ace_marker-layer .ace_selected-word {\n  border-radius: 4px;\n  border: 8px solid #3f475d;\n}\n\n.ace-gruvbox .ace_print-margin {\n  width: 5px;\n  background: #3C3836;\n}\n\n.ace-gruvbox .ace_indent-guide {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNQUFD4z6Crq/sfAAuYAuYl+7lfAAAAAElFTkSuQmCC\") right repeat-y;\n}\n\n.ace-gruvbox .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/gruvbox", ["require", "exports", "module", "ace/theme/gruvbox.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/gruvbox", ["require", "exports", "module", "ace/theme/gruvbox-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-gruvbox";
-    exports.cssText = require("./gruvbox.css");
+    exports.cssText = require("./gruvbox-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/gruvbox"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-gruvbox_dark_hard.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-gruvbox_dark_hard.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/gruvbox_dark_hard.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/gruvbox_dark_hard-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-gruvbox-dark-hard .ace_gutter {\n  background: #1d2021;\n  color: rgb(132,126,106)\n}\n\n.ace-gruvbox-dark-hard .ace_print-margin {\n  width: 1px;\n  background: #e8e8e8\n}\n\n.ace-gruvbox-dark-hard {\n  background-color: #1d2021;\n  color: rgba(235, 219, 178, 0.50)\n}\n\n.ace-gruvbox-dark-hard .ace_cursor {\n  color: #a89984\n}\n\n.ace-gruvbox-dark-hard .ace_marker-layer .ace_selection {\n  background: #3c3836\n}\n\n.ace-gruvbox-dark-hard.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #1d2021;\n  border-radius: 2px\n}\n\n.ace-gruvbox-dark-hard .ace_marker-layer .ace_step {\n  background: rgb(198, 219, 174)\n}\n\n.ace-gruvbox-dark-hard .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(235, 219, 178, 0.15)\n}\n\n.ace-gruvbox-dark-hard .ace_marker-layer .ace_active-line {\n  background: #3c3836\n}\n\n.ace-gruvbox-dark-hard .ace_gutter-active-line {\n  background-color: #3c3836\n}\n\n.ace-gruvbox-dark-hard .ace_marker-layer .ace_selected-word {\n  border: 1px solid #3c3836\n}\n\n.ace-gruvbox-dark-hard .ace_fold {\n  background-color: #b8bb26;\n  border-color: rgba(235, 219, 178, 0.50)\n}\n\n.ace-gruvbox-dark-hard .ace_keyword {\n  color: #fb4934\n}\n\n.ace-gruvbox-dark-hard .ace_keyword.ace_operator {\n  color: #8ec07c\n}\n\n.ace-gruvbox-dark-hard .ace_keyword.ace_other.ace_unit {\n  color: #b16286\n}\n\n.ace-gruvbox-dark-hard .ace_constant {\n  color: #d3869b\n}\n\n.ace-gruvbox-dark-hard .ace_constant.ace_numeric {\n  color: #d3869b\n}\n\n.ace-gruvbox-dark-hard .ace_constant.ace_character.ace_escape {\n  color: #fb4934\n}\n\n.ace-gruvbox-dark-hard .ace_constant.ace_other {\n  color: #d3869b\n}\n\n.ace-gruvbox-dark-hard .ace_support.ace_function {\n  color: #8ec07c\n}\n\n.ace-gruvbox-dark-hard .ace_support.ace_constant {\n  color: #d3869b\n}\n\n.ace-gruvbox-dark-hard .ace_support.ace_constant.ace_property-value {\n  color: #f9f5d7\n}\n\n.ace-gruvbox-dark-hard .ace_support.ace_class {\n  color: #fabd2f\n}\n\n.ace-gruvbox-dark-hard .ace_support.ace_type {\n  color: #fabd2f\n}\n\n.ace-gruvbox-dark-hard .ace_storage {\n  color: #fb4934\n}\n\n.ace-gruvbox-dark-hard .ace_invalid {\n  color: #f9f5d7;\n  background-color: #fb4934\n}\n\n.ace-gruvbox-dark-hard .ace_string {\n  color: #b8bb26\n}\n\n.ace-gruvbox-dark-hard .ace_string.ace_regexp {\n  color: #b8bb26\n}\n\n.ace-gruvbox-dark-hard .ace_comment {\n  font-style: italic;\n  color: #928374\n}\n\n.ace-gruvbox-dark-hard .ace_variable {\n  color: #83a598\n}\n\n.ace-gruvbox-dark-hard .ace_variable.ace_language {\n  color: #d3869b\n}\n\n.ace-gruvbox-dark-hard .ace_variable.ace_parameter {\n  color: #f9f5d7\n}\n\n.ace-gruvbox-dark-hard .ace_meta.ace_tag {\n  color: #f9f5d7\n}\n\n.ace-gruvbox-dark-hard .ace_entity.ace_other.ace_attribute-name {\n  color: #fabd2f\n}\n\n.ace-gruvbox-dark-hard .ace_entity.ace_name.ace_function {\n  color: #b8bb26\n}\n\n.ace-gruvbox-dark-hard .ace_entity.ace_name.ace_tag {\n  color: #83a598\n}\n\n.ace-gruvbox-dark-hard .ace_markup.ace_heading {\n  color: #b8bb26\n}\n\n.ace-gruvbox-dark-hard .ace_markup.ace_list {\n  color: #83a598\n}\n\n.ace-gruvbox-dark-hard .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/gruvbox_dark_hard", ["require", "exports", "module", "ace/theme/gruvbox_dark_hard.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/gruvbox_dark_hard", ["require", "exports", "module", "ace/theme/gruvbox_dark_hard-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-gruvbox-dark-hard";
-    exports.cssText = require("./gruvbox_dark_hard.css");
+    exports.cssText = require("./gruvbox_dark_hard-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass);
 
 });
 (function() {
     window.require(["ace/theme/gruvbox_dark_hard"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-gruvbox_light_hard.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-gruvbox_light_hard.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/gruvbox_light_hard.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/gruvbox_light_hard-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-gruvbox-light-hard .ace_gutter {\n  background: #f9f5d7;\n  color: rgb(155,151,135)\n}\n\n.ace-gruvbox-light-hard .ace_print-margin {\n  width: 1px;\n  background: #e8e8e8\n}\n\n.ace-gruvbox-light-hard {\n  background-color: #f9f5d7;\n  color: rgba(60, 56, 54, 0.50)\n}\n\n.ace-gruvbox-light-hard .ace_cursor {\n  color: #7c6f64\n}\n\n.ace-gruvbox-light-hard .ace_marker-layer .ace_selection {\n  background: #ebdbb2\n}\n\n.ace-gruvbox-light-hard.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #f9f5d7;\n  border-radius: 2px\n}\n\n.ace-gruvbox-light-hard .ace_marker-layer .ace_step {\n  background: rgb(198, 219, 174)\n}\n\n.ace-gruvbox-light-hard .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(60, 56, 54, 0.15)\n}\n\n.ace-gruvbox-light-hard .ace_marker-layer .ace_active-line {\n  background: #ebdbb2\n}\n\n.ace-gruvbox-light-hard .ace_gutter-active-line {\n  background-color: #ebdbb2\n}\n\n.ace-gruvbox-light-hard .ace_marker-layer .ace_selected-word {\n  border: 1px solid #ebdbb2\n}\n\n.ace-gruvbox-light-hard .ace_fold {\n  background-color: #79740e;\n  border-color: rgba(60, 56, 54, 0.50)\n}\n\n.ace-gruvbox-light-hard .ace_keyword {\n  color: #9d0006\n}\n\n.ace-gruvbox-light-hard .ace_keyword.ace_operator {\n  color: #427b58\n}\n\n.ace-gruvbox-light-hard .ace_keyword.ace_other.ace_unit {\n  color: #b16286\n}\n\n.ace-gruvbox-light-hard .ace_constant {\n  color: #8f3f71\n}\n\n.ace-gruvbox-light-hard .ace_constant.ace_numeric {\n  color: #8f3f71\n}\n\n.ace-gruvbox-light-hard .ace_constant.ace_character.ace_escape {\n  color: #9d0006\n}\n\n.ace-gruvbox-light-hard .ace_constant.ace_other {\n  color: #8f3f71\n}\n\n.ace-gruvbox-light-hard .ace_support.ace_function {\n  color: #427b58\n}\n\n.ace-gruvbox-light-hard .ace_support.ace_constant {\n  color: #8f3f71\n}\n\n.ace-gruvbox-light-hard .ace_support.ace_constant.ace_property-value {\n  color: #1d2021\n}\n\n.ace-gruvbox-light-hard .ace_support.ace_class {\n  color: #b57614\n}\n\n.ace-gruvbox-light-hard .ace_support.ace_type {\n  color: #b57614\n}\n\n.ace-gruvbox-light-hard .ace_storage {\n  color: #9d0006\n}\n\n.ace-gruvbox-light-hard .ace_invalid {\n  color: #1d2021;\n  background-color: #9d0006\n}\n\n.ace-gruvbox-light-hard .ace_string {\n  color: #79740e\n}\n\n.ace-gruvbox-light-hard .ace_string.ace_regexp {\n  color: #79740e\n}\n\n.ace-gruvbox-light-hard .ace_comment {\n  font-style: italic;\n  color: #928374\n}\n\n.ace-gruvbox-light-hard .ace_variable {\n  color: #076678\n}\n\n.ace-gruvbox-light-hard .ace_variable.ace_language {\n  color: #8f3f71\n}\n\n.ace-gruvbox-light-hard .ace_variable.ace_parameter {\n  color: #1d2021\n}\n\n.ace-gruvbox-light-hard .ace_meta.ace_tag {\n  color: #1d2021\n}\n\n.ace-gruvbox-light-hard .ace_entity.ace_other.ace_attribute-name {\n  color: #b57614\n}\n\n.ace-gruvbox-light-hard .ace_entity.ace_name.ace_function {\n  color: #79740e\n}\n\n.ace-gruvbox-light-hard .ace_entity.ace_name.ace_tag {\n  color: #076678\n}\n\n.ace-gruvbox-light-hard .ace_markup.ace_heading {\n  color: #79740e\n}\n\n.ace-gruvbox-light-hard .ace_markup.ace_list {\n  color: #076678\n}\n\n.ace-gruvbox-light-hard .ace_indent-guide {\n    background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bLly//BwAmVgd1/w11/gAAAABJRU5ErkJggg==\") right repeat-y;\n}\n\n.ace-gruvbox-light-hard .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n} \n";
 
 });
 
-define("ace/theme/gruvbox_light_hard", ["require", "exports", "module", "ace/theme/gruvbox_light_hard.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/gruvbox_light_hard", ["require", "exports", "module", "ace/theme/gruvbox_light_hard-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
     exports.cssClass = "ace-gruvbox-light-hard";
-    exports.cssText = require("./gruvbox_light_hard.css");
+    exports.cssText = require("./gruvbox_light_hard-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass);
 
 });
 (function() {
     window.require(["ace/theme/gruvbox_light_hard"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-idle_fingers.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-idle_fingers.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/idle_fingers.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/idle_fingers-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-idle-fingers .ace_gutter {\n  background: #3b3b3b;\n  color: rgb(153,153,153)\n}\n\n.ace-idle-fingers .ace_print-margin {\n  width: 1px;\n  background: #3b3b3b\n}\n\n.ace-idle-fingers {\n  background-color: #323232;\n  color: #FFFFFF\n}\n\n.ace-idle-fingers .ace_cursor {\n  color: #91FF00\n}\n\n.ace-idle-fingers .ace_marker-layer .ace_selection {\n  background: rgba(90, 100, 126, 0.88)\n}\n\n.ace-idle-fingers.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #323232;\n}\n\n.ace-idle-fingers .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-idle-fingers .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #404040\n}\n\n.ace-idle-fingers .ace_marker-layer .ace_active-line {\n  background: #353637\n}\n\n.ace-idle-fingers .ace_gutter-active-line {\n  background-color: #353637\n}\n\n.ace-idle-fingers .ace_marker-layer .ace_selected-word {\n  border: 1px solid rgba(90, 100, 126, 0.88)\n}\n\n.ace-idle-fingers .ace_invisible {\n  color: #404040\n}\n\n.ace-idle-fingers .ace_keyword,\n.ace-idle-fingers .ace_meta {\n  color: #CC7833\n}\n\n.ace-idle-fingers .ace_constant,\n.ace-idle-fingers .ace_constant.ace_character,\n.ace-idle-fingers .ace_constant.ace_character.ace_escape,\n.ace-idle-fingers .ace_constant.ace_other,\n.ace-idle-fingers .ace_support.ace_constant {\n  color: #6C99BB\n}\n\n.ace-idle-fingers .ace_invalid {\n  color: #FFFFFF;\n  background-color: #FF0000\n}\n\n.ace-idle-fingers .ace_fold {\n  background-color: #CC7833;\n  border-color: #FFFFFF\n}\n\n.ace-idle-fingers .ace_support.ace_function {\n  color: #B83426\n}\n\n.ace-idle-fingers .ace_variable.ace_parameter {\n  font-style: italic\n}\n\n.ace-idle-fingers .ace_string {\n  color: #A5C261\n}\n\n.ace-idle-fingers .ace_string.ace_regexp {\n  color: #CCCC33\n}\n\n.ace-idle-fingers .ace_comment {\n  font-style: italic;\n  color: #BC9458\n}\n\n.ace-idle-fingers .ace_meta.ace_tag {\n  color: #FFE5BB\n}\n\n.ace-idle-fingers .ace_entity.ace_name {\n  color: #FFC66D\n}\n\n.ace-idle-fingers .ace_collab.ace_user1 {\n  color: #323232;\n  background-color: #FFF980\n}\n\n.ace-idle-fingers .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWMwMjLyZYiPj/8PAAreAwAI1+g0AAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-idle-fingers .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/idle_fingers", ["require", "exports", "module", "ace/theme/idle_fingers.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/idle_fingers", ["require", "exports", "module", "ace/theme/idle_fingers-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-idle-fingers";
-    exports.cssText = require("./idle_fingers.css");
+    exports.cssText = require("./idle_fingers-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/idle_fingers"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-iplastic.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-iplastic.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/iplastic.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/iplastic-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-iplastic .ace_gutter {\n  background: #dddddd;\n  color: #666666\n}\n\n.ace-iplastic .ace_print-margin {\n  width: 1px;\n  background: #bbbbbb\n}\n\n.ace-iplastic {\n  background-color: #eeeeee;\n  color: #333333\n}\n\n.ace-iplastic .ace_cursor {\n  color: #333\n}\n\n.ace-iplastic .ace_marker-layer .ace_selection {\n  background: #BAD6FD;\n}\n\n.ace-iplastic.ace_multiselect .ace_selection.ace_start {\n  border-radius: 4px\n}\n\n.ace-iplastic .ace_marker-layer .ace_step {\n  background: #444444\n}\n\n.ace-iplastic .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #49483E;\n  background: #FFF799\n}\n\n.ace-iplastic .ace_marker-layer .ace_active-line {\n  background: #e5e5e5\n}\n\n.ace-iplastic .ace_gutter-active-line {\n  background-color: #eeeeee\n}\n\n.ace-iplastic .ace_marker-layer .ace_selected-word {\n  border: 1px solid #555555;\n  border-radius:4px\n}\n\n.ace-iplastic .ace_invisible {\n  color: #999999\n}\n\n.ace-iplastic .ace_entity.ace_name.ace_tag,\n.ace-iplastic .ace_keyword,\n.ace-iplastic .ace_meta.ace_tag,\n.ace-iplastic .ace_storage {\n  color: #0000FF\n}\n\n.ace-iplastic .ace_punctuation,\n.ace-iplastic .ace_punctuation.ace_tag {\n  color: #000\n}\n\n.ace-iplastic .ace_constant {\n  color: #333333;\n  font-weight: 700\n}\n\n.ace-iplastic .ace_constant.ace_character,\n.ace-iplastic .ace_constant.ace_language,\n.ace-iplastic .ace_constant.ace_numeric,\n.ace-iplastic .ace_constant.ace_other {\n  color: #0066FF;\n  font-weight: 700\n}\n\n.ace-iplastic .ace_constant.ace_numeric{\n  font-weight: 100\n}\n\n.ace-iplastic .ace_invalid {\n  color: #F8F8F0;\n  background-color: #F92672\n}\n\n.ace-iplastic .ace_invalid.ace_deprecated {\n  color: #F8F8F0;\n  background-color: #AE81FF\n}\n\n.ace-iplastic .ace_support.ace_constant,\n.ace-iplastic .ace_support.ace_function {\n  color: #333333;\n  font-weight: 700\n}\n\n.ace-iplastic .ace_fold {\n  background-color: #464646;\n  border-color: #F8F8F2\n}\n\n.ace-iplastic .ace_storage.ace_type,\n.ace-iplastic .ace_support.ace_class,\n.ace-iplastic .ace_support.ace_type {\n  color: #3333fc;\n  font-weight: 700\n}\n\n.ace-iplastic .ace_entity.ace_name.ace_function,\n.ace-iplastic .ace_entity.ace_other,\n.ace-iplastic .ace_entity.ace_other.ace_attribute-name,\n.ace-iplastic .ace_variable {\n  color: #3366cc;\n  font-style: italic\n}\n\n.ace-iplastic .ace_variable.ace_parameter {\n  font-style: italic;\n  color: #2469E0\n}\n\n.ace-iplastic .ace_string {\n  color: #a55f03\n}\n\n.ace-iplastic .ace_comment {\n  color: #777777;\n  font-style: italic\n}\n\n.ace-iplastic .ace_fold-widget {\n  background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAUAAAAFCAYAAACNbyblAAAANElEQVR42mWKsQ0AMAzC8ixLlrzQjzmBiEjp0A6WwBCSPgKAXoLkqSot7nN3yMwR7pZ32NzpKkVoDBUxKAAAAABJRU5ErkJggg==);\n}\n\n.ace-iplastic .ace_indent-guide {\n  background: url(data:image/png;base64,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) right repeat-y\n}\n\n.ace-iplastic .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/iplastic", ["require", "exports", "module", "ace/theme/iplastic.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/iplastic", ["require", "exports", "module", "ace/theme/iplastic-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
     exports.cssClass = "ace-iplastic";
-    exports.cssText = require("./iplastic.css");
+    exports.cssText = require("./iplastic-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/iplastic"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-katzenmilch.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-katzenmilch.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/katzenmilch.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/katzenmilch-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-katzenmilch .ace_gutter,\n/* THIS THEME WAS AUTOGENERATED BY Theme.tmpl.css (UUID: ) */\n\n.ace-katzenmilch .ace_gutter {\n  background: #e8e8e8;\n  color: #333\n}\n\n.ace-katzenmilch .ace_print-margin {\n  width: 1px;\n  background: #e8e8e8\n}\n\n.ace-katzenmilch {\n  background-color: #f3f2f3;\n  color: rgba(15, 0, 9, 1.0)\n}\n\n.ace-katzenmilch .ace_cursor {\n  border-left: 2px solid #100011\n}\n\n.ace-katzenmilch .ace_overwrite-cursors .ace_cursor {\n  border-left: 0px;\n  border-bottom: 1px solid #100011\n}\n\n.ace-katzenmilch .ace_marker-layer .ace_selection {\n  background: rgba(100, 5, 208, 0.27)\n}\n\n.ace-katzenmilch.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #f3f2f3;\n}\n\n.ace-katzenmilch .ace_marker-layer .ace_step {\n  background: rgb(198, 219, 174)\n}\n\n.ace-katzenmilch .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(0, 0, 0, 0.33);\n}\n\n.ace-katzenmilch .ace_marker-layer .ace_active-line {\n  background: rgb(232, 242, 254)\n}\n\n.ace-katzenmilch .ace_gutter-active-line {\n  background-color: rgb(232, 242, 254)\n}\n\n.ace-katzenmilch .ace_marker-layer .ace_selected-word {\n  border: 1px solid rgba(100, 5, 208, 0.27)\n}\n\n.ace-katzenmilch .ace_invisible {\n  color: #BFBFBF\n}\n\n.ace-katzenmilch .ace_fold {\n  background-color: rgba(2, 95, 73, 0.97);\n  border-color: rgba(15, 0, 9, 1.0)\n}\n\n.ace-katzenmilch .ace_keyword {\n  color: #674Aa8;\n  rbackground-color: rgba(163, 170, 216, 0.055)\n}\n\n.ace-katzenmilch .ace_constant.ace_language {\n  color: #7D7e52;\n  rbackground-color: rgba(189, 190, 130, 0.059)\n}\n\n.ace-katzenmilch .ace_constant.ace_numeric {\n  color: rgba(79, 130, 123, 0.93);\n  rbackground-color: rgba(119, 194, 187, 0.059)\n}\n\n.ace-katzenmilch .ace_constant.ace_character,\n.ace-katzenmilch .ace_constant.ace_other {\n  color: rgba(2, 95, 105, 1.0);\n  rbackground-color: rgba(127, 34, 153, 0.063)\n}\n\n.ace-katzenmilch .ace_support.ace_function {\n  color: #9D7e62;\n  rbackground-color: rgba(189, 190, 130, 0.039)\n}\n\n.ace-katzenmilch .ace_support.ace_class {\n  color: rgba(239, 106, 167, 1.0);\n  rbackground-color: rgba(239, 106, 167, 0.063)\n}\n\n.ace-katzenmilch .ace_storage {\n  color: rgba(123, 92, 191, 1.0);\n  rbackground-color: rgba(139, 93, 223, 0.051)\n}\n\n.ace-katzenmilch .ace_invalid {\n  color: #DFDFD5;\n  rbackground-color: #CC1B27\n}\n\n.ace-katzenmilch .ace_string {\n  color: #5a5f9b;\n  rbackground-color: rgba(170, 175, 219, 0.035)\n}\n\n.ace-katzenmilch .ace_comment {\n  font-style: italic;\n  color: rgba(64, 79, 80, 0.67);\n  rbackground-color: rgba(95, 15, 255, 0.0078)\n}\n\n.ace-katzenmilch .ace_entity.ace_name.ace_function,\n.ace-katzenmilch .ace_variable {\n  color: rgba(2, 95, 73, 0.97);\n  rbackground-color: rgba(34, 255, 73, 0.12)\n}\n\n.ace-katzenmilch .ace_variable.ace_language {\n  color: #316fcf;\n  rbackground-color: rgba(58, 175, 255, 0.039)\n}\n\n.ace-katzenmilch .ace_variable.ace_parameter {\n  font-style: italic;\n  color: rgba(51, 150, 159, 0.87);\n  rbackground-color: rgba(5, 214, 249, 0.043)\n}\n\n.ace-katzenmilch .ace_entity.ace_other.ace_attribute-name {\n  color: rgba(73, 70, 194, 0.93);\n  rbackground-color: rgba(73, 134, 194, 0.035)\n}\n\n.ace-katzenmilch .ace_entity.ace_name.ace_tag {\n  color: #3976a2;\n  rbackground-color: rgba(73, 166, 210, 0.039)\n}\n\n.ace-katzenmilch .ace_indent-guide {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bLly//BwAmVgd1/w11/gAAAABJRU5ErkJggg==\") right repeat-y;\n}\n\n.ace-katzenmilch .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/katzenmilch", ["require", "exports", "module", "ace/theme/katzenmilch.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/katzenmilch", ["require", "exports", "module", "ace/theme/katzenmilch-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
     exports.cssClass = "ace-katzenmilch";
-    exports.cssText = require("./katzenmilch.css");
+    exports.cssText = require("./katzenmilch-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/katzenmilch"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-kr_theme.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-kr_theme.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/kr_theme.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/kr_theme-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-kr-theme .ace_gutter {\n  background: #1c1917;\n  color: #FCFFE0\n}\n\n.ace-kr-theme .ace_print-margin {\n  width: 1px;\n  background: #1c1917\n}\n\n.ace-kr-theme {\n  background-color: #0B0A09;\n  color: #FCFFE0\n}\n\n.ace-kr-theme .ace_cursor {\n  color: #FF9900\n}\n\n.ace-kr-theme .ace_marker-layer .ace_selection {\n  background: rgba(170, 0, 255, 0.45)\n}\n\n.ace-kr-theme.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #0B0A09;\n}\n\n.ace-kr-theme .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-kr-theme .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(255, 177, 111, 0.32)\n}\n\n.ace-kr-theme .ace_marker-layer .ace_active-line {\n  background: #38403D\n}\n\n.ace-kr-theme .ace_gutter-active-line {\n  background-color : #38403D\n}\n\n.ace-kr-theme .ace_marker-layer .ace_selected-word {\n  border: 1px solid rgba(170, 0, 255, 0.45)\n}\n\n.ace-kr-theme .ace_invisible {\n  color: rgba(255, 177, 111, 0.32)\n}\n\n.ace-kr-theme .ace_keyword,\n.ace-kr-theme .ace_meta {\n  color: #949C8B\n}\n\n.ace-kr-theme .ace_constant,\n.ace-kr-theme .ace_constant.ace_character,\n.ace-kr-theme .ace_constant.ace_character.ace_escape,\n.ace-kr-theme .ace_constant.ace_other {\n  color: rgba(210, 117, 24, 0.76)\n}\n\n.ace-kr-theme .ace_invalid {\n  color: #F8F8F8;\n  background-color: #A41300\n}\n\n.ace-kr-theme .ace_support {\n  color: #9FC28A\n}\n\n.ace-kr-theme .ace_support.ace_constant {\n  color: #C27E66\n}\n\n.ace-kr-theme .ace_fold {\n  background-color: #949C8B;\n  border-color: #FCFFE0\n}\n\n.ace-kr-theme .ace_support.ace_function {\n  color: #85873A\n}\n\n.ace-kr-theme .ace_storage {\n  color: #FFEE80\n}\n\n.ace-kr-theme .ace_string {\n  color: rgba(164, 161, 181, 0.8)\n}\n\n.ace-kr-theme .ace_string.ace_regexp {\n  color: rgba(125, 255, 192, 0.65)\n}\n\n.ace-kr-theme .ace_comment {\n  font-style: italic;\n  color: #706D5B\n}\n\n.ace-kr-theme .ace_variable {\n  color: #D1A796\n}\n\n.ace-kr-theme .ace_list,\n.ace-kr-theme .ace_markup.ace_list {\n  background-color: #0F0040\n}\n\n.ace-kr-theme .ace_variable.ace_language {\n  color: #FF80E1\n}\n\n.ace-kr-theme .ace_meta.ace_tag {\n  color: #BABD9C\n}\n\n.ace-kr-theme .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYFBXV/8PAAJoAXX4kT2EAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-kr-theme .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/kr_theme", ["require", "exports", "module", "ace/theme/kr_theme.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/kr_theme", ["require", "exports", "module", "ace/theme/kr_theme-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-kr-theme";
-    exports.cssText = require("./kr_theme.css");
+    exports.cssText = require("./kr_theme-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/kr_theme"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-kuroir.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-kuroir.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/kuroir.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/kuroir-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = "/* THIS THEME WAS AUTOGENERATED BY Theme.tmpl.css (UUID: 467560D0-6ACE-4409-82FD-4791420837AC) */\n\n.ace-kuroir .ace_gutter {\n  background: #e8e8e8;\n  color: #333;\n}\n\n.ace-kuroir .ace_print-margin {\n  width: 1px;\n  background: #e8e8e8;\n}\n\n.ace-kuroir {\n  background-color: #E8E9E8;\n  color: #363636;\n}\n\n.ace-kuroir .ace_cursor {\n  color: #202020;\n}\n\n.ace-kuroir .ace_marker-layer .ace_selection {\n  background: rgba(245, 170, 0, 0.57);\n}\n\n.ace-kuroir.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #E8E9E8;\n}\n\n.ace-kuroir .ace_marker-layer .ace_step {\n  background: rgb(198, 219, 174);\n}\n\n.ace-kuroir .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(0, 0, 0, 0.29);\n}\n\n.ace-kuroir .ace_marker-layer .ace_active-line {\n  background: rgba(203, 220, 47, 0.22);\n}\n\n.ace-kuroir .ace_gutter-active-line {\n  background-color: rgba(203, 220, 47, 0.22);\n}\n\n.ace-kuroir .ace_marker-layer .ace_selected-word {\n  border: 1px solid rgba(245, 170, 0, 0.57);\n}\n\n.ace-kuroir .ace_invisible {\n  color: #BFBFBF\n}\n\n.ace-kuroir .ace_fold {\n  border-color: #363636;\n}\n\n\n\n\n\n.ace-kuroir .ace_constant{color:#CD6839;}.ace-kuroir .ace_constant.ace_numeric{color:#9A5925;}.ace-kuroir .ace_support{color:#104E8B;}.ace-kuroir .ace_support.ace_function{color:#005273;}.ace-kuroir .ace_support.ace_constant{color:#CF6A4C;}.ace-kuroir .ace_storage{color:#A52A2A;}.ace-kuroir .ace_invalid.ace_illegal{color:#FD1224;\nbackground-color:rgba(255, 6, 0, 0.15);}.ace-kuroir .ace_invalid.ace_deprecated{text-decoration:underline;\nfont-style:italic;\ncolor:#FD1732;\nbackground-color:#E8E9E8;}.ace-kuroir .ace_string{color:#639300;}.ace-kuroir .ace_string.ace_regexp{color:#417E00;\nbackground-color:#C9D4BE;}.ace-kuroir .ace_comment{color:rgba(148, 148, 148, 0.91);\nbackground-color:rgba(220, 220, 220, 0.56);}.ace-kuroir .ace_variable{color:#009ACD;}.ace-kuroir .ace_meta.ace_tag{color:#005273;}.ace-kuroir .ace_markup.ace_heading{color:#B8012D;\nbackground-color:rgba(191, 97, 51, 0.051);}.ace-kuroir .ace_markup.ace_list{color:#8F5B26;}\n\n.ace-kuroir .ace_indent-guide {\n    background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bLly//BwAmVgd1/w11/gAAAABJRU5ErkJggg==\") right repeat-y;\n}\n\n.ace-kuroir .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n} \n";
 
 });
 
-define("ace/theme/kuroir", ["require", "exports", "module", "ace/theme/kuroir.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/kuroir", ["require", "exports", "module", "ace/theme/kuroir-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
     exports.cssClass = "ace-kuroir";
-    exports.cssText = require("./kuroir.css");
+    exports.cssText = require("./kuroir-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/kuroir"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-merbivore.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-merbivore.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/merbivore.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/merbivore-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-merbivore .ace_gutter {\n  background: #202020;\n  color: #E6E1DC\n}\n\n.ace-merbivore .ace_print-margin {\n  width: 1px;\n  background: #555651\n}\n\n.ace-merbivore {\n  background-color: #161616;\n  color: #E6E1DC\n}\n\n.ace-merbivore .ace_cursor {\n  color: #FFFFFF\n}\n\n.ace-merbivore .ace_marker-layer .ace_selection {\n  background: #454545\n}\n\n.ace-merbivore.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #161616;\n}\n\n.ace-merbivore .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-merbivore .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #404040\n}\n\n.ace-merbivore .ace_marker-layer .ace_active-line {\n  background: #333435\n}\n\n.ace-merbivore .ace_gutter-active-line {\n  background-color: #333435\n}\n\n.ace-merbivore .ace_marker-layer .ace_selected-word {\n  border: 1px solid #454545\n}\n\n.ace-merbivore .ace_invisible {\n  color: #404040\n}\n\n.ace-merbivore .ace_entity.ace_name.ace_tag,\n.ace-merbivore .ace_keyword,\n.ace-merbivore .ace_meta,\n.ace-merbivore .ace_meta.ace_tag,\n.ace-merbivore .ace_storage,\n.ace-merbivore .ace_support.ace_function {\n  color: #FC6F09\n}\n\n.ace-merbivore .ace_constant,\n.ace-merbivore .ace_constant.ace_character,\n.ace-merbivore .ace_constant.ace_character.ace_escape,\n.ace-merbivore .ace_constant.ace_other,\n.ace-merbivore .ace_support.ace_type {\n  color: #1EDAFB\n}\n\n.ace-merbivore .ace_constant.ace_character.ace_escape {\n  color: #519F50\n}\n\n.ace-merbivore .ace_constant.ace_language {\n  color: #FDC251\n}\n\n.ace-merbivore .ace_constant.ace_library,\n.ace-merbivore .ace_string,\n.ace-merbivore .ace_support.ace_constant {\n  color: #8DFF0A\n}\n\n.ace-merbivore .ace_constant.ace_numeric {\n  color: #58C554\n}\n\n.ace-merbivore .ace_invalid {\n  color: #FFFFFF;\n  background-color: #990000\n}\n\n.ace-merbivore .ace_fold {\n  background-color: #FC6F09;\n  border-color: #E6E1DC\n}\n\n.ace-merbivore .ace_comment {\n  font-style: italic;\n  color: #AD2EA4\n}\n\n.ace-merbivore .ace_entity.ace_other.ace_attribute-name {\n  color: #FFFF89\n}\n\n.ace-merbivore .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWMQFxf3ZXB1df0PAAdsAmERTkEHAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-merbivore .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/merbivore", ["require", "exports", "module", "ace/theme/merbivore.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/merbivore", ["require", "exports", "module", "ace/theme/merbivore-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-merbivore";
-    exports.cssText = require("./merbivore.css");
+    exports.cssText = require("./merbivore-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/merbivore"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-merbivore_soft.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-merbivore_soft.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/merbivore_soft.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/merbivore_soft-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-merbivore-soft .ace_gutter {\n  background: #262424;\n  color: #E6E1DC\n}\n\n.ace-merbivore-soft .ace_print-margin {\n  width: 1px;\n  background: #262424\n}\n\n.ace-merbivore-soft {\n  background-color: #1C1C1C;\n  color: #E6E1DC\n}\n\n.ace-merbivore-soft .ace_cursor {\n  color: #FFFFFF\n}\n\n.ace-merbivore-soft .ace_marker-layer .ace_selection {\n  background: #494949\n}\n\n.ace-merbivore-soft.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #1C1C1C;\n}\n\n.ace-merbivore-soft .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-merbivore-soft .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #404040\n}\n\n.ace-merbivore-soft .ace_marker-layer .ace_active-line {\n  background: #333435\n}\n\n.ace-merbivore-soft .ace_gutter-active-line {\n  background-color: #333435\n}\n\n.ace-merbivore-soft .ace_marker-layer .ace_selected-word {\n  border: 1px solid #494949\n}\n\n.ace-merbivore-soft .ace_invisible {\n  color: #404040\n}\n\n.ace-merbivore-soft .ace_entity.ace_name.ace_tag,\n.ace-merbivore-soft .ace_keyword,\n.ace-merbivore-soft .ace_meta,\n.ace-merbivore-soft .ace_meta.ace_tag,\n.ace-merbivore-soft .ace_storage {\n  color: #FC803A\n}\n\n.ace-merbivore-soft .ace_constant,\n.ace-merbivore-soft .ace_constant.ace_character,\n.ace-merbivore-soft .ace_constant.ace_character.ace_escape,\n.ace-merbivore-soft .ace_constant.ace_other,\n.ace-merbivore-soft .ace_support.ace_type {\n  color: #68C1D8\n}\n\n.ace-merbivore-soft .ace_constant.ace_character.ace_escape {\n  color: #B3E5B4\n}\n\n.ace-merbivore-soft .ace_constant.ace_language {\n  color: #E1C582\n}\n\n.ace-merbivore-soft .ace_constant.ace_library,\n.ace-merbivore-soft .ace_string,\n.ace-merbivore-soft .ace_support.ace_constant {\n  color: #8EC65F\n}\n\n.ace-merbivore-soft .ace_constant.ace_numeric {\n  color: #7FC578\n}\n\n.ace-merbivore-soft .ace_invalid,\n.ace-merbivore-soft .ace_invalid.ace_deprecated {\n  color: #FFFFFF;\n  background-color: #FE3838\n}\n\n.ace-merbivore-soft .ace_fold {\n  background-color: #FC803A;\n  border-color: #E6E1DC\n}\n\n.ace-merbivore-soft .ace_comment,\n.ace-merbivore-soft .ace_meta {\n  font-style: italic;\n  color: #AC4BB8\n}\n\n.ace-merbivore-soft .ace_entity.ace_other.ace_attribute-name {\n  color: #EAF1A3\n}\n\n.ace-merbivore-soft .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWOQkpLyZfD09PwPAAfYAnaStpHRAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-merbivore-soft .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/merbivore_soft", ["require", "exports", "module", "ace/theme/merbivore_soft.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/merbivore_soft", ["require", "exports", "module", "ace/theme/merbivore_soft-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-merbivore-soft";
-    exports.cssText = require("./merbivore_soft.css");
+    exports.cssText = require("./merbivore_soft-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/merbivore_soft"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-mono_industrial.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-mono_industrial.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/mono_industrial.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/mono_industrial-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-mono-industrial .ace_gutter {\n  background: #1d2521;\n  color: #C5C9C9\n}\n\n.ace-mono-industrial .ace_print-margin {\n  width: 1px;\n  background: #555651\n}\n\n.ace-mono-industrial {\n  background-color: #222C28;\n  color: #FFFFFF\n}\n\n.ace-mono-industrial .ace_cursor {\n  color: #FFFFFF\n}\n\n.ace-mono-industrial .ace_marker-layer .ace_selection {\n  background: rgba(145, 153, 148, 0.40)\n}\n\n.ace-mono-industrial.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #222C28;\n}\n\n.ace-mono-industrial .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-mono-industrial .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(102, 108, 104, 0.50)\n}\n\n.ace-mono-industrial .ace_marker-layer .ace_active-line {\n  background: rgba(12, 13, 12, 0.25)\n}\n\n.ace-mono-industrial .ace_gutter-active-line {\n  background-color: rgba(12, 13, 12, 0.25)\n}\n\n.ace-mono-industrial .ace_marker-layer .ace_selected-word {\n  border: 1px solid rgba(145, 153, 148, 0.40)\n}\n\n.ace-mono-industrial .ace_invisible {\n  color: rgba(102, 108, 104, 0.50)\n}\n\n.ace-mono-industrial .ace_string {\n  background-color: #151C19;\n  color: #FFFFFF\n}\n\n.ace-mono-industrial .ace_keyword,\n.ace-mono-industrial .ace_meta {\n  color: #A39E64\n}\n\n.ace-mono-industrial .ace_constant,\n.ace-mono-industrial .ace_constant.ace_character,\n.ace-mono-industrial .ace_constant.ace_character.ace_escape,\n.ace-mono-industrial .ace_constant.ace_numeric,\n.ace-mono-industrial .ace_constant.ace_other {\n  color: #E98800\n}\n\n.ace-mono-industrial .ace_entity.ace_name.ace_function,\n.ace-mono-industrial .ace_keyword.ace_operator,\n.ace-mono-industrial .ace_variable {\n  color: #A8B3AB\n}\n\n.ace-mono-industrial .ace_invalid {\n  color: #FFFFFF;\n  background-color: rgba(153, 0, 0, 0.68)\n}\n\n.ace-mono-industrial .ace_support.ace_constant {\n  color: #C87500\n}\n\n.ace-mono-industrial .ace_fold {\n  background-color: #A8B3AB;\n  border-color: #FFFFFF\n}\n\n.ace-mono-industrial .ace_support.ace_function {\n  color: #588E60\n}\n\n.ace-mono-industrial .ace_entity.ace_name,\n.ace-mono-industrial .ace_support.ace_class,\n.ace-mono-industrial .ace_support.ace_type {\n  color: #5778B6\n}\n\n.ace-mono-industrial .ace_storage {\n  color: #C23B00\n}\n\n.ace-mono-industrial .ace_variable.ace_language,\n.ace-mono-industrial .ace_variable.ace_parameter {\n  color: #648BD2\n}\n\n.ace-mono-industrial .ace_comment {\n  color: #666C68;\n  background-color: #151C19\n}\n\n.ace-mono-industrial .ace_entity.ace_other.ace_attribute-name {\n  color: #909993\n}\n\n.ace-mono-industrial .ace_entity.ace_name.ace_tag {\n  color: #A65EFF\n}\n\n.ace-mono-industrial .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNQ1NbwZfALD/4PAAlTArlEC4r/AAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-mono-industrial .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/mono_industrial", ["require", "exports", "module", "ace/theme/mono_industrial.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/mono_industrial", ["require", "exports", "module", "ace/theme/mono_industrial-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-mono-industrial";
-    exports.cssText = require("./mono_industrial.css");
+    exports.cssText = require("./mono_industrial-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/mono_industrial"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-monokai.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-monokai.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/monokai.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/monokai-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-monokai .ace_gutter {\n  background: #2F3129;\n  color: #8F908A\n}\n\n.ace-monokai .ace_print-margin {\n  width: 1px;\n  background: #555651\n}\n\n.ace-monokai {\n  background-color: #272822;\n  color: #F8F8F2\n}\n\n.ace-monokai .ace_cursor {\n  color: #F8F8F0\n}\n\n.ace-monokai .ace_marker-layer .ace_selection {\n  background: #49483E\n}\n\n.ace-monokai.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #272822;\n}\n\n.ace-monokai .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-monokai .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #49483E\n}\n\n.ace-monokai .ace_marker-layer .ace_active-line {\n  background: #202020\n}\n\n.ace-monokai .ace_gutter-active-line {\n  background-color: #272727\n}\n\n.ace-monokai .ace_marker-layer .ace_selected-word {\n  border: 1px solid #49483E\n}\n\n.ace-monokai .ace_invisible {\n  color: #52524d\n}\n\n.ace-monokai .ace_entity.ace_name.ace_tag,\n.ace-monokai .ace_keyword,\n.ace-monokai .ace_meta.ace_tag,\n.ace-monokai .ace_storage {\n  color: #F92672\n}\n\n.ace-monokai .ace_punctuation,\n.ace-monokai .ace_punctuation.ace_tag {\n  color: #fff\n}\n\n.ace-monokai .ace_constant.ace_character,\n.ace-monokai .ace_constant.ace_language,\n.ace-monokai .ace_constant.ace_numeric,\n.ace-monokai .ace_constant.ace_other {\n  color: #AE81FF\n}\n\n.ace-monokai .ace_invalid {\n  color: #F8F8F0;\n  background-color: #F92672\n}\n\n.ace-monokai .ace_invalid.ace_deprecated {\n  color: #F8F8F0;\n  background-color: #AE81FF\n}\n\n.ace-monokai .ace_support.ace_constant,\n.ace-monokai .ace_support.ace_function {\n  color: #66D9EF\n}\n\n.ace-monokai .ace_fold {\n  background-color: #A6E22E;\n  border-color: #F8F8F2\n}\n\n.ace-monokai .ace_storage.ace_type,\n.ace-monokai .ace_support.ace_class,\n.ace-monokai .ace_support.ace_type {\n  font-style: italic;\n  color: #66D9EF\n}\n\n.ace-monokai .ace_entity.ace_name.ace_function,\n.ace-monokai .ace_entity.ace_other,\n.ace-monokai .ace_entity.ace_other.ace_attribute-name,\n.ace-monokai .ace_variable {\n  color: #A6E22E\n}\n\n.ace-monokai .ace_variable.ace_parameter {\n  font-style: italic;\n  color: #FD971F\n}\n\n.ace-monokai .ace_string {\n  color: #E6DB74\n}\n\n.ace-monokai .ace_comment {\n  color: #75715E\n}\n\n.ace-monokai .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWPQ0FD0ZXBzd/wPAAjVAoxeSgNeAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-monokai .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/monokai", ["require", "exports", "module", "ace/theme/monokai.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/monokai", ["require", "exports", "module", "ace/theme/monokai-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-monokai";
-    exports.cssText = require("./monokai.css");
+    exports.cssText = require("./monokai-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/monokai"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-nord_dark.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-nord_dark.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/nord_dark.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/nord_dark-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-nord-dark .ace_gutter {\n  color: #616e88;\n}\n\n.ace-nord-dark .ace_print-margin {\n  width: 1px;\n  background: #4c566a;\n}\n\n.ace-nord-dark {\n  background-color: #2e3440;\n  color: #d8dee9;\n}\n\n.ace-nord-dark .ace_entity.ace_other.ace_attribute-name,\n.ace-nord-dark .ace_storage {\n  color: #d8dee9;\n}\n\n.ace-nord-dark .ace_cursor {\n  color: #d8dee9;\n}\n\n.ace-nord-dark .ace_string.ace_regexp {\n  color: #bf616a;\n}\n\n.ace-nord-dark .ace_marker-layer .ace_active-line {\n  background: #434c5ecc;\n}\n.ace-nord-dark .ace_marker-layer .ace_selection {\n  background: #434c5ecc;\n}\n\n.ace-nord-dark.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #2e3440;\n}\n\n.ace-nord-dark .ace_marker-layer .ace_step {\n  background: #ebcb8b;\n}\n\n.ace-nord-dark .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #88c0d066;\n}\n\n.ace-nord-dark .ace_gutter-active-line {\n  background-color: #434c5ecc;\n}\n\n.ace-nord-dark .ace_marker-layer .ace_selected-word {\n  border: 1px solid #88c0d066;\n}\n\n.ace-nord-dark .ace_invisible {\n  color: #4c566a;\n}\n\n.ace-nord-dark .ace_keyword,\n.ace-nord-dark .ace_meta,\n.ace-nord-dark .ace_support.ace_class,\n.ace-nord-dark .ace_support.ace_type {\n  color: #81a1c1;\n}\n\n.ace-nord-dark .ace_constant.ace_character,\n.ace-nord-dark .ace_constant.ace_other {\n  color: #d8dee9;\n}\n\n.ace-nord-dark .ace_constant.ace_language {\n  color: #5e81ac;\n}\n\n.ace-nord-dark .ace_constant.ace_escape {\n  color: #ebcB8b;\n}\n\n.ace-nord-dark .ace_constant.ace_numeric {\n  color: #b48ead;\n}\n\n.ace-nord-dark .ace_fold {\n  background-color: #4c566a;\n  border-color: #d8dee9;\n}\n\n.ace-nord-dark .ace_entity.ace_name.ace_function,\n.ace-nord-dark .ace_entity.ace_name.ace_tag,\n.ace-nord-dark .ace_support.ace_function,\n.ace-nord-dark .ace_variable,\n.ace-nord-dark .ace_variable.ace_language {\n  color: #8fbcbb;\n}\n\n.ace-nord-dark .ace_string {\n  color: #a3be8c;\n}\n\n.ace-nord-dark .ace_comment {\n  color: #616e88;\n}\n\n.ace-nord-dark .ace_indent-guide {\n  box-shadow: inset -1px 0 0 0 #434c5eb3;\n}\n\n.ace-nord-dark .ace_indent-guide-active {\n  box-shadow: inset -1px 0 0 0 #8395b8b3;\n}\n";
 
 });
 
-define("ace/theme/nord_dark", ["require", "exports", "module", "ace/theme/nord_dark.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/nord_dark", ["require", "exports", "module", "ace/theme/nord_dark-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-nord-dark";
-    exports.cssText = require("./nord_dark.css");
+    exports.cssText = require("./nord_dark-css");
     exports.$selectionColorConflict = true;
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/nord_dark"], function(m) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-one_dark.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-one_dark.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/one_dark.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/one_dark-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-one-dark .ace_gutter {\n    background: #282c34;\n    color: #6a6f7a\n}\n\n.ace-one-dark .ace_print-margin {\n    width: 1px;\n    background: #e8e8e8\n}\n\n.ace-one-dark {\n    background-color: #282c34;\n    color: #abb2bf\n}\n\n.ace-one-dark .ace_cursor {\n    color: #528bff\n}\n\n.ace-one-dark .ace_marker-layer .ace_selection {\n    background: #3d4350\n}\n\n.ace-one-dark.ace_multiselect .ace_selection.ace_start {\n    box-shadow: 0 0 3px 0 #282c34;\n    border-radius: 2px\n}\n\n.ace-one-dark .ace_marker-layer .ace_step {\n    background: #c6dbae\n}\n\n.ace-one-dark .ace_marker-layer .ace_bracket {\n    margin: -1px 0 0 -1px;\n    border: 1px solid #747369\n}\n\n.ace-one-dark .ace_marker-layer .ace_active-line {\n    background: rgba(76, 87, 103, .19)\n}\n\n.ace-one-dark .ace_gutter-active-line {\n    background-color: rgba(76, 87, 103, .19)\n}\n\n.ace-one-dark .ace_marker-layer .ace_selected-word {\n    border: 1px solid #3d4350\n}\n\n.ace-one-dark .ace_fold {\n    background-color: #61afef;\n    border-color: #abb2bf\n}\n\n.ace-one-dark .ace_keyword {\n    color: #c678dd\n}\n\n.ace-one-dark .ace_keyword.ace_operator {\n    color: #c678dd\n}\n\n.ace-one-dark .ace_keyword.ace_other.ace_unit {\n    color: #d19a66\n}\n\n.ace-one-dark .ace_constant.ace_language {\n    color: #d19a66\n}\n\n.ace-one-dark .ace_constant.ace_numeric {\n    color: #d19a66\n}\n\n.ace-one-dark .ace_constant.ace_character {\n    color: #56b6c2\n}\n\n.ace-one-dark .ace_constant.ace_other {\n    color: #56b6c2\n}\n\n.ace-one-dark .ace_support.ace_function {\n    color: #61afef\n}\n\n.ace-one-dark .ace_support.ace_constant {\n    color: #d19a66\n}\n\n.ace-one-dark .ace_support.ace_class {\n    color: #e5c07b\n}\n\n.ace-one-dark .ace_support.ace_type {\n    color: #e5c07b\n}\n\n.ace-one-dark .ace_storage {\n    color: #c678dd\n}\n\n.ace-one-dark .ace_storage.ace_type {\n    color: #c678dd\n}\n\n.ace-one-dark .ace_invalid {\n    color: #fff;\n    background-color: #f2777a\n}\n\n.ace-one-dark .ace_invalid.ace_deprecated {\n    color: #272b33;\n    background-color: #d27b53\n}\n\n.ace-one-dark .ace_string {\n    color: #98c379\n}\n\n.ace-one-dark .ace_string.ace_regexp {\n    color: #e06c75\n}\n\n.ace-one-dark .ace_comment {\n    font-style: italic;\n    color: #5c6370\n}\n\n.ace-one-dark .ace_variable {\n    color: #e06c75\n}\n\n.ace-one-dark .ace_variable.ace_parameter {\n    color: #d19a66\n}\n\n.ace-one-dark .ace_meta.ace_tag {\n    color: #e06c75\n}\n\n.ace-one-dark .ace_entity.ace_other.ace_attribute-name {\n    color: #e06c75\n}\n\n.ace-one-dark .ace_entity.ace_name.ace_function {\n    color: #61afef\n}\n\n.ace-one-dark .ace_entity.ace_name.ace_tag {\n    color: #e06c75\n}\n\n.ace-one-dark .ace_markup.ace_heading {\n    color: #98c379\n}\n\n.ace-one-dark .ace_indent-guide {\n    background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWPQ09NrYAgMjP4PAAtGAwchHMyAAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-one-dark .ace_indent-guide-active {\n    background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/one_dark", ["require", "exports", "module", "ace/theme/one_dark.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/one_dark", ["require", "exports", "module", "ace/theme/one_dark-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-one-dark";
-    exports.cssText = require("./one_dark.css");
+    exports.cssText = require("./one_dark-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/one_dark"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-pastel_on_dark.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-pastel_on_dark.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/pastel_on_dark.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/pastel_on_dark-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-pastel-on-dark .ace_gutter {\n  background: #353030;\n  color: #8F938F\n}\n\n.ace-pastel-on-dark .ace_print-margin {\n  width: 1px;\n  background: #353030\n}\n\n.ace-pastel-on-dark {\n  background-color: #2C2828;\n  color: #8F938F\n}\n\n.ace-pastel-on-dark .ace_cursor {\n  color: #A7A7A7\n}\n\n.ace-pastel-on-dark .ace_marker-layer .ace_selection {\n  background: rgba(221, 240, 255, 0.20)\n}\n\n.ace-pastel-on-dark.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #2C2828;\n}\n\n.ace-pastel-on-dark .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-pastel-on-dark .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(255, 255, 255, 0.25)\n}\n\n.ace-pastel-on-dark .ace_marker-layer .ace_active-line {\n  background: rgba(255, 255, 255, 0.031)\n}\n\n.ace-pastel-on-dark .ace_gutter-active-line {\n  background-color: rgba(255, 255, 255, 0.031)\n}\n\n.ace-pastel-on-dark .ace_marker-layer .ace_selected-word {\n  border: 1px solid rgba(221, 240, 255, 0.20)\n}\n\n.ace-pastel-on-dark .ace_invisible {\n  color: rgba(255, 255, 255, 0.25)\n}\n\n.ace-pastel-on-dark .ace_keyword,\n.ace-pastel-on-dark .ace_meta {\n  color: #757aD8\n}\n\n.ace-pastel-on-dark .ace_constant,\n.ace-pastel-on-dark .ace_constant.ace_character,\n.ace-pastel-on-dark .ace_constant.ace_character.ace_escape,\n.ace-pastel-on-dark .ace_constant.ace_other {\n  color: #4FB7C5\n}\n\n.ace-pastel-on-dark .ace_keyword.ace_operator {\n  color: #797878\n}\n\n.ace-pastel-on-dark .ace_constant.ace_character {\n  color: #AFA472\n}\n\n.ace-pastel-on-dark .ace_constant.ace_language {\n  color: #DE8E30\n}\n\n.ace-pastel-on-dark .ace_constant.ace_numeric {\n  color: #CCCCCC\n}\n\n.ace-pastel-on-dark .ace_invalid,\n.ace-pastel-on-dark .ace_invalid.ace_illegal {\n  color: #F8F8F8;\n  background-color: rgba(86, 45, 86, 0.75)\n}\n\n.ace-pastel-on-dark .ace_invalid.ace_deprecated {\n  text-decoration: underline;\n  font-style: italic;\n  color: #D2A8A1\n}\n\n.ace-pastel-on-dark .ace_fold {\n  background-color: #757aD8;\n  border-color: #8F938F\n}\n\n.ace-pastel-on-dark .ace_support.ace_function {\n  color: #AEB2F8\n}\n\n.ace-pastel-on-dark .ace_string {\n  color: #66A968\n}\n\n.ace-pastel-on-dark .ace_string.ace_regexp {\n  color: #E9C062\n}\n\n.ace-pastel-on-dark .ace_comment {\n  color: #A6C6FF\n}\n\n.ace-pastel-on-dark .ace_variable {\n  color: #BEBF55\n}\n\n.ace-pastel-on-dark .ace_variable.ace_language {\n  color: #C1C144\n}\n\n.ace-pastel-on-dark .ace_xml-pe {\n  color: #494949\n}\n\n.ace-pastel-on-dark .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYIiPj/8PAARgAh2NTMh8AAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-pastel-on-dark .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/pastel_on_dark", ["require", "exports", "module", "ace/theme/pastel_on_dark.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/pastel_on_dark", ["require", "exports", "module", "ace/theme/pastel_on_dark-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-pastel-on-dark";
-    exports.cssText = require("./pastel_on_dark.css");
+    exports.cssText = require("./pastel_on_dark-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/pastel_on_dark"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-solarized_dark.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-solarized_dark.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/solarized_dark.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/solarized_dark-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-solarized-dark .ace_gutter {\n  background: #01313f;\n  color: #d0edf7\n}\n\n.ace-solarized-dark .ace_print-margin {\n  width: 1px;\n  background: #33555E\n}\n\n.ace-solarized-dark {\n  background-color: #002B36;\n  color: #93A1A1\n}\n\n.ace-solarized-dark .ace_entity.ace_other.ace_attribute-name,\n.ace-solarized-dark .ace_storage {\n  color: #93A1A1\n}\n\n.ace-solarized-dark .ace_cursor,\n.ace-solarized-dark .ace_string.ace_regexp {\n  color: #D30102\n}\n\n.ace-solarized-dark .ace_marker-layer .ace_active-line,\n.ace-solarized-dark .ace_marker-layer .ace_selection {\n  background: rgba(255, 255, 255, 0.1)\n}\n\n.ace-solarized-dark.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #002B36;\n}\n\n.ace-solarized-dark .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-solarized-dark .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(147, 161, 161, 0.50)\n}\n\n.ace-solarized-dark .ace_gutter-active-line {\n  background-color: #0d3440\n}\n\n.ace-solarized-dark .ace_marker-layer .ace_selected-word {\n  border: 1px solid #073642\n}\n\n.ace-solarized-dark .ace_invisible {\n  color: rgba(147, 161, 161, 0.50)\n}\n\n.ace-solarized-dark .ace_keyword,\n.ace-solarized-dark .ace_meta,\n.ace-solarized-dark .ace_support.ace_class,\n.ace-solarized-dark .ace_support.ace_type {\n  color: #859900\n}\n\n.ace-solarized-dark .ace_constant.ace_character,\n.ace-solarized-dark .ace_constant.ace_other {\n  color: #CB4B16\n}\n\n.ace-solarized-dark .ace_constant.ace_language {\n  color: #B58900\n}\n\n.ace-solarized-dark .ace_constant.ace_numeric {\n  color: #D33682\n}\n\n.ace-solarized-dark .ace_fold {\n  background-color: #268BD2;\n  border-color: #93A1A1\n}\n\n.ace-solarized-dark .ace_entity.ace_name.ace_function,\n.ace-solarized-dark .ace_entity.ace_name.ace_tag,\n.ace-solarized-dark .ace_support.ace_function,\n.ace-solarized-dark .ace_variable,\n.ace-solarized-dark .ace_variable.ace_language {\n  color: #268BD2\n}\n\n.ace-solarized-dark .ace_string {\n  color: #2AA198\n}\n\n.ace-solarized-dark .ace_comment {\n  font-style: italic;\n  color: #657B83\n}\n\n.ace-solarized-dark .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNg0Db1ZVCxc/sPAAd4AlUHlLenAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-solarized-dark .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/solarized_dark", ["require", "exports", "module", "ace/theme/solarized_dark.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/solarized_dark", ["require", "exports", "module", "ace/theme/solarized_dark-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-solarized-dark";
-    exports.cssText = require("./solarized_dark.css");
+    exports.cssText = require("./solarized_dark-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/solarized_dark"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-solarized_light.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-solarized_light.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/solarized_light.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/solarized_light-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-solarized-light .ace_gutter {\n  background: #fbf1d3;\n  color: #333\n}\n\n.ace-solarized-light .ace_print-margin {\n  width: 1px;\n  background: #e8e8e8\n}\n\n.ace-solarized-light {\n  background-color: #FDF6E3;\n  color: #586E75\n}\n\n.ace-solarized-light .ace_cursor {\n  color: #000000\n}\n\n.ace-solarized-light .ace_marker-layer .ace_selection {\n  background: rgba(7, 54, 67, 0.09)\n}\n\n.ace-solarized-light.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #FDF6E3;\n}\n\n.ace-solarized-light .ace_marker-layer .ace_step {\n  background: rgb(255, 255, 0)\n}\n\n.ace-solarized-light .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(147, 161, 161, 0.50)\n}\n\n.ace-solarized-light .ace_marker-layer .ace_active-line {\n  background: #EEE8D5\n}\n\n.ace-solarized-light .ace_gutter-active-line {\n  background-color : #EDE5C1\n}\n\n.ace-solarized-light .ace_marker-layer .ace_selected-word {\n  border: 1px solid #7f9390\n}\n\n.ace-solarized-light .ace_invisible {\n  color: rgba(147, 161, 161, 0.50)\n}\n\n.ace-solarized-light .ace_keyword,\n.ace-solarized-light .ace_meta,\n.ace-solarized-light .ace_support.ace_class,\n.ace-solarized-light .ace_support.ace_type {\n  color: #859900\n}\n\n.ace-solarized-light .ace_constant.ace_character,\n.ace-solarized-light .ace_constant.ace_other {\n  color: #CB4B16\n}\n\n.ace-solarized-light .ace_constant.ace_language {\n  color: #B58900\n}\n\n.ace-solarized-light .ace_constant.ace_numeric {\n  color: #D33682\n}\n\n.ace-solarized-light .ace_fold {\n  background-color: #268BD2;\n  border-color: #586E75\n}\n\n.ace-solarized-light .ace_entity.ace_name.ace_function,\n.ace-solarized-light .ace_entity.ace_name.ace_tag,\n.ace-solarized-light .ace_support.ace_function,\n.ace-solarized-light .ace_variable,\n.ace-solarized-light .ace_variable.ace_language {\n  color: #268BD2\n}\n\n.ace-solarized-light .ace_storage {\n  color: #073642\n}\n\n.ace-solarized-light .ace_string {\n  color: #2AA198\n}\n\n.ace-solarized-light .ace_string.ace_regexp {\n  color: #D30102\n}\n\n.ace-solarized-light .ace_comment,\n.ace-solarized-light .ace_entity.ace_other.ace_attribute-name {\n  color: #93A1A1\n}\n\n.ace-solarized-light .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYHjy8NJ/AAjgA5fzQUmBAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-solarized-light .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n} \n";
 
 });
 
-define("ace/theme/solarized_light", ["require", "exports", "module", "ace/theme/solarized_light.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/solarized_light", ["require", "exports", "module", "ace/theme/solarized_light-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
     exports.cssClass = "ace-solarized-light";
-    exports.cssText = require("./solarized_light.css");
+    exports.cssText = require("./solarized_light-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/solarized_light"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-sqlserver.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-sqlserver.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/sqlserver.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/sqlserver-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-sqlserver .ace_gutter {\n    background: #ebebeb;\n    color: #333;\n    overflow: hidden;\n}\n\n.ace-sqlserver .ace_print-margin {\n    width: 1px;\n    background: #e8e8e8;\n}\n\n.ace-sqlserver {\n    background-color: #FFFFFF;\n    color: black;\n}\n\n.ace-sqlserver .ace_identifier {\n    color: black;\n}\n\n.ace-sqlserver .ace_keyword {\n    color: #0000FF;\n}\n\n.ace-sqlserver .ace_numeric {\n    color: black;\n}\n\n.ace-sqlserver .ace_storage {\n    color: #11B7BE;\n}\n\n.ace-sqlserver .ace_keyword.ace_operator,\n.ace-sqlserver .ace_lparen,\n.ace-sqlserver .ace_rparen,\n.ace-sqlserver .ace_punctuation {\n    color: #808080;\n}\n\n.ace-sqlserver .ace_set.ace_statement {\n    color: #0000FF;\n    text-decoration: underline;\n}\n\n.ace-sqlserver .ace_cursor {\n    color: black;\n}\n\n.ace-sqlserver .ace_invisible {\n    color: rgb(191, 191, 191);\n}\n\n.ace-sqlserver .ace_constant.ace_buildin {\n    color: rgb(88, 72, 246);\n}\n\n.ace-sqlserver .ace_constant.ace_language {\n    color: #979797;\n}\n\n.ace-sqlserver .ace_constant.ace_library {\n    color: rgb(6, 150, 14);\n}\n\n.ace-sqlserver .ace_invalid {\n    background-color: rgb(153, 0, 0);\n    color: white;\n}\n\n.ace-sqlserver .ace_support.ace_function {\n    color: #FF00FF;\n}\n\n.ace-sqlserver .ace_support.ace_constant {\n    color: rgb(6, 150, 14);\n}\n\n.ace-sqlserver .ace_class {\n    color: #008080;\n}\n\n.ace-sqlserver .ace_support.ace_other {\n    color: #6D79DE;\n}\n\n.ace-sqlserver .ace_variable.ace_parameter {\n    font-style: italic;\n    color: #FD971F;\n}\n\n.ace-sqlserver .ace_comment {\n    color: #008000;\n}\n\n.ace-sqlserver .ace_constant.ace_numeric {\n    color: black;\n}\n\n.ace-sqlserver .ace_variable {\n    color: rgb(49, 132, 149);\n}\n\n.ace-sqlserver .ace_xml-pe {\n    color: rgb(104, 104, 91);\n}\n\n.ace-sqlserver .ace_support.ace_storedprocedure {\n    color: #800000;\n}\n\n.ace-sqlserver .ace_heading {\n    color: rgb(12, 7, 255);\n}\n\n.ace-sqlserver .ace_list {\n    color: rgb(185, 6, 144);\n}\n\n.ace-sqlserver .ace_marker-layer .ace_selection {\n    background: rgb(181, 213, 255);\n}\n\n.ace-sqlserver .ace_marker-layer .ace_step {\n    background: rgb(252, 255, 0);\n}\n\n.ace-sqlserver .ace_marker-layer .ace_stack {\n    background: rgb(164, 229, 101);\n}\n\n.ace-sqlserver .ace_marker-layer .ace_bracket {\n    margin: -1px 0 0 -1px;\n    border: 1px solid rgb(192, 192, 192);\n}\n\n.ace-sqlserver .ace_marker-layer .ace_active-line {\n    background: rgba(0, 0, 0, 0.07);\n}\n\n.ace-sqlserver .ace_gutter-active-line {\n    background-color: #dcdcdc;\n}\n\n.ace-sqlserver .ace_marker-layer .ace_selected-word {\n    background: rgb(250, 250, 255);\n    border: 1px solid rgb(200, 200, 250);\n}\n\n.ace-sqlserver .ace_meta.ace_tag {\n    color: #0000FF;\n}\n\n.ace-sqlserver .ace_string.ace_regex {\n    color: #FF0000;\n}\n\n.ace-sqlserver .ace_string {\n    color: #FF0000;\n}\n\n.ace-sqlserver .ace_entity.ace_other.ace_attribute-name {\n    color: #994409;\n}\n\n.ace-sqlserver .ace_indent-guide {\n    background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bLly//BwAmVgd1/w11/gAAAABJRU5ErkJggg==\") right repeat-y;\n}\n\n.ace-sqlserver .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n} \n";
 
 });
 
-define("ace/theme/sqlserver", ["require", "exports", "module", "ace/theme/sqlserver.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/sqlserver", ["require", "exports", "module", "ace/theme/sqlserver-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
     exports.cssClass = "ace-sqlserver";
-    exports.cssText = require("./sqlserver.css");
+    exports.cssText = require("./sqlserver-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/sqlserver"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-terminal.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-terminal.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/terminal.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/terminal-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-terminal-theme .ace_gutter {\n  background: #1a0005;\n  color: steelblue\n}\n\n.ace-terminal-theme .ace_print-margin {\n  width: 1px;\n  background: #1a1a1a\n}\n\n.ace-terminal-theme {\n  background-color: black;\n  color: #DEDEDE\n}\n\n.ace-terminal-theme .ace_cursor {\n  color: #9F9F9F\n}\n\n.ace-terminal-theme .ace_marker-layer .ace_selection {\n  background: #424242\n}\n\n.ace-terminal-theme.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px black;\n}\n\n.ace-terminal-theme .ace_marker-layer .ace_step {\n  background: rgb(0, 0, 0)\n}\n\n.ace-terminal-theme .ace_marker-layer .ace_bracket {\n  background: #090;\n}\n\n.ace-terminal-theme .ace_marker-layer .ace_bracket-start {\n  background: #090;\n}\n\n.ace-terminal-theme .ace_marker-layer .ace_bracket-unmatched {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #900\n}\n\n.ace-terminal-theme .ace_marker-layer .ace_active-line {\n  background: #2A2A2A\n}\n\n.ace-terminal-theme .ace_gutter-active-line {\n  background-color: #2A112A\n}\n\n.ace-terminal-theme .ace_marker-layer .ace_selected-word {\n  border: 1px solid #424242\n}\n\n.ace-terminal-theme .ace_invisible {\n  color: #343434\n}\n\n.ace-terminal-theme .ace_keyword,\n.ace-terminal-theme .ace_meta,\n.ace-terminal-theme .ace_storage,\n.ace-terminal-theme .ace_storage.ace_type,\n.ace-terminal-theme .ace_support.ace_type {\n  color: tomato\n}\n\n.ace-terminal-theme .ace_keyword.ace_operator {\n  color: deeppink\n}\n\n.ace-terminal-theme .ace_constant.ace_character,\n.ace-terminal-theme .ace_constant.ace_language,\n.ace-terminal-theme .ace_constant.ace_numeric,\n.ace-terminal-theme .ace_keyword.ace_other.ace_unit,\n.ace-terminal-theme .ace_support.ace_constant,\n.ace-terminal-theme .ace_variable.ace_parameter {\n  color: #E78C45\n}\n\n.ace-terminal-theme .ace_constant.ace_other {\n  color: gold\n}\n\n.ace-terminal-theme .ace_invalid {\n  color: yellow;\n  background-color: red\n}\n\n.ace-terminal-theme .ace_invalid.ace_deprecated {\n  color: #CED2CF;\n  background-color: #B798BF\n}\n\n.ace-terminal-theme .ace_fold {\n  background-color: #7AA6DA;\n  border-color: #DEDEDE\n}\n\n.ace-terminal-theme .ace_entity.ace_name.ace_function,\n.ace-terminal-theme .ace_support.ace_function,\n.ace-terminal-theme .ace_variable {\n  color: #7AA6DA\n}\n\n.ace-terminal-theme .ace_support.ace_class,\n.ace-terminal-theme .ace_support.ace_type {\n  color: #E7C547\n}\n\n.ace-terminal-theme .ace_heading,\n.ace-terminal-theme .ace_string {\n  color: #B9CA4A\n}\n\n.ace-terminal-theme .ace_entity.ace_name.ace_tag,\n.ace-terminal-theme .ace_entity.ace_other.ace_attribute-name,\n.ace-terminal-theme .ace_meta.ace_tag,\n.ace-terminal-theme .ace_string.ace_regexp,\n.ace-terminal-theme .ace_variable {\n  color: #D54E53\n}\n\n.ace-terminal-theme .ace_comment {\n  color: orangered\n}\n\n.ace-terminal-theme .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYLBWV/8PAAK4AYnhiq+xAAAAAElFTkSuQmCC) right repeat-y;\n}\n\n.ace-terminal-theme .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/terminal", ["require", "exports", "module", "ace/theme/terminal.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/terminal", ["require", "exports", "module", "ace/theme/terminal-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-terminal-theme";
-    exports.cssText = require("./terminal.css");
+    exports.cssText = require("./terminal-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/terminal"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-textmate.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-textmate.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
-define("ace/theme/textmate", ["require", "exports", "module", "ace/theme/textmate.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/textmate", ["require", "exports", "module", "ace/theme/textmate-css", "ace/lib/dom"], function(require, exports, module) {
     "use strict";
     exports.isDark = false;
     exports.cssClass = "ace-tm";
-    exports.cssText = require("./textmate.css");
+    exports.cssText = require("./textmate-css");
     exports.$id = "ace/theme/textmate";
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/textmate"], function(m) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-tomorrow.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-tomorrow.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/tomorrow.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/tomorrow-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-tomorrow .ace_gutter {\n  background: #f6f6f6;\n  color: #4D4D4C\n}\n\n.ace-tomorrow .ace_print-margin {\n  width: 1px;\n  background: #f6f6f6\n}\n\n.ace-tomorrow {\n  background-color: #FFFFFF;\n  color: #4D4D4C\n}\n\n.ace-tomorrow .ace_cursor {\n  color: #AEAFAD\n}\n\n.ace-tomorrow .ace_marker-layer .ace_selection {\n  background: #D6D6D6\n}\n\n.ace-tomorrow.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #FFFFFF;\n}\n\n.ace-tomorrow .ace_marker-layer .ace_step {\n  background: rgb(255, 255, 0)\n}\n\n.ace-tomorrow .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #D1D1D1\n}\n\n.ace-tomorrow .ace_marker-layer .ace_active-line {\n  background: #EFEFEF\n}\n\n.ace-tomorrow .ace_gutter-active-line {\n  background-color : #dcdcdc\n}\n\n.ace-tomorrow .ace_marker-layer .ace_selected-word {\n  border: 1px solid #D6D6D6\n}\n\n.ace-tomorrow .ace_invisible {\n  color: #D1D1D1\n}\n\n.ace-tomorrow .ace_keyword,\n.ace-tomorrow .ace_meta,\n.ace-tomorrow .ace_storage,\n.ace-tomorrow .ace_storage.ace_type,\n.ace-tomorrow .ace_support.ace_type {\n  color: #8959A8\n}\n\n.ace-tomorrow .ace_keyword.ace_operator {\n  color: #3E999F\n}\n\n.ace-tomorrow .ace_constant.ace_character,\n.ace-tomorrow .ace_constant.ace_language,\n.ace-tomorrow .ace_constant.ace_numeric,\n.ace-tomorrow .ace_keyword.ace_other.ace_unit,\n.ace-tomorrow .ace_support.ace_constant,\n.ace-tomorrow .ace_variable.ace_parameter {\n  color: #F5871F\n}\n\n.ace-tomorrow .ace_constant.ace_other {\n  color: #666969\n}\n\n.ace-tomorrow .ace_invalid {\n  color: #FFFFFF;\n  background-color: #C82829\n}\n\n.ace-tomorrow .ace_invalid.ace_deprecated {\n  color: #FFFFFF;\n  background-color: #8959A8\n}\n\n.ace-tomorrow .ace_fold {\n  background-color: #4271AE;\n  border-color: #4D4D4C\n}\n\n.ace-tomorrow .ace_entity.ace_name.ace_function,\n.ace-tomorrow .ace_support.ace_function,\n.ace-tomorrow .ace_variable {\n  color: #4271AE\n}\n\n.ace-tomorrow .ace_support.ace_class,\n.ace-tomorrow .ace_support.ace_type {\n  color: #C99E00\n}\n\n.ace-tomorrow .ace_heading,\n.ace-tomorrow .ace_markup.ace_heading,\n.ace-tomorrow .ace_string {\n  color: #718C00\n}\n\n.ace-tomorrow .ace_entity.ace_name.ace_tag,\n.ace-tomorrow .ace_entity.ace_other.ace_attribute-name,\n.ace-tomorrow .ace_meta.ace_tag,\n.ace-tomorrow .ace_string.ace_regexp,\n.ace-tomorrow .ace_variable {\n  color: #C82829\n}\n\n.ace-tomorrow .ace_comment {\n  color: #8E908C\n}\n\n.ace-tomorrow .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bdu3f/BwAlfgctduB85QAAAABJRU5ErkJggg==) right repeat-y\n}\n\n.ace-tomorrow .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n} \n";
 
 });
 
-define("ace/theme/tomorrow", ["require", "exports", "module", "ace/theme/tomorrow.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/tomorrow", ["require", "exports", "module", "ace/theme/tomorrow-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
     exports.cssClass = "ace-tomorrow";
-    exports.cssText = require("./tomorrow.css");
+    exports.cssText = require("./tomorrow-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/tomorrow"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-tomorrow_night.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-tomorrow_night.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/tomorrow_night.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/tomorrow_night-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-tomorrow-night .ace_gutter {\n  background: #25282c;\n  color: #C5C8C6\n}\n\n.ace-tomorrow-night .ace_print-margin {\n  width: 1px;\n  background: #25282c\n}\n\n.ace-tomorrow-night {\n  background-color: #1D1F21;\n  color: #C5C8C6\n}\n\n.ace-tomorrow-night .ace_cursor {\n  color: #AEAFAD\n}\n\n.ace-tomorrow-night .ace_marker-layer .ace_selection {\n  background: #373B41\n}\n\n.ace-tomorrow-night.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #1D1F21;\n}\n\n.ace-tomorrow-night .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-tomorrow-night .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #4B4E55\n}\n\n.ace-tomorrow-night .ace_marker-layer .ace_active-line {\n  background: #282A2E\n}\n\n.ace-tomorrow-night .ace_gutter-active-line {\n  background-color: #282A2E\n}\n\n.ace-tomorrow-night .ace_marker-layer .ace_selected-word {\n  border: 1px solid #373B41\n}\n\n.ace-tomorrow-night .ace_invisible {\n  color: #4B4E55\n}\n\n.ace-tomorrow-night .ace_keyword,\n.ace-tomorrow-night .ace_meta,\n.ace-tomorrow-night .ace_storage,\n.ace-tomorrow-night .ace_storage.ace_type,\n.ace-tomorrow-night .ace_support.ace_type {\n  color: #B294BB\n}\n\n.ace-tomorrow-night .ace_keyword.ace_operator {\n  color: #8ABEB7\n}\n\n.ace-tomorrow-night .ace_constant.ace_character,\n.ace-tomorrow-night .ace_constant.ace_language,\n.ace-tomorrow-night .ace_constant.ace_numeric,\n.ace-tomorrow-night .ace_keyword.ace_other.ace_unit,\n.ace-tomorrow-night .ace_support.ace_constant,\n.ace-tomorrow-night .ace_variable.ace_parameter {\n  color: #DE935F\n}\n\n.ace-tomorrow-night .ace_constant.ace_other {\n  color: #CED1CF\n}\n\n.ace-tomorrow-night .ace_invalid {\n  color: #CED2CF;\n  background-color: #DF5F5F\n}\n\n.ace-tomorrow-night .ace_invalid.ace_deprecated {\n  color: #CED2CF;\n  background-color: #B798BF\n}\n\n.ace-tomorrow-night .ace_fold {\n  background-color: #81A2BE;\n  border-color: #C5C8C6\n}\n\n.ace-tomorrow-night .ace_entity.ace_name.ace_function,\n.ace-tomorrow-night .ace_support.ace_function,\n.ace-tomorrow-night .ace_variable {\n  color: #81A2BE\n}\n\n.ace-tomorrow-night .ace_support.ace_class,\n.ace-tomorrow-night .ace_support.ace_type {\n  color: #F0C674\n}\n\n.ace-tomorrow-night .ace_heading,\n.ace-tomorrow-night .ace_markup.ace_heading,\n.ace-tomorrow-night .ace_string {\n  color: #B5BD68\n}\n\n.ace-tomorrow-night .ace_entity.ace_name.ace_tag,\n.ace-tomorrow-night .ace_entity.ace_other.ace_attribute-name,\n.ace-tomorrow-night .ace_meta.ace_tag,\n.ace-tomorrow-night .ace_string.ace_regexp,\n.ace-tomorrow-night .ace_variable {\n  color: #CC6666\n}\n\n.ace-tomorrow-night .ace_comment {\n  color: #969896\n}\n\n.ace-tomorrow-night .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYHB3d/8PAAOIAdULw8qMAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-tomorrow-night .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/tomorrow_night", ["require", "exports", "module", "ace/theme/tomorrow_night.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/tomorrow_night", ["require", "exports", "module", "ace/theme/tomorrow_night-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-tomorrow-night";
-    exports.cssText = require("./tomorrow_night.css");
+    exports.cssText = require("./tomorrow_night-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/tomorrow_night"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-tomorrow_night_blue.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-tomorrow_night_blue.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/tomorrow_night_blue.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/tomorrow_night_blue-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-tomorrow-night-blue .ace_gutter {\n  background: #00204b;\n  color: #7388b5\n}\n\n.ace-tomorrow-night-blue .ace_print-margin {\n  width: 1px;\n  background: #00204b\n}\n\n.ace-tomorrow-night-blue {\n  background-color: #002451;\n  color: #FFFFFF\n}\n\n.ace-tomorrow-night-blue .ace_constant.ace_other,\n.ace-tomorrow-night-blue .ace_cursor {\n  color: #FFFFFF\n}\n\n.ace-tomorrow-night-blue .ace_marker-layer .ace_selection {\n  background: #003F8E\n}\n\n.ace-tomorrow-night-blue.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #002451;\n}\n\n.ace-tomorrow-night-blue .ace_marker-layer .ace_step {\n  background: rgb(127, 111, 19)\n}\n\n.ace-tomorrow-night-blue .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #404F7D\n}\n\n.ace-tomorrow-night-blue .ace_marker-layer .ace_active-line {\n  background: #00346E\n}\n\n.ace-tomorrow-night-blue .ace_gutter-active-line {\n  background-color: #022040\n}\n\n.ace-tomorrow-night-blue .ace_marker-layer .ace_selected-word {\n  border: 1px solid #003F8E\n}\n\n.ace-tomorrow-night-blue .ace_invisible {\n  color: #404F7D\n}\n\n.ace-tomorrow-night-blue .ace_keyword,\n.ace-tomorrow-night-blue .ace_meta,\n.ace-tomorrow-night-blue .ace_storage,\n.ace-tomorrow-night-blue .ace_storage.ace_type,\n.ace-tomorrow-night-blue .ace_support.ace_type {\n  color: #EBBBFF\n}\n\n.ace-tomorrow-night-blue .ace_keyword.ace_operator {\n  color: #99FFFF\n}\n\n.ace-tomorrow-night-blue .ace_constant.ace_character,\n.ace-tomorrow-night-blue .ace_constant.ace_language,\n.ace-tomorrow-night-blue .ace_constant.ace_numeric,\n.ace-tomorrow-night-blue .ace_keyword.ace_other.ace_unit,\n.ace-tomorrow-night-blue .ace_support.ace_constant,\n.ace-tomorrow-night-blue .ace_variable.ace_parameter {\n  color: #FFC58F\n}\n\n.ace-tomorrow-night-blue .ace_invalid {\n  color: #FFFFFF;\n  background-color: #F99DA5\n}\n\n.ace-tomorrow-night-blue .ace_invalid.ace_deprecated {\n  color: #FFFFFF;\n  background-color: #EBBBFF\n}\n\n.ace-tomorrow-night-blue .ace_fold {\n  background-color: #BBDAFF;\n  border-color: #FFFFFF\n}\n\n.ace-tomorrow-night-blue .ace_entity.ace_name.ace_function,\n.ace-tomorrow-night-blue .ace_support.ace_function,\n.ace-tomorrow-night-blue .ace_variable {\n  color: #BBDAFF\n}\n\n.ace-tomorrow-night-blue .ace_support.ace_class,\n.ace-tomorrow-night-blue .ace_support.ace_type {\n  color: #FFEEAD\n}\n\n.ace-tomorrow-night-blue .ace_heading,\n.ace-tomorrow-night-blue .ace_markup.ace_heading,\n.ace-tomorrow-night-blue .ace_string {\n  color: #D1F1A9\n}\n\n.ace-tomorrow-night-blue .ace_entity.ace_name.ace_tag,\n.ace-tomorrow-night-blue .ace_entity.ace_other.ace_attribute-name,\n.ace-tomorrow-night-blue .ace_meta.ace_tag,\n.ace-tomorrow-night-blue .ace_string.ace_regexp,\n.ace-tomorrow-night-blue .ace_variable {\n  color: #FF9DA4\n}\n\n.ace-tomorrow-night-blue .ace_comment {\n  color: #7285B7\n}\n\n.ace-tomorrow-night-blue .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYJDzqfwPAANXAeNsiA+ZAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-tomorrow-night-blue .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/tomorrow_night_blue", ["require", "exports", "module", "ace/theme/tomorrow_night_blue.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/tomorrow_night_blue", ["require", "exports", "module", "ace/theme/tomorrow_night_blue-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-tomorrow-night-blue";
-    exports.cssText = require("./tomorrow_night_blue.css");
+    exports.cssText = require("./tomorrow_night_blue-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/tomorrow_night_blue"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-tomorrow_night_bright.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-tomorrow_night_bright.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/tomorrow_night_bright.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/tomorrow_night_bright-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-tomorrow-night-bright .ace_gutter {\n  background: #1a1a1a;\n  color: #DEDEDE\n}\n\n.ace-tomorrow-night-bright .ace_print-margin {\n  width: 1px;\n  background: #1a1a1a\n}\n\n.ace-tomorrow-night-bright {\n  background-color: #000000;\n  color: #DEDEDE\n}\n\n.ace-tomorrow-night-bright .ace_cursor {\n  color: #9F9F9F\n}\n\n.ace-tomorrow-night-bright .ace_marker-layer .ace_selection {\n  background: #424242\n}\n\n.ace-tomorrow-night-bright.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #000000;\n}\n\n.ace-tomorrow-night-bright .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-tomorrow-night-bright .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #888888\n}\n\n.ace-tomorrow-night-bright .ace_marker-layer .ace_highlight {\n  border: 1px solid rgb(110, 119, 0);\n  border-bottom: 0;\n  box-shadow: inset 0 -1px rgb(110, 119, 0);\n  margin: -1px 0 0 -1px;\n  background: rgba(255, 235, 0, 0.1)\n}\n\n.ace-tomorrow-night-bright .ace_marker-layer .ace_active-line {\n  background: #2A2A2A\n}\n\n.ace-tomorrow-night-bright .ace_gutter-active-line {\n  background-color: #2A2A2A\n}\n\n.ace-tomorrow-night-bright .ace_stack {\n  background-color: rgb(66, 90, 44)\n}\n\n.ace-tomorrow-night-bright .ace_marker-layer .ace_selected-word {\n  border: 1px solid #888888\n}\n\n.ace-tomorrow-night-bright .ace_invisible {\n  color: #343434\n}\n\n.ace-tomorrow-night-bright .ace_keyword,\n.ace-tomorrow-night-bright .ace_meta,\n.ace-tomorrow-night-bright .ace_storage,\n.ace-tomorrow-night-bright .ace_storage.ace_type,\n.ace-tomorrow-night-bright .ace_support.ace_type {\n  color: #C397D8\n}\n\n.ace-tomorrow-night-bright .ace_keyword.ace_operator {\n  color: #70C0B1\n}\n\n.ace-tomorrow-night-bright .ace_constant.ace_character,\n.ace-tomorrow-night-bright .ace_constant.ace_language,\n.ace-tomorrow-night-bright .ace_constant.ace_numeric,\n.ace-tomorrow-night-bright .ace_keyword.ace_other.ace_unit,\n.ace-tomorrow-night-bright .ace_support.ace_constant,\n.ace-tomorrow-night-bright .ace_variable.ace_parameter {\n  color: #E78C45\n}\n\n.ace-tomorrow-night-bright .ace_constant.ace_other {\n  color: #EEEEEE\n}\n\n.ace-tomorrow-night-bright .ace_invalid {\n  color: #CED2CF;\n  background-color: #DF5F5F\n}\n\n.ace-tomorrow-night-bright .ace_invalid.ace_deprecated {\n  color: #CED2CF;\n  background-color: #B798BF\n}\n\n.ace-tomorrow-night-bright .ace_fold {\n  background-color: #7AA6DA;\n  border-color: #DEDEDE\n}\n\n.ace-tomorrow-night-bright .ace_entity.ace_name.ace_function,\n.ace-tomorrow-night-bright .ace_support.ace_function,\n.ace-tomorrow-night-bright .ace_variable {\n  color: #7AA6DA\n}\n\n.ace-tomorrow-night-bright .ace_support.ace_class,\n.ace-tomorrow-night-bright .ace_support.ace_type {\n  color: #E7C547\n}\n\n.ace-tomorrow-night-bright .ace_heading,\n.ace-tomorrow-night-bright .ace_markup.ace_heading,\n.ace-tomorrow-night-bright .ace_string {\n  color: #B9CA4A\n}\n\n.ace-tomorrow-night-bright .ace_entity.ace_name.ace_tag,\n.ace-tomorrow-night-bright .ace_entity.ace_other.ace_attribute-name,\n.ace-tomorrow-night-bright .ace_meta.ace_tag,\n.ace-tomorrow-night-bright .ace_string.ace_regexp,\n.ace-tomorrow-night-bright .ace_variable {\n  color: #D54E53\n}\n\n.ace-tomorrow-night-bright .ace_comment {\n  color: #969896\n}\n\n.ace-tomorrow-night-bright .ace_c9searchresults.ace_keyword {\n  color: #C2C280\n}\n\n.ace-tomorrow-night-bright .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYFBXV/8PAAJoAXX4kT2EAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-tomorrow-night-bright .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/tomorrow_night_bright", ["require", "exports", "module", "ace/theme/tomorrow_night_bright.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/tomorrow_night_bright", ["require", "exports", "module", "ace/theme/tomorrow_night_bright-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-tomorrow-night-bright";
-    exports.cssText = require("./tomorrow_night_bright.css");
+    exports.cssText = require("./tomorrow_night_bright-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/tomorrow_night_bright"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-tomorrow_night_eighties.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-tomorrow_night_eighties.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/tomorrow_night_eighties.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/tomorrow_night_eighties-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-tomorrow-night-eighties .ace_gutter {\n  background: #272727;\n  color: #CCC\n}\n\n.ace-tomorrow-night-eighties .ace_print-margin {\n  width: 1px;\n  background: #272727\n}\n\n.ace-tomorrow-night-eighties {\n  background-color: #2D2D2D;\n  color: #CCCCCC\n}\n\n.ace-tomorrow-night-eighties .ace_constant.ace_other,\n.ace-tomorrow-night-eighties .ace_cursor {\n  color: #CCCCCC\n}\n\n.ace-tomorrow-night-eighties .ace_marker-layer .ace_selection {\n  background: #515151\n}\n\n.ace-tomorrow-night-eighties.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #2D2D2D;\n}\n\n.ace-tomorrow-night-eighties .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-tomorrow-night-eighties .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #6A6A6A\n}\n\n.ace-tomorrow-night-bright .ace_stack {\n  background: rgb(66, 90, 44)\n}\n\n.ace-tomorrow-night-eighties .ace_marker-layer .ace_active-line {\n  background: #393939\n}\n\n.ace-tomorrow-night-eighties .ace_gutter-active-line {\n  background-color: #393939\n}\n\n.ace-tomorrow-night-eighties .ace_marker-layer .ace_selected-word {\n  border: 1px solid #515151\n}\n\n.ace-tomorrow-night-eighties .ace_invisible {\n  color: #6A6A6A\n}\n\n.ace-tomorrow-night-eighties .ace_keyword,\n.ace-tomorrow-night-eighties .ace_meta,\n.ace-tomorrow-night-eighties .ace_storage,\n.ace-tomorrow-night-eighties .ace_storage.ace_type,\n.ace-tomorrow-night-eighties .ace_support.ace_type {\n  color: #CC99CC\n}\n\n.ace-tomorrow-night-eighties .ace_keyword.ace_operator {\n  color: #66CCCC\n}\n\n.ace-tomorrow-night-eighties .ace_constant.ace_character,\n.ace-tomorrow-night-eighties .ace_constant.ace_language,\n.ace-tomorrow-night-eighties .ace_constant.ace_numeric,\n.ace-tomorrow-night-eighties .ace_keyword.ace_other.ace_unit,\n.ace-tomorrow-night-eighties .ace_support.ace_constant,\n.ace-tomorrow-night-eighties .ace_variable.ace_parameter {\n  color: #F99157\n}\n\n.ace-tomorrow-night-eighties .ace_invalid {\n  color: #CDCDCD;\n  background-color: #F2777A\n}\n\n.ace-tomorrow-night-eighties .ace_invalid.ace_deprecated {\n  color: #CDCDCD;\n  background-color: #CC99CC\n}\n\n.ace-tomorrow-night-eighties .ace_fold {\n  background-color: #6699CC;\n  border-color: #CCCCCC\n}\n\n.ace-tomorrow-night-eighties .ace_entity.ace_name.ace_function,\n.ace-tomorrow-night-eighties .ace_support.ace_function,\n.ace-tomorrow-night-eighties .ace_variable {\n  color: #6699CC\n}\n\n.ace-tomorrow-night-eighties .ace_support.ace_class,\n.ace-tomorrow-night-eighties .ace_support.ace_type {\n  color: #FFCC66\n}\n\n.ace-tomorrow-night-eighties .ace_heading,\n.ace-tomorrow-night-eighties .ace_markup.ace_heading,\n.ace-tomorrow-night-eighties .ace_string {\n  color: #99CC99\n}\n\n.ace-tomorrow-night-eighties .ace_comment {\n  color: #999999\n}\n\n.ace-tomorrow-night-eighties .ace_entity.ace_name.ace_tag,\n.ace-tomorrow-night-eighties .ace_entity.ace_other.ace_attribute-name,\n.ace-tomorrow-night-eighties .ace_meta.ace_tag,\n.ace-tomorrow-night-eighties .ace_variable {\n  color: #F2777A\n}\n\n.ace-tomorrow-night-eighties .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWPQ09NrYAgMjP4PAAtGAwchHMyAAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-tomorrow-night-eighties .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/tomorrow_night_eighties", ["require", "exports", "module", "ace/theme/tomorrow_night_eighties.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/tomorrow_night_eighties", ["require", "exports", "module", "ace/theme/tomorrow_night_eighties-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-tomorrow-night-eighties";
-    exports.cssText = require("./tomorrow_night_eighties.css");
+    exports.cssText = require("./tomorrow_night_eighties-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/tomorrow_night_eighties"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-twilight.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-twilight.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/twilight.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/twilight-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-twilight .ace_gutter {\n  background: #232323;\n  color: #E2E2E2\n}\n\n.ace-twilight .ace_print-margin {\n  width: 1px;\n  background: #232323\n}\n\n.ace-twilight {\n  background-color: #141414;\n  color: #F8F8F8\n}\n\n.ace-twilight .ace_cursor {\n  color: #A7A7A7\n}\n\n.ace-twilight .ace_marker-layer .ace_selection {\n  background: rgba(221, 240, 255, 0.20)\n}\n\n.ace-twilight.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #141414;\n}\n\n.ace-twilight .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-twilight .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid rgba(255, 255, 255, 0.25)\n}\n\n.ace-twilight .ace_marker-layer .ace_active-line {\n  background: rgba(255, 255, 255, 0.031)\n}\n\n.ace-twilight .ace_gutter-active-line {\n  background-color: rgba(255, 255, 255, 0.031)\n}\n\n.ace-twilight .ace_marker-layer .ace_selected-word {\n  border: 1px solid rgba(221, 240, 255, 0.20)\n}\n\n.ace-twilight .ace_invisible {\n  color: rgba(255, 255, 255, 0.25)\n}\n\n.ace-twilight .ace_keyword,\n.ace-twilight .ace_meta {\n  color: #CDA869\n}\n\n.ace-twilight .ace_constant,\n.ace-twilight .ace_constant.ace_character,\n.ace-twilight .ace_constant.ace_character.ace_escape,\n.ace-twilight .ace_constant.ace_other,\n.ace-twilight .ace_heading,\n.ace-twilight .ace_markup.ace_heading,\n.ace-twilight .ace_support.ace_constant {\n  color: #CF6A4C\n}\n\n.ace-twilight .ace_invalid.ace_illegal {\n  color: #F8F8F8;\n  background-color: rgba(86, 45, 86, 0.75)\n}\n\n.ace-twilight .ace_invalid.ace_deprecated {\n  text-decoration: underline;\n  font-style: italic;\n  color: #D2A8A1\n}\n\n.ace-twilight .ace_support {\n  color: #9B859D\n}\n\n.ace-twilight .ace_fold {\n  background-color: #AC885B;\n  border-color: #F8F8F8\n}\n\n.ace-twilight .ace_support.ace_function {\n  color: #DAD085\n}\n\n.ace-twilight .ace_list,\n.ace-twilight .ace_markup.ace_list,\n.ace-twilight .ace_storage {\n  color: #F9EE98\n}\n\n.ace-twilight .ace_entity.ace_name.ace_function,\n.ace-twilight .ace_meta.ace_tag {\n  color: #AC885B\n}\n\n.ace-twilight .ace_string {\n  color: #8F9D6A\n}\n\n.ace-twilight .ace_string.ace_regexp {\n  color: #E9C062\n}\n\n.ace-twilight .ace_comment {\n  font-style: italic;\n  color: #5F5A60\n}\n\n.ace-twilight .ace_variable {\n  color: #7587A6\n}\n\n.ace-twilight .ace_xml-pe {\n  color: #494949\n}\n\n.ace-twilight .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWMQERFpYLC1tf0PAAgOAnPnhxyiAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-twilight .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/twilight", ["require", "exports", "module", "ace/theme/twilight.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/twilight", ["require", "exports", "module", "ace/theme/twilight-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-twilight";
-    exports.cssText = require("./twilight.css");
+    exports.cssText = require("./twilight-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/twilight"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-vibrant_ink.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-vibrant_ink.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/vibrant_ink.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/vibrant_ink-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = ".ace-vibrant-ink .ace_gutter {\n  background: #1a1a1a;\n  color: #BEBEBE\n}\n\n.ace-vibrant-ink .ace_print-margin {\n  width: 1px;\n  background: #1a1a1a\n}\n\n.ace-vibrant-ink {\n  background-color: #0F0F0F;\n  color: #FFFFFF\n}\n\n.ace-vibrant-ink .ace_cursor {\n  color: #FFFFFF\n}\n\n.ace-vibrant-ink .ace_marker-layer .ace_selection {\n  background: #6699CC\n}\n\n.ace-vibrant-ink.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #0F0F0F;\n}\n\n.ace-vibrant-ink .ace_marker-layer .ace_step {\n  background: rgb(102, 82, 0)\n}\n\n.ace-vibrant-ink .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #404040\n}\n\n.ace-vibrant-ink .ace_marker-layer .ace_active-line {\n  background: #333333\n}\n\n.ace-vibrant-ink .ace_gutter-active-line {\n  background-color: #333333\n}\n\n.ace-vibrant-ink .ace_marker-layer .ace_selected-word {\n  border: 1px solid #6699CC\n}\n\n.ace-vibrant-ink .ace_invisible {\n  color: #404040\n}\n\n.ace-vibrant-ink .ace_keyword,\n.ace-vibrant-ink .ace_meta {\n  color: #FF6600\n}\n\n.ace-vibrant-ink .ace_constant,\n.ace-vibrant-ink .ace_constant.ace_character,\n.ace-vibrant-ink .ace_constant.ace_character.ace_escape,\n.ace-vibrant-ink .ace_constant.ace_other {\n  color: #339999\n}\n\n.ace-vibrant-ink .ace_constant.ace_numeric {\n  color: #99CC99\n}\n\n.ace-vibrant-ink .ace_invalid,\n.ace-vibrant-ink .ace_invalid.ace_deprecated {\n  color: #CCFF33;\n  background-color: #000000\n}\n\n.ace-vibrant-ink .ace_fold {\n  background-color: #FFCC00;\n  border-color: #FFFFFF\n}\n\n.ace-vibrant-ink .ace_entity.ace_name.ace_function,\n.ace-vibrant-ink .ace_support.ace_function,\n.ace-vibrant-ink .ace_variable {\n  color: #FFCC00\n}\n\n.ace-vibrant-ink .ace_variable.ace_parameter {\n  font-style: italic\n}\n\n.ace-vibrant-ink .ace_string {\n  color: #66FF00\n}\n\n.ace-vibrant-ink .ace_string.ace_regexp {\n  color: #44B4CC\n}\n\n.ace-vibrant-ink .ace_comment {\n  color: #9933CC\n}\n\n.ace-vibrant-ink .ace_entity.ace_other.ace_attribute-name {\n  font-style: italic;\n  color: #99CC99\n}\n\n.ace-vibrant-ink .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQImWNgYGBgYNDTc/oPAALPAZ7hxlbYAAAAAElFTkSuQmCC) right repeat-y\n}\n\n.ace-vibrant-ink .ace_indent-guide-active {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAEklEQVQIW2PQ1dX9zzBz5sz/ABCcBFFentLlAAAAAElFTkSuQmCC) right repeat-y;\n}\n";
 
 });
 
-define("ace/theme/vibrant_ink", ["require", "exports", "module", "ace/theme/vibrant_ink.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/vibrant_ink", ["require", "exports", "module", "ace/theme/vibrant_ink-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = true;
     exports.cssClass = "ace-vibrant-ink";
-    exports.cssText = require("./vibrant_ink.css");
+    exports.cssText = require("./vibrant_ink-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/vibrant_ink"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/theme-xcode.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/theme-xcode.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
-define("ace/theme/xcode.css", ["require", "exports", "module"], function(require, exports, module) {
+define("ace/theme/xcode-css", ["require", "exports", "module"], function(require, exports, module) {
     module.exports = "/* THIS THEME WAS AUTOGENERATED BY Theme.tmpl.css (UUID: EE3AD170-2B7F-4DE1-B724-C75F13FE0085) */\n\n.ace-xcode .ace_gutter {\n  background: #e8e8e8;\n  color: #333\n}\n\n.ace-xcode .ace_print-margin {\n  width: 1px;\n  background: #e8e8e8\n}\n\n.ace-xcode {\n  background-color: #FFFFFF;\n  color: #000000\n}\n\n.ace-xcode .ace_cursor {\n  color: #000000\n}\n\n.ace-xcode .ace_marker-layer .ace_selection {\n  background: #B5D5FF\n}\n\n.ace-xcode.ace_multiselect .ace_selection.ace_start {\n  box-shadow: 0 0 3px 0px #FFFFFF;\n}\n\n.ace-xcode .ace_marker-layer .ace_step {\n  background: rgb(198, 219, 174)\n}\n\n.ace-xcode .ace_marker-layer .ace_bracket {\n  margin: -1px 0 0 -1px;\n  border: 1px solid #BFBFBF\n}\n\n.ace-xcode .ace_marker-layer .ace_active-line {\n  background: rgba(0, 0, 0, 0.071)\n}\n\n.ace-xcode .ace_gutter-active-line {\n  background-color: rgba(0, 0, 0, 0.071)\n}\n\n.ace-xcode .ace_marker-layer .ace_selected-word {\n  border: 1px solid #B5D5FF\n}\n\n.ace-xcode .ace_constant.ace_language,\n.ace-xcode .ace_keyword,\n.ace-xcode .ace_meta,\n.ace-xcode .ace_variable.ace_language {\n  color: #C800A4\n}\n\n.ace-xcode .ace_invisible {\n  color: #BFBFBF\n}\n\n.ace-xcode .ace_constant.ace_character,\n.ace-xcode .ace_constant.ace_other {\n  color: #275A5E\n}\n\n.ace-xcode .ace_constant.ace_numeric {\n  color: #3A00DC\n}\n\n.ace-xcode .ace_entity.ace_other.ace_attribute-name,\n.ace-xcode .ace_support.ace_constant,\n.ace-xcode .ace_support.ace_function {\n  color: #450084\n}\n\n.ace-xcode .ace_fold {\n  background-color: #C800A4;\n  border-color: #000000\n}\n\n.ace-xcode .ace_entity.ace_name.ace_tag,\n.ace-xcode .ace_support.ace_class,\n.ace-xcode .ace_support.ace_type {\n  color: #790EAD\n}\n\n.ace-xcode .ace_storage {\n  color: #C900A4\n}\n\n.ace-xcode .ace_string {\n  color: #DF0002\n}\n\n.ace-xcode .ace_comment {\n  color: #008E00\n}\n\n.ace-xcode .ace_indent-guide {\n  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAAE0lEQVQImWP4////f4bLly//BwAmVgd1/w11/gAAAABJRU5ErkJggg==) right repeat-y\n}\n\n.ace-xcode .ace_indent-guide-active {\n  background: url(\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAACCAYAAACZgbYnAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAIGNIUk0AAHolAACAgwAA+f8AAIDpAAB1MAAA6mAAADqYAAAXb5JfxUYAAAAZSURBVHjaYvj///9/hivKyv8BAAAA//8DACLqBhbvk+/eAAAAAElFTkSuQmCC\") right repeat-y;\n} \n";
 
 });
 
-define("ace/theme/xcode", ["require", "exports", "module", "ace/theme/xcode.css", "ace/lib/dom"], function(require, exports, module) {
+define("ace/theme/xcode", ["require", "exports", "module", "ace/theme/xcode-css", "ace/lib/dom"], function(require, exports, module) {
     exports.isDark = false;
     exports.cssClass = "ace-xcode";
-    exports.cssText = require("./xcode.css");
+    exports.cssText = require("./xcode-css");
     var dom = require("../lib/dom");
     dom.importCssString(exports.cssText, exports.cssClass, false);
 
 });
 (function() {
     window.require(["ace/theme/xcode"], function(m) {
         if (typeof module == "object" && typeof exports == "object" && module) {
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/worker-base.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/worker-base.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/worker-coffee.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/worker-coffee.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/worker-css.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/worker-css.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/worker-html.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/worker-html.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/worker-javascript.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/worker-javascript.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2493,15 +2493,15 @@
                                 var exports = global._ = factory();
                                 exports.noConflict = function() {
                                     global._ = current;
                                     return exports;
                                 };
                             }()));
                     }(this, (function() {
-                        var VERSION = '1.13.4';
+                        var VERSION = '1.13.6';
                         var root = (typeof self == 'object' && self.self === self && self) ||
                             (typeof global == 'object' && global.global === global && global) ||
                             Function('return this')() || {};
                         var ArrayProto = Array.prototype,
                             ObjProto = Object.prototype;
                         var SymbolProto = typeof Symbol !== 'undefined' ? Symbol.prototype : null;
                         var push = ArrayProto.push,
@@ -7810,15 +7810,15 @@
                                 advance("=");
                                 if (!noin && peek(0).id === "=" && state.tokens.next.identifier) {
                                     warning("W120", state.tokens.next, state.tokens.next.value);
                                 }
                                 var id = state.tokens.prev;
                                 value = expression(context, 10);
                                 if (value) {
-                                    if (value.identifier && value.value === "undefined") {
+                                    if (!isConst && value.identifier && value.value === "undefined") {
                                         warning("W080", id, id.value);
                                     }
                                     if (!lone) {
                                         destructuringPatternMatch(names, value);
                                     }
                                 }
                             }
@@ -11891,15 +11891,15 @@
                     E005: "Input is empty.",
                     E006: "Unexpected early end of program.",
                     E007: "Missing \"use strict\" statement.",
                     E008: "Strict violation.",
                     E009: "Option 'validthis' can't be used in a global scope.",
                     E010: "'with' is not allowed in strict mode.",
                     E011: "'{a}' has already been declared.",
-                    E012: "const '{a}' is initialized to 'undefined'.",
+                    E012: "Missing initializer for constant '{a}'.",
                     E013: "Attempting to override '{a}' which is a constant.",
                     E014: "A regular expression literal can be confused with '/='.",
                     E015: "Unclosed regular expression.",
                     E016: "Invalid regular expression.",
                     E017: "Unclosed comment.",
                     E018: "Unbegun comment.",
                     E019: "Unmatched '{a}'.",
@@ -15967,15 +15967,15 @@
     };
 
     oop.inherits(JavaScriptWorker, Mirror);
 
     (function() {
         this.setOptions = function(options) {
             this.options = options || {
-                esnext: true,
+                esversion: 11,
                 moz: true,
                 devel: true,
                 browser: true,
                 node: true,
                 laxcomma: true,
                 laxbreak: true,
                 lastsemic: true,
```

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/worker-json.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/worker-json.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/worker-lua.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/worker-lua.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/worker-php.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/worker-php.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/worker-xml.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/worker-xml.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/worker-xquery.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/worker-xquery.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/ace/worker-yaml.js` & `django-ace-1.23.4/django_ace/static/django_ace/ace/worker-yaml.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/widget.css` & `django-ace-1.23.4/django_ace/static/django_ace/widget.css`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/static/django_ace/widget.js` & `django-ace-1.23.4/django_ace/static/django_ace/widget.js`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace/widgets.py` & `django-ace-1.23.4/django_ace/widgets.py`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/django_ace.egg-info/PKG-INFO` & `django-ace-1.23.4/django_ace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ace
-Version: 1.22.1
+Version: 1.23.4
 Summary: django-ace provides integration for ajax.org ACE with Django
 Home-page: https://github.com/django-ace/django-ace
 Author: Bradley Ayers
 Author-email: bradley.ayers@gmail.com
 License: Simplified BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -95,14 +95,19 @@
 
 Then browser to ``http://localhost:8000``.
 
 
 Change log
 ==========
 
+v1.23.4
+-------
+
+- Update ACE editor to version v1.23.4.
+
 v1.22.1
 -------
 
 - Update ACE editor to version v1.22.1.
 
 v1.19.0
 -------
```

### Comparing `django-ace-1.22.1/django_ace.egg-info/SOURCES.txt` & `django-ace-1.23.4/django_ace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ace-1.22.1/setup.cfg` & `django-ace-1.23.4/setup.cfg`

 * *Files identical despite different names*

