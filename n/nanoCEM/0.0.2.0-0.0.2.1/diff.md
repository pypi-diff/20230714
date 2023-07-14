# Comparing `tmp/nanoCEM-0.0.2.0.tar.gz` & `tmp/nanoCEM-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.2.0.tar", last modified: Tue Jul 11 11:03:33 2023, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.2.1.tar", last modified: Fri Jul 14 09:47:58 2023, max compression
```

## Comparing `nanoCEM-0.0.2.0.tar` & `nanoCEM-0.0.2.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-11 11:03:33.677532 nanoCEM-0.0.2.0/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.2.0/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9737 2023-07-11 11:03:33.677532 nanoCEM-0.0.2.0/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9154 2023-07-11 11:01:35.000000 nanoCEM-0.0.2.0/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-11 11:03:33.673532 nanoCEM-0.0.2.0/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9703 2023-07-11 10:29:09.000000 nanoCEM-0.0.2.0/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.2.0/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.2.0/nanoCEM/cem_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     8020 2023-07-11 10:29:09.000000 nanoCEM-0.0.2.0/nanoCEM/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.2.0/nanoCEM/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.2.0/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7847 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.0/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11478 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.0/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.0/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-11 11:03:33.677532 nanoCEM-0.0.2.0/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9737 2023-07-11 11:03:33.000000 nanoCEM-0.0.2.0/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-11 11:03:33.000000 nanoCEM-0.0.2.0/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-11 11:03:33.000000 nanoCEM-0.0.2.0/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-11 11:03:33.000000 nanoCEM-0.0.2.0/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-11 11:03:33.000000 nanoCEM-0.0.2.0/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-11 11:03:33.677532 nanoCEM-0.0.2.0/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1134 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.0/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-14 09:47:58.490815 nanoCEM-0.0.2.1/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.2.1/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9994 2023-07-14 09:47:58.490815 nanoCEM-0.0.2.1/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9411 2023-07-14 09:46:47.000000 nanoCEM-0.0.2.1/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-14 09:47:58.490815 nanoCEM-0.0.2.1/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9703 2023-07-14 09:46:47.000000 nanoCEM-0.0.2.1/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.2.1/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-07-14 02:30:08.000000 nanoCEM-0.0.2.1/nanoCEM/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     8110 2023-07-13 02:50:55.000000 nanoCEM-0.0.2.1/nanoCEM/current_events_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.2.1/nanoCEM/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1846 2023-07-14 09:41:28.000000 nanoCEM-0.0.2.1/nanoCEM/extract_sub_fastq_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.2.1/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7847 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.1/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11481 2023-07-11 12:11:54.000000 nanoCEM-0.0.2.1/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13880 2023-07-11 11:03:13.000000 nanoCEM-0.0.2.1/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-14 09:47:58.490815 nanoCEM-0.0.2.1/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9994 2023-07-14 09:47:58.000000 nanoCEM-0.0.2.1/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      467 2023-07-14 09:47:58.000000 nanoCEM-0.0.2.1/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-14 09:47:58.000000 nanoCEM-0.0.2.1/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      137 2023-07-14 09:47:58.000000 nanoCEM-0.0.2.1/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-14 09:47:58.000000 nanoCEM-0.0.2.1/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-14 09:47:58.490815 nanoCEM-0.0.2.1/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1201 2023-07-14 09:47:48.000000 nanoCEM-0.0.2.1/setup.py
```

### Comparing `nanoCEM-0.0.2.0/LICENSE` & `nanoCEM-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.0/PKG-INFO` & `nanoCEM-0.0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.2.0
+Version: 0.0.2.1
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,14 +38,16 @@
 --ref data/23S_rRNA.fasta \
 --rna --cpu 4 --norm
 ```
 Then you can generate the following pdf files.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
 
+## Data release
+For the data we used and related commands in our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-commands)
 ## Before start, you should know
 ### Re-squiggle
 In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
 Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
 ### Data format
 Since the release of the R10, ONT's data formats have become more diverse, including the initial fast5 format, the new pod5 format, and community-provided slow5/blow5 formats. The relationship between them and conversion tools are shown in the following figure.
@@ -55,25 +57,25 @@
 In our program, we assume that the input provided by the user is the **multi-fast5** format by default.
 ### Reference and alignment
 For RNA showcase, the expected input for the vast majority of species is a fasta file of transcripts, rather than the genome. 
 This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
 ### Base shift (only available for f5c)
 The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
 For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. 
-In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo. However, if you trust the original input, you can set the offset to **0**.
+In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo (default : **2**). However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
 ```sh
