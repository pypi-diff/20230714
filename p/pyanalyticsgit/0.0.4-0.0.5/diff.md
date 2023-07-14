# Comparing `tmp/pyanalyticsgit-0.0.4.tar.gz` & `tmp/pyanalyticsgit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanalyticsgit-0.0.4.tar", last modified: Thu Jul 13 14:53:02 2023, max compression
+gzip compressed data, was "pyanalyticsgit-0.0.5.tar", last modified: Fri Jul 14 02:11:38 2023, max compression
```

## Comparing `pyanalyticsgit-0.0.4.tar` & `pyanalyticsgit-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-13 14:53:02.541229 pyanalyticsgit-0.0.4/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1064 2023-07-13 14:51:50.000000 pyanalyticsgit-0.0.4/LICENSE
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6726 2023-07-13 14:53:02.541229 pyanalyticsgit-0.0.4/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6391 2023-07-13 14:52:38.000000 pyanalyticsgit-0.0.4/README.md
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-13 14:53:02.537229 pyanalyticsgit-0.0.4/pyanalyticsgit/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       19 2023-07-13 14:51:50.000000 pyanalyticsgit-0.0.4/pyanalyticsgit/__init__.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      314 2023-07-13 14:52:38.000000 pyanalyticsgit-0.0.4/pyanalyticsgit/monitoramento.py
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-13 14:53:02.541229 pyanalyticsgit-0.0.4/pyanalyticsgit/repo/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-07-13 14:51:50.000000 pyanalyticsgit-0.0.4/pyanalyticsgit/repo/__init__.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4922 2023-07-13 14:52:38.000000 pyanalyticsgit-0.0.4/pyanalyticsgit/repo/automatizar.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4886 2023-07-13 14:52:38.000000 pyanalyticsgit-0.0.4/pyanalyticsgit/repo/commit.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3090 2023-07-13 14:52:38.000000 pyanalyticsgit-0.0.4/pyanalyticsgit/repo/connect.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4423 2023-07-13 14:52:38.000000 pyanalyticsgit-0.0.4/pyanalyticsgit/repo/issue.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3263 2023-07-13 14:52:38.000000 pyanalyticsgit-0.0.4/pyanalyticsgit/repo/milestone.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3642 2023-07-13 14:52:38.000000 pyanalyticsgit-0.0.4/pyanalyticsgit/repo/relatorio.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1361 2023-07-13 14:52:38.000000 pyanalyticsgit-0.0.4/pyanalyticsgit/test_linux.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1363 2023-07-13 14:52:38.000000 pyanalyticsgit-0.0.4/pyanalyticsgit/test_macos.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1063 2023-07-13 14:52:38.000000 pyanalyticsgit-0.0.4/pyanalyticsgit/test_windows.py
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-13 14:53:02.541229 pyanalyticsgit-0.0.4/pyanalyticsgit.egg-info/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6726 2023-07-13 14:53:02.000000 pyanalyticsgit-0.0.4/pyanalyticsgit.egg-info/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      586 2023-07-13 14:53:02.000000 pyanalyticsgit-0.0.4/pyanalyticsgit.egg-info/SOURCES.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-13 14:53:02.000000 pyanalyticsgit-0.0.4/pyanalyticsgit.egg-info/dependency_links.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       92 2023-07-13 14:53:02.000000 pyanalyticsgit-0.0.4/pyanalyticsgit.egg-info/requires.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       35 2023-07-13 14:53:02.000000 pyanalyticsgit-0.0.4/pyanalyticsgit.egg-info/top_level.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       38 2023-07-13 14:53:02.541229 pyanalyticsgit-0.0.4/setup.cfg
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      748 2023-07-13 14:52:47.000000 pyanalyticsgit-0.0.4/setup.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 02:11:38.462043 pyanalyticsgit-0.0.5/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1064 2023-07-13 15:04:24.000000 pyanalyticsgit-0.0.5/LICENSE
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6941 2023-07-14 02:11:38.462043 pyanalyticsgit-0.0.5/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6391 2023-07-13 15:15:11.000000 pyanalyticsgit-0.0.5/README.md
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 02:11:38.454043 pyanalyticsgit-0.0.5/pyanalyticsgit/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       19 2023-07-13 15:04:24.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/__init__.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      314 2023-07-14 02:10:50.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/monitoramento.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 02:11:38.458043 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-07-13 15:04:24.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/__init__.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4922 2023-07-13 15:15:11.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/automatizar.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4886 2023-07-14 01:56:02.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/commit.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4414 2023-07-14 00:22:32.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/connect.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4423 2023-07-14 01:56:04.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/issue.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3263 2023-07-14 01:56:06.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/milestone.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3615 2023-07-14 02:05:10.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/repo/relatorio.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1361 2023-07-13 15:15:11.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/test_linux.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1363 2023-07-13 15:15:11.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/test_macos.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1063 2023-07-13 15:15:11.000000 pyanalyticsgit-0.0.5/pyanalyticsgit/test_windows.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-14 02:11:38.454043 pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     6941 2023-07-14 02:11:38.000000 pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      586 2023-07-14 02:11:38.000000 pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-14 02:11:38.000000 pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       92 2023-07-14 02:11:38.000000 pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/requires.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       35 2023-07-14 02:11:38.000000 pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/top_level.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       38 2023-07-14 02:11:38.462043 pyanalyticsgit-0.0.5/setup.cfg
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      963 2023-07-14 02:08:49.000000 pyanalyticsgit-0.0.5/setup.py
```

### Comparing `pyanalyticsgit-0.0.4/LICENSE` & `pyanalyticsgit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.4/PKG-INFO` & `pyanalyticsgit-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyanalyticsgit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Biblioteca PyAnalyticsGit para gerar relatórios Git.
 Home-page: UNKNOWN
