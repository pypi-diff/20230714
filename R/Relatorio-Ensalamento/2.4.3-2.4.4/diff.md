# Comparing `tmp/Relatorio_Ensalamento-2.4.3.tar.gz` & `tmp/Relatorio_Ensalamento-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Relatorio_Ensalamento-2.4.3.tar", last modified: Fri Jul 14 20:10:10 2023, max compression
+gzip compressed data, was "Relatorio_Ensalamento-2.4.4.tar", last modified: Fri Jul 14 20:55:39 2023, max compression
```

## Comparing `Relatorio_Ensalamento-2.4.3.tar` & `Relatorio_Ensalamento-2.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 20:10:10.332915 Relatorio_Ensalamento-2.4.3/
--rw-rw-rw-   0        0        0      549 2023-07-14 20:10:10.332915 Relatorio_Ensalamento-2.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-01-27 12:58:30.000000 Relatorio_Ensalamento-2.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 20:10:10.288670 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento/
--rw-rw-rw-   0        0        0    49946 2023-07-14 19:51:41.000000 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento/Relatorio_Ensalamento.py
--rw-rw-rw-   0        0        0       38 2023-01-26 12:04:50.000000 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:10:10.314816 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento.egg-info/
--rw-rw-rw-   0        0        0      549 2023-07-14 20:10:10.000000 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-14 20:10:10.000000 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 20:10:10.000000 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-14 20:10:10.000000 Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 20:10:10.320817 Relatorio_Ensalamento-2.4.3/Sugestao/
--rw-rw-rw-   0        0        0    64234 2023-07-14 18:36:16.000000 Relatorio_Ensalamento-2.4.3/Sugestao/Sugestao.py
--rw-rw-rw-   0        0        0       25 2023-01-26 11:56:59.000000 Relatorio_Ensalamento-2.4.3/Sugestao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 20:10:10.330815 Relatorio_Ensalamento-2.4.3/Unificar_XML/
--rw-rw-rw-   0        0        0    18277 2023-07-14 20:10:07.000000 Relatorio_Ensalamento-2.4.3/Unificar_XML/Unificar_XML.py
--rw-rw-rw-   0        0        0       27 2023-02-02 13:41:12.000000 Relatorio_Ensalamento-2.4.3/Unificar_XML/__init__.py
--rw-rw-rw-   0        0        0      114 2023-07-14 20:10:10.337815 Relatorio_Ensalamento-2.4.3/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-07-14 20:10:07.000000 Relatorio_Ensalamento-2.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:55:39.177354 Relatorio_Ensalamento-2.4.4/
+-rw-rw-rw-   0        0        0      549 2023-07-14 20:55:39.178407 Relatorio_Ensalamento-2.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-01-27 12:58:30.000000 Relatorio_Ensalamento-2.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 20:55:39.134882 Relatorio_Ensalamento-2.4.4/Relatorio_Ensalamento/
+-rw-rw-rw-   0        0        0    50179 2023-07-14 20:55:33.000000 Relatorio_Ensalamento-2.4.4/Relatorio_Ensalamento/Relatorio_Ensalamento.py
+-rw-rw-rw-   0        0        0       38 2023-01-26 12:04:50.000000 Relatorio_Ensalamento-2.4.4/Relatorio_Ensalamento/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:55:39.159079 Relatorio_Ensalamento-2.4.4/Relatorio_Ensalamento.egg-info/
+-rw-rw-rw-   0        0        0      549 2023-07-14 20:55:39.000000 Relatorio_Ensalamento-2.4.4/Relatorio_Ensalamento.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-14 20:55:39.000000 Relatorio_Ensalamento-2.4.4/Relatorio_Ensalamento.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 20:55:39.000000 Relatorio_Ensalamento-2.4.4/Relatorio_Ensalamento.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-14 20:55:39.000000 Relatorio_Ensalamento-2.4.4/Relatorio_Ensalamento.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 20:55:39.170300 Relatorio_Ensalamento-2.4.4/Sugestao/
+-rw-rw-rw-   0        0        0    59471 2023-07-14 20:54:43.000000 Relatorio_Ensalamento-2.4.4/Sugestao/Sugestao.py
+-rw-rw-rw-   0        0        0       25 2023-01-26 11:56:59.000000 Relatorio_Ensalamento-2.4.4/Sugestao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 20:55:39.176304 Relatorio_Ensalamento-2.4.4/Unificar_XML/
+-rw-rw-rw-   0        0        0    18277 2023-07-14 20:10:07.000000 Relatorio_Ensalamento-2.4.4/Unificar_XML/Unificar_XML.py
+-rw-rw-rw-   0        0        0       27 2023-02-02 13:41:12.000000 Relatorio_Ensalamento-2.4.4/Unificar_XML/__init__.py
+-rw-rw-rw-   0        0        0      114 2023-07-14 20:55:39.183889 Relatorio_Ensalamento-2.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-07-14 20:55:33.000000 Relatorio_Ensalamento-2.4.4/setup.py
```

### Comparing `Relatorio_Ensalamento-2.4.3/PKG-INFO` & `Relatorio_Ensalamento-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Relatorio_Ensalamento
-Version: 2.4.3
+Version: 2.4.4
 Summary: Conversor utilizado para a geração do relatorio ensalamento
 Home-page: UNKNOWN
 Author: Matheus Henrique Rosa
 Author-email: m.rosa1@pucpr.br
 License: MIT
 Keywords: conversor relatorio ensalamento
 Platform: UNKNOWN
