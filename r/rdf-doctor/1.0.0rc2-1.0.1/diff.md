# Comparing `tmp/rdf_doctor-1.0.0rc2-py3-none-any.whl.zip` & `tmp/rdf_doctor-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 23802 bytes, number of entries: 12
--rw-r--r--  2.0 unx       25 b- defN 23-Jul-12 07:39 doctor/__init__.py
+Zip file size: 23752 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-14 08:54 doctor/__init__.py
 -rw-r--r--  2.0 unx      631 b- defN 23-Jul-10 00:40 doctor/consts.py
--rw-r--r--  2.0 unx    39018 b- defN 23-Jul-12 07:39 doctor/doctor.py
--rw-r--r--  2.0 unx    43474 b- defN 23-Jul-11 05:56 doctor/reference/prefixes.tsv
+-rw-r--r--  2.0 unx    39079 b- defN 23-Jul-14 08:54 doctor/doctor.py
+-rw-r--r--  2.0 unx    43462 b- defN 23-Jul-12 23:57 doctor/reference/prefixes.tsv
 -rw-r--r--  2.0 unx       90 b- defN 23-Jul-10 00:40 doctor/reference/refine-class-uris.tsv
 -rw-r--r--  2.0 unx      577 b- defN 23-Jul-10 05:15 doctor/reference/refine-prefix-uris.tsv
--rw-r--r--  2.0 unx     1061 b- defN 23-Jul-12 07:48 rdf_doctor-1.0.0rc2.dist-info/LICENSE
--rw-r--r--  2.0 unx     8514 b- defN 23-Jul-12 07:48 rdf_doctor-1.0.0rc2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 07:48 rdf_doctor-1.0.0rc2.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-12 07:48 rdf_doctor-1.0.0rc2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-12 07:48 rdf_doctor-1.0.0rc2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1010 b- defN 23-Jul-12 07:48 rdf_doctor-1.0.0rc2.dist-info/RECORD
-12 files, 94551 bytes uncompressed, 22086 bytes compressed:  76.6%
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jul-14 08:59 rdf_doctor-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8525 b- defN 23-Jul-14 08:59 rdf_doctor-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 08:59 rdf_doctor-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-14 08:59 rdf_doctor-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-14 08:59 rdf_doctor-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jul-14 08:59 rdf_doctor-1.0.1.dist-info/RECORD
+12 files, 94590 bytes uncompressed, 22072 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: doctor/reference/refine-class-uris.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefix-uris.tsv
 Comment: 
 
-Filename: rdf_doctor-1.0.0rc2.dist-info/LICENSE
+Filename: rdf_doctor-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-1.0.0rc2.dist-info/METADATA
+Filename: rdf_doctor-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-1.0.0rc2.dist-info/WHEEL
+Filename: rdf_doctor-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-1.0.0rc2.dist-info/entry_points.txt
+Filename: rdf_doctor-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-1.0.0rc2.dist-info/top_level.txt
+Filename: rdf_doctor-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-1.0.0rc2.dist-info/RECORD
+Filename: rdf_doctor-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.0rc2"
+__version__ = "1.0.1"
```

## doctor/doctor.py

```diff
@@ -163,25 +163,25 @@
                         help="write to file instead of stdout",
                         metavar="FILE")
 
     # Target class(-c、--classes [URL1, URL2,...]、default: all、Multiple can be specified.)
     parser.add_argument("-c","--classes", type=str,
                         default=[TARGET_CLASS_ALL],
                         nargs="+",
-                        help="set the target classes to be inspected to one of: all (defalut) or URL1, URL2,...",
+                        help="set the target classes to be inspected to one of: all (defalut) or URL1 URL2...",
                         metavar="URL")
 
