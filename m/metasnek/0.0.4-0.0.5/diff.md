# Comparing `tmp/metasnek-0.0.4.tar.gz` & `tmp/metasnek-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasnek-0.0.4.tar", last modified: Thu Jun 29 08:28:54 2023, max compression
+gzip compressed data, was "metasnek-0.0.5.tar", last modified: Fri Jul 14 07:45:47 2023, max compression
```

## Comparing `metasnek-0.0.4.tar` & `metasnek-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:28:54.032666 metasnek-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-29 08:28:40.000000 metasnek-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 08:28:40.000000 metasnek-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-29 08:28:54.032666 metasnek-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-29 08:28:40.000000 metasnek-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 08:28:40.000000 metasnek-0.0.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:28:54.032666 metasnek-0.0.4/metasnek/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 08:28:40.000000 metasnek-0.0.4/metasnek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-06-29 08:28:40.000000 metasnek-0.0.4/metasnek/fastq_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:28:54.032666 metasnek-0.0.4/metasnek.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-29 08:28:54.000000 metasnek-0.0.4/metasnek.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-29 08:28:54.000000 metasnek-0.0.4/metasnek.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:28:54.000000 metasnek-0.0.4/metasnek.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 08:28:54.000000 metasnek-0.0.4/metasnek.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:28:54.032666 metasnek-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-29 08:28:40.000000 metasnek-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:28:54.032666 metasnek-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-06-29 08:28:40.000000 metasnek-0.0.4/tests/test_fastq_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:45:47.229712 metasnek-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 07:45:33.000000 metasnek-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 07:45:33.000000 metasnek-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-14 07:45:47.229712 metasnek-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-14 07:45:33.000000 metasnek-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 07:45:33.000000 metasnek-0.0.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:45:47.225712 metasnek-0.0.5/metasnek/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-14 07:45:33.000000 metasnek-0.0.5/metasnek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-07-14 07:45:33.000000 metasnek-0.0.5/metasnek/fastq_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:45:47.229712 metasnek-0.0.5/metasnek.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-14 07:45:47.000000 metasnek-0.0.5/metasnek.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-14 07:45:47.000000 metasnek-0.0.5/metasnek.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:45:47.000000 metasnek-0.0.5/metasnek.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 07:45:47.000000 metasnek-0.0.5/metasnek.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 07:45:47.229712 metasnek-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-14 07:45:33.000000 metasnek-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:45:47.229712 metasnek-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-07-14 07:45:33.000000 metasnek-0.0.5/tests/test_fastq_finder.py
```

### Comparing `metasnek-0.0.4/LICENSE` & `metasnek-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metasnek-0.0.4/metasnek/fastq_finder.py` & `metasnek-0.0.5/metasnek/fastq_finder.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,62 +29,76 @@
         if re.search(pattern, file_name, re.IGNORECASE):
             R1_file = None
             R2_file = None
 
             if "_R1" in file_name:
                 sample_name = file_name.rsplit("_R1", 1)[0]
                 R2_file = file_path.replace("_R1", "_R2") + file_ext
+                S_file = file_path.replace("_R1", "_S") + file_ext
                 R1_file = file
             elif "_R2" in file_name:
                 sample_name = file_name.rsplit("_R2", 1)[0]
                 R1_file = file_path.replace("_R2", "_R1") + file_ext
+                S_file = file_path.replace("_R2", "_S") + file_ext
                 R2_file = file
+            elif "_S" in file_name:
+                sample_name = file_name.rsplit("_S", 1)[0]
+                R1_file = file_path.replace("_S", "_R1") + file_ext
+                R2_file = file_path.replace("_S", "_R2") + file_ext
+                S_file = file
             if R1_file and R2_file and R1_file in file_list and R2_file in file_list:
-                paired_files.add((sample_name, R1_file, R2_file))
+                if S_file and S_file in file_list:
+                    paired_files.add((sample_name, R1_file, R2_file, S_file))
+                else:
+                    paired_files.add((sample_name, R1_file, R2_file, None))
             else:
                 sample_name = re.split(r"\.(fasta|fastq)(\.gz)?$", file_name)[0]
                 if "_R1" in sample_name or "_R2" in sample_name:
-                    warnings.warn(f"Orphaned paired read detected: {file_name}", Warning)
+                    warnings.warn("Orphaned paired read detected for " + file_name, Warning)
                 unpaired_files.add((sample_name, file))
 
     return paired_files, unpaired_files
 
 
 def parse_tsv_file(file_path):