```

### Comparing `Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento/Relatorio_Ensalamento.py` & `Relatorio_Ensalamento-2.4.4/Relatorio_Ensalamento/Relatorio_Ensalamento.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,25 +21,27 @@
 import xlsxwriter
 import pytz
 import PySimpleGUI as psg
 from datetime import datetime as dt
 
 contador = 0
 
+
 # Função recebe o resultado do cálculo entre vagas - matriculados e gera um análise
 def analisar_diferenca(diferenca):
     if diferenca > 0:
         return "Vagas Disponíveis"
     elif diferenca == 0:
         return "Não há vagas"
     elif diferenca < 0:
         return "Vagas excedidas"
     else:
         return ""
 
+
 # Função recebe matriculados,  diferença entre matriculados - capacidade para gerar uma análise das capacidades
 def analisar_capacidade(matriculados, diferenca, capacidade, sala):
     if diferenca > 0:
         return "Capacidade disponível"
     elif sala == "Sem sala":
         return "Sem sala"
     elif matriculados > 0 and diferenca == 0:
@@ -49,14 +51,15 @@
     elif capacidade == 0:
         return "Sem Capacidade"
     elif diferenca < 0:
         return "Capacidade excedida"
     else:
         return ""
 
+
 # Função recebe o XML Unificado e dois dicionários um de escolas e outro de turmas fictícias
 def armazenaDadosAscXml(file_name_asc_xml, file_json_turmasfic, contador, file_json_escolas, f):
     tree_xml = ElementTree.parse(file_name_asc_xml)
     root = tree_xml.getroot()
     erro_log_turma = ""
     erro_log_sala = ""
 
@@ -157,54 +160,54 @@
         name = classrooms.get('name')
         short = classrooms.get('short')
 
         dict_classrooms[id] = name, short
 
     # armazenar a id como key e o name,short como value
     dict_class = {}
-    dict_multicom = {
-    '2304': 'CURIE-M',
-    '2236': 'ELIANE BRUM-M', '2237': 'ELIANE BRUM-N',
-    '2225': 'MARCELLO SERPA-M',
-    '2232': 'MARCELLO SERPA-N',
-    '2238': 'MARGARIDA KUNSCH-M',
-    '2214': 'PIAGET-N',
-    '1031183':'MARGARIDA KUNSCH-N'
-    }
+    dict_multicom = {'2304': 'CURIE-M',
+                     '2236': 'ELIANE BRUM-M', '2237': 'ELIANE BRUM-N',
+                     '2225': 'MARCELLO SERPA-M',
+                     '2232': 'MARCELLO SERPA-N',
+                     '2238': 'MARGARIDA KUNSCH-M',
+                     '2214': 'PIAGET-N',
+                     '1031183': 'MARGARIDA KUNSCH-N',
+                     '2301': 'LISPECTOR-M',
+                     '2201': 'MONTESSORI-M',
+                     '2349': 'CLFS-N',
+                     '2249': 'FERMAT-N'}
     for classes in root.iter("class"):
         # parametros
         id = classes.get('id')
         name = classes.get('name')
         short = classes.get('short')
-
         turmas_fic = dict(file_json_turmasfic)
-
-        if name.__contains__('Engenharia;') or name.__contains__('Multicom'):
+        if name.__contains__('Engenharia;') or name.__contains__('Multicom') or name.__contains__('Humanidades'):
             cr_curso = short.split(";")[5]
             periodo = short.split(";")[2]
             tipo = short.split(";")[3]
             turno = short.split(";")[4]
 
             chave_turma_fic = f"{cr_curso}|{periodo}"
 
             if cr_curso in dict_multicom.keys():
                 valor = dict_multicom[cr_curso]
                 new_name = f"{valor.split('-')[0]};{periodo};{tipo};{valor.split('-')[1]}"
 
                 name = new_name
 
             elif chave_turma_fic in turmas_fic.keys():
-                    name = turmas_fic[chave_turma_fic]
+                name = turmas_fic[chave_turma_fic]
 
-                    new_name = f"{name};{periodo};{tipo};{turno}"
-                    name = new_name
+                new_name = f"{name};{periodo};{tipo};{turno}"
+                name = new_name
             else:
-                    contador += 1
-                    f.write(f'#{contador} Aviso[Info]: erro ao converter a multicom name ={name} , short={short}''\n')
-                    continue
+                contador += 1
+                f.write(f'#{contador} Aviso[Info]: erro ao converter a multicom name ={name} , short={short}''\n')
+                continue
 
         dict_class[id] = name, short
 
     # armazenar a id como key e o period,days como value
     # para puxar a id da lesson e saber qual o horario e dia daquela aula
     dict_cards = {}
     for cards in root.iter("card"):
@@ -237,27 +240,29 @@
         id = lessons.get('id')
         subjectid = lessons.get('subjectid')
         groupid = lessons.get('groupids')
         classid = lessons.get('classids')
         classroomsid = lessons.get('classroomids')
 
         name_subject = dict_subject[subjectid]
+
         cr_curso = name_subject.split(';')[0]
 
         quantidade_turma = classid.count(',')
 
         posicao_turma = 0
 
         if quantidade_turma == 0:
             quantidade_turma = 1
         else:
             quantidade_turma += 1
 
         for i in range(0, quantidade_turma):
             try:
