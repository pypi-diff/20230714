# Comparing `tmp/srsgui-0.4.1.tar.gz` & `tmp/srsgui-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-24fcqa60\srsgui-0.4.1.tar", last modified: Thu Jul  6 00:39:16 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-avc40r37\srsgui-0.4.2.tar", last modified: Fri Jul 14 20:48:18 2023, max compression
```

## Comparing `srsgui-0.4.1.tar` & `srsgui-0.4.2.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.473875 srsgui-0.4.1/
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.317450 srsgui-0.4.1/.github/
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.327688 srsgui-0.4.1/.github/workflows/
--rw-rw-rw-   0        0        0      388 2023-06-19 18:04:40.000000 srsgui-0.4.1/.github/workflows/pages.yml
--rw-rw-rw-   0        0        0     1356 2023-05-16 23:33:10.000000 srsgui-0.4.1/.gitignore
--rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4047 2023-07-06 00:39:16.467606 srsgui-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3068 2023-06-27 19:21:08.000000 srsgui-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.352532 srsgui-0.4.1/docs/
--rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.372521 srsgui-0.4.1/docs/_static/
--rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    88057 2023-06-08 18:01:11.000000 srsgui-0.4.1/docs/_static/dock_widget_floating.png
--rw-rw-rw-   0        0        0    97266 2023-06-08 18:01:11.000000 srsgui-0.4.1/docs/_static/dock_widgets_expanded.png
--rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    52123 2023-06-08 23:01:31.000000 srsgui-0.4.1/docs/_static/lockin-capture.png
--rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    38581 2023-06-08 18:01:11.000000 srsgui-0.4.1/docs/_static/task_selection.png
--rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     8703 2023-06-27 19:21:08.000000 srsgui-0.4.1/docs/application.rst
--rw-rw-rw-   0        0        0      840 2023-06-26 20:05:20.000000 srsgui-0.4.1/docs/changelog.rst
--rw-rw-rw-   0        0        0     1921 2023-06-29 20:28:19.000000 srsgui-0.4.1/docs/conf.py
--rw-rw-rw-   0        0        0     6261 2023-07-06 00:33:39.000000 srsgui-0.4.1/docs/create-project.rst
--rw-rw-rw-   0        0        0     7546 2023-06-29 20:28:19.000000 srsgui-0.4.1/docs/create-task.rst
--rw-rw-rw-   0        0        0     6547 2023-06-29 20:28:19.000000 srsgui-0.4.1/docs/define-instrument.rst
--rw-rw-rw-   0        0        0    16624 2023-06-27 19:21:08.000000 srsgui-0.4.1/docs/example.rst
--rw-rw-rw-   0        0        0     3803 2023-06-15 00:44:23.000000 srsgui-0.4.1/docs/index.rst
--rw-rw-rw-   0        0        0     4539 2023-06-27 19:21:08.000000 srsgui-0.4.1/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/make.bat
--rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.4.1/docs/requirements..txt
--rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.4.1/docs/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      930 2023-06-08 18:01:11.000000 srsgui-0.4.1/docs/srsgui.inst.rst
--rw-rw-rw-   0        0        0      113 2023-05-24 20:30:53.000000 srsgui-0.4.1/docs/srsgui.rst
--rw-rw-rw-   0        0        0     1077 2023-05-24 20:30:53.000000 srsgui-0.4.1/docs/srsgui.task.rst
--rw-rw-rw-   0        0        0     2065 2023-05-24 20:30:53.000000 srsgui-0.4.1/docs/srsgui.ui.commandtree.rst
--rw-rw-rw-   0        0        0      603 2023-05-24 20:30:53.000000 srsgui-0.4.1/docs/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1646 2023-05-24 20:30:53.000000 srsgui-0.4.1/docs/srsgui.ui.rst
--rw-rw-rw-   0        0        0     1101 2023-06-23 17:22:50.000000 srsgui-0.4.1/docs/troubleshooting.rst
--rw-rw-rw-   0        0        0     1488 2023-07-06 00:33:39.000000 srsgui-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.4.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 00:39:16.473875 srsgui-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.382514 srsgui-0.4.1/srsgui/
--rw-rw-rw-   0        0        0     1537 2023-07-06 00:38:03.000000 srsgui-0.4.1/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.4.1/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.325684 srsgui-0.4.1/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.382514 srsgui-0.4.1/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.392509 srsgui-0.4.1/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1960 2023-06-27 19:21:08.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.392509 srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2583 2023-06-27 19:21:08.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.402504 srsgui-0.4.1/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.4.1/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9907 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.412499 srsgui-0.4.1/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.4.1/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8774 2023-06-23 17:22:50.000000 srsgui-0.4.1/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    19291 2023-06-23 17:22:50.000000 srsgui-0.4.1/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10410 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9990 2023-06-19 18:04:40.000000 srsgui-0.4.1/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.427623 srsgui-0.4.1/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.4.1/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0     1192 2023-06-27 19:21:08.000000 srsgui-0.4.1/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6989 2023-06-21 20:11:21.000000 srsgui-0.4.1/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5856 2023-06-21 20:11:21.000000 srsgui-0.4.1/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6938 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    25859 2023-06-29 20:28:19.000000 srsgui-0.4.1/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.447616 srsgui-0.4.1/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.4.1/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     6880 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.457636 srsgui-0.4.1/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0        0 2023-05-19 00:30:39.000000 srsgui-0.4.1/srsgui/ui/commandtree/__init__.py
--rw-rw-rw-   0        0        0     3941 2023-05-23 19:11:06.000000 srsgui-0.4.1/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/commandtree/commandhandler.py
--rw-rw-rw-   0        0        0    12605 2023-06-23 17:22:50.000000 srsgui-0.4.1/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     8669 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     5109 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     4852 2023-06-19 18:04:40.000000 srsgui-0.4.1/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.4.1/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9796 2023-06-27 19:21:08.000000 srsgui-0.4.1/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    15880 2023-06-08 18:01:11.000000 srsgui-0.4.1/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    14950 2023-06-27 19:15:07.000000 srsgui-0.4.1/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.467606 srsgui-0.4.1/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1449 2023-05-24 20:30:53.000000 srsgui-0.4.1/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.4.1/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.4.1/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.4.1/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    26550 2023-06-26 20:05:20.000000 srsgui-0.4.1/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.4.1/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.4.1/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-07-06 00:39:16.382514 srsgui-0.4.1/srsgui.egg-info/
--rw-rw-rw-   0        0        0     4047 2023-07-06 00:39:16.000000 srsgui-0.4.1/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3170 2023-07-06 00:39:16.000000 srsgui-0.4.1/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 00:39:16.000000 srsgui-0.4.1/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-06 00:39:16.000000 srsgui-0.4.1/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      103 2023-07-06 00:39:16.000000 srsgui-0.4.1/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 00:39:16.000000 srsgui-0.4.1/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.791865 srsgui-0.4.2/
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.705507 srsgui-0.4.2/.github/
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.715501 srsgui-0.4.2/.github/workflows/
+-rw-rw-rw-   0        0        0      388 2023-07-14 19:39:01.000000 srsgui-0.4.2/.github/workflows/pages.yml
+-rw-rw-rw-   0        0        0     1356 2023-07-14 19:39:01.000000 srsgui-0.4.2/.gitignore
+-rw-rw-rw-   0        0        0     1113 2023-07-14 19:39:01.000000 srsgui-0.4.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     4626 2023-07-14 20:48:18.791865 srsgui-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3595 2023-07-14 19:39:01.000000 srsgui-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.725496 srsgui-0.4.2/docs/
+-rw-rw-rw-   0        0        0      654 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.745485 srsgui-0.4.2/docs/_static/
+-rw-rw-rw-   0        0        0    31067 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    88057 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/dock_widget_floating.png
+-rw-rw-rw-   0        0        0    97266 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/dock_widgets_expanded.png
+-rw-rw-rw-   0        0        0    71070 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    52123 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/lockin-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    38581 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/task_selection.png
+-rw-rw-rw-   0        0        0    39412 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     8703 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/application.rst
+-rw-rw-rw-   0        0        0      840 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1921 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/conf.py
+-rw-rw-rw-   0        0        0     6270 2023-07-14 20:36:38.000000 srsgui-0.4.2/docs/create-project.rst
+-rw-rw-rw-   0        0        0     7546 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/create-task.rst
+-rw-rw-rw-   0        0        0     6547 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/define-instrument.rst
+-rw-rw-rw-   0        0        0    16790 2023-07-14 20:42:29.000000 srsgui-0.4.2/docs/example.rst
+-rw-rw-rw-   0        0        0     3837 2023-07-14 20:26:07.000000 srsgui-0.4.2/docs/index.rst
+-rw-rw-rw-   0        0        0     4539 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/make.bat
+-rw-rw-rw-   0        0        0       34 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/requirements..txt
+-rw-rw-rw-   0        0        0      936 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      930 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      113 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.rst
+-rw-rw-rw-   0        0        0     1077 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.task.rst
+-rw-rw-rw-   0        0        0     2065 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.ui.commandtree.rst
+-rw-rw-rw-   0        0        0      603 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1646 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/srsgui.ui.rst
+-rw-rw-rw-   0        0        0     1101 2023-07-14 19:39:01.000000 srsgui-0.4.2/docs/troubleshooting.rst
+-rw-rw-rw-   0        0        0     1539 2023-07-14 19:39:01.000000 srsgui-0.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-07-14 19:39:01.000000 srsgui-0.4.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 20:48:18.791865 srsgui-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-07-14 19:39:01.000000 srsgui-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.745485 srsgui-0.4.2/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.705507 srsgui-0.4.2/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.745485 srsgui-0.4.2/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.745485 srsgui-0.4.2/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1829 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3147 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1998 2023-07-14 19:58:54.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.755479 srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     4101 2023-07-14 20:06:32.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/captured_fft.py
+-rw-rw-rw-   0        0        0     1662 2023-07-14 20:06:33.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/identify.py
+-rw-rw-rw-   0        0        0     2585 2023-07-14 20:06:33.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/plot_example.py
+-rw-rw-rw-   0        0        0     1946 2023-07-14 20:46:40.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/scope_capture.py
+-rw-rw-rw-   0        0        0     2549 2023-07-14 20:31:28.000000 srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/simulated_fft.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.755479 srsgui-0.4.2/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9908 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.765474 srsgui-0.4.2/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     8309 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1277 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8775 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    11334 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    19292 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      845 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10411 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9991 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.765474 srsgui-0.4.2/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0     1193 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6990 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5858 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6939 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    25860 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4226 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.785463 srsgui-0.4.2/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3895 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     6881 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.791865 srsgui-0.4.2/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0        0 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/__init__.py
+-rw-rw-rw-   0        0        0     3942 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0     1604 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commandhandler.py
+-rw-rw-rw-   0        0        0    12606 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     8670 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     5110 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3453 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     4853 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9797 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3976 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    15881 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    14951 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.791865 srsgui-0.4.2/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      800 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      678 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      778 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1449 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1286 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15479 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2718 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0     1006 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    26551 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-07-14 19:39:01.000000 srsgui-0.4.2/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:48:18.745485 srsgui-0.4.2/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     4626 2023-07-14 20:48:18.000000 srsgui-0.4.2/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3201 2023-07-14 20:48:18.000000 srsgui-0.4.2/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 20:48:18.000000 srsgui-0.4.2/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-14 20:48:18.000000 srsgui-0.4.2/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      103 2023-07-14 20:48:18.000000 srsgui-0.4.2/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-14 20:48:18.000000 srsgui-0.4.2/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.4.1/.gitignore` & `srsgui-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/LICENSE.txt` & `srsgui-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/PKG-INFO` & `srsgui-0.4.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,73 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.4.1
+Version: 0.4.2
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 # ``Srsgui`` - Organize instrument-controlling Python scripts as a GUI application
 
 `Srsgui` is a simple framework:
 
