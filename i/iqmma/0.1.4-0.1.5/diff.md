# Comparing `tmp/iqmma-0.1.4-py3-none-any.whl.zip` & `tmp/iqmma-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 29121 bytes, number of entries: 10
+Zip file size: 29396 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-May-01 14:29 iqmma/__init__.py
 -rw-r--r--  2.0 unx     1051 b- defN 23-May-01 14:29 iqmma/default.ini
--rw-r--r--  2.0 unx    39338 b- defN 23-May-31 13:45 iqmma/iqmma.py
--rw-r--r--  2.0 unx    42523 b- defN 23-May-31 14:09 iqmma/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-31 15:57 iqmma-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    12199 b- defN 23-May-31 15:57 iqmma-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 15:57 iqmma-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 23-May-31 15:57 iqmma-0.1.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-May-31 15:57 iqmma-0.1.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      759 b- defN 23-May-31 15:57 iqmma-0.1.4.dist-info/RECORD
-10 files, 107367 bytes uncompressed, 27841 bytes compressed:  74.1%
+-rw-r--r--  2.0 unx    39658 b- defN 23-Jul-13 21:23 iqmma/iqmma.py
+-rw-r--r--  2.0 unx    43148 b- defN 23-Jul-13 21:20 iqmma/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-13 22:12 iqmma-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12199 b- defN 23-Jul-13 22:12 iqmma-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 22:12 iqmma-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-13 22:12 iqmma-0.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-13 22:12 iqmma-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      759 b- defN 23-Jul-13 22:12 iqmma-0.1.5.dist-info/RECORD
+10 files, 108312 bytes uncompressed, 28116 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: iqmma/iqmma.py
 Comment: 
 
 Filename: iqmma/utils.py
 Comment: 
 
-Filename: iqmma-0.1.4.dist-info/LICENSE
+Filename: iqmma-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: iqmma-0.1.4.dist-info/METADATA
+Filename: iqmma-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: iqmma-0.1.4.dist-info/WHEEL
+Filename: iqmma-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: iqmma-0.1.4.dist-info/entry_points.txt
+Filename: iqmma-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: iqmma-0.1.4.dist-info/top_level.txt
+Filename: iqmma-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: iqmma-0.1.4.dist-info/RECORD
+Filename: iqmma-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iqmma/iqmma.py

