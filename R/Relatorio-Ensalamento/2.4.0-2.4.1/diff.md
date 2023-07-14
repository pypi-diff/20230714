# Comparing `tmp/Relatorio-Ensalamento-2.4.0.tar.gz` & `tmp/Relatorio_Ensalamento-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Relatorio-Ensalamento-2.4.0.tar", last modified: Tue Mar 14 18:42:54 2023, max compression
+gzip compressed data, was "Relatorio_Ensalamento-2.4.1.tar", last modified: Fri Jul 14 18:39:37 2023, max compression
```

## Comparing `Relatorio-Ensalamento-2.4.0.tar` & `Relatorio_Ensalamento-2.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 18:42:54.066497 Relatorio-Ensalamento-2.4.0/
--rw-rw-rw-   0        0        0      506 2023-03-14 18:42:54.066497 Relatorio-Ensalamento-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-01-27 12:58:30.000000 Relatorio-Ensalamento-2.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-14 18:42:53.986300 Relatorio-Ensalamento-2.4.0/Relatorio_Ensalamento/
--rw-rw-rw-   0        0        0    50734 2023-03-14 18:42:23.000000 Relatorio-Ensalamento-2.4.0/Relatorio_Ensalamento/Relatorio_Ensalamento.py
--rw-rw-rw-   0        0        0       38 2023-01-26 12:04:50.000000 Relatorio-Ensalamento-2.4.0/Relatorio_Ensalamento/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 18:42:54.035343 Relatorio-Ensalamento-2.4.0/Relatorio_Ensalamento.egg-info/
--rw-rw-rw-   0        0        0      506 2023-03-14 18:42:53.000000 Relatorio-Ensalamento-2.4.0/Relatorio_Ensalamento.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-03-14 18:42:53.000000 Relatorio-Ensalamento-2.4.0/Relatorio_Ensalamento.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 18:42:53.000000 Relatorio-Ensalamento-2.4.0/Relatorio_Ensalamento.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-03-14 18:42:53.000000 Relatorio-Ensalamento-2.4.0/Relatorio_Ensalamento.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-14 18:42:54.050951 Relatorio-Ensalamento-2.4.0/Sugestao/
--rw-rw-rw-   0        0        0    62196 2023-03-13 19:57:07.000000 Relatorio-Ensalamento-2.4.0/Sugestao/Sugestao.py
--rw-rw-rw-   0        0        0       25 2023-01-26 11:56:59.000000 Relatorio-Ensalamento-2.4.0/Sugestao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-14 18:42:54.066497 Relatorio-Ensalamento-2.4.0/Unificar_XML/
--rw-rw-rw-   0        0        0    18277 2023-03-10 16:38:35.000000 Relatorio-Ensalamento-2.4.0/Unificar_XML/Unificar_XML.py
--rw-rw-rw-   0        0        0       27 2023-02-02 13:41:12.000000 Relatorio-Ensalamento-2.4.0/Unificar_XML/__init__.py
--rw-rw-rw-   0        0        0      114 2023-03-14 18:42:54.082143 Relatorio-Ensalamento-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0      503 2023-03-14 18:15:35.000000 Relatorio-Ensalamento-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:39:37.503948 Relatorio_Ensalamento-2.4.1/
+-rw-rw-rw-   0        0        0      549 2023-07-14 18:39:37.504947 Relatorio_Ensalamento-2.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-01-27 12:58:30.000000 Relatorio_Ensalamento-2.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 18:39:37.454432 Relatorio_Ensalamento-2.4.1/Relatorio_Ensalamento/
+-rw-rw-rw-   0        0        0    48968 2023-02-09 19:07:56.000000 Relatorio_Ensalamento-2.4.1/Relatorio_Ensalamento/Relatorio_Ensalamento.py
+-rw-rw-rw-   0        0        0       38 2023-01-26 12:04:50.000000 Relatorio_Ensalamento-2.4.1/Relatorio_Ensalamento/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:39:37.482859 Relatorio_Ensalamento-2.4.1/Relatorio_Ensalamento.egg-info/
+-rw-rw-rw-   0        0        0      549 2023-07-14 18:39:37.000000 Relatorio_Ensalamento-2.4.1/Relatorio_Ensalamento.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-14 18:39:37.000000 Relatorio_Ensalamento-2.4.1/Relatorio_Ensalamento.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 18:39:37.000000 Relatorio_Ensalamento-2.4.1/Relatorio_Ensalamento.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-14 18:39:37.000000 Relatorio_Ensalamento-2.4.1/Relatorio_Ensalamento.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 18:39:37.491854 Relatorio_Ensalamento-2.4.1/Sugestao/
+-rw-rw-rw-   0        0        0    64234 2023-07-14 18:36:16.000000 Relatorio_Ensalamento-2.4.1/Sugestao/Sugestao.py
+-rw-rw-rw-   0        0        0       25 2023-01-26 11:56:59.000000 Relatorio_Ensalamento-2.4.1/Sugestao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 18:39:37.499856 Relatorio_Ensalamento-2.4.1/Unificar_XML/
+-rw-rw-rw-   0        0        0    17469 2023-02-02 16:23:54.000000 Relatorio_Ensalamento-2.4.1/Unificar_XML/Unificar_XML.py
+-rw-rw-rw-   0        0        0       27 2023-02-02 13:41:12.000000 Relatorio_Ensalamento-2.4.1/Unificar_XML/__init__.py
+-rw-rw-rw-   0        0        0      114 2023-07-14 18:39:37.513494 Relatorio_Ensalamento-2.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-07-14 18:39:33.000000 Relatorio_Ensalamento-2.4.1/setup.py
```

### Comparing `Relatorio-Ensalamento-2.4.0/Relatorio_Ensalamento/Relatorio_Ensalamento.py` & `Relatorio_Ensalamento-2.4.1/Relatorio_Ensalamento/Relatorio_Ensalamento.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import json
 import warnings
 import datetime
 from unidecode import unidecode
 import xlsxwriter
 import pytz
 import PySimpleGUI as psg
-from datetime import datetime as dt
 
 contador = 0
 
 
 # Função recebe o resultado do cálculo entre vagas - matriculados e gera um análise
 def analisar_diferenca(diferenca):
     if diferenca > 0:
@@ -53,15 +52,15 @@
     elif diferenca < 0:
         return "Capacidade excedida"
     else:
         return ""
 
 
 # Função recebe o XML Unificado e dois dicionários um de escolas e outro de turmas fictícias
-def armazenaDadosAscXml(file_name_asc_xml, file_json_turmasfic, contador, file_json_escolas, f,dict_turma_fic):
+def armazenaDadosAscXml(file_name_asc_xml, file_json_turmasfic, contador, file_json_escolas, f):
     tree_xml = ElementTree.parse(file_name_asc_xml)
     root = tree_xml.getroot()
     erro_log_turma = ""
     erro_log_sala = ""
 
     # converte period
     # retorna starttime/endtime
@@ -160,47 +159,32 @@
         name = classrooms.get('name')
         short = classrooms.get('short')
 
         dict_classrooms[id] = name, short
 
     # armazenar a id como key e o name,short como value
     dict_class = {}
-    dict_multicom = {'2304': 'CURIE-M',
-                     '2236': 'ELIANE BRUM-M', '2237': 'ELIANE BRUM-N',
-                     '2225': 'MARCELLO SERPA-M',
-                     '2232': 'MARCELLO SERPA-N',
-                     '2238': 'MARGARIDA KUNSCH-M',
-                     '2214': 'PIAGET-N',
-                     '1031183': 'MARGARIDA KUNSCH-N',
-                     '2301': 'LISPECTOR-M',
-                     '2201': 'MONTESSORI-M',
-                     '2349': 'CLFS-N',
-                     '2249': 'FERMAT-N'}
     for classes in root.iter("class"):
         # parametros
         id = classes.get('id')
         name = classes.get('name')
         short = classes.get('short')
