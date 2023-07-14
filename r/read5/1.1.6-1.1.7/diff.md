# Comparing `tmp/read5-1.1.6.tar.gz` & `tmp/read5-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read5-1.1.6.tar", last modified: Wed Jul 12 21:34:07 2023, max compression
+gzip compressed data, was "read5-1.1.7.tar", last modified: Fri Jul 14 19:03:11 2023, max compression
```

## Comparing `read5-1.1.6.tar` & `read5-1.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 21:34:07.435057 read5-1.1.6/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    35149 2023-04-26 15:37:10.000000 read5-1.1.6/LICENSE
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       22 2023-04-26 15:39:17.000000 read5-1.1.6/MANIFEST.in
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2328 2023-07-12 21:34:07.435057 read5-1.1.6/PKG-INFO
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     3382 2023-07-12 21:30:22.000000 read5-1.1.6/README.md
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     1459 2023-07-12 13:09:27.000000 read5-1.1.6/README.rst
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 21:34:07.451057 read5-1.1.6/read5/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    20135 2023-07-12 12:37:48.000000 read5-1.1.6/read5/AbstractFileReader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      773 2023-07-12 15:11:37.000000 read5-1.1.6/read5/Exceptions.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    13183 2023-07-12 12:39:21.000000 read5-1.1.6/read5/Fast5Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    11653 2023-07-12 12:38:39.000000 read5-1.1.6/read5/Pod5Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      980 2023-07-12 12:52:52.000000 read5-1.1.6/read5/Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     8605 2023-07-12 12:39:08.000000 read5-1.1.6/read5/Slow5Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      148 2023-07-12 12:47:33.000000 read5-1.1.6/read5/__init__.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      497 2023-07-12 21:34:07.451057 read5-1.1.6/read5/_version.py
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 21:34:07.415057 read5-1.1.6/read5.egg-info/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2328 2023-07-12 21:34:07.000000 read5-1.1.6/read5.egg-info/PKG-INFO
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      404 2023-07-12 21:34:07.000000 read5-1.1.6/read5.egg-info/SOURCES.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        1 2023-07-12 21:34:07.000000 read5-1.1.6/read5.egg-info/dependency_links.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       88 2023-07-12 21:34:07.000000 read5-1.1.6/read5.egg-info/requires.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        6 2023-07-12 21:34:07.000000 read5-1.1.6/read5.egg-info/top_level.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      208 2023-07-12 21:34:07.443057 read5-1.1.6/setup.cfg
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     1519 2023-07-12 21:25:01.000000 read5-1.1.6/setup.py
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-12 21:34:07.423057 read5-1.1.6/tests/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    54377 2023-07-12 12:51:42.000000 read5-1.1.6/tests/test_FileReader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    68611 2023-04-26 15:39:17.000000 read5-1.1.6/versioneer.py
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-14 19:03:11.315812 read5-1.1.7/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    35149 2023-04-26 15:37:10.000000 read5-1.1.7/LICENSE
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       22 2023-04-26 15:39:17.000000 read5-1.1.7/MANIFEST.in
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     3377 2023-07-14 19:03:11.319812 read5-1.1.7/PKG-INFO
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     3541 2023-07-14 12:49:29.000000 read5-1.1.7/README.md
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2509 2023-07-12 22:00:39.000000 read5-1.1.7/README.rst
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-14 19:03:11.335812 read5-1.1.7/read5/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    20283 2023-07-14 12:44:04.000000 read5-1.1.7/read5/AbstractFileReader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      773 2023-07-12 15:11:37.000000 read5-1.1.7/read5/Exceptions.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    13183 2023-07-14 12:47:54.000000 read5-1.1.7/read5/Fast5Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    11653 2023-07-12 12:38:39.000000 read5-1.1.7/read5/Pod5Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      980 2023-07-12 12:52:52.000000 read5-1.1.7/read5/Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     8605 2023-07-12 12:39:08.000000 read5-1.1.7/read5/Slow5Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      148 2023-07-13 08:25:24.000000 read5-1.1.7/read5/__init__.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      497 2023-07-14 19:03:11.335812 read5-1.1.7/read5/_version.py
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-14 19:03:11.295812 read5-1.1.7/read5.egg-info/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     3377 2023-07-14 19:03:10.000000 read5-1.1.7/read5.egg-info/PKG-INFO
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      404 2023-07-14 19:03:11.000000 read5-1.1.7/read5.egg-info/SOURCES.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        1 2023-07-14 19:03:11.000000 read5-1.1.7/read5.egg-info/dependency_links.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       88 2023-07-14 19:03:11.000000 read5-1.1.7/read5.egg-info/requires.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        6 2023-07-14 19:03:11.000000 read5-1.1.7/read5.egg-info/top_level.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      208 2023-07-14 19:03:11.327812 read5-1.1.7/setup.cfg
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     1519 2023-07-12 21:25:01.000000 read5-1.1.7/setup.py
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-14 19:03:11.307812 read5-1.1.7/tests/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    54377 2023-07-12 12:51:42.000000 read5-1.1.7/tests/test_FileReader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    68611 2023-04-26 15:39:17.000000 read5-1.1.7/versioneer.py
```

### Comparing `read5-1.1.6/LICENSE` & `read5-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `read5-1.1.6/PKG-INFO` & `read5-1.1.7/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,52 @@
-Metadata-Version: 2.1
-Name: read5
-Version: 1.1.6
-Summary: Wrapper to read fast5, slow5, blow5 and pod5 files.
-Home-page: https://github.com/JannesSP/read5
-Author: Jannes Spangenberg
-Author-email: jannes.spangenberg@uni-jena.de
-License: GNU General Public License v3
-Keywords: read5,slow5,blow5,fast5,pod5,ONT,Oxford Nanopore Technologies,Nanopore,raw data,wrapper
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-License-File: LICENSE
-
 Installation
 ------------
 
-Pod5 is not available via conda (27.06.2023). Read5 Currently available
-via pipy.
+Pypi/pip
+~~~~~~~~
 
 .. code:: bash
 
    pip install read5
 
+Conda
+~~~~~
+
+Pod5 is currently not available via conda (27.06.2023). Please install
+it using pip in your conda environment.
+
+.. code:: bash
+
+   conda install mamba
+   mamba create -n read5 -c jannessp read5
+   conda activate read5
+   pip install pod5 # needed as no pod5 conda package available yet
+
+Alternatively you can create the environment using the
+`conda.recipe/env.yml <conda.recipe/env.yml>`__ file.
+
+.. code:: bash
+
+   conda install mamba
+   mamba env create -f conda.recipe/env.yml
+   conda activate read5
+
 --------------
 
 Usage
 -----
 
 `Click here to see a full documentation about the classes and
 function. <https://jannessp.github.io/read5.github.io/>`__
 
 *my_file* can be a fast5, slow5, blow5 or pod5 file. The wrapper detects
 the file format depending on the file extension.
 
 Small example:
+~~~~~~~~~~~~~~
 
 .. code:: python
 
    from read5 import read # or from read5.Reader import read
 
    r5 = read(my_file) # file with on of these extensions: .fast5, .slow5, .blow5, .pod5
    for readid in r5:
@@ -51,21 +54,43 @@
        norm_signal = r5.getZNormSignal(readid) # returns normalised read signal: norm_signal = (signal - median(signal)) / mad(signal)
        channel = r5.getChannelNumber(readid)
        sampleid = r5.getSampleID(readid)
        runid = r5.getSampleID(readid)
 
    readid_list = r5.getReads()
 
+File Reader Classes
+~~~~~~~~~~~~~~~~~~~
+
 If you want to use the file readers you can import the corresponding
 class like this:
 
 .. code:: python
 
    from read5.Fast5Reader import Fast5Reader # contains the Fast5 Reader class
    from read5.Slow5Reader import Slow5Reader # contains the Slow5 Reader class
    from read5.Pod5Reader import Pod5Reader # contains the Pod5 Reader class
 
+Abstract File Reader Class
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   from read5.AbstractFileReader import AbstractFileReader
+
+Possible Exceptions
+~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   from read5.Exceptions import UnknownFileFormatException, UnknownNormalizationMode
+
+-  UnknownFileFormatException: is raised, when the file extension does
+   not match one of [‘.fast5’, ‘.slow5’, ‘.blow5’, ‘pod5’]
+-  UnknownNormalizationMode: is raised, when an unknown mode is provided
+   for the signal normalization function
+
 Full Documentation
 ------------------
 
 Created with `pdoc3 <https://pdoc3.github.io/pdoc/>`__. Can be found
 `here <https://jannessp.github.io/read5.github.io/>`__.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `read5-1.1.6/README.md` & `read5-1.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ![Alt text](figures/logo.png)
 
 Read5 is a python wrapper to read fast5, slow5/blow5 and pod5 files using the same overloaded functions from different APIs.
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-teal.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/read5)
 
-[![PyPI version](https://badge.fury.io/py/read5.svg)](https://badge.fury.io/py/read5) ![PyPI - Downloads](https://img.shields.io/pypi/dm/read5) ![PyPI - Status](https://img.shields.io/pypi/status/read5)
+![PyPI](https://img.shields.io/pypi/v/read5) ![PyPI - Downloads](https://img.shields.io/pypi/dm/read5) ![PyPI - Status](https://img.shields.io/pypi/status/read5)
 
 
 [![Anaconda-Server Badge](https://anaconda.org/jannessp/read5/badges/version.svg)](https://anaconda.org/jannessp/read5) ![Conda](https://img.shields.io/conda/dn/jannessp/read5) [![Conda package](https://anaconda.org/jannessp/read5/badges/latest_release_date.svg)](https://anaconda.org/jannessp/read5) [![Conda package](https://anaconda.org/jannessp/read5/badges/platforms.svg)](https://anaconda.org/jannessp/read5)
  
 [![DOI](https://zenodo.org/badge/633012569.svg)](https://zenodo.org/badge/latestdoi/633012569)
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/Ja_Spangenberg)](https://twitter.com/Ja_Spangenberg)
@@ -29,14 +29,20 @@
 Pod5 is currently not available via conda (27.06.2023). Please install it using pip in your conda environment.
 ```bash
 conda install mamba
 mamba create -n read5 -c jannessp read5
 conda activate read5
 pip install pod5 # needed as no pod5 conda package available yet
 ```
+Alternatively you can create the environment using the [conda.recipe/env.yml](conda.recipe/env.yml) file.
+```bash
+conda install mamba
+mamba env create -f conda.recipe/env.yml
+conda activate read5
+```
 ___
 ## Usage
 
 [Click here to see a full documentation about the classes and function.](https://jannessp.github.io/read5.github.io/)
 
 *my_file* can be a fast5, slow5, blow5 or pod5 file. The wrapper detects the file format depending on the file extension.
```