```diff
@@ -95,14 +95,15 @@
     parser.add_argument('-outdiff', nargs='?', help='name of diffacto output file (important: .txt)', type=str, default='diffacto_out.txt', const='diffacto_out.txt')
     parser.add_argument('-min_samples', nargs='?', help='minimum number of samples for peptide usage, -1 means that half of the given number of files would be used', type=int, default=-1, const=-1)
     
     parser.add_argument('-mbr', nargs='?', help='match between runs (1 - on, 0 - off)', type=int, default=0, const=0, choices=[0, 1])
     parser.add_argument('-pval_threshold', nargs='?', help='P-value threshold for reliable differetially expressed proteins', type=float, default=0.05, const=0.05)
     parser.add_argument('-fc_threshold', nargs='?', help='Fold change threshold for reliable differetially expressed proteins', type=float, default=2., const=2.)
     parser.add_argument('-dynamic_fc_threshold', nargs='?', help='whether to apply dynamically calculated threshold (1) or not and use static -fc_threshold (0) ', type=int, default=1, const=1, choices=[0, 1])
+    parser.add_argument('-pval_adj', nargs='?', help='P value adjustment method for multiple comparisons: Bonf - Bonferroni correction, BH - Benjamini–Hochberg procedure.', type=str, default='Bonf', const='Bonf', choices=['Bonf', 'BH'])
     
     parser.add_argument('-diffacto_args', nargs='?', help='String of additional arguments to submit into Diffacto (in command line the string should be in double quotes: \'\" \"\', in cfg file in single quotes) except: -i, -out, -samples, -min_samples; default: "-normalize median -impute_threshold 0.25" ', type=str, default='-normalize median -impute_threshold 0.25', const='')
     parser.add_argument('-dino_args', nargs='?', help='String of additional arguments to submit into Dinosaur (in command line the string should be in double quotes: \'\" \"\', in cfg file in single quotes) except: --outDir --outName; default: ""', type=str, default='', const='')
 #    parser.add_argument('-bio_args', nargs='?', help='String of additional arguments to submit into Biosaur (hole string in single quotes in command line) except: -o; default: ""', type=str, default='', const='')
     parser.add_argument('-bio2_args', nargs='?', help='String of additional arguments to submit into Biosaur2 (in command line the string should be in double quotes: \'\" \"\', in cfg file in single quotes) except: -o; default: "-hvf 1000 -minlh 3"', type=str, default='-hvf 1000 -minlh 3', const='')
     parser.add_argument('-openms_args', nargs='?', help='String of additional arguments to submit into OpenMSFeatureFinder (in command line the string should be in double quotes: \'\" \"\', in cfg file in single quotes) except: -in, -out; default: "-algorithm:isotopic_pattern:charge_low 2 -algorithm:isotopic_pattern:charge_high 7"', type=str, default='-algorithm:isotopic_pattern:charge_low 2 -algorithm:isotopic_pattern:charge_high 7', const='')
 
@@ -620,15 +621,16 @@
             save = False
             plot_venn = False
 
         num_changed_prots = generate_users_output(
             diffacto_out = paths['DiffOut'], 
             out_folder = out_directory, 
             plot_venn = plot_venn, 
-            pval_threshold = args['pval_threshold'], 
+            pval_threshold = args['pval_threshold'],
+            pval_adj=args['pval_adj'],
             fc_threshold = args['fc_threshold'], 
             dynamic_fc_threshold = args['dynamic_fc_threshold'], 
             save = save, 
             logger=logger
         )
         
         if sum(list(num_changed_prots.values())) == 0 :
@@ -684,14 +686,15 @@
                 plot_venn = True
 
             num_changed_prots = generate_users_output(
                 diffacto_out = paths['DiffOut'], 
                 out_folder = out_directory, 
                 plot_venn = plot_venn, 
                 pval_threshold = args['pval_threshold'], 
+                pval_adj=args['pval_adj'],
                 fc_threshold = args['fc_threshold'], 
                 dynamic_fc_threshold = args['dynamic_fc_threshold'], 
                 save = save, 
                 logger=logger
             )
             logger.info('Numbers of differentially expressed proteins:')
             for suf in suffixes+['mixed'] :
```

## iqmma/utils.py

