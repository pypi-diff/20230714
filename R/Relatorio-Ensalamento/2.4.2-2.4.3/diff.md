# Comparing `tmp/Relatorio_Ensalamento-2.4.2.tar.gz` & `tmp/Relatorio_Ensalamento-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Relatorio_Ensalamento-2.4.2.tar", last modified: Fri Jul 14 19:51:51 2023, max compression
+gzip compressed data, was "Relatorio_Ensalamento-2.4.3.tar", last modified: Fri Jul 14 20:10:10 2023, max compression
```

## Comparing `Relatorio_Ensalamento-2.4.2.tar` & `Relatorio_Ensalamento-2.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 19:51:51.004404 Relatorio_Ensalamento-2.4.2/
--rw-rw-rw-   0        0        0      549 2023-07-14 19:51:51.006442 Relatorio_Ensalamento-2.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-01-27 12:58:30.000000 Relatorio_Ensalamento-2.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 19:51:50.935426 Relatorio_Ensalamento-2.4.2/Relatorio_Ensalamento/
--rw-rw-rw-   0        0        0    49946 2023-07-14 19:51:41.000000 Relatorio_Ensalamento-2.4.2/Relatorio_Ensalamento/Relatorio_Ensalamento.py
--rw-rw-rw-   0        0        0       38 2023-01-26 12:04:50.000000 Relatorio_Ensalamento-2.4.2/Relatorio_Ensalamento/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 19:51:50.964157 Relatorio_Ensalamento-2.4.2/Relatorio_Ensalamento.egg-info/
--rw-rw-rw-   0        0        0      549 2023-07-14 19:51:50.000000 Relatorio_Ensalamento-2.4.2/Relatorio_Ensalamento.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-14 19:51:50.000000 Relatorio_Ensalamento-2.4.2/Relatorio_Ensalamento.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 19:51:50.000000 Relatorio_Ensalamento-2.4.2/Relatorio_Ensalamento.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-14 19:51:50.000000 Relatorio_Ensalamento-2.4.2/Relatorio_Ensalamento.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 19:51:50.981313 Relatorio_Ensalamento-2.4.2/Sugestao/
--rw-rw-rw-   0        0        0    64234 2023-07-14 18:36:16.000000 Relatorio_Ensalamento-2.4.2/Sugestao/Sugestao.py
--rw-rw-rw-   0        0        0       25 2023-01-26 11:56:59.000000 Relatorio_Ensalamento-2.4.2/Sugestao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 19:51:50.997428 Relatorio_Ensalamento-2.4.2/Unificar_XML/
--rw-rw-rw-   0        0        0    17469 2023-02-02 16:23:54.000000 Relatorio_Ensalamento-2.4.2/Unificar_XML/Unificar_XML.py
--rw-rw-rw-   0        0        0       27 2023-02-02 13:41:12.000000 Relatorio_Ensalamento-2.4.2/Unificar_XML/__init__.py
--rw-rw-rw-   0        0        0      114 2023-07-14 19:51:51.037345 Relatorio_Ensalamento-2.4.2/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-07-14 19:51:41.000000 Relatorio_Ensalamento-2.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:10:10.332915 Relatorio_Ensalamento-2.4.3/
+-rw-rw-rw-   0        0        0      549 2023-07-14 20:10:10.332915 Relatorio_Ensalamento-2.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-01-27 12:58:30.000000 Relatorio_Ensalamento-2.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 20:10:10.288670 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento/
+-rw-rw-rw-   0        0        0    49946 2023-07-14 19:51:41.000000 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento/Relatorio_Ensalamento.py
+-rw-rw-rw-   0        0        0       38 2023-01-26 12:04:50.000000 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:10:10.314816 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento.egg-info/
+-rw-rw-rw-   0        0        0      549 2023-07-14 20:10:10.000000 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-14 20:10:10.000000 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 20:10:10.000000 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-14 20:10:10.000000 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 20:10:10.320817 Relatorio_Ensalamento-2.4.3/Sugestao/
+-rw-rw-rw-   0        0        0    64234 2023-07-14 18:36:16.000000 Relatorio_Ensalamento-2.4.3/Sugestao/Sugestao.py
+-rw-rw-rw-   0        0        0       25 2023-01-26 11:56:59.000000 Relatorio_Ensalamento-2.4.3/Sugestao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:10:10.330815 Relatorio_Ensalamento-2.4.3/Unificar_XML/
+-rw-rw-rw-   0        0        0    18277 2023-07-14 20:10:07.000000 Relatorio_Ensalamento-2.4.3/Unificar_XML/Unificar_XML.py
+-rw-rw-rw-   0        0        0       27 2023-02-02 13:41:12.000000 Relatorio_Ensalamento-2.4.3/Unificar_XML/__init__.py
+-rw-rw-rw-   0        0        0      114 2023-07-14 20:10:10.337815 Relatorio_Ensalamento-2.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-07-14 20:10:07.000000 Relatorio_Ensalamento-2.4.3/setup.py
```

### Comparing `Relatorio_Ensalamento-2.4.2/PKG-INFO` & `Relatorio_Ensalamento-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Relatorio_Ensalamento
-Version: 2.4.2
+Version: 2.4.3
 Summary: Conversor utilizado para a geração do relatorio ensalamento
 Home-page: UNKNOWN
 Author: Matheus Henrique Rosa
 Author-email: m.rosa1@pucpr.br
 License: MIT
 Keywords: conversor relatorio ensalamento
 Platform: UNKNOWN
