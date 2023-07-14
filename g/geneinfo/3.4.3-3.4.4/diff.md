# Comparing `tmp/geneinfo-3.4.3.tar.gz` & `tmp/geneinfo-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneinfo-3.4.3.tar", last modified: Tue Jul 11 09:40:11 2023, max compression
+gzip compressed data, was "geneinfo-3.4.4.tar", last modified: Fri Jul 14 09:41:25 2023, max compression
```

## Comparing `geneinfo-3.4.3.tar` & `geneinfo-3.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-07-11 09:40:11.091822 geneinfo-3.4.3/
--rw-rw-r--   0 kmt       (6358) kmt       (6358)     1069 2023-04-25 13:25:03.000000 geneinfo-3.4.3/LICENSE
--rw-rw-r--   0 kmt       (6358) kmt       (6358)      491 2023-07-11 09:40:11.091822 geneinfo-3.4.3/PKG-INFO
--rw-rw-r--   0 kmt       (6358) kmt       (6358)      174 2023-04-25 13:25:03.000000 geneinfo-3.4.3/README.md
-drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-07-11 09:40:11.087822 geneinfo-3.4.3/geneinfo/
--rw-rw-r--   0 kmt       (6358) kmt       (6358)    52678 2023-05-02 20:23:42.000000 geneinfo-3.4.3/geneinfo/__init__.py
--rw-rw-r--   0 kmt       (6358) kmt       (6358)     3385 2023-04-25 13:25:04.000000 geneinfo-3.4.3/geneinfo/intervals.py
-drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-07-11 09:40:11.090822 geneinfo-3.4.3/geneinfo.egg-info/
--rw-rw-r--   0 kmt       (6358) kmt       (6358)      491 2023-07-11 09:40:11.000000 geneinfo-3.4.3/geneinfo.egg-info/PKG-INFO
--rw-rw-r--   0 kmt       (6358) kmt       (6358)      228 2023-07-11 09:40:11.000000 geneinfo-3.4.3/geneinfo.egg-info/SOURCES.txt
--rw-rw-r--   0 kmt       (6358) kmt       (6358)        1 2023-07-11 09:40:11.000000 geneinfo-3.4.3/geneinfo.egg-info/dependency_links.txt
--rw-rw-r--   0 kmt       (6358) kmt       (6358)       68 2023-07-11 09:40:11.000000 geneinfo-3.4.3/geneinfo.egg-info/requires.txt
--rw-rw-r--   0 kmt       (6358) kmt       (6358)        9 2023-07-11 09:40:11.000000 geneinfo-3.4.3/geneinfo.egg-info/top_level.txt
--rw-rw-r--   0 kmt       (6358) kmt       (6358)       38 2023-07-11 09:40:11.091822 geneinfo-3.4.3/setup.cfg
--rw-rw-r--   0 kmt       (6358) kmt       (6358)      862 2023-07-11 09:38:22.000000 geneinfo-3.4.3/setup.py
+drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-07-14 09:41:25.655327 geneinfo-3.4.4/
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)     1069 2023-04-25 13:25:03.000000 geneinfo-3.4.4/LICENSE
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      491 2023-07-14 09:41:25.655327 geneinfo-3.4.4/PKG-INFO
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      174 2023-04-25 13:25:03.000000 geneinfo-3.4.4/README.md
+drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-07-14 09:41:25.650327 geneinfo-3.4.4/geneinfo/
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)    53255 2023-07-14 09:38:43.000000 geneinfo-3.4.4/geneinfo/__init__.py
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)     3385 2023-04-25 13:25:04.000000 geneinfo-3.4.4/geneinfo/intervals.py
+drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-07-14 09:41:25.654327 geneinfo-3.4.4/geneinfo.egg-info/
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      491 2023-07-14 09:41:25.000000 geneinfo-3.4.4/geneinfo.egg-info/PKG-INFO
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      228 2023-07-14 09:41:25.000000 geneinfo-3.4.4/geneinfo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)        1 2023-07-14 09:41:25.000000 geneinfo-3.4.4/geneinfo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)       68 2023-07-14 09:41:25.000000 geneinfo-3.4.4/geneinfo.egg-info/requires.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)        9 2023-07-14 09:41:25.000000 geneinfo-3.4.4/geneinfo.egg-info/top_level.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)       38 2023-07-14 09:41:25.655327 geneinfo-3.4.4/setup.cfg
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      862 2023-07-14 09:39:13.000000 geneinfo-3.4.4/setup.py
```

### Comparing `geneinfo-3.4.3/LICENSE` & `geneinfo-3.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geneinfo-3.4.3/geneinfo/__init__.py` & `geneinfo-3.4.4/geneinfo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,21 @@
 import requests
 from Bio import Entrez
 
 from .intervals import *
 
 # sys.path.append('.')
 
+# if this runs on a cluster node we need to set proxies to access external resources:
+if re.match(r's\d+n\d+', os.environ['HOSTNAME']):
+    os.environ['http_proxy'] = 'http://proxy-default:3128'
+    os.environ['https_proxy'] = 'http://proxy-default:3128'
+    os.environ['ftp_proxy'] = 'http://proxy-default:3128'
+    os.environ['ftps_proxy'] = 'http://proxy-default:3128'
+
 CACHE = dict()
 
 class NotFound(Exception):
     """query returned no result"""
     pass
 
 
