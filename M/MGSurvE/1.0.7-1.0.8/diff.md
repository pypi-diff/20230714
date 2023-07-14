# Comparing `tmp/MGSurvE-1.0.7.tar.gz` & `tmp/MGSurvE-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MGSurvE-1.0.7.tar", last modified: Fri Jul 14 17:13:33 2023, max compression
+gzip compressed data, was "MGSurvE-1.0.8.tar", last modified: Fri Jul 14 19:45:38 2023, max compression
```

## Comparing `MGSurvE-1.0.7.tar` & `MGSurvE-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-14 17:13:33.666114 MGSurvE-1.0.7/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/LICENSE
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-14 17:13:33.665049 MGSurvE-1.0.7/MGSurvE/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/MGSurvE/__init__.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-07-14 17:13:33.000000 MGSurvE-1.0.7/MGSurvE/_version.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/MGSurvE/auxiliary.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      605 2023-06-01 22:38:54.000000 MGSurvE-1.0.7/MGSurvE/colors.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-06-29 19:56:26.000000 MGSurvE-1.0.7/MGSurvE/constants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     7191 2023-06-08 23:51:28.000000 MGSurvE-1.0.7/MGSurvE/kernels.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21887 2023-07-14 17:12:03.000000 MGSurvE-1.0.7/MGSurvE/landscape.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/MGSurvE/matrices.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/MGSurvE/network.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    45037 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/MGSurvE/optimization.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-06-26 18:35:57.000000 MGSurvE-1.0.7/MGSurvE/optimizationPSO.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18240 2023-07-12 17:23:30.000000 MGSurvE-1.0.7/MGSurvE/plots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-05-11 16:34:41.000000 MGSurvE-1.0.7/MGSurvE/pointProcess.py
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-14 17:13:33.665789 MGSurvE-1.0.7/MGSurvE.egg-info/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-07-14 17:13:33.000000 MGSurvE-1.0.7/MGSurvE.egg-info/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-07-14 17:13:33.000000 MGSurvE-1.0.7/MGSurvE.egg-info/SOURCES.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-07-14 17:13:33.000000 MGSurvE-1.0.7/MGSurvE.egg-info/dependency_links.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      231 2023-07-14 17:13:33.000000 MGSurvE-1.0.7/MGSurvE.egg-info/requires.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-07-14 17:13:33.000000 MGSurvE-1.0.7/MGSurvE.egg-info/top_level.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-07-14 17:13:33.665986 MGSurvE-1.0.7/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4172 2023-06-29 18:04:52.000000 MGSurvE-1.0.7/README.md
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-07-14 17:13:33.666159 MGSurvE-1.0.7/setup.cfg
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1441 2023-06-28 20:50:45.000000 MGSurvE-1.0.7/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-14 19:45:38.332280 MGSurvE-1.0.8/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 16:34:41.000000 MGSurvE-1.0.8/LICENSE
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-14 19:45:38.331108 MGSurvE-1.0.8/MGSurvE/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      275 2023-05-11 16:34:41.000000 MGSurvE-1.0.8/MGSurvE/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-07-14 19:45:38.000000 MGSurvE-1.0.8/MGSurvE/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6881 2023-05-11 16:34:41.000000 MGSurvE-1.0.8/MGSurvE/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      605 2023-06-01 22:38:54.000000 MGSurvE-1.0.8/MGSurvE/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1665 2023-06-29 19:56:26.000000 MGSurvE-1.0.8/MGSurvE/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     7191 2023-06-08 23:51:28.000000 MGSurvE-1.0.8/MGSurvE/kernels.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    21887 2023-07-14 17:12:03.000000 MGSurvE-1.0.8/MGSurvE/landscape.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4924 2023-05-11 16:34:41.000000 MGSurvE-1.0.8/MGSurvE/matrices.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1358 2023-05-11 16:34:41.000000 MGSurvE-1.0.8/MGSurvE/network.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    48723 2023-07-14 18:52:09.000000 MGSurvE-1.0.8/MGSurvE/optimization.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     9200 2023-06-26 18:35:57.000000 MGSurvE-1.0.8/MGSurvE/optimizationPSO.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    18819 2023-07-14 17:50:13.000000 MGSurvE-1.0.8/MGSurvE/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6849 2023-05-11 16:34:41.000000 MGSurvE-1.0.8/MGSurvE/pointProcess.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-14 19:45:38.331930 MGSurvE-1.0.8/MGSurvE.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-07-14 19:45:38.000000 MGSurvE-1.0.8/MGSurvE.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      451 2023-07-14 19:45:38.000000 MGSurvE-1.0.8/MGSurvE.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-07-14 19:45:38.000000 MGSurvE-1.0.8/MGSurvE.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      231 2023-07-14 19:45:38.000000 MGSurvE-1.0.8/MGSurvE.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        8 2023-07-14 19:45:38.000000 MGSurvE-1.0.8/MGSurvE.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4604 2023-07-14 19:45:38.332131 MGSurvE-1.0.8/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4172 2023-06-29 18:04:52.000000 MGSurvE-1.0.8/README.md
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-07-14 19:45:38.332340 MGSurvE-1.0.8/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1441 2023-06-28 20:50:45.000000 MGSurvE-1.0.8/setup.py
```

### Comparing `MGSurvE-1.0.7/LICENSE` & `MGSurvE-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.7/MGSurvE/auxiliary.py` & `MGSurvE-1.0.8/MGSurvE/auxiliary.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.7/MGSurvE/colors.py` & `MGSurvE-1.0.8/MGSurvE/colors.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.7/MGSurvE/constants.py` & `MGSurvE-1.0.8/MGSurvE/constants.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.7/MGSurvE/kernels.py` & `MGSurvE-1.0.8/MGSurvE/kernels.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.7/MGSurvE/landscape.py` & `MGSurvE-1.0.8/MGSurvE/landscape.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.7/MGSurvE/matrices.py` & `MGSurvE-1.0.8/MGSurvE/matrices.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.7/MGSurvE/network.py` & `MGSurvE-1.0.8/MGSurvE/network.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.7/MGSurvE/optimization.py` & `MGSurvE-1.0.8/MGSurvE/optimization.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,17 +86,28 @@
     Q = tau[:sitesN, :sitesN]
     R = tau[:sitesN, -trapsN:]
     I = np.identity(Q.shape[0])
     F = np.linalg.pinv(np.subtract(I, Q), rcond=rcond)
     return F
 
 def getFundamentalVector(tau, sitesN):