+
         turmas_fic = dict(file_json_turmasfic)
-        if name.__contains__('Engenharia;') or name.__contains__('Multicom') or name.__contains__('Humanidades'):
+
+        if name.__contains__('Engenharia;') or name.__contains__('Multicom'):
             cr_curso = short.split(";")[5]
             periodo = short.split(";")[2]
             tipo = short.split(";")[3]
             turno = short.split(";")[4]
 
             chave_turma_fic = f"{cr_curso}|{periodo}"
 
-            if cr_curso in dict_multicom.keys():
-                valor = dict_multicom[cr_curso]
-                new_name = f"{valor.split('-')[0]};{periodo};{tipo};{valor.split('-')[1]}"
-
-                name = new_name
-
-            elif chave_turma_fic in dict_turma_fic.keys():
-                name = dict_turma_fic[chave_turma_fic]
+            if chave_turma_fic in turmas_fic.keys():
+                name = turmas_fic[chave_turma_fic]
 
                 new_name = f"{name};{periodo};{tipo};{turno}"
                 name = new_name
             else:
                 contador += 1
                 f.write(f'#{contador} Aviso[Info]: erro ao converter a multicom name ={name} , short={short}''\n')
                 continue
@@ -365,15 +349,14 @@
         if turma in siglas.keys():
             return siglas[turma]
         else:
             return turma
 
     # armazena os valores das colunas importantes
     todos_valores = []
-    dict_turma_fic = {}
 
     df = pandas.read_excel(file_name_turma_disciplina)
     posicao = 0
     df['Divisão'] = df['Divisão'].fillna('Teórico')
     for i in df.iterrows():
 
         cortes = df['Tem Corte'][posicao]
@@ -413,31 +396,25 @@
         dia = df['Data da Semana'][posicao]
         hora_inicio = df['Horário de Início'][posicao]
         hora_final = df['Horário de Término'][posicao]
         agrupamento = df['Agrupamento'][posicao]
         turno = df['Turno'][posicao]
         qtd_alunos = df['Qtde de Alunos Matriculados'][posicao]
         qtd_vagas = df['Nr Vagas Cadastradas'][posicao]
-        estabelecimento = df['Estabelecimento'][posicao]
         posicao += 1
 
         if divisao == ' ' or divisao == '  ' or divisao == '   ' or divisao == 'Teórico':
             divisao = '  '
 
         valores = f"{cr_curso}|{nome_curso}|{periodo}|{nome_turma}|{nome_disciplina}|{id_disciplina}|{divisao}|{dia}|{hora_inicio}|{hora_final}|" \
-                  f"{agrupamento}|{turno}|{qtd_alunos}|{qtd_vagas}|{professor}|{estabelecimento}"
-
-        chave = f"{cr_curso}|{periodo}"
-        valor =nome_turma.split('-')[0]
-        if nome_turma.__contains__('ENGENHARIA') or len(valor) > 5 :
-            dict_turma_fic[chave] = valor[:-1]
+                  f"{agrupamento}|{turno}|{qtd_alunos}|{qtd_vagas}|{professor}"
 
         todos_valores.append(valores)
 
-    return todos_valores,dict_turma_fic
+    return todos_valores
 
 
 def gerarRelatorio(file_name_turma_disciplina, file_name_asc_xml, file_json_sigla, file_name_capacidade,
                    file_json_turmasfic, contador, file_json_escolas, file_json_tipos, f, file_name):
     siglas = dict(file_json_sigla)
     escolas = dict(file_json_escolas)
     tipos = dict(file_json_tipos)
@@ -460,17 +437,17 @@
     def geraEscola(cr_curso):
         if cr_curso in escolas.keys():
             return escolas[cr_curso]
         else:
             return ' '
 
     # armazenando dados
-    array_turmas_disciplinas,dict_turma_fic = armazenaDadosTurmaDisciplina(file_name_turma_disciplina, file_json_sigla, contador, f)
+    array_turmas_disciplinas = armazenaDadosTurmaDisciplina(file_name_turma_disciplina, file_json_sigla, contador, f)
 
-    array_asc_xml = armazenaDadosAscXml(file_name_asc_xml, file_json_turmasfic, contador, file_json_escolas, f,dict_turma_fic)
+    array_asc_xml = armazenaDadosAscXml(file_name_asc_xml, file_json_turmasfic, contador, file_json_escolas, f)
 
     array_capacidade = armazenaDadosCapacidade(file_name_capacidade, contador, f)
 
     dict_capacidade = {}
 
     for i in array_capacidade:
         abrev_sala = i.split('|')[0]
@@ -488,30 +465,28 @@
         periodo = i.split('|')[2]
         nome_turma_final = i.split('|')[3].replace('- 2022/1', '').replace('2022/2', '').replace('2023/1', '').replace(
             '2023/2', '')
         nome_turma = i.split('|')[3].replace('- 2022/1', '').replace('-', '').replace('2022/2', '').replace('2023/1',
                                                                                                             '').replace(
             '2023/2', '')
         # valores
-        nome_disciplina = i.split('|')[4]
+        nome_disciplina = unidecode(i.split('|')[4]).upper()
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
-        hora_inicio_old = f"{i.split('|')[8]}:".ljust(8, '0')[0:8] if i.split('|')[8] != '--' and i.split('|')[
-            8] != 'nan' else i.split('|')[8]
+        hora_inicio_old = i.split('|')[8]
         professor = i.split('|')[14]
-        estabelecimento = i.split('|')[15]
         hora_inicio = str(hora_inicio_old.split(':')[:-1]).replace(',', ':').replace("'", "").replace("[", "").replace(
             "]", "").replace(' ', '')
         chave_dia = f"{periodo},{nome_turma},{cr_disciplina},{hora_inicio}".replace(' ', '').replace('2022/2',
                                                                                                      '').replace(
             '2023/1', '').upper()
         chave = f"{periodo},{nome_turma},{cr_disciplina},{hora_inicio},{dia},{divisao}".replace(' ', '').upper()
         tipo = gerarTipo(agrupamento)
@@ -529,16 +504,15 @@
             'hora_final': hora_final,
             'cr_disciplina': cr_disciplina,
             'Agrupamento': agrupamento,
             'Turno': turno,
             'qtd_alunos': qtd_alunos,
             'qtd_vagas': qtd_vagas,
             'professor': professor,
-            'Tipo': tipo,
-            'estabelecimento': estabelecimento
+            'Tipo': tipo
         }
 
         chave_horario_repetido = f"{chave}{hora_inicio}"
         try:
             if chave_horario_repetido not in horario_repetido:
                 retorna_horario_inicio[chave_dia] += f"|{hora_inicio},{dia},{divisao}"
                 horario_repetido.append(chave_horario_repetido)
@@ -571,16 +545,14 @@
 
         turma_nome = converteSigla(turma.split(';')[0])
         abrev_turma = dados.split('|')[2].split('/')[1].replace(barra, '').replace(barra, '').replace(barra,
                                                                                                       '').replace(barra,
                                                                                                                   '').replace(
             "'", '').replace('(', '')
         nome_turma = f"{turma_nome}{periodo}{abrev_turma.split(';')[3]}{turma.split(';')[-1][0]}"
