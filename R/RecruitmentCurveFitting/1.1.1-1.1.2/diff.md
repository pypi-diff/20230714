# Comparing `tmp/RecruitmentCurveFitting-1.1.1-py2.py3-none-any.whl.zip` & `tmp/RecruitmentCurveFitting-1.1.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 106314 bytes, number of entries: 12
+Zip file size: 106350 bytes, number of entries: 12
 -rw-r--r--  2.0 unx    35821 b- defN 23-May-27 05:45 RecruitmentCurveFitting/COPYING
 -rw-r--r--  2.0 unx    18750 b- defN 23-May-30 15:02 RecruitmentCurveFitting/CurveFitting.py
--rw-r--r--  2.0 unx    28502 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting/RecruitmentCurves.py
--rw-r--r--  2.0 unx     4110 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting/__init__.py
+-rw-r--r--  2.0 unx    28640 b- defN 23-Jul-14 16:53 RecruitmentCurveFitting/RecruitmentCurves.py
+-rw-r--r--  2.0 unx     4252 b- defN 23-Jul-14 16:53 RecruitmentCurveFitting/__init__.py
 -rw-r--r--  2.0 unx     7820 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting/__main__.py
 -rw-r--r--  2.0 unx     1491 b- defN 23-May-27 02:43 RecruitmentCurveFitting/example-data1.txt
 -rw-r--r--  2.0 unx     2291 b- defN 23-May-27 02:24 RecruitmentCurveFitting/example-data2.txt
 -rw-r--r--  2.0 unx   208425 b- defN 23-May-27 02:24 RecruitmentCurveFitting/example-waveforms.csv
--rw-r--r--  2.0 unx     2559 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting-1.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1135 b- defN 23-Jun-29 18:00 RecruitmentCurveFitting-1.1.1.dist-info/RECORD
-12 files, 311038 bytes uncompressed, 104374 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx     2529 b- defN 23-Jul-14 16:53 RecruitmentCurveFitting-1.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-14 16:53 RecruitmentCurveFitting-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jul-14 16:53 RecruitmentCurveFitting-1.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1135 b- defN 23-Jul-14 16:53 RecruitmentCurveFitting-1.1.2.dist-info/RECORD
+12 files, 311288 bytes uncompressed, 104410 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: RecruitmentCurveFitting/example-data2.txt
 Comment: 
 
 Filename: RecruitmentCurveFitting/example-waveforms.csv
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.1.1.dist-info/METADATA
+Filename: RecruitmentCurveFitting-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.1.1.dist-info/WHEEL
+Filename: RecruitmentCurveFitting-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.1.1.dist-info/top_level.txt
+Filename: RecruitmentCurveFitting-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: RecruitmentCurveFitting-1.1.1.dist-info/RECORD
+Filename: RecruitmentCurveFitting-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## RecruitmentCurveFitting/RecruitmentCurves.py

```diff
@@ -46,27 +46,31 @@
 
     hMaxStim, hMax = hFit.Find( 'max' )
     mMax = mFit.uHeight.finalValue
     mThresholdStim = mFit.Backward( 0.1, scaled=False )
 
     mFit.Plot( markX=mThresholdStim, markY=mMax )
     hFit.Plot( markX=hMaxStim, markY=hMax, hold=True)
+    
+    import matplotlib.pyplot as plt; plt.show()  # if necessary
 
 This module also contains a higher-level class, `RecruitmentCurve`, which
 you construct using an array of EMG time-series, and use to extract both
 `m` and `h` magnitudes and fit them, given their start and end points in
 milliseconds::
     
     from RecruitmentCurveFitting import RecruitmentCurve, UnpackExamples
 
     UnpackExamples() # writes assorted example files to the current directory
 
     z = RecruitmentCurve('example-waveforms.csv') # that's one of the files
     z.Fit( boundsM=[8.1, 15.9], boundsH=[34.6, 42.4] )
     z.Plot() # try hovering the mouse pointer over each data-point, it's fun
+    
+    import matplotlib.pyplot as plt; plt.show()  # if necessary
 	
 This module can also be run as a standalone command-line utility. Input files
 should be formatted as comma- or space-delimited numeric tables where the last
 three columns are stimulation intensity, M-wave size and H-reflex size. Prior
 columns, if present, are used to separate different conditions from each other
 (each condition generates one pair of curve fits, and one figure if requested)
 Column headings are optional. For example::
```