-    # Equivalent to:
-    #   np.sum(srv.getFundamentalMatrix(tau, sitesN, trapsN), axis=1)
-    #   np.sum(srv.getFundamentalMatrixPseudoInverse(tau, sitesN, trapsN), axis=1)
+    """ Get Markov's fundamental vector.
+    
+    Equivalent to:
+      np.sum(srv.getFundamentalMatrix(tau, sitesN, trapsN), axis=1)
+      np.sum(srv.getFundamentalMatrixPseudoInverse(tau, sitesN, trapsN), axis=1)
+
+    Parameters:
+        tau (numpy array): Traps migration matrix in canonical form.
+        sitesN (int): Number of sites.
+
+    Returns:
+        (numpy array): Time to fall into absorbing states from anywhere in landscape.
+    """
+
     Q = tau[:sitesN, :sitesN]
     I = np.identity(Q.shape[0])
     o = np.ones(Q.shape[0])
     F = np.linalg.solve(I-Q, o)
     return F
 
 def getFundamentalFitness(
@@ -141,14 +152,24 @@
     Q = tau[:sitesN, :sitesN]
     R = tau[:sitesN, -trapsN:]
     I = np.identity(Q.shape[0])
     return {'Q': Q, 'R': R, 'I': I}
 
 
 def getMeanTimeToCapture(canonElems, pseudoInv=True, rcond=1e-20):
+    """Calculates the average time to capture given the Q, R, I Markov canonical elements.
+
+    Args:
+        canonElems (dict): Dictionary containing the Q, R, and I matrices as calculated by Markov's fundamental matrix.
+        pseudoInv (bool, optional): Boolean to choose either normal matrix inverse or matrix pseudo-inverse. Defaults to True.
+        rcond (_type_, optional): Limit condation for floating precision on pseudo-inverse. Defaults to 1e-20.
+
+    Returns:
+        float: Mean time to capture.
+    """    
     (Q, R, I) = [canonElems[d] for d in ('Q', 'R', 'I')]
     # Get fundamental matrix
     if pseudoInv:
         N = np.linalg.pinv(np.subtract(I, Q), rcond=rcond)
     else:
         N = np.linalg.inv(np.subtract(I, Q))
     # Calculate mean time to capture
@@ -157,14 +178,23 @@
 
 
 def getTimeToCapture(
         landscape, 
         fitFuns={'outer': np.sum}, 
         pseudoInv=True, rcond=1e-10
     ):
+    """Wrapper function for 'getMeanTimeToCapture' given a landscape.
+
+    Args:
+        landscappe (object): Landscape object
+        fitFuns (dict): Dictionary containing the outer function for summarize.
+
+    Returns:
+        float: Mean time to capture.
+    """ 
     canonElems = getCanonicalElements(
         landscape.trapsMigration,
         landscape.pointNumber, 
         landscape.trapsNumber
     )
     t = getMeanTimeToCapture(canonElems, pseudoInv=pseudoInv, rcond=rcond)
     fit = fitFuns['outer'](t)
@@ -370,14 +400,24 @@
             offB[ix] = ind1[ix]
     (ind1[:], ind2[:]) = (offA[:], offB[:])
     return (ind1, ind2)
 ###############################################################################
 # GA (Extended)
 ###############################################################################
 def mutShuffleIndexes(individual, typeOptimMask, indpb=.5):
+    """Shuffles allele indices in pairs.
+
+    Args:
+        individual (list): Chromosome for optimization
+        typeOptimMask (bool numpy array): Array of bools that define which alleles can be mutated (1).
+        indpb (float, optional): Mutation probability for each independent allele. Defaults to 0.5.
+
+    Returns:
+        list: Mutated chromosome
+    """    
     (size, clen) = (len(typeOptimMask), len(individual))
     for i in range(size):
         # If the allele can be mutated and was sampled
         if (typeOptimMask[i]):
             if (random.random() < indpb):
                 swap_indx = random.randint(0, clen-2)
                 if swap_indx >= i:
@@ -396,14 +436,27 @@
 
 def initChromosomeMixed(
         trapsCoords, 
         fixedTrapsMask, typeOptimMask,
         coordsRange, trapsPool, 
         indpb=.75
     ):
+    """Generates a compound chromosome for optimization with a coordinates-type composition (currently unusued).
+
+    Args:
+        trapsCoords (numpy array): Current traps positions.
+        fxdTrpsMsk (bool numpy array): Array of bools that define which alleles can be mutated (1). 
+        typeOptimMask (bool numpy array): Array of bools that define which alleles can be mutated (1).
+        coordsRange (numpy array): Allowed trap coordinates for init.
+        trapsPool (integers array): Types of traps available in the pool.
+        indpb (float, optional): Allele mutation probability. Defaults to .75.
+
+    Returns:
+        list: Randomly-generated chromosome.
+    """    
     coordSect = initChromosome(trapsCoords, fixedTrapsMask, coordsRange)
     typesInit = mutShuffleIndexes(trapsPool, typeOptimMask, indpb)[0]
     return [float(i) for i in coordSect]+list(typesInit)
 
 def mutateChromosomeMixed(
         chromosome,
         fixedTrapsMask, typeOptimMask,
@@ -413,14 +466,28 @@
             'indpb': 0.5
         },
         mutTypeFun=mutShuffleIndexes,
         mutTypeArgs={
             'indpb': 0.5
         }
     ):
