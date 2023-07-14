# Comparing `tmp/LTEpy-0.1.0.tar.gz` & `tmp/LTEpy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LTEpy-0.1.0.tar", last modified: Wed Jul 12 22:03:51 2023, max compression
+gzip compressed data, was "LTEpy-1.0.0.tar", last modified: Fri Jul 14 15:20:01 2023, max compression
```

## Comparing `LTEpy-0.1.0.tar` & `LTEpy-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-12 22:03:51.123712 LTEpy-0.1.0/
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-12 22:03:51.121536 LTEpy-0.1.0/LTEpy/
--rw-r--r--   0 calebharada   (501) staff       (20)       21 2023-07-12 16:10:18.000000 LTEpy-0.1.0/LTEpy/__init__.py
--rw-r--r--   0 calebharada   (501) staff       (20)     3242 2023-07-12 16:10:18.000000 LTEpy-0.1.0/LTEpy/atom.py
--rw-r--r--   0 calebharada   (501) staff       (20)     2033 2023-07-12 16:10:18.000000 LTEpy-0.1.0/LTEpy/constants.py
--rw-r--r--   0 calebharada   (501) staff       (20)    10176 2023-07-12 21:34:44.000000 LTEpy-0.1.0/LTEpy/lte.py
--rw-r--r--   0 calebharada   (501) staff       (20)     5311 2023-07-12 16:10:18.000000 LTEpy-0.1.0/LTEpy/plot.py
-drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-12 22:03:51.123021 LTEpy-0.1.0/LTEpy.egg-info/
--rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-07-12 22:03:51.000000 LTEpy-0.1.0/LTEpy.egg-info/PKG-INFO
--rw-r--r--   0 calebharada   (501) staff       (20)      212 2023-07-12 22:03:51.000000 LTEpy-0.1.0/LTEpy.egg-info/SOURCES.txt
--rw-r--r--   0 calebharada   (501) staff       (20)        1 2023-07-12 22:03:51.000000 LTEpy-0.1.0/LTEpy.egg-info/dependency_links.txt
--rw-r--r--   0 calebharada   (501) staff       (20)        6 2023-07-12 22:03:51.000000 LTEpy-0.1.0/LTEpy.egg-info/top_level.txt
--rw-r--r--   0 calebharada   (501) staff       (20)      313 2023-07-12 22:03:51.123430 LTEpy-0.1.0/PKG-INFO
--rw-r--r--   0 calebharada   (501) staff       (20)      560 2023-07-12 18:10:18.000000 LTEpy-0.1.0/README.md
--rw-r--r--   0 calebharada   (501) staff       (20)       38 2023-07-12 22:03:51.123811 LTEpy-0.1.0/setup.cfg
--rw-r--r--   0 calebharada   (501) staff       (20)      875 2023-07-12 17:59:38.000000 LTEpy-0.1.0/setup.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 15:20:01.625787 LTEpy-1.0.0/
+-rw-r--r--   0 calebharada   (501) staff       (20)     1089 2023-07-14 14:07:27.000000 LTEpy-1.0.0/LICENSE
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 15:20:01.622343 LTEpy-1.0.0/LTEpy/
+-rw-r--r--   0 calebharada   (501) staff       (20)       21 2023-07-14 15:16:18.000000 LTEpy-1.0.0/LTEpy/__init__.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     3275 2023-07-14 14:07:27.000000 LTEpy-1.0.0/LTEpy/atom.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     2033 2023-07-12 16:10:18.000000 LTEpy-1.0.0/LTEpy/constants.py
+-rw-r--r--   0 calebharada   (501) staff       (20)    11933 2023-07-14 14:07:27.000000 LTEpy-1.0.0/LTEpy/lte.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     5354 2023-07-14 14:07:27.000000 LTEpy-1.0.0/LTEpy/plot.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 15:20:01.623693 LTEpy-1.0.0/LTEpy.egg-info/
+-rw-r--r--   0 calebharada   (501) staff       (20)      335 2023-07-14 15:20:01.000000 LTEpy-1.0.0/LTEpy.egg-info/PKG-INFO
+-rw-r--r--   0 calebharada   (501) staff       (20)      309 2023-07-14 15:20:01.000000 LTEpy-1.0.0/LTEpy.egg-info/SOURCES.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)        1 2023-07-14 15:20:01.000000 LTEpy-1.0.0/LTEpy.egg-info/dependency_links.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)       12 2023-07-14 15:20:01.000000 LTEpy-1.0.0/LTEpy.egg-info/top_level.txt
+-rw-r--r--   0 calebharada   (501) staff       (20)      335 2023-07-14 15:20:01.625477 LTEpy-1.0.0/PKG-INFO
+-rw-r--r--   0 calebharada   (501) staff       (20)     1199 2023-07-14 15:16:18.000000 LTEpy-1.0.0/README.md
+-rw-r--r--   0 calebharada   (501) staff       (20)       38 2023-07-14 15:20:01.625915 LTEpy-1.0.0/setup.cfg
+-rw-r--r--   0 calebharada   (501) staff       (20)      875 2023-07-12 17:59:38.000000 LTEpy-1.0.0/setup.py
+drwxr-xr-x   0 calebharada   (501) staff       (20)        0 2023-07-14 15:20:01.625019 LTEpy-1.0.0/tests/
+-rw-r--r--   0 calebharada   (501) staff       (20)        0 2023-07-14 14:07:27.000000 LTEpy-1.0.0/tests/__init__.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     2258 2023-07-14 14:07:27.000000 LTEpy-1.0.0/tests/test_atom.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     1159 2023-07-14 14:07:27.000000 LTEpy-1.0.0/tests/test_boltzmann_factor.py
+-rw-r--r--   0 calebharada   (501) staff       (20)     1329 2023-07-14 14:07:27.000000 LTEpy-1.0.0/tests/test_planck.py
```

### Comparing `LTEpy-0.1.0/LTEpy/atom.py` & `LTEpy-1.0.0/LTEpy/atom.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,128 +3,116 @@
 from LTEpy.constants import EVOLT, KBOLTZ
 
 
 class Atom():
     """ Class for storing energy levels and degeneracies for any atom.
     
     Attributes : 
-    levels : NDarray of ints
-        Energy levels
-    energy : NDarray of floats
-        Energy of each energy level, in ergs
-    gdegen : NDarray of ints
-        Degeneracy of each energy level
+        levels (NDarray of ints) energy levels
+        energy (NDarray of floats): Energy of each energy level, in ergs
+        gdegen (NDarray of ints): Degeneracy of each energy level
     """
 