-    """Parses a 3-column TSV file of sample names and sequencing reads (column 3 is optional)
+    """Parses a 2-4 column TSV file of sample names and sequencing reads (column 3/4 is optional)
 
     Args:
         file_path (str): Path to the TSV file.
 
     Returns:
         tuple: A tuple containing two lists:
-            - paired_reads: A list of tuples with the sample name, R1 file, and R2 file (if available).
+            - paired_reads: A list of tuples with the sample name, R1 file, R2 file, and singleton file.
             - unpaired_reads: A list of tuples with the sample name and R1 file (for unpaired reads).
     """
 
     paired_reads = set()
     unpaired_reads = set()
 
     with open(file_path, 'r') as tsv_file:
         reader = csv.reader(tsv_file, delimiter='\t')
 
         for row in reader:
 
             sample_name = row[0].strip()
             r1_file = row[1].strip()
             r2_file = row[2].strip() if len(row) >= 3 else None
+            s_file = row[3].strip() if len(row) >= 4 else None
 
             if not os.path.isfile(r1_file):
                 raise FileNotFoundError(f"R1 file '{r1_file}' does not exist.")
 
             if r2_file and not os.path.isfile(r2_file) and not r2_file.lower() in ["none", "null"]:
                 raise FileNotFoundError(f"R2 file '{r2_file}' does not exist.")
 
+            if s_file and not os.path.isfile(s_file) and not s_file.lower() in ["none", "null"]:
+                raise FileNotFoundError(f"S file '{s_file}' does not exist.")
+
             if r2_file:
-                paired_reads.add((sample_name, r1_file, r2_file))
+                paired_reads.add((sample_name, r1_file, r2_file, s_file))
             else:
                 unpaired_reads.add((sample_name, r1_file))
 
     return paired_reads, unpaired_reads
 
 
 def parse_samples(input_file_or_directory):
@@ -127,21 +141,21 @@
             - sample name (dict):
                 - R1 (str): filepath of R1 reads file
                 - R2 (str): filepath of R2 reads file or None for unpaired
     """
 
     reads_dictionary = {}
 
-    for sample_name, r1_file, r2_file in paired_reads:
+    for sample_name, r1_file, r2_file, s_file in paired_reads:
         if sample_name not in reads_dictionary:
-            reads_dictionary[sample_name] = {'R1': r1_file, 'R2': r2_file}
+            reads_dictionary[sample_name] = {'R1': r1_file, 'R2': r2_file, 'S': s_file}
 
     for sample_name, r1_file in unpaired_reads:
         if sample_name not in reads_dictionary:
-            reads_dictionary[sample_name] = {'R1': r1_file, 'R2': None}
+            reads_dictionary[sample_name] = {'R1': r1_file, 'R2': None, 'S': None}
 
     return reads_dictionary
 
 
 def parse_samples_to_dictionary(input_file_or_directory):
     """Convenience function to parse the samples directory or TSV and return the samples dictionary
 
@@ -149,30 +163,38 @@
         input_file_or_directory (str): filepath of samples TSV or directory
 
     Returns:
         dict:
             - sample name (dict):
                 - R1 (str): filepath of R1 reads file
                 - R2 (str): filepath of R2 reads file or None for unpaired
+                - S (str): filepath of singleton reads file or None
     """
     paired, unpaired = parse_samples(input_file_or_directory)
     sample_dictionary = convert_to_dictionary(paired, unpaired)
     return sample_dictionary
 
 
 def write_samples_tsv(dictionary, output_file):
     """Write the samples dictionary to a TSV file
 
     Args:
         dictionary:
             - sample name (dict):
                 - R1 (str): filepath of R1 reads file
-                - R2 (str): filepath of R2 reads file or None for unpaired
+                - R2 (str): filepath of R2 reads file or None
+                - S (str): filepath of singleton reads file or None
         output_file (str): filepath of output file for writing
     """
 
     with open(output_file, "w") as out:
         for sample in dictionary.keys():