+
                 turma = str(dict_class[classid.split(',')[posicao_turma]]).replace(',', '/')
             except:
                 contador += 1
                 erro_log_turma += f'#{contador} Aviso[Ação]; Turma nao identificada na aula: {id}\n'
                 continue
 
             try:
@@ -328,14 +333,15 @@
 
             posicao_turma += 1
 
     f.write(erro_log_turma)
     f.write('\n\n')
     return valores
 
+
 # Função recebe o excel de capacidade e retorna apenas a abrev da sala e a sua capacidade
 def armazenaDadosCapacidade(file_name_capacidade, contador, f):
     # armazena os valores das colunas importantes
     todos_valores = []
 
     df = pandas.read_excel(file_name_capacidade, sheet_name="BASE DE CAPACIDADES CWB", header=2)
 
@@ -347,14 +353,15 @@
 
         posicao += 1
 
         todos_valores.append(f"{abrev_sala}|{capacidade}")
 
     return todos_valores
 
+
 def armazenaDadosTurmaDisciplina(file_name_turma_disciplina, file_json_sigla, contador, f):
     siglas = dict(file_json_sigla)
 
     def converteSigla(turma):
         if turma in siglas.keys():
             return siglas[turma]
         else:
@@ -418,24 +425,22 @@
         valores = f"{cr_curso}|{nome_curso}|{periodo}|{nome_turma}|{nome_disciplina}|{id_disciplina}|{divisao}|{dia}|{hora_inicio}|{hora_final}|" \
                   f"{agrupamento}|{turno}|{qtd_alunos}|{qtd_vagas}|{professor}|{estabelecimento}"
 
         todos_valores.append(valores)
 
     return todos_valores
 
+
 def gerarRelatorio(file_name_turma_disciplina, file_name_asc_xml, file_json_sigla, file_name_capacidade,
                    file_json_turmasfic, contador, file_json_escolas, file_json_tipos, f, file_name):
-
-    #transforma json em dict
     siglas = dict(file_json_sigla)
     escolas = dict(file_json_escolas)
     tipos = dict(file_json_tipos)
     log_sala = {}
 
-    #filter aviso
     warnings.simplefilter(action='ignore', category=UserWarning)
 
     def gerarTipo(tipo):
         if tipo in tipos.keys():
             return tipos[tipo]
         else:
             return tipo
@@ -455,48 +460,50 @@
     # armazenando dados
     array_turmas_disciplinas = armazenaDadosTurmaDisciplina(file_name_turma_disciplina, file_json_sigla, contador, f)
 
     array_asc_xml = armazenaDadosAscXml(file_name_asc_xml, file_json_turmasfic, contador, file_json_escolas, f)
 
     array_capacidade = armazenaDadosCapacidade(file_name_capacidade, contador, f)
 
-    #dict que retorna capacidade
     dict_capacidade = {}
+
     for i in array_capacidade:
         abrev_sala = i.split('|')[0]
         capacidade = i.split('|')[1]
 
         dict_capacidade[abrev_sala] = str(capacidade)
 
-    # cria dict dos dados do Excel
     dict_valores = {}
     dict_retorna_cr_disciplina = {}
     retorna_horario_inicio = {}
     horario_repetido = []
     for i in array_turmas_disciplinas:
         # valores chave
         cr_curso_aluno = i.split('|')[0]
         periodo = i.split('|')[2]
         nome_turma_final = i.split('|')[3].replace('- 2022/1', '').replace('2022/2', '').replace('2023/1', '').replace(
             '2023/2', '')
-        nome_turma = i.split('|')[3].replace('- 2022/1', '').replace('-', '').replace('2022/2', '').replace('2023/1','').replace('2023/2', '')
+        nome_turma = i.split('|')[3].replace('- 2022/1', '').replace('-', '').replace('2022/2', '').replace('2023/1',
+                                                                                                            '').replace(
+            '2023/2', '')
         # valores
         nome_disciplina = i.split('|')[4]
         id_disciplina = i.split('|')[5]
         divisao = i.split('|')[6]
         dia = i.split('|')[7]
         escola = geraEscola(cr_curso_aluno)
         hora_final = i.split('|')[9]
         cr_disciplina = i.split('|')[5]
         nome_curso = i.split('|')[1]
         agrupamento = i.split('|')[10]
         turno = i.split('|')[11]
         qtd_alunos = i.split('|')[12]
         qtd_vagas = i.split('|')[13]
-        hora_inicio_old = f"{i.split('|')[8]}:".ljust(8, '0')[0:8] if i.split('|')[8] != '--' and i.split('|')[8] != 'nan' else i.split('|')[8]
+        hora_inicio_old = f"{i.split('|')[8]}:".ljust(8, '0')[0:8] if i.split('|')[8] != '--' and i.split('|')[
+            8] != 'nan' else i.split('|')[8]
         professor = i.split('|')[14]
         estabelecimento = i.split('|')[15]
         hora_inicio = str(hora_inicio_old.split(':')[:-1]).replace(',', ':').replace("'", "").replace("[", "").replace(
             "]", "").replace(' ', '')
         chave_dia = f"{periodo},{nome_turma},{cr_disciplina},{hora_inicio}".replace(' ', '').replace('2022/2',
                                                                                                      '').replace(
             '2023/1', '').upper()
@@ -520,15 +527,14 @@
             'qtd_alunos': qtd_alunos,
             'qtd_vagas': qtd_vagas,
             'professor': professor,
             'Tipo': tipo,
             'estabelecimento': estabelecimento
         }
 