-    def __init__(self, name, gdegen, energy, levels=None):
+    def __init__(self, gdegen, energy, levels=None):
         """ 
-        Parameters
-        ----------
-        name : str
-            name of atom
-        degen : dict
-            degeneracies
-        elevels : dict
-            energy levels
+        Args:
+            gdegen (array): degeneracies.
+            energy (array): energy at each level.
+            levels (array or None): number of each energy level corresponding to gdegen and energy.
         
         """
-        self.name = name
+
+        if np.any(gdegen<=0):
+            raise ValueError(f"All {gdegen=} must be positive.")
         self.gdegen = gdegen
+
+        if np.any(energy>=0):
+            raise ValueError(f"All {energy=} must be negative for bound states.")
         self.energy = energy
 
         if levels is None:
-            levels = np.arange(1,len(gdegen))
+            levels = np.arange(1,len(gdegen)+1)
 
         self.levels = levels
     
     def boltzmann_factor(self, levii, temp):
         """ Calculate the Boltzmann factor for a given energy level.
-        gi
-        Parameters
-        ----------
-        levii : int
-            Energy level, ii. Must be included in levels
-        temp : arraylike
-
+        
+        Args:
+            levii (int): Energy level, ii. Must be included in levels.
+            temp (float): Temperature in Kelvin.
 
-        Returns
-        -------
-        boltzfact : scalar
-            Boltzmann factor, proportional to the probability of being in state ii
 
+        Returns:
+            bfact (float): Boltzmann factor, proportional to the probability of being in state ii.
+        
+        NOTE: Not tested
         """
         ii = list(self.levels).index(levii)
         Eii = self.energy[ii]
 
-        boltzfact = np.exp(-Eii/KBOLTZ/temp)
-        return boltzfact
+        bfact = np.exp(-Eii/KBOLTZ/temp)
+        return bfact
     
     def partition_function(self, temp):
         """ Calculate the partition function, the sum of all the Boltzmann factors,
         using all levels belonging to the atom.
         
-        
+        Args:
+            temp (float): Temperature in Kelvin.
+
+        NOTE: Not tested
         """
         sum = 0
         for lev in self.levels:
             sum += self.boltzmann_factor(lev, temp)
         return sum
 
 
 class Hydrogen(Atom):