-            if dictionary[sample]['R2'] is not None and dictionary[sample]['R2'].lower() not in ["none", "null"]:
-                out.write(f"{sample}\t{dictionary[sample]['R1']}\t{dictionary[sample]['R2']}\n")
-            else:
-                out.write(f"{sample}\t{dictionary[sample]['R1']}\n")
+            out.write(f"{sample}\t{dictionary[sample]['R1']}")
+            if "R2" in dictionary[sample].keys() \
+                    and dictionary[sample]['R2'] is not None \
+                    and dictionary[sample]['R2'].lower() not in ["none", "null"]:
+                out.write(f"\t{dictionary[sample]['R2']}")
+                if "S" in dictionary[sample].keys() \
+                        and dictionary[sample]['S'] is not None \
+                        and dictionary[sample]['S'].lower() not in ["none", "null"]:
+                    out.write(f"\t{dictionary[sample]['S']}")
+            out.write("\n")
```

### Comparing `metasnek-0.0.4/setup.py` & `metasnek-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 
 
 setup(
     name="metasnek",
     url="https://github.com/beardymcjohnface/metasnek",
-    python_requires=">=3.9",
+    python_requires=">=3.8",
     description="Misc functions for metagenomics pipelines",
     long_description=get_description(),
     long_description_content_type="text/markdown",
     version=get_version(),
     author="Michael Roach",
     author_email="beardymcjohnface@gmail.com",
 )
```

### Comparing `metasnek-0.0.4/tests/test_fastq_finder.py` & `metasnek-0.0.5/tests/test_fastq_finder.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,33 +21,39 @@
 @pytest.fixture(scope="session")
 def file_list(temp_directory):
     _file_list = [
         os.path.join(str(temp_directory), "sample1_R1.fastq"),
         os.path.join(str(temp_directory), "sample1_R2.fastq"),
         os.path.join(str(temp_directory), "sample2_R1_001.fastq.gz"),
         os.path.join(str(temp_directory), "sample2_R2_001.fastq.gz"),
+        os.path.join(str(temp_directory), "sample2_S_001.fastq.gz"),
         os.path.join(str(temp_directory), "sample3.fastq"),
         os.path.join(str(temp_directory), "sample4_R2.fastq"),
         os.path.join(str(temp_directory), "sample5.fasta.gz"),
         os.path.join(str(temp_directory), "sample6.fastq.gz"),
     ]
 
     for file_path in _file_list:
         open(file_path, "w").close()
 
     return _file_list
 
 
 def assert_parsed_files(paired_files, unpaired_files, temp_directory):
     # Assert paired files
-    assert ("sample1", os.path.join(str(temp_directory), "sample1_R1.fastq"), os.path.join(str(temp_directory), "sample1_R2.fastq")) in paired_files
+    assert ("sample1",
+            os.path.join(str(temp_directory), "sample1_R1.fastq"),
+            os.path.join(str(temp_directory), "sample1_R2.fastq"),
+            None
+            ) in paired_files
     assert (
         "sample2",
         os.path.join(str(temp_directory), "sample2_R1_001.fastq.gz"),
         os.path.join(str(temp_directory), "sample2_R2_001.fastq.gz"),
+        os.path.join(str(temp_directory), "sample2_S_001.fastq.gz"),
     ) in paired_files
     # Assert unpaired files
     assert ("sample3", os.path.join(str(temp_directory), "sample3.fastq")) in unpaired_files
     assert ("sample4_R2", os.path.join(str(temp_directory), "sample4_R2.fastq")) in unpaired_files
     assert ("sample5", os.path.join(str(temp_directory), "sample5.fasta.gz")) in unpaired_files
     assert ("sample6", os.path.join(str(temp_directory), "sample6.fastq.gz")) in unpaired_files
 
@@ -63,14 +69,16 @@
             + "\t"
             + os.path.join(str(temp_directory), "sample1_R2.fastq")
             + "\n"
             "sample2\t"
             + os.path.join(str(temp_directory), "sample2_R1_001.fastq.gz")
             + "\t"
             + os.path.join(str(temp_directory), "sample2_R2_001.fastq.gz")
+            + "\t"
+            + os.path.join(str(temp_directory), "sample2_S_001.fastq.gz")
             + "\n"
             "sample3\t" + os.path.join(str(temp_directory), "sample3.fastq") + "\n"
             "sample4_R2\t"
             + os.path.join(str(temp_directory), "sample4_R2.fastq")
             + "\n"
             "sample5\t" + os.path.join(str(temp_directory), "sample5.fasta.gz") + "\n"
             "sample6\t" + os.path.join(str(temp_directory), "sample6.fastq.gz") + "\n"
