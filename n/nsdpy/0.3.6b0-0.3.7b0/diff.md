# Comparing `tmp/nsdpy-0.3.6b0.tar.gz` & `tmp/nsdpy-0.3.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdpy-0.3.6b0.tar", max compression
+gzip compressed data, was "nsdpy-0.3.7b0.tar", max compression
```

## Comparing `nsdpy-0.3.6b0.tar` & `nsdpy-0.3.7b0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-05-29 18:26:14.471852 nsdpy-0.3.6b0/LICENSE
--rw-r--r--   0        0        0     2720 2023-05-29 18:26:14.472080 nsdpy-0.3.6b0/README.md
--rw-r--r--   0        0        0    37320 2023-06-17 14:13:34.144899 nsdpy-0.3.6b0/functions.py
--rw-r--r--   0        0        0    13273 2023-06-17 14:15:00.690285 nsdpy-0.3.6b0/nsdpy.py
--rw-r--r--   0        0        0      841 2023-06-17 14:15:20.968769 nsdpy-0.3.6b0/pyproject.toml
--rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 nsdpy-0.3.6b0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-29 18:26:14.471852 nsdpy-0.3.7b0/LICENSE
+-rw-r--r--   0        0        0     2720 2023-06-24 11:46:18.810797 nsdpy-0.3.7b0/README.md
+-rw-r--r--   0        0        0    37996 2023-07-14 13:21:20.856554 nsdpy-0.3.7b0/functions.py
+-rw-r--r--   0        0        0    13280 2023-07-14 13:25:44.554297 nsdpy-0.3.7b0/nsdpy.py
+-rw-r--r--   0        0        0      841 2023-07-14 13:25:44.367772 nsdpy-0.3.7b0/pyproject.toml
+-rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 nsdpy-0.3.7b0/PKG-INFO
```

### Comparing `nsdpy-0.3.6b0/LICENSE` & `nsdpy-0.3.7b0/LICENSE`

 * *Files identical despite different names*

### Comparing `nsdpy-0.3.6b0/README.md` & `nsdpy-0.3.7b0/README.md`

 * *Files identical despite different names*

### Comparing `nsdpy-0.3.6b0/functions.py` & `nsdpy-0.3.7b0/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 def download(parameters, address):
     """ 
     Sends requests to the API until getting a result
     
     INPUTS: download(parameters, address)
         parameters: DICT, parameters of the get request to the API
-        Address: STRING, API bas URL
+        Address: STRING, API base URL
 
     OUTPUT: object, <class 'requests.models.Response'>
         if an exceptions.HTTPError is triggered: returns 1
     """ 
     connect = 0
     while True:
         try:
@@ -161,14 +161,19 @@
         for line in f:
             if len(line.split('<DocSum>')) > 1:
                 taxid = ''
                 seqnb = ''
             else:
                 try:
                     version = line.split('<Item Name="AccessionVersion" Type="String">', 1)[1]
+                    ''' 
+                        AccessionVersion is made of accession number plus versions number. 
+                        Accession numbers pattern: [alphabetical prefix][series of digits]
+                        see: https://www.ncbi.nlm.nih.gov/books/NBK470040/#:~:text=The%20accession%20number%20is%20a,the%20accession%20munumber%2C%20an%20Accession.
+                    '''
                     seqnb = version.split("<")[0].strip()
                 except IndexError:
                     pass
 
                 TaxId = line.split('<Item Name="TaxId" Type="Integer">', 1)
                 if len(TaxId) > 1:
                     taxid = TaxId[1].split("<")[0].strip()
@@ -282,14 +287,15 @@
         result = download(parameters, EFETCH_URL)
 
         # comments
         if verb > 1:
             print(f'{round((int(retstart)/count)*100, 1)} % of the taxonomy found')
 
         ## analyse the results from efetch
+        # split batch results string in single results array
         result = result.text.split('</Taxon>\n<Taxon>')
 
         for seq in result:
             dicttemp = {}
             try:
                 TaxId, _ = seq.split('</TaxId>', 1)
                 _, TaxId = TaxId.split('<TaxId>', 1)