-        # se a aula tiver mais de um horario salva todos na mesma chave
         chave_horario_repetido = f"{chave}{hora_inicio}"
         try:
             if chave_horario_repetido not in horario_repetido:
                 retorna_horario_inicio[chave_dia] += f"|{hora_inicio},{dia},{divisao}"
                 horario_repetido.append(chave_horario_repetido)
         except:
             retorna_horario_inicio[chave_dia] = f"{hora_inicio},{dia},{divisao}"
@@ -605,16 +611,14 @@
         try:
             if not dict_retorna_abrev_salaxml[sala].__contains__(abrev_sala):
                 dict_retorna_abrev_salaxml[sala] += f",{abrev_sala}"
                 # dict_retorna_abrev_salaxml[sala] = abrev_sala
         except:
             dict_retorna_abrev_salaxml[sala] = abrev_sala
 
-
-    #mescla os dados
     log_sem_salas = {}
     log_sala_abrev = {}
     log_sem_turmas_disciplinas = {}
     for dados in array_asc_xml:
         erro_repetido = []
         # barra invertida para poder retirar ela do texto
         barra = r"'\'"
@@ -631,15 +635,16 @@
         try:
             nome_disciplina = dados.split('|')[6].split(';')[2]
         except:
             f.write(dados.split('|')[6] + 'esta no formato errado')
             continue
 
         # - tratamento nome turma
-        turma = dados.split('|')[2].split('/')[0].replace(barra, '').replace(barra, '').replace(barra, '').replace(barra, '').replace("'", '')
+        turma = dados.split('|')[2].split('/')[0].replace(barra, '').replace(barra, '').replace(barra, '').replace(
+            barra, '').replace("'", '')
         turma = turma[1:]
         turma_nome = converteSigla(turma.split(';')[0])
         # turma utilizada para melhor entendimento
         turma_final = f"{turma_nome} - {periodo} - {abrev_turma.split(';')[3]} - {abrev_turma.split(';')[4]}"
         # turma utilizada como key
         nome_turma = f"{turma_nome}{periodo}{abrev_turma.split(';')[3]}{turma.split(';')[-1][0]}"
         try:
@@ -817,15 +822,15 @@
         if dados[1]['Divisão'] == ' ' or dados[1]['Divisão'] == '  ' or dados[1]['Divisão'] == '   ':
             dados[1]['Divisão'] = '-'
         if dados[1] not in valores_repetidos:
             Relatorio[dados[0]] = dados[1]
             valores_repetidos.append(dados[1])
 
     df = pandas.DataFrame(data=Relatorio)
-    df = df.T
+    df = (df.T)
     df = df.drop_duplicates()
 
     df.insert(14, 'Análise Vagas', '')
     df.insert(15, 'Diferença Vagas', '')
     df.insert(23, 'Análise Capacidade', '')
     df.insert(24, 'Diferença Capacidade', '')
 
@@ -1087,15 +1092,16 @@
     worksheet.set_column('R:R', 20)
     worksheet.set_column('S:S', 20)
     worksheet.set_column('T:T', 45)
     worksheet.set_column('U:U', 42)
     worksheet.set_column('V:V', 20)
     worksheet.set_column('W:W', 42)
 
-    df_capacidade = pandas.read_excel(file_name_capacidade, sheet_name="BASE DE CAPACIDADES CWB", header=2,usecols=range(5, 26))
+    df_capacidade = pandas.read_excel(file_name_capacidade, sheet_name="BASE DE CAPACIDADES CWB", header=2,
+                                      usecols=range(5, 26))
 
     df_capacidade.to_excel(writer, index=False, sheet_name="Ambientes de Aprendizagem")
 
     df_horarios = pandas.DataFrame()
 
     df_horarios["NOME ESPAÇO ASC"] = df_capacidade["NOME ESPAÇO ASC"]
 
@@ -1134,14 +1140,15 @@
     worksheet.set_column('A:A', 25)
     worksheet.set_column('B:B', 25)
     worksheet.set_column('C:C', 15)
 
     writer.close()
     return nome_arquivo
 
+
 def retorna_analista(escola):
     if escola == 'Belas Artes':
         analista = 'Diego'
 
     elif escola == 'Ciências da Vida':
         analista = 'Sheyla'
 
@@ -1160,52 +1167,54 @@
     elif escola == 'Politécnica':
         analista = 'Edivane'
     else:
         analista = 'não encontrado'
 
     return analista
 
+
 def verifica_numero(valor):
     try:
         numero = int(valor)
     except:
         if valor == "nan":
             numero = 0
         else:
             numero = float(valor)
             numero = int(numero)
     return numero
 
+
 def retorna_status(sala, diferenca, capacidade):
     if sala == 'Sem sala':
         valor = 'Sem sala'
     elif capacidade == '0' or capacidade == 0:
         valor = 'Sem info capacidade'
     elif diferenca < 0:
         valor = 'Lotada - rever ensalamento'
     elif diferenca < 5:
         valor = 'Próximo da capacidade'
     else:
         valor = 'Ok'
     return valor
 