@@ -144,49 +152,68 @@
         tsv_file.write(invalid_tsv_content)
 
     with pytest.raises(ValueError):
         parse_samples(invalid_tsv_file)
 
 
 def test_convert_to_dictionary():
-    paired_reads = {("sample1", "sample1_R1.fastq", "sample1_R2.fastq"), ("sample2", "sample2_R1.fastq", "sample2_R2.fastq")}
+    paired_reads = {("sample1", "sample1_R1.fastq", "sample1_R2.fastq", None),
+                    ("sample2", "sample2_R1.fastq", "sample2_R2.fastq", "sample2_S.fastq")}
     unpaired_reads = {("sample3", "sample3_R1.fastq"), ("sample4", "sample4_R1.fastq")}
 
     expected_dictionary = {
-        "sample1": {"R1": "sample1_R1.fastq", "R2": "sample1_R2.fastq"},
-        "sample2": {"R1": "sample2_R1.fastq", "R2": "sample2_R2.fastq"},
-        "sample3": {"R1": "sample3_R1.fastq", "R2": None},
-        "sample4": {"R1": "sample4_R1.fastq", "R2": None},
+        "sample1": {"R1": "sample1_R1.fastq", "R2": "sample1_R2.fastq", "S": None},
+        "sample2": {"R1": "sample2_R1.fastq", "R2": "sample2_R2.fastq", "S": "sample2_S.fastq"},
+        "sample3": {"R1": "sample3_R1.fastq", "R2": None, "S": None},
+        "sample4": {"R1": "sample4_R1.fastq", "R2": None, "S": None},
     }
 
     assert convert_to_dictionary(paired_reads, unpaired_reads) == expected_dictionary
 
 
 @pytest.mark.filterwarnings("ignore:Orphaned paired")
 def test_parse_samples_to_dictionary(temp_directory, create_sample_tsv):
     # Test parsing a directory
     directory_dictionary = {
-        "sample1": {"R1": os.path.join(temp_directory, "sample1_R1.fastq"), "R2": os.path.join(temp_directory, "sample1_R2.fastq")},
-        "sample2": {"R1": os.path.join(temp_directory, "sample2_R1_001.fastq.gz"), "R2": os.path.join(temp_directory, "sample2_R2_001.fastq.gz")},
-        "sample3": {"R1": os.path.join(temp_directory, "sample3.fastq"), "R2": None},
-        "sample4_R2": {"R1": os.path.join(temp_directory, "sample4_R2.fastq"), "R2": None},
-        "sample5": {"R1": os.path.join(temp_directory, "sample5.fasta.gz"), "R2": None},
-        "sample6": {"R1": os.path.join(temp_directory, "sample6.fastq.gz"), "R2": None},
+        "sample1": {"R1": os.path.join(temp_directory, "sample1_R1.fastq"),
+                    "R2": os.path.join(temp_directory, "sample1_R2.fastq"),
+                    "S": None},
+        "sample2": {"R1": os.path.join(temp_directory, "sample2_R1_001.fastq.gz"),
+                    "R2": os.path.join(temp_directory, "sample2_R2_001.fastq.gz"),
+                    "S": os.path.join(temp_directory, "sample2_S_001.fastq.gz")},
+        "sample3": {"R1": os.path.join(temp_directory, "sample3.fastq"),
+                    "R2": None,
+                    "S": None},
+        "sample4_R2": {"R1": os.path.join(temp_directory, "sample4_R2.fastq"),
+                       "R2": None,
+                       "S": None},
+        "sample5": {"R1": os.path.join(temp_directory, "sample5.fasta.gz"),
+                    "R2": None,
+                    "S": None},
+        "sample6": {"R1": os.path.join(temp_directory, "sample6.fastq.gz"),
+                    "R2": None,
+                    "S": None},
     }
 
     assert parse_samples_to_dictionary(temp_directory) == directory_dictionary
 
     # Test parsing a TSV file
     tsv_dictionary = {
-        "sample1": {"R1": os.path.join(temp_directory, "sample1_R1.fastq"), "R2": os.path.join(temp_directory, "sample1_R2.fastq")},
-        "sample2": {"R1": os.path.join(temp_directory, "sample2_R1_001.fastq.gz"), "R2": os.path.join(temp_directory, "sample2_R2_001.fastq.gz")},
-        "sample3": {"R1": os.path.join(temp_directory, "sample3.fastq"), "R2": None},
-        "sample4_R2": {"R1": os.path.join(temp_directory, "sample4_R2.fastq"), "R2": None},
-        "sample5": {"R1": os.path.join(temp_directory, "sample5.fasta.gz"), "R2": None},
-        "sample6": {"R1": os.path.join(temp_directory, "sample6.fastq.gz"), "R2": None},
+        "sample1": {"R1": os.path.join(temp_directory, "sample1_R1.fastq"),
+                    "R2": os.path.join(temp_directory, "sample1_R2.fastq"),
+                    "S": None},
+        "sample2": {"R1": os.path.join(temp_directory, "sample2_R1_001.fastq.gz"),
+                    "R2": os.path.join(temp_directory, "sample2_R2_001.fastq.gz"),
+                    "S": os.path.join(temp_directory, "sample2_S_001.fastq.gz")},
+        "sample3": {"R1": os.path.join(temp_directory, "sample3.fastq"),
+                    "R2": None,
+                    "S": None},
+        "sample4_R2": {"R1": os.path.join(temp_directory, "sample4_R2.fastq"), "R2": None, "S": None},
+        "sample5": {"R1": os.path.join(temp_directory, "sample5.fasta.gz"), "R2": None, "S": None},
+        "sample6": {"R1": os.path.join(temp_directory, "sample6.fastq.gz"), "R2": None, "S": None},
     }
 
     assert parse_samples_to_dictionary(create_sample_tsv) == tsv_dictionary
 
     # Test parsing an invalid file or directory
     invalid_path = os.path.join(temp_directory, "nonexistent_file.tsv")
     with pytest.raises(ValueError):