```diff
@@ -128,14 +128,15 @@
 def gaus(x, a, x0, sigma):
     return a * np.exp(-(x - x0) ** 2 / (2 * sigma ** 2))
 
 def generate_users_output(diffacto_out={},
                           out_folder='',
                           plot_venn=True,
                           pval_threshold=0.05,
+                          pval_adj='Bonf',
                           fc_threshold=2,
                           dynamic_fc_threshold=True,
                           save = True, 
                           logger = logging.getLogger('function')
                           ) :
     # diffacto_out = {
     #     'suf1': path_to_diffacto_results,
@@ -158,41 +159,51 @@
             continue
         table['log2_FC'] = np.log2(table['s1']/table['s2'])
         table['FC'] = table['s1']/table['s2']
         table.sort_values('P(PECA)', ascending=True, inplace=True)
         if flag :
             comp_df = table[['Protein']]
             flag = False
-
-        bonferroni = pval_threshold/len(table)
+        if pval_adj == 'Bonf' :
+            bonferroni = pval_threshold/len(table)
+            table['pval_adj_pass'] = table['P(PECA)'] <= bonferroni
+            logger.info('Bonferroni p value correction is applied')
+        elif pval_adj == 'BH' :
+            l = len(table)
+            table['BH'] = pd.Series([(i+1)*pval_threshold/l for i in range(l)], index=table.index)
+            table['pval_adj_pass'] = table['P(PECA)'] <= table['BH']
+            logger.info('Benjamini–Hochberg p value correction procedure is applied')
+        else :
+            logger.critical('Wrong value for the `pval_adj` argument')
+            return dict([(suf, 0) for suf in suffixes])
+        
         table = table[ table['S/N'] > 0.01 ]
-        if len(table[table['P(PECA)'] > bonferroni]['log2_FC']) < 100:
+        
+        if len(table[~table['pval_adj_pass']]['log2_FC']) < 100:
             logger.info('Low number of proteins for FC dynamic threshold')
             dynamic_fc_threshold = 0
-            fc_threshold = 0.5
-    
         if not dynamic_fc_threshold :
-            table = table[table['P(PECA)'] < bonferroni][['Protein', 'P(PECA)', 'log2_FC']]
+            table = table[table['pval_adj_pass']][['Protein', 'P(PECA)', 'log2_FC']]
             logger.info('Static fold change threshold is applied')
             border_fc = fc_threshold
             table = table[abs(table['log2_FC']) > border_fc]
         else:
-            t = table[table['P(PECA)'] > bonferroni]['log2_FC'].to_numpy()
+            t = table[~table['pval_adj_pass']]['log2_FC'].to_numpy()
             t = t[~np.isnan(t)]
             w = opt_bin(t, logger=logger)
             bbins = np.arange(min(t), max(t), w)
             H2, b2 = np.histogram(t, bins=bbins)
             m, mi, s = max(H2), b2[np.argmax(H2)], (max(t) - min(t))/6
             noise = min(H2)
             popt, pcov = curve_fit(noisygaus, b2[1:], H2, p0=[m, mi, s, noise])
             shift, sigma = popt[1], abs(popt[2])
             right_fc_threshold = shift + 3*sigma
             left_fc_threshold = shift - 3*sigma
             logger.info('Dynamic fold change threshold is applied for {}: {} {}'.format(suf, left_fc_threshold, right_fc_threshold, ))
-            table = table[table['P(PECA)'] < bonferroni][['Protein', 'P(PECA)', 'log2_FC']]
+            table = table[table['pval_adj_pass']][['Protein', 'P(PECA)', 'log2_FC']]
             table = table.query('`log2_FC` >= @right_fc_threshold or `log2_FC` <= @left_fc_threshold')
         comp_df = comp_df.merge(table, how='outer', on='Protein', suffixes = (None, '_'+suf))
     comp_df.rename(columns={'log2_FC': 'log2_FC_'+suffixes[0], 'P(PECA)': 'P(PECA)_'+suffixes[0] }, inplace=True )
     comp_df.dropna(how = 'all', subset=['log2_FC_' + suf for suf in suffixes], inplace=True)
     # comp_df.loc['Total number', :] = df0.notna().sum(axis=0)
     
     total_de_prots = {}
@@ -220,15 +231,15 @@
             colors[suf] = color
         legend_elements = [
             matplotlib.lines.Line2D([0], [0], color = 'w', markerfacecolor = colors[suf], marker = 's', markersize = 10, markeredgecolor = 'k',  
                    markeredgewidth = .1, label = suf) for suf in suffixes
         ]
         ax.legend(handles = legend_elements, fontsize = 24, markerscale = 2.5)
         plt.savefig(os.path.join(out_folder, 'venn.png'))
-        # logger.info('Venn diagram created')
+        logger.info('Venn diagram created')
         
     return total_de_prots
 
 
 def diffacto_call(diffacto_path='',
                   out_path='',
                   peptide_path='',
```

## Comparing `iqmma-0.1.4.dist-info/LICENSE` & `iqmma-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `iqmma-0.1.4.dist-info/METADATA` & `iqmma-0.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqmma
-Version: 0.1.4
+Version: 0.1.5
 Summary: A MS1 feature mapping for MS2 spectra identifications.
 Author: Valeriy Postoenko & Leyla Garibova
 Author-email: pyteomics@googlegroups.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Education
```

