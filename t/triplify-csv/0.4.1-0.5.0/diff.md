# Comparing `tmp/triplify_csv-0.4.1.tar.gz` & `tmp/triplify_csv-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triplify_csv-0.4.1.tar", max compression
+gzip compressed data, was "triplify_csv-0.5.0.tar", max compression
```

## Comparing `triplify_csv-0.4.1.tar` & `triplify_csv-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1526 2023-05-28 12:11:08.656135 triplify_csv-0.4.1/LICENSE
--rw-r--r--   0        0        0     7905 2023-05-28 12:11:08.658135 triplify_csv-0.4.1/README.md
--rw-r--r--   0        0        0      585 2023-05-28 12:19:10.176120 triplify_csv-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-28 12:11:08.739135 triplify_csv-0.4.1/triplify_csv/__init__.py
--rwxr-xr-x   0        0        0    18065 2023-05-28 12:11:08.745135 triplify_csv-0.4.1/triplify_csv/triplify_csv.py
--rw-r--r--   0        0        0     8734 1970-01-01 00:00:00.000000 triplify_csv-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-07-03 17:07:53.114156 triplify_csv-0.5.0/LICENSE
+-rw-r--r--   0        0        0     8007 2023-07-14 16:02:34.486997 triplify_csv-0.5.0/README.md
+-rw-r--r--   0        0        0      585 2023-07-07 16:01:20.910360 triplify_csv-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-03 17:07:53.205155 triplify_csv-0.5.0/triplify_csv/__init__.py
+-rwxr-xr-x   0        0        0    18764 2023-07-06 07:31:04.719065 triplify_csv-0.5.0/triplify_csv/triplify_csv.py
+-rw-r--r--   0        0        0     8836 1970-01-01 00:00:00.000000 triplify_csv-0.5.0/PKG-INFO
```

### Comparing `triplify_csv-0.4.1/LICENSE` & `triplify_csv-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `triplify_csv-0.4.1/README.md` & `triplify_csv-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 
 The configuration file contains a set of mappings for triplify\_csv to follow to set the subjects, predicates and objects or literal values of your triples or nquads from the data in one or more CSV files. These mappings are RDF triples in the turtle syntax. The terms that can be used are a subset of the terms defined in the R2RML standard.
 
 R2RML was not designed for this purpose. R2RML is '.. a language for expressing customized mappings from relational databases to RDF datasets.' (see [https://www.w3.org/TR/r2rml/](https://www.w3.org/TR/r2rml/) ). Triplify\_csv uses a subset of R2RML to express customised mappings from CSV files to RDF datasets. Where R2RML refers to the tables of a database using 'rr:logicalTable' this should be understood in the triplify\_csv use of R2RML as referring to the name (without '.csv') of a corresponding csv file. 'rr:sqlQuery', the term of the R2RML language that lets you express mappings from database queries to RDF isn't supported in the triplify\_csv usage. Also, there is no need to support 'rr:sqlVersion'.
 
 For a complete list of what parts of the R2RML language are supported see the examples in the /tests folder and refer to the R2RML test cases document ([https://www.w3.org/TR/rdb2rdf-test-cases/](https://www.w3.org/TR/rdb2rdf-test-cases/)). As of version 0.3.0 the test cases supported are
 
+- R2RMLTC0003c - Using 'rr:template' within objectmaps to build up string literals for object values
 - R2RMLTC0007a - Typing resources by relying on rdf:type predicate
 - R2RMLTC0007b - Assigning triples to Named Graphs
 - R2RMLTC0007c - One column mapping, using rr:class
 - R2RMLTC0007d - One column mapping, specifying an rr:predicateObjectMap with rdf:type
 - R2RMLTC0007e - One column mapping, using rr:graphMap and rr:class
 - R2RMLTC0007f - One column mapping, using rr:graphMap and specifying an rr:predicateObjectMap with rdf:type
 - R2RMLTC0007g - Assigning triples to the default graph
@@ -165,8 +166,8 @@
 
 If you wanted this serialised to json-ld format instead you could use the following command ...
 
 ```
 triplify_csv -m 'contactsmap.ttl' -c 'Contacts.csv' -o 'contactstriples.json' -f 'json-ld'
 ```
 
- triplify_csv uses rdflib and can output to all the serialisation formats that [rdflib](https://pypi.org/project/rdflib/) provides. (See also 'format' [here](https://rdflib.readthedocs.io/en/stable/apidocs/rdflib.html#rdflib.Graph.serialize))
+ triplify_csv uses rdflib and can output to all the serialisation formats that [rdflib](https://pypi.org/project/rdflib/) provides. (See also 'format' [here](https://rdflib.readthedocs.io/en/stable/apidocs/rdflib.html#rdflib.Graph.serialize))
```