-        if nome_turma.__contains__('LEAEAD'):
-            nome_turma = f"{abrev_turma.split(';')[3]}{turma.split(';')[-1][0]}"
         divisao = dados.split('|')[8]
         dia = dados.split('|')[7]
         hora_inicio = dados.split('|')[9]
         abrev_sala = dados.split('|')[4]
         abrev_sala = abrev_sala.replace(')', '').replace("'", "").replace(' ', '')
 
         try:
@@ -651,17 +623,14 @@
             barra, '').replace("'", '')
         turma = turma[1:]
         turma_nome = converteSigla(turma.split(';')[0])
         # turma utilizada para melhor entendimento
         turma_final = f"{turma_nome} - {periodo} - {abrev_turma.split(';')[3]} - {abrev_turma.split(';')[4]}"
         # turma utilizada como key
         nome_turma = f"{turma_nome}{periodo}{abrev_turma.split(';')[3]}{turma.split(';')[-1][0]}"
-
-        if nome_turma.__contains__('LEAEAD'):
-            nome_turma = f"{abrev_turma.split(';')[3]}{turma.split(';')[-1][0]}"
         try:
             cr = dados.split('|')[6].split(';')[3]
 
             cr_curso = dados.split('|')[6].split(';')[0]
             try:
                 cr_disciplina = int(cr)
             except:
@@ -682,15 +651,14 @@
 
         # chave
         chave = f"{periodo},{nome_turma},{cr_disciplina},{hora_inicio_chave_sala}".replace(' ', '').upper().replace("'",
                                                                                                                     '')
 
         # armazena a lista de horarios de inicio da turma e disciplina para alocar na chave
         try:
-
             lista_horario_de_inicio_dia = retorna_horario_inicio[chave]
         except:
             try:
                 chave_fic = f"{periodo},{nome_turma[:-1]},{cr_disciplina},{hora_inicio_chave_sala}".replace(' ',
                                                                                                             '').upper().replace(
                     "'", '')
                 lista_horario_de_inicio_dia = retorna_horario_inicio[chave_fic]
@@ -774,15 +742,15 @@
                 except:
                     contador += 1
                     f.write(f'#{contador} Aviso[Ação]: dia e hora nao encontrado ' + chave_dia_hora + '\n')
                     continue
                 # gerando dict que vai ser inserido no excel
 
                 dict_relatorio_final[key_final] = {
-                    'Estabelecimento': valores['estabelecimento'],
+                    'Estabelecimento': 'PUCPR - CURITIBA',
                     'Escola': valores['escola'],
                     'CR Curso': str(valores['cr_curso'].split('.')[0]),
                     'Curso': valores['Curso'],
                     'Periodo': periodo,
                     'Sigla': valores['Agrupamento'],
                     'Tipo': valores['Tipo'],
                     'Turma Prime': f"{valores['Nome_Turma']}2023/1",
@@ -1104,16 +1072,15 @@
     worksheet.set_column('R:R', 20)
     worksheet.set_column('S:S', 20)
     worksheet.set_column('T:T', 45)
     worksheet.set_column('U:U', 42)
     worksheet.set_column('V:V', 20)
     worksheet.set_column('W:W', 42)
 
-    df_capacidade = pandas.read_excel(file_name_capacidade, sheet_name="BASE DE CAPACIDADES CWB", header=2,
-                                      usecols=range(5, 26))
+    df_capacidade = pandas.read_excel(file_name_capacidade, sheet_name="BASE DE CAPACIDADES CWB", header=2,usecols=range(5, 26))
 
     df_capacidade.to_excel(writer, index=False, sheet_name="Ambientes de Aprendizagem")
 
     df_horarios = pandas.DataFrame()
 
     df_horarios["NOME ESPAÇO ASC"] = df_capacidade["NOME ESPAÇO ASC"]
 
@@ -1206,52 +1173,51 @@
     elif diferenca < 5:
         valor = 'Próximo da capacidade'
     else:
         valor = 'Ok'
     return valor
 
 
-def main(arquivo_carga_horaria, arquivo_capacidade, arquivo_xml, file_name, caminho_auxiliar):
+def main(arquivo_carga_horaria, arquivo_capacidade, arquivo_xml, file_name):
     # pega somente o nome do arquivo para que o log seja salvo na mesma pasta
     utc_now = pytz.utc.localize(datetime.datetime.utcnow())
     dt_now = utc_now.astimezone(pytz.timezone("America/Sao_Paulo"))
-    f = open(f"{caminho_auxiliar}/Log/{str(dt_now.strftime('%y-%m-%d %H-%M'))}.txt", "w+", encoding="utf8")
+    f = open(f"./Arquivos_Auxiliares/Log/{str(dt_now.strftime('%y-%m-%d %H-%M'))}.txt", "w+", encoding="utf8")
 
     file_name_turma_disciplina = arquivo_carga_horaria
 
     file_name_asc_xml = arquivo_xml
 
     file_name_capacidade = arquivo_capacidade
     print('Carregando...')
 
-    with open(f'{caminho_auxiliar}/siglas.json', 'r', encoding="utf-8") as j:
+    with open('./Arquivos_Auxiliares/siglas.json', 'r', encoding="utf-8") as j:
         file_json_sigla = json.loads(j.read())
 
-    with open(f'{caminho_auxiliar}/turmasfic.json', 'r', encoding="utf-8") as j:
+    with open('./Arquivos_Auxiliares/turmasfic.json', 'r', encoding="utf-8") as j:
         file_json_turmasfic = json.loads(j.read())
 
-    with open(f'{caminho_auxiliar}/escolas.json', 'r', encoding="utf-8") as j:
+    with open('./Arquivos_Auxiliares/escolas.json', 'r', encoding="utf-8") as j:
         file_json_escolas = json.loads(j.read())
 
-    with open(f'{caminho_auxiliar}/tipos.json', 'r', encoding="utf-8") as j:
+    with open('./Arquivos_Auxiliares/tipos.json', 'r', encoding="utf-8") as j:
         file_json_tipos = json.loads(j.read())
 
     nome_arquivo = gerarRelatorio(file_name_turma_disciplina, file_name_asc_xml, file_json_sigla, file_name_capacidade,
                                   file_json_turmasfic, contador, file_json_escolas, file_json_tipos, f, file_name)
     return nome_arquivo
 
 
-def gerarExcel(file_carga_horaria, file_capacidade, file_xml, file_name, caminho_aux):
+def gerarExcel(file_carga_horaria, file_capacidade, file_xml, file_name):
     # le os valores vindo da tela
     arquivo_carga_horaria = file_carga_horaria
     arquivo_capacidade = file_capacidade
 
-    arquivo_xml = Unificar_XML.main(file_xml, caminho_aux)
-
-    nome_arquivo = main(arquivo_carga_horaria, arquivo_capacidade, arquivo_xml, file_name, caminho_aux)
+    arquivo_xml = Unificar_XML.main(file_xml)
 
-    Sugestao.main(nome_arquivo, arquivo_capacidade, caminho_aux)
+    nome_arquivo = main(arquivo_carga_horaria, arquivo_capacidade, arquivo_xml, file_name)
 
+    Sugestao.main(nome_arquivo, arquivo_capacidade)
 
 if __name__ == '__main__':
 
     gerarExcel()
```

### Comparing `Relatorio-Ensalamento-2.4.0/Sugestao/Sugestao.py` & `Relatorio_Ensalamento-2.4.1/Sugestao/Sugestao.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,34 +28,32 @@
         if capacidade_sala == 0:
             porcentagem_utilizacao = 0 - alunos_matriculados
         else:
             porcentagem_utilizacao = (alunos_matriculados / capacidade_sala) * 100
             porcentagem_utilizacao = round(porcentagem_utilizacao, 2)
 
         self.porcentagem_utilizacao = round(porcentagem_utilizacao, 2)
-class Subutilizada:
-    def __init__(self, sala, disciplina):
-        self.sala = sala
-        self.disciplina = disciplina
+
+
 class AmbienteDeAprendizagem:
-    def __init__(self, nome_sala, nome_sala_abrev, capacidade_sala, status, disciplina, tipo, tipo_detalhado, escola,curso):
+    def __init__(self, nome_sala, nome_sala_abrev, capacidade_sala, status, disciplina, tipo, tipo_detalhado, escola):
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
-        self.curso = curso
+
 
 def create_objects(file_name, dict_retorna_status_type, list, dict_retorna_utilizado_graduacao):
     df = pandas.read_excel(file_name, sheet_name='Completo')
     list_sem_status = []
     dict_retorna_escola = {}
 
     for data in df.iterrows():
@@ -68,15 +66,14 @@
         nome_sala = data[1]['Sala']
         nome_sala_abrev = data[1]['Sala Abreviação']
         capacidade_sala = data[1]['Capacidade da Sala']
         diferenca_capacidade = data[1]['Diferença Capacidade']
         analise_capacidade = data[1]['Análise Capacidade']
         df_sala = df.loc[df['Sala'] == nome_sala]
         escola = data[1]['Escola']
-        curso = data[1]['Curso']
         dia = data[1]['Dia da Semana']
 
         try:
             utilizado_graduacao = dict_retorna_utilizado_graduacao[nome_sala]
         except:
             utilizado_graduacao = "Sim"
 
@@ -115,18 +112,18 @@
             tipo_detalhado = dict_retorna_status_type[nome_sala][2]
         except:
             if nome_sala not in list_sem_status:
                 list_sem_status.append(nome_sala)
                 # print('Sem status pois, não encontrada na capacidade sala: ',nome_sala)
             status = 'Ativa'
             tipo = " "
-            tipo_detalhado = "Sala não esta planilha de infra."
+            tipo_detalhado = " "
 
         sala = AmbienteDeAprendizagem(nome_sala, nome_sala_abrev, capacidade_sala, status, list_objects_disciplinas,
-                                      tipo, tipo_detalhado, escola,curso)
+                                      tipo, tipo_detalhado, escola)
         dict_retorna_escola[nome_sala] = escola
         list.append(sala)
 
     return list, dict_retorna_escola
 
 
 def insert_matriz(list):
