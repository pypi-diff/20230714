# Comparing `tmp/LineDetect-0.1.tar.gz` & `tmp/LineDetect-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LineDetect-0.1.tar", last modified: Mon Apr  3 01:10:52 2023, max compression
+gzip compressed data, was "LineDetect-0.11.tar", last modified: Fri Jul 14 03:34:51 2023, max compression
```

## Comparing `LineDetect-0.1.tar` & `LineDetect-0.11.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-03 01:10:52.668841 LineDetect-0.1/
--rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2023-04-02 22:08:01.000000 LineDetect-0.1/LICENSE.txt
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-03 01:10:52.666245 LineDetect-0.1/LineDetect/
--rwxr-xr-x   0 daniel     (501) staff       (20)       26 2023-04-02 22:08:01.000000 LineDetect-0.1/LineDetect/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    43581 2023-04-02 23:24:03.000000 LineDetect-0.1/LineDetect/continuum_finder.py
--rw-r--r--   0 daniel     (501) staff       (20)    22101 2023-04-02 22:08:01.000000 LineDetect-0.1/LineDetect/feature_finder.py
--rw-r--r--   0 daniel     (501) staff       (20)    16061 2023-04-03 01:01:39.000000 LineDetect-0.1/LineDetect/spectra_processor.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-04-03 01:10:52.668219 LineDetect-0.1/LineDetect.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      595 2023-04-03 01:10:52.000000 LineDetect-0.1/LineDetect.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      341 2023-04-03 01:10:52.000000 LineDetect-0.1/LineDetect.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-04-03 01:10:52.000000 LineDetect-0.1/LineDetect.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)       47 2023-04-03 01:10:52.000000 LineDetect-0.1/LineDetect.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)       11 2023-04-03 01:10:52.000000 LineDetect-0.1/LineDetect.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)       50 2023-04-02 22:08:01.000000 LineDetect-0.1/MANIFEST.in
--rw-r--r--   0 daniel     (501) staff       (20)      595 2023-04-03 01:10:52.668563 LineDetect-0.1/PKG-INFO
--rwxr-xr-x   0 daniel     (501) staff       (20)      752 2023-04-02 22:08:01.000000 LineDetect-0.1/README.md
--rw-r--r--   0 daniel     (501) staff       (20)      191 2023-04-02 22:08:01.000000 LineDetect-0.1/pyproject.toml
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-04-03 01:10:52.668929 LineDetect-0.1/setup.cfg
--rwxr-xr-x   0 daniel     (501) staff       (20)      935 2023-04-03 01:09:44.000000 LineDetect-0.1/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-14 03:34:51.157514 LineDetect-0.11/
+-rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2023-04-26 22:34:10.000000 LineDetect-0.11/LICENSE.txt
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-14 03:34:51.153717 LineDetect-0.11/LineDetect/
+-rwxr-xr-x   0 daniel     (501) staff       (20)       26 2023-04-26 22:34:10.000000 LineDetect-0.11/LineDetect/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    17960 2023-07-12 21:07:12.000000 LineDetect-0.11/LineDetect/continuum_finder.py
+-rw-r--r--   0 daniel     (501) staff       (20)     9405 2023-07-12 21:49:35.000000 LineDetect-0.11/LineDetect/detect_elements.py
+-rw-r--r--   0 daniel     (501) staff       (20)    14157 2023-07-12 22:26:41.000000 LineDetect-0.11/LineDetect/feature_finder.py
+-rw-r--r--   0 daniel     (501) staff       (20)    15368 2023-07-14 03:28:13.000000 LineDetect-0.11/LineDetect/spectra_processor.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-07-14 03:34:51.155995 LineDetect-0.11/LineDetect.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      596 2023-07-14 03:34:51.000000 LineDetect-0.11/LineDetect.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      371 2023-07-14 03:34:51.000000 LineDetect-0.11/LineDetect.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-07-14 03:34:51.000000 LineDetect-0.11/LineDetect.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       53 2023-07-14 03:34:51.000000 LineDetect-0.11/LineDetect.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       11 2023-07-14 03:34:51.000000 LineDetect-0.11/LineDetect.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       50 2023-04-26 22:34:10.000000 LineDetect-0.11/MANIFEST.in
+-rw-r--r--   0 daniel     (501) staff       (20)      596 2023-07-14 03:34:51.157047 LineDetect-0.11/PKG-INFO
+-rwxr-xr-x   0 daniel     (501) staff       (20)      634 2023-04-26 22:34:10.000000 LineDetect-0.11/README.md
+-rw-r--r--   0 daniel     (501) staff       (20)      207 2023-07-11 22:59:14.000000 LineDetect-0.11/pyproject.toml
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-07-14 03:34:51.157655 LineDetect-0.11/setup.cfg
+-rwxr-xr-x   0 daniel     (501) staff       (20)      945 2023-07-11 22:59:38.000000 LineDetect-0.11/setup.py
```

### Comparing `LineDetect-0.1/LICENSE.txt` & `LineDetect-0.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LineDetect-0.1/LineDetect/spectra_processor.py` & `LineDetect-0.11/LineDetect/spectra_processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,68 +12,68 @@
 from operator import itemgetter
 import matplotlib.pyplot as plt  ## To plot the spectrum
 
 from astropy.io import fits  ## To read the spectrum and load the wavelengths and flux into arrays
 from astropy.wcs import WCS
 from progress.bar import FillingSquaresBar
 
