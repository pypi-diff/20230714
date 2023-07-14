# Comparing `tmp/cruiz-1.4.0a2.tar.gz` & `tmp/cruiz-1.4.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cruiz-1.4.0a2.tar", last modified: Thu Jun 29 07:29:31 2023, max compression
+gzip compressed data, was "cruiz-1.4.0a3.tar", last modified: Fri Jul 14 13:46:18 2023, max compression
```

## Comparing `cruiz-1.4.0a2.tar` & `cruiz-1.4.0a3.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.092252 cruiz-1.4.0a2/cruiz/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz/RELEASE_VERSION.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1828 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.092252 cruiz-1.4.0a2/cruiz/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/conanconf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/conanenv.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6322 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/conaninvocation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25565 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/context.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/guardedlisttoflush.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2401 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/logdetails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4189 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/messagereplyprocessor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5555 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/commands/metarequestconaninvocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/dumpobjecttypes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3770 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/interop/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/commandparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/commonparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/packagebinaryparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/packageidparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/packagenode.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/packagerevisionsparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/reciperevisionsparameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/interop/searchrecipesparameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/load_recipe/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/loadrecipewizard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/load_recipe/pages/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/pages/initialprofilepage.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/pages/intropage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/pages/localcachepage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/load_recipe/pages/packageversionpage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28296 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/mainwindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/manage_local_cache/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36004 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/managelocalcachesdialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/addenvironmentdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2425 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2570 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/addremotedialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/configpathorurl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3712 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/installconfigdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/keyvaluetable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8370 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/movelocalcachedialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7548 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/newlocalcachewizard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1683 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/progressdialogs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4933 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/remotestable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2239 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/runconancommanddialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/model/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/model/conanpackagetypeflags.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2494 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/model/graphaslistmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.096252 cruiz-1.4.0a2/cruiz/pyside6/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/pyside6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.100252 cruiz-1.4.0a2/cruiz/recipe/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/dependencyview.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1206 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/expressioneditordialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1586 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/findtextdialog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.100252 cruiz-1.4.0a2/cruiz/recipe/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/logs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6022 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/logs/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2234 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/recipe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59849 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/recipewidget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.100252 cruiz-1.4.0a2/cruiz/recipe/toolbars/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/toolbars/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6621 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/toolbars/behaviour.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9887 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/toolbars/buildfeatures.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32749 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/recipe/toolbars/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.100252 cruiz-1.4.0a2/cruiz/remote_browser/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.100252 cruiz-1.4.0a2/cruiz/remote_browser/pages/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/packagebinarypage.py
--rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/packageidpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/packagereferencepage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/packagerevisionpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/pages/reciperevisionpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/remote_browser/remotebrowser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resourcegeneration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.104252 cruiz-1.4.0a2/cruiz/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/001-rubbish.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/002-null.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/003-chemistry.svg
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/004-share.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/005-box.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/006-toolbox.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/007-book.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/008-cloud-computing.svg
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/009-import.svg
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/010-draw.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/012-hammer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/013-pencil.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/014-code.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/Cmake.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/about_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/cruise.png
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/cruizres.qrc
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/find_text_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    53573 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/license-cruise.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    96863 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/license.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/load_recipe_wizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_add_environment.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_add_profile_directory.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_add_remote.ui
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_install_config.ui
--rw-r--r--   0 runner    (1001) docker     (123)    27112 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_manage.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_move.ui
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_new_wizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_remove_environment.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/local_cache_run_command_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)    41069 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/preferences.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_cmake_features_frame.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_compilercache_features_frame.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_cpucores_frame.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_local_workflow_expression_editor.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_profile_frame.ui
--rw-r--r--   0 runner    (1001) docker     (123)    33767 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/recipe_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)    28688 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/remote_browser.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/resources/remote_browser_fileview.ui
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/revealonfilesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.104252 cruiz-1.4.0a2/cruiz/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      582 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/ensuredefaultlocalcache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/cruiz/settings/managers/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10185 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/basesettings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4871 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/cleansettings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1728 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/cmakepreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3244 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/compilercachepreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2499 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/conanpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2309 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/fontpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/generalpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1890 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/graphvizpreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3903 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/localcachepreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14295 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/namedlocalcache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1830 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/ninjapreferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3681 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/recentconanconfigs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3590 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/recentconanremotes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/recentrecipes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18314 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/recipe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/restoredefaults.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7928 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/shortcuts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/valueclasses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4187 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/managers/writermixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/cruiz/settings/models/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1419 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/models/recentconanconfigmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/models/recentconanremotesmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2727 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/models/recipesmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54673 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/preferencesdialog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14331 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/settings/updatesettings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5848 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/svggraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/cruiz/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/widgets/aboutcruizdialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/widgets/debugging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1387 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/widgets/shortcutlineedit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2050 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/widgets/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/cruiz/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/cruiz/workers/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/cruiz/workers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/colorarma_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/formatoptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/qtlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/text2html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/cruiz/workers/utils/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:29:31.092252 cruiz-1.4.0a2/cruiz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 07:29:31.000000 cruiz-1.4.0a2/cruiz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 07:29:31.108252 cruiz-1.4.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-29 07:29:13.000000 cruiz-1.4.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.449237 cruiz-1.4.0a3/cruiz/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz/RELEASE_VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1828 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.453237 cruiz-1.4.0a3/cruiz/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/conanconf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/conanenv.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6322 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/conaninvocation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25561 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/guardedlisttoflush.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2401 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/logdetails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4189 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/messagereplyprocessor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5555 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/commands/metarequestconaninvocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/dumpobjecttypes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3770 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.453237 cruiz-1.4.0a3/cruiz/interop/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17403 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/commandparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/commonparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/packagebinaryparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/packageidparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/packagenode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/packagerevisionsparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/reciperevisionsparameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/interop/searchrecipesparameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.453237 cruiz-1.4.0a3/cruiz/load_recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/loadrecipewizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.457237 cruiz-1.4.0a3/cruiz/load_recipe/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/pages/initialprofilepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/pages/intropage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/pages/localcachepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/load_recipe/pages/packageversionpage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28296 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/mainwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.457237 cruiz-1.4.0a3/cruiz/manage_local_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36004 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/managelocalcachesdialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.461237 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2465 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/addenvironmentdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2425 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2525 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/addremotedialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      950 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/configpathorurl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3684 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/installconfigdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/keyvaluetable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8370 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/movelocalcachedialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7548 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/newlocalcachewizard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1683 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/progressdialogs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4933 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/remotestable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2239 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/runconancommanddialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.461237 cruiz-1.4.0a3/cruiz/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/model/conanpackagetypeflags.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2494 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/model/graphaslistmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.461237 cruiz-1.4.0a3/cruiz/pyside6/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/pyside6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.465237 cruiz-1.4.0a3/cruiz/recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/dependencyview.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1206 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/expressioneditordialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1586 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/findtextdialog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.465237 cruiz-1.4.0a3/cruiz/recipe/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/logs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6022 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/logs/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2234 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/recipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61387 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/recipewidget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.465237 cruiz-1.4.0a3/cruiz/recipe/toolbars/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/toolbars/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6621 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/toolbars/behaviour.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9887 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/toolbars/buildfeatures.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33104 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/recipe/toolbars/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.465237 cruiz-1.4.0a3/cruiz/remote_browser/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.469237 cruiz-1.4.0a3/cruiz/remote_browser/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/packagebinarypage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/packageidpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/packagereferencepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/packagerevisionpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/pages/reciperevisionpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/remote_browser/remotebrowser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resourcegeneration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.477237 cruiz-1.4.0a3/cruiz/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/001-rubbish.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/002-null.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/003-chemistry.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/004-share.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/005-box.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/006-toolbox.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/007-book.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/008-cloud-computing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/009-import.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/010-draw.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/012-hammer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/013-pencil.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/014-code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/Cmake.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/about_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/cruise.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/cruizres.qrc
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/find_text_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    53573 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/license-cruise.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    96863 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/license.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/load_recipe_wizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_add_environment.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_add_profile_directory.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_add_remote.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_install_config.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    27112 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_manage.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_move.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_new_wizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_remove_environment.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/local_cache_run_command_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    41069 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/preferences.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_cmake_features_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_compilercache_features_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_cpucores_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_local_workflow_expression_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_profile_frame.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    34335 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/recipe_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    28688 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/remote_browser.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/resources/remote_browser_fileview.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/revealonfilesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.481238 cruiz-1.4.0a3/cruiz/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      582 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/ensuredefaultlocalcache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.485237 cruiz-1.4.0a3/cruiz/settings/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10185 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/basesettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4871 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/cleansettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1728 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/cmakepreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3244 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/compilercachepreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2499 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/conanpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2309 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/fontpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6803 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/generalpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1890 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/graphvizpreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3903 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/localcachepreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14295 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/namedlocalcache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1830 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/ninjapreferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3681 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/recentconanconfigs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3590 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/recentconanremotes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/recentrecipes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18314 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/recipe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/restoredefaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7928 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/shortcuts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1149 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/valueclasses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4187 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/managers/writermixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.485237 cruiz-1.4.0a3/cruiz/settings/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1419 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/models/recentconanconfigmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1345 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/models/recentconanremotesmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2727 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/models/recipesmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54673 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/preferencesdialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14331 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/settings/updatesettings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5848 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/svggraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/cruiz/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/widgets/aboutcruizdialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/widgets/debugging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1387 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/widgets/shortcutlineedit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2050 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/widgets/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/cruiz/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/cruiz/workers/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/cruiz/workers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/colorarma_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/formatoptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/qtlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/text2html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/cruiz/workers/utils/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:46:18.449237 cruiz-1.4.0a3/cruiz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 13:46:18.000000 cruiz-1.4.0a3/cruiz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 13:46:18.489237 cruiz-1.4.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-14 13:45:58.000000 cruiz-1.4.0a3/setup.py
```

### Comparing `cruiz-1.4.0a2/LICENSE` & `cruiz-1.4.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/PKG-INFO` & `cruiz-1.4.0a3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: cruiz
-Version: 1.4.0a2
+Version: 1.4.0a3
 Summary: Conan recipe user interface
 Home-page: https://github.com/markfinal/cruiz
 Author: Mark Final
 Author-email: markfinal@hotmail.com
 Project-URL: Documentation, https://cruiz.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/markfinal/cruiz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7, <3.12
+Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # cruiz
 
 Conan recipe user interface
@@ -37,15 +36,15 @@
 
 - Intel x86_64 platforms:
   - Windows 10+
   - Linux (CentOS 7.5+/Ubuntu 18+)
   - macOS (11.0+)
 - Apple Silicon platforms:
   - macOS (11.0+)
-- Python 3.7-3.11
+- Python 3.8-3.11
 - Conan 1.x (from 1.17.1 onwards) and 2.x (from 2.0.7 onwards)
 
 All other Python dependencies are installed when the package is installed.
 
 In order to use the dependency graph visualisation, an additional installation of GraphViz is required from https://graphviz.org/download/. Assign the installed location to the preferences.
 
 ## Conan versions
```

### Comparing `cruiz-1.4.0a2/README.md` & `cruiz-1.4.0a3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 - Intel x86_64 platforms:
   - Windows 10+
   - Linux (CentOS 7.5+/Ubuntu 18+)
   - macOS (11.0+)
 - Apple Silicon platforms:
   - macOS (11.0+)
-- Python 3.7-3.11
+- Python 3.8-3.11
 - Conan 1.x (from 1.17.1 onwards) and 2.x (from 2.0.7 onwards)
 
 All other Python dependencies are installed when the package is installed.
 
 In order to use the dependency graph visualisation, an additional installation of GraphViz is required from https://graphviz.org/download/. Assign the installed location to the preferences.
 
 ## Conan versions
```

### Comparing `cruiz-1.4.0a2/cruiz/application.py` & `cruiz-1.4.0a3/cruiz/application.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/commands/conanenv.py` & `cruiz-1.4.0a3/cruiz/commands/conanenv.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/commands/conaninvocation.py` & `cruiz-1.4.0a3/cruiz/commands/conaninvocation.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/commands/context.py` & `cruiz-1.4.0a3/cruiz/commands/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -598,15 +598,15 @@
         conandata, exception = self._meta_invocation.request_data(
             "get_conandata", {"path": recipe_path}
         )
         if exception:
             if self.parent():
                 self.parent().record_exception(exception)
             else:
-                raise Exception(
+                raise ValueError(
                     "Failed to get conandata YAML dict for recipe"
                 ) from exception
         return conandata
 
     def get_boolean_config(
         self, config: ConanConfigBoolean, default_value: bool
     ) -> bool:
@@ -648,17 +648,17 @@
     @property
     def is_default(self) -> bool:
         """
         Does this context refer to the 'default' local cache?
         """
         return self.cache_name == DEFAULT_CACHE_NAME
 
-    def get_conan_config_environment_variables(self) -> typing.Dict[str, str]:
+    def get_conan_config_environment_variables(self) -> typing.List[str]:
         """
-        Get a dictionary of all Conan environment variables.
+        Get a list of all Conan environment variables names.
         This doesn't get all of them, but at least some.
         """
         envvars, exception = self._meta_invocation.request_data("get_config_envvars")
         if exception:
             if self.parent():
                 self.parent().record_exception(exception)
             else:
```

### Comparing `cruiz-1.4.0a2/cruiz/commands/guardedlisttoflush.py` & `cruiz-1.4.0a3/cruiz/commands/guardedlisttoflush.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/commands/logdetails.py` & `cruiz-1.4.0a3/cruiz/commands/logdetails.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/commands/messagereplyprocessor.py` & `cruiz-1.4.0a3/cruiz/commands/messagereplyprocessor.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/commands/metarequestconaninvocation.py` & `cruiz-1.4.0a3/cruiz/commands/metarequestconaninvocation.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/constants.py` & `cruiz-1.4.0a3/cruiz/constants.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/dumpobjecttypes.py` & `cruiz-1.4.0a3/cruiz/dumpobjecttypes.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/entrypoint.py` & `cruiz-1.4.0a3/cruiz/entrypoint.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/environ.py` & `cruiz-1.4.0a3/cruiz/environ.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/exceptions.py` & `cruiz-1.4.0a3/cruiz/exceptions.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/globals.py` & `cruiz-1.4.0a3/cruiz/globals.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/interop/commandparameters.py` & `cruiz-1.4.0a3/cruiz/interop/commandparameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         self._force: typing.Optional[bool] = None
         self._package_reference: typing.Optional[str] = None
         self._args: typing.List[str] = []
         self._named_args: typing.Dict[str, str] = {}
         self._time_commands: typing.Optional[bool] = None
         self._v2_omit_test_folder: typing.Optional[bool] = None
         self._v2_needs_reference: typing.Optional[bool] = None
+        self._extra_options: typing.Optional[str] = None
 
     def to_args(self) -> typing.List[str]:
         """
         Get the argument list corresponding to these command parameters.
         """
         components = [self.verb]
         if self._profile:
@@ -396,20 +397,26 @@
     @property
     def options(self) -> typing.Dict[str, str]:  # TODO: should this be immutable?
         """
         Get the recipe options.
         """
         return self._options
 
-    def add_option(self, package_name: str, key: str, value: str) -> None:
+    def add_option(
+        self, package_name: typing.Optional[str], key: str, value: str
+    ) -> None:
         """
         Add an option key-value pair.
+        If package_name is provided, the option key is prefixed with package_name:
         """
         assert key not in self._options
-        self._options[f"{package_name}:{key}"] = value
+        if package_name:
+            self._options[f"{package_name}:{key}"] = value
+        else:
+            self._options[key] = value
 
     @property
     def force(self) -> typing.Optional[bool]:
         """
         Get whether an option is forced.
         May be None.
         """
@@ -496,7 +503,19 @@
         Conan v2+
         """
         return self._v2_needs_reference
 
     @v2_need_reference.setter
     def v2_need_reference(self, value: typing.Optional[bool]) -> None:
         self._v2_needs_reference = value
+
+    @property
+    def extra_options(self) -> typing.Optional[str]:
+        """
+        Get the extra options string.
+        May be None.
+        """
+        return self._extra_options
+
+    @extra_options.setter
+    def extra_options(self, value: typing.Optional[str]) -> None:
+        self._extra_options = value
```

### Comparing `cruiz-1.4.0a2/cruiz/interop/dependencygraph.py` & `cruiz-1.4.0a3/cruiz/interop/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/interop/message.py` & `cruiz-1.4.0a3/cruiz/interop/message.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/interop/packagenode.py` & `cruiz-1.4.0a3/cruiz/interop/packagenode.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/interop/pod.py` & `cruiz-1.4.0a3/cruiz/interop/pod.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/interop/reciperevisionsparameters.py` & `cruiz-1.4.0a3/cruiz/interop/reciperevisionsparameters.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/interop/searchrecipesparameters.py` & `cruiz-1.4.0a3/cruiz/interop/searchrecipesparameters.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/load_recipe/loadrecipewizard.py` & `cruiz-1.4.0a3/cruiz/load_recipe/loadrecipewizard.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,20 @@
 
         if self.disambiguation_required:
             self.ui.intro_message.hide()
             log_details = LogDetails(self.ui.intro_message, None, True, False, None)
             log_details.logging.connect(self._on_error_loading)
             with managed_conan_context(DEFAULT_CACHE_NAME, log_details) as context:
                 self.recipe_attributes = context.inspect_recipe(self._path)
-                self.conandata = context.get_conandata(self._path)
+                try:
+                    self.conandata = context.get_conandata(self._path)
+                except ValueError:
+                    log_details.stderr(
+                        "Unable to obtain version numbers from conandata.yml"
+                    )
 
     def _on_error_loading(self) -> None:
         self.ui.intro_message.show()
         self.has_load_errors = True
 
     @property
     def disambiguation_required(self) -> bool:
```

### Comparing `cruiz-1.4.0a2/cruiz/load_recipe/pages/initialprofilepage.py` & `cruiz-1.4.0a3/cruiz/load_recipe/pages/initialprofilepage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/load_recipe/pages/localcachepage.py` & `cruiz-1.4.0a3/cruiz/load_recipe/pages/localcachepage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/load_recipe/pages/packageversionpage.py` & `cruiz-1.4.0a3/cruiz/load_recipe/pages/packageversionpage.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,73 +30,81 @@
         return 2
 
     def initializePage(self) -> None:
         self.registerField("version*", self._ui.version, "currentText")  # type: ignore
 
         self._ui.version.currentTextChanged.connect(self._on_version_changed)
 
-        self._uuid_versions = {}
-        if self.wizard().recipe_attributes["version"] is None:
-            # get versions from conandata.yml
-            versions = self._get_versions_from_conandata(self.wizard().conandata)
-            if versions:
-                # get the versions from uuids with the same paths
-                for uuid in self.wizard().matching_uuids:
-                    with RecipeSettingsReader.from_uuid(uuid) as settings:
-                        attributes = settings.attribute_overrides.resolve()
-                    if "version" in attributes:
-                        self._uuid_versions[attributes["version"]] = uuid
-
-                with BlockSignals(self._ui.version) as blocked_widget:
-                    blocked_widget.clear()
-                    model = blocked_widget.model()
-                    for i, version in enumerate(versions):
-                        if version in self._uuid_versions:
-                            blocked_widget.addItem(QtGui.QIcon(":/cruiz.png"), version)
-                            if cruiz.globals.get_main_window().is_recipe_active(
-                                self._uuid_versions[version]
-                            ):
-                                item = model.item(i)
-                                item.setFlags(item.flags() & ~QtGui.Qt.ItemIsEnabled)
-                        else:
-                            blocked_widget.addItem(version)
-                    blocked_widget.setCurrentIndex(-1)
-        else:
-            with BlockSignals(self._ui.version) as blocked_widget:
-                blocked_widget.clear()
-                blocked_widget.addItem(self.wizard().recipe_attributes["version"])
-            # combobox disabled to ensure it's clear that there's no choice
-            self._ui.version.setEnabled(False)
+        self._uuid_versions: typing.Dict[str, str] = {}
+        self._resolve_ui_to_possible_versions()
         super().initializePage()
 
     def cleanupPage(self) -> None:
         self._ui.version.currentTextChanged.disconnect()
         return super().cleanupPage()
 
     def _on_version_changed(self, text: str) -> None:
         if text in self._uuid_versions:
             self.setFinalPage(True)
             self.wizard().uuid = self._uuid_versions[text]
         else:
             self.wizard().uuid = None
         self.completeChanged.emit()
 
+    def _resolve_ui_to_possible_versions(self) -> None:
+        self._ui.version.setEditable(False)
+        version_in_recipe = self.wizard().recipe_attributes.get("version")
+        if version_in_recipe is None:
+            # get versions from conandata.yml
+            conandata = self.wizard().conandata
+            if conandata:
+                versions = self._get_versions_from_conandata(conandata)
+                if versions:
+                    # get the versions from uuids with the same paths
+                    for uuid in self.wizard().matching_uuids:
+                        with RecipeSettingsReader.from_uuid(uuid) as settings:
+                            attributes = settings.attribute_overrides.resolve()
+                        if "version" in attributes:
+                            self._uuid_versions[attributes["version"]] = uuid
+
+                    with BlockSignals(self._ui.version) as blocked_widget:
+                        blocked_widget.clear()
+                        model = blocked_widget.model()
+                        for i, version in enumerate(versions):
+                            if version in self._uuid_versions:
+                                blocked_widget.addItem(
+                                    QtGui.QIcon(":/cruiz.png"), version
+                                )
+                                if cruiz.globals.get_main_window().is_recipe_active(
+                                    self._uuid_versions[version]
+                                ):
+                                    item = model.item(i)
+                                    item.setFlags(
+                                        item.flags() & ~QtGui.Qt.ItemIsEnabled
+                                    )
+                            else:
+                                blocked_widget.addItem(version)
+                        blocked_widget.setCurrentIndex(-1)
+            else:
+                # if the conandata.yml is not available, manually specify a version
+                self._ui.version.setEditable(True)
+                self._ui.version.lineEdit().setPlaceholderText(
+                    "Package version to use, e.g. 1.2.3"
+                )
+        else:
+            with BlockSignals(self._ui.version) as blocked_widget:
+                blocked_widget.clear()
+                blocked_widget.addItem(version_in_recipe)
+            # combobox disabled to ensure it's clear that there's no choice
+            self._ui.version.setEnabled(False)
+
     def _get_versions_from_conandata(
         self, conandata: typing.Dict[str, typing.Dict[str, str]]
     ) -> typing.Optional[typing.List[str]]:
-        if not conandata:
-            QtWidgets.QMessageBox.information(
-                self,
-                "No conandata.yaml file beside recipe",
-                "Unable to read the conandata.yml beside the recipe. "
-                "Does the file exist?\n"
-                "The package version number can be manually specified, "
-                "or the conanfile.yml can be added next to the recipe.",
-            )
-            return None
+        assert conandata
         with ConanSettingsReader() as settings:
             path_segments = settings.conandata_version_yaml_pathsegment.resolve()
         if path_segments is None:
             QtWidgets.QMessageBox.information(
                 self,
                 "Cannot identify recipe version numbers from conandata.yml file",
                 "The conandata.yml beside the recipe cannot be parsed for version "
```

### Comparing `cruiz-1.4.0a2/cruiz/mainwindow.py` & `cruiz-1.4.0a3/cruiz/mainwindow.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/managelocalcachesdialog.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/managelocalcachesdialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/__init__.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/addenvironmentdialog.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/addenvironmentdialog.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #!/usr/bin/env python3
 
 """
 Dialog for adding an environment variable
 """
 
 from dataclasses import dataclass
+import typing
 
 from qtpy import QtCore, QtGui, QtWidgets
 
+import cruiz.globals
+
 from cruiz.commands.context import ConanContext
 
 from cruiz.pyside6.local_cache_add_environment import Ui_AddEnvironmentDialog
 
 
 @dataclass
 class KeyValuePair:
@@ -29,25 +32,27 @@
     """
 
     def __init__(self, context: ConanContext, parent: QtWidgets.QWidget) -> None:
         super().__init__(parent)
         self.setAttribute(QtCore.Qt.WA_DeleteOnClose, True)
         self._ui = Ui_AddEnvironmentDialog()
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
-        conan_environment_menu = QtWidgets.QMenu("Conan environment variables", self)
-        for key, _ in context.get_conan_config_environment_variables().items():
+        conan_environment_actions: typing.List[QtGui.QAction] = []
+        for key in context.get_conan_config_environment_variables():
             key_action = QtGui.QAction(key, self)
             key_action.triggered.connect(self._set_name)
-            conan_environment_menu.addAction(key_action)
-        conan_environment_menu.addSeparator()
-        # TODO: CONAN_V2_MODE is obsolete
-        conan_v2_mode_action = QtGui.QAction("CONAN_V2_MODE", self)
-        conan_v2_mode_action.triggered.connect(self._set_name)  # type: ignore
-        conan_environment_menu.addAction(conan_v2_mode_action)
-        self._ui.name.set_custom_menu(conan_environment_menu)
+            conan_environment_actions.append(key_action)
+        if cruiz.globals.CONAN_MAJOR_VERSION == 1:
+            # TODO: CONAN_V2_MODE is obsolete
+            conan_v2_mode_action = QtGui.QAction("CONAN_V2_MODE", self)
+            conan_v2_mode_action.triggered.connect(self._set_name)  # type: ignore
+            conan_environment_actions.append(conan_v2_mode_action)
+        self._ui.name.add_submenu_actions(
+            "Conan environment variables", conan_environment_actions
+        )
         self._ui.name.textChanged.connect(self._updated)
         self._ui.value.textChanged.connect(self._updated)
         self._ui.buttonBox.button(QtWidgets.QDialogButtonBox.Ok).setEnabled(False)
         self._name: str = ""
         self._value: str = ""
 
     def _set_name(self) -> None:
```

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/addextraprofiledirectorydialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/addremotedialog.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/addremotedialog.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,25 +24,23 @@
     """
 
     def __init__(self, parent: QtWidgets.QWidget) -> None:
         super().__init__(parent)
         self.setAttribute(QtCore.Qt.WA_DeleteOnClose, True)
         self._ui = Ui_AddRemoteDialog()
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
-        recent_remotes_menu = QtWidgets.QMenu("Recent remotes", self)
+        recent_remotes_actions: typing.List[QtGui.QAction] = []
         with RecentConanRemotesSettingsReader() as settings:
             recent_remote_urls = settings.urls.resolve()
         if recent_remote_urls:
             for remote in recent_remote_urls:
                 remote_action = QtGui.QAction(remote, self)
                 remote_action.triggered.connect(partial(self._set_remote_url, remote))
-                recent_remotes_menu.addAction(remote_action)
-        else:
-            recent_remotes_menu.setEnabled(False)
-        self._ui.url.set_custom_menu(recent_remotes_menu)
+                recent_remotes_actions.append(remote_action)
+        self._ui.url.add_submenu_actions("Recent remotes", recent_remotes_actions)
         self._ui.url.textChanged.connect(self._updated)
         self._ui.name.textChanged.connect(self._updated)
         self._ui.buttonBox.button(QtWidgets.QDialogButtonBox.Ok).clicked.connect(
             self.accept
         )
         self._ui.buttonBox.button(QtWidgets.QDialogButtonBox.Ok).setEnabled(False)
         self._ui.buttonBox.button(QtWidgets.QDialogButtonBox.Cancel).clicked.connect(
```

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/installconfigdialog.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/installconfigdialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,25 +29,25 @@
 
     def __init__(self, context: ConanContext, parent: QtWidgets.QWidget) -> None:
         super().__init__(parent)
         self.setAttribute(QtCore.Qt.WA_DeleteOnClose, True)
         self._ui = Ui_InstallConfigDialog()
         self._ui.setupUi(self)  # type: ignore[no-untyped-call]
         self._context = context
-        recent_config_paths_menu = QtWidgets.QMenu("Recent config paths", self)
+        recent_config_paths_actions: typing.List[QtGui.QAction] = []
         with RecentConanConfigSettingsReader() as settings:
             config_paths = settings.paths.resolve()
         if config_paths:
             for path in config_paths:
                 path_action = QtGui.QAction(path, self)
                 path_action.triggered.connect(partial(self._set_url, path))
-                recent_config_paths_menu.addAction(path_action)
-        else:
-            recent_config_paths_menu.setEnabled(False)
-        self._ui.pathOrUrl.set_custom_menu(recent_config_paths_menu)
+                recent_config_paths_actions.append(path_action)
+        self._ui.pathOrUrl.add_submenu_actions(
+            "Recent config paths", recent_config_paths_actions
+        )
         self._ui.pathOrUrl.textChanged.connect(self._path_updated)
         self._ui.installButton.setEnabled(False)
         self._ui.installButton.clicked.connect(self._install)
         self._ui.buttonBox.button(QtWidgets.QDialogButtonBox.Cancel).clicked.connect(
             self._cancel
         )
```

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/keyvaluetable.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/keyvaluetable.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/movelocalcachedialog.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/movelocalcachedialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/newlocalcachewizard.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/newlocalcachewizard.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/newlocalcachewizardpages.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/progressdialogs.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/progressdialogs.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/remotestable.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/remotestable.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/removeenvironmentdialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/manage_local_cache/widgets/runconancommanddialog.py` & `cruiz-1.4.0a3/cruiz/manage_local_cache/widgets/runconancommanddialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/model/graphaslistmodel.py` & `cruiz-1.4.0a3/cruiz/model/graphaslistmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/recipe/dependencyview.py` & `cruiz-1.4.0a3/cruiz/recipe/dependencyview.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/recipe/expressioneditordialog.py` & `cruiz-1.4.0a3/cruiz/recipe/expressioneditordialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/recipe/findtextdialog.py` & `cruiz-1.4.0a3/cruiz/recipe/findtextdialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/recipe/logs/command.py` & `cruiz-1.4.0a3/cruiz/recipe/logs/command.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/recipe/recipe.py` & `cruiz-1.4.0a3/cruiz/recipe/recipe.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/recipe/recipewidget.py` & `cruiz-1.4.0a3/cruiz/recipe/recipewidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,20 +253,31 @@
         )
         self._ui.localWorkflowProfileAndVersionBasedSubdirs.clicked.connect(
             self._local_workflow_full_spec_folders
         )
         self._ui.localWorkflowExpressionEditor.clicked.connect(
             self._local_workflow_expression_editor
         )
+        extra_option_list_regex = QtCore.QRegularExpression(
+            # of the form <pkg>:<option>=<value>[,<repeat>]
+            r"^$|^([^:=,\s]+:[^=,\s]+=[^,\s]+)(\s*,\s*[^:=,\s]+:[^=,\s]+=[^,\s]+)*$"
+        )
+        extra_option_list_validator = QtGui.QRegularExpressionValidator(
+            extra_option_list_regex, self
+        )
+        self._ui.configureAdditionalOptions.setValidator(extra_option_list_validator)
         rgx = QtCore.QRegularExpression(r"(^$|^@([a-zA-Z]+)\/([a-zA-Z]+)$)")
         comValidator = QtGui.QRegularExpressionValidator(rgx, self)
         self._ui.configurePkgRefNamespace.setValidator(comValidator)
         self._ui.configurePkgRefNamespace.editingFinished.connect(
             self._configure_packageref_namespace
         )
+        self._ui.configureAdditionalOptions.editingFinished.connect(
+            self._configure_additional_options
+        )
         self._ui.configurePackageId.customContextMenuRequested.connect(
             self._on_configure_packageid_context_menu
         )
         # tabify the docks on the right hand side
         self.tabifyDockWidget(
             self._ui.conanLocalWorkflowDock, self._ui.conanConfigureDock
         )
@@ -696,14 +707,17 @@
         with RecipeSettingsReader.from_recipe(self.recipe) as settings:
             options = settings.options.resolve()
             attributes = settings.attribute_overrides.resolve()
         if "user" in attributes:
             assert "channel" in attributes
             with BlockSignals(self._ui.configurePkgRefNamespace) as blocked_widget:
                 blocked_widget.setText(f"@{attributes['user']}/{attributes['channel']}")
+        if "extra_config_options" in attributes:
+            with BlockSignals(self._ui.configureAdditionalOptions) as blocked_widget:
+                blocked_widget.setText(attributes["extra_config_options"])
         clear_widgets_from_layout(self._ui.optionsLayout)
         recipe_options = self._get_options_from_recipe(recipe_attributes)
         for i, (key, values, default_value) in enumerate(recipe_options):
             self._ui.optionsLayout.addWidget(QtWidgets.QLabel(key), i, 0)
             if (isinstance(values, str) and values == "ANY") or (
                 isinstance(values, list) and "ANY" in values
             ):
@@ -1016,14 +1030,24 @@
                 {"user": user, "channel": channel}  # type: ignore
             )
         else:
             settings.append_attribute({"user": None, "channel": None})  # type: ignore
         RecipeSettingsWriter.from_recipe(self.recipe).sync(settings)
         self.configuration_changed.emit()
 
+    def _configure_additional_options(self) -> None:
+        text = self.sender().text()
+        settings = RecipeSettings()
+        if text:
+            settings.append_attribute({"extra_config_options": text})  # type: ignore
+        else:
+            settings.append_attribute({"extra_config_options": None})  # type: ignore
+        RecipeSettingsWriter.from_recipe(self.recipe).sync(settings)
+        self.configuration_changed.emit()
+
     def _open_recipe_in_editor(self) -> None:
         # TODO: make the editor a preference
         with GeneralSettingsReader() as settings:
             recipe_editor = settings.default_recipe_editor.resolve()
         if recipe_editor:
             script_args = [str(self.recipe.path)]
             QtCore.QProcess.execute(recipe_editor, script_args)
@@ -1066,14 +1090,19 @@
         params.user = self.recipe.user
         params.channel = self.recipe.channel
         with RecipeSettingsReader.from_recipe(self.recipe) as settings:
             params.profile = settings.profile.resolve()
             for key, value in settings.options.resolve().items():
                 # TODO: is this the most efficient algorithm?
                 params.add_option(params.name, key, value)  # type: ignore
+            attributes = settings.attribute_overrides.resolve()
+            if "extra_config_options" in attributes:
+                for keyvalue in attributes["extra_config_options"].split(","):
+                    option_name, option_value = keyvalue.split("=")
+                    params.add_option(None, option_name, option_value)
         self._dependency_generate_context.conancommand(
             params,
             None,
             self._on_dependency_graph_generated,
         )
 
     def _on_dependency_graph_generated(
```

### Comparing `cruiz-1.4.0a2/cruiz/recipe/toolbars/behaviour.py` & `cruiz-1.4.0a3/cruiz/recipe/toolbars/behaviour.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/recipe/toolbars/buildfeatures.py` & `cruiz-1.4.0a3/cruiz/recipe/toolbars/buildfeatures.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/recipe/toolbars/command.py` & `cruiz-1.4.0a3/cruiz/recipe/toolbars/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,14 +388,19 @@
                     )
             if with_options:
                 for key, value in settings.options.resolve().items():
                     assert recipe_attributes["name"]
                     params.add_option(
                         recipe_attributes["name"], key, value
                     )  # TODO: is this the most efficient algorithm?
