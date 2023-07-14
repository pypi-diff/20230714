# Comparing `tmp/Relatorio_Ensalamento-2.4.5.tar.gz` & `tmp/Relatorio_Ensalamento-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Relatorio_Ensalamento-2.4.5.tar", last modified: Fri Jul 14 21:19:25 2023, max compression
+gzip compressed data, was "Relatorio_Ensalamento-2.4.6.tar", last modified: Fri Jul 14 21:20:01 2023, max compression
```

## Comparing `Relatorio_Ensalamento-2.4.5.tar` & `Relatorio_Ensalamento-2.4.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 21:19:25.713897 Relatorio_Ensalamento-2.4.5/
--rw-rw-rw-   0        0        0      549 2023-07-14 21:19:25.714928 Relatorio_Ensalamento-2.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-01-27 12:58:30.000000 Relatorio_Ensalamento-2.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 21:19:25.666268 Relatorio_Ensalamento-2.4.5/Relatorio_Ensalamento/
--rw-rw-rw-   0        0        0    50179 2023-07-14 20:55:33.000000 Relatorio_Ensalamento-2.4.5/Relatorio_Ensalamento/Relatorio_Ensalamento.py
--rw-rw-rw-   0        0        0       38 2023-01-26 12:04:50.000000 Relatorio_Ensalamento-2.4.5/Relatorio_Ensalamento/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 21:19:25.693280 Relatorio_Ensalamento-2.4.5/Relatorio_Ensalamento.egg-info/
--rw-rw-rw-   0        0        0      549 2023-07-14 21:19:25.000000 Relatorio_Ensalamento-2.4.5/Relatorio_Ensalamento.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-14 21:19:25.000000 Relatorio_Ensalamento-2.4.5/Relatorio_Ensalamento.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 21:19:25.000000 Relatorio_Ensalamento-2.4.5/Relatorio_Ensalamento.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-14 21:19:25.000000 Relatorio_Ensalamento-2.4.5/Relatorio_Ensalamento.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 21:19:25.703286 Relatorio_Ensalamento-2.4.5/Sugestao/
--rw-rw-rw-   0        0        0    59471 2023-07-14 21:19:02.000000 Relatorio_Ensalamento-2.4.5/Sugestao/Sugestao.py
--rw-rw-rw-   0        0        0       25 2023-01-26 11:56:59.000000 Relatorio_Ensalamento-2.4.5/Sugestao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 21:19:25.710839 Relatorio_Ensalamento-2.4.5/Unificar_XML/
--rw-rw-rw-   0        0        0    18277 2023-07-14 20:10:07.000000 Relatorio_Ensalamento-2.4.5/Unificar_XML/Unificar_XML.py
--rw-rw-rw-   0        0        0       27 2023-02-02 13:41:12.000000 Relatorio_Ensalamento-2.4.5/Unificar_XML/__init__.py
--rw-rw-rw-   0        0        0      114 2023-07-14 21:19:25.719837 Relatorio_Ensalamento-2.4.5/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-07-14 21:19:15.000000 Relatorio_Ensalamento-2.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 21:20:01.443735 Relatorio_Ensalamento-2.4.6/
+-rw-rw-rw-   0        0        0      549 2023-07-14 21:20:01.443735 Relatorio_Ensalamento-2.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-01-27 12:58:30.000000 Relatorio_Ensalamento-2.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 21:20:01.404283 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento/
+-rw-rw-rw-   0        0        0    50179 2023-07-14 20:55:33.000000 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento/Relatorio_Ensalamento.py
+-rw-rw-rw-   0        0        0       38 2023-01-26 12:04:50.000000 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 21:20:01.426481 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento.egg-info/
+-rw-rw-rw-   0        0        0      549 2023-07-14 21:20:01.000000 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-14 21:20:01.000000 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 21:20:01.000000 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-14 21:20:01.000000 Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 21:20:01.434477 Relatorio_Ensalamento-2.4.6/Sugestao/
+-rw-rw-rw-   0        0        0    59471 2023-07-14 21:19:02.000000 Relatorio_Ensalamento-2.4.6/Sugestao/Sugestao.py
+-rw-rw-rw-   0        0        0       25 2023-01-26 11:56:59.000000 Relatorio_Ensalamento-2.4.6/Sugestao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 21:20:01.441689 Relatorio_Ensalamento-2.4.6/Unificar_XML/
+-rw-rw-rw-   0        0        0    18277 2023-07-14 20:10:07.000000 Relatorio_Ensalamento-2.4.6/Unificar_XML/Unificar_XML.py
+-rw-rw-rw-   0        0        0       27 2023-02-02 13:41:12.000000 Relatorio_Ensalamento-2.4.6/Unificar_XML/__init__.py
+-rw-rw-rw-   0        0        0      114 2023-07-14 21:20:01.448648 Relatorio_Ensalamento-2.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-07-14 21:19:58.000000 Relatorio_Ensalamento-2.4.6/setup.py
```

### Comparing `Relatorio_Ensalamento-2.4.5/PKG-INFO` & `Relatorio_Ensalamento-2.4.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Relatorio_Ensalamento
-Version: 2.4.5
+Version: 2.4.6
 Summary: Conversor utilizado para a geração do relatorio ensalamento
 Home-page: UNKNOWN
 Author: Matheus Henrique Rosa
 Author-email: m.rosa1@pucpr.br
 License: MIT
 Keywords: conversor relatorio ensalamento
 Platform: UNKNOWN
```

### Comparing `Relatorio_Ensalamento-2.4.5/Relatorio_Ensalamento/Relatorio_Ensalamento.py` & `Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento/Relatorio_Ensalamento.py`

 * *Files identical despite different names*

### Comparing `Relatorio_Ensalamento-2.4.5/Relatorio_Ensalamento.egg-info/PKG-INFO` & `Relatorio_Ensalamento-2.4.6/Relatorio_Ensalamento.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Relatorio-Ensalamento
-Version: 2.4.5
+Version: 2.4.6
 Summary: Conversor utilizado para a geração do relatorio ensalamento
 Home-page: UNKNOWN
 Author: Matheus Henrique Rosa
 Author-email: m.rosa1@pucpr.br
 License: MIT
 Keywords: conversor relatorio ensalamento
 Platform: UNKNOWN
```

### Comparing `Relatorio_Ensalamento-2.4.5/Sugestao/Sugestao.py` & `Relatorio_Ensalamento-2.4.6/Sugestao/Sugestao.py`

 * *Files identical despite different names*

### Comparing `Relatorio_Ensalamento-2.4.5/Unificar_XML/Unificar_XML.py` & `Relatorio_Ensalamento-2.4.6/Unificar_XML/Unificar_XML.py`

 * *Files identical despite different names*