@@ -135,16 +132,16 @@
         return [["         "] * n_colunas for _ in range(n_linhas)]
 
     matriz = create_matriz(len(list), 140)
 
     row = 0
     for object in list:
         matriz[row][0] = object
-        if object.Disciplina != None:
-            for disciplina in object.Disciplina:
+        if object.Turma != None:
+            for disciplina in object.Turma:
                 list_aux = []
                 indice = get_indice(disciplina)
                 matriz[row][indice] = disciplina
         row += 1
 
     return matriz
 
@@ -168,54 +165,56 @@
         indice = 99
     elif dia == "FLUTUANTE":
         indice = 119
     else:
         print('erro em encontrar o dia no indice: ', dia)
         exit()
 
-    if hora_inicio == "07:50:00":
+    if hora_inicio == "07:05:00":
         indice += 1
-    elif hora_inicio == "08:35:00":
+    elif hora_inicio == "07:50:00":
         indice += 2
-    elif hora_inicio == "09:40:00":
+    elif hora_inicio == "08:35:00":
         indice += 3
-    elif hora_inicio == "10:25:00":
+    elif hora_inicio == "09:40:00":
         indice += 4
-    elif hora_inicio == "11:10:00":
+    elif hora_inicio == "10:25:00":
         indice += 5
-    elif hora_inicio == "11:55:00":
+    elif hora_inicio == "11:10:00":
         indice += 6
-    elif hora_inicio == "12:40:00":
+    elif hora_inicio == "11:55:00":
         indice += 7
-    elif hora_inicio == "13:25:00":
+    elif hora_inicio == "12:40:00":
         indice += 8
-    elif hora_inicio == "14:10:00":
+    elif hora_inicio == "13:25:00":
         indice += 9
-    elif hora_inicio == "15:15:00":
+    elif hora_inicio == "14:10:00":
         indice += 10
-    elif hora_inicio == "16:00:00":
+    elif hora_inicio == "15:15:00":
         indice += 11
-    elif hora_inicio == "16:45:00":
+    elif hora_inicio == "16:00:00":
         indice += 12
-    elif hora_inicio == "17:30:00":
+    elif hora_inicio == "16:45:00":
         indice += 13
-    elif hora_inicio == "18:15:00":
+    elif hora_inicio == "17:30:00":
         indice += 14
-    elif hora_inicio == "19:00:00":
+    elif hora_inicio == "18:15:00":
         indice += 15
-    elif hora_inicio == "19:45:00":
+    elif hora_inicio == "19:00:00":
         indice += 16
-    elif hora_inicio == "20:45:00":
+    elif hora_inicio == "19:45:00":
         indice += 17
-    elif hora_inicio == "21:30:00":
+    elif hora_inicio == "20:45:00":
         indice += 18
-    elif hora_inicio == "22:15:00":
+    elif hora_inicio == "21:30:00":
         indice += 19
-    elif hora_inicio == "--":
+    elif hora_inicio == "22:15:00":
         indice += 20
+    elif hora_inicio == "--":
+        indice += 21
     else:
         print('erro em encontrar o horário no indice: ', hora_inicio)
         exit()
 
     return indice
 
 
@@ -293,27 +292,25 @@
     salas_ativas = []
     list = []
     for sala in List_objects:
         salas_ativas.append(sala.nome_sala)
 
     df = pandas.read_excel(arquivo_capacidade, sheet_name="BASE DE CAPACIDADES CWB", header=2)
     for data in df.iterrows():
-
         nome_sala = data[1]['NOME ESPAÇO ASC']
         utilizado_graduacao = data[1]['UTILIZADO NA GRADUACAO']
 
         if utilizado_graduacao == "Não" or nome_sala.__contains__("AULA EXTERNA") is False:
             continue
 
         if nome_sala not in salas_ativas:
             nome_sala_abrev = data[1]['CÓD. ASC'].replace(' ', '')
             capacidade_sala = data[1]['CAPACIDADE']
             status = data[1]['STATUS']
             tipo = str(data[1]['TIPO DE INSTALAÇÃO'])
-
             tipo_detalhado = str(data[1]['TIPO DE INSTALAÇÃO DETALHADO'])
 
             try:
                 escola = dict_retorna_escola[nome_sala]
             except:
                 escola = ""
 
@@ -322,114 +319,56 @@
             sala = AmbienteDeAprendizagem(nome_sala, nome_sala_abrev, capacidade_sala, status, list_objects_disciplinas,
                                           tipo, tipo_detalhado, escola)
 
             list.append(sala)
     return list
 
 
-def insert_excel(nome_arquivo, dict_retorna_sugestao, dict_retorna_sugestao_list, dict_retorna_sugestao_subutilizada,dict_retona_status):
+def insert_excel(nome_arquivo, dict_retorna_sugestao, dict_retorna_sugestao_list, dict_retorna_sugestao_subutilizada):
     # key = nome da sala, nome da disciplina, dia, hora inicio
     def retorna_sugestao(nome_sala, nome_disciplina, dia, hora_inicio, analise, dict_retorna_sugestao):
         key = f"{nome_sala},{nome_disciplina},{dia},{hora_inicio}"
         key = key.upper()
         sala = ""
         if analise == 'Capacidade excedida' or analise == 'Sem Capacidade' \
                 or analise == 'Sala lotada' or analise == 'Sem sala':
             if key in dict_retorna_sugestao.keys():
                 sala = dict_retorna_sugestao[key]
                 sala = f"{sala.nome_sala} ({sala.capacidade_sala})"
