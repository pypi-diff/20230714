# Comparing `tmp/scutls-0.3.2.tar.gz` & `tmp/scutls-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scutls-0.3.2.tar", max compression
+gzip compressed data, was "scutls-0.3.3.tar", max compression
```

## Comparing `scutls-0.3.2.tar` & `scutls-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      601 2023-07-13 03:56:30.293056 scutls-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-13 04:04:57.949309 scutls-0.3.2/scutls/__init__.py
--rw-r--r--   0        0        0     7560 2023-07-12 14:28:04.640198 scutls-0.3.2/scutls/arguments.py
--rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.3.2/scutls/assets/genome_ensembl_107_54_54_54.json
--rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.3.2/scutls/assets/genome_ensembl_release_all.txt
--rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.3.2/scutls/assets/genome_ensembl_release_use.txt
--rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.3.2/scutls/assets/genome_ucsc.json
--rw-r--r--   0        0        0     2269 2023-07-08 04:35:05.254780 scutls-0.3.2/scutls/bam.py
--rw-r--r--   0        0        0     5820 2023-06-21 04:19:39.366335 scutls-0.3.2/scutls/barcode.py
--rw-r--r--   0        0        0     1381 2023-07-08 04:30:45.312955 scutls-0.3.2/scutls/cli.py
--rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.3.2/scutls/download.py
--rw-r--r--   0        0        0     4984 2023-06-29 04:31:23.564846 scutls-0.3.2/scutls/fastq.py
--rw-r--r--   0        0        0    14186 2023-07-13 03:48:31.653526 scutls-0.3.2/scutls/util.py
--rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 scutls-0.3.2/setup.py
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 scutls-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      601 2023-07-14 03:40:20.289609 scutls-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-14 03:40:35.401859 scutls-0.3.3/scutls/__init__.py
+-rw-r--r--   0        0        0     7916 2023-07-14 03:37:33.658144 scutls-0.3.3/scutls/arguments.py
+-rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.3.3/scutls/assets/genome_ensembl_107_54_54_54.json
+-rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.3.3/scutls/assets/genome_ensembl_release_all.txt
+-rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.3.3/scutls/assets/genome_ensembl_release_use.txt
+-rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.3.3/scutls/assets/genome_ucsc.json
+-rw-r--r--   0        0        0     3427 2023-07-14 03:33:14.643408 scutls-0.3.3/scutls/bam.py
+-rw-r--r--   0        0        0     5820 2023-06-21 04:19:39.366335 scutls-0.3.3/scutls/barcode.py
+-rw-r--r--   0        0        0     1429 2023-07-14 02:56:18.566606 scutls-0.3.3/scutls/cli.py
+-rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.3.3/scutls/download.py
+-rw-r--r--   0        0        0     4984 2023-06-29 04:31:23.564846 scutls-0.3.3/scutls/fastq.py
+-rw-r--r--   0        0        0    15192 2023-07-14 03:36:41.082108 scutls-0.3.3/scutls/util.py
+-rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 scutls-0.3.3/setup.py
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 scutls-0.3.3/PKG-INFO
```

### Comparing `scutls-0.3.2/pyproject.toml` & `scutls-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scutls"
-version = "0.3.2"
+version = "0.3.3"
 description = "Single-cell data processing utility tools"
 authors = ["Kai Hu <kai.hu@umassmed.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 importlib-resources = "^5.8.0"
 wget = "^3.2"
```

### Comparing `scutls-0.3.2/scutls/arguments.py` & `scutls-0.3.3/scutls/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,20 +137,26 @@
     required = False, type = str, default = None
 )
 parser_bam.add_argument(
     "-nproc", "--num_processor",
     help = "number of parallel jobs",
     required = False, type = int, default = 1
 )