-    """ Class for a hydrogen atom, including hydrogen-specific energy level functions.
+    """ Class for hydrogen atoms.
     
     """
 
-    def __init__(self, name='hydrogen', levels=np.arange(1,11)):
+    def __init__(self, levels=np.arange(1,11)):
         """ 
-        Parameters
-        ----------
-        name : str
-            name of atom
-        levels : NDarray of integers
-            Levels at which to calculate energy and degeneracy, 
-            default 1 to 10.
+        Args:
+            levels (NDarray of integers): Levels at which to calculate energy and degeneracy, default 1 to 10.
         
         """
-        self.name = name
         self.levels = levels
         self.gdegen = self.gdegen_at_level(levels)
         self.energy = self.energy_at_level(levels)
 
     def energy_at_level(self, levels):
         """ Calculate the energy at each level of a hydrogen atom.
 
-        Parameters
-        ----------
-        levels : arraylike
-            Energy level(s), n
+        Args: 
+            levels (arraylike of integers): Energy level(s).
 
         Returns
-        -------
-        energy : arraylike
-            Energy of each energy level, in cgs units (ergs)
+            energy (arraylike): Energy at (each) level, in ergs.
+        
+        ..math::
+            E_n = (-13.6\mathrm{eV}) / n^2
 
-        TODO: Use more precise/generic version of this eq. using Z and rydberg const
-        E = -13.6 eV / n^2
+        TODO: Use more precise/generalizable version of this eq. 
         """
+
         energy = -13.6*EVOLT/levels**2
         return energy
     
     def gdegen_at_level(self, levels):
         """ Calculate the degeneracy at each level of a hydrogen atom.
 
-        Parameters
-        ----------
-        level : arraylike
-            Energy level(s), n
+        Args:
+            level (arraylike of integers): Energy level(s)
 
-        Returns
-        -------
-        gdegen : arraylike
-            Degeneracy of each energy level
+        Returns:
+            gdegen (arraylike): Degeneracy of each energy level
         
-        g = 2 n^2
+        .. math::
+            g(n) = 2 n^2
         """
         gdegen = 2*levels**2
         return gdegen
```

### Comparing `LTEpy-0.1.0/LTEpy/constants.py` & `LTEpy-1.0.0/LTEpy/constants.py`

 * *Files identical despite different names*

### Comparing `LTEpy-0.1.0/LTEpy/lte.py` & `LTEpy-1.0.0/LTEpy/lte.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,27 +25,38 @@
     Args:
         temp (float): Temperature in K.
     """
 
     def __init__(self, temp):
 
         super().__init__(temp)
-        self.temp = temp
+
+        if temp > 0:
+            self.temp = temp
+        elif temp == 0:
+            raise ValueError('Temperature must be greater than 0.')
+        else:
+            raise ValueError('Temperature cannot be negative.')
         
 
     def set_temp(self, temp):
         """Set temperature.
 
-        Changes the temperature of this Planck object.
+        Change the temperature of this Planck LTE object.
 
         Args:
             temp (float): Temperature in K.
         """
 
-        self.temp = temp
+        if temp > 0:
+            self.temp = temp
+        elif temp == 0:
+            raise ValueError('Temperature must be greater than 0.')
+        else:
+            raise ValueError('Temperature cannot be negative.')
 
 
     def compute_B_nu(self, nu):
         """Spectral radiance in frequency space.
 
         Calculate the spectral radiance (or specific intensity) :math:`B_\\nu`
         for a given frequency in cgs units.
@@ -196,154 +207,169 @@
 
 
 
 
 
 
 class Maxwell_Boltzmann(_LTE):
-    """ Class for computing the Maxwell Boltzmann distribution for a given particle and temperature
-    
-    """
+    """Maxwell-Boltzmann Distribution.
 
-    def __init__(self, temp, mass):
-        """ Initialize
+    Class for calculating the Maxwell-Boltzmann Distribution for a system
+    in Local Thermodynamic Equilibrium, given a particle mass.
 
-        Parameters
-        ----------
-        temp : scalar
-            Temperature in K
-        mass : scale
-            Particle mass in AMU
+    Args:
+        temp (float): Temperature in K.
+        mass (float): Particle mass in AMU.
+    """
 