+    """Generates a compound chromosome for optimization with a coordinates-type composition (currently unusued).
+
+    Args:
+        trapsCoords (numpy array): Current traps positions.
+        fxdTrpsMsk (bool numpy array): Array of bools that define which alleles can be mutated (1). 
+        typeOptimMask (bool numpy array): Array of bools that define which alleles can be mutated (1).
+        mutCoordFun (function): Coordinates mutation function.
+        mutCoordArgs (dictionary): Coordinates mutation function's arguments.
+        mutTypeFun (function): Trap types mutation function.
+        mutTypeArgs (dictionary): Trap types mutation function's arguments.
+
+    Returns:
+        list: Mutated chromosome.
+    """    
     # Split chromosome in parts -----------------------------------------------
     (coordsSect, typesSect) = (
         chromosome[:len(fixedTrapsMask)], 
         chromosome[len(fixedTrapsMask):]
     )
     # Mutate coordinates section ----------------------------------------------
     coordsMut = mutCoordFun(coordsSect, fixedTrapsMask,**mutCoordArgs)[0]
@@ -476,14 +543,23 @@
     )     
     daysTillTrapped = getFundamentalFitness(funMat, fitFuns=fitFuns)
     return daysTillTrapped
 
 def getDaysTillTrappedVector(
         landscape, fitFuns={'outer': np.mean, 'inner': None}
     ):
+    """Gets the number of timesteps until a walker falls into a trap in vector form.
+
+    Parameters:
+        landscape (object): Landscape object to use for the analysis.
+        fitFuns (dict): Dictionary with the outer (row) and inner (col) functions to use on the matrix.
+
+    Returns:
+        (float): Number of days for mosquitoes to fall into traps given the fitFuns.
+    """
     funVct = getFundamentalVector(
         landscape.trapsMigration, 
         landscape.pointNumber
     )   
     daysTillTrapped = getFundamentalFitness(funVct, fitFuns=fitFuns)
     return daysTillTrapped
 