-from LineDetect.continuum_finder import apertureEW, MgII, Continuum
+from LineDetect.continuum_finder import Continuum
+from LineDetect.detect_elements import MgII 
 
 class Spectrum:
     """
     A class for processing spectral data stored in FITS files.
 
     Can process either a set of .fits files or single spectra.
 
     Note:
         If the line is detected the spectrum features will be added
         to the DataFrame `df` attribute, which will always append new detections. 
         If no line is detected then nothing will be added to the DataFrame,
         but a message with the object name will print.
 
     Args:
-        line (str): The line to detect when running the procedure. Options include: 'MgII' or 'CaIV'. Defaults to 'MgII'.
-        method (str): The method to apply when estimating the continuum, options include: 'median', 'savgol',
-            gaussian', or 'butter'. Defaults to 'median'       
         halfWindow (int, list, np.ndarray): The half-size of the window/kernel (in Angstroms) used to compute the continuum. 
             If this is a list/array of integers, then the continuum will be calculated
             as the median curve across the fits across all half-window sizes in the list/array.
             Defaults to 25.
         poly_order (int): The order of the polynomial used for smoothing the spectrum.
         resolution_range (tuple): A tuple of the minimum and maximum resolution (in km/s) used to detect MgII absorption.
+            Can also be an integer or a float.
         directory (str): The path to the directory containing the FITS files. Defaults to None.
         save_all (bool): Parameter to control whether to save the non-detections. If the spectral feature is not detected 
             and save_all=True, the qso_name will be appended alongside 'None' entries. Defaults to False to save only positive detections.
 
     Methods:
         process_files(): Process the FITS files in the directory.
         process_spectrum(Lambda, y, sig_y, z, file_name): Process a single instance of spectral data.
         _reprocess(): Re-runs the process_spectrum method using the saved spectrum attributes.
         plot(include, errorbar, xlim, ylim, xlog, ylog, savefig): Plots the spectrum and/or continuum.
         find_MgII_absorption(Lambda, y, yC, sig_y, sig_yC, z, qso_name): Find the MgII lines, if present.
-        find_CaIV_absorption(Lambda, y, yC, sig_y, sig_yC, z, qso_name): Find the CaIV lines, if present.
+        find_CIV_absorption(Lambda, y, yC, sig_y, sig_yC, z, qso_name): Find the CIV lines, if present.
     """
 
-
-    def __init__(self, line='MgII', method='median', halfWindow=25, poly_order=2, resolution_range=(1400, 1700), directory=None, save_all=True):
-        self.line = line 
-        self.method = method
+    def __init__(self, halfWindow=25, resolution_range=(1400, 1700), 
+        resolution_element=3, N_sig_1=5, N_sig_2=3, rest_wavelength_1=2796.35,
+        rest_wavelength_2=2803.53, directory=None, save_all=False):
+        
         self.halfWindow = halfWindow
-        self.poly_order = poly_order 
         self.resolution_range = resolution_range