-        """
+    def __init__(self, temp, mass):
 
         super().__init__(temp)
-
         self.temp = temp
         self.mass = mass
 
 
     def set_mass(self, mass):
-        """Helper function to set the mass of the particle
+        """Set mass.
 
-        Parameters
-        ----------
-        mass : scalar
-            Particle mass in AMU
-        
+        Change the mass of this Maxwell-Boltzmann LTE object.
+
+        Args:
+            mass (float): Mass in AMU.
         """
 
         self.mass = mass
-
+    
 
     def set_temp(self, temp):
-        """Set the temperature of this Planck object
+        """Set temperature.
 
-        Parameters
-        ----------
-        temp : scalar
-            temperature in Kelvin
-        
+        Change the temperature of this Maxwell-Boltzmann LTE object.
+
+        Args:
+            temp (float): Temperature in K.
         """
 
         self.temp = temp
     
 
     def compute_maxwell_boltzmann(self, speed):
-        """ Calculate the probability density function of a given speed for a particle of given mass
+        """Maxwell-Boltzmann speed distribution.
 
-        Parameters
-        ----------
-        speed : scalar
-            particle speed in cm/s
+        Compute the probabilty density of a particle with a given mass having a given speed.
 
-        
-        f(v) = (m / 2*pi*k*T)^1.5 * 4*pi*v^2 * exp[-m*v^2 / (2*k*T)]
-        
+        .. math::
+            f(v) = \\bigg(\\frac{m}{2 \pi k T}\\bigg)^{3/2} 4 \pi v^2 e^{-m v^2 / 2 k T}
+
+        Args:
+            speed (float or :obj:`np.array`): Speed in cm/s.
+
+        Returns:
+            float or :obj:`np.array`: Probability density s/cm
         """
 
         mass = self.mass * AMU
 
         f_v = 4 * np.pi * speed**2 * (mass / (2 * np.pi * KBOLTZ * self.temp))**1.5 * np.exp(-mass * speed**2 / (2 * KBOLTZ * self.temp))
 
         return f_v
     
     
-    def plot_fv(self, speed_1, speed_2, N_speed=500, lw=1, ax=None, **kwargs):
-        """ Plot specific intensity B_nu between two frequencies
-        
-        Parameters
-        ----------
-        speed_1 : scalar
-            first speed in cm/s
-        speed_2 : scalar
-            second speed in cm/s
-        N_speed : scalar
-            number of speed points to plot
-        lw : scalar
-            line width for plotting
-        ax : matplotlib axis object
-            option to choose which axis to plot on
-        
+    def plot_fv(self, speed_1, speed_2, N_speed=500, lw=1, ax=None, **ax_kwargs):
+        """Plot the Maxwell-Boltzmann Distribution.
+
+        Plot the distributino of particle speeds defined by the Maxwell-Boltzmann
+        Distribution between two speeds.
+
+        Args:
+            speed_1 (float): First speed in cm/s.
+            speed_2 (float): Second speed in cm/s.
+            N_speed (int, optional): Number of speed points to plot. Defaults to 500.
+            lw (int, optional): Plot line width. Defaults to 1.
+            ax (:obj:`matplotlib.pyplot.Axes`, optional): Matplotlib axis for plotting. Defaults to None.
+            **ax_kwargs: Keyword arguments passed to :obj:`matplotlib.pyplot.Axes` object.
+
+        Returns:
+            :obj:`matplotlib.pyplot.Axes`: Matplotlib axis
         """
 
         speeds = np.linspace(speed_1, speed_2, N_speed)  # define speed array
 
         if not ax:
-            fig, ax = plt.subplots()
+            _, ax = plt.subplots()
 
-        ax.plot(speeds, self.compute_maxwell_boltzmann(speeds), lw=lw, **kwargs)
+        ax.plot(speeds, self.compute_maxwell_boltzmann(speeds), lw=lw, **ax_kwargs)
         ax.set_xlabel("Speed (cm s$^{-1}$)")
         ax.set_ylabel("Probability density (s cm$^{-1}$)")
         
-        if not ax:
-            return fig, ax
+        return ax
 
 
 
 class Boltzmann_Factor(_LTE): 
     """ Class for calculating Boltzmann Factor 
     between two energy levels of a given atom.
     