-    # Prefix URI dictionary file path(-p, --prefix-dict [FILE]、default: reference/refine-prefix-uris.tsv)
-    parser.add_argument("-p","--prefix-dict", type=str,
+    # Prefix URI dictionary file path(-p, --prefix-uri-dict [FILE]、default: reference/refine-prefix-uris.tsv)
+    parser.add_argument("-p","--prefix-uri-dict", type=str,
                         default=str(Path(__file__).resolve().parent.joinpath(REFINE_PREFIX_URIS_FILE_PATH)),
                         help='(only when "-r md"(same as "-r markdown") is specified) path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the prefix (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/refine-prefix-uris.tsv)',
                         metavar="FILE")
 
-    # Class URI dictionary file path(-l, --class-dict [FILE]、default: reference/refine-class-uris.tsv)
-    parser.add_argument("-l","--class-dict", type=str,
+    # Class URI dictionary file path(-l, --class-uri-dict [FILE]、default: reference/refine-class-uris.tsv)
+    parser.add_argument("-l","--class-uri-dict", type=str,
                         default=str(Path(__file__).resolve().parent.joinpath(REFINE_CLASS_URIS_FILE_PATH)),
                         help='(only when "-r md"(same as "-r markdown") is specified) path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the class (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/refine-class-uris.tsv)',
                         metavar="FILE")
 
     # Prefix list file path(-x, --prefix-list [FILE]、default: reference/prefixes.tsv)
     parser.add_argument("-x","--prefix-list", type=str,
                         default=str(Path(__file__).resolve().parent.joinpath(PREFIXES_FILE_PATH)),
@@ -308,38 +308,38 @@
     if args.force_format is not None:
         if args.force_format != TURTLE and \
             args.force_format != NT:
             error_msg = 'Input format error: "' + args.force_format + '" is an unsupported input format. "' + TURTLE + '" and "' + NT + '" are supported.'
             return False, error_msg
 
     # Prefix URIs dictionary file can be specified only in md/markdown mode
-    if args.prefix_dict != str(Path(__file__).resolve().parent.joinpath(REFINE_PREFIX_URIS_FILE_PATH)) and args.report == REPORT_FORMAT_SHEX:
+    if args.prefix_uri_dict != str(Path(__file__).resolve().parent.joinpath(REFINE_PREFIX_URIS_FILE_PATH)) and args.report == REPORT_FORMAT_SHEX:
         error_msg = 'Prefix URIs dictionary file error: Prefix URIs dictionary file can only be specified if "md"(same as "markdown") is specified in the -r, --report option.'
         return False, error_msg
 
-    if os.path.isfile(args.prefix_dict) == False:
+    if os.path.isfile(args.prefix_uri_dict) == False:
         error_msg = "Prefix URIs dictionary file error: Prefix dictionary does not exist or you don't have read permission."
         return False, error_msg
 
     # Check if the file has read permission
-    if os.access(args.prefix_dict, os.R_OK) == False:
+    if os.access(args.prefix_uri_dict, os.R_OK) == False:
         error_msg = "Prefix URIs dictionary file error: you don't have permission to read the input file."
         return False, error_msg
 
     # Class URIs dictionary file can be specified only in md/markdown mode
-    if args.class_dict != str(Path(__file__).resolve().parent.joinpath(REFINE_CLASS_URIS_FILE_PATH)) and args.report == REPORT_FORMAT_SHEX:
+    if args.class_uri_dict != str(Path(__file__).resolve().parent.joinpath(REFINE_CLASS_URIS_FILE_PATH)) and args.report == REPORT_FORMAT_SHEX:
         error_msg = 'Class URIs dictionary file error: Class URIs dictionary file can only be specified if "md"(same as "markdown") is specified in the -r, --report option.'
         return False, error_msg
 
-    if os.path.isfile(args.class_dict) == False:
+    if os.path.isfile(args.class_uri_dict) == False:
         error_msg = "Class URIs dictionary file error: Class dictionary does not exist or you don't have read permission."
         return False, error_msg
 
     # Check if the file has read permission
-    if os.access(args.class_dict, os.R_OK) == False:
+    if os.access(args.class_uri_dict, os.R_OK) == False:
         error_msg = "Class URIs dictionary file error: you don't have permission to read the input file."
         return False, error_msg
 
     if os.path.isfile(args.prefix_list) == False:
         error_msg = "Prefix list file error: Prefix list does not exist or you don't have read permission."
         return False, error_msg
 
@@ -443,15 +443,15 @@
             result_prefix_reuse_percentage.append("```\n\n")
 
         # Refer to the dictionary of prefix URIs and obtain a list that combines candidate pairs of URI rewrite source and rewrite destination
         if args.verbose:
             print_overwrite(get_dt_now() + " -- Comparing with prefix URIs dictionary...")
 
         result_refine_prefix_uris = []
-        prefix_comparison_result = get_prefix_comparison_result(input_prefixes, args.prefix_dict)
+        prefix_comparison_result = get_prefix_comparison_result(input_prefixes, args.prefix_uri_dict)
         # When there is data to output
         if len(prefix_comparison_result) != 0:
             result_refine_prefix_uris.append("Found a more widely used one for the prefix URI inputed.\n")
             result_refine_prefix_uris.append("```\n")
             result_refine_prefix_uris.append("Input-QName\tInput-prefix-URI\tSuggested-prefix-URI\n")
             result_refine_prefix_uris.extend(prefix_comparison_result)
             result_refine_prefix_uris.append("```\n\n")
@@ -473,15 +473,15 @@
 
         # Refers to the class URIs dictionary, acquires the list for result output that candidate pairs of URI rewrite source and rewrite destinations,
         # and generate the class corresponding to each key in fingerprint format stored in dictionary format.
         if args.verbose:
             print_overwrite(get_dt_now() + " -- Comparing with class URIs dictionary...")
 
         result_refine_class_uris = []
-        class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, args.class_dict)
+        class_comparison_result, fingerprint_class_dict = get_class_comparison_result(input_classes, args.class_uri_dict)
         # When there is data to output
         if len(class_comparison_result) != 0:
             result_refine_class_uris.append("Found a more widely used one for the class URI inputed.\n")
             result_refine_class_uris.append("```\n")
             result_refine_class_uris.append("Input-class-URI\tSuggested-class-URI\n")
             result_refine_class_uris.extend(class_comparison_result)
             result_refine_class_uris.append("```\n\n")
@@ -598,15 +598,15 @@
             with gzip.open(input_file, "rb") as f:
                 data = f.read()
             g.parse(data=data, format=input_format)
         else:
             g.parse(input_file, format=input_format)
 
         # Filter by classes(command line arguments)
-        class_filter = ",".join(target_classes)
+        class_filter = "<" + ">, <".join(target_classes) + ">"
 
         query = """
             SELECT DISTINCT ?class_name
             WHERE {
                 [] a ?class_name .
                 FILTER(! isBlank(?class_name))
         """
```

## doctor/reference/prefixes.tsv

```diff
@@ -921,15 +921,15 @@
 resid:	http://purl.obolibrary.org/obo/RESID_
 rex:	http://purl.obolibrary.org/obo/REX_
 rnao:	http://purl.obolibrary.org/obo/RNAO_
 rs:	http://purl.obolibrary.org/obo/RS_
 rxno:	http://purl.obolibrary.org/obo/RXNO_
 sao:	http://purl.obolibrary.org/obo/SAO_
 sbo:	http://purl.obolibrary.org/obo/SBO_
-178956970.291667	http://purl.obolibrary.org/obo/SEP_
+sep:	http://purl.obolibrary.org/obo/SEP_
 sibo:	http://purl.obolibrary.org/obo/SIBO_
 sopharm:	http://purl.obolibrary.org/obo/SOPHARM_
 spd:	http://purl.obolibrary.org/obo/SPD_
 swo:	http://purl.obolibrary.org/obo/SWO_
 symp:	http://purl.obolibrary.org/obo/SYMP_
 tads:	http://purl.obolibrary.org/obo/TADS_
 tahe:	http://purl.obolibrary.org/obo/TAHE_
```

## Comparing `rdf_doctor-1.0.0rc2.dist-info/LICENSE` & `rdf_doctor-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-1.0.0rc2.dist-info/METADATA` & `rdf_doctor-1.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 1.0.0rc2
+Version: 1.0.1
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -58,18 +58,18 @@
   -i RDF-FILE [RDF-FILE ...], --input RDF-FILE [RDF-FILE ...]
                         input RDF file(s)(.ttl or .nt or gzip-compressed versions of them). Use the same extension when specifying multiple.
   -r REPORT-FORMAT, --report REPORT-FORMAT
                         set the output format/serializer of report to one of: shex (defalut) or md or markdown(same as md)
   -o FILE, --output FILE
                         write to file instead of stdout
   -c URL [URL ...], --classes URL [URL ...]
-                        set the target classes to be inspected to one of: all (defalut) or URL1, URL2,...
-  -p FILE, --prefix-dict FILE
+                        set the target classes to be inspected to one of: all (defalut) or URL1 URL2...
+  -p FILE, --prefix-uri-dict FILE
                         (only when "-r md"(same as "-r markdown") is specified) path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the prefix (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/refine-prefix-uris.tsv)
-  -l FILE, --class-dict FILE
+  -l FILE, --class-uri-dict FILE
                         (only when "-r md"(same as "-r markdown") is specified) path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the class (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/refine-class-uris.tsv)
   -x FILE, --prefix-list FILE
                         list of prefixes (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/prefixes.tsv)
   -f INPUT-FORMAT, --force-format INPUT-FORMAT
                         This option should not normally be used. Because the input format is automatically determined by the file extension. Use it only when you want to force specification. If used, "turtle" or "nt" can be specified.
 ```
 
@@ -168,15 +168,15 @@
 ```
 ````
 
 
 ## Example of dictionary file
 You can specify arbitrary dictionary files for prefixes and class URIs. It is a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination one per line like [this](https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/refine-prefix-uris.tsv).
 This dictionary file is used only if -r or --report option is specified as md (same as markdown).
-Specify -p, --prefix-dict for prefix, -l, --class-dict for class, followed by file.
+Specify -p, --prefix-uri-dict for prefix, -l, --class-uri-dict for class, followed by file.
 See: https://github.com/dbcls/rdf-doctor#command-line-interface
 
 
 ## Example of prefix list
 You can specify arbitrary files for prefix list. It is a tab delimited file listing QName and URI like [this](https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/prefixes.tsv).
 This prefix list is used to calculate prefix reuse percentages(in "-r md") and to present widely used QName(in "-r shex").
 Specify -x, --prefix-list, followed by file.
```

## Comparing `rdf_doctor-1.0.0rc2.dist-info/RECORD` & `rdf_doctor-1.0.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-doctor/__init__.py,sha256=NkOwQwfEdXwwG-cmd9A-IS_-fhgqwRMABKCUsUI45tE,25
+doctor/__init__.py,sha256=d4QHYmS_30j0hPN8NmNPnQ_Z0TphDRbu4MtQj9cT9e8,22
 doctor/consts.py,sha256=g8qN1vFAkkiFWF_HMGBpkoED0SdtPsxNUc33fcyLeow,631
-doctor/doctor.py,sha256=VQQOYUY-9doE06_pL633_yw6RshrJxfNJcxkixzSEQc,39018
-doctor/reference/prefixes.tsv,sha256=9zIvWdCO3X65YnULmiBEsIapiZvmplZbB6MywGJp54s,43474
+doctor/doctor.py,sha256=uPiOh-BU4SKhSXEdcnZm-Lg5paX-NRNh-avhhUxgMvA,39079
+doctor/reference/prefixes.tsv,sha256=ZqRUe166NU5FhN6XND_fPlyXl58FPc-R-8fALfHK6II,43462
 doctor/reference/refine-class-uris.tsv,sha256=pd_nOSjR7bia96u9hhcjhBg9J6LUAuDFlyy-JE9tsys,90
 doctor/reference/refine-prefix-uris.tsv,sha256=KY5PZ4WCaLeB0APNBjAWq7_Q5Whc6FLg9ncX7BSPeuw,577
-rdf_doctor-1.0.0rc2.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
-rdf_doctor-1.0.0rc2.dist-info/METADATA,sha256=uJAeYHb9cu0fqq4LT7NIr7WylNEPROj614x9sUV3ZS8,8514
-rdf_doctor-1.0.0rc2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rdf_doctor-1.0.0rc2.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
-rdf_doctor-1.0.0rc2.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
-rdf_doctor-1.0.0rc2.dist-info/RECORD,,
+rdf_doctor-1.0.1.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
+rdf_doctor-1.0.1.dist-info/METADATA,sha256=o7ca_v1ZS-TB0M0464FKix_lUyKYaFMUmD756LdBDM4,8525
+rdf_doctor-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rdf_doctor-1.0.1.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
+rdf_doctor-1.0.1.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
+rdf_doctor-1.0.1.dist-info/RECORD,,
```