@@ -984,41 +990,47 @@
         xml: string
     OUTPUTS:
         classif: dict
 """
 def parseClassifXML(xml):
     classif = {}
 
+# parse the name before lineageex as well 
     if "</ScientificName>" in xml and "<ScientificName>" in xml:
-        scientificName, newXml = xml.split('</ScientificName>', 1)
+        scientificName, _ = xml.split('</ScientificName>', 1)
         _, scientificName = scientificName.split('<ScientificName>', 1)
         classif['ScientificName'] = scientificName
 
     if "</LineageEx>" in xml and "<LineageEx>" in xml:
-        lineageInfo, _ = xml.split("</LineageEx>", 1)
-        _, lineageInfo = lineageInfo.split("<LineageEx>", 1)
-        taxons = lineageInfo.split("</Taxon>")
-        
-        for taxon in taxons:
-            keys = classif.keys()
-            if "</ScientificName>" in taxon and "<ScientificName>" in taxon and "<Rank>" in taxon and "</Rank>" in taxon:
-                name, _ = taxon.split("</ScientificName>", 1)
-                _, name = name.split("<ScientificName>", 1)
-                name = re.sub(r"\s+", '_', name)
-                rank, _ = taxon.split("</Rank>", 1)
-                _, rank= rank.split("<Rank>", 1)
-                rank = re.sub(r"\s+", '_', rank)
-                if rank == 'clade':
-                    if rank not in keys: 
-                        classif['clade'] = [name]
-                    else:
-                        classif['clade'].append(name)
+        lineageInfo, general_infos = xml.split("</LineageEx>", 1)
+        general_infos, lineageInfo = lineageInfo.split("<LineageEx>", 1)
+
+    if "</Rank>" in general_infos and "<Rank>" in general_infos and 'ScientificName' in classif:
+        taxon_info = general_infos.split("</Rank>", 1)[0].split("<Rank>", 1)[1]
+        classif[taxon_info] = classif['ScientificName']
+
+
+    taxons = lineageInfo.split("</Taxon>")
+    for taxon in taxons:
+        keys = classif.keys()
+        if "</ScientificName>" in taxon and "<ScientificName>" in taxon and "<Rank>" in taxon and "</Rank>" in taxon:
+            name, _ = taxon.split("</ScientificName>", 1)
+            _, name = name.split("<ScientificName>", 1)
+            name = re.sub(r"\s+", '_', name)
+            rank, _ = taxon.split("</Rank>", 1)
+            _, rank= rank.split("<Rank>", 1)
+            rank = re.sub(r"\s+", '_', rank)
+            if rank == 'clade':
+                if rank not in keys: 
+                    classif['clade'] = [name]
                 else:
-                    classif[rank] = name
-                    
+                    classif['clade'].append(name)
+            else:
+                classif[rank] = name
+                
     return classif
 
 
 if __name__=="_main_":
     countDown()
     download()
     dispatch()
```

### Comparing `nsdpy-0.3.6b0/nsdpy.py` & `nsdpy-0.3.7b0/nsdpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.3.6-beta'
+__version__ = '0.3.7-beta'
 __author__ = "Raphael Hebert, Emese Meglecz"
 __email__ = "raphaelhebert18@gmail.com, emese.meglecz@imbe.fr"
 __license__ = "MIT"
 
 import sys
 import os
 import argparse                     #parsing command line arguments
@@ -51,15 +51,15 @@
     group3.add_argument("-p", "--phylum", help="output one file text per phylum", action="store_true" )
     group3.add_argument("-l", "--levels", help="find only the taxon given by user", nargs="+")
     group3.add_argument("-s", "--species",\
         help="classify the results in different text file one for each (specie + n) level found, exp: -s correspond to lowest levels, -ss 2nd lowest, -sssss 5th lowest and so on",\
         action="count", default=2)
     group3.add_argument("-x", "--custom",\
         help="classify the result for the given taxonomic level",\
-        nargs="+")
+        nargs="+", type=str)
 
     # information line
     parser.add_argument("-i", "--information", help="just add the taxonomic information in the information line of the output file(s)", action="store_true" )
 
     args = parser.parse_args()
 
     #################################################
@@ -116,15 +116,15 @@
     elif args.phylum:
         classif = 0
         options_report.append("--phylum (-p)")
     elif args.levels:
         # here isinstance(classif, list) == true
         classif = args.levels
         options_report.append(f"--levels (-l) {args.levels[0]}")
-    elif args.custom[0]:
+    elif args.custom:
         classif = args.custom[0]
         options_report.append(f"--custom (-x) {args.custom}")
     elif args.species:
         classif = args.species
         if args.species != 2:
             options_report.append("--species (-" + "s" * ( args.species - 2 ) + ")")
     else:
```

### Comparing `nsdpy-0.3.6b0/pyproject.toml` & `nsdpy-0.3.7b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdpy"
-version = "0.3.6-beta"
+version = "0.3.7-beta"
 description = "Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)"
 authors = ["RaphaelHebert <raphaelhebert18@gmail.com>", "Emese Meglecz <emese.meglecz@imbe.fr>"]
 include = ["functions.py"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/RaphaelHebert/nsdpy"
 homepage = "https://github.com/RaphaelHebert/nsdpy"
```

### Comparing `nsdpy-0.3.6b0/PKG-INFO` & `nsdpy-0.3.7b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdpy
-Version: 0.3.6b0
+Version: 0.3.7b0
 Summary: Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)
 Home-page: https://github.com/RaphaelHebert/nsdpy
 License: MIT
 Keywords: NCBI,Taxonomy,DNA
 Author: RaphaelHebert
 Author-email: raphaelhebert18@gmail.com
 Requires-Python: >=3.8,<4.0
```