@@ -561,14 +637,24 @@
         abs(optimFunction(lnd, fitFuns=optimFunctionArgs)) for lnd in 
         (landscapeMale, landscapeFemale)
     ]
     fitVal = (fit[0]*weightMale+fit[1]*weightFemale)/(2*(weightMale+weightFemale))
     return (fitVal, )
 
 def chromosomeIDtoXY(chromosome, ptsID, pointCoords):
+    """Converts a sites-ID crhomosome into a set of XY or lon-lat coordinates.
+
+    Parameters:
+        chromosome (list): Discrete optimization chromosome.
+        ptsID (list): Set of IDs for the sites (usually lnd.pointID).
+        pointCoords (numpy array): Set of coordinates for matching points IDs (usually lnd.pointCoords)
+        
+    Returns:
+        (numpy array): Traps positions xy or lon-lat pairs as defined by the selected sites IDs.
+    """    
     siteIndex = [ptsID.index(i) for i in chromosome]
     trapXY = np.asarray([pointCoords[i] for i in siteIndex])
     return trapXY
 
 def calcDiscreteFitness(
         chromosome, landscape,
         optimFunction=getDaysTillTrapped,
```

### Comparing `MGSurvE-1.0.7/MGSurvE/optimizationPSO.py` & `MGSurvE-1.0.8/MGSurvE/optimizationPSO.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.7/MGSurvE/plots.py` & `MGSurvE-1.0.8/MGSurvE/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''Data-Visualization functions (thanks to Elijah Bartolome in the impelemntation of some of the visualization functions).
+'''Data-Visualization functions (thanks to Elijah Bartolome in the implementation of some of the visualization functions).
 
 '''
 
 import warnings
 import matplotlib
 from os import path
 from math import log
@@ -477,17 +477,30 @@
         **kwargs
     )
     return (fig, ax)
 
 
 def plotTrapsKernels(
         fig, ax, lnd,
-        colors=cst.TRP_COLS, maxSca=5, alpha=.75,
+        colors=cst.TRP_COLS, alpha=.75,
         distRange=(0, 100), aspect=.3
     ):
+    """ Creates a distance-attractiveness plot for kernels present in the landscape.
+
+    Parameters:
+        fig (matplotlib): Matplotlib fig object.
+        ax (matplotlib): Matplotlib ax object.
+        colors (list of hex): List of colors to be used in the kernel profiles.
+        alpha (float): Opacity for the traces.
+        distRange (tuple): Distances range for the x-axis.
+        aspect (float): Aspect ratio for the axes.
+    
+    Returns:
+        (fig, ax): Matplotlib (fig, ax) tuple.
+    """ 
     kers = lnd.trapsKernels
     ktypes = list(lnd.trapsKernels.keys())
     # dMax = max(max([kers[i]['radii'] for i in range(len(kers))])) * maxSca
     dMax = distRange[1]
     # Generate figure
     for i in range(len(kers)):
         ker = kers[i]
@@ -497,15 +510,17 @@
     ax.set_xlim(0, dMax)
     ax.set_ylim(0, 1)
     ax.set_aspect(aspect/ax.get_data_ratio())
     return (fig, ax)
 
 
 def plotsClearMemory():
-    # https://stackoverflow.com/questions/28757348/how-to-clear-memory-completely-of-all-matplotlib-plots
+    """ Forces matplotlib to clear all memory (probably an overkill).
+        https://stackoverflow.com/questions/28757348/how-to-clear-memory-completely-of-all-matplotlib-plots
+    """
     allfignums = matplotlib.pyplot.get_fignums()
     for i in allfignums:
         fig = matplotlib.pyplot.figure(i)
         fig.clear()
         matplotlib.pyplot.close(fig)
```

### Comparing `MGSurvE-1.0.7/MGSurvE/pointProcess.py` & `MGSurvE-1.0.8/MGSurvE/pointProcess.py`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.7/MGSurvE.egg-info/PKG-INFO` & `MGSurvE-1.0.8/MGSurvE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 1.0.7
+Version: 1.0.8
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-1.0.7/PKG-INFO` & `MGSurvE-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGSurvE
-Version: 1.0.7
+Version: 1.0.8
 Summary: MGSurvE
 Home-page: https://github.com/Chipdelmal/MGSurvE
 Author: Hector M. Sanchez C.
 Author-email: sanchez.hmsc@berkeley.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `MGSurvE-1.0.7/README.md` & `MGSurvE-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `MGSurvE-1.0.7/setup.py` & `MGSurvE-1.0.8/setup.py`

 * *Files identical despite different names*