+                attributes = settings.attribute_overrides.resolve()
+                if "extra_config_options" in attributes:
+                    for keyvalue in attributes["extra_config_options"].split(","):
+                        option_name, option_value = keyvalue.split("=")
+                        params.add_option(None, option_name, option_value)
             self._append_build_features(params, settings)
             if with_exclusive_package_folder:
                 # export-pkg requires
                 # - if package_folder is present, do not specify source or build folder
                 # - if package_folder is NOT present, you might still need the fudge of
                 #   the source folder
                 if settings.local_workflow_package_folder.resolve() is None:
```

### Comparing `cruiz-1.4.0a2/cruiz/remote_browser/pages/packagebinarypage.py` & `cruiz-1.4.0a3/cruiz/remote_browser/pages/packagebinarypage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/remote_browser/pages/packageidpage.py` & `cruiz-1.4.0a3/cruiz/remote_browser/pages/packageidpage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/remote_browser/pages/packagereferencepage.py` & `cruiz-1.4.0a3/cruiz/remote_browser/pages/packagereferencepage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/remote_browser/pages/packagerevisionpage.py` & `cruiz-1.4.0a3/cruiz/remote_browser/pages/packagerevisionpage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/remote_browser/pages/page.py` & `cruiz-1.4.0a3/cruiz/remote_browser/pages/page.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/remote_browser/pages/reciperevisionpage.py` & `cruiz-1.4.0a3/cruiz/remote_browser/pages/reciperevisionpage.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/remote_browser/remotebrowser.py` & `cruiz-1.4.0a3/cruiz/remote_browser/remotebrowser.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resourcegeneration.py` & `cruiz-1.4.0a3/cruiz/resourcegeneration.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/001-rubbish.svg` & `cruiz-1.4.0a3/cruiz/resources/001-rubbish.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/002-null.svg` & `cruiz-1.4.0a3/cruiz/resources/002-null.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/003-chemistry.svg` & `cruiz-1.4.0a3/cruiz/resources/003-chemistry.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/004-share.svg` & `cruiz-1.4.0a3/cruiz/resources/004-share.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/005-box.svg` & `cruiz-1.4.0a3/cruiz/resources/005-box.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/006-toolbox.svg` & `cruiz-1.4.0a3/cruiz/resources/006-toolbox.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/007-book.svg` & `cruiz-1.4.0a3/cruiz/resources/007-book.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/008-cloud-computing.svg` & `cruiz-1.4.0a3/cruiz/resources/008-cloud-computing.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/009-import.svg` & `cruiz-1.4.0a3/cruiz/resources/009-import.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/010-draw.svg` & `cruiz-1.4.0a3/cruiz/resources/010-draw.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/012-hammer.svg` & `cruiz-1.4.0a3/cruiz/resources/012-hammer.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/013-pencil.svg` & `cruiz-1.4.0a3/cruiz/resources/013-pencil.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/014-code.svg` & `cruiz-1.4.0a3/cruiz/resources/014-code.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/Cmake.svg` & `cruiz-1.4.0a3/cruiz/resources/Cmake.svg`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/about_dialog.ui` & `cruiz-1.4.0a3/cruiz/resources/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/cruise.png` & `cruiz-1.4.0a3/cruiz/resources/cruise.png`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/cruizres.qrc` & `cruiz-1.4.0a3/cruiz/resources/cruizres.qrc`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/find_text_dialog.ui` & `cruiz-1.4.0a3/cruiz/resources/find_text_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/license-cruise.pdf` & `cruiz-1.4.0a3/cruiz/resources/license-cruise.pdf`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/license.pdf` & `cruiz-1.4.0a3/cruiz/resources/license.pdf`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/load_recipe_wizard.ui` & `cruiz-1.4.0a3/cruiz/resources/load_recipe_wizard.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/local_cache_add_environment.ui` & `cruiz-1.4.0a3/cruiz/resources/local_cache_add_environment.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/local_cache_add_profile_directory.ui` & `cruiz-1.4.0a3/cruiz/resources/local_cache_add_profile_directory.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/local_cache_add_remote.ui` & `cruiz-1.4.0a3/cruiz/resources/local_cache_add_remote.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/local_cache_install_config.ui` & `cruiz-1.4.0a3/cruiz/resources/local_cache_install_config.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/local_cache_manage.ui` & `cruiz-1.4.0a3/cruiz/resources/local_cache_manage.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/local_cache_move.ui` & `cruiz-1.4.0a3/cruiz/resources/local_cache_move.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/local_cache_new_wizard.ui` & `cruiz-1.4.0a3/cruiz/resources/local_cache_new_wizard.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/local_cache_remove_environment.ui` & `cruiz-1.4.0a3/cruiz/resources/local_cache_remove_environment.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/local_cache_run_command_dialog.ui` & `cruiz-1.4.0a3/cruiz/resources/local_cache_run_command_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/preferences.ui` & `cruiz-1.4.0a3/cruiz/resources/preferences.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/recipe_cmake_features_frame.ui` & `cruiz-1.4.0a3/cruiz/resources/recipe_cmake_features_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui` & `cruiz-1.4.0a3/cruiz/resources/recipe_compiler_cache_configuration_dialog.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/recipe_compilercache_features_frame.ui` & `cruiz-1.4.0a3/cruiz/resources/recipe_compilercache_features_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/recipe_cpucores_frame.ui` & `cruiz-1.4.0a3/cruiz/resources/recipe_cpucores_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/recipe_local_workflow_expression_editor.ui` & `cruiz-1.4.0a3/cruiz/resources/recipe_local_workflow_expression_editor.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/recipe_profile_frame.ui` & `cruiz-1.4.0a3/cruiz/resources/recipe_profile_frame.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/recipe_window.ui` & `cruiz-1.4.0a3/cruiz/resources/recipe_window.ui`

 * *Files 1% similar despite different names*