### Comparing `triplify_csv-0.4.1/pyproject.toml` & `triplify_csv-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "triplify_csv"
-version = "0.4.1"
+version = "0.5.0"
 description = "A tool to generate triples from CSV files according to a configuration file."
 authors = ["Adrian Atley"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/AAtley/triplify_csv"
 
 [tool.poetry.dependencies]
```

### Comparing `triplify_csv-0.4.1/triplify_csv/triplify_csv.py` & `triplify_csv-0.5.0/triplify_csv/triplify_csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -361,16 +361,14 @@
 								pom_column = pom[rr('objectMap')][rr('column')]
 								if rr('language') in pom[rr('objectMap')]:
 									literal_lang = pom[rr('objectMap')][rr('language')]
 								else:
 									if rr('datatype') in pom[rr('objectMap')]:
 										lit_datatype = pom[rr('objectMap')][rr('datatype')]
 										
-										
-								
 							# if objectmap in pom and key of this om is also in tmap then it is a refobjmap
 							if rr('objectMap') in pom and str(pom[rr('objectMap')]) in tmaps.keys() and rr('parentTriplesMap') in tmaps[str(pom[rr('objectMap')])] and tmaps[str(pom[rr('objectMap')])][rr('parentTriplesMap')] in tmaps.keys():
 								rom = pom[rr('objectMap')]
 								
 								ptm = tmaps[rom][rr('parentTriplesMap')]
 								ptmSubjectTemplate = tmaps[ptm][rr('subjectMap')][rr('template')]
 								object = URIRef(self.get_Uri_From_Template(ptmSubjectTemplate,row))
@@ -404,18 +402,40 @@
 												if fkrow[parent] ==  childval:
 													record = fkrow
 											# get uri from fk csv's template and fk row
 											ptmSubjectTemplate = tmaps[ptm][rr('subjectMap')][rr('template')]
 											
 											object = URIRef(self.get_Uri_From_Template(ptmSubjectTemplate,record))
 							
+							# R2RMLTC0003c
+							elif rr('objectMap') in pom and rr('template') in pom[rr('objectMap')]:
+								ocols = []
+								objmap_template = pom[rr('objectMap')][rr('template')]
+								for match in re.finditer(r'{"([^>]+?)"}',objmap_template):
+									ocols.append(match.group(0).strip('{}"'))
+								
+								
+								
+								if set(ocols).issubset(csvinfo.columnNames):
+									
+									o = re.sub('[{"}]','',objmap_template)
+									for ocol in ocols:			
+										o = o.replace(ocol,urllib.parse.quote(str(row[ocol])))
+										
+									#object = URIRef(o)
+									object = self.get_literal(o)
+									
+									print('object is ' + object)
+								
 							elif len(pom_column) > 0 and pom_column in row.keys():
+								print('in elif')
 								
 								object = self.get_literal(row[pom_column],csvinfo.options.dateformat, literal_lang, lit_datatype)
 							else:
+								print('in else')
 								object = URIRef(pom_object)
 	
 							# add to Dataset for quads if non-default graph else add just add triple
 							if making_quads:
 								gc = self.triples.graph(URIRef(context))
 								self.triples.add((subject, predicate, object, gc))
 								
@@ -510,8 +530,7 @@
 	    raise
 	for e in s.errors:
 		print(e)
 		
 	
 if __name__ == "__main__":
 	process()
-
```

### Comparing `triplify_csv-0.4.1/PKG-INFO` & `triplify_csv-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triplify-csv
-Version: 0.4.1
+Version: 0.5.0
 Summary: A tool to generate triples from CSV files according to a configuration file.
 Home-page: https://github.com/AAtley/triplify_csv
 License: BSD-3-Clause
 Author: Adrian Atley
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -92,14 +92,15 @@
 
 The configuration file contains a set of mappings for triplify\_csv to follow to set the subjects, predicates and objects or literal values of your triples or nquads from the data in one or more CSV files. These mappings are RDF triples in the turtle syntax. The terms that can be used are a subset of the terms defined in the R2RML standard.
 
 R2RML was not designed for this purpose. R2RML is '.. a language for expressing customized mappings from relational databases to RDF datasets.' (see [https://www.w3.org/TR/r2rml/](https://www.w3.org/TR/r2rml/) ). Triplify\_csv uses a subset of R2RML to express customised mappings from CSV files to RDF datasets. Where R2RML refers to the tables of a database using 'rr:logicalTable' this should be understood in the triplify\_csv use of R2RML as referring to the name (without '.csv') of a corresponding csv file. 'rr:sqlQuery', the term of the R2RML language that lets you express mappings from database queries to RDF isn't supported in the triplify\_csv usage. Also, there is no need to support 'rr:sqlVersion'.
 
 For a complete list of what parts of the R2RML language are supported see the examples in the /tests folder and refer to the R2RML test cases document ([https://www.w3.org/TR/rdb2rdf-test-cases/](https://www.w3.org/TR/rdb2rdf-test-cases/)). As of version 0.3.0 the test cases supported are
 
+- R2RMLTC0003c - Using 'rr:template' within objectmaps to build up string literals for object values
 - R2RMLTC0007a - Typing resources by relying on rdf:type predicate
 - R2RMLTC0007b - Assigning triples to Named Graphs
 - R2RMLTC0007c - One column mapping, using rr:class
 - R2RMLTC0007d - One column mapping, specifying an rr:predicateObjectMap with rdf:type
 - R2RMLTC0007e - One column mapping, using rr:graphMap and rr:class
 - R2RMLTC0007f - One column mapping, using rr:graphMap and specifying an rr:predicateObjectMap with rdf:type
 - R2RMLTC0007g - Assigning triples to the default graph
@@ -187,7 +188,8 @@
 If you wanted this serialised to json-ld format instead you could use the following command ...
 
 ```
 triplify_csv -m 'contactsmap.ttl' -c 'Contacts.csv' -o 'contactstriples.json' -f 'json-ld'
 ```
 
  triplify_csv uses rdflib and can output to all the serialisation formats that [rdflib](https://pypi.org/project/rdflib/) provides. (See also 'format' [here](https://rdflib.readthedocs.io/en/stable/apidocs/rdflib.html#rdflib.Graph.serialize))
+
```