### Comparing `read5-1.1.6/read5/AbstractFileReader.py` & `read5-1.1.7/read5/AbstractFileReader.py`

 * *Files 0% similar despite different names*

```diff
@@ -979,8 +979,16 @@
         readid : str
 
         Returns
         -------
         startTime : int
             start of sequencing converted to minutes after sequencing start
         '''
-        return self.getStartTime(readid) / self.getSamplingRate(readid) / 60
+        return self.getStartTime(readid) / self.getSamplingRate(readid) / 60
+    
+    def getFilePath(self) -> str:
+        '''
+        Returns
+        -------
+        filepath : str
+        '''
+        return self._filepath
```

### Comparing `read5-1.1.6/read5/Exceptions.py` & `read5-1.1.7/read5/Exceptions.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.6/read5/Fast5Reader.py` & `read5-1.1.7/read5/Fast5Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.6/read5/Pod5Reader.py` & `read5-1.1.7/read5/Pod5Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.6/read5/Reader.py` & `read5-1.1.7/read5/Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.6/read5/Slow5Reader.py` & `read5-1.1.7/read5/Slow5Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.6/read5.egg-info/PKG-INFO` & `read5-1.1.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: read5
-Version: 1.1.6
+Version: 1.1.7
 Summary: Wrapper to read fast5, slow5, blow5 and pod5 files.
 Home-page: https://github.com/JannesSP/read5
 Author: Jannes Spangenberg
 Author-email: jannes.spangenberg@uni-jena.de
 License: GNU General Public License v3
 Keywords: read5,slow5,blow5,fast5,pod5,ONT,Oxford Nanopore Technologies,Nanopore,raw data,wrapper
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,33 +17,56 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE
 
 Installation
 ------------
 