#### Comparing `cruiz-1.4.0a2/cruiz/resources/recipe_window.ui` & `cruiz-1.4.0a3/cruiz/resources/recipe_window.ui`

```diff
@@ -312,16 +312,16 @@
                 <bool>true</bool>
               </property>
               <widget class="QWidget" name="scrollAreaWidgetContents_2">
                 <property name="geometry">
                   <rect>
                     <x>0</x>
                     <y>0</y>
-                    <width>313</width>
-                    <height>211</height>
+                    <width>312</width>
+                    <height>281</height>
                   </rect>
                 </property>
                 <layout class="QVBoxLayout" name="verticalLayout_13">
                   <item>
                     <widget class="QGroupBox" name="groupBox_7">
                       <property name="title">
                         <string>Package ID</string>
@@ -348,14 +348,29 @@
                       <property name="title">
                         <string>Options</string>
                       </property>
                       <layout class="QGridLayout" name="optionsLayout"/>
                     </widget>
                   </item>
                   <item>
+                    <widget class="QGroupBox" name="groupBox">
+                      <property name="toolTip">
+                        <string>A comma separated list of &lt;pkg&gt;:&lt;option&gt;=&lt;value&gt;</string>
+                      </property>
+                      <property name="title">
+                        <string>Additional options</string>
+                      </property>
+                      <layout class="QVBoxLayout" name="verticalLayout_20">
+                        <item>
+                          <widget class="QLineEdit" name="configureAdditionalOptions"/>
+                        </item>
+                      </layout>
+                    </widget>
+                  </item>
+                  <item>
                     <widget class="QGroupBox" name="groupBox_2">
                       <property name="title">
                         <string>Package reference namespace</string>
                       </property>
                       <layout class="QVBoxLayout" name="verticalLayout_19">
                         <item>
                           <widget class="QLineEdit" name="configurePkgRefNamespace">
@@ -414,15 +429,15 @@
                 <bool>true</bool>
               </property>
               <widget class="QWidget" name="scrollAreaWidgetContents">
                 <property name="geometry">
                   <rect>
                     <x>0</x>
                     <y>0</y>
-                    <width>328</width>
+                    <width>327</width>
                     <height>535</height>
                   </rect>
                 </property>
                 <layout class="QVBoxLayout" name="verticalLayout_12">
                   <item>
                     <layout class="QGridLayout" name="gridLayout_3">
                       <item row="0" column="0">
@@ -629,15 +644,15 @@
                 <bool>true</bool>
               </property>
               <widget class="QWidget" name="scrollAreaWidgetContents_3">
                 <property name="geometry">
                   <rect>
                     <x>0</x>
                     <y>0</y>
-                    <width>326</width>
+                    <width>214</width>
                     <height>531</height>
                   </rect>
                 </property>
                 <layout class="QVBoxLayout" name="verticalLayout_14">
                   <item>
                     <widget class="QTabWidget" name="dependentsTabs">
                       <property name="currentIndex">
```

