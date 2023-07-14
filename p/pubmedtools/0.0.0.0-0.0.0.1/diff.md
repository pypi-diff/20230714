# Comparing `tmp/pubmedtools-0.0.0.0-py3.10.egg` & `tmp/pubmedtools-0.0.0.1-py3.10.egg`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6393 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     3767 b- defN 23-Jul-13 23:49 EGG-INFO/PKG-INFO
--rw-rw-rw-  2.0 fat      277 b- defN 23-Jul-13 23:49 EGG-INFO/SOURCES.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-13 23:49 EGG-INFO/dependency_links.txt
+Zip file size: 6336 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     3566 b- defN 23-Jul-13 23:53 EGG-INFO/PKG-INFO
+-rw-rw-rw-  2.0 fat      277 b- defN 23-Jul-13 23:53 EGG-INFO/SOURCES.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-13 23:53 EGG-INFO/dependency_links.txt
 -rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-13 23:13 EGG-INFO/not-zip-safe
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-13 23:49 EGG-INFO/requires.txt
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-13 23:49 EGG-INFO/top_level.txt
--rw-rw-rw-  2.0 fat      178 b- defN 23-Jul-13 23:49 pubmedtools/__init__.pyc
--rw-rw-rw-  2.0 fat     8166 b- defN 23-Jul-13 23:49 pubmedtools/pubmedtools.pyc
-8 files, 12420 bytes uncompressed, 5401 bytes compressed:  56.5%
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-13 23:53 EGG-INFO/requires.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-13 23:53 EGG-INFO/top_level.txt
+-rw-rw-rw-  2.0 fat      178 b- defN 23-Jul-13 23:53 pubmedtools/__init__.pyc
+-rw-rw-rw-  2.0 fat     8166 b- defN 23-Jul-13 23:53 pubmedtools/pubmedtools.pyc
+8 files, 12219 bytes uncompressed, 5344 bytes compressed:  56.3%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,68 +1,69 @@
 Metadata-Version: 2.1
 Name: pubmedtools
-Version: 0.0.0.0
+Version: 0.0.0.1
 Summary: Pubmed Tools (pubmedtools) package provides functions forsearching and retrieving articles from the PubMed databaseusing Biopython and NCBI Entrez Direct.
 Home-page: https://github.com/diogomachado-bioinfo/pubmedtools
 Author: Diogo de J. S. Machado
 Author-email: diogomachado.bioinfo@gmail.com
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 
-# Pubmed Tools (pubmedtools)
-Pubmed Tools (pubmedtools) package provides functions for searching and
+# PubmedTools (pubmedtools)
+PubmedTools (pubmedtools) package provides functions for searching and
 retrieving articles from the PubMed database using Biopython and NCBI Entrez
 Direct. This is not an official NCBI library and has no direct affiliation
 with the organization.
 
 ---
+
+---
 # Features
 
 ## PubMed Tools (biotext.pubmedtoos)
 - `aminocode.pubmed_search_biopython`: Searches the PubMed database using a
                                        given term.
 - `aminocode.pubmed_search_edirect`: Searches the PubMed database using the
-                                     Entrez
-                                           Direct tool.
+                                     Entrez Direct tool.
 - `aminocode.prepare_edirect_folder`: Prepares the Entrez Direct folder for use
                                       with the pubmed_search_edirect function.
 
-## Word Embedding Tools (biotext.wordembtools)
-- `wordembtools.WordEmbedding`: A class for generating word embeddings from a
-                                        collection of texts.
+---
 
 ---
 # Installation
-You can install Pubmed Tools using pip:
+You can install PubmedTools using pip:
 
     pip install pubmedtools
 
 ---
+
+---
 # Functions
 
 ## pubmedtools
 
 ---
-### pubmedtools.pubmed_search_biopython
+### `pubmedtools.pubmed_search_biopython`
 Searches the PubMed database using a given term and retrieves the abstract,
 title, publication date, authors, MeSH terms, and other terms related to each
 article. This function use the Bio.Entrez package from Biopython. The search is
 limited to 10,000 results.
 
 **Parameters**
 
-- term : str
+- `term` : str
     - The search term to be used in the query.
-- email : str, optional
+- `email` : str, optional
     - Email address to be used in case the Entrez server needs to contact you.
-- api_key : str, optional
+- `api_key` : str, optional
     - API key to access the Entrez server.
-- batch_size : int, optional
+- `batch_size` : int, optional
     - Number of articles to be downloaded per iteration. Default is 1000.
-- verbose : bool, optional
+- `verbose` : bool, optional
     - Whether to print progress messages. Default is True.
 
 **Returns**
 
 - pandas.DataFrame
     - A DataFrame with columns 'pmid', 'ti', 'ab', 'fau', 'dp', 'mh', and 'ot'.
     - Each row contains information related to a single article retrieved from
@@ -78,17 +79,17 @@
 ### pubmedtools.pubmed_search_edirect
 Searches the PubMed database using a given term and retrieves the abstract,
 title, publication date, authors, MeSH terms, and other terms related to each
 article. This function use the official NCBI Entrez Direct tool.
 
 **Parameters**
 
-- query : str
+- `query` : str
     - The query to be searched in PubMed.
-- api_key : str, optional
+- `api_key` : str, optional
     - The NCBI API key. If not provided, the search will be performed without
     the API key.
 
 **Returns**
 
 - pandas.DataFrame
     - A pandas DataFrame containing the search results.
```