-Pod5 is not available via conda (27.06.2023). Read5 Currently available
-via pipy.
+Pypi/pip
+~~~~~~~~
 
 .. code:: bash
 
    pip install read5
 
+Conda
+~~~~~
+
+Pod5 is currently not available via conda (27.06.2023). Please install
+it using pip in your conda environment.
+
+.. code:: bash
+
+   conda install mamba
+   mamba create -n read5 -c jannessp read5
+   conda activate read5
+   pip install pod5 # needed as no pod5 conda package available yet
+
+Alternatively you can create the environment using the
+`conda.recipe/env.yml <conda.recipe/env.yml>`__ file.
+
+.. code:: bash
+
+   conda install mamba
+   mamba env create -f conda.recipe/env.yml
+   conda activate read5
+
 --------------
 
 Usage
 -----
 
 `Click here to see a full documentation about the classes and
 function. <https://jannessp.github.io/read5.github.io/>`__
 
 *my_file* can be a fast5, slow5, blow5 or pod5 file. The wrapper detects
 the file format depending on the file extension.
 
 Small example:
+~~~~~~~~~~~~~~
 
 .. code:: python
 
    from read5 import read # or from read5.Reader import read
 
    r5 = read(my_file) # file with on of these extensions: .fast5, .slow5, .blow5, .pod5
    for readid in r5:
@@ -51,21 +74,43 @@
        norm_signal = r5.getZNormSignal(readid) # returns normalised read signal: norm_signal = (signal - median(signal)) / mad(signal)
        channel = r5.getChannelNumber(readid)
        sampleid = r5.getSampleID(readid)
        runid = r5.getSampleID(readid)
 
    readid_list = r5.getReads()
 
+File Reader Classes
+~~~~~~~~~~~~~~~~~~~
+
 If you want to use the file readers you can import the corresponding
 class like this:
 
 .. code:: python
 
    from read5.Fast5Reader import Fast5Reader # contains the Fast5 Reader class
    from read5.Slow5Reader import Slow5Reader # contains the Slow5 Reader class
    from read5.Pod5Reader import Pod5Reader # contains the Pod5 Reader class
 
+Abstract File Reader Class
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   from read5.AbstractFileReader import AbstractFileReader
+
+Possible Exceptions
+~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   from read5.Exceptions import UnknownFileFormatException, UnknownNormalizationMode
+
+-  UnknownFileFormatException: is raised, when the file extension does
+   not match one of [‘.fast5’, ‘.slow5’, ‘.blow5’, ‘pod5’]
+-  UnknownNormalizationMode: is raised, when an unknown mode is provided
+   for the signal normalization function
+
 Full Documentation
 ------------------
 
 Created with `pdoc3 <https://pdoc3.github.io/pdoc/>`__. Can be found
 `here <https://jannessp.github.io/read5.github.io/>`__.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `read5-1.1.6/setup.py` & `read5-1.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.6/tests/test_FileReader.py` & `read5-1.1.7/tests/test_FileReader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.6/versioneer.py` & `read5-1.1.7/versioneer.py`

 * *Files identical despite different names*