### Comparing `cruiz-1.4.0a2/cruiz/resources/remote_browser.ui` & `cruiz-1.4.0a3/cruiz/resources/remote_browser.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/resources/remote_browser_fileview.ui` & `cruiz-1.4.0a3/cruiz/resources/remote_browser_fileview.ui`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/revealonfilesystem.py` & `cruiz-1.4.0a3/cruiz/revealonfilesystem.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/ensuredefaultlocalcache.py` & `cruiz-1.4.0a3/cruiz/settings/ensuredefaultlocalcache.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/__init__.py` & `cruiz-1.4.0a3/cruiz/settings/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/basesettings.py` & `cruiz-1.4.0a3/cruiz/settings/managers/basesettings.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/cleansettings.py` & `cruiz-1.4.0a3/cruiz/settings/managers/cleansettings.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/cmakepreferences.py` & `cruiz-1.4.0a3/cruiz/settings/managers/cmakepreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/compilercachepreferences.py` & `cruiz-1.4.0a3/cruiz/settings/managers/compilercachepreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/conanpreferences.py` & `cruiz-1.4.0a3/cruiz/settings/managers/conanpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/fontpreferences.py` & `cruiz-1.4.0a3/cruiz/settings/managers/fontpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/generalpreferences.py` & `cruiz-1.4.0a3/cruiz/settings/managers/generalpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/graphvizpreferences.py` & `cruiz-1.4.0a3/cruiz/settings/managers/graphvizpreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/localcachepreferences.py` & `cruiz-1.4.0a3/cruiz/settings/managers/localcachepreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/namedlocalcache.py` & `cruiz-1.4.0a3/cruiz/settings/managers/namedlocalcache.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/ninjapreferences.py` & `cruiz-1.4.0a3/cruiz/settings/managers/ninjapreferences.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/recentconanconfigs.py` & `cruiz-1.4.0a3/cruiz/settings/managers/recentconanconfigs.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/recentconanremotes.py` & `cruiz-1.4.0a3/cruiz/settings/managers/recentconanremotes.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/recentrecipes.py` & `cruiz-1.4.0a3/cruiz/settings/managers/recentrecipes.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/recipe.py` & `cruiz-1.4.0a3/cruiz/settings/managers/recipe.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/shortcuts.py` & `cruiz-1.4.0a3/cruiz/settings/managers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/valueclasses.py` & `cruiz-1.4.0a3/cruiz/settings/managers/valueclasses.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/managers/writermixin.py` & `cruiz-1.4.0a3/cruiz/settings/managers/writermixin.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/models/recentconanconfigmodel.py` & `cruiz-1.4.0a3/cruiz/settings/models/recentconanconfigmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/models/recentconanremotesmodel.py` & `cruiz-1.4.0a3/cruiz/settings/models/recentconanremotesmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/models/recipesmodel.py` & `cruiz-1.4.0a3/cruiz/settings/models/recipesmodel.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/preferencesdialog.py` & `cruiz-1.4.0a3/cruiz/settings/preferencesdialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/settings/updatesettings.py` & `cruiz-1.4.0a3/cruiz/settings/updatesettings.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/svggraph.py` & `cruiz-1.4.0a3/cruiz/svggraph.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/version.py` & `cruiz-1.4.0a3/cruiz/version.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/widgets/aboutcruizdialog.py` & `cruiz-1.4.0a3/cruiz/widgets/aboutcruizdialog.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/widgets/debugging.py` & `cruiz-1.4.0a3/cruiz/widgets/debugging.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/widgets/shortcutlineedit.py` & `cruiz-1.4.0a3/cruiz/widgets/shortcutlineedit.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/widgets/util.py` & `cruiz-1.4.0a3/cruiz/widgets/util.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/workers/api/__init__.py` & `cruiz-1.4.0a3/cruiz/workers/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/workers/utils/colorarma_conversion.py` & `cruiz-1.4.0a3/cruiz/workers/utils/colorarma_conversion.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/workers/utils/env.py` & `cruiz-1.4.0a3/cruiz/workers/utils/env.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/workers/utils/formatoptions.py` & `cruiz-1.4.0a3/cruiz/workers/utils/formatoptions.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/workers/utils/qtlogger.py` & `cruiz-1.4.0a3/cruiz/workers/utils/qtlogger.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/workers/utils/stream.py` & `cruiz-1.4.0a3/cruiz/workers/utils/stream.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/workers/utils/text2html.py` & `cruiz-1.4.0a3/cruiz/workers/utils/text2html.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz/workers/utils/worker.py` & `cruiz-1.4.0a3/cruiz/workers/utils/worker.py`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/cruiz.egg-info/PKG-INFO` & `cruiz-1.4.0a3/cruiz.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: cruiz
-Version: 1.4.0a2
+Version: 1.4.0a3
 Summary: Conan recipe user interface
 Home-page: https://github.com/markfinal/cruiz
 Author: Mark Final
 Author-email: markfinal@hotmail.com
 Project-URL: Documentation, https://cruiz.readthedocs.io/en/latest/
 Project-URL: GitHub, https://github.com/markfinal/cruiz
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7, <3.12
+Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # cruiz
 
 Conan recipe user interface
@@ -37,15 +36,15 @@
 
 - Intel x86_64 platforms:
   - Windows 10+
   - Linux (CentOS 7.5+/Ubuntu 18+)
   - macOS (11.0+)
 - Apple Silicon platforms:
   - macOS (11.0+)
-- Python 3.7-3.11
+- Python 3.8-3.11
 - Conan 1.x (from 1.17.1 onwards) and 2.x (from 2.0.7 onwards)
 
 All other Python dependencies are installed when the package is installed.
 
 In order to use the dependency graph visualisation, an additional installation of GraphViz is required from https://graphviz.org/download/. Assign the installed location to the preferences.
 
 ## Conan versions
```

### Comparing `cruiz-1.4.0a2/cruiz.egg-info/SOURCES.txt` & `cruiz-1.4.0a3/cruiz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cruiz-1.4.0a2/setup.py` & `cruiz-1.4.0a3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,19 +140,18 @@
         ],
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    python_requires=">=3.7, <3.12",
+    python_requires=">=3.8, <3.12",
     project_urls={
         "Documentation": "https://cruiz.readthedocs.io/en/latest/",
         "GitHub": "https://github.com/markfinal/cruiz",
     },
 )
```