-Author: Jefferson Sena
-Author-email: jeffersonsena12144@gmail.com
+Author: Gabriel Barbosa, Jefferson Sena, Mateus Levy, Pedro Henrique, Rodrigo Fonseca, Tiago Albuquerque
+Author-email: gabrielb.alencarr@gmail.com, jeffersonsena12144@gmail.com, mateuslevy06@gmail.com, pedrolulhenrique@gmail.com, Rodrigofonseca399@gmail.com, tiago28973@gmail.com 
 License: MIT License
 Keywords: pyAnalyticsGit
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
```

### Comparing `pyanalyticsgit-0.0.4/README.md` & `pyanalyticsgit-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.4/pyanalyticsgit/repo/automatizar.py` & `pyanalyticsgit-0.0.5/pyanalyticsgit/repo/automatizar.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.4/pyanalyticsgit/repo/commit.py` & `pyanalyticsgit-0.0.5/pyanalyticsgit/repo/commit.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.4/pyanalyticsgit/repo/issue.py` & `pyanalyticsgit-0.0.5/pyanalyticsgit/repo/issue.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.4/pyanalyticsgit/repo/milestone.py` & `pyanalyticsgit-0.0.5/pyanalyticsgit/repo/milestone.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.4/pyanalyticsgit/repo/relatorio.py` & `pyanalyticsgit-0.0.5/pyanalyticsgit/repo/relatorio.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 caminho_pasta = os.path.join(diretorio_raiz, nome_pasta)
 
 class Relatorio:
     """Classe para gerar relatório de commits, issues e milestones"""
     def __init__(self):
         """Construtor da classe Relatorio"""
         self.nome_arquivo = "relatorio_padrao.md"
-        self.titulo = "# PyAnalyticsGit - Relatório automatizado"
+        self.titulo = "# Relatório dos dados do Repositório"
         if not os.path.exists(caminho_pasta):
             os.makedirs(caminho_pasta)
         self.caminho_arquivo = os.path.join(caminho_pasta, self.nome_arquivo)
         with open(self.caminho_arquivo, 'w+') as arq:
             arq.seek(0)
             if self.titulo not in arq.read():
                 arq.write(f'{self.titulo}\n\n')
@@ -82,10 +82,8 @@
             arq.write("# Milestones\n\n")
             arq.write("## Gráfico de Milestones\n\n")
             arq.write("<div align='center'>\n\n")
             arq.write("![Gráfico de Milestones](grafico_milestone.png)\n\n")
             arq.write("</div>\n\n")
 
         grafico_tabela_milestone.criar_tabela_milestone(self.caminho_arquivo)
-    
-                    
-
+
```

### Comparing `pyanalyticsgit-0.0.4/pyanalyticsgit/test_linux.py` & `pyanalyticsgit-0.0.5/pyanalyticsgit/test_linux.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.4/pyanalyticsgit/test_macos.py` & `pyanalyticsgit-0.0.5/pyanalyticsgit/test_macos.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.4/pyanalyticsgit/test_windows.py` & `pyanalyticsgit-0.0.5/pyanalyticsgit/test_windows.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.0.4/pyanalyticsgit.egg-info/PKG-INFO` & `pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pyanalyticsgit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Biblioteca PyAnalyticsGit para gerar relatórios Git.
 Home-page: UNKNOWN
-Author: Jefferson Sena
-Author-email: jeffersonsena12144@gmail.com
+Author: Gabriel Barbosa, Jefferson Sena, Mateus Levy, Pedro Henrique, Rodrigo Fonseca, Tiago Albuquerque
+Author-email: gabrielb.alencarr@gmail.com, jeffersonsena12144@gmail.com, mateuslevy06@gmail.com, pedrolulhenrique@gmail.com, Rodrigofonseca399@gmail.com, tiago28973@gmail.com 
 License: MIT License
 Keywords: pyAnalyticsGit
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
```

### Comparing `pyanalyticsgit-0.0.4/pyanalyticsgit.egg-info/SOURCES.txt` & `pyanalyticsgit-0.0.5/pyanalyticsgit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