+        self.resolution_element = resolution_element
+        self.N_sig_1 = N_sig_1
+        self.N_sig_2 = N_sig_2
+        self.rest_wavelength_1 = rest_wavelength_1
+        self.rest_wavelength_2 = rest_wavelength_2
+
         self.directory = directory
         self.save_all = save_all
 
         #Declare a dataframe to hold the info
         self.df = pd.DataFrame(columns=['QSO', 'Wavelength', 'z', 'W', 'deltaW']) 
 
-        valid_options = ['MgII', 'CaIV']
-        if self.line not in valid_options:
-            raise ValueError('Invalid line input! Current options include: {}'.format(valid_options))
-
     def process_files(self):
         """
         Processes each FITS file in the directory, detecting any Mg II absorption that may be present.
 
         The method iterates through each FITS file in the directory specified during initialization, 
         reads in the spectrum data and associated header information, applies continuum normalization, 
         identifies Mg II absorption features, and calculates the equivalent widths of said absorptions.
@@ -104,29 +104,30 @@
                 w = WCS(hdu[0].header, naxis=1, relax=False, fix=False)
                 Lambda = w.wcs_pix2world(np.arange(len(flux)), 0)[0]
 
                 #Cut the spectrum blueward of the LyAlpha line
                 z = hdu[0].header['Z'] #Redshift
                 #Cut the spectrum blueward of the LyAlpha line
                 Lya = (1 + z) * 1216 + 20 #Lya Line at 121.6 nm
-                mask = (Lambda > Lya) 
+                mask1 = (Lambda > Lya) 
+                rest_frame = (1 + z) * rest_wavelength_1
+                mask2 = (Lambda[mask1] < rest_frame)
+
+                mask = mask1[mask2]
                 Lambda, flux, flux_err = Lambda[mask], flux[mask], flux_err[mask]
                 
                 try:
                     #Generate the contiuum
-                    continuum = Continuum(Lambda, flux, flux_err, method=self.method, halfWindow=self.halfWindow, poly_order=self.poly_order)
-                    continuum.estimate(fit_legendre=True)
+                    continuum = Continuum(Lambda, flux, flux_err, halfWindow=self.halfWindow, N_sig=self.N_sig_2, resolution_element=self.resolution_element)
+                    continuum.estimate()
                 except ValueError: #This will catch the failed to fit message!
                     print(); print('Failed to fit the continuum, skipping file: {}'.format(file))
                     progress_bar.next(); continue
                 #Find the MgII Absorption
-                if self.line == 'MgII':
-                    self.find_MgII_absorption(Lambda, flux, continuum.continuum, flux_err, continuum.continuum_err, z=z, qso_name=file)
-                elif self.line == 'CaIV':
-                    self.find_CaIV_absorption(Lambda, flux, continuum.continuum, flux_err, continuum.continuum_err, z=z, qso_name=file)
+                self.find_MgII_absorption(Lambda, flux, continuum.continuum, flux_err, continuum.continuum_err, z=z, qso_name=file)
                 
                 progress_bar.next()
 
         progress_bar.finish()
 
         return 
 
@@ -146,27 +147,27 @@
             None
         """
 
         qso_name = 'No_Name' if qso_name is None else qso_name
 
         #Cut the spectrum blueward of the LyAlpha line
         Lya = (1 + z) * 1216 + 20 #Lya Line at 121.6 nm
-        mask = (Lambda > Lya) 
+        rest_frame = (1 + z) * self.rest_wavelength_1
+        mask = np.where((Lambda > Lya)&(Lambda < rest_frame))
+        
         Lambda, flux, flux_err = Lambda[mask], flux[mask], flux_err[mask]
-  
+        
         #Generate the contiuum
-        continuum = Continuum(Lambda, flux, flux_err, method=self.method, halfWindow=self.halfWindow, poly_order=self.poly_order)
-        continuum.estimate(fit_legendre=True)
+        continuum = Continuum(Lambda, flux, flux_err, halfWindow=self.halfWindow, N_sig=self.N_sig_2, resolution_element=self.resolution_element)
+        continuum.estimate()
         #Save the continuum attributes
         self.continuum, self.continuum_err = continuum.continuum, continuum.continuum_err