-def geracao_analise(arquivo_carga_horaria, arquivo_capacidade, arquivo_xml, file_name,caminho_auxiliar):
+
+def main(arquivo_carga_horaria, arquivo_capacidade, arquivo_xml, file_name, caminho_auxiliar):
     # pega somente o nome do arquivo para que o log seja salvo na mesma pasta
     utc_now = pytz.utc.localize(datetime.datetime.utcnow())
     dt_now = utc_now.astimezone(pytz.timezone("America/Sao_Paulo"))
     f = open(f"{caminho_auxiliar}/Log/{str(dt_now.strftime('%y-%m-%d %H-%M'))}.txt", "w+", encoding="utf8")
 
     file_name_turma_disciplina = arquivo_carga_horaria
 
     file_name_asc_xml = arquivo_xml
 
     file_name_capacidade = arquivo_capacidade
     print('Carregando...')
 
-    #salva arquivos auxiliares
     with open(f'{caminho_auxiliar}/siglas.json', 'r', encoding="utf-8") as j:
         file_json_sigla = json.loads(j.read())
 
     with open(f'{caminho_auxiliar}/turmasfic.json', 'r', encoding="utf-8") as j:
         file_json_turmasfic = json.loads(j.read())
 
     with open(f'{caminho_auxiliar}/escolas.json', 'r', encoding="utf-8") as j:
@@ -1214,20 +1223,24 @@
     with open(f'{caminho_auxiliar}/tipos.json', 'r', encoding="utf-8") as j:
         file_json_tipos = json.loads(j.read())
 
     nome_arquivo = gerarRelatorio(file_name_turma_disciplina, file_name_asc_xml, file_json_sigla, file_name_capacidade,
                                   file_json_turmasfic, contador, file_json_escolas, file_json_tipos, f, file_name)
     return nome_arquivo
 
-def gerarExcel(file_carga_horaria, file_capacidade, file_xml, file_name,caminho_aux):
+
+def gerarExcel(file_carga_horaria, file_capacidade, file_xml, file_name, caminho_aux):
     # le os valores vindo da tela
     arquivo_carga_horaria = file_carga_horaria
     arquivo_capacidade = file_capacidade
 
-    arquivo_xml = Unificar_XML.main(file_xml,caminho_aux)
+    arquivo_xml = Unificar_XML.main(file_xml, caminho_aux)
 
-    nome_arquivo = geracao_analise(arquivo_carga_horaria, arquivo_capacidade, arquivo_xml, file_name,caminho_aux)
+    nome_arquivo = main(arquivo_carga_horaria, arquivo_capacidade, arquivo_xml, file_name, caminho_aux)
+
+    Sugestao.main(nome_arquivo, arquivo_capacidade, caminho_aux)
 
-    Sugestao.main(nome_arquivo, arquivo_capacidade,caminho_aux)
 
 if __name__ == '__main__':
+
+
     gerarExcel()
```

### Comparing `Relatorio_Ensalamento-2.4.3/Relatorio_Ensalamento.egg-info/PKG-INFO` & `Relatorio_Ensalamento-2.4.4/Relatorio_Ensalamento.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Relatorio-Ensalamento
-Version: 2.4.3
+Version: 2.4.4
 Summary: Conversor utilizado para a geração do relatorio ensalamento
 Home-page: UNKNOWN
 Author: Matheus Henrique Rosa
 Author-email: m.rosa1@pucpr.br
 License: MIT
 Keywords: conversor relatorio ensalamento
 Platform: UNKNOWN
```

### Comparing `Relatorio_Ensalamento-2.4.3/Sugestao/Sugestao.py` & `Relatorio_Ensalamento-2.4.4/Sugestao/Sugestao.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,31 +29,34 @@
             porcentagem_utilizacao = 0 - alunos_matriculados
         else:
             porcentagem_utilizacao = (alunos_matriculados / capacidade_sala) * 100
             porcentagem_utilizacao = round(porcentagem_utilizacao, 2)
 
         self.porcentagem_utilizacao = round(porcentagem_utilizacao, 2)
 
-
+class Subutilizada:
+    def __init__(self, sala, disciplina):
+        self.sala = sala
+        self.disciplina = disciplina
 class AmbienteDeAprendizagem:
-    def __init__(self, nome_sala, nome_sala_abrev, capacidade_sala, status, disciplina, tipo, tipo_detalhado, escola):
+    def __init__(self, nome_sala, nome_sala_abrev, capacidade_sala, status, disciplina, tipo, tipo_detalhado, escola,curso):
         self.nome_sala = nome_sala
         self.nome_sala_abrev = nome_sala_abrev
 
         try:
             self.capacidade_sala = int(capacidade_sala)
         except:
             self.capacidade_sala = 0
 
         self.status = status
         self.Disciplina = disciplina
         self.tipo = tipo
         self.tipo_detalhado = tipo_detalhado
         self.escola = escola
-
+        self.curso = curso
 
 def create_objects(file_name, dict_retorna_status_type, list, dict_retorna_utilizado_graduacao):
     df = pandas.read_excel(file_name, sheet_name='Completo')
     list_sem_status = []
     dict_retorna_escola = {}
 
     for data in df.iterrows():
@@ -66,14 +69,15 @@
         nome_sala = data[1]['Sala']
         nome_sala_abrev = data[1]['Sala Abreviação']
         capacidade_sala = data[1]['Capacidade da Sala']
         diferenca_capacidade = data[1]['Diferença Capacidade']
         analise_capacidade = data[1]['Análise Capacidade']
         df_sala = df.loc[df['Sala'] == nome_sala]
         escola = data[1]['Escola']