```

### Comparing `Relatorio_Ensalamento-2.4.2/Relatorio_Ensalamento/Relatorio_Ensalamento.py` & `Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento/Relatorio_Ensalamento.py`

 * *Files identical despite different names*

### Comparing `Relatorio_Ensalamento-2.4.2/Relatorio_Ensalamento.egg-info/PKG-INFO` & `Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Relatorio-Ensalamento
-Version: 2.4.2
+Version: 2.4.3
 Summary: Conversor utilizado para a geração do relatorio ensalamento
 Home-page: UNKNOWN
 Author: Matheus Henrique Rosa
 Author-email: m.rosa1@pucpr.br
 License: MIT
 Keywords: conversor relatorio ensalamento
 Platform: UNKNOWN
```

### Comparing `Relatorio_Ensalamento-2.4.2/Sugestao/Sugestao.py` & `Relatorio_Ensalamento-2.4.3/Sugestao/Sugestao.py`

 * *Files identical despite different names*

### Comparing `Relatorio_Ensalamento-2.4.2/Unificar_XML/Unificar_XML.py` & `Relatorio_Ensalamento-2.4.3/Unificar_XML/Unificar_XML.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,29 @@
                            endtime="21:30")
     ElementTree.SubElement(periods, "period", name="21:30", short="21:30", period="19", starttime="21:30",
                            endtime="22:15")
     ElementTree.SubElement(periods, "period", name="22:15", short="22:15", period="20", starttime="22:15",
                            endtime="23:00")
 
     # tag daysdef
-    ElementTree.SubElement(root_unificado, "daysdefs", columns="id,days,name,short")
+    daysdefs = ElementTree.SubElement(root_unificado, "daysdefs", columns="id,days,name,short")
+    ElementTree.SubElement(daysdefs, "daysdef", id="6B3F12A34D97076A", name="Qualquer dia", short="X",
+                           days="1000000,0100000,0010000,0001000,0000100,0000010,0000001")
+    ElementTree.SubElement(daysdefs, "daysdef", id="805BDEBDA010C1F2", name="Cada dia", short="E", days="1111111")
+    ElementTree.SubElement(daysdefs, "daysdef", id="A8F237B2F9E6B675", name="Segunda-feira ", short="Seg",
+                           days="1000000")
+    ElementTree.SubElement(daysdefs, "daysdef", id="CAB97D0425BEC0DA", name="Terça-feira", short="Ter", days="0100000")
+    ElementTree.SubElement(daysdefs, "daysdef", id="60850D9314471122", name="Quarta-feira ", short="Qua",
+                           days="0010000")
+    ElementTree.SubElement(daysdefs, "daysdef", id="DDF4362F91A753AB", name="Quinta-feira ", short="Qui",
+                           days="0001000")
+    ElementTree.SubElement(daysdefs, "daysdef", id="E87DBCE4E7616290", name="Sexta-feira ", short="Sex", days="0000100")
+    ElementTree.SubElement(daysdefs, "daysdef", id="23651B657C8E30B9", name="Sábado ", short="Sáb", days="0000010")
+    ElementTree.SubElement(daysdefs, "daysdef", id="0E5CEC8F57D233C2", name="Horário Flutuante", short="Flutuante",
+                           days="0000001")
 
     # tag weeksdef
     weeksdefs = ElementTree.SubElement(root_unificado, "weekdefs", options="canadd,export:silent",
                                        columns="id,weeks,name,short")
     ElementTree.SubElement(weeksdefs, "weekdef", id="4D751412E50EC8F8", name="Todas as semanas", short="Todas",
                            weeks="1")
 
@@ -115,25 +129,15 @@
     # tag cards
     ElementTree.SubElement(root_unificado, "cards", options="canadd,export:silent",
                            columns="lessonid,period,days,weeks,terms,classroomids")
 
     return root_unificado
 
 