## RecruitmentCurveFitting/__init__.py

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 
 # $BEGIN_RECRUITMENTCURVEFITTING_LICENSE$
 # 
 # This file is part of the RecruitmentCurveFitting project, a Python
 # package for fitting sigmoid and bell-shaped functions to EMG
 # recruitment-curve measurements.
 # 
@@ -36,35 +36,38 @@
 If you use this software in your research, your report should cite the article
 in which this approach was introduced, as follows:
 
 - McKinnon ML, Hill NJ, Carp JS, Dellenbach B & Thompson AK (2023).
   Methods for automated delineation and assessment of EMG responses evoked by
   peripheral nerve stimulation in diagnostic and closed-loop therapeutic
   applications.
-  @JOURNAL@ @NUMBER@(@VOLUME@):@PAGES@
-  @DOI@
+  Journal of Neural Engineering (in press)
+  https://doi.org/10.1088/1741-2552/ace6fb
     
 The corresponding BibTeX entry is::
 
     @article{mckinnonhill2023,
       author  = {McKinnon, Michael L. and Hill, N. Jeremy and Carp, Jonathan S.
                  and Dellenbach, Blair and Thompson, Aiko K.},
       title   = {Methods for Automated Delineation and Assessment of {EMG}
                  Responses Evoked by Peripheral Nerve Stimulation in Diagnostic
                  and Closed-Loop Therapeutic Applications},
-      journal = {TBD},
+      journal = {Journal of Neural Engineering},
+      year    = {2023},
+      doi     = {10.1088/1741-2552/ace6fb},
+      url     = {https://doi.org/10.1088/1741-2552/ace6fb},
+    }
+"""
+
+"""
+      month   = {TBD},
+      date    = {2023-TBD-TBD},
       volume  = {TBD},
       number  = {TBD},
       pages   = {TBD--TBD},
-      month   = {TBD},
-      year    = {2023},
-      date    = {2023-TBD-TBD},
-      doi     = {TBD/TBD},
-      url     = {https://doi.org/TBD/TBD},
-    }
 """
 
 def Cite( command=None, prefix='', stream=None ):
 	"""
 =============================================================================
 This is the RecruitmentCurveFitting package version @VERSION@ by Jeremy Hill,
 running in Python @PYVERSION@.
@@ -90,16 +93,17 @@
 		try: stream.flush()
 		except: pass
 Cite.__doc__ = Cite.__doc__.replace( '@VERSION@', __version__ ).replace( '@PYVERSION@', '%s.%s' % ( sys.version_info.major, sys.version_info.minor ) ).replace( '@CITATION_INFO@', CITATION_INFO.strip() )
 hooks = [ lambda: ( 
 	( Preferences().get( 'nag', True ) and Cite( stream=sys.stderr, prefix='# ' ) ),
 	hooks.pop( 0 )
 ) ]
-#from . import CurveFitting; CurveFitting.Curve._Curve__hooks = hooks
-# TODO: uncomment the line above when the citation info is finalized, to arm the nag message
+from . import CurveFitting; CurveFitting.Curve._Curve__hooks = hooks # comment out to disarm the nag message
+# uncomment the line above when the citation info is finalized, to arm the nag message
+
 def Preferences( **kwargs ):
 	prefsFile = os.path.expanduser( '~/.' + __name__ )
 	try: prefs = ast.literal_eval( open( prefsFile, 'rt' ).read() )
 	except: prefs = {}
 	if kwargs:
 		prefs.update( kwargs )
 		prefsText = '{\n' + ''.join( '\t%r : %r,\n' % item for item in prefs.items() ) + '}\n'
```

## Comparing `RecruitmentCurveFitting-1.1.1.dist-info/METADATA` & `RecruitmentCurveFitting-1.1.2.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RecruitmentCurveFitting
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package for fitting sigmoid and bell-shaped functions to EMG recruitment-curve measurements
 Home-page: UNKNOWN
 Author: Jeremy Hill
 Author-email: jezhill@gmail.com
 License: GPL v3+
 Platform: UNKNOWN
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, <4
@@ -37,31 +37,26 @@
 If you use this software in your research, your report should cite the article
 in which this approach was introduced, as follows:
 
 - McKinnon ML, Hill NJ, Carp JS, Dellenbach B & Thompson AK (2023).
   Methods for automated delineation and assessment of EMG responses evoked by
   peripheral nerve stimulation in diagnostic and closed-loop therapeutic
   applications.
-  @JOURNAL@ @NUMBER@(@VOLUME@):@PAGES@
-  @DOI@
+  Journal of Neural Engineering (in press)
+  https://doi.org/10.1088/1741-2552/ace6fb
     
 The corresponding BibTeX entry is::
 
     @article{mckinnonhill2023,
       author  = {McKinnon, Michael L. and Hill, N. Jeremy and Carp, Jonathan S.
                  and Dellenbach, Blair and Thompson, Aiko K.},
       title   = {Methods for Automated Delineation and Assessment of {EMG}
                  Responses Evoked by Peripheral Nerve Stimulation in Diagnostic
                  and Closed-Loop Therapeutic Applications},
-      journal = {TBD},
-      volume  = {TBD},
-      number  = {TBD},
-      pages   = {TBD--TBD},
-      month   = {TBD},
+      journal = {Journal of Neural Engineering},
       year    = {2023},
-      date    = {2023-TBD-TBD},
-      doi     = {TBD/TBD},
-      url     = {https://doi.org/TBD/TBD},
+      doi     = {10.1088/1741-2552/ace6fb},
+      url     = {https://doi.org/10.1088/1741-2552/ace6fb},
     }
```

## Comparing `RecruitmentCurveFitting-1.1.1.dist-info/RECORD` & `RecruitmentCurveFitting-1.1.2.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 RecruitmentCurveFitting/COPYING,sha256=Czg9WmPaZE9ijZnDOXbqZIftiaqlnwsyV5kt6sEXHms,35821
 RecruitmentCurveFitting/CurveFitting.py,sha256=80RF2UuoP9KUl-pydCIwa_FHD9k8-J7OFvefHWRfL2A,18750
-RecruitmentCurveFitting/RecruitmentCurves.py,sha256=UPeHS19jOlkMuvKRp8sMT_5zyEXE5KONCznWG-QWLmg,28502
-RecruitmentCurveFitting/__init__.py,sha256=Tb-5fhd6Rpicm1qs9l3eoe6jj0IH7UiG3HjeDDTpeGc,4110
+RecruitmentCurveFitting/RecruitmentCurves.py,sha256=dLMjlYzPga1Fk02dUcmg5HLCwKZ8YXKy3U39LC1_HRk,28640
+RecruitmentCurveFitting/__init__.py,sha256=UcN47a5WENmUknrgfFhy3bV-XCbiFtfNyMvtxYqjx8w,4252
 RecruitmentCurveFitting/__main__.py,sha256=515xY1F8yjh3qF-hpvkFFMnAbFcDeKSTJWkrL3XEhUE,7820
 RecruitmentCurveFitting/example-data1.txt,sha256=FeaYwnAMGemLQKM9Kj1IPi_3fey7gyY9SLOJYttZcXc,1491
 RecruitmentCurveFitting/example-data2.txt,sha256=SBv6zHDxt1YOhylfZSMMHSCsDNwL1brHpTgAdH8esvg,2291
 RecruitmentCurveFitting/example-waveforms.csv,sha256=eWF7HtChJAv5uHfiQ1Pg__l-d9eYKtGWr8PlYp7-kis,208425
-RecruitmentCurveFitting-1.1.1.dist-info/METADATA,sha256=beBgHI4rbQ0tD68qxbAkmujUdELSWrigafelDoPUBMs,2559
-RecruitmentCurveFitting-1.1.1.dist-info/WHEEL,sha256=h_aVn5OB2IERUjMbi2pucmR_zzWJtk303YXvhh60NJ8,110
-RecruitmentCurveFitting-1.1.1.dist-info/top_level.txt,sha256=GaYHShtnr9zJ_unau13fDnezLMr3kyCH0-KQN_Go6WM,24
-RecruitmentCurveFitting-1.1.1.dist-info/RECORD,,
+RecruitmentCurveFitting-1.1.2.dist-info/METADATA,sha256=twgs6DgNW0HihY7erMvIfQv-_dUEcX2-W_Tpm5vwJmg,2529
+RecruitmentCurveFitting-1.1.2.dist-info/WHEEL,sha256=h_aVn5OB2IERUjMbi2pucmR_zzWJtk303YXvhh60NJ8,110
+RecruitmentCurveFitting-1.1.2.dist-info/top_level.txt,sha256=GaYHShtnr9zJ_unau13fDnezLMr3kyCH0-KQN_Go6WM,24
+RecruitmentCurveFitting-1.1.2.dist-info/RECORD,,
```