-            else:
-                try:
-                    tipo_detalhado = dict_retona_status[nome_sala][2]
-                    if tipo_detalhado == "não especificado na planilha de infra.":
-                        sala = 'Não encontrado na planilha de infra.'
-                        return sala
-                    else:
-                        sala = f'Nenhum ambiente do tipo "{tipo_detalhado.lower()}" esta disponivel'
-                        return sala
-                except:
-                    sala = 'Não encontrado na planilha de infra.'
-                    return sala
         return sala
 
     def retorna_sugestao_sugestao_subutilizada(nome_sala, nome_disciplina, dia, hora_inicio, analise,
                                                dict_retorna_sugestao_subutilizada):
         key = f"{nome_sala},{nome_disciplina},{dia},{hora_inicio}"
         key = key.upper()
         sala = ""
         numero = 1
-        list_aux = []
-
         if analise == 'Capacidade excedida' or analise == 'Sem Capacidade' \
                 or analise == 'Sala lotada' or analise == 'Sem sala':
             if key in dict_retorna_sugestao_subutilizada.keys():
                 list_sala = dict_retorna_sugestao_subutilizada[key]
-
-                num = len(list_sala)
                 for sala_aux in list_sala:
-                    nome = sala_aux.sala.nome_sala
-                    capacidade = sala_aux.sala.capacidade_sala
-                    tipo = sala_aux.sala.tipo.lower()
-                    alunos_matriculados = sala_aux.disciplina.alunos_matriculados
-
-                    sala += f"{numero}. {nome} ({alunos_matriculados}/{capacidade}) | \n"
+                    sala += f"{numero}. {sala_aux.nome_sala} ({sala_aux.capacidade_sala}) | \n"
                     numero += 1
-
-                while numero <= 5:
-                    sala += f'{numero}. Nenhum ambiente do tipo "{tipo}" esta disponivel | \n'
-                    numero += 1
-            else:
-                try:
-                    tipo_detalhado = dict_retona_status[nome_sala][2]
-                    if tipo_detalhado == "não especificado na planilha de infra.":
-                        sala = 'Não encontrado na planilha de infra.'
-                        return sala
-
-                    sala = f'Nenhum ambiente do tipo "{tipo_detalhado.lower()}" esta disponivel'
-                    return sala
-                except:
-                    sala = 'Não encontrado na planilha de infra.'
-                    return sala
-
         sala = sala[:-1]
         return sala
 
     def retorna_sugestao_list(nome_sala, nome_disciplina, dia, hora_inicio, analise, dict_retorna_sugestao_list):
         key = f"{nome_sala},{nome_disciplina},{dia},{hora_inicio}"
         key = key.upper()
         sala = ""
         numero = 1
         if analise == 'Capacidade excedida' or analise == 'Sem Capacidade' \
                 or analise == 'Sala lotada' or analise == 'Sem sala':
             if key in dict_retorna_sugestao_list.keys():
                 list_sala = dict_retorna_sugestao_list[key]
                 for sala_aux in list_sala:
-                    nome = sala_aux.sala.nome_sala
-                    capacidade = sala_aux.sala.capacidade_sala
-                    tipo = sala_aux.sala.tipo.lower()
-
-                    sala += f"{numero}. {nome} ({capacidade}) | \n"
+                    sala += f"{numero}. {sala_aux.nome_sala} ({sala_aux.capacidade_sala}) | \n"
                     numero += 1
 
-                while numero <= 5:
-                    sala += f'{numero}. Nenhum ambiente do tipo "{tipo}" esta disponivel | \n'
-                    numero += 1
-            else:
-                try:
-                    tipo_detalhado = dict_retona_status[nome_sala][2]
-                    if tipo_detalhado == "não especificado na planilha de infra.":
-                        sala = 'Não encontrado na planilha de infra.'
-                        return sala
-
-                    sala = f'Nenhum ambiente do tipo "{tipo_detalhado.lower()}" esta disponivel'
-                    return sala
-                except:
-                    sala = 'Não encontrado na planilha de infra.'
-                    return sala
-
         sala = sala[:-1]
         return sala
 
     df = pandas.read_excel(nome_arquivo, sheet_name=None)
 
     df_completo = df['Completo']
 
@@ -739,26 +678,23 @@
     writer.close()
 
 
 def create_dict_status_type(arquivo_capacidade, dict_retorna_utilizado_graduacao):
     dict_retona_status = {}
 
     df = pandas.read_excel(arquivo_capacidade, sheet_name="BASE DE CAPACIDADES CWB", header=2)
-    df = df.fillna('')
     for data in df.iterrows():
         nome_sala = str(data[1]['NOME ESPAÇO ASC'])
         status = str(data[1]['STATUS'])
         tipo = str(data[1]['TIPO DE INSTALAÇÃO'])
         tipo_detalhado = str(data[1]['TIPO DE INSTALAÇÃO DETALHADO'])
         utilizado_graduacao = data[1]['UTILIZADO NA GRADUACAO']
 
         dict_retorna_utilizado_graduacao[nome_sala] = utilizado_graduacao
 
-        if tipo_detalhado == '':
-            tipo_detalhado = "Não especificado na planilha de infra."
         dict_retona_status[nome_sala] = status, tipo, tipo_detalhado
 
     return dict_retona_status, dict_retorna_utilizado_graduacao
 
 
 def analyze_matriz(matriz, df_capacidade_excedida, dict_retorna_status_type, dict_retorna_prioridade_escola):
     m = np.array(matriz)
@@ -908,18 +844,15 @@
                     and f"{classroom_name},{column}" not in repeated_classrooms and status == 'Ativa' \
                     and detailed_type == detailed_type_aux:
                 # não repetir sugestão
                 repeated_classrooms.append(f"{classroom_name},{column}")
                 list_aux.append(classroom)
                 dict_retorna_sugestao[key] = classroom
 
-
-
-
-        '''# todo 4 verificação
+        # todo 4 verificação
         # verificar o bloco atual e o tipo
         for classroom in list_empty_classroom:
 
             # atributos da sala sendo analisada
             capacidade_sala_aux = classroom.capacidade_sala
             bloco_aux = classroom.nome_sala.split('-')[0]
             type_aux = classroom.tipo
@@ -1041,24 +974,24 @@
             # verifica utilizando o bloco
             if capacidade_sala_aux > capacidade_esperada and key not in dict_retorna_sugestao.keys() \
                     and f"{classroom_name},{column}" not in repeated_classrooms and status == 'Ativa':
                 # não repetir sugestão
                 repeated_classrooms.append(f"{classroom_name},{column}")
                 list_aux.append(classroom)
                 dict_retorna_sugestao[key] = classroom
-'''
+
     return dict_retorna_sugestao
 
 
 def analyze_matriz_list(matriz, df_capacidade_excedida, dict_retorna_status_type, dict_retorna_prioridade_escola):
     m = np.array(matriz)
     row_number, column_number = m.shape
 
     dict_retorna_sugestao_lista = {}
-    disciplina={}
+
     for data in df_capacidade_excedida.iterrows():
         # não repetir sugestão na mesma lista de sugestões
         repeated_classrooms = []
 
         # lista de salas vazias
         list_empty_classroom = []
 
@@ -1081,15 +1014,14 @@
             detailed_type = dict_retorna_status_type[classroom_name][2]
         except:
             type = " "
             detailed_type = " "
 
         for row_aux in range(0, row_number):
             if matriz[row_aux][column] == "         ":