-def unifica_xml(root_unificado, root, contagem):
-    if contagem == 0:
-        for day in root.iter("daysdef"):
-            for child in root_unificado:
-                tag = child.tag
-                if tag == "daysdefs":
-                    ElementTree.SubElement(child, "daysdef", id=day.get("id"), name=str(day.get("name")),
-                                           short=day.get("short")
-                                           , days=day.get("days"))
-
-    contagem += 1
+def unifica_xml(root_unificado, root):
     # tag subjects
     # subjects = ElementTree.Element(root_unificado, "subject")
     for sub in root.iter("subject"):
         for child in root_unificado:
             tag = child.tag
             if tag == "subjects":
                 ElementTree.SubElement(child, "subject", id=sub.get("id"), name=str(sub.get("name")),
@@ -212,15 +216,15 @@
             if tag == "cards":
                 ElementTree.SubElement(child, "card", lessonid=car.get("lessonid"),
                                        classroomids=car.get("classroomids"),
                                        period=car.get("period"),
                                        terms=car.get("terms"),
                                        days=car.get("days"))
 
-    return root_unificado, contagem
+    return root_unificado
 
 
 def corrige_caracteres_especiais(file_name):
     # Substitui o símbolo que causa erro
     # file_data = file_name.replace("&quot;", "").replace('& amp;','').replace(" &amp; ", "").replace(" ", "")
     file_data = file_name
     return file_data
@@ -292,41 +296,41 @@
     for group in root.find("groups").findall("group"):
         if group.get("id") not in active_groups:
             root.find("groups").remove(group)
 
     return root
 
 
-def main(caminho_pasta):
+def main(caminho_pasta, caminho_aux):
     utc_now = pytz.utc.localize(datetime.datetime.utcnow())
     dt_now = utc_now.astimezone(pytz.timezone("America/Sao_Paulo"))
     pasta_raiz = caminho_pasta
 
     root_unificado = cria_unificado()
     tree = ""
-    contagem = 0
     # Para cada diretório dentro do diretório raiz
     for dirpath, dirnames, filenames in os.walk(pasta_raiz):
         # dirpath =  caminho
 
         for file in filenames:
             file = file.upper()
-            if not file.__contains__(".XML"):
+            if not file.__contains__("XML"):
                 continue
 
             # criando o xml que vai passar os dados
             file_name_xml = dirpath + "/" + file
             tree_xml = ElementTree.parse(file_name_xml)
             root = tree_xml.getroot()
             # unificando
-            tree, contagem = unifica_xml(root_unificado, root, contagem)
+            tree = unifica_xml(root_unificado, root)
 
-        # tree_sem_flutuantes = retira_flutuantes(tree)
+        tree_sem_flutuantes = retira_flutuantes(tree)
 
-        # xml_string_sem_flutuantes = minidom.parseString(ElementTree.tostring(tree_sem_flutuantes, encoding="windows-1252")).toprettyxml(indent="   ")
+        xml_string_sem_flutuantes = minidom.parseString(
+            ElementTree.tostring(tree_sem_flutuantes, encoding="windows-1252")).toprettyxml(indent="   ")
         xml_string = minidom.parseString(ElementTree.tostring(tree, encoding="windows-1252")).toprettyxml(indent="   ")
 
         # forçar a mudança do enconding
         # contar quantas vezes o ? se repete para que na segunda vez sobreescreva o enconding correto
         posicao = 0
         contagem = 0
         lista = list(xml_string)
@@ -340,26 +344,26 @@
             posicao += 1
         xml_string = "".join(lista)
 
         # forçar a mudança do enconding
         # contar quantas vezes o ? se repete para que na segunda vez sobreescreva o enconding correto
         posicao = 0
         contagem = 0
-        # lista = list(xml_string_sem_flutuantes)
-        '''for i in xml_string_sem_flutuantes:
+        lista = list(xml_string_sem_flutuantes)
+        for i in xml_string_sem_flutuantes:
             if i == "?":
                 contagem += 1
             if contagem == 2:
                 contagem = 3
                 lista[posicao] = "encoding='windows-1252'?"
 
             posicao += 1
-        xml_string_sem_flutuantes = "".join(lista)'''
+        xml_string_sem_flutuantes = "".join(lista)
 
-        name = f"./Arquivos_Auxiliares/XML/XML_unificado_{str(dt_now.strftime('%y-%m-%d %H-%M'))}.xml"
+        name = f"{caminho_aux}/XML/XML_unificado_{str(dt_now.strftime('%y-%m-%d %H-%M'))}.xml"
         with open(name, "w", encoding="windows-1252") as f:
             xml_string = corrige_caracteres_especiais(xml_string)
             f.write(xml_string)
 
         return name
```

