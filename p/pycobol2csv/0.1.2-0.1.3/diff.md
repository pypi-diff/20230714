# Comparing `tmp/pycobol2csv-0.1.2-py3-none-any.whl.zip` & `tmp/pycobol2csv-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7809 bytes, number of entries: 7
+Zip file size: 7986 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       52 b- defN 21-Sep-15 00:40 pycobol2csv/__init__.py
--rw-rw-rw-  2.0 fat    18785 b- defN 21-Sep-17 12:03 pycobol2csv/convert.py
--rw-rw-rw-  2.0 fat     1086 b- defN 21-Sep-18 07:20 pycobol2csv-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1817 b- defN 21-Sep-18 07:20 pycobol2csv-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 21-Sep-18 07:20 pycobol2csv-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 21-Sep-18 07:20 pycobol2csv-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      564 b- defN 21-Sep-18 07:20 pycobol2csv-0.1.2.dist-info/RECORD
-7 files, 22408 bytes uncompressed, 6807 bytes compressed:  69.6%
+-rw-rw-rw-  2.0 fat    18899 b- defN 23-Jul-14 07:06 pycobol2csv/convert.py
+-rw-rw-rw-  2.0 fat     1086 b- defN 23-Jul-14 07:37 pycobol2csv-0.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2167 b- defN 23-Jul-14 07:37 pycobol2csv-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-14 07:37 pycobol2csv-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-14 07:37 pycobol2csv-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      564 b- defN 23-Jul-14 07:37 pycobol2csv-0.1.3.dist-info/RECORD
+7 files, 22872 bytes uncompressed, 6984 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pycobol2csv/__init__.py
 Comment: 
 
 Filename: pycobol2csv/convert.py
 Comment: 
 
-Filename: pycobol2csv-0.1.2.dist-info/LICENSE
+Filename: pycobol2csv-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: pycobol2csv-0.1.2.dist-info/METADATA
+Filename: pycobol2csv-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: pycobol2csv-0.1.2.dist-info/WHEEL
+Filename: pycobol2csv-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pycobol2csv-0.1.2.dist-info/top_level.txt
+Filename: pycobol2csv-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pycobol2csv-0.1.2.dist-info/RECORD
+Filename: pycobol2csv-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pycobol2csv/convert.py

```diff
@@ -99,16 +99,16 @@
 def parse_cobol(lines):
     output = []
 
     intify = ["level", "occurs"]
 
     # All in 1 line now, let's parse
     for row in lines:
-        print("Processing ", row)
-        print("=====================")
+        # print("Processing ", row)
+        # print("=====================")
         bcd_type_indicator = False
         occurs3_indicator = False
         if " USAGE COMP-3" in row:
             row = row.replace(" USAGE COMP-3", "")
             bcd_type_indicator = True
 
         # if 'OCCURS 3 TIMES' in row:
@@ -119,25 +119,25 @@
             occurs3_index = row.find("OCCURS ")
             whitespace_index = occurs3_index - 1
             while whitespace_index >= 0 and row[whitespace_index] == " ":
                 whitespace_index = whitespace_index - 1
 
             times_index = row.find(" TIMES", occurs3_index)
             times_number = row[occurs3_index + len(" TIMES") : times_index]
-            print("times number is ", times_number)
+            # print("times number is ", times_number)
 
             # string_to_replace = ' '* (occurs3_index - whitespace_index -1) + 'OCCURS 3 TIMES'
             string_to_replace = (
                 " " * (occurs3_index - whitespace_index - 1)
                 + row[occurs3_index : times_index + len(" TIMES")]
             )
-            print("string to replace is ", string_to_replace)
+            # print("string to replace is ", string_to_replace)
 
             row = row.replace(string_to_replace, "")
-            print("Found OCCURS 3 TIMES and new row is ", row)
+            # print("Found OCCURS 3 TIMES and new row is ", row)
             # occurs3_indicator = True
             occurs3_indicator = times_number
 
         match = CobolPatterns.row_pattern.match(row.strip())
 
         if not match:
             print("Found unmatched row", row.strip())
@@ -312,15 +312,15 @@
 
     default_padding = " " * 7
 
     levels = [0]
 
     for row in lines:
         row_output = []
-        print(row)
+        # print(row)
         if row["level"] > levels[-1]:
             levels.append(row["level"])
         else:
             while row["level"] < levels[-1]:
                 levels.pop()
 
         row_output.append((len(levels) - 1) * "  ")
@@ -385,16 +385,16 @@
                 previous_level = row["level"]
 
             if (
                 "occurs3" in row and row["occurs3"]
             ):  ### repeat for all items in the same group as the group is repeated!!!!
                 previous_occurs3 = row["occurs3"]  # True
             if "pic" in row and row["pic"] != None:
-                print("Current row")
-                print(row)
+                # print("Current row")
+                # print(row)
 
                 if previous_occurs3:
                     # print(previous_occurs3)
                     for index in range(int(previous_occurs3)):
                         # element = {'name': str(name_prefix) + '.' + row['name'] + '_' + str(index+1), 'type': row['pic_info']['type']}
                         element = {
                             "name": row["name"] + "_" + str(index + 1),
@@ -478,29 +478,30 @@
 
     """
     new_name = name.replace("-", "_")[:251]
     return new_name
 
 
 def convert_cobol_file(
-    copybook_filename, data_filename, output_filename, config_filename, codepage
+    copybook_filename, data_filename, output_filename, config_filename, codepage, debug=False
 ):
     # decode_ebcdic_file(datafile, processed_data_file)
     (row_length, cobol_struc) = decode_copybook_file(copybook_filename)
     headers = [sanitize_col_name_for_database(item["name"]) for item in cobol_struc]
-    print("total length per row is ")
-    print(row_length)
-    print("Cobol strucuture to consume is ")
-    print(cobol_struc)
+    if debug:
+        print("total length per row is ")
+        print(row_length)
+        print("Cobol strucuture to consume is ")
+        print(cobol_struc)
     with open(output_filename, "w", newline="") as csvfile, open(
         config_filename
     ) as json_file, open(data_filename, "rb") as data_file:
         config = json.load(json_file)
-
-        print(config)
+        if debug:
+            print(config)
 
         csvwriter = csv.writer(
             csvfile,
             delimiter=config["csv_config"]["delimiter"],
             quoting=config["csv_config"]["quoting_level"],
             quotechar=config["csv_config"]["quote_char"],
         )
@@ -514,22 +515,23 @@
                 data_read = data_file.read(item["length"])
                 if not data_read:
                     eof = True
                     break
                 if "Signed Integer" in item["type"]:
                     data_row.append(unpack_number(data_read))
                 elif "Signed Float" in item["type"]:
-                    print("Processing float ", item)
+                    # print("Processing float ", item)
                     integer_array = [hex(data_read[i]) for i in range(item["length"])]
-                    print(item["type"], item["name"], integer_array)
+                    # print(item["type"], item["name"], integer_array)
                     int_val = unpack_number(data_read)
                     float_val = float(int_val) / pow(10, item["precision"])
                     data_row.append(float_val)
-                    print(int_val, float_val)
+                    # print(int_val, float_val)
                 else:
                     original_str = codecs.decode(data_read, codepage).strip()
                     new_str = "".join(custom_encoder(original_str))
                     data_row.append(new_str)
                 current_pos = current_pos + item["length"]
-            print(data_row)
+            if debug:
+                print(data_row)
             if len(data_row) > 2:
                 csvwriter.writerow(data_row)
```