+        curso = data[1]['Curso']
         dia = data[1]['Dia da Semana']
 
         try:
             utilizado_graduacao = dict_retorna_utilizado_graduacao[nome_sala]
         except:
             utilizado_graduacao = "Sim"
 
@@ -112,18 +116,18 @@
             tipo_detalhado = dict_retorna_status_type[nome_sala][2]
         except:
             if nome_sala not in list_sem_status:
                 list_sem_status.append(nome_sala)
                 # print('Sem status pois, não encontrada na capacidade sala: ',nome_sala)
             status = 'Ativa'
             tipo = " "
-            tipo_detalhado = " "
+            tipo_detalhado = "Sala não esta planilha de infra."
 
         sala = AmbienteDeAprendizagem(nome_sala, nome_sala_abrev, capacidade_sala, status, list_objects_disciplinas,
-                                      tipo, tipo_detalhado, escola)
+                                      tipo, tipo_detalhado, escola,curso)
         dict_retorna_escola[nome_sala] = escola
         list.append(sala)
 
     return list, dict_retorna_escola
 
 
 def insert_matriz(list):
@@ -132,16 +136,16 @@
         return [["         "] * n_colunas for _ in range(n_linhas)]
 
     matriz = create_matriz(len(list), 140)
 
     row = 0
     for object in list:
         matriz[row][0] = object
-        if object.Turma != None:
-            for disciplina in object.Turma:
+        if object.Disciplina != None:
+            for disciplina in object.Disciplina:
                 list_aux = []
                 indice = get_indice(disciplina)
                 matriz[row][indice] = disciplina
         row += 1
 
     return matriz
 
@@ -292,25 +296,27 @@
     salas_ativas = []
     list = []
     for sala in List_objects:
         salas_ativas.append(sala.nome_sala)
 
     df = pandas.read_excel(arquivo_capacidade, sheet_name="BASE DE CAPACIDADES CWB", header=2)
     for data in df.iterrows():
+
         nome_sala = data[1]['NOME ESPAÇO ASC']
         utilizado_graduacao = data[1]['UTILIZADO NA GRADUACAO']
 
         if utilizado_graduacao == "Não" or nome_sala.__contains__("AULA EXTERNA") is False:
             continue
 
         if nome_sala not in salas_ativas:
             nome_sala_abrev = data[1]['CÓD. ASC'].replace(' ', '')
             capacidade_sala = data[1]['CAPACIDADE']
             status = data[1]['STATUS']
             tipo = str(data[1]['TIPO DE INSTALAÇÃO'])
+
             tipo_detalhado = str(data[1]['TIPO DE INSTALAÇÃO DETALHADO'])
 
             try:
                 escola = dict_retorna_escola[nome_sala]
             except:
                 escola = ""
 
@@ -338,21 +344,37 @@
 
     def retorna_sugestao_sugestao_subutilizada(nome_sala, nome_disciplina, dia, hora_inicio, analise,
                                                dict_retorna_sugestao_subutilizada):
         key = f"{nome_sala},{nome_disciplina},{dia},{hora_inicio}"
         key = key.upper()
         sala = ""
         numero = 1
+        list_aux = []
+
         if analise == 'Capacidade excedida' or analise == 'Sem Capacidade' \
                 or analise == 'Sala lotada' or analise == 'Sem sala':
             if key in dict_retorna_sugestao_subutilizada.keys():
                 list_sala = dict_retorna_sugestao_subutilizada[key]
+
+                num = len(list_sala)
                 for sala_aux in list_sala:
-                    sala += f"{numero}. {sala_aux.nome_sala} ({sala_aux.capacidade_sala}) | \n"
+                    nome = sala_aux.sala.nome_sala
+                    capacidade = sala_aux.sala.capacidade_sala
+                    tipo = sala_aux.sala.tipo.lower()
+                    alunos_matriculados = sala_aux.disciplina.alunos_matriculados
+
+                    sala += f"{numero}. {nome} ({alunos_matriculados}/{capacidade}) | \n"
                     numero += 1
+
+                while numero <= 5:
+                    sala += f'{numero}. Nenhum ambiente do tipo "{tipo}" esta disponivel | \n'
+                    numero += 1
+
+
+
         sala = sala[:-1]
         return sala
 
     def retorna_sugestao_list(nome_sala, nome_disciplina, dia, hora_inicio, analise, dict_retorna_sugestao_list):
         key = f"{nome_sala},{nome_disciplina},{dia},{hora_inicio}"
         key = key.upper()
         sala = ""
@@ -678,23 +700,27 @@
     writer.close()
 
 
 def create_dict_status_type(arquivo_capacidade, dict_retorna_utilizado_graduacao):
     dict_retona_status = {}
 
     df = pandas.read_excel(arquivo_capacidade, sheet_name="BASE DE CAPACIDADES CWB", header=2)
+    df = df.fillna('')
     for data in df.iterrows():
         nome_sala = str(data[1]['NOME ESPAÇO ASC'])
         status = str(data[1]['STATUS'])
         tipo = str(data[1]['TIPO DE INSTALAÇÃO'])
         tipo_detalhado = str(data[1]['TIPO DE INSTALAÇÃO DETALHADO'])
         utilizado_graduacao = data[1]['UTILIZADO NA GRADUACAO']
 
         dict_retorna_utilizado_graduacao[nome_sala] = utilizado_graduacao
 