@@ -361,14 +368,16 @@
     axes[-1].set_ylim(-2, offset+2)
     axes[-1].get_yaxis().set_visible(False)
     axes[-1].invert_yaxis()
     axes[-1].spines['top'].set_visible(False)
     axes[-1].spines['right'].set_visible(False)
     axes[-1].spines['left'].set_visible(False)
 
+    # TODO: add optional title explaining gene name styles
+
     for ax in axes[:-1]:
         ax.set_xlim(axes[-1].get_xlim())
 
         if despine:
             ax.spines['top'].set_visible(False)
             ax.spines['right'].set_visible(False)
     
@@ -613,15 +622,15 @@
                         print(ncbi_id, 'not in symbol2ncbi index')
                         raise NotFound
                         
                         
                     geneids.append(symbol2ncbi.loc[ncbi_id])
                     # geneids.append(ensembl2ncbi(ensembl_id(symbol)))                    
                 except NotFound:
-                    print(f'Could not map "{symbol}" to ncbi id', file=sys.stderr)
+                    print(f'Could not map gene symbol "{symbol}" to ncbi id', file=sys.stderr)
         return geneids
 
 
 def _cached_ncbi2symbol(geneids, taxid=9606):
 
     symbol2ncbi_file = f'geneinfo_cache/{taxid}_symbol2ncbi.h5'
     symbol2ncbi = pd.read_hdf(symbol2ncbi_file, 'ncbi2symbol')
@@ -629,15 +638,15 @@
         return symbol2ncbi.loc[geneids].tolist()
     except KeyError:
         symbols = []
         for geneid in geneids:
             try:
                 symbols.append(ncbi2symbol.loc[geneid])
             except KeyError:
-                print(f'Could not map "{geneid}" to gene symbol', file=sys.stderr)
+                print(f'Could not map ncbi id "{geneid}" to gene symbol', file=sys.stderr)
         return symbols
 
 
 def _tidy_taxid(taxid):
     try:
         taxid = int(taxid)
     except ValueError:
@@ -1197,14 +1206,15 @@
                      'hg38': {'chr1': 248956422, 'chr2': 242193529, 'chr3': 198295559, 'chr4': 190214555, 
                               'chr5': 181538259, 'chr6': 170805979, 'chr7': 159345973, 'chr8': 145138636, 
                               'chr9': 138394717, 'chr10': 133797422, 'chr11': 135086622, 'chr12': 133275309, 
                               'chr13': 114364328, 'chr14': 107043718, 'chr15': 101991189, 'chr16': 90338345, 
                               'chr17': 83257441, 'chr18': 80373285, 'chr19': 58617616, 'chr20': 64444167, 
                               'chr21': 46709983, 'chr22': 50818468, 'chrX': 156040895, 'chrY': 57227415}}    
 
+    # TODO: make the centromeres fit each assembly!
     centromeres = {
         'chr1':    (121700000, 125100000),
         'chr10':   (38000000, 41600000),
         'chr11':   (51000000, 55800000),
         'chr12':   (33200000, 37800000),
         'chr13':   (16500000, 18900000),
         'chr14':   (16100000, 18200000),
@@ -1259,17 +1269,17 @@
             ax.spines['top'].set_visible(False)
             ax.spines['right'].set_visible(False)
             ax.spines['bottom'].set_visible(False)
             ax.spines['left'].set_visible(False)
             ax.set_ylim((0, 3))
 
             if i in [20, 21]:   
-                x = -3500000
+                x = -3500000 * 10 / figsize[1]
             else:
-                x = -2000000
+                x = -2000000 * 10 / figsize[1]
             ax.text(x, 1, chrom.replace('chr', ''), fontsize=8, horizontalalignment='right', weight='bold')
 
             # h = ax.set_ylabel(chrom)
             # h.set_rotation(0)
             ax.set_yticklabels([])
 
             if i == 0:
@@ -1303,15 +1313,18 @@
             xy = [[cent_start, 1], [cent_start, 2], [cent_end, 1], [cent_end, 2]]
             g = ax.add_patch(Polygon(xy, closed=True, zorder=3, fill=True,
                                      # color='#666666',
                                      color='#777777',
                                     ))
 
 
-        def plot_segment(chrom, start, end, color='red', label=None, base=1, height=1):
+        def plot_segment(chrom, start, end, color='red', label=None, base=0, height=1):
+
+            base += 1
+            
             x, y, width = start, base, end-start
 
             if width < min_visible_width:
                 x -= min_visible_width/2
                 width += min_visible_width
 
             rect = Rectangle((x, y), width, height, linewidth=1, edgecolor='none', facecolor=color, zorder=3)
```

### Comparing `geneinfo-3.4.3/geneinfo/intervals.py` & `geneinfo-3.4.4/geneinfo/intervals.py`

 * *Files identical despite different names*

### Comparing `geneinfo-3.4.3/setup.py` & `geneinfo-3.4.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="geneinfo",
-    version="3.4.3",
+    version="3.4.4",
     author="Kasper Munch",
     author_email="kaspermunch@birc.au.dk",
     description="Functions for showing gene information in jupyter notebooks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kaspermunch/geneinfo",
     packages=setuptools.find_packages(),
```