-parser_bam.add_argument(
+## add mutually exclusive groups
+parser_bam_group = parser_bam.add_mutually_exclusive_group()
+parser_bam_group.add_argument(
     "-lpir", "--locate_pos_in_read",
     help = "reference coordinate to be located in each read",
-    required = False, type = int, default = 1
+    required = False, type = int, default = None
+)
+parser_bam_group.add_argument(
+    "-lpiref", "--locate_pos_in_ref",
+    help = "find out the coordinates in reference for each cigar tuple for each read, output will be like: read_id,cigar_char,cigar_char_length,ref_pos",
+    required = False, action = 'store_true', default = False
 )
-## add mutually exclusive groups
 ## set default values
 parser_bam.set_defaults(func = cli.run_bam)
 
 # sub-command: barcode
 parser_barcode = subparsers.add_parser(
     "barcode", description = "handle barcode file")
 parser_barcode.add_argument(
```

### Comparing `scutls-0.3.2/scutls/assets/genome_ensembl_107_54_54_54.json` & `scutls-0.3.3/scutls/assets/genome_ensembl_107_54_54_54.json`

 * *Files identical despite different names*

### Comparing `scutls-0.3.2/scutls/assets/genome_ensembl_release_all.txt` & `scutls-0.3.3/scutls/assets/genome_ensembl_release_all.txt`

 * *Files identical despite different names*

### Comparing `scutls-0.3.2/scutls/assets/genome_ucsc.json` & `scutls-0.3.3/scutls/assets/genome_ucsc.json`

 * *Files identical despite different names*

### Comparing `scutls-0.3.2/scutls/bam.py` & `scutls-0.3.3/scutls/bam.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,101 @@
 import argparse
 from multiprocessing import Pool
 import functools
-from .util import bam_chunk_interval, bam_locate_pos_in_read
+from .util import bam_chunk_interval, bam_locate_pos_in_read, bam_locate_pos_in_ref
 
-def bam(input = None, output = None, locate_pos_in_read = None, nproc = 1):
+def bam(input = None, output = None, locate_pos_in_read = None, locate_pos_in_ref = False, nproc = 1):
     """bam subcommand
     Paramters
     ---------
 
     input : str
         input file name, must end with .bam
     output : str
         output file name
     locate_pos_in_read : int
         a reference coornidate to be located in each read in the bam file
-        
         ------------------
         Ref:    AATCCGGC
         Query:  AA  CGGC
         Q-pos:  12  3456
         ------------------
-        For the above case, if trying to locate reference coordinate 2 (0-based), which is "T", the query pos 2 will be returned. One can add 1 to easily obtain
-        
-    nproc: int
+        For the above case, if trying to locate reference coordinate 2 (0-based), which is "T", the query pos 2 will be returned. 
+    locate_pos_in_ref : bool
+        for each read in bam: for every cigar tuple, output the corresponding reference coordinate
+    
+    nproc : int
         number of parallel jobs, default to 1
         funtions that support nproc: locate_pos_in_read
 
     """
-
     args = list(locals().keys())
 
     local = locals()
     if all(bool(local[key]) is not True for key in args): # use True since args can be either None or False
         print("scutls bam: warning: use 'scutls bam -h' for usage")
 
-    if output == None:
-        pass
-    else:
-        print("Processing ...")
+    # locate a given reference coordinate in each read
+    if locate_pos_in_read:
+        if output == None:
+            pass
+        else:
+            print("Processing ...")
+            
+        intervals = bam_chunk_interval(bam = input, nproc = nproc)
+        p = Pool(nproc)
+        res = p.map_async(
+            functools.partial(
+                bam_locate_pos_in_read,
+                bam = input,
+                ref_coordinate = int(locate_pos_in_read)),
+                intervals.values()).get()
+
+        res_locate = []
+        for x in range(len(res)):
+            res_locate += res[x]
         
-    intervals = bam_chunk_interval(bam = input, nproc = nproc)
-    p = Pool(nproc)
-    res = p.map_async(
-        functools.partial(
-            bam_locate_pos_in_read,
-            bam = input,
-            ref_coordinate = int(locate_pos_in_read)),
-            intervals.values()).get()
-
-    res_locate = []
-    for x in range(len(res)):
-        res_locate += res[x]
-    
-    if output == None:
-        for x in res_locate:
-            print(x)
-    else:
-        with open(output, "w") as f:
+        print(res_locate)
+        
+        if output == None:
+            for x in res_locate:
+                print(x)
+        else:
+            with open(output, "w") as f:
+                for x in res_locate:
+                    f.write(x + "\n")
+            print("Done!")
+
+    # locate each cigar tuple in reference coordinate for every read
+    if locate_pos_in_ref:
+        if output == None:
+            pass
+        else:
+            print("Processing ...")
+            
+        intervals = bam_chunk_interval(bam = input, nproc = nproc)
+        p = Pool(nproc)
+        res = p.map_async(
+            functools.partial(
+                bam_locate_pos_in_ref,
+                bam = input),
+                intervals.values()).get()
+
+        res_locate = []
+        for x in range(len(res)):
+            res_locate += res[x]
+        
+        if output == None:
             for x in res_locate:
-                f.write(x + "\n")
-        print("Done!")
+                print(x)
+        else:
+            with open(output, "w") as f:
+                for x in res_locate:
+                    f.write(x + "\n")
+            print("Done!")
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('--input',  '-i', type = str)
     parser.add_argument('--output', '-o', type = str, default = None)
     parser.add_argument('--locate_pos_in_read', '-lpir', default = 0)
     parser.add_argument('--num_processor', '-nproc', default = 1, type = int)
```

### Comparing `scutls-0.3.2/scutls/barcode.py` & `scutls-0.3.3/scutls/barcode.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.2/scutls/cli.py` & `scutls-0.3.3/scutls/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     )
 
 def run_bam(args):
     bam.bam(
     input  = args.input,
     output = args.output,
     locate_pos_in_read = args.locate_pos_in_read,
+    locate_pos_in_ref = args.locate_pos_in_ref,
     nproc = args.num_processor
     )
 
 def run_barcode(args):
     barcode.barcode(
     input  = args.input,
     output = args.output,
```

### Comparing `scutls-0.3.2/scutls/download.py` & `scutls-0.3.3/scutls/download.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.2/scutls/fastq.py` & `scutls-0.3.3/scutls/fastq.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.2/scutls/util.py` & `scutls-0.3.3/scutls/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -252,14 +252,26 @@
                 else:
                     res.append([record.id, "NA", len(record.seq)])
     return(res)
 
 # if containing the following characters, the pattern will be passed directly to regex:
 special_search_character = ["{", "}", "(", ")", "*", "="]
 
+# map cigar number to letter
+cigar_num2char = {}
+cigar_num2char[0] = "M"
+cigar_num2char[1] = "I"
+cigar_num2char[2] = "D"
+cigar_num2char[3] = "N"
+cigar_num2char[4] = "S"
+cigar_num2char[5] = "H"
+cigar_num2char[6] = "P"
+cigar_num2char[7] = "="
+cigar_num2char[8] = "X"
+
 # calculate CIGAR consumption, used for "scutls bam --locate_pos_in_read"
 def cigar_consume(cigar_tuple):
     """_calculate the query and reference consumption given cigar_tuple, return tuple (query_consumed, ref_consumed)_
     
     Ref: https://samtools.github.io/hts-specs/SAMv1.pdf
     
     M 0 alignment match (can be a sequence match or mismatch) yes yes
@@ -347,9 +359,26 @@
                                     break
                                 else:
                                     # the last checked CIGAR tuple must be D, and already covered since read_pos must == read_pos_tem
                                     res.append(alignment.query_name + ",invalid")
                                     break
     return(res)
 
+# locate for each cigar tuple the corresponding reference coordinate for each read
+def bam_locate_pos_in_ref(interval, bam):
+    res = []
+    with pysam.AlignmentFile(bam, 'rb') as bam_file:
+        for i, alignment in enumerate(bam_file):
+            if i in interval:
+                ref_pos  = alignment.reference_start
+                read_pos = 0
+                for i, v in enumerate(alignment.cigartuples):
+                    res.append(",".join([alignment.query_name, cigar_num2char[v[0]], str(v[1]), str(ref_pos)]))
+                    
+                    query_consume, ref_consume = cigar_consume(v)
+                    ref_pos = ref_pos + ref_consume 
+                    read_pos = read_pos + query_consume
+    return(res)
+
+
 if __name__ == "__main__":
     update_ensembl_release()
```

### Comparing `scutls-0.3.2/setup.py` & `scutls-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'wget>=3.2,<4.0']
 
 entry_points = \
 {'console_scripts': ['scutls = scutls.arguments:main']}
 
 setup_kwargs = {
     'name': 'scutls',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'Single-cell data processing utility tools',
     'long_description': 'None',
     'author': 'Kai Hu',
     'author_email': 'kai.hu@umassmed.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scutls-0.3.2/PKG-INFO` & `scutls-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scutls
-Version: 0.3.2
+Version: 0.3.3
 Summary: Single-cell data processing utility tools
 Author: Kai Hu
 Author-email: kai.hu@umassmed.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