+
         #Find the MgII Absorption
-        if self.line == 'MgII':
-            self.find_MgII_absorption(Lambda, flux, self.continuum, flux_err, self.continuum_err, z=z, qso_name=qso_name)
-        elif self.line == 'CaIV':
-            self.find_CaIV_absorption(Lambda, flux, self.continuum, flux_err, self.continuum_err, z=z, qso_name=qso_name)
+        self.find_MgII_absorption(Lambda, flux, self.continuum, flux_err, self.continuum_err, z=z, qso_name=qso_name)
                 
         self.Lambda, self.flux, self.flux_err, self.z, self.qso_name = Lambda, flux, flux_err, z, qso_name #For plotting
 
         return
 
     def _reprocess(self, qso_name=None):
         """
@@ -187,35 +188,34 @@
 
         #Cut the spectrum blueward of the LyAlpha line
         Lya = (1 + self.z) * 1216 + 20 #Lya Line at 121.6 nm
         mask = (self.Lambda > Lya) 
         self.Lambda, self.flux, self.flux_err = self.Lambda[mask], self.flux[mask], self.flux_err[mask]
   
         #Generate the contiuum
-        continuum = Continuum(self.Lambda, self.flux, self.flux_err, method=self.method, halfWindow=self.halfWindow, poly_order=self.poly_order)
-        continuum.estimate(fit_legendre=True)
+        continuum = Continuum(self.Lambda, self.flux, self.flux_err, halfWindow=self.halfWindow, N_sig=self.N_sig_2, resolution_element=self.resolution_element)
+        continuum.estimate()
         #Save the continuum attributes
         self.continuum, self.continuum_err = continuum.continuum, continuum.continuum_err
         #Find the MgII Absorption
-        if self.line == 'MgII':
-            self.find_MgII_absorption(self.Lambda, self.flux, self.continuum, self.flux_err, self.continuum_err, z=self.z, qso_name=self.qso_name)
-        elif self.line == 'CaIV':
-            self.find_CaIV_absorption(self.Lambda, self.flux, self.continuum, self.flux_err, self.continuum_err, z=self.z, qso_name=self.qso_name)
-           
+        self.find_MgII_absorption(self.Lambda, self.flux, self.continuum, self.flux_err, self.continuum_err, z=self.z, qso_name=self.qso_name)
+        
         return 
 
-    def plot(self, include='both', errorbar=False, xlim=None, ylim=None, xlog=False, ylog=False, 
+    def plot(self, include='both', highlight=False, errorbar=False, xlim=None, ylim=None, xlog=False, ylog=False, 
         savefig=False, path=None):
         """
         Plots the spectrum and/or continuum.
     
         Args:
             include (float): Designates what to plot, options include
                 'spectrum', 'continuum', or 'both.
-            errorbar (bool): Defaults to True.
+            highlight (bool): If True then the line will be highlighted with accompanying
+                vertical lines to visualize the equivalent width. Defaults to False.
+            errorbar (bool): Whether to include the flux_err as y-errors. Defaults to False.
             xlim: Limits for the x-axis. Ex) xlim = (4000, 6000)
             ylim: Limits for the y-axis. Ex) ylim = (0.9, 0.94)
             xlog (boolean): If True the x-axis will be log-scaled.
                 Defaults to True.
             ylog (boolean): If True the y-axis will be log-scaled.
                 Defaults to False.
             savefig (bool): If True the figure will not disply but will be saved instead.