@@ -206,30 +233,34 @@
     with pytest.raises(ValueError):
         parse_samples_to_dictionary(invalid_tsv_file)
 
 
 def test_write_samples_tsv(temp_directory):
     samples_dictionary = {
         "sample1": {"R1": os.path.join(temp_directory, "sample1_R1.fastq"), "R2": os.path.join(temp_directory, "sample1_R2.fastq")},
-        "sample2": {"R1": os.path.join(temp_directory, "sample2_R1_001.fastq.gz"), "R2": os.path.join(temp_directory, "sample2_R2_001.fastq.gz")},
+        "sample2": {"R1": os.path.join(temp_directory, "sample2_R1_001.fastq.gz"),
+                    "R2": os.path.join(temp_directory, "sample2_R2_001.fastq.gz"),
+                    "S": os.path.join(temp_directory, "sample2_S_001.fastq.gz")},
         "sample3": {"R1": os.path.join(temp_directory, "sample3.fastq"), "R2": None},
         "sample4_R2": {"R1": os.path.join(temp_directory, "sample4_R2.fastq"), "R2": None},
         "sample5": {"R1": os.path.join(temp_directory, "sample5.fasta.gz"), "R2": None},
         "sample6": {"R1": os.path.join(temp_directory, "sample6.fastq.gz"), "R2": None},
     }
 
     output_file = os.path.join(temp_directory, "output.tsv")
     write_samples_tsv(samples_dictionary, output_file)
 
     with open(output_file, "r") as file:
         content = file.read()
 
     expected_content = (
         "sample1\t" + os.path.join(temp_directory, "sample1_R1.fastq") + "\t" + os.path.join(temp_directory, "sample1_R2.fastq") + "\n"
-        "sample2\t" + os.path.join(temp_directory, "sample2_R1_001.fastq.gz") + "\t" + os.path.join(temp_directory, "sample2_R2_001.fastq.gz") + "\n"
+        "sample2\t" + os.path.join(temp_directory, "sample2_R1_001.fastq.gz") +
+        "\t" + os.path.join(temp_directory, "sample2_R2_001.fastq.gz") +
+        "\t" + os.path.join(temp_directory, "sample2_S_001.fastq.gz") + "\n"
         "sample3\t" + os.path.join(temp_directory, "sample3.fastq") + "\n"
         "sample4_R2\t" + os.path.join(temp_directory, "sample4_R2.fastq") + "\n"
         "sample5\t" + os.path.join(temp_directory, "sample5.fasta.gz") + "\n"
         "sample6\t" + os.path.join(temp_directory, "sample6.fastq.gz") + "\n"
     )
 
     assert content == expected_content
```