+        if tipo_detalhado == '':
+            tipo_detalhado = "Não especificado na planilha de infra."
+
         dict_retona_status[nome_sala] = status, tipo, tipo_detalhado
 
     return dict_retona_status, dict_retorna_utilizado_graduacao
 
 
 def analyze_matriz(matriz, df_capacidade_excedida, dict_retorna_status_type, dict_retorna_prioridade_escola):
     m = np.array(matriz)
@@ -1292,17 +1318,19 @@
             detailed_type = dict_retorna_status_type[classroom_name][2]
         except:
             type = " "
             detailed_type = " "
 
         # buscando as opções na matriz
         #      verificando se esta vazio e se sua capacidade atinge menos de 30%
+        disciplina = {}
         for row_aux in range(0, row_number):
             if matriz[row_aux][column] != "         " \
-                    and matriz[row_aux][column].porcentagem_utilizacao < 45:
+                    and matriz[row_aux][column].porcentagem_utilizacao < 50:
+                disciplina[matriz[row_aux][0]] = matriz[row_aux][column]
                 list_underused_classroom.append(matriz[row_aux][0])
 
         # lista que vai ser inserida como sugestão
         list_aux = []
 
         # ordenando em ordem crescente a lista
         list_underused_classroom = sorted(list_underused_classroom, key=lambda x: x.capacidade_sala)
@@ -1319,14 +1347,18 @@
 
             # atributos da sala sendo analisada
             capacidade_sala_aux = classroom.capacidade_sala
             bloco_aux = classroom.nome_sala.split('-')[0]
             detailed_type_aux = classroom.tipo_detalhado
             status = classroom.status
 
+            #ignorando salas sem tipo detalhado definido
+            if detailed_type_aux == "Não especificado na planilha de infra." or detailed_type_aux == "Sala não esta planilha de infra.":
+                continue
+
             # verificando se é um numero valido
             try:
                 int(capacidade_sala_aux)
             except:
                 continue
 
             # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
@@ -1336,15 +1368,19 @@
             if len(list_aux) >= 5:
                 break
 
             if capacidade_sala_aux > capacidade_esperada and bloco == bloco_aux and \
                     classroom.nome_sala not in repeated_classrooms \
                     and status == 'Ativa' and detailed_type == detailed_type_aux:
                 repeated_classrooms.append(classroom.nome_sala)
-                list_aux.append(classroom)
+
+                valor = f"{classroom.nome_sala},{classroom.capacidade_sala},{disciplina[classroom].alunos_matriculados},{type}"
+
+                sala_subutilizada = Subutilizada(classroom,disciplina[classroom])
+                list_aux.append(sala_subutilizada)
                 dict_retorna_sugestao_subutilizada[key] = list_aux
 
         # todo 2 verificação
         # verificando o bloco prioridade da escola e o tipo detalhado
         for numero_bloco in list_blocos:
 
             if numero_bloco <= 9:
@@ -1357,111 +1393,18 @@
 
                 # atributos da sala sendo analisada
                 capacidade_sala_aux = classroom.capacidade_sala
                 bloco_aux = classroom.nome_sala.split('-')[0]
                 detailed_type_aux = classroom.tipo_detalhado
                 status = classroom.status
 
-                # verificando se é um numero valido
-                try:
-                    int(capacidade_sala_aux)
-                except:
+                # ignorando salas sem tipo detalhado definido
+                if detailed_type_aux == "Não especificado na planilha de infra." or detailed_type_aux == "Sala não esta planilha de infra.":
                     continue
 
-                # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
-                key = f"{classroom_name},{subject_name},{day},{start_hour}"
-                key = key.upper()
-
-                if len(list_aux) >= 5:
-                    break
-
-                if capacidade_sala_aux > capacidade_esperada and bloco == bloco_aux and \
-                        classroom.nome_sala not in repeated_classrooms \
-                        and status == 'Ativa' and detailed_type == detailed_type_aux:
-                    repeated_classrooms.append(classroom.nome_sala)
-                    list_aux.append(classroom)
-                    dict_retorna_sugestao_subutilizada[key] = list_aux
-
-        # todo 3 verificação
-        # verificando o tipo detalhado
-        for classroom in list_underused_classroom:
-
-            # atributos da sala sendo analisada
-            capacidade_sala_aux = classroom.capacidade_sala
-            detailed_type_aux = classroom.tipo_detalhado
-            status = classroom.status
-
-            # verificando se é um numero valido
-            try:
-                int(capacidade_sala_aux)
-            except:
-                continue
-
-            # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
-            key = f"{classroom_name},{subject_name},{day},{start_hour}"
-            key = key.upper()
-
-            if len(list_aux) >= 5:
-                break
-
-            if capacidade_sala_aux > capacidade_esperada and \
-                    classroom.nome_sala not in repeated_classrooms \
-                    and status == 'Ativa' and detailed_type == detailed_type_aux:
-                repeated_classrooms.append(classroom.nome_sala)
-                list_aux.append(classroom)
-                dict_retorna_sugestao_subutilizada[key] = list_aux
-
-        # todo 4 verificação
-        # verificando o bloco atual e o tipo
-        for classroom in list_underused_classroom:
-
-            # atributos da sala sendo analisada
-            capacidade_sala_aux = classroom.capacidade_sala
-            bloco_aux = classroom.nome_sala.split('-')[0]
-            type_aux = classroom.tipo
-            status = classroom.status
-
-            # verificando se é um numero valido
-            try:
-                int(capacidade_sala_aux)
-            except:
-                continue
-
-            # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
-            key = f"{classroom_name},{subject_name},{day},{start_hour}"
-            key = key.upper()
-
-            if len(list_aux) >= 5:
-                break
-
-            if capacidade_sala_aux > capacidade_esperada and bloco == bloco_aux and \
-                    classroom.nome_sala not in repeated_classrooms \
-                    and status == 'Ativa' and type == type_aux:
-                repeated_classrooms.append(classroom.nome_sala)
-                list_aux.append(classroom)
-                dict_retorna_sugestao_subutilizada[key] = list_aux
-
-        # todo 5 verificação
-        # verificando o bloco prioridade da escola e o tipo
-        for numero_bloco in list_blocos:
-
-            if numero_bloco <= 9:
-                bloco = f"Bloco 0{numero_bloco} "
-            else:
-                bloco = f"Bloco {numero_bloco} "
-
-            # utilizando o bloco para validar
-            for classroom in list_underused_classroom:
-
-                # atributos da sala sendo analisada
-                capacidade_sala_aux = classroom.capacidade_sala
-                bloco_aux = classroom.nome_sala.split('-')[0]
-                type_aux = classroom.tipo
-                status = classroom.status
-
                 # verificando se é um numero valido
                 try:
                     int(capacidade_sala_aux)
                 except:
                     continue
 
                 # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