-    TODO: Add subclass, Gibbs factor, that also allows for a mu term.
     """ 
     def __init__(self, temp, atom): # , levjj):
         """ Initialize
 
-        Parameters
-        ----------
-        temp : scalar
-            Temperature in K
-        atom : equations.Atom Object
-            Atom, contains levels, energy levels, and degeneracies.
+        Args:
+            temp (float): Temperature in K
+            atom (:obj:'atom.Atom'): Atom, contains levels, energy levels, and degeneracies.
 
         """
+
+        # check that temperature is positive
+        if temp == 0: 
+            err = f"{temp=} must be > 0 Kelvin."
+            raise ValueError(err)
+        
+        # set attributes
         self.temp = temp
         self.atom = atom
         self._bfact = None
 
     @property
     def bfact(self):
-        """ Calculate probability ratio of probabilities p_i/p_j between energy levels i and j.
-     
+        """ Boltzmann factor
+        
+        Calculate Boltzmann factor for each energy level.
+
+        Returns:
+            _bfact (:obj:`np.array`) : Boltzmann factor
 
-        factor = exp[(-E_i)/kT]
+     
+        .. math::
+            \\beta(n, T) = \exp \\bigg(\\frac{-E_n}{k_B T}\\bigg)
 
         """
         if self._bfact is None:
             atom = self.atom
             bfact = np.zeros_like(atom.levels, dtype=float)
             for ii, lev in enumerate(atom.levels):
                 eng = atom.energy[ii]
                 bfact[ii] = np.float64(np.exp(-(eng)/KBOLTZ/self.temp))
             self._bfact = bfact
         return self._bfact
 
 
     def draw_bfact(self, ax, levmin=None, levmax=None, color=None):
+        """ Draw the Boltzmann factors
+        
+        Plot the Boltzmann factors for each energy level at a fixed temperature, 
+        and return the line handle.
+        
+        Args:
+            levmin (float or None): Lowest level to plot.
+            levman (float or None): Highest level to plot.
+            
+        Returns:
+            :obj:'matplotlib.Line2D.Line': Line handle
+        """
         if levmin is not None:
             iimin = list(self.atom.levels).index[levmin]
         else:
             iimin = 0
         if levmax is not None:
             iimax = list(self.atom.levels).index[levmax]
         else:
@@ -355,14 +381,27 @@
         hh, = ax.plot(xx, yy, '-o', label=label, color=color)
         ax.set_xlabel(plot.LABEL_LEVEL)
         ax.set_ylabel(plot.LABEL_BFACT)
 
         return hh,
 
     def plot_bfact(self, levmin=None, levmax=None,):
+        """ Plot the Boltzmann factor 
+        
+        Plot the Boltzmann factor for each energy level at a fixed temperature.
+
+        Args:
+            levmin (float or None): Lowest level to plot.
+            levman (float or None): Highest level to plot.
+            
+        Returns:
+            :obj:`matplotlib.pyplot.Figure`: Matplotlib figure
+            :obj:'matplotlib.Line2D.Line': Line handle
+        
+        """
 
         fig, ax = plot.figax(xscale='linear')
         hh, = self.draw_bfact(ax, levmin, levmax)
         ax.set_xlabel(plot.LABEL_LEVEL)
         ax.set_ylabel(plot.LABEL_BFACT)
 
         return fig, hh
```

### Comparing `LTEpy-0.1.0/LTEpy/plot.py` & `LTEpy-1.0.0/LTEpy/plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-#import matplotlib as mpl
+import os
 import matplotlib.pyplot as plt
 import numpy as np
 
-
-plt.style.use('../styles/custom.mplstyle')   # avoid dark backgrounds from dark theme vscode
+ROOT_DIR = os.path.dirname(os.path.abspath(__file__))
+plt.style.use(ROOT_DIR + '/sty/custom.mplstyle')   # avoid dark backgrounds from dark theme vscode
 # plt.rcParams['axes.grid'] = True
 # plt.rcParams['grid.alpha'] = 0.15
 # plt.rcParams["mathtext.fontset"] = "cm"
 # plt.rcParams["font.family"] = "serif"
 # plt.rcParams["legend.handlelength"] = 1.5
 # plt.rcParams["lines.solid_capstyle"] = 'round'
```

### Comparing `LTEpy-0.1.0/setup.py` & `LTEpy-1.0.0/setup.py`

 * *Files identical despite different names*