@@ -228,15 +228,15 @@
         """
 
         if self.continuum is None or self.flux is None:
             raise ValueError('This method only works after a single spectrum has been processed via the process_spectrum method.')
 
         if errorbar:
             continuum_err = self.continuum_err if include == 'continuum' or include == 'both' else None
-            flux_err = self.flux_err if include == 'sp (ectrum' or include == 'both' else None
+            flux_err = self.flux_err if include == 'spectrum' or include == 'both' else None
         else:
             flux_err = continuum_err = None
 
         if include == 'continuum' or include == 'both':
             plt.errorbar(self.Lambda, self.continuum, yerr=continuum_err, fmt='r--', linewidth=0.6, label='Continuum')
         if include == 'spectrum' or include == 'both':
             plt.errorbar(self.Lambda, self.flux, yerr=flux_err, fmt='k-.', linewidth=0.2)
@@ -244,14 +244,24 @@
         plt.title(self.qso_name, size=14)
         plt.xlabel('Wavelength [Å]', size=12); plt.ylabel('Flux', alpha=1, color='k', size=12)
         plt.xticks(fontsize=10); plt.yticks(fontsize=12)
         plt.xscale('log') if xlog else None; plt.yscale('log') if ylog else None 
         plt.xlim(xlim) if xlim is not None else None; plt.ylim(ylim) if ylim is not None else None
         plt.legend(prop={'size': 12})#, loc='upper left')
         
+        if highlight:
+            if len(self.Mg2796) == 0:
+                print('The highlight parameter is enabled but no line was detected!')
+            else:
+                for i in range(0, len(self.Mg2796) - 1, 2):
+                    plt.axvline(x = self.Lambda[self.Mg2796[i]], color = 'orange')
+                    plt.axvline(x = self.Lambda[self.Mg2796[i+1]], color = 'orange')
+                    plt.axvline(x = self.Lambda[self.Mg2803[i]], color = 'red')
+                    plt.axvline(x = self.Lambda[self.Mg2803[i + 1]], color = 'red')
+
         if savefig:
             path = str(Path.home()) if path is None else path 
             path += '/' if path[-1] != '/' else ''
             plt.savefig(path+'Spectrum_'+self.qso_name+'.png', dpi=300, bbox_inches='tight')
             print('Figure saved in: {}'.format(path)); plt.clf()
         else:
             plt.show()
@@ -274,49 +284,29 @@
                 saved in the DataFrame. Defaults to None, in which case 'No_Name' is used.
             
         Returns:
             None
         """
 
         #Declare an array to hold the resolution at each wavelength
-        R = np.linspace(self.resolution_range[0], self.resolution_range[1], len(Lambda))
+        if isinstance(self.resolution_range, int) or isinstance(self.resolution_range, float):
+            R = [[self.resolution_range] * len(Lambda)]
+        else:
+            R = np.linspace(self.resolution_range[0], self.resolution_range[1], len(Lambda))
 
         #The MgII function finds the lines
-        Mg2796, Mg2803, EW2796, EW2803, deltaEW2796, deltaEW2803 = MgII(Lambda, y, yC, sig_y, sig_yC, R)
-        Mg2796, Mg2803 = Mg2796.astype(int), Mg2803.astype(int)
-
-        for i in range(0, len(Mg2796), 2):
-            wavelength = (Lambda[Mg2796[i]] + Lambda[Mg2796[i+1]])/2
-            if Lambda[Mg2796[i]] != Lambda[Mg2803[i]]:
-                EW, sigEW = apertureEW(Mg2796[i], Mg2796[i+1], Lambda, y, yC, sig_y, sig_yC)
-                new_row = {'QSO': qso_name, 'Wavelength': wavelength, 'z': wavelength/2796 - 1, 'W': EW, 'deltaW': sigEW}
+        Mg2796, Mg2803, EW2796, EW2803, deltaEW2796, deltaEW2803 = MgII(Lambda, y, yC, sig_y, sig_yC, R, N_sig_1=self.N_sig_1, N_sig_2=self.N_sig_2, 
+            resolution_element=self.resolution_element, rest_wavelength_1=self.rest_wavelength_1, rest_wavelength_2=self.rest_wavelength_2)
+        Mg2796, Mg2803 = np.array(Mg2796), np.array(Mg2803)
+        self.Mg2796, self.Mg2803 = Mg2796.astype(int), Mg2803.astype(int)
+
+        if len(self.Mg2796) != 0:
+            for i in range(0, len(Mg2796) - 1, 2):
+                wavelength = (Lambda[self.Mg2796[i]] + Lambda[self.Mg2796[i+1]])/2
+                new_row = {'QSO': qso_name, 'Wavelength': wavelength, 'z': wavelength/self.rest_wavelength_1 - 1, 'W': EW2796[i], 'deltaW': deltaEW2796[i]}
                 self.df = pd.concat([self.df, pd.DataFrame(new_row, index=[0])], ignore_index=True)