@@ -1469,90 +1412,20 @@
                 key = key.upper()
 
                 if len(list_aux) >= 5:
                     break
 
                 if capacidade_sala_aux > capacidade_esperada and bloco == bloco_aux and \
                         classroom.nome_sala not in repeated_classrooms \
-                        and status == 'Ativa' and type == type_aux:
-                    repeated_classrooms.append(classroom.nome_sala)
-                    list_aux.append(classroom)
-                    dict_retorna_sugestao_subutilizada[key] = list_aux
-
-        # todo 6 verificação
-        # verificando o tipo
-        for numero_bloco in list_blocos:
-
-            if numero_bloco <= 9:
-                bloco = f"Bloco 0{numero_bloco} "
-            else:
-                bloco = f"Bloco {numero_bloco} "
-
-            # utilizando o bloco para validar
-            for classroom in list_underused_classroom:
-
-                # atributos da sala sendo analisada
-                capacidade_sala_aux = classroom.capacidade_sala
-                type_aux = classroom.tipo
-                status = classroom.status
-
-                # verificando se é um numero valido
-                try:
-                    int(capacidade_sala_aux)
-                except:
-                    continue
-
-                # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
-                key = f"{classroom_name},{subject_name},{day},{start_hour}"
-                key = key.upper()
-
-                if len(list_aux) >= 5:
-                    break
-
-                if capacidade_sala_aux > capacidade_esperada and \
-                        classroom.nome_sala not in repeated_classrooms \
-                        and status == 'Ativa' and type == type_aux:
+                        and status == 'Ativa' and detailed_type == detailed_type_aux:
                     repeated_classrooms.append(classroom.nome_sala)
-                    list_aux.append(classroom)
-                    dict_retorna_sugestao_subutilizada[key] = list_aux
 
-        # todo 7 verificação
-        # sem verificação
-        for numero_bloco in list_blocos:
-
-            if numero_bloco <= 9:
-                bloco = f"Bloco 0{numero_bloco} "
-            else:
-                bloco = f"Bloco {numero_bloco} "
-
-            # utilizando o bloco para validar
-            for classroom in list_underused_classroom:
-
-                # atributos da sala sendo analisada
-                capacidade_sala_aux = classroom.capacidade_sala
-                status = classroom.status
-
-                # verificando se é um numero valido
-                try:
-                    int(capacidade_sala_aux)
-                except:
-                    continue
-
-                # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
-                key = f"{classroom_name},{subject_name},{day},{start_hour}"
-                key = key.upper()
-
-                if len(list_aux) >= 5:
-                    break
-
-                if capacidade_sala_aux > capacidade_esperada and \
-                        classroom.nome_sala not in repeated_classrooms \
-                        and status == 'Ativa':
-                    repeated_classrooms.append(classroom.nome_sala)
-                    list_aux.append(classroom)
+                    valor = f"{classroom.nome_sala},{classroom.capacidade_sala},{disciplina[classroom].alunos_matriculados},{type}"
+                    sala_subutilizada = Subutilizada(classroom, disciplina[classroom])
+                    list_aux.append(sala_subutilizada)
                     dict_retorna_sugestao_subutilizada[key] = list_aux
 
     return dict_retorna_sugestao_subutilizada
 
 
 def create_dict_prioridade_escola(caminho_aux):
     df_prioridades = pandas.read_excel(f'{caminho_aux}/Prioridade_escolas.xlsx')
@@ -1626,8 +1499,9 @@
                                                      dict_retorna_prioridade_escola)
 
     print('Inserindo no excel...')
     insert_excel(nome_arquivo, dict_retorna_sugestao, dict_retorna_sugestao_list, dict_retorna_sugestao_subutilizada)
     print("Arquivo gerado com sucesso.")
 
 if __name__ == '__main__':
+
     main()
```

### Comparing `Relatorio_Ensalamento-2.4.3/Unificar_XML/Unificar_XML.py` & `Relatorio_Ensalamento-2.4.4/Unificar_XML/Unificar_XML.py`

 * *Files identical despite different names*