-                disciplina[matriz[row_aux][0]] = matriz[row_aux][column]
                 list_empty_classroom.append(matriz[row_aux][0])
 
         # ordenando em ordem crescente a lista
         list_empty_classroom = sorted(list_empty_classroom, key=lambda x: x.capacidade_sala)
 
         # armazenando lista de prioridades da escola
         try:
@@ -1123,16 +1055,15 @@
             if len(list_aux) >= 5:
                 break
 
             if capacidade_sala_aux > capacidade_esperada and bloco == bloco_aux and \
                     classroom.nome_sala not in repeated_classrooms \
                     and status == 'Ativa' and detailed_type == detailed_type_aux:
                 repeated_classrooms.append(classroom.nome_sala)
-                sala_subutilizada = Subutilizada(classroom,disciplina[classroom])
-                list_aux.append(sala_subutilizada)
+                list_aux.append(classroom)
                 dict_retorna_sugestao_lista[key] = list_aux
 
         # todo 2 verificação
         # veriricar o bloco prioridade da escola e o tipo detalhado
         for numero_bloco in list_blocos:
 
             if numero_bloco <= 9:
@@ -1161,17 +1092,17 @@
                 if len(list_aux) >= 5:
                     break
 
                 if capacidade_sala_aux > capacidade_esperada and bloco == bloco_aux and \
                         classroom.nome_sala not in repeated_classrooms \
                         and status == 'Ativa' and detailed_type == detailed_type_aux:
                     repeated_classrooms.append(classroom.nome_sala)
-                    sala_subutilizada = Subutilizada(classroom, disciplina[classroom])
-                    list_aux.append(sala_subutilizada)
+                    list_aux.append(classroom)
                     dict_retorna_sugestao_lista[key] = list_aux
+
         # todo 3 verificação
         # verificar o tipo detalhado
         for classroom in list_empty_classroom:
 
             # atributos da sala sendo analisada
             capacidade_sala_aux = classroom.capacidade_sala
             detailed_type_aux = classroom.tipo_detalhado
@@ -1190,19 +1121,18 @@
             if len(list_aux) >= 5:
                 break
 
             if capacidade_sala_aux > capacidade_esperada and \
                     classroom.nome_sala not in repeated_classrooms \
                     and status == 'Ativa' and detailed_type == detailed_type_aux:
                 repeated_classrooms.append(classroom.nome_sala)
-                sala_subutilizada = Subutilizada(classroom,disciplina[classroom])
-                list_aux.append(sala_subutilizada)
+                list_aux.append(classroom)
                 dict_retorna_sugestao_lista[key] = list_aux
 
-        '''# todo 4 verificação
+        # todo 4 verificação
         # verificar o bloco atual e o tipo
         for classroom in list_empty_classroom:
 
             # atributos da sala sendo analisada
             capacidade_sala_aux = classroom.capacidade_sala
             status = classroom.status
             type_aux = classroom.tipo
@@ -1319,15 +1249,15 @@
                 break
 
             if capacidade_sala_aux > capacidade_esperada and \
                     classroom.nome_sala not in repeated_classrooms \
                     and status == 'Ativa':
                 repeated_classrooms.append(classroom.nome_sala)
                 list_aux.append(classroom)
-                dict_retorna_sugestao_lista[key] = list_aux'''
+                dict_retorna_sugestao_lista[key] = list_aux
 
     return dict_retorna_sugestao_lista
 
 
 def analyze_matriz_subutilizada(matriz, df_capacidade_excedida, dict_retorna_status_type,
                                 dict_retorna_prioridade_escola):
     m = np.array(matriz)
@@ -1362,19 +1292,17 @@
             detailed_type = dict_retorna_status_type[classroom_name][2]
         except:
             type = " "
             detailed_type = " "
 
         # buscando as opções na matriz
         #      verificando se esta vazio e se sua capacidade atinge menos de 30%
-        disciplina = {}
         for row_aux in range(0, row_number):
             if matriz[row_aux][column] != "         " \
-                    and matriz[row_aux][column].porcentagem_utilizacao < 50:
-                disciplina[matriz[row_aux][0]] = matriz[row_aux][column]
+                    and matriz[row_aux][column].porcentagem_utilizacao < 45:
                 list_underused_classroom.append(matriz[row_aux][0])
 
         # lista que vai ser inserida como sugestão
         list_aux = []
 
         # ordenando em ordem crescente a lista
         list_underused_classroom = sorted(list_underused_classroom, key=lambda x: x.capacidade_sala)
@@ -1391,18 +1319,14 @@
 
             # atributos da sala sendo analisada
             capacidade_sala_aux = classroom.capacidade_sala
             bloco_aux = classroom.nome_sala.split('-')[0]
             detailed_type_aux = classroom.tipo_detalhado
             status = classroom.status
 
-            #ignorando salas sem tipo detalhado definido
-            if detailed_type_aux == "Não especificado na planilha de infra." or detailed_type_aux == "Sala não esta planilha de infra.":
-                continue
-
             # verificando se é um numero valido
             try:
                 int(capacidade_sala_aux)
             except:
                 continue
 
             # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
@@ -1412,19 +1336,15 @@
             if len(list_aux) >= 5:
                 break
 
             if capacidade_sala_aux > capacidade_esperada and bloco == bloco_aux and \
                     classroom.nome_sala not in repeated_classrooms \
                     and status == 'Ativa' and detailed_type == detailed_type_aux:
                 repeated_classrooms.append(classroom.nome_sala)
-
-                valor = f"{classroom.nome_sala},{classroom.capacidade_sala},{disciplina[classroom].alunos_matriculados},{type}"
-
-                sala_subutilizada = Subutilizada(classroom,disciplina[classroom])
-                list_aux.append(sala_subutilizada)
+                list_aux.append(classroom)
                 dict_retorna_sugestao_subutilizada[key] = list_aux
 
         # todo 2 verificação
         # verificando o bloco prioridade da escola e o tipo detalhado
         for numero_bloco in list_blocos:
 
             if numero_bloco <= 9:
@@ -1437,18 +1357,111 @@
 
                 # atributos da sala sendo analisada
                 capacidade_sala_aux = classroom.capacidade_sala
                 bloco_aux = classroom.nome_sala.split('-')[0]
                 detailed_type_aux = classroom.tipo_detalhado
                 status = classroom.status
 
-                # ignorando salas sem tipo detalhado definido
-                if detailed_type_aux == "Não especificado na planilha de infra." or detailed_type_aux == "Sala não esta planilha de infra.":
+                # verificando se é um numero valido
+                try:
+                    int(capacidade_sala_aux)
+                except:
                     continue
 