-pip install nanoCEM==0.0.1.8
+pip install nanoCEM==0.0.2.0
 ```
 
 Other tools if you needed
 ```sh
-pip install ont-fast5-api pod
-conda install -c bioconda f5c slow5tools minimap2 
+pip install ont-fast5-api pod5
+conda install -c bioconda f5c slow5tools minimap2 samtools
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
 current_events_magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
@@ -115,24 +117,25 @@
   --strand STRAND       Strand of your interest (default:+)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 
                         Turn on the RNA mode
   --base_shift BASE_SHIFT
-                        base shift if required (default:0)
+                        base shift if required (default:2)
   --norm                Turn on the normalization
 ```
 ## Quick start
 ### 1. Run Basecaller and alignment on your ONT data
 ```sh
 # assumed your fast5 file folder name is fast5/ and reference is reference.fasta
+# q 30 is recommended but you can try other filter in your data
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
-minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 16 -o file.bam
+minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 -q 30 - | samtools sort -@ 16 -o file.bam
 samtools index file.bam
 ```
 Option ```-c``` means config file ,which will depend on your data
 ### 2. Decide the chrom or transcript name and region of your interest
 In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1 and I am intereted in A2030 on the plus strand.
 So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
 ### 3. Subsample (Optional)
@@ -199,8 +202,7 @@
 --base_shift 2 --rna --norm
 ```
 
 
 
 
 
-
```

### Comparing `nanoCEM-0.0.2.0/README.md` & `nanoCEM-0.0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 --ref data/23S_rRNA.fasta \
 --rna --cpu 4 --norm
 ```
 Then you can generate the following pdf files.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
 
+## Data release
+For the data we used and related commands in our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-commands)
 ## Before start, you should know
 ### Re-squiggle
 In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
 Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
 ### Data format
 Since the release of the R10, ONT's data formats have become more diverse, including the initial fast5 format, the new pod5 format, and community-provided slow5/blow5 formats. The relationship between them and conversion tools are shown in the following figure.
@@ -41,25 +43,25 @@
 In our program, we assume that the input provided by the user is the **multi-fast5** format by default.
 ### Reference and alignment
 For RNA showcase, the expected input for the vast majority of species is a fasta file of transcripts, rather than the genome. 
 This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
 ### Base shift (only available for f5c)
 The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
 For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. 
-In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo. However, if you trust the original input, you can set the offset to **0**.
+In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo (default : **2**). However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
 ```sh
-pip install nanoCEM==0.0.1.8
+pip install nanoCEM==0.0.2.0
 ```
 
 Other tools if you needed
 ```sh
-pip install ont-fast5-api pod
-conda install -c bioconda f5c slow5tools minimap2 
+pip install ont-fast5-api pod5
+conda install -c bioconda f5c slow5tools minimap2 samtools
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
 current_events_magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
@@ -101,24 +103,25 @@
   --strand STRAND       Strand of your interest (default:+)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 
                         Turn on the RNA mode
   --base_shift BASE_SHIFT
-                        base shift if required (default:0)
+                        base shift if required (default:2)
   --norm                Turn on the normalization
 ```
 ## Quick start
 ### 1. Run Basecaller and alignment on your ONT data
 ```sh
 # assumed your fast5 file folder name is fast5/ and reference is reference.fasta
+# q 30 is recommended but you can try other filter in your data
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
-minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 16 -o file.bam
+minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 -q 30 - | samtools sort -@ 16 -o file.bam
 samtools index file.bam
 ```
 Option ```-c``` means config file ,which will depend on your data
 ### 2. Decide the chrom or transcript name and region of your interest
 In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1 and I am intereted in A2030 on the plus strand.
 So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
 ### 3. Subsample (Optional)
@@ -185,8 +188,7 @@
 --base_shift 2 --rna --norm
 ```
 
 
 
 
 
-
```

### Comparing `nanoCEM-0.0.2.0/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.2.1/nanoCEM/CE_magnifier_test.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.0/nanoCEM/cem_utils.py` & `nanoCEM-0.0.2.1/nanoCEM/cem_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     reverse_fasta = list(reversed(''.join(ref)))
     return ''.join(reverse_fasta)
 
 def save_fasta_dict(fasta_dict,path):
     f=open(path,'w+')
     for key,value in fasta_dict.items():
         f.write('>'+key+'\n')