-   - To define instrument classes for instruments that use remote communication,
-     based on the `Instrument` class and the communication `Interface` class. 
+   - To define instrument classes for instruments that use remote communication, based on the 
+     [`Instrument`](https://thinksrs.github.io/srsgui/srsgui.inst.html#module-srsgui.inst.instrument) 
+     class and the communication 
+     [`Interface`](https://thinksrs.github.io/srsgui/srsgui.inst.communications.html) classes. 
      (By default, serial and TCPIP is available. VXI11, GPIB and USB-TMC are optional).
 
-   - To write Python scripts (tasks) that run in GUI environment with simple APIs
-     provided in ``Task`` class.
+   - To write Python scripts (tasks) that run in graphic user interface (GUI) environment using simple
+     application programming interfaces (APIs) provided in 
+     [``Task``](https://thinksrs.github.io/srsgui/srsgui.task.html) class.
 
    - To organize instrument classes and task scripts presented in a GUI application
-     using a configuration (.taskconfig) file for a project.
+     using a configuration 
+     [(.taskconfig)](https://thinksrs.github.io/srsgui/create-project.html#populating-the-taskconfig-file)
+     file for a project.
 
 ![screenshot](https://thinksrs.github.io/srsgui/_images/example-screen-capture-2.png " ")
 
 ## Installation
 
-To run ``srsgui`` as an application, create a virtual environment, if necessary, 
+To run ``srsgui`` as an GUI application, create a virtual environment, if necessary, 
 and install using ``pip`` with the `[full]` option:  
 
     python -m pip install srsgui[full]
 
 ``Srsgui`` package has the following 3 main dependencies: 
 [pyserial](https://pypi.org/project/pyserial/), 
 [matplotlib](https://pypi.org/project/matplotlib/) and
-[PySide6](https://pypi.org/project/PySide6/). If the installation above fails, 
+[PySide6](https://pypi.org/project/PySide6/) 
+(or [PySide2](https://pypi.org/project/PySide2/)). If the installation above fails, 
 you have to install the failed pacakge manually. Using a virtual environment will
 eliminate possible conflicts between packages in the main Python installation and 
-the packages. Some Linux distributions offer certain Python packages from their repositories only (i.e. not from ``pip``). 
+the packages. Some Linux distributions offer certain Python packages from their 
+repositories only (not from ``pip``). 
 Run a web search for more information on system-specific installation.   
 
-Once pyserial, matplotlib and PySide6 are installed properly, or if you plan to use `srsgui` for instrument drivers only without GUI support, 
+Once pyserial, matplotlib and PySide6 (or PySide2) are installed properly, or if you plan to use 
+`srsgui` for instrument drivers only without GUI support, 
 you can install ``srsgui`` without the `[full]` option:
 
     python -m pip install srsgui
 
 ## Start ``srsgui`` application
     
 If the Python Script directory is in the PATH environment variable,
@@ -69,22 +78,24 @@
 If the script directory is not in PATH, run the srsgui module with Python. 
 
     python -m srsgui
 
 
 ## Run the example project
 
-By default, the `srsgui` application starts with the project that was running when it was last closed.
+By default, the `srsgui` application starts with the project that was running when it was closed the last time.
  
-To open the **oscilloscope example project** included in the `srsgui` package 
+To open the [**oscilloscope example project**](https://thinksrs.github.io/srsgui/example.html)
+included in the `srsgui` package  
 (if `srsgui` does not start with the example project), select File/Open config, 
-go to the `srsgui` package directory, find the examples directory, and select the `oscilloscope example project.taskconfig` file
-in the example project folder. 
+go to the `srsgui` package directory, find the examples directory, and select the 
+`oscilloscope example project.taskconfig` file in the example project folder. 
 
-You can run the **Plot example** and **FFT of simulated waveform** tasks from the Task menu without any instruments connected.
+You can run the **Plot example** and **FFT of simulated waveform** tasks from 
+the Task menu without any instruments connected.
 
 ## Create a project
 
 `Srsgui` is a framework to help you to write your own instrument-controlling 
 Python scripts and run them from a GUI application. Using its APIs, you can write 
 scripts running in GUI with the same amount of code as writing console-based 
 scripts. For programming using the API, refer to the
```

### Comparing `srsgui-0.4.1/README.md` & `srsgui-0.4.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 # ``Srsgui`` - Organize instrument-controlling Python scripts as a GUI application
 
 `Srsgui` is a simple framework:
 
-   - To define instrument classes for instruments that use remote communication,
-     based on the `Instrument` class and the communication `Interface` class. 
+   - To define instrument classes for instruments that use remote communication, based on the 
+     [`Instrument`](https://thinksrs.github.io/srsgui/srsgui.inst.html#module-srsgui.inst.instrument) 
+     class and the communication 
+     [`Interface`](https://thinksrs.github.io/srsgui/srsgui.inst.communications.html) classes. 
      (By default, serial and TCPIP is available. VXI11, GPIB and USB-TMC are optional).
 
-   - To write Python scripts (tasks) that run in GUI environment with simple APIs
-     provided in ``Task`` class.
+   - To write Python scripts (tasks) that run in graphic user interface (GUI) environment using simple
+     application programming interfaces (APIs) provided in 
+     [``Task``](https://thinksrs.github.io/srsgui/srsgui.task.html) class.
 
    - To organize instrument classes and task scripts presented in a GUI application
-     using a configuration (.taskconfig) file for a project.
+     using a configuration 
+     [(.taskconfig)](https://thinksrs.github.io/srsgui/create-project.html#populating-the-taskconfig-file)
+     file for a project.
 
 ![screenshot](https://thinksrs.github.io/srsgui/_images/example-screen-capture-2.png " ")
 
 ## Installation
 
-To run ``srsgui`` as an application, create a virtual environment, if necessary, 
+To run ``srsgui`` as an GUI application, create a virtual environment, if necessary, 
 and install using ``pip`` with the `[full]` option:  
 
     python -m pip install srsgui[full]
 
 ``Srsgui`` package has the following 3 main dependencies: 
 [pyserial](https://pypi.org/project/pyserial/), 
 [matplotlib](https://pypi.org/project/matplotlib/) and
-[PySide6](https://pypi.org/project/PySide6/). If the installation above fails, 
+[PySide6](https://pypi.org/project/PySide6/) 
+(or [PySide2](https://pypi.org/project/PySide2/)). If the installation above fails, 
 you have to install the failed pacakge manually. Using a virtual environment will
 eliminate possible conflicts between packages in the main Python installation and 
-the packages. Some Linux distributions offer certain Python packages from their repositories only (i.e. not from ``pip``). 
+the packages. Some Linux distributions offer certain Python packages from their 
+repositories only (not from ``pip``). 
 Run a web search for more information on system-specific installation.   
 
-Once pyserial, matplotlib and PySide6 are installed properly, or if you plan to use `srsgui` for instrument drivers only without GUI support, 
+Once pyserial, matplotlib and PySide6 (or PySide2) are installed properly, or if you plan to use 
+`srsgui` for instrument drivers only without GUI support, 
 you can install ``srsgui`` without the `[full]` option:
 
     python -m pip install srsgui
 
 ## Start ``srsgui`` application
     
 If the Python Script directory is in the PATH environment variable,
@@ -45,22 +53,24 @@
 If the script directory is not in PATH, run the srsgui module with Python. 
 
     python -m srsgui
 
 
 ## Run the example project
 
-By default, the `srsgui` application starts with the project that was running when it was last closed.
+By default, the `srsgui` application starts with the project that was running when it was closed the last time.
  
-To open the **oscilloscope example project** included in the `srsgui` package 
+To open the [**oscilloscope example project**](https://thinksrs.github.io/srsgui/example.html)
+included in the `srsgui` package  
 (if `srsgui` does not start with the example project), select File/Open config, 
-go to the `srsgui` package directory, find the examples directory, and select the `oscilloscope example project.taskconfig` file
-in the example project folder. 
+go to the `srsgui` package directory, find the examples directory, and select the 
+`oscilloscope example project.taskconfig` file in the example project folder. 
 
-You can run the **Plot example** and **FFT of simulated waveform** tasks from the Task menu without any instruments connected.
+You can run the **Plot example** and **FFT of simulated waveform** tasks from 
+the Task menu without any instruments connected.
 
 ## Create a project
 
 `Srsgui` is a framework to help you to write your own instrument-controlling 
 Python scripts and run them from a GUI application. Using its APIs, you can write 
 scripts running in GUI with the same amount of code as writing console-based 
 scripts. For programming using the API, refer to the
```

### Comparing `srsgui-0.4.1/docs/Makefile` & `srsgui-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.4.2/docs/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/cg-terminal-screen-capture.png` & `srsgui-0.4.2/docs/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/connect-dialog-box-capture.png` & `srsgui-0.4.2/docs/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/dock_widget_floating.png` & `srsgui-0.4.2/docs/_static/dock_widget_floating.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/dock_widgets_expanded.png` & `srsgui-0.4.2/docs/_static/dock_widgets_expanded.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/example-screen-capture-1.png` & `srsgui-0.4.2/docs/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/example-screen-capture-2.png` & `srsgui-0.4.2/docs/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/initial-screen-capture.png` & `srsgui-0.4.2/docs/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/lockin-capture.png` & `srsgui-0.4.2/docs/_static/lockin-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.4.2/docs/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/second-task-screen-capture.png` & `srsgui-0.4.2/docs/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/task_selection.png` & `srsgui-0.4.2/docs/_static/task_selection.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/terminal-with-example-2.png` & `srsgui-0.4.2/docs/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/_static/terminal-with-example.png` & `srsgui-0.4.2/docs/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/application.rst` & `srsgui-0.4.2/docs/application.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/changelog.rst` & `srsgui-0.4.2/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/conf.py` & `srsgui-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/create-project.rst` & `srsgui-0.4.2/docs/create-project.rst`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,16 @@
 .. code-block::
 
     name: Srsgui Example - Oscilloscope and Clock Generator
 
     inst: cg,  instruments.cg635,   CG635
     inst: osc, instruments.sds1202, SDS1202
 
-    task: *IDN test,    tasks.first,  FirstTask
-    task: Plot example, tasks.second, SecondTask
+    task: *IDN test,    tasks.identify,  Identify
+    task: Plot example, tasks.plot_example, PlotExample
     ...
 
 
 The keyword `name:` is used as
 
     - The title of the SRSGUI application main window (see the top of
       this :ref:`screen capture <top-of-screen-capture-1>`).
```

### Comparing `srsgui-0.4.1/docs/create-task.rst` & `srsgui-0.4.2/docs/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/define-instrument.rst` & `srsgui-0.4.2/docs/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/example.rst` & `srsgui-0.4.2/docs/example.rst`

 * *Files 2% similar despite different names*

```diff
@@ -135,905 +135,916 @@
 00000860: 616d 706c 6520 7072 6f6a 6563 7420 6469  ample project di
 00000870: 7265 6374 6f72 790d 0a20 2020 2020 2020  rectory..       
 00000880: 202f 696e 7374 7275 6d65 6e74 730d 0a20   /instruments.. 
 00000890: 2020 2020 2020 2020 2020 2063 6736 3335             cg635
 000008a0: 2e70 790d 0a20 2020 2020 2020 2020 2020  .py..           
 000008b0: 2073 6473 3132 3032 2e70 790d 0a20 2020   sds1202.py..   
 000008c0: 2020 2020 202f 7461 736b 730d 0a20 2020       /tasks..   
-000008d0: 2020 2020 2020 2020 2066 6972 7374 2e70           first.p
-000008e0: 790d 0a20 2020 2020 2020 2020 2020 2073  y..            s
-000008f0: 6563 6f6e 642e 7079 0d0a 2020 2020 2020  econd.py..      
-00000900: 2020 2020 2020 2e2e 2e0d 0a0d 0a20 2020        .......   
-00000910: 2020 2020 206f 7363 696c 6c6f 7363 6f70       oscilloscop
-00000920: 6520 6578 616d 706c 6520 7072 6f6a 6563  e example projec
-00000930: 742e 7461 736b 636f 6e66 6967 0d0a 0d0a  t.taskconfig....
-00000940: 5468 6973 2066 696c 6520 7374 7275 6374  This file struct
-00000950: 7572 6520 666f 6c6c 6f77 7320 7468 6520  ure follows the 
-00000960: 6775 6964 656c 696e 6520 6465 7363 7269  guideline descri
-00000970: 6265 6420 696e 0d0a 3a72 6566 3a60 4372  bed in..:ref:`Cr
-00000980: 6561 7469 6e67 2066 696c 6520 7374 7275  eating file stru
-00000990: 6374 7572 6520 666f 7220 6120 7072 6f6a  cture for a proj
-000009a0: 6563 7460 2e0d 0a57 6520 6861 7665 2074  ect`...We have t
-000009b0: 776f 2069 6e73 7472 756d 656e 7420 6472  wo instrument dr
-000009c0: 6976 6572 2073 6372 6970 7473 2066 6f72  iver scripts for
-000009d0: 2053 4453 3132 3032 5845 5f20 616e 6420   SDS1202XE_ and 
-000009e0: 4347 3633 355f 0d0a 696e 2074 6865 2073  CG635_..in the s
-000009f0: 7562 6469 7265 6374 6f72 7920 6361 6c6c  ubdirectory call
-00000a00: 6564 202a 2a69 6e73 7472 756d 656e 7473  ed **instruments
-00000a10: 2a2a 2c20 6669 7665 2074 6173 6b20 7363  **, five task sc
-00000a20: 7269 7074 730d 0a69 6e20 7468 6520 7375  ripts..in the su
-00000a30: 6264 6972 6563 746f 7279 2063 616c 6c65  bdirectory calle
-00000a40: 6420 2a2a 7461 736b 732a 2a2c 2070 6c75  d **tasks**, plu
-00000a50: 7320 6120 636f 6e66 6967 7572 6174 696f  s a configuratio
-00000a60: 6e20 6669 6c65 0d0a 696e 2074 6865 2070  n file..in the p
-00000a70: 726f 6a65 6374 2072 6f6f 7420 6469 7265  roject root dire
-00000a80: 6374 6f72 792e 0d0a 0d0a 5072 6f6a 6563  ctory.....Projec
-00000a90: 7420 636f 6e66 6967 7572 6174 696f 6e20  t configuration 
-00000aa0: 6669 6c65 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d  file..----------
+000008d0: 2020 2020 2020 2020 2069 6465 6e74 6966           identif
+000008e0: 792e 7079 0d0a 2020 2020 2020 2020 2020  y.py..          
+000008f0: 2020 706c 6f74 5f65 7861 6d70 6c65 2e70    plot_example.p
+00000900: 790d 0a20 2020 2020 2020 2020 2020 202e  y..            .
+00000910: 2e2e 0d0a 0d0a 2020 2020 2020 2020 6f73  ......        os
+00000920: 6369 6c6c 6f73 636f 7065 2065 7861 6d70  cilloscope examp
+00000930: 6c65 2070 726f 6a65 6374 2e74 6173 6b63  le project.taskc
+00000940: 6f6e 6669 670d 0a0d 0a54 6869 7320 6669  onfig....This fi
+00000950: 6c65 2073 7472 7563 7475 7265 2066 6f6c  le structure fol
+00000960: 6c6f 7773 2074 6865 2067 7569 6465 6c69  lows the guideli
+00000970: 6e65 2064 6573 6372 6962 6564 2069 6e0d  ne described in.
+00000980: 0a3a 7265 663a 6043 7265 6174 696e 6720  .:ref:`Creating 
+00000990: 6669 6c65 2073 7472 7563 7475 7265 2066  file structure f
+000009a0: 6f72 2061 2070 726f 6a65 6374 602e 0d0a  or a project`...
+000009b0: 5765 2068 6176 6520 7477 6f20 696e 7374  We have two inst
+000009c0: 7275 6d65 6e74 2064 7269 7665 7220 7363  rument driver sc
+000009d0: 7269 7074 7320 666f 7220 5344 5331 3230  ripts for SDS120
+000009e0: 3258 455f 2061 6e64 2043 4736 3335 5f0d  2XE_ and CG635_.
+000009f0: 0a69 6e20 7468 6520 7375 6264 6972 6563  .in the subdirec
+00000a00: 746f 7279 2063 616c 6c65 6420 2a2a 696e  tory called **in
+00000a10: 7374 7275 6d65 6e74 732a 2a2c 2066 6976  struments**, fiv
+00000a20: 6520 7461 736b 2073 6372 6970 7473 0d0a  e task scripts..
+00000a30: 696e 2074 6865 2073 7562 6469 7265 6374  in the subdirect
+00000a40: 6f72 7920 6361 6c6c 6564 202a 2a74 6173  ory called **tas
+00000a50: 6b73 2a2a 2c20 706c 7573 2061 2063 6f6e  ks**, plus a con
+00000a60: 6669 6775 7261 7469 6f6e 2066 696c 650d  figuration file.
+00000a70: 0a69 6e20 7468 6520 7072 6f6a 6563 7420  .in the project 
+00000a80: 726f 6f74 2064 6972 6563 746f 7279 2e0d  root directory..
+00000a90: 0a0d 0a50 726f 6a65 6374 2063 6f6e 6669  ...Project confi
+00000aa0: 6775 7261 7469 6f6e 2066 696c 650d 0a2d  guration file..-
 00000ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000ac0: 2d2d 2d0d 0a0d 0a54 6865 2073 7472 7563  ---....The struc
-00000ad0: 7475 7265 206f 6620 6120 2e74 6173 6b63  ture of a .taskc
-00000ae0: 6f6e 6669 6720 6669 6c65 2069 7320 7369  onfig file is si
-00000af0: 6d70 6c65 2061 6e64 0d0a 6578 706c 6169  mple and..explai
-00000b00: 6e65 6420 696e 203a 7265 663a 6050 6f70  ned in :ref:`Pop
-00000b10: 756c 6174 696e 6720 7468 6520 2e74 6173  ulating the .tas
-00000b20: 6b63 6f6e 6669 6720 6669 6c65 600d 0a0d  kconfig file`...
-00000b30: 0a2e 2e20 636f 6465 2d62 6c6f 636b 3a3a  ... code-block::
-00000b40: 0d0a 2020 2020 3a6c 696e 656e 6f73 3a0d  ..    :linenos:.
-00000b50: 0a0d 0a20 2020 206e 616d 653a 2053 7273  ...    name: Srs
-00000b60: 6775 6920 4578 616d 706c 6520 2d20 4f73  gui Example - Os
-00000b70: 6369 6c6c 6f73 636f 7065 2061 6e64 2043  cilloscope and C
-00000b80: 6c6f 636b 2047 656e 6572 6174 6f72 0d0a  lock Generator..
-00000b90: 0d0a 2020 2020 696e 7374 3a20 6367 2c20  ..    inst: cg, 
-00000ba0: 2069 6e73 7472 756d 656e 7473 2e63 6736   instruments.cg6
-00000bb0: 3335 2c20 2020 4347 3633 350d 0a20 2020  35,   CG635..   
-00000bc0: 2069 6e73 743a 206f 7363 2c20 696e 7374   inst: osc, inst
-00000bd0: 7275 6d65 6e74 732e 7364 7331 3230 322c  ruments.sds1202,
-00000be0: 2053 4453 3132 3032 0d0a 0d0a 2020 2020   SDS1202....    
-00000bf0: 7461 736b 3a20 2a49 444e 2074 6573 742c  task: *IDN test,
-00000c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c10: 2074 6173 6b73 2e66 6972 7374 2c20 2046   tasks.first,  F
-00000c20: 6972 7374 5461 736b 0d0a 2020 2020 7461  irstTask..    ta
-00000c30: 736b 3a20 506c 6f74 2065 7861 6d70 6c65  sk: Plot example
-00000c40: 2c20 2020 2020 2020 2020 2020 2020 2074  ,              t
-00000c50: 6173 6b73 2e73 6563 6f6e 642c 2053 6563  asks.second, Sec
-00000c60: 6f6e 6454 6173 6b0d 0a20 2020 202e 2e2e  ondTask..    ...
-00000c70: 0d0a 0d0a 496e 7374 7275 6d65 6e74 2064  ....Instrument d
-00000c80: 7269 7665 7273 0d0a 2d2d 2d2d 2d2d 2d2d  rivers..--------
-00000c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a  ------------....
-00000ca0: 4347 3633 350d 0a5e 5e5e 5e5e 0d0a 0d0a  CG635..^^^^^....
-00000cb0: 4c65 7427 7320 7461 6b65 2061 206c 6f6f  Let's take a loo
-00000cc0: 6b20 696e 746f 2074 6865 2060 696e 7374  k into the `inst
-00000cd0: 7275 6d65 6e74 732f 6367 3633 352e 7079  ruments/cg635.py
-00000ce0: 6020 6d6f 6475 6c65 2e20 4576 656e 2074  ` module. Even t
-00000cf0: 686f 7567 6820 6974 2073 6565 6d73 206c  hough it seems l
-00000d00: 6f6e 672c 0d0a 6974 2068 6173 206f 6e6c  ong,..it has onl
-00000d10: 7920 3520 6c69 6e65 7320 6f66 206e 6f6e  y 5 lines of non
-00000d20: 2d63 6f6d 6d65 6e74 2063 6f64 652e 2049  -comment code. I
-00000d30: 6620 796f 7520 6861 7665 2061 2043 4736  f you have a CG6
-00000d40: 3335 2c0d 0a63 6f6e 6772 6174 756c 6174  35,..congratulat
-00000d50: 696f 6e73 2120 596f 7520 6361 6e20 7573  ions! You can us
-00000d60: 6520 7468 6520 6669 6c65 2061 7320 6973  e the file as is
-00000d70: 2e20 4966 2079 6f75 2068 6176 6520 616e  . If you have an
-00000d80: 7920 6675 6e63 7469 6f6e 0d0a 6765 6e65  y function..gene
-00000d90: 7261 746f 7220 7468 6174 2063 616e 2063  rator that can c
-00000da0: 6861 6e67 6520 7468 6520 6f75 7470 7574  hange the output
-00000db0: 2066 7265 7175 656e 6379 2c20 796f 7520   frequency, you 
-00000dc0: 6361 6e20 7573 6520 6974 2069 6e73 7465  can use it inste
-00000dd0: 6164 206f 6620 7468 6520 4347 3633 350d  ad of the CG635.
-00000de0: 0a69 6e20 7468 6520 6578 616d 706c 652e  .in the example.
-00000df0: 2059 6f75 2063 6861 6e67 6520 7468 6520   You change the 
-00000e00: 636c 6173 7320 6e61 6d65 2061 6e64 205f  class name and _
-00000e10: 4964 5374 7269 6e67 2074 6f20 6d61 7463  IdString to matc
-00000e20: 6820 7468 6520 696e 7374 7275 6d65 6e74  h the instrument
-00000e30: 206e 616d 652c 0d0a 616c 6f6e 6720 7769   name,..along wi
-00000e40: 7468 205f 7465 726d 5f63 6861 722e 204c  th _term_char. L
-00000e50: 6f6f 6b20 7570 2074 6865 2063 6f6d 6d61  ook up the comma
-00000e60: 6e64 2074 6f20 6368 616e 6765 2066 7265  nd to change fre
-00000e70: 7175 656e 6379 2c20 7265 6665 7272 696e  quency, referrin
-00000e80: 6720 746f 2074 6865 206d 616e 7561 6c2e  g to the manual.
-00000e90: 0d0a 5361 7665 2074 6865 202e 7079 2066  ..Save the .py f
-00000ea0: 696c 6520 7769 7468 2061 2028 6469 6666  ile with a (diff
-00000eb0: 6572 656e 7429 2061 7070 726f 7072 6961  erent) appropria
-00000ec0: 7465 2066 696c 656e 616d 652e 2043 6861  te filename. Cha
-00000ed0: 6e67 6520 7468 6520 6069 6e73 743a 6020  nge the `inst:` 
-00000ee0: 6c69 6e65 2066 6f72 2060 6367 600d 0a69  line for `cg`..i
-00000ef0: 6e20 7468 6520 2e74 6173 6b63 6f6e 6669  n the .taskconfi
-00000f00: 6720 6669 6c65 2074 6f20 6d61 7463 6820  g file to match 
-00000f10: 7468 6520 6d6f 6475 6c65 2070 6174 6820  the module path 
-00000f20: 616e 6420 7468 6520 636c 6173 7320 6e61  and the class na
-00000f30: 6d65 2074 6861 7420 796f 7520 6372 6561  me that you crea
-00000f40: 7465 642e 0d0a 0d0a 2e2e 2063 6f64 652d  ted....... code-
-00000f50: 626c 6f63 6b3a 3a0d 0a20 2020 203a 6c69  block::..    :li
-00000f60: 6e65 6e6f 733a 0d0a 0d0a 2020 2020 6672  nenos:....    fr
-00000f70: 6f6d 2073 7273 6775 6920 696d 706f 7274  om srsgui import
-00000f80: 2049 6e73 7472 756d 656e 740d 0a20 2020   Instrument..   
-00000f90: 2066 726f 6d20 7372 7367 7569 2e69 6e73   from srsgui.ins
-00000fa0: 7420 696d 706f 7274 2046 6c6f 6174 436f  t import FloatCo
-00000fb0: 6d6d 616e 640d 0a0d 0a20 2020 2063 6c61  mmand....    cla
-00000fc0: 7373 2043 4736 3335 2849 6e73 7472 756d  ss CG635(Instrum
-00000fd0: 656e 7429 3a0d 0a20 2020 2020 2020 205f  ent):..        _
-00000fe0: 4964 5374 7269 6e67 203d 2027 4347 3633  IdString = 'CG63
-00000ff0: 3527 0d0a 2020 2020 2020 2020 6672 6571  5'..        freq
-00001000: 7565 6e63 7920 3d20 466c 6f61 7443 6f6d  uency = FloatCom
-00001010: 6d61 6e64 2827 4652 4551 2729 0d0a 0d0a  mand('FREQ')....
-00001020: 5769 7468 6f75 7420 7265 6465 6669 6e69  Without redefini
-00001030: 6e67 202a 2a61 7661 696c 6162 6c65 5f69  ng **available_i
-00001040: 6e74 6572 6661 6365 732a 2a20 636c 6173  nterfaces** clas
-00001050: 7320 6174 7472 6962 7574 652c 2079 6f75  s attribute, you
-00001060: 2063 616e 2075 7365 2073 6572 6961 6c0d   can use serial.
-00001070: 0a63 6f6d 6d75 6e69 6361 7469 6f6e 206f  .communication o
-00001080: 6e6c 792e 2049 6620 796f 7520 7761 6e74  nly. If you want
-00001090: 2074 6f20 7573 6520 4750 4942 2063 6f6d   to use GPIB com
-000010a0: 6d75 6e69 6361 7469 6f6e 2c20 796f 7520  munication, you 
-000010b0: 6861 7665 2074 6f20 756e 2d63 6f6d 6d65  have to un-comme
-000010c0: 6e74 2074 6865 0d0a 2a2a 6176 6169 6c61  nt the..**availa
-000010d0: 626c 655f 696e 7465 7266 6163 6573 2a2a  ble_interfaces**
-000010e0: 2069 6e20 4347 3633 3520 636c 6173 732e   in CG635 class.
-000010f0: 0d0a 0d0a 2e2e 2063 6f64 652d 626c 6f63  ...... code-bloc
-00001100: 6b3a 3a0d 0a0d 0a20 2020 2066 726f 6d20  k::....    from 
-00001110: 7372 7367 7569 2069 6d70 6f72 7420 5365  srsgui import Se
-00001120: 7269 616c 496e 7465 7266 6163 652c 2046  rialInterface, F
-00001130: 696e 644c 6973 7449 6e70 7574 0d0a 2020  indListInput..  
-00001140: 2020 6672 6f6d 2073 7273 696e 7374 2e73    from srsinst.s
-00001150: 7238 3630 2069 6d70 6f72 7420 5669 7361  r860 import Visa
-00001160: 496e 7465 7266 6163 650d 0a0d 0a20 2020  Interface....   
-00001170: 2061 7661 696c 6162 6c65 5f69 6e74 6572   available_inter
-00001180: 6661 6365 7320 3d20 5b0d 0a20 2020 2020  faces = [..     
-00001190: 2020 205b 2020 2053 6572 6961 6c49 6e74     [   SerialInt
-000011a0: 6572 6661 6365 2c0d 0a20 2020 2020 2020  erface,..       
-000011b0: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
-000011c0: 2020 2020 2020 2020 2743 4f4d 2070 6f72          'COM por
-000011d0: 7427 3a20 4669 6e64 4c69 7374 496e 7075  t': FindListInpu
-000011e0: 7428 292c 0d0a 2020 2020 2020 2020 2020  t(),..          
-000011f0: 2020 2020 2020 2762 6175 6420 7261 7465        'baud rate
-00001200: 273a 2039 3630 300d 0a20 2020 2020 2020  ': 9600..       
-00001210: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00001220: 5d2c 0d0a 2020 2020 2020 2020 5b20 2020  ],..        [   
-00001230: 5669 7361 496e 7465 7266 6163 652c 0d0a  VisaInterface,..
-00001240: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
-00001250: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00001260: 7265 736f 7572 6365 273a 2046 696e 644c  resource': FindL
-00001270: 6973 7449 6e70 7574 2829 2c0d 0a20 2020  istInput(),..   
-00001280: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00001290: 2020 2020 5d2c 0d0a 2020 2020 5d0d 0a0d      ],..    ]...
-000012a0: 0a59 6f75 206d 7573 7420 696e 7374 616c  .You must instal
-000012b0: 6c20 6073 7273 696e 7374 2e73 7238 3630  l `srsinst.sr860
-000012c0: 605f 2066 6f72 2056 6973 6149 6e74 6572  `_ for VisaInter
-000012d0: 6661 6365 2063 6c61 7373 2c20 616e 6420  face class, and 
-000012e0: 5079 5649 5341 5f20 616e 640d 0a69 7473  PyVISA_ and..its
-000012f0: 2062 6163 6b65 6e64 206c 6962 7261 7279   backend library
-00001300: 2c20 666f 6c6c 6f77 696e 6720 5079 5669  , following PyVi
-00001310: 7361 2069 6e73 7461 6c6c 6174 696f 6e20  sa installation 
-00001320: 696e 7374 7275 6374 696f 6e2e 0d0a 0d0a  instruction.....
-00001330: 4f6e 6365 2074 6865 2043 4736 3335 2028  Once the CG635 (
-00001340: 6f72 2079 6f75 7220 6675 6e63 7469 6f6e  or your function
-00001350: 2067 656e 6572 6174 6f72 2920 6973 2063   generator) is c
-00001360: 6f6e 6e65 6374 6564 2c20 0d0a 796f 7520  onnected, ..you 
-00001370: 7769 6c6c 2073 6565 2074 6865 2063 6f6e  will see the con
-00001380: 6e65 6374 696f 6e20 696e 666f 726d 6174  nection informat
-00001390: 696f 6e20 696e 2074 6865 2069 6e73 7472  ion in the instr
-000013a0: 756d 656e 7420 696e 666f 2070 616e 656c  ument info panel
-000013b0: 2c0d 0a61 6e64 2079 6f75 2063 616e 2075  ,..and you can u
-000013c0: 7365 2069 7420 696e 2074 6865 2074 6572  se it in the ter
-000013d0: 6d69 6e61 6c2c 2061 7320 7368 6f77 6e20  minal, as shown 
-000013e0: 6265 6c6f 772e 0d0a 0d0a 2e2e 2066 6967  below....... fig
-000013f0: 7572 653a 3a20 2e2f 5f73 7461 7469 632f  ure:: ./_static/
-00001400: 6367 2d74 6572 6d69 6e61 6c2d 7363 7265  cg-terminal-scre
-00001410: 656e 2d63 6170 7475 7265 2e70 6e67 0d0a  en-capture.png..
-00001420: 2020 2020 3a61 6c69 676e 3a20 6365 6e74      :align: cent
-00001430: 6572 0d0a 2020 2020 3a66 6967 636c 6173  er..    :figclas
-00001440: 733a 2061 6c69 676e 2d63 656e 7465 720d  s: align-center.
-00001450: 0a0d 0a7c 0d0a 0d0a 546f 2066 6978 2074  ...|....To fix t
-00001460: 6865 2027 4e6f 7420 696d 706c 656d 656e  he 'Not implemen
-00001470: 7465 6427 2077 6172 6e69 6e67 2c0d 0a3a  ted' warning,..:
-00001480: 6d65 7468 3a60 496e 7374 7275 6d65 6e74  meth:`Instrument
-00001490: 2e67 6574 5f73 7461 7475 7328 2920 3c73  .get_status() <s
-000014a0: 7273 6775 692e 696e 7374 2e69 6e73 7472  rsgui.inst.instr
-000014b0: 756d 656e 742e 496e 7374 7275 6d65 6e74  ument.Instrument
-000014c0: 2e67 6574 5f73 7461 7475 733e 600d 0a6e  .get_status>`..n
-000014d0: 6565 6473 2074 6f20 6265 2072 6564 6566  eeds to be redef
-000014e0: 696e 6564 2e20 0d0a 466f 7220 6578 616d  ined. ..For exam
-000014f0: 706c 652c 2077 6520 6361 6e20 6f76 6572  ple, we can over
-00001500: 7269 6465 2069 7420 6173 2066 6f6c 6c6f  ride it as follo
-00001510: 7769 6e67 3a0d 0a0d 0a2e 2e20 636f 6465  wing:...... code
-00001520: 2d62 6c6f 636b 3a3a 0d0a 0d0a 2020 2020  -block::....    
-00001530: 6465 6620 6765 745f 7374 6174 7573 2873  def get_status(s
-00001540: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00001550: 6574 7572 6e20 2753 7461 7475 733a 204f  eturn 'Status: O
-00001560: 4b27 0d0a 0d0a 2849 6620 796f 7520 6172  K'....(If you ar
-00001570: 6520 6661 6d69 6c69 6172 2077 6974 6820  e familiar with 
-00001580: 7374 6174 7573 2062 7974 6573 2c20 796f  status bytes, yo
-00001590: 7520 6361 6e20 6f76 6572 7269 6465 2074  u can override t
-000015a0: 6865 2060 6765 745f 7374 6174 7573 6020  he `get_status` 
-000015b0: 6d65 7468 6f64 0d0a 746f 2071 7565 7279  method..to query
-000015c0: 2074 6865 2073 7461 7475 7320 6279 7465   the status byte
-000015d0: 2873 2920 616e 6420 7265 7475 726e 2074  (s) and return t
-000015e0: 6865 2072 656c 6576 616e 7420 7374 6174  he relevant stat
-000015f0: 7573 2069 6e66 6f72 6d61 7469 6f6e 2061  us information a
-00001600: 7320 796f 7520 6465 7369 7265 2e29 0d0a  s you desire.)..
-00001610: 0d0a 5765 2077 696c 6c20 7573 6520 6f6e  ..We will use on
-00001620: 6c79 206f 6e65 2063 6f6d 6d61 6e64 205c  ly one command \
-00001630: 2e66 7265 7175 656e 6379 2c20 6f72 2069  .frequency, or i
-00001640: 7473 2072 6177 2072 656d 6f74 6520 636f  ts raw remote co
-00001650: 6d6d 616e 642c 2027 6672 6571 2720 696e  mmand, 'freq' in
-00001660: 2074 6869 7320 6578 616d 706c 652e 0d0a   this example...
-00001670: 4265 6361 7573 6520 2763 6727 2069 7320  Because 'cg' is 
-00001680: 7468 6520 6465 6661 756c 7420 696e 7374  the default inst
-00001690: 7275 6d65 6e74 2028 7468 6520 6669 7273  rument (the firs
-000016a0: 7420 696e 7374 7275 6d65 6e74 206d 656e  t instrument men
-000016b0: 7469 6f6e 6564 2069 6e20 7468 6520 2e74  tioned in the .t
-000016c0: 6173 6b63 6f6e 6669 6720 6669 6c65 292c  askconfig file),
-000016d0: 0d0a 616e 7920 7261 7720 7265 6d6f 7465  ..any raw remote
-000016e0: 2063 6f6d 6d61 6e64 2077 6974 686f 7574   command without
-000016f0: 2074 6865 2027 6367 3a27 2070 7265 6669   the 'cg:' prefi
-00001700: 7820 7769 6c6c 2062 6520 7365 6e74 2074  x will be sent t
-00001710: 6f20 6974 2e0d 0a42 6f74 6820 275c 2a69  o it...Both '\*i
-00001720: 646e 3f27 2061 6e64 2027 6367 3a5c 2a69  dn?' and 'cg:\*i
-00001730: 646e 3f27 2077 696c 6c20 7265 7475 726e  dn?' will return
-00001740: 2074 6865 2073 616d 6520 7265 706c 792e   the same reply.
-00001750: 0d0a 0d0a 5765 2075 7365 2074 6865 2070  ....We use the p
-00001760: 7265 6669 7820 2763 673a 2720 666f 7220  refix 'cg:' for 
-00001770: 7261 7720 7265 6d6f 7465 2063 6f6d 6d61  raw remote comma
-00001780: 6e64 2061 6e64 2074 6865 2070 7265 6669  nd and the prefi
-00001790: 7820 2763 672e 2720 666f 7220 5079 7468  x 'cg.' for Pyth
-000017a0: 6f6e 2063 6f6d 6d61 6e64 732e 0d0a 496e  on commands...In
-000017b0: 2074 6865 2074 6572 6d69 6e61 6c20 616c   the terminal al
-000017c0: 6c20 6174 7472 6962 7574 6573 2061 6e64  l attributes and
-000017d0: 206d 6574 686f 6473 206f 6620 4347 3833   methods of CG83
-000017e0: 3520 636c 6173 7320 6361 6e20 6265 2075  5 class can be u
-000017f0: 7365 6420 7769 7468 2070 7265 6669 7820  sed with prefix 
-00001800: 2763 672e 272e 0d0a 4265 6361 7573 6520  'cg.'...Because 
-00001810: 7765 2064 6566 696e 6564 2066 7265 7175  we defined frequ
-00001820: 656e 6379 2061 7320 6120 466c 6f61 7443  ency as a FloatC
-00001830: 6f6d 6d61 6e64 2c20 7765 2063 616e 2061  ommand, we can a
-00001840: 6c73 6f20 7573 6520 7468 6520 2763 672e  lso use the 'cg.
-00001850: 6672 6571 7565 6e63 7927 2070 726f 7065  frequency' prope
-00001860: 7274 7920 696e 2074 6865 0d0a 7465 726d  rty in the..term
-00001870: 696e 616c 2e20 5468 6973 206d 6561 6e73  inal. This means
-00001880: 2074 6861 7420 7468 6520 666f 6c6c 6f77   that the follow
-00001890: 696e 6720 6172 6520 6571 7569 7661 6c65  ing are equivale
-000018a0: 6e74 3a0d 0a2d 2060 6367 3a66 7265 7120  nt:..- `cg:freq 
-000018b0: 3130 302e 3060 0d0a 2d20 6063 672e 6672  100.0`..- `cg.fr
-000018c0: 6571 7565 6e63 7920 3130 3060 0d0a 2020  equency 100`..  
-000018d0: 0d0a 4675 7274 6865 726d 6f72 652c 2066  ..Furthermore, f
-000018e0: 726f 6d20 6120 5079 7468 6f6e 2073 6372  rom a Python scr
-000018f0: 6970 742c 206f 6e63 6520 6067 6574 5f69  ipt, once `get_i
-00001900: 6e73 7472 756d 656e 7428 2763 6727 2960  nstrument('cg')`
-00001910: 2068 6173 2062 6565 6e20 6361 6c6c 6564   has been called
-00001920: 2069 6e20 6120 7461 736b 2063 6c61 7373   in a task class
-00001930: 2c0d 0a79 6f75 2063 616e 2075 7365 2060  ,..you can use `
-00001940: 6367 2e66 7265 7175 656e 6379 203d 2031  cg.frequency = 1
-00001950: 3030 6020 696e 2074 6865 2050 7974 686f  00` in the Pytho
-00001960: 6e20 7461 736b 2063 6f64 6520 286f 7220  n task code (or 
-00001970: 6063 672e 6672 6571 7565 6e63 7960 2061  `cg.frequency` a
-00001980: 7320 7468 6520 7175 6572 7920 666f 726d  s the query form
-00001990: 292e 0d0a 0d0a 4163 7475 616c 6c79 2079  ).....Actually y
-000019a0: 6f75 2063 616e 2075 7365 2061 6c6c 2074  ou can use all t
-000019b0: 6865 2061 7474 7269 6275 7465 7320 616e  he attributes an
-000019c0: 6420 6d65 7468 6f64 7320 6465 6669 6e65  d methods define
-000019d0: 6420 696e 2074 6865 2043 4736 3335 2063  d in the CG635 c
-000019e0: 6c61 7373 2061 6e64 2069 7473 2073 7570  lass and its sup
-000019f0: 6572 2063 6c61 7373 6573 2e0d 0a54 6865  er classes...The
-00001a00: 2060 6367 2e64 6972 2829 6020 6d65 7468   `cg.dir()` meth
-00001a10: 6f64 2028 7768 6572 6520 6064 6972 2829  od (where `dir()
-00001a20: 6020 6973 2064 6566 696e 6564 2069 6e20  ` is defined in 
-00001a30: 3a63 6c61 7373 3a60 436f 6d70 6f6e 656e  :class:`Componen
-00001a40: 7420 3c73 7273 6775 692e 696e 7374 2e63  t <srsgui.inst.c
-00001a50: 6f6d 706f 6e65 6e74 2e43 6f6d 706f 6e65  omponent.Compone
-00001a60: 6e74 3e60 2063 6c61 7373 290d 0a73 686f  nt>` class)..sho
-00001a70: 7773 2061 6c6c 2074 6865 2061 7661 696c  ws all the avail
-00001a80: 6162 6c65 2063 6f6d 706f 6e65 6e74 732c  able components,
-00001a90: 2063 6f6d 6d61 6e64 732c 2061 6e64 206d   commands, and m
-00001aa0: 6574 686f 6473 2061 7661 696c 6162 6c65  ethods available
-00001ab0: 2074 6f20 616e 2069 6e73 7461 6e63 6520   to an instance 
-00001ac0: 6f66 2074 6865 2043 4736 3335 2063 6c61  of the CG635 cla
-00001ad0: 7373 2e20 0d0a 5468 6973 2068 656c 7073  ss. ..This helps
-00001ae0: 2075 7320 746f 206e 6176 6967 6174 6520   us to navigate 
-00001af0: 7468 726f 7567 6820 7265 736f 7572 6365  through resource
-00001b00: 7320 6176 6169 6c61 626c 6520 7769 7468  s available with
-00001b10: 2074 6865 2063 6c61 7373 2e0d 0a0d 0a2e   the class......
-00001b20: 2e20 6669 6775 7265 3a3a 202e 2f5f 7374  . figure:: ./_st
-00001b30: 6174 6963 2f63 672d 6469 722d 7465 726d  atic/cg-dir-term
-00001b40: 696e 616c 2d73 6372 6565 6e2d 6361 7074  inal-screen-capt
-00001b50: 7572 652e 706e 670d 0a20 2020 203a 616c  ure.png..    :al
-00001b60: 6967 6e3a 2063 656e 7465 720d 0a20 2020  ign: center..   
-00001b70: 203a 6669 6763 6c61 7373 3a20 616c 6967   :figclass: alig
-00001b80: 6e2d 6365 6e74 6572 0d0a 0d0a 0d0a 4372  n-center......Cr
-00001b90: 6163 6b69 6e67 206f 7065 6e20 7468 6520  acking open the 
-00001ba0: 696e 7374 7275 6d65 6e74 206d 616e 7561  instrument manua
-00001bb0: 6c20 616e 6420 6465 6669 6e69 6e67 2075  l and defining u
-00001bc0: 7365 6675 6c20 6d65 7468 6f64 7320 696e  seful methods in
-00001bd0: 2061 6e20 696e 7374 7275 6d65 6e74 2063   an instrument c
-00001be0: 6c61 7373 200d 0a70 726f 7669 6465 7320  lass ..provides 
-00001bf0: 6561 7365 206f 6620 696e 7374 7275 6d65  ease of instrume
-00001c00: 6e74 2063 6f6e 7472 6f6c 2066 726f 6d20  nt control from 
-00001c10: 6569 7468 6572 2074 6865 2054 6572 6d69  either the Termi
-00001c20: 6e61 6c20 6f72 2066 726f 6d20 796f 7572  nal or from your
-00001c30: 2074 6173 6b20 636f 6465 2c20 0d0a 7769   task code, ..wi
-00001c40: 7468 6f75 7420 6861 7669 6e67 2074 6f20  thout having to 
-00001c50: 7265 6d65 6d62 6572 2074 6865 2072 656d  remember the rem
-00001c60: 6f74 6520 636f 6d6d 616e 6420 6d6e 656d  ote command mnem
-00001c70: 6f6e 6963 7320 7468 656d 7365 6c76 6573  onics themselves
-00001c80: 2e20 0d0a 0d0a 5344 5331 3230 320d 0a5e  . ....SDS1202..^
-00001c90: 5e5e 5e5e 5e5e 0d0a 0d0a 4576 656e 2074  ^^^^^^....Even t
-00001ca0: 686f 7567 6820 796f 7520 6d61 7920 6e6f  hough you may no
-00001cb0: 7420 6861 7665 2061 6e20 5344 5331 3230  t have an SDS120
-00001cc0: 3220 6f73 6369 6c6c 6f73 636f 7065 2074  2 oscilloscope t
-00001cd0: 6861 7420 4920 6861 7070 656e 6564 0d0a  hat I happened..
-00001ce0: 746f 2075 7365 2066 6f72 2074 6869 7320  to use for this 
-00001cf0: 6578 616d 706c 652c 2049 2062 6574 2079  example, I bet y
-00001d00: 6f75 2063 616e 2066 696e 6420 616e 206f  ou can find an o
-00001d10: 7363 696c 6c6f 7363 6f70 6520 736f 6d65  scilloscope some
-00001d20: 7768 6572 650d 0a69 6e20 796f 7572 2062  where..in your b
-00001d30: 7569 6c64 696e 672e 2057 6865 6e20 796f  uilding. When yo
-00001d40: 7520 6765 7420 6120 686f 6c64 206f 6620  u get a hold of 
-00001d50: 6f6e 652c 2069 7420 6d61 7920 6861 7665  one, it may have
-00001d60: 2061 2055 5342 2063 6f6e 6e65 6374 6f72   a USB connector
-00001d70: 206f 6e6c 792c 0d0a 6c69 6b65 2061 206c   only,..like a l
-00001d80: 6f74 206f 6620 6261 7365 206d 6f64 656c  ot of base model
-00001d90: 206f 7363 696c 6c6f 7363 6f70 6573 2064   oscilloscopes d
-00001da0: 6f2e 0d0a 5468 6973 206d 6561 6e73 2079  o...This means y
-00001db0: 6f75 206d 6179 2068 6176 6520 746f 2075  ou may have to u
-00001dc0: 7365 2055 5342 2d54 4d43 2069 6e74 6572  se USB-TMC inter
-00001dd0: 6661 6365 2e20 0d0a 496e 206f 7264 6572  face. ..In order
-00001de0: 2074 6f20 646f 2074 6861 742c 2079 6f75   to do that, you
-00001df0: 206e 6565 6420 746f 2069 6e73 7461 6c6c   need to install
-00001e00: 2050 7956 4953 412e 200d 0a59 6f75 206e   PyVISA. ..You n
-00001e10: 6565 6420 746f 2075 6e63 6f6d 6d65 6e74  eed to uncomment
-00001e20: 2074 6865 2061 7661 696c 6162 6c65 5f69   the available_i
-00001e30: 6e74 6572 6661 6365 7320 6f66 2053 4453  nterfaces of SDS
-00001e40: 3132 3032 2063 6c61 7373 2c20 0d0a 6d6f  1202 class, ..mo
-00001e50: 6469 6679 2069 7420 746f 2066 6974 2074  dify it to fit t
-00001e60: 6865 2073 7065 6369 6669 6361 7469 6f6e  he specification
-00001e70: 206f 6620 796f 7572 206f 7363 696c 6c6f   of your oscillo
-00001e80: 7363 6f70 652c 2061 6c6f 6e67 2077 6974  scope, along wit
-00001e90: 680d 0a63 6861 6e67 696e 6720 746f 2074  h..changing to t
-00001ea0: 6865 2063 6f72 7265 6374 2060 5f49 6453  he correct `_IdS
-00001eb0: 7472 696e 6760 2e20 0d0a 5468 656e 2079  tring`. ..Then y
-00001ec0: 6f75 2068 6176 6520 746f 2067 6574 2077  ou have to get w
-00001ed0: 6176 6566 6f72 6d20 646f 776e 6c6f 6164  aveform download
-00001ee0: 2077 6f72 6b69 6e67 2c20 7768 6963 6820   working, which 
-00001ef0: 6f66 7465 6e20 696e 766f 6c76 6573 2072  often involves r
-00001f00: 6563 6965 7669 6e67 2061 6e64 2070 726f  ecieving and pro
-00001f10: 7065 726c 7920 7061 7273 696e 6720 6269  perly parsing bi
-00001f20: 6e61 7279 2064 6174 610d 0a28 6269 6e61  nary data..(bina
-00001f30: 7279 2064 6174 6120 6973 2075 7365 6420  ry data is used 
-00001f40: 746f 206d 696e 696d 697a 6520 7468 6520  to minimize the 
-00001f50: 6e75 6d62 6572 206f 6620 6368 6172 6163  number of charac
-00001f60: 7465 7273 2073 656e 7420 6f76 6572 2074  ters sent over t
-00001f70: 6865 2072 656d 6f74 6520 636f 6d6d 756e  he remote commun
-00001f80: 6963 6174 696f 6e20 696e 7465 7266 6163  ication interfac
-00001f90: 652c 0d0a 7468 6572 6562 7920 6d61 6b69  e,..thereby maki
-00001fa0: 6e67 2064 6174 6120 7472 616e 7366 6572  ng data transfer
-00001fb0: 7320 6f66 2070 6572 6861 7073 2076 6572  s of perhaps ver
-00001fc0: 7920 6c65 6e67 7468 7920 7761 7665 666f  y lengthy wavefo
-00001fd0: 726d 7320 7265 6c61 7469 7665 6c79 2066  rms relatively f
-00001fe0: 6173 7429 2e0d 0a49 6620 796f 7520 6172  ast)...If you ar
-00001ff0: 6520 6c75 636b 792c 2079 6f75 2063 616e  e lucky, you can
-00002000: 2066 696e 6420 6120 776f 726b 696e 6720   find a working 
-00002010: 5079 7468 6f6e 2073 6e69 7070 6574 2066  Python snippet f
-00002020: 726f 6d20 6a75 6469 6369 6f75 7320 7765  rom judicious we
-00002030: 6220 7365 6172 6368 2e0d 0a49 6620 6e6f  b search...If no
-00002040: 742c 2079 6f75 2068 6176 6520 746f 2064  t, you have to d
-00002050: 6563 6970 6865 7220 7468 6520 7072 6f67  ecipher the prog
-00002060: 7261 6d6d 696e 6720 6d61 6e75 616c 206f  ramming manual o
-00002070: 6620 7468 6520 6f73 6369 6c6c 6f73 636f  f the oscillosco
-00002080: 7065 2e20 0d0a 4974 206d 6179 2074 616b  pe. ..It may tak
-00002090: 6520 7469 6d65 2c20 6275 7420 6974 2077  e time, but it w
-000020a0: 696c 6c20 6265 2076 6572 7920 7265 7761  ill be very rewa
-000020b0: 7264 696e 6720 666f 7220 796f 7572 2064  rding for your d
-000020c0: 6174 6120 6163 7175 6973 6974 696f 6e0d  ata acquisition.
-000020d0: 0a73 6b69 6c6c 2d73 6574 2069 6d70 726f  .skill-set impro
-000020e0: 7665 6d65 6e74 2e0d 0a0d 0a4f 7468 6572  vement.....Other
-000020f0: 2074 6861 6e20 7468 6520 6269 6e61 7279   than the binary
-00002100: 2077 6176 6566 6f72 6d20 646f 776e 6c6f   waveform downlo
-00002110: 6164 2c20 0d0a 6d6f 7374 206f 7468 6572  ad, ..most other
-00002120: 2063 6f6d 6d61 6e64 7320 666f 7220 696e   commands for in
-00002130: 7465 7261 6374 696e 6720 7769 7468 2074  teracting with t
-00002140: 6865 206f 7363 696c 6c6f 7363 6f70 6520  he oscilloscope 
-00002150: 0d0a 7769 6c6c 2062 6520 7374 616e 6461  ..will be standa
-00002160: 7264 2041 5343 4949 2d62 6173 6564 2074  rd ASCII-based t
-00002170: 6578 7420 636f 6d6d 616e 6473 2e0d 0a0d  ext commands....
-00002180: 0a2e 2e20 6e6f 7465 3a3a 0d0a 2020 5769  ... note::..  Wi
-00002190: 7468 2064 6566 6175 6c74 2061 7661 696c  th default avail
-000021a0: 6162 6c65 5f69 6e74 6572 6661 6365 7320  able_interfaces 
-000021b0: 6f66 2049 6e73 7472 756d 656e 7420 636c  of Instrument cl
-000021c0: 6173 732c 2054 6370 6970 496e 7465 7266  ass, TcpipInterf
-000021d0: 6163 6520 7368 6f75 6c64 2062 6520 7573  ace should be us
-000021e0: 6564 2077 6974 6820 706f 7274 2035 3032  ed with port 502
-000021f0: 352e 0d0a 0d0a 5468 6520 696e 7374 7275  5.....The instru
-00002200: 6d65 6e74 2064 7269 7665 7220 666f 7220  ment driver for 
-00002210: 5344 5331 3230 3220 7769 6c6c 2077 6f72  SDS1202 will wor
-00002220: 6b20 7769 7468 2034 206c 696e 6573 206f  k with 4 lines o
-00002230: 6620 636f 6465 2c20 6a75 7374 206c 696b  f code, just lik
-00002240: 6520 7468 6520 4347 3633 352c 0d0a 6265  e the CG635,..be
-00002250: 666f 7265 2061 6464 696e 6720 7468 6520  fore adding the 
-00002260: 6d65 7468 6f64 2074 6f20 646f 776e 6c6f  method to downlo
-00002270: 6164 2077 6176 6566 6f72 6d73 2066 726f  ad waveforms fro
-00002280: 6d20 7468 6520 6f73 6369 6c6c 6f73 636f  m the oscillosco
-00002290: 7065 2e20 0d0a 4164 6420 6174 7472 6962  pe. ..Add attrib
-000022a0: 7574 6573 2061 6e64 206d 6574 686f 6473  utes and methods
-000022b0: 2069 6e63 7265 6d65 6e74 616c 6c79 2061   incrementally a
-000022c0: 7320 796f 7520 6e65 6564 2074 6f20 7573  s you need to us
-000022d0: 6520 6d6f 7265 2066 756e 6374 696f 6e73  e more functions
-000022e0: 206f 6620 7468 6520 696e 7374 7275 6d65   of the instrume
-000022f0: 6e74 2e0d 0a0d 0a2e 2e20 636f 6465 2d62  nt....... code-b
-00002300: 6c6f 636b 3a3a 0d0a 2020 2020 3a6c 696e  lock::..    :lin
-00002310: 656e 6f73 3a0d 0a0d 0a20 2020 2069 6d70  enos:....    imp
-00002320: 6f72 7420 6e75 6d70 7920 6173 206e 700d  ort numpy as np.
-00002330: 0a20 2020 2066 726f 6d20 7372 7367 7569  .    from srsgui
-00002340: 2069 6d70 6f72 7420 496e 7374 7275 6d65   import Instrume
-00002350: 6e74 0d0a 0d0a 2020 2020 636c 6173 7320  nt....    class 
-00002360: 5344 5331 3230 3228 496e 7374 7275 6d65  SDS1202(Instrume
-00002370: 6e74 293a 0d0a 2020 2020 2020 2020 5f49  nt):..        _I
-00002380: 6453 7472 696e 6720 3d20 2753 4453 3132  dString = 'SDS12
-00002390: 3032 270d 0a0d 0a20 2020 2020 2020 2064  02'....        d
-000023a0: 6566 2067 6574 5f77 6176 6566 6f72 6d28  ef get_waveform(
-000023b0: 7365 6c66 2c20 6368 616e 6e65 6c29 3a0d  self, channel):.
-000023c0: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-000023d0: 0d0a 0d0a 2020 2020 2020 2020 6465 6620  ....        def 
-000023e0: 6765 745f 7361 6d70 6c69 6e67 5f72 6174  get_sampling_rat
-000023f0: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
-00002400: 2020 2020 2020 2e2e 2e0d 0a0d 0a4f 6e63        .......Onc
-00002410: 6520 7468 6520 6f73 6369 6c6c 6f73 636f  e the oscillosco
-00002420: 7065 2069 7320 636f 6e6e 6563 7465 6420  pe is connected 
-00002430: 746f 2074 6865 2061 7070 6c69 6361 7469  to the applicati
-00002440: 6f6e 2c20 796f 7520 6361 6e20 7573 6520  on, you can use 
-00002450: 7468 6520 7465 726d 696e 616c 2074 6f20  the terminal to 
-00002460: 6578 706c 6f72 6520 7468 6520 6f73 6369  explore the osci
-00002470: 6c6c 6f73 636f 7065 2e0d 0a0d 0a2e 2e20  lloscope....... 
-00002480: 6669 6775 7265 3a3a 202e 2f5f 7374 6174  figure:: ./_stat
-00002490: 6963 2f6f 7363 2d64 6972 2d74 6572 6d69  ic/osc-dir-termi
-000024a0: 6e61 6c2d 7363 7265 656e 2d63 6170 7475  nal-screen-captu
-000024b0: 7265 2e70 6e67 0d0a 2020 2020 3a61 6c69  re.png..    :ali
-000024c0: 676e 3a20 6365 6e74 6572 0d0a 2020 2020  gn: center..    
-000024d0: 3a66 6967 636c 6173 733a 2061 6c69 676e  :figclass: align
-000024e0: 2d63 656e 7465 720d 0a0d 0a7c 0d0a 0d0a  -center....|....
-000024f0: 4265 6361 7573 6520 276f 7363 2720 6973  Because 'osc' is
-00002500: 206e 6f74 2074 6865 2064 6566 6175 6c74   not the default
-00002510: 2069 6e73 7472 756d 656e 742c 2079 6f75   instrument, you
-00002520: 2068 6176 6520 746f 2075 7365 2074 6865   have to use the
-00002530: 2070 7265 6669 7820 276f 7363 3a27 2077   prefix 'osc:' w
-00002540: 6974 6820 616c 6c20 7468 650d 0a72 6177  ith all the..raw
-00002550: 2072 656d 6f74 6520 636f 6d6d 616e 6473   remote commands
-00002560: 2079 6f75 2073 656e 6420 746f 2074 6865   you send to the
-00002570: 2069 6e73 7472 756d 656e 742e 2041 7320   instrument. As 
-00002580: 7368 6f77 6e20 7769 7468 2027 6f73 632e  shown with 'osc.
-00002590: 6469 7227 2c20 7468 6572 6520 6172 6520  dir', there are 
-000025a0: 6d61 6e79 206d 6574 686f 6473 0d0a 6176  many methods..av
-000025b0: 6169 6c61 626c 6520 7769 7468 2027 6f73  ailable with 'os
-000025c0: 632e 2720 4576 656e 206f 7363 2e67 6574  c.' Even osc.get
-000025d0: 5f77 6176 6566 6f72 6d28 2920 6973 2061  _waveform() is a
-000025e0: 7661 696c 6162 6c65 2066 726f 6d20 7468  vailable from th
-000025f0: 6520 7465 726d 696e 616c 2e20 0d0a 5768  e terminal. ..Wh
-00002600: 656e 2079 6f75 2075 7365 2061 206d 6574  en you use a met
-00002610: 686f 6420 696e 636f 7272 6563 746c 792c  hod incorrectly,
-00002620: 2074 6865 2074 6572 6d69 6e61 6c20 6b69   the terminal ki
-00002630: 6e64 6c79 2074 656c 6c73 206d 6520 7468  ndly tells me th
-00002640: 6174 2074 6865 7265 2069 7320 6120 6d69  at there is a mi
-00002650: 7373 696e 6720 6172 6775 6d65 6e74 200d  ssing argument .
-00002660: 0a69 6e20 6120 6675 6e63 7469 6f6e 2063  .in a function c
-00002670: 616c 6c2e 0d0a 596f 7520 6361 6e20 7365  all...You can se
-00002680: 6520 606f 7363 2e67 6574 5f77 6176 6566  e `osc.get_wavef
-00002690: 6f72 6d28 6368 616e 6e65 6c29 6020 7265  orm(channel)` re
-000026a0: 7475 726e 7320 7477 6f20 6e75 6d70 7920  turns two numpy 
-000026b0: 6172 7261 7973 2e0d 0a57 6861 7420 6966  arrays...What if
-000026c0: 2079 6f75 2077 616e 7420 746f 2070 6c6f   you want to plo
-000026d0: 7420 7468 6520 6461 7461 3f0d 0a41 7320  t the data?..As 
-000026e0: 7468 6520 6d65 7468 6f64 7320 796f 7520  the methods you 
-000026f0: 696d 706c 656d 656e 7420 666f 7220 696e  implement for in
-00002700: 7465 7261 6374 696e 6720 7769 7468 2079  teracting with y
-00002710: 6f75 7220 696e 7374 7275 6d65 6e74 7320  our instruments 
-00002720: 616e 6420 6461 7461 2067 726f 7720 696e  and data grow in
-00002730: 2063 6f6d 706c 6578 6974 792c 0d0a 796f   complexity,..yo
-00002740: 7520 6d61 7920 6e65 6564 2074 6f20 6772  u may need to gr
-00002750: 6164 7561 7465 2066 726f 6d20 7465 726d  aduate from term
-00002760: 696e 616c 2d62 6173 6564 2069 6e74 6572  inal-based inter
-00002770: 6163 7469 6f6e 2074 6f20 7461 736b 2d62  action to task-b
-00002780: 6173 6564 2069 6e74 6572 6163 7469 6f6e  ased interaction
-00002790: 2e20 5265 6164 206f 6e2e 0d0a 0d0a 5461  . Read on.....Ta
-000027a0: 736b 730d 0a2d 2d2d 2d2d 2d2d 0d0a 0d0a  sks..-------....
-000027b0: 486f 7720 746f 2072 756e 2061 2074 6173  How to run a tas
-000027c0: 6b0d 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e 5e5e  k..^^^^^^^^^^^^^
-000027d0: 5e5e 5e5e 5e5e 0d0a 0d0a 5374 6172 7420  ^^^^^^....Start 
-000027e0: 7468 6520 6060 7372 7367 7569 6060 2061  the ``srsgui`` a
-000027f0: 7070 6c69 6361 7469 6f6e 2e20 596f 7520  pplication. You 
-00002800: 6361 6e20 7365 6520 7768 6572 6520 7468  can see where th
-00002810: 6520 2e74 6173 6b63 6f6e 6669 6720 6669  e .taskconfig fi
-00002820: 6c65 2069 7320 6f70 656e 6564 0d0a 6672  le is opened..fr
-00002830: 6f6d 2074 6865 2063 6f6e 736f 6c65 2077  om the console w
-00002840: 696e 646f 7720 283a 7265 663a 6068 6572  indow (:ref:`her
-00002850: 6520 3c74 6f70 2d6f 662d 696e 6974 6961  e <top-of-initia
-00002860: 6c2d 7363 7265 656e 2d63 6170 7475 7265  l-screen-capture
-00002870: 3e60 292e 0d0a 4966 2079 6f75 206d 6164  >`)...If you mad
-00002880: 6520 6120 636f 7079 206f 6620 7468 6520  e a copy of the 
-00002890: 6f72 6967 696e 616c 2065 7861 6d70 6c65  original example
-000028a0: 2066 726f 6d20 7468 6520 6060 7372 7367   from the ``srsg
-000028b0: 7569 6060 0d0a 7061 636b 6167 6520 6469  ui``..package di
-000028c0: 7265 6374 6f72 792c 206f 7065 6e20 6974  rectory, open it
-000028d0: 2061 6761 696e 2066 726f 6d20 7468 6520   again from the 
-000028e0: 636f 7272 6563 7420 6469 7265 6374 6f72  correct director
-000028f0: 792e 0d0a 0d0a 4966 2074 6865 7265 2061  y.....If there a
-00002900: 7265 206e 6f20 6572 726f 7220 6d65 7373  re no error mess
-00002910: 6167 6573 2069 6e20 7468 6520 436f 6e73  ages in the Cons
-00002920: 6f6c 6520 7769 6e64 6f77 2c20 636f 6e6e  ole window, conn
-00002930: 6563 7420 7468 6520 6675 6e63 7469 6f6e  ect the function
-00002940: 2067 656e 6572 6174 6f72 0d0a 616e 6420   generator..and 
-00002950: 7468 6520 6f73 6369 6c6c 6f73 636f 7065  the oscilloscope
-00002960: 2066 726f 6d20 7468 6520 496e 7374 7275   from the Instru
-00002970: 6d65 6e74 7320 6d65 6e75 2e0d 0a0d 0a54  ments menu.....T
-00002980: 6865 206f 7665 7261 6c6c 2073 7472 7563  he overall struc
-00002990: 7475 7265 206f 6620 6120 7461 736b 2069  ture of a task i
-000029a0: 7320 6465 7363 7269 6265 6420 696e 203a  s described in :
-000029b0: 7265 663a 6057 7269 7469 6e67 2061 2074  ref:`Writing a t
-000029c0: 6173 6b20 7363 7269 7074 6020 7365 6374  ask script` sect
-000029d0: 696f 6e2e 0d0a 5468 6572 6520 6172 6520  ion...There are 
-000029e0: 3520 7461 736b 7320 6172 6520 696e 636c  5 tasks are incl
-000029f0: 7564 6564 2069 6e20 7468 6520 6578 616d  uded in the exam
-00002a00: 706c 6520 7072 6f6a 6563 742e 2054 6865  ple project. The
-00002a10: 7920 6772 6164 7561 6c6c 7920 6164 6420  y gradually add 
-00002a20: 6d6f 7265 2066 6561 7475 7265 730d 0a6f  more features..o
-00002a30: 6e20 7468 6520 746f 7020 6f66 2074 6865  n the top of the
-00002a40: 2070 7265 7669 6f75 7320 7461 736b 732e   previous tasks.
-00002a50: 200d 0a54 6865 7920 6172 6520 6465 7369   ..They are desi
-00002a60: 676e 6564 2074 6f20 7368 6f77 6361 7365  gned to showcase
-00002a70: 2068 6f77 2074 6f20 7573 6520 7468 6520   how to use the 
-00002a80: 5461 736b 2063 6c61 7373 2e0d 0a0d 0a53  Task class.....S
-00002a90: 656c 6563 7420 7468 6520 6669 7273 7420  elect the first 
-00002aa0: 7461 736b 2028 5c2a 4944 4e20 7465 7374  task (\*IDN test
-00002ab0: 2920 6672 6f6d 2074 6865 2054 6173 6b73  ) from the Tasks
-00002ac0: 206d 656e 750d 0a61 6e64 2063 6c69 636b   menu..and click
-00002ad0: 2074 6865 2067 7265 656e 2061 7272 6f77   the green arrow
-00002ae0: 2069 6e20 7468 6520 746f 6f6c 2062 6172   in the tool bar
-00002af0: 2074 6f20 7275 6e20 7468 6520 7461 736b   to run the task
-00002b00: 2e0d 0a0d 0a46 6972 7374 5461 736b 0d0a  .....FirstTask..
-00002b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a54  -----------....T
-00002b20: 6865 2066 6972 7374 2074 6173 6b20 7368  he first task sh
-00002b30: 6f77 733a 0d0a 0d0a 2020 2020 2d20 486f  ows:....    - Ho
-00002b40: 7720 746f 2075 7365 206d 6f64 756c 652d  w to use module-
-00002b50: 6c65 7665 6c20 6c6f 6767 6572 2066 6f72  level logger for
-00002b60: 2050 7974 686f 6e20 6c6f 6767 696e 675f   Python logging_
-00002b70: 2069 6e20 6120 7461 736b 0d0a 2020 2020   in a task..    
-00002b80: 2d20 486f 7720 746f 2075 7365 2069 6e73  - How to use ins
-00002b90: 7472 756d 656e 7473 2064 6566 696e 6564  truments defined
-00002ba0: 2069 6e20 7468 6520 636f 6e66 6967 7572   in the configur
-00002bb0: 6174 696f 6e20 6669 6c65 0d0a 2020 2020  ation file..    
-00002bc0: 2d20 486f 7720 746f 2075 7365 2074 6578  - How to use tex
-00002bd0: 7420 6f75 7470 7574 2074 6f20 7468 6520  t output to the 
-00002be0: 636f 6e73 6f6c 6520 7769 6e64 6f77 0d0a  console window..
-00002bf0: 0d0a 4974 2069 7320 6e6f 7420 6d75 6368  ..It is not much
-00002c00: 2064 6966 6665 7265 6e74 2066 726f 6d20   different from 
-00002c10: 7468 6520 3a72 6566 3a60 6261 7265 2062  the :ref:`bare b
-00002c20: 6f6e 6520 7374 7275 6374 7572 6520 3c74  one structure <t
-00002c30: 6f70 2d6f 662d 6261 7265 2d62 6f6e 652d  op-of-bare-bone-
-00002c40: 7461 736b 3e60 0d0a 7368 6f77 6e20 696e  task>`..shown in
-00002c50: 2074 6865 203a 7265 663a 6057 7269 7469   the :ref:`Writi
-00002c60: 6e67 2061 2074 6173 6b20 7363 7269 7074  ng a task script
-00002c70: 6020 7365 6374 696f 6e2e 0d0a 0d0a 2e2e  ` section.......
-00002c80: 206c 6974 6572 616c 696e 636c 7564 653a   literalinclude:
-00002c90: 3a20 2e2e 2f73 7273 6775 692f 6578 616d  : ../srsgui/exam
-00002ca0: 706c 6573 2f6f 7363 696c 6c6f 7363 6f70  ples/oscilloscop
-00002cb0: 6520 6578 616d 706c 652f 7461 736b 732f  e example/tasks/
-00002cc0: 6669 7273 742e 7079 0d0a 2020 2020 3a6c  first.py..    :l
-00002cd0: 616e 6775 6167 653a 2050 7974 686f 6e0d  anguage: Python.
-00002ce0: 0a20 2020 203a 6c69 6e65 6e6f 733a 0d0a  .    :linenos:..
-00002cf0: 0d0a 5573 696e 6720 2a2a 7365 6c66 2e6c  ..Using **self.l
-00002d00: 6f67 6765 722a 2a20 7365 6e64 7320 7468  ogger** sends th
-00002d10: 6520 6c6f 6767 696e 6720 6f75 7470 7574  e logging output
-00002d20: 2074 6f20 7468 6520 636f 6e73 6f6c 6520   to the console 
-00002d30: 7769 6e64 6f77 2c20 7468 6520 6d61 7374  window, the mast
-00002d40: 6572 206c 6f67 6769 6e67 2066 696c 6520  er logging file 
-00002d50: 696e 0d0a 607e 2f74 6173 6b2d 7265 7375  in..`~/task-resu
-00002d60: 6c74 7320 6469 7265 6374 6f72 792f 6d61  lts directory/ma
-00002d70: 696e 6c6f 672d 7878 2e74 7874 2e78 602c  inlog-xx.txt.x`,
-00002d80: 2061 6e64 2074 6f20 7468 6520 7461 736b   and to the task
-00002d90: 2072 6573 756c 7420 6461 7461 2066 696c   result data fil
-00002da0: 6520 6c6f 6361 7465 6420 696e 0d0a 607e  e located in..`~
-00002db0: 2f74 6173 6b2d 7265 7375 6c74 732f 7072  /task-results/pr
-00002dc0: 6f6a 6563 742d 6e61 6d65 2d69 6e2d 636f  oject-name-in-co
-00002dd0: 6e66 6967 2d66 696c 652f 524e 7878 7860  nfig-file/RNxxx`
-00002de0: 2064 6972 6563 746f 7279 2e0d 0a0d 0a57   directory.....W
-00002df0: 6974 6820 3a6d 6574 683a 6067 6574 5f69  ith :meth:`get_i
-00002e00: 6e73 7472 756d 656e 7420 3c73 7273 6775  nstrument <srsgu
-00002e10: 692e 7461 736b 2e74 6173 6b2e 5461 736b  i.task.task.Task
-00002e20: 2e67 6574 5f69 6e73 7472 756d 656e 743e  .get_instrument>
-00002e30: 6020 796f 7520 6361 6e20 6765 7420 7468  ` you can get th
-00002e40: 6520 696e 7374 7275 6d65 6e74 0d0a 6465  e instrument..de
-00002e50: 6669 6e65 6420 696e 2074 6865 2063 6f6e  fined in the con
-00002e60: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
-00002e70: 696e 2061 2074 6173 6b2e 202a 2a44 6f20  in a task. **Do 
-00002e80: 6e6f 7420 6469 7363 6f6e 6e65 6374 2074  not disconnect t
-00002e90: 6865 2069 6e73 7472 756d 656e 7420 696e  he instrument in
-00002ea0: 2074 6865 2074 6173 6b21 2a2a 0d0a 496e   the task!**..In
-00002eb0: 7374 7275 6d65 6e74 2043 6f6e 6e65 6374  strument Connect
-00002ec0: 6976 6974 7920 6973 206d 616e 6167 6564  ivity is managed
-00002ed0: 2061 7420 7468 6520 6060 7372 7367 7569   at the ``srsgui
-00002ee0: 6060 2061 7070 6c69 6361 7469 6f6e 206c  `` application l
-00002ef0: 6576 656c 2e0d 0a0d 0a54 6869 7320 7461  evel.....This ta
-00002f00: 736b 2068 6967 686c 6967 6874 7320 686f  sk highlights ho
-00002f10: 7720 7265 6d6f 7465 2063 6f6d 6d61 6e64  w remote command
-00002f20: 2073 6574 2061 6e64 2071 7565 7279 2074   set and query t
-00002f30: 7261 6e73 6163 7469 6f6e 7320 6172 6520  ransactions are 
-00002f40: 7369 6d70 6c69 6669 6564 2062 7920 6465  simplified by de
-00002f50: 6669 6e69 6e67 200d 0a61 6e20 6174 7472  fining ..an attr
-00002f60: 6962 7574 6520 7573 696e 6720 3a6d 6f64  ibute using :mod
-00002f70: 3a60 7372 7367 7569 2e69 6e73 742e 636f  :`srsgui.inst.co
-00002f80: 6d6d 616e 6473 6020 6d6f 6475 6c65 2c20  mmands` module, 
-00002f90: 0d0a 7768 6963 6820 6973 2075 7469 6c69  ..which is utili
-00002fa0: 7a65 6420 696e 2074 6865 2043 4736 3335  zed in the CG635
-00002fb0: 2063 6c61 7373 2064 6566 696e 6974 696f   class definitio
-00002fc0: 6e20 7669 6120 7468 6520 666f 6c6c 6f77  n via the follow
-00002fd0: 696e 6720 6c69 6e65 3a20 200d 0a0d 0a60  ing line:  ....`
-00002fe0: 6066 7265 7175 656e 6379 203d 2046 6c6f  `frequency = Flo
-00002ff0: 6174 436f 6d6d 616e 6428 2746 5245 5127  atCommand('FREQ'
-00003000: 2960 600d 0a0d 0a54 6869 7320 7369 6d70  )``....This simp
-00003010: 6c65 206c 696e 6520 6d61 6b65 7320 6974  le line makes it
-00003020: 2070 6f73 7369 626c 6520 746f 2073 6574   possible to set
-00003030: 2061 6e64 2071 7565 7279 2074 6865 2060   and query the `
-00003040: 6367 2e66 7265 7175 656e 6379 6020 0d0a  cg.frequency` ..
-00003050: 7769 7468 6f75 7420 6861 7669 6e67 2074  without having t
-00003060: 6f20 6469 7265 6374 6c79 206d 616e 6970  o directly manip
-00003070: 756c 6174 6520 636f 6d6d 616e 6420 6f72  ulate command or
-00003080: 2072 6573 706f 6e73 6520 7374 7269 6e67   response string
-00003090: 732e 200d 0a0d 0a53 6563 6f6e 6454 6173  s. ....SecondTas
-000030a0: 6b0d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  k..-----------..
-000030b0: 0d0a 5468 6520 7365 636f 6e64 2074 6173  ..The second tas
-000030c0: 6b20 7265 7175 6972 6573 206e 6f20 696e  k requires no in
-000030d0: 7374 7275 6d65 6e74 2063 6f6e 6e65 6374  strument connect
-000030e0: 696f 6e73 2c20 616e 6420 7368 6f77 733a  ions, and shows:
-000030f0: 0d0a 0d0a 2020 2020 2d20 486f 7720 746f  ....    - How to
-00003100: 2064 6566 696e 6520 3a61 7474 723a 6069   define :attr:`i
-00003110: 6e70 7574 5f70 6172 616d 6574 6572 7320  nput_parameters 
-00003120: 3c73 7273 6775 692e 7461 736b 2e74 6173  <srsgui.task.tas
-00003130: 6b2e 5461 736b 2e69 6e70 7574 5f70 6172  k.Task.input_par
-00003140: 616d 6574 6572 733e 600d 0a20 2020 2020  ameters>`..     
-00003150: 2066 6f72 2069 6e74 6572 6163 7469 7665   for interactive
-00003160: 2075 7365 7220 696e 7075 7420 6672 6f6d   user input from
-00003170: 2074 6865 2061 7070 6c69 6361 7469 6f6e   the application
-00003180: 2069 6e70 7574 2070 616e 656c 0d0a 2020   input panel..  
-00003190: 2020 2d20 486f 7720 746f 2075 7365 206d    - How to use m
-000031a0: 6174 706c 6f74 6c69 6220 6669 6775 7265  atplotlib figure
-000031b0: 7320 666f 7220 706c 6f74 7469 6e67 2064  s for plotting d
-000031c0: 6174 610d 0a20 2020 202d 2048 6f77 2074  ata..    - How t
-000031d0: 6f20 7365 6e64 2074 6578 7420 6f75 7470  o send text outp
-000031e0: 7574 2074 6f20 7468 6520 7265 7375 6c74  ut to the result
-000031f0: 2077 696e 646f 7720 7573 696e 670d 0a20   window using.. 
-00003200: 2020 2020 203a 6d65 7468 3a60 6469 7370       :meth:`disp
-00003210: 6c61 795f 7265 7375 6c74 2829 203c 7372  lay_result() <sr
-00003220: 7367 7569 2e74 6173 6b2e 7461 736b 2e54  sgui.task.task.T
-00003230: 6173 6b2e 6469 7370 6c61 795f 7265 7375  ask.display_resu
-00003240: 6c74 3e60 0d0a 2020 2020 2d20 486f 7720  lt>`..    - How 
-00003250: 746f 2073 746f 7020 7468 6520 7461 736b  to stop the task
-00003260: 2062 7920 6368 6563 6b69 6e67 0d0a 2020   by checking..  
-00003270: 2020 2020 3a6d 6574 683a 6069 735f 7275      :meth:`is_ru
-00003280: 6e6e 696e 6728 2920 3c73 7273 6775 692e  nning() <srsgui.
-00003290: 7461 736b 2e74 6173 6b2e 5461 736b 2e69  task.task.Task.i
-000032a0: 735f 7275 6e6e 696e 673e 602e 0d0a 0d0a  s_running>`.....
-000032b0: 2e2e 206c 6974 6572 616c 696e 636c 7564  .. literalinclud
-000032c0: 653a 3a20 2e2e 2f73 7273 6775 692f 6578  e:: ../srsgui/ex
-000032d0: 616d 706c 6573 2f6f 7363 696c 6c6f 7363  amples/oscillosc
-000032e0: 6f70 6520 6578 616d 706c 652f 7461 736b  ope example/task
-000032f0: 732f 7365 636f 6e64 2e70 790d 0a20 2020  s/second.py..   
-00003300: 203a 6c61 6e67 7561 6765 3a20 5079 7468   :language: Pyth
-00003310: 6f6e 0d0a 2020 2020 3a6c 696e 656e 6f73  on..    :linenos
-00003320: 3a0d 0a0d 0a55 7369 6e67 206d 6174 706c  :....Using matpl
-00003330: 6f74 6c69 625f 2077 6974 6820 6060 7372  otlib_ with ``sr
-00003340: 7367 7569 6060 2069 7320 7374 7261 6967  sgui`` is straig
-00003350: 6874 666f 7277 6172 6420 6966 2079 6f75  htforward if you
-00003360: 2061 7265 2061 6c72 6561 6479 2066 616d   are already fam
-00003370: 696c 6961 7220 7769 7468 2069 7473 2075  iliar with its u
-00003380: 7361 6765 2e0d 0a28 5265 6665 7220 746f  sage...(Refer to
-00003390: 206d 6174 706c 6f74 6c69 625f 2064 6f63   matplotlib_ doc
-000033a0: 756d 656e 7461 7469 6f6e 292e 0d0a 0d0a  umentation).....
-000033b0: 5468 6520 696d 706f 7274 616e 7420 6469  The important di
-000033c0: 6666 6572 656e 6365 7320 7768 656e 2075  fferences when u
-000033d0: 7369 6e67 206d 6174 706c 6f74 6c69 6220  sing matplotlib 
-000033e0: 696e 2060 6073 7273 6775 6960 6020 6172  in ``srsgui`` ar
-000033f0: 653a 0d0a 2020 2020 2d20 596f 7520 6861  e:..    - You ha
-00003400: 7665 2074 6f20 6765 7420 7468 6520 6669  ve to get the fi
-00003410: 6775 7265 2075 7369 6e67 2067 6574 5f66  gure using get_f
-00003420: 6967 7572 6528 292c 2072 6174 6865 7220  igure(), rather 
-00003430: 7468 616e 2063 7265 6174 696e 6720 6f6e  than creating on
-00003440: 6520 6f6e 2079 6f75 7220 6f77 6e2e 0d0a  e on your own...
-00003450: 2020 2020 2d20 506c 6f74 7320 6172 6520      - Plots are 
-00003460: 6372 6561 7465 6420 6475 7269 6e67 2060  created during `
-00003470: 7365 7475 7028 2960 2c20 6265 6361 7573  setup()`, becaus
-00003480: 6520 6974 2069 7320 6120 736c 6f77 2070  e it is a slow p
-00003490: 726f 6365 7373 2e20 4475 7269 6e67 2060  rocess. During `
-000034a0: 7465 7374 2829 602c 0d0a 2020 2020 2020  test()`,..      
-000034b0: 796f 7520 7369 6d70 6c79 2075 7064 6174  you simply updat
-000034c0: 6520 6461 7461 2075 7369 6e67 2060 7365  e data using `se
-000034d0: 745f 6461 7461 2829 6020 6f72 2073 696d  t_data()` or sim
-000034e0: 696c 6961 7220 6d65 7468 6f64 7320 666f  iliar methods fo
-000034f0: 7220 6461 7461 2075 7064 6174 652e 0d0a  r data update...
-00003500: 2020 2020 2d20 596f 7520 6d75 7374 2075      - You must u
-00003510: 7365 2060 7265 7175 6573 745f 6669 6775  se `request_figu
-00003520: 7265 5f75 7064 6174 6528 2960 2074 6f20  re_update()` to 
-00003530: 7265 6472 6177 2074 6865 2070 6c6f 742c  redraw the plot,
-00003540: 2061 6674 6572 2060 7365 745f 6461 7461   after `set_data
-00003550: 2829 602e 0d0a 2020 2020 2020 5468 6520  ()`...      The 
-00003560: 6576 656e 7420 6c6f 6f70 2068 616e 646c  event loop handl
-00003570: 6572 2069 6e20 7468 6520 6d61 696e 2061  er in the main a
-00003580: 7070 6c69 6361 7469 6f6e 2077 696c 6c20  pplication will 
-00003590: 7570 6461 7465 2074 6865 2070 6c6f 7420  update the plot 
-000035a0: 6174 2069 7473 2065 6172 6c69 6573 740d  at its earliest.
-000035b0: 0a20 2020 2020 2063 6f6e 7665 6e69 656e  .      convenien
-000035c0: 6365 2e0d 0a0d 0a0d 0a2e 2e20 6669 6775  ce......... figu
-000035d0: 7265 3a3a 202e 2f5f 7374 6174 6963 2f73  re:: ./_static/s
-000035e0: 6563 6f6e 642d 7461 736b 2d73 6372 6565  econd-task-scree
-000035f0: 6e2d 6361 7074 7572 652e 706e 670d 0a20  n-capture.png.. 
-00003600: 2020 203a 616c 6967 6e3a 2063 656e 7465     :align: cente
-00003610: 720d 0a20 2020 203a 6669 6763 6c61 7373  r..    :figclass
-00003620: 3a20 616c 6967 6e2d 6365 6e74 6572 0d0a  : align-center..
-00003630: 0d0a 7c0d 0a0d 0a54 6869 7264 5461 736b  ..|....ThirdTask
-00003640: 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d  ..-----------...
-00003650: 0a54 6865 2074 6869 7264 2074 6173 6b20  .The third task 
-00003660: 7573 6573 2074 6865 206f 7363 696c 6c6f  uses the oscillo
-00003670: 7363 6f70 6520 6f6e 6c79 2e20 4974 2067  scope only. It g
-00003680: 6574 7320 7468 6520 7265 7175 6573 7465  ets the requeste
-00003690: 6420 6e75 6d62 6572 206f 6620 6361 7074  d number of capt
-000036a0: 7572 6573 2066 726f 6d20 7573 6572 2069  ures from user i
-000036b0: 6e70 7574 2c0d 0a74 6865 6e20 7265 7065  nput,..then repe
-000036c0: 6174 7320 6f73 6369 6c6c 6f73 636f 7065  ats oscilloscope
-000036d0: 2077 6176 6566 6f72 6d20 6361 7074 7572   waveform captur
-000036e0: 6520 616e 6420 7570 6461 7465 7320 7468  e and updates th
-000036f0: 6520 7761 7665 666f 726d 2070 6c6f 742e  e waveform plot.
-00003700: 200d 0a49 7420 7374 6f70 7320 6f6e 6365   ..It stops once
-00003710: 2074 6865 2064 6573 6972 6564 206e 756d   the desired num
-00003720: 6265 7220 6f66 2063 6170 7475 7265 7320  ber of captures 
-00003730: 6861 7665 2062 6565 6e20 6f62 7461 696e  have been obtain
-00003740: 6564 2c20 6f72 2077 6865 6e20 7468 6520  ed, or when the 
-00003750: 5374 6f70 2062 7574 746f 6e20 6973 2070  Stop button is p
-00003760: 7265 7373 6564 2e0d 0a57 6176 6566 6f72  ressed...Wavefor
-00003770: 6d73 2061 7265 2063 6170 7475 7265 6420  ms are captured 
-00003780: 7769 7468 2037 3030 3030 3020 706f 696e  with 700000 poin
-00003790: 7473 2061 626f 7574 2065 7665 7279 2030  ts about every 0
-000037a0: 2e32 2073 6563 6f6e 6473 206f 7665 7220  .2 seconds over 
-000037b0: 5443 502f 4950 2063 6f6d 6d75 6e63 6174  TCP/IP communcat
-000037c0: 696f 6e2e 0d0a 0d0a 0d0a 2e2e 206c 6974  ion......... lit
-000037d0: 6572 616c 696e 636c 7564 653a 3a20 2e2e  eralinclude:: ..
-000037e0: 2f73 7273 6775 692f 6578 616d 706c 6573  /srsgui/examples
-000037f0: 2f6f 7363 696c 6c6f 7363 6f70 6520 6578  /oscilloscope ex
-00003800: 616d 706c 652f 7461 736b 732f 7468 6972  ample/tasks/thir
-00003810: 642e 7079 0d0a 2020 2020 3a6c 616e 6775  d.py..    :langu
-00003820: 6167 653a 2050 7974 686f 6e0d 0a20 2020  age: Python..   
-00003830: 203a 6c69 6e65 6e6f 733a 0d0a 0d0a 466f   :linenos:....Fo
-00003840: 7572 7468 5461 736b 0d0a 2d2d 2d2d 2d2d  urthTask..------
-00003850: 2d2d 2d2d 2d0d 0a0d 0a54 6865 2066 6f75  -----....The fou
-00003860: 7274 6820 6578 616d 706c 6520 6973 2074  rth example is t
-00003870: 6865 2063 6c69 6d61 7820 6f66 2074 6865  he climax of the
-00003880: 2065 7861 6d70 6c65 7320 7365 7269 6573   examples series
-00003890: 2028 3a72 6566 3a60 7363 7265 656e 7368   (:ref:`screensh
-000038a0: 6f74 203c 746f 702d 6f66 2d73 6372 6565  ot <top-of-scree
-000038b0: 6e2d 6361 7074 7572 652d 313e 6029 2e0d  n-capture-1>`)..
-000038c0: 0a49 7420 7573 6573 2060 696e 7075 745f  .It uses `input_
-000038d0: 7061 7261 6d65 7465 7273 6020 746f 2063  parameters` to c
-000038e0: 6861 6e67 6520 6f75 7470 7574 2066 7265  hange output fre
-000038f0: 7175 656e 6379 206f 6620 7468 6520 636c  quency of the cl
-00003900: 6f63 6b20 6765 6e65 7261 746f 7220 696e  ock generator in
-00003910: 7465 7261 6374 6976 656c 792c 0d0a 6361  teractively,..ca
-00003920: 7074 7572 6573 2077 6176 6566 6f72 6d73  ptures waveforms
-00003930: 2066 726f 6d20 7468 6520 6f73 6369 6c6c   from the oscill
-00003940: 6f73 636f 7065 2c20 6361 6c63 756c 6174  oscope, calculat
-00003950: 6573 2061 6e20 4646 5420 6f66 2074 6865  es an FFT of the
-00003960: 2077 6176 6566 6f72 6d73 2077 6974 6820   waveforms with 
-00003970: 6e75 6d70 792c 0d0a 616e 6420 6765 6e65  numpy,..and gene
-00003980: 7261 7465 7320 706c 6f74 7320 7573 696e  rates plots usin
-00003990: 6720 3220 6d61 7470 6c6f 746c 6962 2066  g 2 matplotlib f
-000039a0: 6967 7572 6573 2e0d 0a0d 0a42 7920 6164  igures.....By ad
-000039b0: 6469 6e67 2074 6865 206e 616d 6573 206f  ding the names o
-000039c0: 6620 6669 6775 7265 7320 7468 6174 2079  f figures that y
-000039d0: 6f75 2077 616e 7420 746f 2075 7365 2069  ou want to use i
-000039e0: 6e20 6164 6469 7469 6f6e 616c 5f66 6967  n additional_fig
-000039f0: 7572 655f 6e61 6d65 732c 0d0a 6060 7372  ure_names,..``sr
-00003a00: 7367 7569 6060 2070 726f 7669 6465 7320  sgui`` provides 
-00003a10: 6d6f 7265 2066 6967 7572 6573 2074 6f20  more figures to 
-00003a20: 7468 6520 7461 736b 2062 6566 6f72 6520  the task before 
-00003a30: 6974 2073 7461 7274 732e 0d0a 0d0a 2e2e  it starts.......
-00003a40: 206c 6974 6572 616c 696e 636c 7564 653a   literalinclude:
-00003a50: 3a20 2e2e 2f73 7273 6775 692f 6578 616d  : ../srsgui/exam
-00003a60: 706c 6573 2f6f 7363 696c 6c6f 7363 6f70  ples/oscilloscop
-00003a70: 6520 6578 616d 706c 652f 7461 736b 732f  e example/tasks/
-00003a80: 666f 7572 7468 2e70 790d 0a20 2020 203a  fourth.py..    :
-00003a90: 6c61 6e67 7561 6765 3a20 5079 7468 6f6e  language: Python
-00003aa0: 0d0a 2020 2020 3a6c 696e 656e 6f73 3a0d  ..    :linenos:.
-00003ab0: 0a0d 0a46 6966 7468 5461 736b 0d0a 2d2d  ...FifthTask..--
-00003ac0: 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a 5468 6520  --------....The 
-00003ad0: 6669 6674 6820 7461 736b 2073 686f 7773  fifth task shows
-00003ae0: 2068 6f77 2074 6f20 7375 6263 6c61 7373   how to subclass
-00003af0: 2061 6e20 6578 6973 7469 6e67 2074 6173   an existing tas
-00003b00: 6b20 636c 6173 7320 666f 7220 7265 7573  k class for reus
-00003b10: 652e 0d0a 5468 6520 6d65 7468 6f64 2067  e...The method g
-00003b20: 6574 5f77 6176 6566 6f72 6d28 2920 696e  et_waveform() in
-00003b30: 2074 6865 2066 6f75 7274 6820 6578 616d   the fourth exam
-00003b40: 706c 6520 6973 2072 6569 6d70 6c65 6d65  ple is reimpleme
-00003b50: 6e74 6564 2074 6f20 6765 6e65 7261 7465  nted to generate
-00003b60: 0d0a 7369 6d75 6c61 7465 6420 7761 7665  ..simulated wave
-00003b70: 666f 726d 2074 6861 7420 7275 6e73 2077  form that runs w
-00003b80: 6974 686f 7574 2061 6e79 2072 6561 6c20  ithout any real 
-00003b90: 6f73 6369 6c6c 6f73 636f 7065 2e0d 0a0d  oscilloscope....
-00003ba0: 0a4e 6f74 6520 7468 6174 2074 6865 2073  .Note that the s
-00003bb0: 7175 6172 6520 7761 7665 2065 6467 6520  quare wave edge 
-00003bc0: 6361 6c63 756c 6174 696f 6e20 6973 2063  calculation is c
-00003bd0: 7275 6465 2c20 6361 7573 696e 6720 6d6f  rude, causing mo
-00003be0: 6475 6c61 7469 6f6e 2069 6e20 7075 6c73  dulation in puls
-00003bf0: 6520 7769 6474 680d 0a61 6e64 2073 6964  e width..and sid
-00003c00: 6520 6261 6e64 7320 696e 2074 6865 2046  e bands in the F
-00003c10: 4654 2073 7065 6374 7275 6d20 6966 2074  FT spectrum if t
-00003c20: 6865 2073 6574 2066 7265 7175 656e 6379  he set frequency
-00003c30: 2069 7320 6e6f 7420 636f 6d6d 656e 7375   is not commensu
-00003c40: 7261 7465 2077 6974 680d 0a74 6865 2073  rate with..the s
-00003c50: 616d 706c 696e 6720 7261 7465 2e20 546f  ampling rate. To
-00003c60: 2067 656e 6572 6174 6520 6120 636c 6561   generate a clea
-00003c70: 6e20 7371 7561 7265 2077 6176 652c 2074  n square wave, t
-00003c80: 6865 2072 6973 696e 6720 616e 6420 6661  he rising and fa
-00003c90: 6c6c 696e 6720 6564 6765 7320 7368 6f75  lling edges shou
-00003ca0: 6c64 0d0a 6861 7665 2061 7420 6c65 6173  ld..have at leas
-00003cb0: 7420 7477 6f20 706f 696e 7473 2074 6f20  t two points to 
-00003cc0: 7265 7072 6573 656e 7420 6578 6163 7420  represent exact 
-00003cd0: 7068 6173 652e 2044 6972 6563 7420 7472  phase. Direct tr
-00003ce0: 616e 7369 7469 6f6e 2066 726f 6d20 6c6f  ansition from lo
-00003cf0: 7720 746f 2068 6967 680d 0a77 6974 686f  w to high..witho
-00003d00: 7574 2061 6e79 2069 6e74 6572 6d65 6469  ut any intermedi
-00003d10: 6174 6520 706f 696e 7473 2073 7566 6665  ate points suffe
-00003d20: 7273 2066 726f 6d20 7375 6274 6c65 206d  rs from subtle m
-00003d30: 6f64 756c 6174 696f 6e20 696e 2074 696d  odulation in tim
-00003d40: 6520 646f 6d61 696e 2c0d 0a77 6869 6368  e domain,..which
-00003d50: 206d 616e 6966 6573 7473 2061 7320 7369   manifests as si
-00003d60: 6465 2062 616e 6473 2069 6e20 4646 542e  de bands in FFT.
-00003d70: 2054 6869 7320 6973 2061 2063 6f6d 6d6f   This is a commo
-00003d80: 6e20 7072 6f62 6c65 6d20 696e 2064 6967  n problem in dig
-00003d90: 6974 616c 2073 6967 6e61 6c0d 0a70 726f  ital signal..pro
-00003da0: 6365 7373 696e 672e 2049 7420 6973 206e  cessing. It is n
-00003db0: 6f74 2061 2070 726f 626c 656d 2069 6e20  ot a problem in 
-00003dc0: 7468 6520 7265 616c 2077 6f72 6c64 2c20  the real world, 
-00003dd0: 6265 6361 7573 6520 7468 6520 7369 676e  because the sign
-00003de0: 616c 2069 7320 616e 616c 6f67 2c0d 0a61  al is analog,..a
-00003df0: 6e64 2074 6865 2073 616d 706c 696e 6720  nd the sampling 
-00003e00: 7261 7465 2069 7320 6c69 6d69 7465 6420  rate is limited 
-00003e10: 6279 2074 6865 2062 616e 6477 6964 7468  by the bandwidth
-00003e20: 206f 6620 7468 6520 7369 676e 616c 2e0d   of the signal..
-00003e30: 0a0d 0a0d 0a2e 2e20 6c69 7465 7261 6c69  ....... literali
-00003e40: 6e63 6c75 6465 3a3a 202e 2e2f 7372 7367  nclude:: ../srsg
-00003e50: 7569 2f65 7861 6d70 6c65 732f 6f73 6369  ui/examples/osci
-00003e60: 6c6c 6f73 636f 7065 2065 7861 6d70 6c65  lloscope example
-00003e70: 2f74 6173 6b73 2f66 6966 7468 2e70 790d  /tasks/fifth.py.
-00003e80: 0a20 2020 203a 6c61 6e67 7561 6765 3a20  .    :language: 
-00003e90: 5079 7468 6f6e 0d0a 2020 2020 3a6c 696e  Python..    :lin
-00003ea0: 656e 6f73 3a0d 0a0d 0a0d 0a0d 0a2e 2e20  enos:.......... 
-00003eb0: 5f50 7956 6973 613a 2068 7474 7073 3a2f  _PyVisa: https:/
-00003ec0: 2f70 7976 6973 612e 7265 6164 7468 6564  /pyvisa.readthed
-00003ed0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00003ee0: 2f0d 0a2e 2e20 5f73 7273 696e 7374 2e73  /.... _srsinst.s
-00003ef0: 7238 3630 3a20 6874 7470 733a 2f2f 7079  r860: https://py
-00003f00: 7069 2e6f 7267 2f70 726f 6a65 6374 2f73  pi.org/project/s
-00003f10: 7273 696e 7374 2e73 7238 3630 2f0d 0a2e  rsinst.sr860/...
-00003f20: 2e20 5f56 5849 3131 3a20 6874 7470 733a  . _VXI11: https:
-00003f30: 2f2f 7777 772e 6c78 6973 7461 6e64 6172  //www.lxistandar
-00003f40: 642e 6f72 672f 4162 6f75 742f 5658 492d  d.org/About/VXI-
-00003f50: 3131 2d61 6e64 2d4c 5849 2e61 7370 780d  11-and-LXI.aspx.
-00003f60: 0a2e 2e20 5f47 5049 423a 2068 7474 7073  ... _GPIB: https
-00003f70: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-00003f80: 6f72 672f 7769 6b69 2f49 4545 452d 3438  org/wiki/IEEE-48
-00003f90: 380d 0a2e 2e20 5f55 5342 2d54 4d43 3a20  8.... _USB-TMC: 
-00003fa0: 6874 7470 733a 2f2f 7777 772e 7465 7374  https://www.test
-00003fb0: 616e 646d 6561 7375 7265 6d65 6e74 7469  andmeasurementti
-00003fc0: 7073 2e63 6f6d 2f72 656d 6f74 652d 636f  ps.com/remote-co
-00003fd0: 6d6d 756e 6963 6174 696f 6e2d 7769 7468  mmunication-with
-00003fe0: 2d75 7362 746d 632d 6661 712f 0d0a 2e2e  -usbtmc-faq/....
-00003ff0: 205f 5344 5331 3230 3258 453a 2068 7474   _SDS1202XE: htt
-00004000: 7073 3a2f 2f73 6967 6c65 6e74 6e61 2e63  ps://siglentna.c
-00004010: 6f6d 2f70 726f 6475 6374 2f73 6473 3132  om/product/sds12
-00004020: 3032 782d 652f 0d0a 2e2e 205f 5352 533a  02x-e/.... _SRS:
-00004030: 2068 7474 7073 3a2f 2f74 6869 6e6b 7372   https://thinksr
-00004040: 732e 636f 6d2f 0d0a 2e2e 205f 4347 3633  s.com/.... _CG63
-00004050: 353a 2068 7474 7073 3a2f 2f74 6869 6e6b  5: https://think
-00004060: 7372 732e 636f 6d2f 7072 6f64 7563 7473  srs.com/products
-00004070: 2f63 6736 3335 2e68 746d 6c0d 0a2e 2e20  /cg635.html.... 
-00004080: 5f6c 6f67 6769 6e67 3a20 6874 7470 733a  _logging: https:
-00004090: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
-000040a0: 672f 332f 686f 7774 6f2f 6c6f 6767 696e  g/3/howto/loggin
-000040b0: 672e 6874 6d6c 0d0a 2e2e 205f 6d61 7470  g.html.... _matp
-000040c0: 6c6f 746c 6962 3a20 6874 7470 733a 2f2f  lotlib: https://
-000040d0: 6d61 7470 6c6f 746c 6962 2e6f 7267 2f73  matplotlib.org/s
-000040e0: 7461 626c 652f 696e 6465 782e 6874 6d6c  table/index.html
+00000ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a  ------------....
+00000ad0: 5468 6520 7374 7275 6374 7572 6520 6f66  The structure of
+00000ae0: 2061 202e 7461 736b 636f 6e66 6967 2066   a .taskconfig f
+00000af0: 696c 6520 6973 2073 696d 706c 6520 616e  ile is simple an
+00000b00: 640d 0a65 7870 6c61 696e 6564 2069 6e20  d..explained in 
+00000b10: 3a72 6566 3a60 506f 7075 6c61 7469 6e67  :ref:`Populating
+00000b20: 2074 6865 202e 7461 736b 636f 6e66 6967   the .taskconfig
+00000b30: 2066 696c 6560 0d0a 0d0a 2e2e 2063 6f64   file`...... cod
+00000b40: 652d 626c 6f63 6b3a 3a0d 0a20 2020 203a  e-block::..    :
+00000b50: 6c69 6e65 6e6f 733a 0d0a 0d0a 2020 2020  linenos:....    
+00000b60: 6e61 6d65 3a20 5372 7367 7569 2045 7861  name: Srsgui Exa
+00000b70: 6d70 6c65 202d 204f 7363 696c 6c6f 7363  mple - Oscillosc
+00000b80: 6f70 6520 616e 6420 436c 6f63 6b20 4765  ope and Clock Ge
+00000b90: 6e65 7261 746f 720d 0a0d 0a20 2020 2069  nerator....    i
+00000ba0: 6e73 743a 2063 672c 2020 696e 7374 7275  nst: cg,  instru
+00000bb0: 6d65 6e74 732e 6367 3633 352c 2020 2043  ments.cg635,   C
+00000bc0: 4736 3335 0d0a 2020 2020 696e 7374 3a20  G635..    inst: 
+00000bd0: 6f73 632c 2069 6e73 7472 756d 656e 7473  osc, instruments
+00000be0: 2e73 6473 3132 3032 2c20 5344 5331 3230  .sds1202, SDS120
+00000bf0: 320d 0a0d 0a20 2020 2074 6173 6b3a 202a  2....    task: *
+00000c00: 4944 4e20 7465 7374 2c20 2020 2020 2020  IDN test,       
+00000c10: 2020 2020 2020 2020 2020 7461 736b 732e            tasks.
+00000c20: 6964 656e 6669 6679 2c20 2049 6465 6e74  idenfify,  Ident
+00000c30: 6966 790d 0a20 2020 2074 6173 6b3a 2050  ify..    task: P
+00000c40: 6c6f 7420 6578 616d 706c 652c 2020 2020  lot example,    
+00000c50: 2020 2020 2020 2020 2020 7461 736b 732e            tasks.
+00000c60: 706c 6f74 5f65 7861 6d70 6c65 2c20 506c  plot_example, Pl
+00000c70: 6f74 4578 616d 706c 650d 0a20 2020 202e  otExample..    .
+00000c80: 2e2e 0d0a 0d0a 496e 7374 7275 6d65 6e74  ......Instrument
+00000c90: 2064 7269 7665 7273 0d0a 2d2d 2d2d 2d2d   drivers..------
+00000ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
+00000cb0: 0d0a 4347 3633 350d 0a5e 5e5e 5e5e 0d0a  ..CG635..^^^^^..
+00000cc0: 0d0a 4c65 7427 7320 7461 6b65 2061 206c  ..Let's take a l
+00000cd0: 6f6f 6b20 696e 746f 2074 6865 2060 696e  ook into the `in
+00000ce0: 7374 7275 6d65 6e74 732f 6367 3633 352e  struments/cg635.
+00000cf0: 7079 6020 6d6f 6475 6c65 2e20 4576 656e  py` module. Even
+00000d00: 2074 686f 7567 6820 6974 2073 6565 6d73   though it seems
+00000d10: 206c 6f6e 672c 0d0a 6974 2068 6173 206f   long,..it has o
+00000d20: 6e6c 7920 3520 6c69 6e65 7320 6f66 206e  nly 5 lines of n
+00000d30: 6f6e 2d63 6f6d 6d65 6e74 2063 6f64 652e  on-comment code.
+00000d40: 2049 6620 796f 7520 6861 7665 2061 2043   If you have a C
+00000d50: 4736 3335 2c0d 0a63 6f6e 6772 6174 756c  G635,..congratul
+00000d60: 6174 696f 6e73 2120 596f 7520 6361 6e20  ations! You can 
+00000d70: 7573 6520 7468 6520 6669 6c65 2061 7320  use the file as 
+00000d80: 6973 2e20 4966 2079 6f75 2068 6176 6520  is. If you have 
+00000d90: 616e 7920 6675 6e63 7469 6f6e 0d0a 6765  any function..ge
+00000da0: 6e65 7261 746f 7220 7468 6174 2063 616e  nerator that can
+00000db0: 2063 6861 6e67 6520 7468 6520 6f75 7470   change the outp
+00000dc0: 7574 2066 7265 7175 656e 6379 2c20 796f  ut frequency, yo
+00000dd0: 7520 6361 6e20 7573 6520 6974 2069 6e73  u can use it ins
+00000de0: 7465 6164 206f 6620 7468 6520 4347 3633  tead of the CG63
+00000df0: 350d 0a69 6e20 7468 6520 6578 616d 706c  5..in the exampl
+00000e00: 652e 2059 6f75 2063 6861 6e67 6520 7468  e. You change th
+00000e10: 6520 636c 6173 7320 6e61 6d65 2061 6e64  e class name and
+00000e20: 205f 4964 5374 7269 6e67 2074 6f20 6d61   _IdString to ma
+00000e30: 7463 6820 7468 6520 696e 7374 7275 6d65  tch the instrume
+00000e40: 6e74 206e 616d 652c 0d0a 616c 6f6e 6720  nt name,..along 
+00000e50: 7769 7468 205f 7465 726d 5f63 6861 722e  with _term_char.
+00000e60: 204c 6f6f 6b20 7570 2074 6865 2063 6f6d   Look up the com
+00000e70: 6d61 6e64 2074 6f20 6368 616e 6765 2066  mand to change f
+00000e80: 7265 7175 656e 6379 2c20 7265 6665 7272  requency, referr
+00000e90: 696e 6720 746f 2074 6865 206d 616e 7561  ing to the manua
+00000ea0: 6c2e 0d0a 5361 7665 2074 6865 202e 7079  l...Save the .py
+00000eb0: 2066 696c 6520 7769 7468 2061 2028 6469   file with a (di
+00000ec0: 6666 6572 656e 7429 2061 7070 726f 7072  fferent) appropr
+00000ed0: 6961 7465 2066 696c 656e 616d 652e 2043  iate filename. C
+00000ee0: 6861 6e67 6520 7468 6520 6069 6e73 743a  hange the `inst:
+00000ef0: 6020 6c69 6e65 2066 6f72 2060 6367 600d  ` line for `cg`.
+00000f00: 0a69 6e20 7468 6520 2e74 6173 6b63 6f6e  .in the .taskcon
+00000f10: 6669 6720 6669 6c65 2074 6f20 6d61 7463  fig file to matc
+00000f20: 6820 7468 6520 6d6f 6475 6c65 2070 6174  h the module pat
+00000f30: 6820 616e 6420 7468 6520 636c 6173 7320  h and the class 
+00000f40: 6e61 6d65 2074 6861 7420 796f 7520 6372  name that you cr
+00000f50: 6561 7465 642e 0d0a 0d0a 2e2e 2063 6f64  eated....... cod
+00000f60: 652d 626c 6f63 6b3a 3a0d 0a20 2020 203a  e-block::..    :
+00000f70: 6c69 6e65 6e6f 733a 0d0a 0d0a 2020 2020  linenos:....    
+00000f80: 6672 6f6d 2073 7273 6775 6920 696d 706f  from srsgui impo
+00000f90: 7274 2049 6e73 7472 756d 656e 740d 0a20  rt Instrument.. 
+00000fa0: 2020 2066 726f 6d20 7372 7367 7569 2e69     from srsgui.i
+00000fb0: 6e73 7420 696d 706f 7274 2046 6c6f 6174  nst import Float
+00000fc0: 436f 6d6d 616e 640d 0a0d 0a20 2020 2063  Command....    c
+00000fd0: 6c61 7373 2043 4736 3335 2849 6e73 7472  lass CG635(Instr
+00000fe0: 756d 656e 7429 3a0d 0a20 2020 2020 2020  ument):..       
+00000ff0: 205f 4964 5374 7269 6e67 203d 2027 4347   _IdString = 'CG
+00001000: 3633 3527 0d0a 2020 2020 2020 2020 6672  635'..        fr
+00001010: 6571 7565 6e63 7920 3d20 466c 6f61 7443  equency = FloatC
+00001020: 6f6d 6d61 6e64 2827 4652 4551 2729 0d0a  ommand('FREQ')..
+00001030: 0d0a 5769 7468 6f75 7420 7265 6465 6669  ..Without redefi
+00001040: 6e69 6e67 202a 2a61 7661 696c 6162 6c65  ning **available
+00001050: 5f69 6e74 6572 6661 6365 732a 2a20 636c  _interfaces** cl
+00001060: 6173 7320 6174 7472 6962 7574 652c 2079  ass attribute, y
+00001070: 6f75 2063 616e 2075 7365 2073 6572 6961  ou can use seria
+00001080: 6c0d 0a63 6f6d 6d75 6e69 6361 7469 6f6e  l..communication
+00001090: 206f 6e6c 792e 2049 6620 796f 7520 7761   only. If you wa
+000010a0: 6e74 2074 6f20 7573 6520 4750 4942 2063  nt to use GPIB c
+000010b0: 6f6d 6d75 6e69 6361 7469 6f6e 2c20 796f  ommunication, yo
+000010c0: 7520 6861 7665 2074 6f20 756e 2d63 6f6d  u have to un-com
+000010d0: 6d65 6e74 2074 6865 0d0a 2a2a 6176 6169  ment the..**avai
+000010e0: 6c61 626c 655f 696e 7465 7266 6163 6573  lable_interfaces
+000010f0: 2a2a 2069 6e20 4347 3633 3520 636c 6173  ** in CG635 clas
+00001100: 732e 0d0a 0d0a 2e2e 2063 6f64 652d 626c  s....... code-bl
+00001110: 6f63 6b3a 3a0d 0a0d 0a20 2020 2066 726f  ock::....    fro
+00001120: 6d20 7372 7367 7569 2069 6d70 6f72 7420  m srsgui import 
+00001130: 5365 7269 616c 496e 7465 7266 6163 652c  SerialInterface,
+00001140: 2046 696e 644c 6973 7449 6e70 7574 0d0a   FindListInput..
+00001150: 2020 2020 6672 6f6d 2073 7273 696e 7374      from srsinst
+00001160: 2e73 7238 3630 2069 6d70 6f72 7420 5669  .sr860 import Vi
+00001170: 7361 496e 7465 7266 6163 650d 0a0d 0a20  saInterface.... 
+00001180: 2020 2061 7661 696c 6162 6c65 5f69 6e74     available_int
+00001190: 6572 6661 6365 7320 3d20 5b0d 0a20 2020  erfaces = [..   
+000011a0: 2020 2020 205b 2020 2053 6572 6961 6c49       [   SerialI
+000011b0: 6e74 6572 6661 6365 2c0d 0a20 2020 2020  nterface,..     
+000011c0: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
+000011d0: 2020 2020 2020 2020 2020 2743 4f4d 2070            'COM p
+000011e0: 6f72 7427 3a20 4669 6e64 4c69 7374 496e  ort': FindListIn
+000011f0: 7075 7428 292c 0d0a 2020 2020 2020 2020  put(),..        
+00001200: 2020 2020 2020 2020 2762 6175 6420 7261          'baud ra
+00001210: 7465 273a 2039 3630 300d 0a20 2020 2020  te': 9600..     
+00001220: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00001230: 2020 5d2c 0d0a 2020 2020 2020 2020 5b20    ],..        [ 
+00001240: 2020 5669 7361 496e 7465 7266 6163 652c    VisaInterface,
+00001250: 0d0a 2020 2020 2020 2020 2020 2020 7b0d  ..            {.
+00001260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001270: 2027 7265 736f 7572 6365 273a 2046 696e   'resource': Fin
+00001280: 644c 6973 7449 6e70 7574 2829 2c0d 0a20  dListInput(),.. 
+00001290: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+000012a0: 2020 2020 2020 5d2c 0d0a 2020 2020 5d0d        ],..    ].
+000012b0: 0a0d 0a59 6f75 206d 7573 7420 696e 7374  ...You must inst
+000012c0: 616c 6c20 6073 7273 696e 7374 2e73 7238  all `srsinst.sr8
+000012d0: 3630 605f 2066 6f72 2056 6973 6149 6e74  60`_ for VisaInt
+000012e0: 6572 6661 6365 2063 6c61 7373 2c20 616e  erface class, an
+000012f0: 6420 5079 5649 5341 5f20 616e 640d 0a69  d PyVISA_ and..i
+00001300: 7473 2062 6163 6b65 6e64 206c 6962 7261  ts backend libra
+00001310: 7279 2c20 666f 6c6c 6f77 696e 6720 5079  ry, following Py
+00001320: 5669 7361 2069 6e73 7461 6c6c 6174 696f  Visa installatio
+00001330: 6e20 696e 7374 7275 6374 696f 6e2e 0d0a  n instruction...
+00001340: 0d0a 4f6e 6365 2074 6865 2043 4736 3335  ..Once the CG635
+00001350: 2028 6f72 2079 6f75 7220 6675 6e63 7469   (or your functi
+00001360: 6f6e 2067 656e 6572 6174 6f72 2920 6973  on generator) is
+00001370: 2063 6f6e 6e65 6374 6564 2c20 0d0a 796f   connected, ..yo
+00001380: 7520 7769 6c6c 2073 6565 2074 6865 2063  u will see the c
+00001390: 6f6e 6e65 6374 696f 6e20 696e 666f 726d  onnection inform
+000013a0: 6174 696f 6e20 696e 2074 6865 2069 6e73  ation in the ins
+000013b0: 7472 756d 656e 7420 696e 666f 2070 616e  trument info pan
+000013c0: 656c 2c0d 0a61 6e64 2079 6f75 2063 616e  el,..and you can
+000013d0: 2075 7365 2069 7420 696e 2074 6865 2074   use it in the t
+000013e0: 6572 6d69 6e61 6c2c 2061 7320 7368 6f77  erminal, as show
+000013f0: 6e20 6265 6c6f 772e 0d0a 0d0a 2e2e 2066  n below....... f
+00001400: 6967 7572 653a 3a20 2e2f 5f73 7461 7469  igure:: ./_stati
+00001410: 632f 6367 2d74 6572 6d69 6e61 6c2d 7363  c/cg-terminal-sc
+00001420: 7265 656e 2d63 6170 7475 7265 2e70 6e67  reen-capture.png
+00001430: 0d0a 2020 2020 3a61 6c69 676e 3a20 6365  ..    :align: ce
+00001440: 6e74 6572 0d0a 2020 2020 3a66 6967 636c  nter..    :figcl
+00001450: 6173 733a 2061 6c69 676e 2d63 656e 7465  ass: align-cente
+00001460: 720d 0a0d 0a7c 0d0a 0d0a 546f 2066 6978  r....|....To fix
+00001470: 2074 6865 2027 4e6f 7420 696d 706c 656d   the 'Not implem
+00001480: 656e 7465 6427 2077 6172 6e69 6e67 2c0d  ented' warning,.
+00001490: 0a3a 6d65 7468 3a60 496e 7374 7275 6d65  .:meth:`Instrume
+000014a0: 6e74 2e67 6574 5f73 7461 7475 7328 2920  nt.get_status() 
+000014b0: 3c73 7273 6775 692e 696e 7374 2e69 6e73  <srsgui.inst.ins
+000014c0: 7472 756d 656e 742e 496e 7374 7275 6d65  trument.Instrume
+000014d0: 6e74 2e67 6574 5f73 7461 7475 733e 600d  nt.get_status>`.
+000014e0: 0a6e 6565 6473 2074 6f20 6265 2072 6564  .needs to be red
+000014f0: 6566 696e 6564 2e20 0d0a 466f 7220 6578  efined. ..For ex
+00001500: 616d 706c 652c 2077 6520 6361 6e20 6f76  ample, we can ov
+00001510: 6572 7269 6465 2069 7420 6173 2066 6f6c  erride it as fol
+00001520: 6c6f 7769 6e67 3a0d 0a0d 0a2e 2e20 636f  lowing:...... co
+00001530: 6465 2d62 6c6f 636b 3a3a 0d0a 0d0a 2020  de-block::....  
+00001540: 2020 6465 6620 6765 745f 7374 6174 7573    def get_status
+00001550: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00001560: 2072 6574 7572 6e20 2753 7461 7475 733a   return 'Status:
+00001570: 204f 4b27 0d0a 0d0a 2849 6620 796f 7520   OK'....(If you 
+00001580: 6172 6520 6661 6d69 6c69 6172 2077 6974  are familiar wit
+00001590: 6820 7374 6174 7573 2062 7974 6573 2c20  h status bytes, 
+000015a0: 796f 7520 6361 6e20 6f76 6572 7269 6465  you can override
+000015b0: 2074 6865 2060 6765 745f 7374 6174 7573   the `get_status
+000015c0: 6020 6d65 7468 6f64 0d0a 746f 2071 7565  ` method..to que
+000015d0: 7279 2074 6865 2073 7461 7475 7320 6279  ry the status by
+000015e0: 7465 2873 2920 616e 6420 7265 7475 726e  te(s) and return
+000015f0: 2074 6865 2072 656c 6576 616e 7420 7374   the relevant st
+00001600: 6174 7573 2069 6e66 6f72 6d61 7469 6f6e  atus information
+00001610: 2061 7320 796f 7520 6465 7369 7265 2e29   as you desire.)
+00001620: 0d0a 0d0a 5765 2077 696c 6c20 7573 6520  ....We will use 
+00001630: 6f6e 6c79 206f 6e65 2063 6f6d 6d61 6e64  only one command
+00001640: 205c 2e66 7265 7175 656e 6379 2c20 6f72   \.frequency, or
+00001650: 2069 7473 2072 6177 2072 656d 6f74 6520   its raw remote 
+00001660: 636f 6d6d 616e 642c 2027 6672 6571 2720  command, 'freq' 
+00001670: 696e 2074 6869 7320 6578 616d 706c 652e  in this example.
+00001680: 0d0a 4265 6361 7573 6520 2763 6727 2069  ..Because 'cg' i
+00001690: 7320 7468 6520 6465 6661 756c 7420 696e  s the default in
+000016a0: 7374 7275 6d65 6e74 2028 7468 6520 6669  strument (the fi
+000016b0: 7273 7420 696e 7374 7275 6d65 6e74 206d  rst instrument m
+000016c0: 656e 7469 6f6e 6564 2069 6e20 7468 6520  entioned in the 
+000016d0: 2e74 6173 6b63 6f6e 6669 6720 6669 6c65  .taskconfig file
+000016e0: 292c 0d0a 616e 7920 7261 7720 7265 6d6f  ),..any raw remo
+000016f0: 7465 2063 6f6d 6d61 6e64 2077 6974 686f  te command witho
+00001700: 7574 2074 6865 2027 6367 3a27 2070 7265  ut the 'cg:' pre
+00001710: 6669 7820 7769 6c6c 2062 6520 7365 6e74  fix will be sent
+00001720: 2074 6f20 6974 2e0d 0a42 6f74 6820 275c   to it...Both '\
+00001730: 2a69 646e 3f27 2061 6e64 2027 6367 3a5c  *idn?' and 'cg:\
+00001740: 2a69 646e 3f27 2077 696c 6c20 7265 7475  *idn?' will retu
+00001750: 726e 2074 6865 2073 616d 6520 7265 706c  rn the same repl
+00001760: 792e 0d0a 0d0a 5765 2075 7365 2074 6865  y.....We use the
+00001770: 2070 7265 6669 7820 2763 673a 2720 666f   prefix 'cg:' fo
+00001780: 7220 7261 7720 7265 6d6f 7465 2063 6f6d  r raw remote com
+00001790: 6d61 6e64 2061 6e64 2074 6865 2070 7265  mand and the pre
+000017a0: 6669 7820 2763 672e 2720 666f 7220 5079  fix 'cg.' for Py
+000017b0: 7468 6f6e 2063 6f6d 6d61 6e64 732e 0d0a  thon commands...
+000017c0: 496e 2074 6865 2074 6572 6d69 6e61 6c20  In the terminal 
+000017d0: 616c 6c20 6174 7472 6962 7574 6573 2061  all attributes a
+000017e0: 6e64 206d 6574 686f 6473 206f 6620 4347  nd methods of CG
+000017f0: 3833 3520 636c 6173 7320 6361 6e20 6265  835 class can be
+00001800: 2075 7365 6420 7769 7468 2070 7265 6669   used with prefi
+00001810: 7820 2763 672e 272e 0d0a 4265 6361 7573  x 'cg.'...Becaus
+00001820: 6520 7765 2064 6566 696e 6564 2066 7265  e we defined fre
+00001830: 7175 656e 6379 2061 7320 6120 466c 6f61  quency as a Floa
+00001840: 7443 6f6d 6d61 6e64 2c20 7765 2063 616e  tCommand, we can
+00001850: 2061 6c73 6f20 7573 6520 7468 6520 2763   also use the 'c
+00001860: 672e 6672 6571 7565 6e63 7927 2070 726f  g.frequency' pro
+00001870: 7065 7274 7920 696e 2074 6865 0d0a 7465  perty in the..te
+00001880: 726d 696e 616c 2e20 5468 6973 206d 6561  rminal. This mea
+00001890: 6e73 2074 6861 7420 7468 6520 666f 6c6c  ns that the foll
+000018a0: 6f77 696e 6720 6172 6520 6571 7569 7661  owing are equiva
+000018b0: 6c65 6e74 3a0d 0a2d 2060 6367 3a66 7265  lent:..- `cg:fre
+000018c0: 7120 3130 302e 3060 0d0a 2d20 6063 672e  q 100.0`..- `cg.
+000018d0: 6672 6571 7565 6e63 7920 3130 3060 0d0a  frequency 100`..
+000018e0: 2020 0d0a 4675 7274 6865 726d 6f72 652c    ..Furthermore,
+000018f0: 2066 726f 6d20 6120 5079 7468 6f6e 2073   from a Python s
+00001900: 6372 6970 742c 206f 6e63 6520 6067 6574  cript, once `get
+00001910: 5f69 6e73 7472 756d 656e 7428 2763 6727  _instrument('cg'
+00001920: 2960 2068 6173 2062 6565 6e20 6361 6c6c  )` has been call
+00001930: 6564 2069 6e20 6120 7461 736b 2063 6c61  ed in a task cla
+00001940: 7373 2c0d 0a79 6f75 2063 616e 2075 7365  ss,..you can use
+00001950: 2060 6367 2e66 7265 7175 656e 6379 203d   `cg.frequency =
+00001960: 2031 3030 6020 696e 2074 6865 2050 7974   100` in the Pyt
+00001970: 686f 6e20 7461 736b 2063 6f64 6520 286f  hon task code (o
+00001980: 7220 6063 672e 6672 6571 7565 6e63 7960  r `cg.frequency`
+00001990: 2061 7320 7468 6520 7175 6572 7920 666f   as the query fo
+000019a0: 726d 292e 0d0a 0d0a 4163 7475 616c 6c79  rm).....Actually
+000019b0: 2079 6f75 2063 616e 2075 7365 2061 6c6c   you can use all
+000019c0: 2074 6865 2061 7474 7269 6275 7465 7320   the attributes 
+000019d0: 616e 6420 6d65 7468 6f64 7320 6465 6669  and methods defi
+000019e0: 6e65 6420 696e 2074 6865 2043 4736 3335  ned in the CG635
+000019f0: 2063 6c61 7373 2061 6e64 2069 7473 2073   class and its s
+00001a00: 7570 6572 2063 6c61 7373 6573 2e0d 0a54  uper classes...T
+00001a10: 6865 2060 6367 2e64 6972 2829 6020 6d65  he `cg.dir()` me
+00001a20: 7468 6f64 2028 7768 6572 6520 6064 6972  thod (where `dir
+00001a30: 2829 6020 6973 2064 6566 696e 6564 2069  ()` is defined i
+00001a40: 6e20 3a63 6c61 7373 3a60 436f 6d70 6f6e  n :class:`Compon
+00001a50: 656e 7420 3c73 7273 6775 692e 696e 7374  ent <srsgui.inst
+00001a60: 2e63 6f6d 706f 6e65 6e74 2e43 6f6d 706f  .component.Compo
+00001a70: 6e65 6e74 3e60 2063 6c61 7373 290d 0a73  nent>` class)..s
+00001a80: 686f 7773 2061 6c6c 2074 6865 2061 7661  hows all the ava
+00001a90: 696c 6162 6c65 2063 6f6d 706f 6e65 6e74  ilable component
+00001aa0: 732c 2063 6f6d 6d61 6e64 732c 2061 6e64  s, commands, and
+00001ab0: 206d 6574 686f 6473 2061 7661 696c 6162   methods availab
+00001ac0: 6c65 2074 6f20 616e 2069 6e73 7461 6e63  le to an instanc
+00001ad0: 6520 6f66 2074 6865 2043 4736 3335 2063  e of the CG635 c
+00001ae0: 6c61 7373 2e20 0d0a 5468 6973 2068 656c  lass. ..This hel
+00001af0: 7073 2075 7320 746f 206e 6176 6967 6174  ps us to navigat
+00001b00: 6520 7468 726f 7567 6820 7265 736f 7572  e through resour
+00001b10: 6365 7320 6176 6169 6c61 626c 6520 7769  ces available wi
+00001b20: 7468 2074 6865 2063 6c61 7373 2e0d 0a0d  th the class....
+00001b30: 0a2e 2e20 6669 6775 7265 3a3a 202e 2f5f  ... figure:: ./_
+00001b40: 7374 6174 6963 2f63 672d 6469 722d 7465  static/cg-dir-te
+00001b50: 726d 696e 616c 2d73 6372 6565 6e2d 6361  rminal-screen-ca
+00001b60: 7074 7572 652e 706e 670d 0a20 2020 203a  pture.png..    :
+00001b70: 616c 6967 6e3a 2063 656e 7465 720d 0a20  align: center.. 
+00001b80: 2020 203a 6669 6763 6c61 7373 3a20 616c     :figclass: al
+00001b90: 6967 6e2d 6365 6e74 6572 0d0a 0d0a 0d0a  ign-center......
+00001ba0: 4372 6163 6b69 6e67 206f 7065 6e20 7468  Cracking open th
+00001bb0: 6520 696e 7374 7275 6d65 6e74 206d 616e  e instrument man
+00001bc0: 7561 6c20 616e 6420 6465 6669 6e69 6e67  ual and defining
+00001bd0: 2075 7365 6675 6c20 6d65 7468 6f64 7320   useful methods 
+00001be0: 696e 2061 6e20 696e 7374 7275 6d65 6e74  in an instrument
+00001bf0: 2063 6c61 7373 200d 0a70 726f 7669 6465   class ..provide
+00001c00: 7320 6561 7365 206f 6620 696e 7374 7275  s ease of instru
+00001c10: 6d65 6e74 2063 6f6e 7472 6f6c 2066 726f  ment control fro
+00001c20: 6d20 6569 7468 6572 2074 6865 2054 6572  m either the Ter
+00001c30: 6d69 6e61 6c20 6f72 2066 726f 6d20 796f  minal or from yo
+00001c40: 7572 2074 6173 6b20 636f 6465 2c20 0d0a  ur task code, ..
+00001c50: 7769 7468 6f75 7420 6861 7669 6e67 2074  without having t
+00001c60: 6f20 7265 6d65 6d62 6572 2074 6865 2072  o remember the r
+00001c70: 656d 6f74 6520 636f 6d6d 616e 6420 6d6e  emote command mn
+00001c80: 656d 6f6e 6963 7320 7468 656d 7365 6c76  emonics themselv
+00001c90: 6573 2e20 0d0a 0d0a 5344 5331 3230 320d  es. ....SDS1202.
+00001ca0: 0a5e 5e5e 5e5e 5e5e 0d0a 0d0a 4576 656e  .^^^^^^^....Even
+00001cb0: 2074 686f 7567 6820 796f 7520 6d61 7920   though you may 
+00001cc0: 6e6f 7420 6861 7665 2061 6e20 5344 5331  not have an SDS1
+00001cd0: 3230 3220 6f73 6369 6c6c 6f73 636f 7065  202 oscilloscope
+00001ce0: 2074 6861 7420 4920 6861 7070 656e 6564   that I happened
+00001cf0: 0d0a 746f 2075 7365 2066 6f72 2074 6869  ..to use for thi
+00001d00: 7320 6578 616d 706c 652c 2049 2062 6574  s example, I bet
+00001d10: 2079 6f75 2063 616e 2066 696e 6420 616e   you can find an
+00001d20: 206f 7363 696c 6c6f 7363 6f70 6520 736f   oscilloscope so
+00001d30: 6d65 7768 6572 650d 0a69 6e20 796f 7572  mewhere..in your
+00001d40: 2062 7569 6c64 696e 672e 2057 6865 6e20   building. When 
+00001d50: 796f 7520 6765 7420 6120 686f 6c64 206f  you get a hold o
+00001d60: 6620 6f6e 652c 2069 7420 6d61 7920 6861  f one, it may ha
+00001d70: 7665 2061 2055 5342 2063 6f6e 6e65 6374  ve a USB connect
+00001d80: 6f72 206f 6e6c 792c 0d0a 6c69 6b65 2061  or only,..like a
+00001d90: 206c 6f74 206f 6620 6261 7365 206d 6f64   lot of base mod
+00001da0: 656c 206f 7363 696c 6c6f 7363 6f70 6573  el oscilloscopes
+00001db0: 2064 6f2e 0d0a 5468 6973 206d 6561 6e73   do...This means
+00001dc0: 2079 6f75 206d 6179 2068 6176 6520 746f   you may have to
+00001dd0: 2075 7365 2055 5342 2d54 4d43 2069 6e74   use USB-TMC int
+00001de0: 6572 6661 6365 2e20 0d0a 496e 206f 7264  erface. ..In ord
+00001df0: 6572 2074 6f20 646f 2074 6861 742c 2079  er to do that, y
+00001e00: 6f75 206e 6565 6420 746f 2069 6e73 7461  ou need to insta
+00001e10: 6c6c 2050 7956 4953 412e 200d 0a59 6f75  ll PyVISA. ..You
+00001e20: 206e 6565 6420 746f 2075 6e63 6f6d 6d65   need to uncomme
+00001e30: 6e74 2074 6865 2061 7661 696c 6162 6c65  nt the available
+00001e40: 5f69 6e74 6572 6661 6365 7320 6f66 2053  _interfaces of S
+00001e50: 4453 3132 3032 2063 6c61 7373 2c20 0d0a  DS1202 class, ..
+00001e60: 6d6f 6469 6679 2069 7420 746f 2066 6974  modify it to fit
+00001e70: 2074 6865 2073 7065 6369 6669 6361 7469   the specificati
+00001e80: 6f6e 206f 6620 796f 7572 206f 7363 696c  on of your oscil
+00001e90: 6c6f 7363 6f70 652c 2061 6c6f 6e67 2077  loscope, along w
+00001ea0: 6974 680d 0a63 6861 6e67 696e 6720 746f  ith..changing to
+00001eb0: 2074 6865 2063 6f72 7265 6374 2060 5f49   the correct `_I
+00001ec0: 6453 7472 696e 6760 2e20 0d0a 5468 656e  dString`. ..Then
+00001ed0: 2079 6f75 2068 6176 6520 746f 2067 6574   you have to get
+00001ee0: 2077 6176 6566 6f72 6d20 646f 776e 6c6f   waveform downlo
+00001ef0: 6164 2077 6f72 6b69 6e67 2c20 7768 6963  ad working, whic
+00001f00: 6820 6f66 7465 6e20 696e 766f 6c76 6573  h often involves
+00001f10: 2072 6563 6965 7669 6e67 2061 6e64 2070   recieving and p
+00001f20: 726f 7065 726c 7920 7061 7273 696e 6720  roperly parsing 
+00001f30: 6269 6e61 7279 2064 6174 610d 0a28 6269  binary data..(bi
+00001f40: 6e61 7279 2064 6174 6120 6973 2075 7365  nary data is use
+00001f50: 6420 746f 206d 696e 696d 697a 6520 7468  d to minimize th
+00001f60: 6520 6e75 6d62 6572 206f 6620 6368 6172  e number of char
+00001f70: 6163 7465 7273 2073 656e 7420 6f76 6572  acters sent over
+00001f80: 2074 6865 2072 656d 6f74 6520 636f 6d6d   the remote comm
+00001f90: 756e 6963 6174 696f 6e20 696e 7465 7266  unication interf
+00001fa0: 6163 652c 0d0a 7468 6572 6562 7920 6d61  ace,..thereby ma
+00001fb0: 6b69 6e67 2064 6174 6120 7472 616e 7366  king data transf
+00001fc0: 6572 7320 6f66 2070 6572 6861 7073 2076  ers of perhaps v
+00001fd0: 6572 7920 6c65 6e67 7468 7920 7761 7665  ery lengthy wave
+00001fe0: 666f 726d 7320 7265 6c61 7469 7665 6c79  forms relatively
+00001ff0: 2066 6173 7429 2e0d 0a49 6620 796f 7520   fast)...If you 
+00002000: 6172 6520 6c75 636b 792c 2079 6f75 2063  are lucky, you c
+00002010: 616e 2066 696e 6420 6120 776f 726b 696e  an find a workin
+00002020: 6720 5079 7468 6f6e 2073 6e69 7070 6574  g Python snippet
+00002030: 2066 726f 6d20 6a75 6469 6369 6f75 7320   from judicious 
+00002040: 7765 6220 7365 6172 6368 2e0d 0a49 6620  web search...If 
+00002050: 6e6f 742c 2079 6f75 2068 6176 6520 746f  not, you have to
+00002060: 2064 6563 6970 6865 7220 7468 6520 7072   decipher the pr
+00002070: 6f67 7261 6d6d 696e 6720 6d61 6e75 616c  ogramming manual
+00002080: 206f 6620 7468 6520 6f73 6369 6c6c 6f73   of the oscillos
+00002090: 636f 7065 2e20 0d0a 4974 206d 6179 2074  cope. ..It may t
+000020a0: 616b 6520 7469 6d65 2c20 6275 7420 6974  ake time, but it
+000020b0: 2077 696c 6c20 6265 2076 6572 7920 7265   will be very re
+000020c0: 7761 7264 696e 6720 666f 7220 796f 7572  warding for your
+000020d0: 2064 6174 6120 6163 7175 6973 6974 696f   data acquisitio
+000020e0: 6e0d 0a73 6b69 6c6c 2d73 6574 2069 6d70  n..skill-set imp
+000020f0: 726f 7665 6d65 6e74 2e0d 0a0d 0a4f 7468  rovement.....Oth
+00002100: 6572 2074 6861 6e20 7468 6520 6269 6e61  er than the bina
+00002110: 7279 2077 6176 6566 6f72 6d20 646f 776e  ry waveform down
+00002120: 6c6f 6164 2c20 0d0a 6d6f 7374 206f 7468  load, ..most oth
+00002130: 6572 2063 6f6d 6d61 6e64 7320 666f 7220  er commands for 
+00002140: 696e 7465 7261 6374 696e 6720 7769 7468  interacting with
+00002150: 2074 6865 206f 7363 696c 6c6f 7363 6f70   the oscilloscop
+00002160: 6520 0d0a 7769 6c6c 2062 6520 7374 616e  e ..will be stan
+00002170: 6461 7264 2041 5343 4949 2d62 6173 6564  dard ASCII-based
+00002180: 2074 6578 7420 636f 6d6d 616e 6473 2e0d   text commands..
+00002190: 0a0d 0a2e 2e20 6e6f 7465 3a3a 0d0a 2020  ..... note::..  
+000021a0: 5769 7468 2064 6566 6175 6c74 2061 7661  With default ava
+000021b0: 696c 6162 6c65 5f69 6e74 6572 6661 6365  ilable_interface
+000021c0: 7320 6f66 2049 6e73 7472 756d 656e 7420  s of Instrument 
+000021d0: 636c 6173 732c 2054 6370 6970 496e 7465  class, TcpipInte
+000021e0: 7266 6163 6520 7368 6f75 6c64 2062 6520  rface should be 
+000021f0: 7573 6564 2077 6974 6820 706f 7274 2035  used with port 5
+00002200: 3032 352e 0d0a 0d0a 5468 6520 696e 7374  025.....The inst
+00002210: 7275 6d65 6e74 2064 7269 7665 7220 666f  rument driver fo
+00002220: 7220 5344 5331 3230 3220 7769 6c6c 2077  r SDS1202 will w
+00002230: 6f72 6b20 7769 7468 2034 206c 696e 6573  ork with 4 lines
+00002240: 206f 6620 636f 6465 2c20 6a75 7374 206c   of code, just l
+00002250: 696b 6520 7468 6520 4347 3633 352c 0d0a  ike the CG635,..
+00002260: 6265 666f 7265 2061 6464 696e 6720 7468  before adding th
+00002270: 6520 6d65 7468 6f64 2074 6f20 646f 776e  e method to down
+00002280: 6c6f 6164 2077 6176 6566 6f72 6d73 2066  load waveforms f
+00002290: 726f 6d20 7468 6520 6f73 6369 6c6c 6f73  rom the oscillos
+000022a0: 636f 7065 2e20 0d0a 4164 6420 6174 7472  cope. ..Add attr
+000022b0: 6962 7574 6573 2061 6e64 206d 6574 686f  ibutes and metho
+000022c0: 6473 2069 6e63 7265 6d65 6e74 616c 6c79  ds incrementally
+000022d0: 2061 7320 796f 7520 6e65 6564 2074 6f20   as you need to 
+000022e0: 7573 6520 6d6f 7265 2066 756e 6374 696f  use more functio
+000022f0: 6e73 206f 6620 7468 6520 696e 7374 7275  ns of the instru
+00002300: 6d65 6e74 2e0d 0a0d 0a2e 2e20 636f 6465  ment....... code
+00002310: 2d62 6c6f 636b 3a3a 0d0a 2020 2020 3a6c  -block::..    :l
+00002320: 696e 656e 6f73 3a0d 0a0d 0a20 2020 2069  inenos:....    i
+00002330: 6d70 6f72 7420 6e75 6d70 7920 6173 206e  mport numpy as n
+00002340: 700d 0a20 2020 2066 726f 6d20 7372 7367  p..    from srsg
+00002350: 7569 2069 6d70 6f72 7420 496e 7374 7275  ui import Instru
+00002360: 6d65 6e74 0d0a 0d0a 2020 2020 636c 6173  ment....    clas
+00002370: 7320 5344 5331 3230 3228 496e 7374 7275  s SDS1202(Instru
+00002380: 6d65 6e74 293a 0d0a 2020 2020 2020 2020  ment):..        
+00002390: 5f49 6453 7472 696e 6720 3d20 2753 4453  _IdString = 'SDS
+000023a0: 3132 3032 270d 0a0d 0a20 2020 2020 2020  1202'....       
+000023b0: 2064 6566 2067 6574 5f77 6176 6566 6f72   def get_wavefor
+000023c0: 6d28 7365 6c66 2c20 6368 616e 6e65 6c29  m(self, channel)
+000023d0: 3a0d 0a20 2020 2020 2020 2020 2020 202e  :..            .
+000023e0: 2e2e 0d0a 0d0a 2020 2020 2020 2020 6465  ......        de
+000023f0: 6620 6765 745f 7361 6d70 6c69 6e67 5f72  f get_sampling_r
+00002400: 6174 6528 7365 6c66 293a 0d0a 2020 2020  ate(self):..    
+00002410: 2020 2020 2020 2020 2e2e 2e0d 0a0d 0a4f          .......O
+00002420: 6e63 6520 7468 6520 6f73 6369 6c6c 6f73  nce the oscillos
+00002430: 636f 7065 2069 7320 636f 6e6e 6563 7465  cope is connecte
+00002440: 6420 746f 2074 6865 2061 7070 6c69 6361  d to the applica
+00002450: 7469 6f6e 2c20 796f 7520 6361 6e20 7573  tion, you can us
+00002460: 6520 7468 6520 7465 726d 696e 616c 2074  e the terminal t
+00002470: 6f20 6578 706c 6f72 6520 7468 6520 6f73  o explore the os
+00002480: 6369 6c6c 6f73 636f 7065 2e0d 0a0d 0a2e  cilloscope......
+00002490: 2e20 6669 6775 7265 3a3a 202e 2f5f 7374  . figure:: ./_st
+000024a0: 6174 6963 2f6f 7363 2d64 6972 2d74 6572  atic/osc-dir-ter
+000024b0: 6d69 6e61 6c2d 7363 7265 656e 2d63 6170  minal-screen-cap
+000024c0: 7475 7265 2e70 6e67 0d0a 2020 2020 3a61  ture.png..    :a
+000024d0: 6c69 676e 3a20 6365 6e74 6572 0d0a 2020  lign: center..  
+000024e0: 2020 3a66 6967 636c 6173 733a 2061 6c69    :figclass: ali
+000024f0: 676e 2d63 656e 7465 720d 0a0d 0a7c 0d0a  gn-center....|..
+00002500: 0d0a 4265 6361 7573 6520 276f 7363 2720  ..Because 'osc' 
+00002510: 6973 206e 6f74 2074 6865 2064 6566 6175  is not the defau
+00002520: 6c74 2069 6e73 7472 756d 656e 742c 2079  lt instrument, y
+00002530: 6f75 2068 6176 6520 746f 2075 7365 2074  ou have to use t
+00002540: 6865 2070 7265 6669 7820 276f 7363 3a27  he prefix 'osc:'
+00002550: 2077 6974 6820 616c 6c20 7468 650d 0a72   with all the..r
+00002560: 6177 2072 656d 6f74 6520 636f 6d6d 616e  aw remote comman
+00002570: 6473 2079 6f75 2073 656e 6420 746f 2074  ds you send to t
+00002580: 6865 2069 6e73 7472 756d 656e 742e 2041  he instrument. A
+00002590: 7320 7368 6f77 6e20 7769 7468 2027 6f73  s shown with 'os
+000025a0: 632e 6469 7227 2c20 7468 6572 6520 6172  c.dir', there ar
+000025b0: 6520 6d61 6e79 206d 6574 686f 6473 0d0a  e many methods..
+000025c0: 6176 6169 6c61 626c 6520 7769 7468 2027  available with '
+000025d0: 6f73 632e 2720 4576 656e 206f 7363 2e67  osc.' Even osc.g
+000025e0: 6574 5f77 6176 6566 6f72 6d28 2920 6973  et_waveform() is
+000025f0: 2061 7661 696c 6162 6c65 2066 726f 6d20   available from 
+00002600: 7468 6520 7465 726d 696e 616c 2e20 0d0a  the terminal. ..
+00002610: 5768 656e 2079 6f75 2075 7365 2061 206d  When you use a m
+00002620: 6574 686f 6420 696e 636f 7272 6563 746c  ethod incorrectl
+00002630: 792c 2074 6865 2074 6572 6d69 6e61 6c20  y, the terminal 
+00002640: 6b69 6e64 6c79 2074 656c 6c73 206d 6520  kindly tells me 
+00002650: 7468 6174 2074 6865 7265 2069 7320 6120  that there is a 
+00002660: 6d69 7373 696e 6720 6172 6775 6d65 6e74  missing argument
+00002670: 200d 0a69 6e20 6120 6675 6e63 7469 6f6e   ..in a function
+00002680: 2063 616c 6c2e 0d0a 596f 7520 6361 6e20   call...You can 
+00002690: 7365 6520 606f 7363 2e67 6574 5f77 6176  see `osc.get_wav
+000026a0: 6566 6f72 6d28 6368 616e 6e65 6c29 6020  eform(channel)` 
+000026b0: 7265 7475 726e 7320 7477 6f20 6e75 6d70  returns two nump
+000026c0: 7920 6172 7261 7973 2e0d 0a57 6861 7420  y arrays...What 
+000026d0: 6966 2079 6f75 2077 616e 7420 746f 2070  if you want to p
+000026e0: 6c6f 7420 7468 6520 6461 7461 3f0d 0a41  lot the data?..A
+000026f0: 7320 7468 6520 6d65 7468 6f64 7320 796f  s the methods yo
+00002700: 7520 696d 706c 656d 656e 7420 666f 7220  u implement for 
+00002710: 696e 7465 7261 6374 696e 6720 7769 7468  interacting with
+00002720: 2079 6f75 7220 696e 7374 7275 6d65 6e74   your instrument
+00002730: 7320 616e 6420 6461 7461 2067 726f 7720  s and data grow 
+00002740: 696e 2063 6f6d 706c 6578 6974 792c 0d0a  in complexity,..
+00002750: 796f 7520 6d61 7920 6e65 6564 2074 6f20  you may need to 
+00002760: 6772 6164 7561 7465 2066 726f 6d20 7465  graduate from te
+00002770: 726d 696e 616c 2d62 6173 6564 2069 6e74  rminal-based int
+00002780: 6572 6163 7469 6f6e 2074 6f20 7461 736b  eraction to task
+00002790: 2d62 6173 6564 2069 6e74 6572 6163 7469  -based interacti
+000027a0: 6f6e 2e20 5265 6164 206f 6e2e 0d0a 0d0a  on. Read on.....
+000027b0: 5461 736b 730d 0a2d 2d2d 2d2d 2d2d 0d0a  Tasks..-------..
+000027c0: 0d0a 486f 7720 746f 2072 756e 2061 2074  ..How to run a t
+000027d0: 6173 6b0d 0a5e 5e5e 5e5e 5e5e 5e5e 5e5e  ask..^^^^^^^^^^^
+000027e0: 5e5e 5e5e 5e5e 5e5e 0d0a 0d0a 5374 6172  ^^^^^^^^....Star
+000027f0: 7420 7468 6520 6060 7372 7367 7569 6060  t the ``srsgui``
+00002800: 2061 7070 6c69 6361 7469 6f6e 2e20 596f   application. Yo
+00002810: 7520 6361 6e20 7365 6520 7768 6572 6520  u can see where 
+00002820: 7468 6520 2e74 6173 6b63 6f6e 6669 6720  the .taskconfig 
+00002830: 6669 6c65 2069 7320 6f70 656e 6564 0d0a  file is opened..
+00002840: 6672 6f6d 2074 6865 2063 6f6e 736f 6c65  from the console
+00002850: 2077 696e 646f 7720 283a 7265 663a 6068   window (:ref:`h
+00002860: 6572 6520 3c74 6f70 2d6f 662d 696e 6974  ere <top-of-init
+00002870: 6961 6c2d 7363 7265 656e 2d63 6170 7475  ial-screen-captu
+00002880: 7265 3e60 292e 0d0a 4966 2079 6f75 206d  re>`)...If you m
+00002890: 6164 6520 6120 636f 7079 206f 6620 7468  ade a copy of th
+000028a0: 6520 6f72 6967 696e 616c 2065 7861 6d70  e original examp
+000028b0: 6c65 2066 726f 6d20 7468 6520 6060 7372  le from the ``sr
+000028c0: 7367 7569 6060 0d0a 7061 636b 6167 6520  sgui``..package 
+000028d0: 6469 7265 6374 6f72 792c 206f 7065 6e20  directory, open 
+000028e0: 6974 2061 6761 696e 2066 726f 6d20 7468  it again from th
+000028f0: 6520 636f 7272 6563 7420 6469 7265 6374  e correct direct
+00002900: 6f72 792e 0d0a 0d0a 4966 2074 6865 7265  ory.....If there
+00002910: 2061 7265 206e 6f20 6572 726f 7220 6d65   are no error me
+00002920: 7373 6167 6573 2069 6e20 7468 6520 436f  ssages in the Co
+00002930: 6e73 6f6c 6520 7769 6e64 6f77 2c20 636f  nsole window, co
+00002940: 6e6e 6563 7420 7468 6520 6675 6e63 7469  nnect the functi
+00002950: 6f6e 2067 656e 6572 6174 6f72 0d0a 616e  on generator..an
+00002960: 6420 7468 6520 6f73 6369 6c6c 6f73 636f  d the oscillosco
+00002970: 7065 2066 726f 6d20 7468 6520 496e 7374  pe from the Inst
+00002980: 7275 6d65 6e74 7320 6d65 6e75 2e0d 0a0d  ruments menu....
+00002990: 0a54 6865 206f 7665 7261 6c6c 2073 7472  .The overall str
+000029a0: 7563 7475 7265 206f 6620 6120 7461 736b  ucture of a task
+000029b0: 2069 7320 6465 7363 7269 6265 6420 696e   is described in
+000029c0: 203a 7265 663a 6057 7269 7469 6e67 2061   :ref:`Writing a
+000029d0: 2074 6173 6b20 7363 7269 7074 6020 7365   task script` se
+000029e0: 6374 696f 6e2e 0d0a 5468 6572 6520 6172  ction...There ar
+000029f0: 6520 3520 7461 736b 7320 6172 6520 696e  e 5 tasks are in
+00002a00: 636c 7564 6564 2069 6e20 7468 6520 6578  cluded in the ex
+00002a10: 616d 706c 6520 7072 6f6a 6563 742e 2054  ample project. T
+00002a20: 6865 7920 6772 6164 7561 6c6c 7920 6164  hey gradually ad
+00002a30: 6420 6d6f 7265 2066 6561 7475 7265 730d  d more features.
+00002a40: 0a6f 6e20 7468 6520 746f 7020 6f66 2074  .on the top of t
+00002a50: 6865 2070 7265 7669 6f75 7320 7461 736b  he previous task
+00002a60: 732e 200d 0a54 6865 7920 6172 6520 6465  s. ..They are de
+00002a70: 7369 676e 6564 2074 6f20 7368 6f77 6361  signed to showca
+00002a80: 7365 2068 6f77 2074 6f20 7573 6520 7468  se how to use th
+00002a90: 6520 5461 736b 2063 6c61 7373 2e0d 0a0d  e Task class....
+00002aa0: 0a53 656c 6563 7420 7468 6520 6669 7273  .Select the firs
+00002ab0: 7420 7461 736b 2028 5c2a 4944 4e20 7465  t task (\*IDN te
+00002ac0: 7374 2920 6672 6f6d 2074 6865 2054 6173  st) from the Tas
+00002ad0: 6b73 206d 656e 750d 0a61 6e64 2063 6c69  ks menu..and cli
+00002ae0: 636b 2074 6865 2067 7265 656e 2061 7272  ck the green arr
+00002af0: 6f77 2069 6e20 7468 6520 746f 6f6c 2062  ow in the tool b
+00002b00: 6172 2074 6f20 7275 6e20 7468 6520 7461  ar to run the ta
+00002b10: 736b 2e0d 0a0d 0a49 6465 6e74 6966 7920  sk.....Identify 
+00002b20: 7461 736b 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d  task..----------
+00002b30: 2d2d 2d2d 0d0a 0d0a 5468 6520 4964 656e  ----....The Iden
+00002b40: 7469 6679 2074 6173 6b20 7368 6f77 733a  tify task shows:
+00002b50: 0d0a 0d0a 2020 2020 2d20 486f 7720 746f  ....    - How to
+00002b60: 2075 7365 206d 6f64 756c 652d 6c65 7665   use module-leve
+00002b70: 6c20 6c6f 6767 6572 2066 6f72 2050 7974  l logger for Pyt
+00002b80: 686f 6e20 6c6f 6767 696e 675f 2069 6e20  hon logging_ in 
+00002b90: 6120 7461 736b 0d0a 2020 2020 2d20 486f  a task..    - Ho
+00002ba0: 7720 746f 2075 7365 2069 6e73 7472 756d  w to use instrum
+00002bb0: 656e 7473 2064 6566 696e 6564 2069 6e20  ents defined in 
+00002bc0: 7468 6520 636f 6e66 6967 7572 6174 696f  the configuratio
+00002bd0: 6e20 6669 6c65 0d0a 2020 2020 2d20 486f  n file..    - Ho
+00002be0: 7720 746f 2075 7365 2074 6578 7420 6f75  w to use text ou
+00002bf0: 7470 7574 2074 6f20 7468 6520 636f 6e73  tput to the cons
+00002c00: 6f6c 6520 7769 6e64 6f77 0d0a 0d0a 4974  ole window....It
+00002c10: 2069 7320 6e6f 7420 6d75 6368 2064 6966   is not much dif
+00002c20: 6665 7265 6e74 2066 726f 6d20 7468 6520  ferent from the 
+00002c30: 3a72 6566 3a60 6261 7265 2062 6f6e 6520  :ref:`bare bone 
+00002c40: 7374 7275 6374 7572 6520 3c74 6f70 2d6f  structure <top-o
+00002c50: 662d 6261 7265 2d62 6f6e 652d 7461 736b  f-bare-bone-task
+00002c60: 3e60 0d0a 7368 6f77 6e20 696e 2074 6865  >`..shown in the
+00002c70: 203a 7265 663a 6057 7269 7469 6e67 2061   :ref:`Writing a
+00002c80: 2074 6173 6b20 7363 7269 7074 6020 7365   task script` se
+00002c90: 6374 696f 6e2e 0d0a 0d0a 2e2e 206c 6974  ction....... lit
+00002ca0: 6572 616c 696e 636c 7564 653a 3a20 2e2e  eralinclude:: ..
+00002cb0: 2f73 7273 6775 692f 6578 616d 706c 6573  /srsgui/examples
+00002cc0: 2f6f 7363 696c 6c6f 7363 6f70 6520 6578  /oscilloscope ex
+00002cd0: 616d 706c 652f 7461 736b 732f 6964 656e  ample/tasks/iden
+00002ce0: 7469 6679 2e70 790d 0a20 2020 203a 6c61  tify.py..    :la
+00002cf0: 6e67 7561 6765 3a20 5079 7468 6f6e 0d0a  nguage: Python..
+00002d00: 2020 2020 3a6c 696e 656e 6f73 3a0d 0a0d      :linenos:...
+00002d10: 0a55 7369 6e67 202a 2a73 656c 662e 6c6f  .Using **self.lo
+00002d20: 6767 6572 2a2a 2073 656e 6473 2074 6865  gger** sends the
+00002d30: 206c 6f67 6769 6e67 206f 7574 7075 7420   logging output 
+00002d40: 746f 2074 6865 2063 6f6e 736f 6c65 2077  to the console w
+00002d50: 696e 646f 772c 2074 6865 206d 6173 7465  indow, the maste
+00002d60: 7220 6c6f 6767 696e 6720 6669 6c65 2069  r logging file i
+00002d70: 6e0d 0a60 7e2f 7461 736b 2d72 6573 756c  n..`~/task-resul
+00002d80: 7473 2064 6972 6563 746f 7279 2f6d 6169  ts directory/mai
+00002d90: 6e6c 6f67 2d78 782e 7478 742e 7860 2c20  nlog-xx.txt.x`, 
+00002da0: 616e 6420 746f 2074 6865 2074 6173 6b20  and to the task 
+00002db0: 7265 7375 6c74 2064 6174 6120 6669 6c65  result data file
+00002dc0: 206c 6f63 6174 6564 2069 6e0d 0a60 7e2f   located in..`~/
+00002dd0: 7461 736b 2d72 6573 756c 7473 2f70 726f  task-results/pro
+00002de0: 6a65 6374 2d6e 616d 652d 696e 2d63 6f6e  ject-name-in-con
+00002df0: 6669 672d 6669 6c65 2f52 4e78 7878 6020  fig-file/RNxxx` 
+00002e00: 6469 7265 6374 6f72 792e 0d0a 0d0a 5769  directory.....Wi
+00002e10: 7468 203a 6d65 7468 3a60 6765 745f 696e  th :meth:`get_in
+00002e20: 7374 7275 6d65 6e74 203c 7372 7367 7569  strument <srsgui
+00002e30: 2e74 6173 6b2e 7461 736b 2e54 6173 6b2e  .task.task.Task.
+00002e40: 6765 745f 696e 7374 7275 6d65 6e74 3e60  get_instrument>`
+00002e50: 2079 6f75 2063 616e 2067 6574 2074 6865   you can get the
+00002e60: 2069 6e73 7472 756d 656e 740d 0a64 6566   instrument..def
+00002e70: 696e 6564 2069 6e20 7468 6520 636f 6e66  ined in the conf
+00002e80: 6967 7572 6174 696f 6e20 6669 6c65 2069  iguration file i
+00002e90: 6e20 6120 7461 736b 2e20 2a2a 446f 206e  n a task. **Do n
+00002ea0: 6f74 2064 6973 636f 6e6e 6563 7420 7468  ot disconnect th
+00002eb0: 6520 696e 7374 7275 6d65 6e74 2069 6e20  e instrument in 
+00002ec0: 7468 6520 7461 736b 212a 2a0d 0a49 6e73  the task!**..Ins
+00002ed0: 7472 756d 656e 7420 436f 6e6e 6563 7469  trument Connecti
+00002ee0: 7669 7479 2069 7320 6d61 6e61 6765 6420  vity is managed 
+00002ef0: 6174 2074 6865 2060 6073 7273 6775 6960  at the ``srsgui`
+00002f00: 6020 6170 706c 6963 6174 696f 6e20 6c65  ` application le
+00002f10: 7665 6c2e 0d0a 0d0a 5468 6973 2074 6173  vel.....This tas
+00002f20: 6b20 6869 6768 6c69 6768 7473 2068 6f77  k highlights how
+00002f30: 2072 656d 6f74 6520 636f 6d6d 616e 6420   remote command 
+00002f40: 7365 7420 616e 6420 7175 6572 7920 7472  set and query tr
+00002f50: 616e 7361 6374 696f 6e73 2061 7265 2073  ansactions are s
+00002f60: 696d 706c 6966 6965 6420 6279 2064 6566  implified by def
+00002f70: 696e 696e 6720 0d0a 616e 2061 7474 7269  ining ..an attri
+00002f80: 6275 7465 2075 7369 6e67 203a 6d6f 643a  bute using :mod:
+00002f90: 6073 7273 6775 692e 696e 7374 2e63 6f6d  `srsgui.inst.com
+00002fa0: 6d61 6e64 7360 206d 6f64 756c 652c 200d  mands` module, .
+00002fb0: 0a77 6869 6368 2069 7320 7574 696c 697a  .which is utiliz
+00002fc0: 6564 2069 6e20 7468 6520 4347 3633 3520  ed in the CG635 
+00002fd0: 636c 6173 7320 6465 6669 6e69 7469 6f6e  class definition
+00002fe0: 2076 6961 2074 6865 2066 6f6c 6c6f 7769   via the followi
+00002ff0: 6e67 206c 696e 653a 2020 0d0a 0d0a 6060  ng line:  ....``
+00003000: 6672 6571 7565 6e63 7920 3d20 466c 6f61  frequency = Floa
+00003010: 7443 6f6d 6d61 6e64 2827 4652 4551 2729  tCommand('FREQ')
+00003020: 6060 0d0a 0d0a 5468 6973 2073 696d 706c  ``....This simpl
+00003030: 6520 6c69 6e65 206d 616b 6573 2069 7420  e line makes it 
+00003040: 706f 7373 6962 6c65 2074 6f20 7365 7420  possible to set 
+00003050: 616e 6420 7175 6572 7920 7468 6520 6063  and query the `c
+00003060: 672e 6672 6571 7565 6e63 7960 200d 0a77  g.frequency` ..w
+00003070: 6974 686f 7574 2068 6176 696e 6720 746f  ithout having to
+00003080: 2064 6972 6563 746c 7920 6d61 6e69 7075   directly manipu
+00003090: 6c61 7465 2063 6f6d 6d61 6e64 206f 7220  late command or 
+000030a0: 7265 7370 6f6e 7365 2073 7472 696e 6773  response strings
+000030b0: 2e20 0d0a 0d0a 506c 6f74 4578 616d 706c  . ....PlotExampl
+000030c0: 6520 7461 736b 0d0a 2d2d 2d2d 2d2d 2d2d  e task..--------
+000030d0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a54 6865  ---------....The
+000030e0: 2050 6c6f 7445 7861 6d70 6c65 2074 6173   PlotExample tas
+000030f0: 6b20 7265 7175 6972 6573 206e 6f20 696e  k requires no in
+00003100: 7374 7275 6d65 6e74 2063 6f6e 6e65 6374  strument connect
+00003110: 696f 6e73 2c20 616e 6420 7368 6f77 733a  ions, and shows:
+00003120: 0d0a 0d0a 2020 2020 2d20 486f 7720 746f  ....    - How to
+00003130: 2064 6566 696e 6520 3a61 7474 723a 6069   define :attr:`i
+00003140: 6e70 7574 5f70 6172 616d 6574 6572 7320  nput_parameters 
+00003150: 3c73 7273 6775 692e 7461 736b 2e74 6173  <srsgui.task.tas
+00003160: 6b2e 5461 736b 2e69 6e70 7574 5f70 6172  k.Task.input_par
+00003170: 616d 6574 6572 733e 600d 0a20 2020 2020  ameters>`..     
+00003180: 2066 6f72 2069 6e74 6572 6163 7469 7665   for interactive
+00003190: 2075 7365 7220 696e 7075 7420 6672 6f6d   user input from
+000031a0: 2074 6865 2061 7070 6c69 6361 7469 6f6e   the application
+000031b0: 2069 6e70 7574 2070 616e 656c 0d0a 2020   input panel..  
+000031c0: 2020 2d20 486f 7720 746f 2075 7365 206d    - How to use m
+000031d0: 6174 706c 6f74 6c69 6220 6669 6775 7265  atplotlib figure
+000031e0: 7320 666f 7220 706c 6f74 7469 6e67 2064  s for plotting d
+000031f0: 6174 610d 0a20 2020 202d 2048 6f77 2074  ata..    - How t
+00003200: 6f20 7365 6e64 2074 6578 7420 6f75 7470  o send text outp
+00003210: 7574 2074 6f20 7468 6520 7265 7375 6c74  ut to the result
+00003220: 2077 696e 646f 7720 7573 696e 670d 0a20   window using.. 
+00003230: 2020 2020 203a 6d65 7468 3a60 6469 7370       :meth:`disp
+00003240: 6c61 795f 7265 7375 6c74 2829 203c 7372  lay_result() <sr
+00003250: 7367 7569 2e74 6173 6b2e 7461 736b 2e54  sgui.task.task.T
+00003260: 6173 6b2e 6469 7370 6c61 795f 7265 7375  ask.display_resu
+00003270: 6c74 3e60 0d0a 2020 2020 2d20 486f 7720  lt>`..    - How 
+00003280: 746f 2073 746f 7020 7468 6520 7461 736b  to stop the task
+00003290: 2062 7920 6368 6563 6b69 6e67 0d0a 2020   by checking..  
+000032a0: 2020 2020 3a6d 6574 683a 6069 735f 7275      :meth:`is_ru
+000032b0: 6e6e 696e 6728 2920 3c73 7273 6775 692e  nning() <srsgui.
+000032c0: 7461 736b 2e74 6173 6b2e 5461 736b 2e69  task.task.Task.i
+000032d0: 735f 7275 6e6e 696e 673e 602e 0d0a 0d0a  s_running>`.....
+000032e0: 2e2e 206c 6974 6572 616c 696e 636c 7564  .. literalinclud
+000032f0: 653a 3a20 2e2e 2f73 7273 6775 692f 6578  e:: ../srsgui/ex
+00003300: 616d 706c 6573 2f6f 7363 696c 6c6f 7363  amples/oscillosc
+00003310: 6f70 6520 6578 616d 706c 652f 7461 736b  ope example/task
+00003320: 732f 706c 6f74 5f65 7861 6d70 6c65 2e70  s/plot_example.p
+00003330: 790d 0a20 2020 203a 6c61 6e67 7561 6765  y..    :language
+00003340: 3a20 5079 7468 6f6e 0d0a 2020 2020 3a6c  : Python..    :l
+00003350: 696e 656e 6f73 3a0d 0a0d 0a55 7369 6e67  inenos:....Using
+00003360: 206d 6174 706c 6f74 6c69 625f 2077 6974   matplotlib_ wit
+00003370: 6820 6060 7372 7367 7569 6060 2069 7320  h ``srsgui`` is 
+00003380: 7374 7261 6967 6874 666f 7277 6172 6420  straightforward 
+00003390: 6966 2079 6f75 2061 7265 2061 6c72 6561  if you are alrea
+000033a0: 6479 2066 616d 696c 6961 7220 7769 7468  dy familiar with
+000033b0: 2069 7473 2075 7361 6765 2e0d 0a28 5265   its usage...(Re
+000033c0: 6665 7220 746f 206d 6174 706c 6f74 6c69  fer to matplotli
+000033d0: 625f 2064 6f63 756d 656e 7461 7469 6f6e  b_ documentation
+000033e0: 292e 0d0a 0d0a 5468 6520 696d 706f 7274  ).....The import
+000033f0: 616e 7420 6469 6666 6572 656e 6365 7320  ant differences 
+00003400: 7768 656e 2075 7369 6e67 206d 6174 706c  when using matpl
+00003410: 6f74 6c69 6220 696e 2060 6073 7273 6775  otlib in ``srsgu
+00003420: 6960 6020 6172 653a 0d0a 2020 2020 2d20  i`` are:..    - 
+00003430: 596f 7520 6861 7665 2074 6f20 6765 7420  You have to get 
+00003440: 7468 6520 6669 6775 7265 2075 7369 6e67  the figure using
+00003450: 2067 6574 5f66 6967 7572 6528 292c 2072   get_figure(), r
+00003460: 6174 6865 7220 7468 616e 2063 7265 6174  ather than creat
+00003470: 696e 6720 6f6e 6520 6f6e 2079 6f75 7220  ing one on your 
+00003480: 6f77 6e2e 0d0a 2020 2020 2d20 506c 6f74  own...    - Plot
+00003490: 7320 6172 6520 6372 6561 7465 6420 6475  s are created du
+000034a0: 7269 6e67 2060 7365 7475 7028 2960 2c20  ring `setup()`, 
+000034b0: 6265 6361 7573 6520 6974 2069 7320 6120  because it is a 
+000034c0: 736c 6f77 2070 726f 6365 7373 2e20 4475  slow process. Du
+000034d0: 7269 6e67 2060 7465 7374 2829 602c 0d0a  ring `test()`,..
+000034e0: 2020 2020 2020 796f 7520 7369 6d70 6c79        you simply
+000034f0: 2075 7064 6174 6520 6461 7461 2075 7369   update data usi
+00003500: 6e67 2060 7365 745f 6461 7461 2829 6020  ng `set_data()` 
+00003510: 6f72 2073 696d 696c 6172 206d 6574 686f  or similar metho
+00003520: 6473 2066 6f72 2064 6174 6120 7570 6461  ds for data upda
+00003530: 7465 2e0d 0a20 2020 202d 2059 6f75 206d  te...    - You m
+00003540: 7573 7420 7573 6520 6072 6571 7565 7374  ust use `request
+00003550: 5f66 6967 7572 655f 7570 6461 7465 2829  _figure_update()
+00003560: 6020 746f 2072 6564 7261 7720 7468 6520  ` to redraw the 
+00003570: 706c 6f74 2c20 6166 7465 7220 6073 6574  plot, after `set
+00003580: 5f64 6174 6128 2960 2e0d 0a20 2020 2020  _data()`...     
+00003590: 2054 6865 2065 7665 6e74 206c 6f6f 7020   The event loop 
+000035a0: 6861 6e64 6c65 7220 696e 2074 6865 206d  handler in the m
+000035b0: 6169 6e20 6170 706c 6963 6174 696f 6e20  ain application 
+000035c0: 7769 6c6c 2075 7064 6174 6520 7468 6520  will update the 
+000035d0: 706c 6f74 2061 7420 6974 7320 6561 726c  plot at its earl
+000035e0: 6965 7374 0d0a 2020 2020 2020 636f 6e76  iest..      conv
+000035f0: 656e 6965 6e63 652e 0d0a 0d0a 0d0a 2e2e  enience.........
+00003600: 2066 6967 7572 653a 3a20 2e2f 5f73 7461   figure:: ./_sta
+00003610: 7469 632f 7365 636f 6e64 2d74 6173 6b2d  tic/second-task-
+00003620: 7363 7265 656e 2d63 6170 7475 7265 2e70  screen-capture.p
+00003630: 6e67 0d0a 2020 2020 3a61 6c69 676e 3a20  ng..    :align: 
+00003640: 6365 6e74 6572 0d0a 2020 2020 3a66 6967  center..    :fig
+00003650: 636c 6173 733a 2061 6c69 676e 2d63 656e  class: align-cen
+00003660: 7465 720d 0a0d 0a7c 0d0a 0d0a 5363 6f70  ter....|....Scop
+00003670: 6543 6170 7475 7265 2074 6173 6b0d 0a2d  eCapture task..-
+00003680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003690: 2d0d 0a0d 0a54 6865 2053 636f 7065 4361  -....The ScopeCa
+000036a0: 7074 7572 6520 7461 736b 2075 7365 7320  pture task uses 
+000036b0: 7468 6520 6f73 6369 6c6c 6f73 636f 7065  the oscilloscope
+000036c0: 206f 6e6c 792e 2049 7420 6765 7473 2074   only. It gets t
+000036d0: 6865 2072 6571 7565 7374 6564 206e 756d  he requested num
+000036e0: 6265 7220 6f66 2063 6170 7475 7265 7320  ber of captures 
+000036f0: 6672 6f6d 2075 7365 7220 696e 7075 742c  from user input,
+00003700: 0d0a 7468 656e 2072 6570 6561 7473 206f  ..then repeats o
+00003710: 7363 696c 6c6f 7363 6f70 6520 7761 7665  scilloscope wave
+00003720: 666f 726d 2063 6170 7475 7265 2061 6e64  form capture and
+00003730: 2075 7064 6174 6573 2074 6865 2077 6176   updates the wav
+00003740: 6566 6f72 6d20 706c 6f74 2e20 0d0a 4974  eform plot. ..It
+00003750: 2073 746f 7073 206f 6e63 6520 7468 6520   stops once the 
+00003760: 6465 7369 7265 6420 6e75 6d62 6572 206f  desired number o
+00003770: 6620 6361 7074 7572 6573 2068 6176 6520  f captures have 
+00003780: 6265 656e 206f 6274 6169 6e65 642c 206f  been obtained, o
+00003790: 7220 7768 656e 2074 6865 2053 746f 7020  r when the Stop 
+000037a0: 6275 7474 6f6e 2069 7320 7072 6573 7365  button is presse
+000037b0: 642e 0d0a 5761 7665 666f 726d 7320 6172  d...Waveforms ar
+000037c0: 6520 6361 7074 7572 6564 2077 6974 6820  e captured with 
+000037d0: 3730 3030 3030 2070 6f69 6e74 7320 6162  700000 points ab
+000037e0: 6f75 7420 6576 6572 7920 302e 3220 7365  out every 0.2 se
+000037f0: 636f 6e64 7320 6f76 6572 2054 4350 2f49  conds over TCP/I
+00003800: 5020 636f 6d6d 756e 6963 6174 696f 6e2e  P communication.
+00003810: 0d0a 0d0a 0d0a 2e2e 206c 6974 6572 616c  ........ literal
+00003820: 696e 636c 7564 653a 3a20 2e2e 2f73 7273  include:: ../srs
+00003830: 6775 692f 6578 616d 706c 6573 2f6f 7363  gui/examples/osc
+00003840: 696c 6c6f 7363 6f70 6520 6578 616d 706c  illoscope exampl
+00003850: 652f 7461 736b 732f 7363 6f70 655f 6361  e/tasks/scope_ca
+00003860: 7074 7572 652e 7079 0d0a 2020 2020 3a6c  pture.py..    :l
+00003870: 616e 6775 6167 653a 2050 7974 686f 6e0d  anguage: Python.
+00003880: 0a20 2020 203a 6c69 6e65 6e6f 733a 0d0a  .    :linenos:..
+00003890: 0d0a 2e2e 205f 746f 702d 6f66 2d63 6170  .... _top-of-cap
+000038a0: 7475 7265 642d 6666 743a 0d0a 0d0a 4361  tured-fft:....Ca
+000038b0: 7074 7572 6564 4646 5420 7461 736b 0d0a  pturedFFT task..
+000038c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000038d0: 2d0d 0a0d 0a54 6865 2043 6170 7475 7265  -....The Capture
+000038e0: 4646 5420 7461 736b 2069 7320 7468 6520  FFT task is the 
+000038f0: 636c 696d 6178 206f 6620 7468 6520 6578  climax of the ex
+00003900: 616d 706c 6573 2073 6572 6965 7320 283a  amples series (:
+00003910: 7265 663a 6073 6372 6565 6e73 686f 7420  ref:`screenshot 
+00003920: 3c74 6f70 2d6f 662d 7363 7265 656e 2d63  <top-of-screen-c
+00003930: 6170 7475 7265 2d31 3e60 292e 0d0a 4974  apture-1>`)...It
+00003940: 2075 7365 7320 6069 6e70 7574 5f70 6172   uses `input_par
+00003950: 616d 6574 6572 7360 2074 6f20 6368 616e  ameters` to chan
+00003960: 6765 206f 7574 7075 7420 6672 6571 7565  ge output freque
+00003970: 6e63 7920 6f66 2074 6865 2063 6c6f 636b  ncy of the clock
+00003980: 2067 656e 6572 6174 6f72 2069 6e74 6572   generator inter
+00003990: 6163 7469 7665 6c79 2c0d 0a63 6170 7475  actively,..captu
+000039a0: 7265 7320 7761 7665 666f 726d 7320 6672  res waveforms fr
+000039b0: 6f6d 2074 6865 206f 7363 696c 6c6f 7363  om the oscillosc
+000039c0: 6f70 652c 2063 616c 6375 6c61 7465 7320  ope, calculates 
+000039d0: 616e 2046 4654 206f 6620 7468 6520 7761  an FFT of the wa
+000039e0: 7665 666f 726d 7320 7769 7468 206e 756d  veforms with num
+000039f0: 7079 2c0d 0a61 6e64 2067 656e 6572 6174  py,..and generat
+00003a00: 6573 2070 6c6f 7473 2075 7369 6e67 2032  es plots using 2
+00003a10: 206d 6174 706c 6f74 6c69 6220 6669 6775   matplotlib figu
+00003a20: 7265 732e 0d0a 0d0a 4279 2061 6464 696e  res.....By addin
+00003a30: 6720 7468 6520 6e61 6d65 7320 6f66 2066  g the names of f
+00003a40: 6967 7572 6573 2074 6861 7420 796f 7520  igures that you 
+00003a50: 7761 6e74 2074 6f20 7573 6520 696e 2061  want to use in a
+00003a60: 6464 6974 696f 6e61 6c5f 6669 6775 7265  dditional_figure
+00003a70: 5f6e 616d 6573 2c0d 0a60 6073 7273 6775  _names,..``srsgu
+00003a80: 6960 6020 7072 6f76 6964 6573 206d 6f72  i`` provides mor
+00003a90: 6520 6669 6775 7265 7320 746f 2074 6865  e figures to the
+00003aa0: 2074 6173 6b20 6265 666f 7265 2069 7420   task before it 
+00003ab0: 7374 6172 7473 2e0d 0a0d 0a2e 2e20 6c69  starts....... li
+00003ac0: 7465 7261 6c69 6e63 6c75 6465 3a3a 202e  teralinclude:: .
+00003ad0: 2e2f 7372 7367 7569 2f65 7861 6d70 6c65  ./srsgui/example
+00003ae0: 732f 6f73 6369 6c6c 6f73 636f 7065 2065  s/oscilloscope e
+00003af0: 7861 6d70 6c65 2f74 6173 6b73 2f63 6170  xample/tasks/cap
+00003b00: 7475 7265 645f 6666 742e 7079 0d0a 2020  tured_fft.py..  
+00003b10: 2020 3a6c 616e 6775 6167 653a 2050 7974    :language: Pyt
+00003b20: 686f 6e0d 0a20 2020 203a 6c69 6e65 6e6f  hon..    :lineno
+00003b30: 733a 0d0a 0d0a 5369 6d75 6c61 7465 6446  s:....SimulatedF
+00003b40: 4654 2074 6173 6b0d 0a2d 2d2d 2d2d 2d2d  FT task..-------
+00003b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a54  -----------....T
+00003b60: 6865 2053 696d 756c 6174 6564 4646 5420  he SimulatedFFT 
+00003b70: 7461 736b 2073 686f 7773 2068 6f77 2074  task shows how t
+00003b80: 6f20 7375 6263 6c61 7373 2061 6e20 6578  o subclass an ex
+00003b90: 6973 7469 6e67 2074 6173 6b20 636c 6173  isting task clas
+00003ba0: 7320 666f 7220 7265 7573 652e 0d0a 5468  s for reuse...Th
+00003bb0: 6520 6d65 7468 6f64 2067 6574 5f77 6176  e method get_wav
+00003bc0: 6566 6f72 6d28 2920 696e 2074 6865 2043  eform() in the C
+00003bd0: 6170 7475 7265 4646 5420 6578 616d 706c  aptureFFT exampl
+00003be0: 6520 6973 2072 6569 6d70 6c65 6d65 6e74  e is reimplement
+00003bf0: 6564 2074 6f20 6765 6e65 7261 7465 0d0a  ed to generate..
+00003c00: 7369 6d75 6c61 7465 6420 7761 7665 666f  simulated wavefo
+00003c10: 726d 2074 6861 7420 7275 6e73 2077 6974  rm that runs wit
+00003c20: 686f 7574 2061 6e79 2072 6561 6c20 6f73  hout any real os
+00003c30: 6369 6c6c 6f73 636f 7065 2e0d 0a0d 0a4e  cilloscope.....N
+00003c40: 6f74 6520 7468 6174 2074 6865 2073 7175  ote that the squ
+00003c50: 6172 6520 7761 7665 2065 6467 6520 6361  are wave edge ca
+00003c60: 6c63 756c 6174 696f 6e20 6973 2063 7275  lculation is cru
+00003c70: 6465 2c20 6361 7573 696e 6720 6d6f 6475  de, causing modu
+00003c80: 6c61 7469 6f6e 2069 6e20 7075 6c73 6520  lation in pulse 
+00003c90: 7769 6474 680d 0a61 6e64 2073 6964 6520  width..and side 
+00003ca0: 6261 6e64 7320 696e 2074 6865 2046 4654  bands in the FFT
+00003cb0: 2073 7065 6374 7275 6d20 6966 2074 6865   spectrum if the
+00003cc0: 2073 6574 2066 7265 7175 656e 6379 2069   set frequency i
+00003cd0: 7320 6e6f 7420 636f 6d6d 656e 7375 7261  s not commensura
+00003ce0: 7465 2077 6974 680d 0a74 6865 2073 616d  te with..the sam
+00003cf0: 706c 696e 6720 7261 7465 2e20 546f 2067  pling rate. To g
+00003d00: 656e 6572 6174 6520 6120 636c 6561 6e20  enerate a clean 
+00003d10: 7371 7561 7265 2077 6176 652c 2074 6865  square wave, the
+00003d20: 2072 6973 696e 6720 616e 6420 6661 6c6c   rising and fall
+00003d30: 696e 6720 6564 6765 7320 7368 6f75 6c64  ing edges should
+00003d40: 0d0a 6861 7665 2061 7420 6c65 6173 7420  ..have at least 
+00003d50: 7477 6f20 706f 696e 7473 2074 6f20 7265  two points to re
+00003d60: 7072 6573 656e 7420 6578 6163 7420 7068  present exact ph
+00003d70: 6173 652e 2044 6972 6563 7420 7472 616e  ase. Direct tran
+00003d80: 7369 7469 6f6e 2066 726f 6d20 6c6f 7720  sition from low 
+00003d90: 746f 2068 6967 680d 0a77 6974 686f 7574  to high..without
+00003da0: 2061 6e79 2069 6e74 6572 6d65 6469 6174   any intermediat
+00003db0: 6520 706f 696e 7473 2073 7566 6665 7273  e points suffers
+00003dc0: 2066 726f 6d20 7375 6274 6c65 206d 6f64   from subtle mod
+00003dd0: 756c 6174 696f 6e20 696e 2074 696d 6520  ulation in time 
+00003de0: 646f 6d61 696e 2c0d 0a77 6869 6368 206d  domain,..which m
+00003df0: 616e 6966 6573 7473 2061 7320 7369 6465  anifests as side
+00003e00: 2062 616e 6473 2069 6e20 4646 542e 2054   bands in FFT. T
+00003e10: 6869 7320 6973 2061 2063 6f6d 6d6f 6e20  his is a common 
+00003e20: 7072 6f62 6c65 6d20 696e 2064 6967 6974  problem in digit
+00003e30: 616c 2073 6967 6e61 6c0d 0a70 726f 6365  al signal..proce
+00003e40: 7373 696e 672e 2049 7420 6973 206e 6f74  ssing. It is not
+00003e50: 2061 2070 726f 626c 656d 2069 6e20 7468   a problem in th
+00003e60: 6520 7265 616c 2077 6f72 6c64 2c20 6265  e real world, be
+00003e70: 6361 7573 6520 7468 6520 7369 676e 616c  cause the signal
+00003e80: 2069 7320 616e 616c 6f67 2c0d 0a61 6e64   is analog,..and
+00003e90: 2074 6865 2073 616d 706c 696e 6720 7261   the sampling ra
+00003ea0: 7465 2069 7320 6c69 6d69 7465 6420 6279  te is limited by
+00003eb0: 2074 6865 2062 616e 6477 6964 7468 206f   the bandwidth o
+00003ec0: 6620 7468 6520 7369 676e 616c 2e0d 0a0d  f the signal....
+00003ed0: 0a0d 0a2e 2e20 6c69 7465 7261 6c69 6e63  ..... literalinc
+00003ee0: 6c75 6465 3a3a 202e 2e2f 7372 7367 7569  lude:: ../srsgui
+00003ef0: 2f65 7861 6d70 6c65 732f 6f73 6369 6c6c  /examples/oscill
+00003f00: 6f73 636f 7065 2065 7861 6d70 6c65 2f74  oscope example/t
+00003f10: 6173 6b73 2f73 696d 756c 6174 6564 5f66  asks/simulated_f
+00003f20: 6674 2e70 790d 0a20 2020 203a 6c61 6e67  ft.py..    :lang
+00003f30: 7561 6765 3a20 5079 7468 6f6e 0d0a 2020  uage: Python..  
+00003f40: 2020 3a6c 696e 656e 6f73 3a0d 0a0d 0a0d    :linenos:.....
+00003f50: 0a0d 0a2e 2e20 5f50 7956 6973 613a 2068  ..... _PyVisa: h
+00003f60: 7474 7073 3a2f 2f70 7976 6973 612e 7265  ttps://pyvisa.re
+00003f70: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00003f80: 6c61 7465 7374 2f0d 0a2e 2e20 5f73 7273  latest/.... _srs
+00003f90: 696e 7374 2e73 7238 3630 3a20 6874 7470  inst.sr860: http
+00003fa0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00003fb0: 6a65 6374 2f73 7273 696e 7374 2e73 7238  ject/srsinst.sr8
+00003fc0: 3630 2f0d 0a2e 2e20 5f56 5849 3131 3a20  60/.... _VXI11: 
+00003fd0: 6874 7470 733a 2f2f 7777 772e 6c78 6973  https://www.lxis
+00003fe0: 7461 6e64 6172 642e 6f72 672f 4162 6f75  tandard.org/Abou
+00003ff0: 742f 5658 492d 3131 2d61 6e64 2d4c 5849  t/VXI-11-and-LXI
+00004000: 2e61 7370 780d 0a2e 2e20 5f47 5049 423a  .aspx.... _GPIB:
+00004010: 2068 7474 7073 3a2f 2f65 6e2e 7769 6b69   https://en.wiki
+00004020: 7065 6469 612e 6f72 672f 7769 6b69 2f49  pedia.org/wiki/I
+00004030: 4545 452d 3438 380d 0a2e 2e20 5f55 5342  EEE-488.... _USB
+00004040: 2d54 4d43 3a20 6874 7470 733a 2f2f 7777  -TMC: https://ww
+00004050: 772e 7465 7374 616e 646d 6561 7375 7265  w.testandmeasure
+00004060: 6d65 6e74 7469 7073 2e63 6f6d 2f72 656d  menttips.com/rem
+00004070: 6f74 652d 636f 6d6d 756e 6963 6174 696f  ote-communicatio
+00004080: 6e2d 7769 7468 2d75 7362 746d 632d 6661  n-with-usbtmc-fa
+00004090: 712f 0d0a 2e2e 205f 5344 5331 3230 3258  q/.... _SDS1202X
+000040a0: 453a 2068 7474 7073 3a2f 2f73 6967 6c65  E: https://sigle
+000040b0: 6e74 6e61 2e63 6f6d 2f70 726f 6475 6374  ntna.com/product
+000040c0: 2f73 6473 3132 3032 782d 652f 0d0a 2e2e  /sds1202x-e/....
+000040d0: 205f 5352 533a 2068 7474 7073 3a2f 2f74   _SRS: https://t
+000040e0: 6869 6e6b 7372 732e 636f 6d2f 0d0a 2e2e  hinksrs.com/....
+000040f0: 205f 4347 3633 353a 2068 7474 7073 3a2f   _CG635: https:/
+00004100: 2f74 6869 6e6b 7372 732e 636f 6d2f 7072  /thinksrs.com/pr
+00004110: 6f64 7563 7473 2f63 6736 3335 2e68 746d  oducts/cg635.htm
+00004120: 6c0d 0a2e 2e20 5f6c 6f67 6769 6e67 3a20  l.... _logging: 
+00004130: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
+00004140: 686f 6e2e 6f72 672f 332f 686f 7774 6f2f  hon.org/3/howto/
+00004150: 6c6f 6767 696e 672e 6874 6d6c 0d0a 2e2e  logging.html....
+00004160: 205f 6d61 7470 6c6f 746c 6962 3a20 6874   _matplotlib: ht
+00004170: 7470 733a 2f2f 6d61 7470 6c6f 746c 6962  tps://matplotlib
+00004180: 2e6f 7267 2f73 7461 626c 652f 696e 6465  .org/stable/inde
+00004190: 782e 6874 6d6c                           x.html
```

### Comparing `srsgui-0.4.1/docs/index.rst` & `srsgui-0.4.2/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 how many lines of code you need to write to get ``srsgui`` working for control and data acquisition
 from a couple of arbitrary instruments and data visualization for a small task.
 
    - 5 lines of code for CG635 to control its
      output frequency (if not count comment lines);
    - 40 lines to capture waveforms from an oscilloscope (it has a method
      to download a waveform from the oscilloscope);
-   - 100 lines in the fourth example to check if set frequency
+   - 100 lines in the :ref:`CapturedFFT <top-of-captured-fft>` example to check if set frequency
      changed from the input panel, set a new frequency if changed,
      capture a new waveform of 700000 points, calculate FFT of the waveform
      and plot them every 0.2 second;
    - 8 line in the configuration file to put all together.
 
 If you want to implement a well-defined single operation, it will be as simple as this.
 Well, it is mostly thanks to conciseness of Python code and its rich libraries, though.
```

### Comparing `srsgui-0.4.1/docs/installation.rst` & `srsgui-0.4.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/make.bat` & `srsgui-0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/srsgui.inst.communications.rst` & `srsgui-0.4.2/docs/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/srsgui.inst.rst` & `srsgui-0.4.2/docs/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/srsgui.task.rst` & `srsgui-0.4.2/docs/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/srsgui.ui.commandtree.rst` & `srsgui-0.4.2/docs/srsgui.ui.commandtree.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/srsgui.ui.qt.rst` & `srsgui-0.4.2/docs/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/srsgui.ui.rst` & `srsgui-0.4.2/docs/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/docs/troubleshooting.rst` & `srsgui-0.4.2/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/pyproject.toml` & `srsgui-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 classifiers = [
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering"
 ]
 dependencies = [
     "pyserial >= 3",
 ]
 dynamic = ["version"]
```

### Comparing `srsgui-0.4.1/srsgui/__init__.py` & `srsgui-0.4.2/srsgui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.4.1"  # Global version number
+__version__ = "0.4.2"  # Global version number
```

### Comparing `srsgui-0.4.1/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.4.2/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 from srsgui import Instrument
 from srsgui.inst import FloatCommand
 
 # Uncomment the following import to use VisaInterface
```

### Comparing `srsgui-0.4.1/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.4.2/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import numpy as np
 from srsgui import Instrument
 
 # Uncomment the following import to use the customized interface definition
```

### Comparing `srsgui-0.4.1/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.4.2/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files 9% similar despite different names*

```diff
@@ -27,12 +27,12 @@
 
 # A line that starts with 'task: ' adds a task to the project.
 # The first column is the task name that will be used across the application as a dictionary key
 # of the task, displayed in GUI Task menu for selection, and used in task result data file.
 # The Second column is the Python module that contains the task class with relative path from the Task config file.
 # The third column is a task class  that is a Task subclass in the module.
 
-task: *IDN test,                 tasks.first,  FirstTask
-task: Plot example,              tasks.second, SecondTask
-task: Capture Osc. waveform,     tasks.third,  ThirdTask
-task: FFT of captured waveform,  tasks.fourth, FourthTask
-task: FFT of simulated waveform, tasks.fifth,  FifthTask
+task: *IDN test,                 tasks.identify,  Identify
+task: Plot example,              tasks.plot_example, PlotExample
+task: Capture Osc. waveform,     tasks.scope_capture,  ScopeCapture
+task: FFT of captured waveform,  tasks.captured_fft, CapturedFFT
+task: FFT of simulated waveform, tasks.simulated_fft,  SimulatedFFT
```

### Comparing `srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/simulated_fft.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import time
 import math
 import logging
 import numpy as np
 
 from srsgui import Task
 from srsgui import IntegerInput
 
-from tasks.fourth import FourthTask
+from tasks.captured_fft import CapturedFFT
 
 try:
     # Use SciPy signal library if available
     from scipy import signal
 except:
     SCIPY_IMPORTED = False
 else:
     SCIPY_IMPORTED = True
 
-class FifthTask(FourthTask):
+
+class SimulatedFFT(CapturedFFT):
     """
-It subclasses FourthTask (Display FFT waveform) to use simulated \
+It subclasses CapturedFFT class in the capturedfft.py module to use simulated \
 waveforms instead of ones from a real oscilloscope. \
 By isolating and overriding hardware related codes in separate methods, \
 the existing task can be reused.
 
 Note that simply calculated square waveform adds modulated side bands \
 in FFT spectrum caused by time quantization error.
```

### Comparing `srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/identify.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 from srsgui import Task
 
 
-class FirstTask(Task):
+class Identify(Task):
     """
 Query *IDN? to instruments, 'cg' and 'osc' \
 defined in the configuration file.
     """
     
     # No interactive input parameters to set before running 
     input_parameters = {}
```

### Comparing `srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/captured_fft.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import time
 import numpy as np
 from srsgui import Task
 from srsgui import IntegerInput
 
 
-class FourthTask(Task):
+class CapturedFFT(Task):
     """
 Change the frequency of the clock generator output interactively, \
 capture waveforms from the oscilloscope, \
 calculate FFT of the waveforms, \
 plot the waveforms and repeat until the stop button pressed.  
     """
```

### Comparing `srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/plot_example.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import time
 import math
 
 from srsgui import Task
 from srsgui import IntegerInput
 
 
-class SecondTask(Task):
+class PlotExample(Task):
     """
 Example to demonstrate the use of matplotlib plot in a task.
 No hardware connection is required.
 Generates a plot of y = sin(x) vs. x, \
 for x in the range [initial angle, final angle]. 
     """
```

### Comparing `srsgui-0.4.1/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.4.2/srsgui/examples/oscilloscope example/tasks/scope_capture.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##!
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
-##! 
+##!
 
 import time
 from srsgui import Task
 from srsgui import IntegerInput
 
 
-class ThirdTask(Task):
+class ScopeCapture(Task):
     """
 It captures waveforms from an oscilloscope, \
 and plot the waveforms real time.
     """
-    
-    # Use input_parameters to set parameters before running 
+
+    # Use input_parameters to set parameters before running
     Count = 'number of captures'
     input_parameters = {
-        Count: IntegerInput(100) 
+        Count: IntegerInput(100)
     }
-    
+
     def setup(self):
         self.repeat_count = self.get_input_parameter(self.Count)
-        self.logger = self.get_logger(__file__)        
+        self.logger = self.get_logger(__file__)
 
         self.osc = self.get_instrument('osc') # use the inst name in taskconfig file
-        
+
         # Get the Matplotlib figure to plot in
         self.figure = self.get_figure()
 
         # Once you get the figure, the following are about Matplotlib things to plot
         self.ax = self.figure.add_subplot(111)
         self.ax.set_xlim(-1e-5, 1e-5)
         self.ax.set_ylim(-1.5, 1.5)
         self.ax.set_title('Scope waveform Capture')
         self.x_data = [0]
         self.y_data = [0]
         self.line, = self.ax.plot(self.x_data,self.y_data)
-        
+
     def test(self):
         prev_time = time.time()
         for i in range(self.repeat_count):
             if not self.is_running(): # if the Stop button is pressed
                 break
-            
+
             # Add data to the Matplotlib line and update the figure
             t, v = self.osc.get_waveform('C1')  # Get a waveform of the Channel 1 from the oscilloscope
             self.line.set_data(t, v)
             self.request_figure_update()
-            
+
             # Calculate the time for each capture
             current_time = time.time()
             diff = current_time - prev_time
             self.logger.info(f'Capture time for {len(v)} points of waveform {i}: {diff:.3f} s')
             prev_time = current_time
-            
+
     def cleanup(self):
         pass
```

### Comparing `srsgui-0.4.1/srsgui/inst/__init__.py` & `srsgui-0.4.2/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/srsgui/inst/commands.py` & `srsgui-0.4.2/srsgui/inst/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 """
 Module to wrap remote commands used in communication with an instrument
 in `Python descriptors <https://docs.python.org/3/howto/descriptor.html>`_.
```

### Comparing `srsgui-0.4.1/srsgui/inst/communications/interface.py` & `srsgui-0.4.2/srsgui/inst/communications/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import threading
 
 TERM_CHAR = b'\n'   # Termination character for communication
```

### Comparing `srsgui-0.4.1/srsgui/inst/communications/serial_ports.py` & `srsgui-0.4.2/srsgui/inst/communications/serial_ports.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 """
 Get all available serial ports.
 
 Snippet from http://stackoverflow.com/questions/12090503/listing-available-com-ports-with-python
```

### Comparing `srsgui-0.4.1/srsgui/inst/communications/serialinterface.py` & `srsgui-0.4.2/srsgui/inst/communications/serialinterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import time
 
 from srsgui.inst.exceptions import InstCommunicationError
 from .interface import Interface
```

### Comparing `srsgui-0.4.1/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.4.2/srsgui/inst/communications/tcpipinterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import time
 
 import socket
 import select
```

### Comparing `srsgui-0.4.1/srsgui/inst/component.py` & `srsgui-0.4.2/srsgui/inst/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 from .communications import Interface
 from .commands import Command, GetCommand, BoolCommand, IntCommand, \
                       FloatCommand, DictCommand
 from .indexcommands import IndexCommand, BoolIndexCommand, IntIndexCommand, \
```

### Comparing `srsgui-0.4.1/srsgui/inst/exceptions.py` & `srsgui-0.4.2/srsgui/inst/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 class InstException(Exception):
     """
     Package-wide base exception
     """
```

### Comparing `srsgui-0.4.1/srsgui/inst/indexcommands.py` & `srsgui-0.4.2/srsgui/inst/indexcommands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 """
 Module to wrap remote commands with an index argument in dunder methods, __setitem__ and __get_item__.
 
 If an instrument has a remote command using an index, 'PARAM', for  setting and querying a value,
```

### Comparing `srsgui-0.4.1/srsgui/inst/instrument.py` & `srsgui-0.4.2/srsgui/inst/instrument.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import re
 import time
 from .communications import Interface, SerialInterface, TcpipInterface
 from .component import Component
```

### Comparing `srsgui-0.4.1/srsgui/task/callbacks.py` & `srsgui-0.4.2/srsgui/task/callbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import logging
 from matplotlib.figure import Figure
 
 logger = logging.getLogger(__file__)
```

### Comparing `srsgui-0.4.1/srsgui/task/config.py` & `srsgui-0.4.2/srsgui/task/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import sys
 import os
 import logging
 from pathlib import Path
```

### Comparing `srsgui-0.4.1/srsgui/task/inputs.py` & `srsgui-0.4.2/srsgui/task/inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 """
 Interface for input parameters in  :class:`Task <srsgui.task.task.Task>` instance
 and :class:`InputPanel <srsgui.ui.inputpanel.InputPanel>` instance in GUI
 
@@ -169,15 +169,15 @@
         return '.'.join(li)
 
 
 class CommandInput(IntegerInput):
     """
     It provides the interface to :class:`InputPanel <srsgui.ui.inputpanel.InputPanel>`
     to query the value of a command and to change the set value of the command.
-    Currently InputPanel does not update self.value. Do not use get_value().
+    Currently, InputPanel does not update self.value. Do not use get_value().
     Query the command directly in a task.
     """
 
     def __init__(self, cmd_name, cmd_instance=None):
         super().__init__(None)
 
         self.inst_name = ''
```

### Comparing `srsgui-0.4.1/srsgui/task/sessionhandler.py` & `srsgui-0.4.2/srsgui/task/sessionhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import json
 import logging
 from pathlib import Path
 from datetime import datetime
```

### Comparing `srsgui-0.4.1/srsgui/task/task.py` & `srsgui-0.4.2/srsgui/task/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import sys
 import traceback
 import logging
 import time
```

### Comparing `srsgui-0.4.1/srsgui/task/taskresult.py` & `srsgui-0.4.2/srsgui/task/taskresult.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 from datetime import datetime
 
 import logging
 logger = logging.getLogger(__name__)
```

### Comparing `srsgui-0.4.1/srsgui/ui/commandhandler.py` & `srsgui-0.4.2/srsgui/ui/commandhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import time
 import logging
 from .qt.QtCore import QObject, QThread, Signal, Slot
 from .qt.QtWidgets import QMessageBox
```

### Comparing `srsgui-0.4.1/srsgui/ui/commandterminal.py` & `srsgui-0.4.2/srsgui/ui/commandterminal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import logging
 from .qt.QtCore import Signal
 
 from .qt.QtGui import QKeySequence
```

### Comparing `srsgui-0.4.1/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.4.2/srsgui/ui/commandtree/commanddelegate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import logging
 
 from srsgui.ui.qt.QtCore import Qt
 from srsgui.ui.qt.QtWidgets import QStyledItemDelegate, QComboBox
```

### Comparing `srsgui-0.4.1/srsgui/ui/commandtree/commandhandler.py` & `srsgui-0.4.2/srsgui/ui/commandtree/commandhandler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import logging
 
 from srsgui.ui.qt.QtCore import QObject, QThread, QModelIndex, Signal
 from .commanditem import Index
```

### Comparing `srsgui-0.4.1/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.4.2/srsgui/ui/commandtree/commanditem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import time
 import math
 
 from srsgui import Component
```

### Comparing `srsgui-0.4.1/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.4.2/srsgui/ui/commandtree/commandmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import sys
 import logging
 
 from typing import Any, Iterable, List, Dict, Union
```

### Comparing `srsgui-0.4.1/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.4.2/srsgui/ui/commandtree/commandspinbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import sys
 import math
 
 from srsgui.ui.qt.QtCore import Qt, Signal
```

### Comparing `srsgui-0.4.1/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.4.2/srsgui/ui/commandtree/commandtreeview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import sys
 import inspect
 import logging
```

### Comparing `srsgui-0.4.1/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.4.2/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import logging
 import time
 
 from srsgui.ui.qt.QtCore import Qt, QModelIndex
```

### Comparing `srsgui-0.4.1/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.4.2/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/srsgui/ui/connectdlg.py` & `srsgui-0.4.2/srsgui/ui/connectdlg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import logging
 from .qt.QtCore import Qt, QSettings
 from .qt.QtWidgets import QDialog, QDialogButtonBox, \
                           QVBoxLayout, QGridLayout,\
```

### Comparing `srsgui-0.4.1/srsgui/ui/deviceinfohandler.py` & `srsgui-0.4.2/srsgui/ui/deviceinfohandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import logging
 
 from .qt.QtWidgets import QTabWidget, QWidget,  QTextBrowser, QHBoxLayout
```

### Comparing `srsgui-0.4.1/srsgui/ui/dockhandler.py` & `srsgui-0.4.2/srsgui/ui/dockhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import time
 import logging
 
 from .qt.QtCore import Qt
```

### Comparing `srsgui-0.4.1/srsgui/ui/inputpanel.py` & `srsgui-0.4.2/srsgui/ui/inputpanel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import math
 from .qt.QtCore import Qt
 from .qt.QtWidgets import QWidget, QDoubleSpinBox, QSpinBox, QComboBox, \
                           QLineEdit, QLabel, QGridLayout, QPushButton, QScrollArea
```

### Comparing `srsgui-0.4.1/srsgui/ui/qt/QtCore.py` & `srsgui-0.4.2/srsgui/ui/qt/QtCore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 """
 Adapter module for QtCore package for PySide6, PySide2 and PyQt5.
 """
```

### Comparing `srsgui-0.4.1/srsgui/ui/qt/QtGui.py` & `srsgui-0.4.2/srsgui/ui/qt/QtGui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 """
 Adapter module for QtGui package for  PySide6, PySide2 and PyQt5
 """
```

### Comparing `srsgui-0.4.1/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.4.2/srsgui/ui/qt/QtWidgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 """
 Adapter module for QtWidgets package for PySide6, PySide2 and PyQt5
 """
```

### Comparing `srsgui-0.4.1/srsgui/ui/qt/__init__.py` & `srsgui-0.4.2/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/srsgui/ui/qtloghandler.py` & `srsgui-0.4.2/srsgui/ui/qtloghandler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 from logging import getLogger, Handler
 
 from .qt.QtCore import QObject
 from .qt.QtCore import Signal
```

### Comparing `srsgui-0.4.1/srsgui/ui/resource_rc.py` & `srsgui-0.4.2/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/srsgui/ui/signalhandler.py` & `srsgui-0.4.2/srsgui/ui/signalhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 from .qt.QtCore import QObject
 from .qt.QtCore import Signal
 
 from matplotlib.figure import Figure
```

### Comparing `srsgui-0.4.1/srsgui/ui/srslogo.jpg` & `srsgui-0.4.2/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/srsgui/ui/stdout.py` & `srsgui-0.4.2/srsgui/ui/stdout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import sys
 
 from .qt.QtCore import QObject
 from .qt.QtCore import Signal
```

### Comparing `srsgui-0.4.1/srsgui/ui/taskmain.py` & `srsgui-0.4.2/srsgui/ui/taskmain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ##! 
-##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
+##! Copyright(c) 2022, 2023 Stanford Research Systems, All rights reserved
 ##! Subject to the MIT License
 ##! 
 
 import os
 import sys
 
 import logging
```

### Comparing `srsgui-0.4.1/srsgui/ui/taskmain.ui` & `srsgui-0.4.2/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/srsgui/ui/ui_taskmain.py` & `srsgui-0.4.2/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.4.1/srsgui.egg-info/PKG-INFO` & `srsgui-0.4.2/srsgui.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,73 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.4.1
+Version: 0.4.2
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
 Keywords: instrument control,data acquisition,data visualization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: docs
 License-File: LICENSE.txt
 
 # ``Srsgui`` - Organize instrument-controlling Python scripts as a GUI application
 
 `Srsgui` is a simple framework:
 
-   - To define instrument classes for instruments that use remote communication,
-     based on the `Instrument` class and the communication `Interface` class. 
+   - To define instrument classes for instruments that use remote communication, based on the 
+     [`Instrument`](https://thinksrs.github.io/srsgui/srsgui.inst.html#module-srsgui.inst.instrument) 
+     class and the communication 
+     [`Interface`](https://thinksrs.github.io/srsgui/srsgui.inst.communications.html) classes. 
      (By default, serial and TCPIP is available. VXI11, GPIB and USB-TMC are optional).
 
-   - To write Python scripts (tasks) that run in GUI environment with simple APIs
-     provided in ``Task`` class.
+   - To write Python scripts (tasks) that run in graphic user interface (GUI) environment using simple
+     application programming interfaces (APIs) provided in 
+     [``Task``](https://thinksrs.github.io/srsgui/srsgui.task.html) class.
 
    - To organize instrument classes and task scripts presented in a GUI application
-     using a configuration (.taskconfig) file for a project.
+     using a configuration 
+     [(.taskconfig)](https://thinksrs.github.io/srsgui/create-project.html#populating-the-taskconfig-file)
+     file for a project.
 
 ![screenshot](https://thinksrs.github.io/srsgui/_images/example-screen-capture-2.png " ")
 
 ## Installation
 
-To run ``srsgui`` as an application, create a virtual environment, if necessary, 
+To run ``srsgui`` as an GUI application, create a virtual environment, if necessary, 
 and install using ``pip`` with the `[full]` option:  
 
     python -m pip install srsgui[full]
 
 ``Srsgui`` package has the following 3 main dependencies: 
 [pyserial](https://pypi.org/project/pyserial/), 
 [matplotlib](https://pypi.org/project/matplotlib/) and
-[PySide6](https://pypi.org/project/PySide6/). If the installation above fails, 
+[PySide6](https://pypi.org/project/PySide6/) 
+(or [PySide2](https://pypi.org/project/PySide2/)). If the installation above fails, 
 you have to install the failed pacakge manually. Using a virtual environment will
 eliminate possible conflicts between packages in the main Python installation and 
-the packages. Some Linux distributions offer certain Python packages from their repositories only (i.e. not from ``pip``). 
+the packages. Some Linux distributions offer certain Python packages from their 
+repositories only (not from ``pip``). 
 Run a web search for more information on system-specific installation.   
 
-Once pyserial, matplotlib and PySide6 are installed properly, or if you plan to use `srsgui` for instrument drivers only without GUI support, 
+Once pyserial, matplotlib and PySide6 (or PySide2) are installed properly, or if you plan to use 
+`srsgui` for instrument drivers only without GUI support, 
 you can install ``srsgui`` without the `[full]` option:
 
     python -m pip install srsgui
 
 ## Start ``srsgui`` application
     
 If the Python Script directory is in the PATH environment variable,
@@ -69,22 +78,24 @@
 If the script directory is not in PATH, run the srsgui module with Python. 
 
     python -m srsgui
 
 
 ## Run the example project
 
-By default, the `srsgui` application starts with the project that was running when it was last closed.
+By default, the `srsgui` application starts with the project that was running when it was closed the last time.
  
-To open the **oscilloscope example project** included in the `srsgui` package 
+To open the [**oscilloscope example project**](https://thinksrs.github.io/srsgui/example.html)
+included in the `srsgui` package  
 (if `srsgui` does not start with the example project), select File/Open config, 
-go to the `srsgui` package directory, find the examples directory, and select the `oscilloscope example project.taskconfig` file
-in the example project folder. 
+go to the `srsgui` package directory, find the examples directory, and select the 
+`oscilloscope example project.taskconfig` file in the example project folder. 
 
-You can run the **Plot example** and **FFT of simulated waveform** tasks from the Task menu without any instruments connected.
+You can run the **Plot example** and **FFT of simulated waveform** tasks from 
+the Task menu without any instruments connected.
 
 ## Create a project
 
 `Srsgui` is a framework to help you to write your own instrument-controlling 
 Python scripts and run them from a GUI application. Using its APIs, you can write 
 scripts running in GUI with the same amount of code as writing console-based 
 scripts. For programming using the API, refer to the
```

### Comparing `srsgui-0.4.1/srsgui.egg-info/SOURCES.txt` & `srsgui-0.4.2/srsgui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,19 +47,19 @@
 srsgui.egg-info/dependency_links.txt
 srsgui.egg-info/entry_points.txt
 srsgui.egg-info/requires.txt
 srsgui.egg-info/top_level.txt
 srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
 srsgui/examples/oscilloscope example/instruments/cg635.py
 srsgui/examples/oscilloscope example/instruments/sds1202.py
-srsgui/examples/oscilloscope example/tasks/fifth.py
-srsgui/examples/oscilloscope example/tasks/first.py
-srsgui/examples/oscilloscope example/tasks/fourth.py
-srsgui/examples/oscilloscope example/tasks/second.py
-srsgui/examples/oscilloscope example/tasks/third.py
+srsgui/examples/oscilloscope example/tasks/captured_fft.py
+srsgui/examples/oscilloscope example/tasks/identify.py
+srsgui/examples/oscilloscope example/tasks/plot_example.py
+srsgui/examples/oscilloscope example/tasks/scope_capture.py
+srsgui/examples/oscilloscope example/tasks/simulated_fft.py
 srsgui/inst/__init__.py
 srsgui/inst/commands.py
 srsgui/inst/component.py
 srsgui/inst/exceptions.py
 srsgui/inst/indexcommands.py
 srsgui/inst/instrument.py
 srsgui/inst/communications/__init__.py
```