-        
-        #If EW variable was never created, then no line was found!
-        print(); print('No {} line found in "{}" using method="{}" and halfWindow={}'.format(self.line, qso_name, self.method, self.halfWindow)) if 'EW' not in locals() else None
-        if self.save_all and 'EW' not in locals():
-            new_row = {'QSO': qso_name, 'Wavelength': 'None', 'z': 'None', 'W': 'None', 'deltaW': 'None'}
-            self.df = pd.concat([self.df, pd.DataFrame(new_row, index=[0])], ignore_index=True)
-        
+        else: 
+            if self.save_all and 'EW' not in locals():
+                new_row = {'QSO': qso_name, 'Wavelength': 'None', 'z': 'None', 'W': 'None', 'deltaW': 'None'}
+                self.df = pd.concat([self.df, pd.DataFrame(new_row, index=[0])], ignore_index=True)
+            
         return 
-
-    def find_CaIV_absorption(self, Lambda, y, yC, sig_y, sig_yC, z, qso_name=None):
-            """
-            Finds Carbob IV absorption features in the QSO spectrum and adds the line information to the DataFrame,
-            including the Equivalent Width and the corresponding error. 
-
-            Args:
-                Lambda (array-like): Wavelength array.
-                y (array-like): Observed flux array.
-                yC (array-like): Estimated continuum flux array.
-                sig_y (array-like): Observed flux error array.
-                sig_yC (array-like): Estimated continuum flux error array.
-                z (float): The redshift of the QSO associated with the spectrum.
-                qso_name (str, optional): The name of the QSO associated with the spectrum, will be
-                    saved in the DataFrame. Defaults to None, in which case 'No_Name' is used.
-
-            Returns:
-                None
-            """
-
-            print('CaIV finder not yet available, Ezra will write'); return 
-
```

### Comparing `LineDetect-0.1/LineDetect.egg-info/PKG-INFO` & `LineDetect-0.11/LineDetect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LineDetect
-Version: 0.1
+Version: 0.11
 Summary: A pipeline for detecting absorption lines in spectra
 Home-page: https://github.com/Professor-G/LineDetect
 Author: Asif Abbas & Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `LineDetect-0.1/PKG-INFO` & `LineDetect-0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LineDetect
-Version: 0.1
+Version: 0.11
 Summary: A pipeline for detecting absorption lines in spectra
 Home-page: https://github.com/Professor-G/LineDetect
 Author: Asif Abbas & Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `LineDetect-0.1/README.md` & `LineDetect-0.11/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,22 +6,15 @@
 
 # Installation
 
 ```
     $ pip install LineDetect
 ```
 
-
 # [Documentation](https://linedetect.readthedocs.io/en/latest/)
 
 For technical details and an example of how to implement LineDetect, check out our [Documentation](https://linedetect.readthedocs.io/en/latest/).
 
 
-
-# Documentation
-
-For technical details and an example of how to implement LineDetect, check out the Documentation.
-
-
 # How to Contribute?
 
-Want to contribute? Bug detections? Comments? Suggestions? Please email us: asif@nmsu.edu, godines@nmsu.edu
+Want to contribute? Bug detections? Comments? Suggestions? Please email us: asif@nmsu.edu, godines@nmsu.edu
```

### Comparing `LineDetect-0.1/setup.py` & `LineDetect-0.11/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 @author: danielgodinez
 """
 from setuptools import setup, find_packages, Extension
 
 setup(
     name="LineDetect",
-    version="0.1",
+    version="0.11",
     author="Asif Abbas & Daniel Godines",
     author_email="danielgodinez123@gmail.com",
     description="A pipeline for detecting absorption lines in spectra",
     license='GPL-3.0',
     url = "https://github.com/Professor-G/LineDetect",
     classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'Intended Audience :: Developers',
 		'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
 		'Programming Language :: Python :: 3',	   
 ],
     packages=find_packages('.'),
-    install_requires = ['numpy', 'progress', 'astropy', 'scipy', 'matplotlib', 'pandas'],
+    install_requires = ['numpy', 'progress', 'astropy', 'scipy', 'matplotlib', 'pandas', 'lmfit'],
     python_requires='>=3.7,<4',
     include_package_data=False,
     test_suite="nose.collector",
 )
```