+                # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
+                key = f"{classroom_name},{subject_name},{day},{start_hour}"
+                key = key.upper()
+
+                if len(list_aux) >= 5:
+                    break
+
+                if capacidade_sala_aux > capacidade_esperada and bloco == bloco_aux and \
+                        classroom.nome_sala not in repeated_classrooms \
+                        and status == 'Ativa' and detailed_type == detailed_type_aux:
+                    repeated_classrooms.append(classroom.nome_sala)
+                    list_aux.append(classroom)
+                    dict_retorna_sugestao_subutilizada[key] = list_aux
+
+        # todo 3 verificação
+        # verificando o tipo detalhado
+        for classroom in list_underused_classroom:
+
+            # atributos da sala sendo analisada
+            capacidade_sala_aux = classroom.capacidade_sala
+            detailed_type_aux = classroom.tipo_detalhado
+            status = classroom.status
+
+            # verificando se é um numero valido
+            try:
+                int(capacidade_sala_aux)
+            except:
+                continue
+
+            # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
+            key = f"{classroom_name},{subject_name},{day},{start_hour}"
+            key = key.upper()
+
+            if len(list_aux) >= 5:
+                break
+
+            if capacidade_sala_aux > capacidade_esperada and \
+                    classroom.nome_sala not in repeated_classrooms \
+                    and status == 'Ativa' and detailed_type == detailed_type_aux:
+                repeated_classrooms.append(classroom.nome_sala)
+                list_aux.append(classroom)
+                dict_retorna_sugestao_subutilizada[key] = list_aux
+
+        # todo 4 verificação
+        # verificando o bloco atual e o tipo
+        for classroom in list_underused_classroom:
+
+            # atributos da sala sendo analisada
+            capacidade_sala_aux = classroom.capacidade_sala
+            bloco_aux = classroom.nome_sala.split('-')[0]
+            type_aux = classroom.tipo
+            status = classroom.status
+
+            # verificando se é um numero valido
+            try:
+                int(capacidade_sala_aux)
+            except:
+                continue
+
+            # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
+            key = f"{classroom_name},{subject_name},{day},{start_hour}"
+            key = key.upper()
+
+            if len(list_aux) >= 5:
+                break
+
+            if capacidade_sala_aux > capacidade_esperada and bloco == bloco_aux and \
+                    classroom.nome_sala not in repeated_classrooms \
+                    and status == 'Ativa' and type == type_aux:
+                repeated_classrooms.append(classroom.nome_sala)
+                list_aux.append(classroom)
+                dict_retorna_sugestao_subutilizada[key] = list_aux
+
+        # todo 5 verificação
+        # verificando o bloco prioridade da escola e o tipo
+        for numero_bloco in list_blocos:
+
+            if numero_bloco <= 9:
+                bloco = f"Bloco 0{numero_bloco} "
+            else:
+                bloco = f"Bloco {numero_bloco} "
+
+            # utilizando o bloco para validar
+            for classroom in list_underused_classroom:
+
+                # atributos da sala sendo analisada
+                capacidade_sala_aux = classroom.capacidade_sala
+                bloco_aux = classroom.nome_sala.split('-')[0]
+                type_aux = classroom.tipo
+                status = classroom.status
+
                 # verificando se é um numero valido
                 try:
                     int(capacidade_sala_aux)
                 except:
                     continue
 
                 # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
@@ -1456,20 +1469,90 @@
                 key = key.upper()
 
                 if len(list_aux) >= 5:
                     break
 
                 if capacidade_sala_aux > capacidade_esperada and bloco == bloco_aux and \
                         classroom.nome_sala not in repeated_classrooms \
-                        and status == 'Ativa' and detailed_type == detailed_type_aux:
+                        and status == 'Ativa' and type == type_aux:
+                    repeated_classrooms.append(classroom.nome_sala)
+                    list_aux.append(classroom)
+                    dict_retorna_sugestao_subutilizada[key] = list_aux
+
+        # todo 6 verificação
+        # verificando o tipo
+        for numero_bloco in list_blocos:
+
+            if numero_bloco <= 9:
+                bloco = f"Bloco 0{numero_bloco} "
+            else:
+                bloco = f"Bloco {numero_bloco} "
+
+            # utilizando o bloco para validar
+            for classroom in list_underused_classroom:
+
+                # atributos da sala sendo analisada
+                capacidade_sala_aux = classroom.capacidade_sala
+                type_aux = classroom.tipo
+                status = classroom.status
+
+                # verificando se é um numero valido
+                try:
+                    int(capacidade_sala_aux)
+                except:
+                    continue
+
+                # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
+                key = f"{classroom_name},{subject_name},{day},{start_hour}"
+                key = key.upper()
+
+                if len(list_aux) >= 5:
+                    break
+
+                if capacidade_sala_aux > capacidade_esperada and \
+                        classroom.nome_sala not in repeated_classrooms \
+                        and status == 'Ativa' and type == type_aux:
                     repeated_classrooms.append(classroom.nome_sala)
+                    list_aux.append(classroom)
+                    dict_retorna_sugestao_subutilizada[key] = list_aux
 
-                    valor = f"{classroom.nome_sala},{classroom.capacidade_sala},{disciplina[classroom].alunos_matriculados},{type}"
-                    sala_subutilizada = Subutilizada(classroom, disciplina[classroom])
-                    list_aux.append(sala_subutilizada)
+        # todo 7 verificação
+        # sem verificação
+        for numero_bloco in list_blocos:
+
+            if numero_bloco <= 9:
+                bloco = f"Bloco 0{numero_bloco} "
+            else:
+                bloco = f"Bloco {numero_bloco} "
+
+            # utilizando o bloco para validar
+            for classroom in list_underused_classroom:
+
+                # atributos da sala sendo analisada
+                capacidade_sala_aux = classroom.capacidade_sala
+                status = classroom.status
+
+                # verificando se é um numero valido
+                try:
+                    int(capacidade_sala_aux)
+                except:
+                    continue
+
+                # key = nome da sala, nome da disciplina, dia, hora inicio, divisao
+                key = f"{classroom_name},{subject_name},{day},{start_hour}"
+                key = key.upper()
+
+                if len(list_aux) >= 5:
+                    break
+
+                if capacidade_sala_aux > capacidade_esperada and \
+                        classroom.nome_sala not in repeated_classrooms \
+                        and status == 'Ativa':
+                    repeated_classrooms.append(classroom.nome_sala)
+                    list_aux.append(classroom)
                     dict_retorna_sugestao_subutilizada[key] = list_aux
 
     return dict_retorna_sugestao_subutilizada
 
 
 def create_dict_prioridade_escola(caminho_aux):
     df_prioridades = pandas.read_excel(f'{caminho_aux}/Prioridade_escolas.xlsx')
@@ -1494,15 +1577,15 @@
     # dicts
     dict_retorna_sugestao = {}
     dict_retorna_sugestao_subutilizada = {}
     dict_retorna_sugestao_list = {}
     dict_retorna_escola = {}
     dict_retorna_prioridade_escola = {}
     dict_retorna_utilizado_graduacao = {}
-    print('carregando excel...')
+
     # lista dos objetos
     list_objects = []
 
     # dict utioizado para retornar o status da planilha de capacidade
     dict_retorna_status_type, dict_retorna_utilizado_graduacao = create_dict_status_type(arquivo_capacidade,
                                                                                          dict_retorna_utilizado_graduacao)
 
@@ -1539,18 +1622,12 @@
 
     # retorna um top 5 de sugestões, repetindo sugestão se necessario
     print('Criando lista de sugestões...')
     dict_retorna_sugestao_list = analyze_matriz_list(matriz, df_problemas, dict_retorna_status_type,
                                                      dict_retorna_prioridade_escola)
 
     print('Inserindo no excel...')
-    insert_excel(nome_arquivo, dict_retorna_sugestao, dict_retorna_sugestao_list, dict_retorna_sugestao_subutilizada,dict_retorna_status_type)
+    insert_excel(nome_arquivo, dict_retorna_sugestao, dict_retorna_sugestao_list, dict_retorna_sugestao_subutilizada)
     print("Arquivo gerado com sucesso.")
 
 if __name__ == '__main__':
-
-
-    '''    nome_arq = "C:/Users\m.rosa1\Downloads\Relatorio_Ensalamento_s.xlsx"
-    arq_cap = "C:/Users\m.rosa1\Downloads\Relatório dos Espaços de Ensino_Novo Layout_20230108 (1) (2).xlsx"
-    a = 'C:/Users\m.rosa1\Documents\Git\codigos\Relatorio_Ensalamento\Arquivos_Auxiliares'''
-
     main()