## Comparing `pycobol2csv-0.1.2.dist-info/LICENSE` & `pycobol2csv-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pycobol2csv-0.1.2.dist-info/METADATA` & `pycobol2csv-0.1.3.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,61 @@
-Metadata-Version: 2.1
-Name: pycobol2csv
-Version: 0.1.2
-Summary: A Python library to convert COBOL ebcdic file to CSV format
-Home-page: https://github.com/jasonli-lijie/pycobol2csv
-Author: Jason Li
-Author-email: niomobileapp@gmail.com
-License: MIT
-Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
-Project-URL: Bug Tracker, https://github.com/jasonli-lijie/pycobol2csv/issues
-Keywords: COBOL,EBCDIC,CSV
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: ebcdic
-
-# pycobol2csv
-pycobol2csv is a Python library to convert COBOL ebcdic file to CSV format. The package is built to cater for advanced features in COBOL copybooks such as *OCCURES x TIMES*. 
-
-The CSV file is RDBMS friendly and all headers are ready to be used as database column names.
-CSV conversion is controlled by config file in *csv_config.json*
-
-Install the python module:
-
-`pip install pycobol2csv`
-
-To use the module:
-
-```
-from pycobol2csv import convert_cobol_file
-
-convert_cobol_file(copybook_file, data_file, output_file, config_file, codepage)
-
-```
-
-- copybook_file: copybook filename
-- data_file: data filename 
-- output_file: output csv filename
-- config_file: csv configuration filename, refer to csv_config.json
-- codepage: codepage for edibic, refer to https://docs.python.org/3.7/library/codecs.html#standard-encodings for details
-
-Repo: https://github.com/jasonli-lijie/pycobol2csv
-
-
+Metadata-Version: 2.1
+Name: pycobol2csv
+Version: 0.1.3
+Summary: A Python library to convert COBOL ebcdic file to CSV format
+Home-page: https://github.com/jasonli-lijie/pycobol2csv
+Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
+Author: Jason Li
+Author-email: niomobileapp@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/jasonli-lijie/pycobol2csv/issues
+Keywords: COBOL,EBCDIC,CSV
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ebcdic
+
+# pycobol2csv
+pycobol2csv is a Python library to convert COBOL ebcdic file to CSV format. The package is built to cater for advanced features in COBOL copybooks such as *OCCURES x TIMES*. 
+
+The CSV file is RDBMS friendly and all headers are ready to be used as database column names.
+CSV conversion is controlled by config file in *csv_config.json*
+
+Install the python module:
+
+`pip install pycobol2csv`
+
+To use the module:
+
+```
+from pycobol2csv import convert_cobol_file
+
+convert_cobol_file(copybook_file, data_file, output_file, config_file, codepage, debug=False)
+
+```
+
+- copybook_file: copybook filename
+- data_file: data filename 
+- output_file: output csv filename
+- config_file: csv configuration filename, refer to csv_config.json
+- codepage: codepage for edibic, refer to https://docs.python.org/3.7/library/codecs.html#standard-encodings for details
+- debug: enable for more debug information, default is OFF
+
+## test 
+
+2 sets of test data have been created from scratch. Each set includes a copybook and an EBCDIC data file.
+
+To test:
+
+```
+python convert_cobol_test_main.py --copybook [COPYBOOK_FILE] --data [DATA_FILE] --output [CSV_FILE]
+
+```
+
+Repo: https://github.com/jasonli-lijie/pycobol2csv
```