-        line = len(value) //70 + 1
+        line = len(value) //80 + 1
         for i in range(0, line):
-            f.write(value[i*70:(i+1)*70]+'\n')
+            f.write(value[i*80:(i+1)*80]+'\n')
         f.close()
 # fasta=read_fasta_to_dic("/data/Ecoli_23s/23S_rRNA.fasta")
 # for key,value in fasta.items():
 #     fasta[key]=reverse_fasta(value)
 # save_fasta_dict(fasta,'test.fasta')
```

### Comparing `nanoCEM-0.0.2.0/nanoCEM/current_events_magnifier.py` & `nanoCEM-0.0.2.1/nanoCEM/current_events_magnifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,27 +30,28 @@
                         help='The attribute group to extract the training data from. e.g. RawGenomeCorrected_000')
     parser_tombo.add_argument('--basecall_subgroup', default='BaseCalled_template',
                         help='Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template')
     parser_tombo.add_argument('-i', "--input_fast5", required=True,
                         help="input_fast5_file")
     parser_tombo.add_argument('-c', "--control_fast5",
                         help="control_fast5_file")
+    # parser_tombo.add_argument('-b', "--bam", help="bam file to help index to speed up")
     parser_tombo.add_argument('-o', "--output", default="tombo_result", help="output_file")
     parser_tombo.add_argument('-t', "--cpu", default=4, type=int, help="num of process")
     add_public_argument(parser_tombo)
 
     # f5c subparser
     parser_f5c = subparsers.add_parser('f5c', help='tackle f5c re-squiggle')
     parser_f5c.add_argument("-i", "--input", required=True,
                         help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
                         help="control_blow5_path")
     parser_f5c.add_argument('-o', "--output", default="f5c_result", help="output_file")
 
-    parser_f5c.add_argument('--base_shift',type=int, default=0, help="output_file")
+    parser_f5c.add_argument('--base_shift',type=int, default=2, help="output_file")
     add_public_argument(parser_f5c)
     return parser
 
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
```

### Comparing `nanoCEM-0.0.2.0/nanoCEM/extract_sub_fast5_from_bam.py` & `nanoCEM-0.0.2.1/nanoCEM/extract_sub_fast5_from_bam.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.0/nanoCEM/normalization.py` & `nanoCEM-0.0.2.1/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.0/nanoCEM/plot.py` & `nanoCEM-0.0.2.1/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.0/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.2.1/nanoCEM/read_f5c_resquiggle.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,19 +167,19 @@
 
 
 
 def read_blow5(path,position,length,chromo,strand,subsapmle_num=500,base_shift=2,norm=True):
     global info_dict,s5,pbar
     bam_file = path+".bam"
     if not os.path.exists(path+'.bam'):
-        raise RuntimeError(path+'.bam' +"is not exist in your path!")
+        raise RuntimeError(path+'.bam ' +"is not exist in your path!")
     if not os.path.exists(path+'.paf'):
-        raise RuntimeError(path+'.paf' +"is not exist in your path!")
+        raise RuntimeError(path+'.paf ' +"is not exist in your path!")
     if not os.path.exists(path+'.blow5'):
-        raise RuntimeError(path+'.blow5' +"is not exist in your path!")
+        raise RuntimeError(path+'.blow5 ' +"is not exist in your path!")
     bam_file=pysam.AlignmentFile(bam_file,'rb')
     # if rna_mode:
     #     if strand =='+':
     #         position=position+ (kmer_model-1)
     #     else:
     #         position=position- (kmer_model-1)
     info_dict=extract_pairs_pos(bam_file,position,length,chromo,strand)