```

### Comparing `Relatorio-Ensalamento-2.4.0/Unificar_XML/Unificar_XML.py` & `Relatorio_Ensalamento-2.4.1/Unificar_XML/Unificar_XML.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,29 +54,15 @@
                            endtime="21:30")
     ElementTree.SubElement(periods, "period", name="21:30", short="21:30", period="19", starttime="21:30",
                            endtime="22:15")
     ElementTree.SubElement(periods, "period", name="22:15", short="22:15", period="20", starttime="22:15",
                            endtime="23:00")
 
     # tag daysdef
-    daysdefs = ElementTree.SubElement(root_unificado, "daysdefs", columns="id,days,name,short")
-    ElementTree.SubElement(daysdefs, "daysdef", id="6B3F12A34D97076A", name="Qualquer dia", short="X",
-                           days="1000000,0100000,0010000,0001000,0000100,0000010,0000001")
-    ElementTree.SubElement(daysdefs, "daysdef", id="805BDEBDA010C1F2", name="Cada dia", short="E", days="1111111")
-    ElementTree.SubElement(daysdefs, "daysdef", id="A8F237B2F9E6B675", name="Segunda-feira ", short="Seg",
-                           days="1000000")
-    ElementTree.SubElement(daysdefs, "daysdef", id="CAB97D0425BEC0DA", name="Terça-feira", short="Ter", days="0100000")
-    ElementTree.SubElement(daysdefs, "daysdef", id="60850D9314471122", name="Quarta-feira ", short="Qua",
-                           days="0010000")
-    ElementTree.SubElement(daysdefs, "daysdef", id="DDF4362F91A753AB", name="Quinta-feira ", short="Qui",
-                           days="0001000")
-    ElementTree.SubElement(daysdefs, "daysdef", id="E87DBCE4E7616290", name="Sexta-feira ", short="Sex", days="0000100")
-    ElementTree.SubElement(daysdefs, "daysdef", id="23651B657C8E30B9", name="Sábado ", short="Sáb", days="0000010")
-    ElementTree.SubElement(daysdefs, "daysdef", id="0E5CEC8F57D233C2", name="Horário Flutuante", short="Flutuante",
-                           days="0000001")
+    ElementTree.SubElement(root_unificado, "daysdefs", columns="id,days,name,short")
 
     # tag weeksdef
     weeksdefs = ElementTree.SubElement(root_unificado, "weekdefs", options="canadd,export:silent",
                                        columns="id,weeks,name,short")
     ElementTree.SubElement(weeksdefs, "weekdef", id="4D751412E50EC8F8", name="Todas as semanas", short="Todas",
                            weeks="1")
 
@@ -129,15 +115,25 @@
     # tag cards
     ElementTree.SubElement(root_unificado, "cards", options="canadd,export:silent",
                            columns="lessonid,period,days,weeks,terms,classroomids")
 
     return root_unificado
 
 
-def unifica_xml(root_unificado, root):
+def unifica_xml(root_unificado, root, contagem):
+    if contagem == 0:
+        for day in root.iter("daysdef"):
+            for child in root_unificado:
+                tag = child.tag
+                if tag == "daysdefs":
+                    ElementTree.SubElement(child, "daysdef", id=day.get("id"), name=str(day.get("name")),
+                                           short=day.get("short")
+                                           , days=day.get("days"))
+
+    contagem += 1
     # tag subjects
     # subjects = ElementTree.Element(root_unificado, "subject")
     for sub in root.iter("subject"):
         for child in root_unificado:
             tag = child.tag
             if tag == "subjects":
                 ElementTree.SubElement(child, "subject", id=sub.get("id"), name=str(sub.get("name")),
@@ -216,15 +212,15 @@
             if tag == "cards":
                 ElementTree.SubElement(child, "card", lessonid=car.get("lessonid"),
                                        classroomids=car.get("classroomids"),
                                        period=car.get("period"),
                                        terms=car.get("terms"),
                                        days=car.get("days"))
 
-    return root_unificado
+    return root_unificado, contagem
 
 
 def corrige_caracteres_especiais(file_name):
     # Substitui o símbolo que causa erro
     # file_data = file_name.replace("&quot;", "").replace('& amp;','').replace(" &amp; ", "").replace(" ", "")
     file_data = file_name
     return file_data
@@ -296,41 +292,41 @@
     for group in root.find("groups").findall("group"):
         if group.get("id") not in active_groups:
             root.find("groups").remove(group)
 
     return root
 
 
-def main(caminho_pasta, caminho_aux):
+def main(caminho_pasta):
     utc_now = pytz.utc.localize(datetime.datetime.utcnow())
     dt_now = utc_now.astimezone(pytz.timezone("America/Sao_Paulo"))
     pasta_raiz = caminho_pasta
 
     root_unificado = cria_unificado()
     tree = ""
+    contagem = 0
     # Para cada diretório dentro do diretório raiz
     for dirpath, dirnames, filenames in os.walk(pasta_raiz):
         # dirpath =  caminho
 
         for file in filenames:
             file = file.upper()
-            if not file.__contains__("XML"):
+            if not file.__contains__(".XML"):
                 continue
 
             # criando o xml que vai passar os dados
-            file_name_xml = f"{dirpath}\\{file}"
+            file_name_xml = dirpath + "/" + file
             tree_xml = ElementTree.parse(file_name_xml)
             root = tree_xml.getroot()
             # unificando
-            tree = unifica_xml(root_unificado, root)
+            tree, contagem = unifica_xml(root_unificado, root, contagem)
 
-        tree_sem_flutuantes = retira_flutuantes(tree)
+        # tree_sem_flutuantes = retira_flutuantes(tree)
 
-        xml_string_sem_flutuantes = minidom.parseString(
-            ElementTree.tostring(tree_sem_flutuantes, encoding="windows-1252")).toprettyxml(indent="   ")
+        # xml_string_sem_flutuantes = minidom.parseString(ElementTree.tostring(tree_sem_flutuantes, encoding="windows-1252")).toprettyxml(indent="   ")
         xml_string = minidom.parseString(ElementTree.tostring(tree, encoding="windows-1252")).toprettyxml(indent="   ")
 
         # forçar a mudança do enconding
         # contar quantas vezes o ? se repete para que na segunda vez sobreescreva o enconding correto
         posicao = 0
         contagem = 0
         lista = list(xml_string)
@@ -344,26 +340,26 @@
             posicao += 1
         xml_string = "".join(lista)
 
         # forçar a mudança do enconding
         # contar quantas vezes o ? se repete para que na segunda vez sobreescreva o enconding correto
         posicao = 0
         contagem = 0
-        lista = list(xml_string_sem_flutuantes)
-        for i in xml_string_sem_flutuantes:
+        # lista = list(xml_string_sem_flutuantes)
+        '''for i in xml_string_sem_flutuantes:
             if i == "?":
                 contagem += 1
             if contagem == 2:
                 contagem = 3
                 lista[posicao] = "encoding='windows-1252'?"
 
             posicao += 1
-        xml_string_sem_flutuantes = "".join(lista)
+        xml_string_sem_flutuantes = "".join(lista)'''
 
-        name = f"{caminho_aux}/XML/XML_unificado_{str(dt_now.strftime('%y-%m-%d %H-%M'))}.xml"
+        name = f"./Arquivos_Auxiliares/XML/XML_unificado_{str(dt_now.strftime('%y-%m-%d %H-%M'))}.xml"
         with open(name, "w", encoding="windows-1252") as f:
             xml_string = corrige_caracteres_especiais(xml_string)
             f.write(xml_string)
 
         return name
```