```

### Comparing `nanoCEM-0.0.2.0/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.2.1/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.2.0/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.2.1/nanoCEM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.2.0
+Version: 0.0.2.1
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle program(tombo and f5c).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,14 +38,16 @@
 --ref data/23S_rRNA.fasta \
 --rna --cpu 4 --norm
 ```
 Then you can generate the following pdf files.
 ![alt text](example/boxplot.png)
 ![alt text](example/violin.png)
 
+## Data release
+For the data we used and related commands in our paper, please view our [wiki](https://github.com/lrslab/nanoCEM/wiki/Data-release-and-commands)
 ## Before start, you should know
 ### Re-squiggle
 In ONT technology, "resquiggle" refers to the process of converting the raw electrical signals from the sequencer into corresponding DNA/RNA sequence information, which is then corrected and realigned. 
 This process utilizes the signal features of ONT sequencing, such as changes in electrical resistance and noisy signals, to capture information from the DNA/RNA sequence and analyze and interpret it. 
 Although new basecaller program (Guppy/Boinito/Dorado) generated the bam file with move table to record the event index,but  resquiggle is a more fine alignment than the move table in most cases.
 ### Data format
 Since the release of the R10, ONT's data formats have become more diverse, including the initial fast5 format, the new pod5 format, and community-provided slow5/blow5 formats. The relationship between them and conversion tools are shown in the following figure.
@@ -55,25 +57,25 @@
 In our program, we assume that the input provided by the user is the **multi-fast5** format by default.
 ### Reference and alignment
 For RNA showcase, the expected input for the vast majority of species is a fasta file of transcripts, rather than the genome. 
 This is because RNA undergoes splicing and other phenomena after transcription, allowing a single gene to produce multiple different transcripts with varying splicing forms and exon compositions.
 ### Base shift (only available for f5c)
 The mechanism of tombo and f5c is different, f5c applied a k-mer model, which means base should satisfy at least 4 bases before it.
 For example, in CTAT**G**, f5c will only return the last **G**'s current event.So, compared to tombo, there is always an offset in the results of f5c. 
-In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo. However, if you trust the original input, you can set the offset to **0**.
+In order to make the results of the two methods comparable and draw similar conclusions, we recommend using an offset of **2** maintained a distance no greater than **1** base compared with Tombo (default : **2**). However, if you trust the original input, you can set the offset to **0**.
 ## Installation
 Requirement : Python >=3.7, <3.10
 ```sh
-pip install nanoCEM==0.0.1.8
+pip install nanoCEM==0.0.2.0
 ```
 
 Other tools if you needed
 ```sh
-pip install ont-fast5-api pod
-conda install -c bioconda f5c slow5tools minimap2 
+pip install ont-fast5-api pod5
+conda install -c bioconda f5c slow5tools minimap2 samtools
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
 current_events_magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
@@ -115,24 +117,25 @@
   --strand STRAND       Strand of your interest (default:+)
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 
                         Turn on the RNA mode
   --base_shift BASE_SHIFT
-                        base shift if required (default:0)
+                        base shift if required (default:2)
   --norm                Turn on the normalization
 ```
 ## Quick start
 ### 1. Run Basecaller and alignment on your ONT data
 ```sh
 # assumed your fast5 file folder name is fast5/ and reference is reference.fasta
+# q 30 is recommended but you can try other filter in your data
 guppy_basecaller -i fast5/ -s ./guppy_out --recursive --device auto -c rna_r9.4.1_70bps_hac.cfg  &
 cat guppy_out/*/*.fastq > all.fastq
-minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 - | samtools sort -@ 16 -o file.bam
+minimap2 -ax map-ont -t 16 --MD reference.fasta all.fastq | samtools view -hbS -F 260 -q 30 - | samtools sort -@ 16 -o file.bam
 samtools index file.bam
 ```
 Option ```-c``` means config file ,which will depend on your data
 ### 2. Decide the chrom or transcript name and region of your interest
 In this sample, I plot the 23s rRNA whose header in fasta file is NR_103073.1 and I am intereted in A2030 on the plus strand.
 So for the following command , I used ```--chrom NR_103073.1  --pos 2030 --strand +```.
 ### 3. Subsample (Optional)
@@ -199,8 +202,7 @@
 --base_shift 2 --rna --norm
 ```
 
 
 
 
 
-
```

### Comparing `nanoCEM-0.0.2.0/setup.py` & `nanoCEM-0.0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.2.0",
+    version="0.0.2.1",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle program(tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/nanoCEM",
@@ -24,11 +24,12 @@
         'h5py==3.8.0',
         'numpy>=1.23.0',
         'pandas>=1.1.5',
         'plotnine>=0.8.0',
         'tqdm>=4.62.0',
         "pysam>=0.21.0",
         "pyslow5>=1.0.0",
-        "vbz_h5py_plugin>=1.0.1"
+        "vbz_h5py_plugin>=1.0.1",
+        "biopython>=1.80"
     ],
-    scripts=['nanoCEM/current_events_magnifier.py','nanoCEM/extract_sub_fast5_from_bam.py']
+    scripts=['nanoCEM/current_events_magnifier.py','nanoCEM/extract_sub_fast5_from_bam.py','nanoCEM/extract_sub_fastq_from_bam.py']
 )
```

